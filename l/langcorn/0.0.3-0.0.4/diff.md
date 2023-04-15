# Comparing `tmp/langcorn-0.0.3.tar.gz` & `tmp/langcorn-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langcorn-0.0.3.tar", max compression
+gzip compressed data, was "langcorn-0.0.4.tar", max compression
```

## Comparing `langcorn-0.0.3.tar` & `langcorn-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1088 2023-04-14 20:23:21.753494 langcorn-0.0.3/LICENSE
--rw-r--r--   0        0        0     3213 2023-04-14 20:23:21.753494 langcorn-0.0.3/Readme.md
--rw-r--r--   0        0        0       77 2023-04-14 20:23:21.753494 langcorn-0.0.3/langcorn/__init__.py
--rw-r--r--   0        0        0      417 2023-04-14 20:23:21.753494 langcorn-0.0.3/langcorn/__main__.py
--rw-r--r--   0        0        0        0 2023-04-14 20:23:21.753494 langcorn-0.0.3/langcorn/server/__init__.py
--rw-r--r--   0        0        0     2257 2023-04-14 20:23:21.753494 langcorn-0.0.3/langcorn/server/api.py
--rw-r--r--   0        0        0      825 2023-04-14 20:23:21.753494 langcorn-0.0.3/langcorn/server/test_api.py
--rw-r--r--   0        0        0      922 2023-04-14 20:23:21.753494 langcorn-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4195 1970-01-01 00:00:00.000000 langcorn-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-04-15 10:21:27.252307 langcorn-0.0.4/LICENSE
+-rw-r--r--   0        0        0     4011 2023-04-15 10:21:27.252307 langcorn-0.0.4/Readme.md
+-rw-r--r--   0        0        0       77 2023-04-15 10:21:27.252307 langcorn-0.0.4/langcorn/__init__.py
+-rw-r--r--   0        0        0      417 2023-04-15 10:21:27.252307 langcorn-0.0.4/langcorn/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-15 10:21:27.252307 langcorn-0.0.4/langcorn/server/__init__.py
+-rw-r--r--   0        0        0     2267 2023-04-15 10:21:27.252307 langcorn-0.0.4/langcorn/server/api.py
+-rw-r--r--   0        0        0      825 2023-04-15 10:21:27.252307 langcorn-0.0.4/langcorn/server/test_api.py
+-rw-r--r--   0        0        0      944 2023-04-15 10:21:27.252307 langcorn-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4993 1970-01-01 00:00:00.000000 langcorn-0.0.4/PKG-INFO
```

### Comparing `langcorn-0.0.3/LICENSE` & `langcorn-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `langcorn-0.0.3/Readme.md` & `langcorn-0.0.4/Readme.md`

 * *Files 23% similar despite different names*

```diff
@@ -46,26 +46,45 @@
 chain = LLMMathChain(llm=llm, verbose=True)
 ```
 
 Run your LangCorn FastAPI server:
 
 ```shell
 langcorn server examples.ex1:chain
+
+
+[INFO] 2023-04-14 23:28:57.52 | api:create_service:81 | Endpoint: /docs
+[INFO] 2023-04-14 23:28:57.52 | api:create_service:81 | Endpoint: /examples.ex1/run
+INFO:     Started server process [87033]
+INFO:     Waiting for application startup.
+INFO:     Application startup complete.
+INFO:     Uvicorn running on http://127.0.0.1:8718 (Press CTRL+C to quit)
 ```
 
 or as an alternative
 
 ```shell
 python -m langcorn server examples.ex1:chain
+
 ```
 
 Run multiple chains
 
 ```shell
 python -m langcorn server examples.ex1:chain examples.ex2:chain
+
+
+
+[INFO] 2023-04-14 23:28:57.52 | api:create_service:81 | Endpoint: /docs
+[INFO] 2023-04-14 23:28:57.52 | api:create_service:81 | Endpoint: /examples.ex1/run
+[INFO] 2023-04-14 23:28:57.52 | api:create_service:81 | Endpoint: /examples.ex2/run
+INFO:     Started server process [87033]
+INFO:     Waiting for application startup.
+INFO:     Application startup complete.
+INFO:     Uvicorn running on http://127.0.0.1:8718 (Press CTRL+C to quit)
 ```
 
 Import the necessary packages and create your FastAPI app:
 
 ```python
 
 from fastapi import FastAPI
```

### Comparing `langcorn-0.0.3/langcorn/server/api.py` & `langcorn-0.0.4/langcorn/server/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             dependencies=[_authenticate_or_401],
         )
         async def predict_sync(
             request: LangRequest,
         ):
             output = chain.run(request.prompt)
             # add error handling
-            return LangResponse(output=output)
+            return LangResponse(output=output, error="")
 
     @app.get("/ht")
     async def health_check():
         return dict(functions=[*lc_apps])
 
     logger.info("Serving")
     for endpoint in endpoints:
```

### Comparing `langcorn-0.0.3/langcorn/server/test_api.py` & `langcorn-0.0.4/langcorn/server/test_api.py`

 * *Files identical despite different names*

### Comparing `langcorn-0.0.3/pyproject.toml` & `langcorn-0.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langcorn"
-version = "0.0.3"
+version = "0.0.4"
 description = "A Python package creating rest api interface for LangChain"
 authors = ["Alexander Miasoiedov <msoedov@gmail.com>"]
 maintainers = [
     "Alexander Miasoiedov <msoedov@gmail.com>",
 ]
 repository = "https://github.com/msoedov/langcorn"
 license = "MIT"
@@ -27,14 +27,15 @@
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 mypy = "^1.1.1"
 httpx = "^0.23.3"
 pytest = "^7.2.2"
 types-requests = "^2.28.11"
+pre-commit = "^3.2.2"
 
 [tool.ruff]
 line-length = 120
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `langcorn-0.0.3/PKG-INFO` & `langcorn-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langcorn
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python package creating rest api interface for LangChain
 Home-page: https://github.com/msoedov/langcorn
 License: MIT
 Keywords: nlp,langchain,openai,gpt,fastapi
 Author: Alexander Miasoiedov
 Author-email: msoedov@gmail.com
 Maintainer: Alexander Miasoiedov
@@ -72,26 +72,45 @@
 chain = LLMMathChain(llm=llm, verbose=True)
 ```
 
 Run your LangCorn FastAPI server:
 
 ```shell
 langcorn server examples.ex1:chain
+
+
+[INFO] 2023-04-14 23:28:57.52 | api:create_service:81 | Endpoint: /docs
+[INFO] 2023-04-14 23:28:57.52 | api:create_service:81 | Endpoint: /examples.ex1/run
+INFO:     Started server process [87033]
+INFO:     Waiting for application startup.
+INFO:     Application startup complete.
+INFO:     Uvicorn running on http://127.0.0.1:8718 (Press CTRL+C to quit)
 ```
 
 or as an alternative
 
 ```shell
 python -m langcorn server examples.ex1:chain
+
 ```
 
 Run multiple chains
 
 ```shell
 python -m langcorn server examples.ex1:chain examples.ex2:chain
+
+
+
+[INFO] 2023-04-14 23:28:57.52 | api:create_service:81 | Endpoint: /docs
+[INFO] 2023-04-14 23:28:57.52 | api:create_service:81 | Endpoint: /examples.ex1/run
+[INFO] 2023-04-14 23:28:57.52 | api:create_service:81 | Endpoint: /examples.ex2/run
+INFO:     Started server process [87033]
+INFO:     Waiting for application startup.
+INFO:     Application startup complete.
+INFO:     Uvicorn running on http://127.0.0.1:8718 (Press CTRL+C to quit)
 ```
 
 Import the necessary packages and create your FastAPI app:
 
 ```python
 
 from fastapi import FastAPI
```

