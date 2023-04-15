# Comparing `tmp/databutton_logger-0.9.1.tar.gz` & `tmp/databutton_logger-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databutton_logger-0.9.1.tar", max compression
+gzip compressed data, was "databutton_logger-0.9.2.tar", max compression
```

## Comparing `databutton_logger-0.9.1.tar` & `databutton_logger-0.9.2.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0       77 2022-12-03 22:23:57.059172 databutton_logger-0.9.1/databutton_logger/__init__.py
--rw-r--r--   0        0        0     3751 2022-12-03 22:23:45.235425 databutton_logger-0.9.1/databutton_logger/logger.py
--rw-r--r--   0        0        0     1335 2022-12-03 22:23:45.235425 databutton_logger-0.9.1/databutton_logger/middleware.py
--rw-r--r--   0        0        0      820 2022-12-03 22:23:57.067172 databutton_logger-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 databutton_logger-0.9.1/setup.py
--rw-r--r--   0        0        0      472 1970-01-01 00:00:00.000000 databutton_logger-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0       77 2023-04-15 16:09:06.118775 databutton_logger-0.9.2/databutton_logger/__init__.py
+-rw-r--r--   0        0        0     3021 2023-04-15 16:08:33.162604 databutton_logger-0.9.2/databutton_logger/logger.py
+-rw-r--r--   0        0        0     1335 2023-04-15 16:08:33.162604 databutton_logger-0.9.2/databutton_logger/middleware.py
+-rw-r--r--   0        0        0      838 2023-04-15 16:09:06.126774 databutton_logger-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 databutton_logger-0.9.2/PKG-INFO
```

### Comparing `databutton_logger-0.9.1/databutton_logger/logger.py` & `databutton_logger-0.9.2/databutton_logger/logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,49 @@
 import json
 import logging
 import os
 import re
 import sys
 from functools import partial
+from typing import Optional
 
 from asgi_correlation_id import CorrelationIdMiddleware
 from asgi_correlation_id.context import correlation_id
 from fastapi import FastAPI
 from loguru import logger
 from starlette.middleware.base import BaseHTTPMiddleware
 
 from .middleware import (
     cloud_trace_context,
     http_request_context,
     http_request_middleware_func,
 )
 
 GCP_LABELS_LOG_KEY = "logging.googleapis.com/labels"
+SPAN_ID_PATTERN = re.compile(r"^\w+")
 
 
 class InterceptHandler(logging.Handler):
-    """
-    Default handler from examples in loguru documentaion.
-    See https://loguru.readthedocs.io/en/stable/overview.html#entirely-compatible-with-standard-logging
-    """
-
     def emit(self, record: logging.LogRecord):
-        # Get corresponding Loguru level if it exists
         try:
             level = logger.level(record.levelname).name
         except ValueError:
             level = record.levelno
 
-        # Find caller from where originated the logged message
         frame, depth = logging.currentframe(), 2
         while frame.f_code.co_filename == logging.__file__:
             frame = frame.f_back
             depth += 1
 
         logger.opt(depth=depth, exception=record.exc_info).log(
             level, record.getMessage()
         )
 
 
-def stackdriver_sink(message, project):
-    """
-    Uses google's structured logging to get nice logs in stackdriver.
-    https://cloud.google.com/logging/docs/structured-logging for more info.
-    This guide has also server as inspiration
-    https://dev.to/floflock/enable-feature-rich-logging-for-fastapi-on-google-cloud-logging-j3i
-    """
+def stackdriver_sink(message, project: str):
     record = message.record
     http_request = http_request_context.get()
     labels: dict[str, str] = record.get("extra").get("labels", {})
     log_info = {
         "severity": record["level"].name,
         "message": record["message"],
         "timestamp": record["time"].timestamp(),
@@ -74,42 +63,38 @@
     trace = cloud_trace_context.get()
     if trace is not None:
         split_header = trace.split("/", 1)
 
         trace_id = f"projects/{project}/traces/{split_header[0]}"
 
         header_suffix = split_header[1]
-        span_id = re.findall(r"^\w+", header_suffix)[0]
+        span_id = SPAN_ID_PATTERN.findall(header_suffix)[0]
 
         log_info["logging.googleapis.com/trace"] = trace_id
         log_info["logging.googleapis.com/spanId"] = span_id
     serialized = json.dumps(log_info)
     print(serialized, file=sys.stderr)
 
 
-def setup_logging_fastapi_gcp(app: FastAPI, *, GCP_PROJECT="databutton"):
-    """
-    Sets up logging and tracing for FastAPI based projects.
-    """
+def setup_logging_fastapi_gcp(
+    app: FastAPI, *, GCP_PROJECT: Optional[str] = "databutton"
+):
     app.add_middleware(BaseHTTPMiddleware, dispatch=http_request_middleware_func)
-    # I don't know how to validate nanoids which is what we generate in Caddy
     app.add_middleware(CorrelationIdMiddleware, validator=lambda str: len(str) > 10)
 
     loggers = (
         logging.getLogger(name)
         for name in logging.root.manager.loggerDict
         if name.startswith("uvicorn.")
     )
     for uvicorn_logger in loggers:
         uvicorn_logger.handlers = []
 
-    # change handler for default uvicorn logger
     intercept_handler = InterceptHandler()
     logging.getLogger("uvicorn").handlers = [intercept_handler]
 
     logger.remove()
     sink_for_project = partial(stackdriver_sink, project=GCP_PROJECT)
     logger.add(
         sink_for_project,
-        # serialize=True,
         level=os.environ.get("LOGURU_LEVEL", "INFO"),
     )
```

### Comparing `databutton_logger-0.9.1/databutton_logger/middleware.py` & `databutton_logger-0.9.2/databutton_logger/middleware.py`

 * *Files identical despite different names*

### Comparing `databutton_logger-0.9.1/pyproject.toml` & `databutton_logger-0.9.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "databutton-logger"
-version = "0.9.1"
+version = "0.9.2"
 description = "Logger utilities for databutton"
 authors = ["Databutton"]
 packages = [
   { include = "databutton_logger"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-asgi-correlation-id = "^3.0.1"
+asgi-correlation-id = "^4.1.0"
 fastapi = ">=0.80"
-loguru = "^0.6.0"
+loguru = "^0.7.0"
+httpx = "^0.24.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 black = "^22.8.0"
 isort = "^5.10.1"
 flake8 = "^5.0.4"
 python-semantic-release = "^7.31.4"
```

