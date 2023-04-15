# Comparing `tmp/artemis-common-0.2.5b0.tar.gz` & `tmp/artemis-common-0.3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artemis-common-0.2.5b0.tar", last modified: Fri Apr 14 19:02:11 2023, max compression
+gzip compressed data, was "artemis-common-0.3.0b0.tar", last modified: Sat Apr 15 20:41:51 2023, max compression
```

## Comparing `artemis-common-0.2.5b0.tar` & `artemis-common-0.3.0b0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:02:11.644840 artemis-common-0.2.5b0/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-14 19:02:11.644840 artemis-common-0.2.5b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:02:11.640840 artemis-common-0.2.5b0/artemis_common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:02:11.644840 artemis-common-0.2.5b0/artemis_common/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/clients/async_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/clients/params_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/clients/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:02:11.644840 artemis-common-0.2.5b0/artemis_common/config/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/config/config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/config/pem.key
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/config/uvicorn_disable_logging.json
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/custom_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:02:11.644840 artemis-common-0.2.5b0/artemis_common/models/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/models/bases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:02:11.644840 artemis-common-0.2.5b0/artemis_common/models/dal/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/models/dal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/models/dal/fred.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/models/dal/user_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/models/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/models/model_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:02:11.644840 artemis-common-0.2.5b0/artemis_common/models/server/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/models/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/models/server/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/models/server/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:02:11.644840 artemis-common-0.2.5b0/artemis_common/server/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/server/exception_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:02:11.644840 artemis-common-0.2.5b0/artemis_common/server/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/server/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/server/middlewares/logging_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/server/swagger.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/server/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:02:11.640840 artemis-common-0.2.5b0/artemis_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-14 19:02:11.000000 artemis-common-0.2.5b0/artemis_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-14 19:02:11.000000 artemis-common-0.2.5b0/artemis_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:02:11.000000 artemis-common-0.2.5b0/artemis_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-14 19:02:11.000000 artemis-common-0.2.5b0/artemis_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 19:02:11.000000 artemis-common-0.2.5b0/artemis_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 19:02:11.644840 artemis-common-0.2.5b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 19:02:10.000000 artemis-common-0.2.5b0/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:41:51.512592 artemis-common-0.3.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-15 20:41:51.512592 artemis-common-0.3.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:41:51.508592 artemis-common-0.3.0b0/artemis_common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:41:51.508592 artemis-common-0.3.0b0/artemis_common/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/clients/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/clients/params_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/clients/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:41:51.508592 artemis-common-0.3.0b0/artemis_common/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/config/config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/config/pem.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/config/uvicorn_disable_logging.json
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/custom_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:41:51.508592 artemis-common-0.3.0b0/artemis_common/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/models/bases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:41:51.508592 artemis-common-0.3.0b0/artemis_common/models/dal/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/models/dal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/models/dal/fred.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/models/dal/user_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/models/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/models/model_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:41:51.508592 artemis-common-0.3.0b0/artemis_common/models/server/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/models/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/models/server/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/models/server/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:41:51.508592 artemis-common-0.3.0b0/artemis_common/server/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/server/exception_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:41:51.512592 artemis-common-0.3.0b0/artemis_common/server/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/server/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/server/middlewares/logging_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/server/swagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/artemis_common/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:41:51.508592 artemis-common-0.3.0b0/artemis_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-15 20:41:51.000000 artemis-common-0.3.0b0/artemis_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-15 20:41:51.000000 artemis-common-0.3.0b0/artemis_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 20:41:51.000000 artemis-common-0.3.0b0/artemis_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-15 20:41:51.000000 artemis-common-0.3.0b0/artemis_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-15 20:41:51.000000 artemis-common-0.3.0b0/artemis_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 20:41:51.512592 artemis-common-0.3.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-15 20:41:41.000000 artemis-common-0.3.0b0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-15 20:41:50.000000 artemis-common-0.3.0b0/version
```

### Comparing `artemis-common-0.2.5b0/artemis_common/clients/async_client.py` & `artemis-common-0.3.0b0/artemis_common/clients/async_client.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.5b0/artemis_common/clients/params_model.py` & `artemis-common-0.3.0b0/artemis_common/clients/params_model.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.5b0/artemis_common/config/config.py` & `artemis-common-0.3.0b0/artemis_common/config/config.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.5b0/artemis_common/config/config_loader.py` & `artemis-common-0.3.0b0/artemis_common/config/config_loader.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.5b0/artemis_common/config/uvicorn_disable_logging.json` & `artemis-common-0.3.0b0/artemis_common/config/uvicorn_disable_logging.json`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.5b0/artemis_common/consts.py` & `artemis-common-0.3.0b0/artemis_common/consts.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 ARTEMIS_DAL_API_KEY_NAME = 'x-artemis-dal-api-key'
 
 
 class ArtemisEnvironment(BaseSettings):
     artemis_env: str = 'dev'
     artemis_debug: str = 'False'
+    version: str
+    service: str = Field(..., env='dd_service')
 
 
 artemis_env = ArtemisEnvironment().artemis_env
 is_prod_env = artemis_env == 'prod'
 is_artemis_debug = str_to_bool(ArtemisEnvironment().artemis_debug)
```

### Comparing `artemis-common-0.2.5b0/artemis_common/custom_logging.py` & `artemis-common-0.3.0b0/artemis_common/custom_logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from structlog.processors import CallsiteParameter
 from structlog.types import EventDict
 from structlog.types import Processor
 
 from artemis_common.consts import artemis_env
 from artemis_common.consts import is_artemis_debug
 from artemis_common.consts import is_prod_env
-from artemis_common.logging import RawTCPHandler
+from artemis_common.logging import DatadogLoggingHandler
 from artemis_common.models import LoggingCenterModel
 
 
 def get_log_level(
     is_debug: bool = False,
 ) -> int:
     """
@@ -202,18 +202,15 @@
     stream_handler = logging.StreamHandler()
     stream_handler.setFormatter(formatter)
     root_logger = logging.getLogger()
     root_logger.setLevel(log_level)
     root_logger.addHandler(stream_handler)
 
     if logging_center:
-        tcp_handler = RawTCPHandler(
-            host=logging_center.host,
-            port=logging_center.logs_port,
-        )
+        tcp_handler = DatadogLoggingHandler()
         tcp_handler.setFormatter(formatter)
         root_logger.addHandler(tcp_handler)
 
     _reconfigure_uvicorn_logger()
 
     sys.excepthook = _handle_exception_hook
```

### Comparing `artemis-common-0.2.5b0/artemis_common/exceptions.py` & `artemis-common-0.3.0b0/artemis_common/exceptions.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.5b0/artemis_common/models/bases.py` & `artemis-common-0.3.0b0/artemis_common/models/bases.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.5b0/artemis_common/models/dal/fred.py` & `artemis-common-0.3.0b0/artemis_common/models/dal/fred.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.5b0/artemis_common/models/jwt.py` & `artemis-common-0.3.0b0/artemis_common/models/jwt.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.5b0/artemis_common/models/model_parser.py` & `artemis-common-0.3.0b0/artemis_common/models/model_parser.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.5b0/artemis_common/models/server/response.py` & `artemis-common-0.3.0b0/artemis_common/models/server/response.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.5b0/artemis_common/server/exception_handlers.py` & `artemis-common-0.3.0b0/artemis_common/server/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.5b0/artemis_common/server/middlewares/logging_middleware.py` & `artemis-common-0.3.0b0/artemis_common/server/middlewares/logging_middleware.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.5b0/artemis_common/server/swagger.py` & `artemis-common-0.3.0b0/artemis_common/server/swagger.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.5b0/artemis_common/server/utils.py` & `artemis-common-0.3.0b0/artemis_common/server/utils.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.5b0/artemis_common/token.py` & `artemis-common-0.3.0b0/artemis_common/token.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.5b0/artemis_common.egg-info/SOURCES.txt` & `artemis-common-0.3.0b0/artemis_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.5b0/setup.py` & `artemis-common-0.3.0b0/setup.py`

 * *Files identical despite different names*

