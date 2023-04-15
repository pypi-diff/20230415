# Comparing `tmp/citoplasm-0.0.4.tar.gz` & `tmp/citoplasm-0.0.5.tar.gz`

## Comparing `citoplasm-0.0.4.tar` & `citoplasm-0.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 citoplasm-0.0.4/mypy.ini
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 citoplasm-0.0.4/requirements.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 citoplasm-0.0.4/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 citoplasm-0.0.4/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 citoplasm-0.0.4/.pytest_cache/README.md
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 citoplasm-0.0.4/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 citoplasm-0.0.4/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 citoplasm-0.0.4/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 citoplasm-0.0.4/citoplasm/__init__.py
--rw-r--r--   0        0        0     5763 2020-02-02 00:00:00.000000 citoplasm-0.0.4/citoplasm/cito.py
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 citoplasm-0.0.4/citoplasm/context.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 citoplasm-0.0.4/citoplasm/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 citoplasm-0.0.4/citoplasm/agent/__init__.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 citoplasm-0.0.4/citoplasm/agent/agent.py
--rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 citoplasm-0.0.4/citoplasm/agent/openai_chat_agent.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 citoplasm-0.0.4/citoplasm/functions/__init__.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 citoplasm-0.0.4/citoplasm/functions/ask.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 citoplasm-0.0.4/citoplasm/functions/chain.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 citoplasm-0.0.4/citoplasm/functions/compare.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 citoplasm-0.0.4/citoplasm/functions/verify.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 citoplasm-0.0.4/citoplasm/tools/__init__.py
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 citoplasm-0.0.4/citoplasm/tools/python.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 citoplasm-0.0.4/citoplasm/tools/search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 citoplasm-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 citoplasm-0.0.4/tests/test_chain.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 citoplasm-0.0.4/tests/test_classify.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 citoplasm-0.0.4/tests/test_qa.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 citoplasm-0.0.4/tests/test_verify.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 citoplasm-0.0.4/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 citoplasm-0.0.4/LICENSE
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 citoplasm-0.0.4/README.md
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 citoplasm-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     5080 2020-02-02 00:00:00.000000 citoplasm-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 citoplasm-0.0.5/mypy.ini
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 citoplasm-0.0.5/requirements.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 citoplasm-0.0.5/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 citoplasm-0.0.5/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 citoplasm-0.0.5/.pytest_cache/README.md
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 citoplasm-0.0.5/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 citoplasm-0.0.5/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 citoplasm-0.0.5/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 citoplasm-0.0.5/citoplasm/__init__.py
+-rw-r--r--   0        0        0     5763 2020-02-02 00:00:00.000000 citoplasm-0.0.5/citoplasm/cito.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 citoplasm-0.0.5/citoplasm/context.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 citoplasm-0.0.5/citoplasm/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 citoplasm-0.0.5/citoplasm/agent/__init__.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 citoplasm-0.0.5/citoplasm/agent/agent.py
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 citoplasm-0.0.5/citoplasm/agent/openai_chat_agent.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 citoplasm-0.0.5/citoplasm/functions/__init__.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 citoplasm-0.0.5/citoplasm/functions/ask.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 citoplasm-0.0.5/citoplasm/functions/chain.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 citoplasm-0.0.5/citoplasm/functions/compare.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 citoplasm-0.0.5/citoplasm/functions/verify.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 citoplasm-0.0.5/citoplasm/tools/__init__.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 citoplasm-0.0.5/citoplasm/tools/python.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 citoplasm-0.0.5/citoplasm/tools/search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 citoplasm-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 citoplasm-0.0.5/tests/test_chain.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 citoplasm-0.0.5/tests/test_classify.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 citoplasm-0.0.5/tests/test_qa.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 citoplasm-0.0.5/tests/test_verify.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 citoplasm-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 citoplasm-0.0.5/LICENSE
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 citoplasm-0.0.5/README.md
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 citoplasm-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     7826 2020-02-02 00:00:00.000000 citoplasm-0.0.5/PKG-INFO
```

### Comparing `citoplasm-0.0.4/requirements.txt` & `citoplasm-0.0.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.4/.pytest_cache/v/cache/nodeids` & `citoplasm-0.0.5/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.4/citoplasm/cito.py` & `citoplasm-0.0.5/citoplasm/cito.py`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.4/citoplasm/context.py` & `citoplasm-0.0.5/citoplasm/context.py`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.4/citoplasm/agent/openai_chat_agent.py` & `citoplasm-0.0.5/citoplasm/agent/openai_chat_agent.py`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.4/citoplasm/functions/ask.py` & `citoplasm-0.0.5/citoplasm/functions/ask.py`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.4/citoplasm/functions/chain.py` & `citoplasm-0.0.5/citoplasm/functions/chain.py`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.4/citoplasm/functions/compare.py` & `citoplasm-0.0.5/citoplasm/functions/compare.py`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.4/citoplasm/functions/verify.py` & `citoplasm-0.0.5/citoplasm/functions/verify.py`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.4/citoplasm/tools/python.py` & `citoplasm-0.0.5/citoplasm/tools/python.py`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.4/citoplasm/tools/search.py` & `citoplasm-0.0.5/citoplasm/tools/search.py`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.4/tests/test_chain.py` & `citoplasm-0.0.5/tests/test_chain.py`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.4/tests/test_classify.py` & `citoplasm-0.0.5/tests/test_classify.py`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.4/tests/test_qa.py` & `citoplasm-0.0.5/tests/test_qa.py`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.4/tests/test_verify.py` & `citoplasm-0.0.5/tests/test_verify.py`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.4/LICENSE` & `citoplasm-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.4/README.md` & `citoplasm-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.4/pyproject.toml` & `citoplasm-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,24 @@
 [build-system]
-requires = [
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "citoplasm"
+version = "0.0.5"
+authors = [{ name = "Joshua Maxwell Pollock", email = "jopo@mit.edu" }]
+description = "CITOplasm is a Python library for writing LLM code in a declarative way."
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+  "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
+]
+dependencies = [
   "anyio==3.6.2",
   "attrs==22.2.0",
   "black==23.3.0",
   "certifi==2022.12.7",
   "charset-normalizer==3.1.0",
   "click==8.1.3",
   "contourpy==1.0.7",
@@ -14,15 +29,14 @@
   "executing==1.2.0",
   "Faker==18.3.2",
   "fastapi==0.95.0",
   "filelock==3.10.7",
   "fonttools==4.39.3",
   "fvalues==0.0.3",
   "h11==0.14.0",
-  "hatchling",
   "httpcore==0.16.3",
   "httpx==0.23.3",
   "huggingface-hub==0.13.3",
   "idna==3.4",
   "iniconfig==2.0.0",
   "joblib==1.2.0",
   "kiwisolver==1.4.4",
@@ -83,25 +97,11 @@
   "typing_extensions==4.5.0",
   "tzdata==2023.3",
   "urllib3==1.26.15",
   "uvicorn==0.21.1",
   "wcwidth==0.2.6",
   "websockets==11.0",
 ]
-build-backend = "hatchling.build"
-
-[project]
-name = "citoplasm"
-version = "0.0.4"
-authors = [{ name = "Joshua Maxwell Pollock", email = "jopo@mit.edu" }]
-description = "CITOplasm is a Python library for writing LLM code in a declarative way."
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = [
-  "Programming Language :: Python :: 3",
-  "License :: OSI Approved :: MIT License",
-  "Operating System :: OS Independent",
-]
 
 [project.urls]
 "Homepage" = "https://github.com/joshpoll/CITOplasm"
 "Bug Tracker" = "https://github.com/joshpoll/CITOplasm/issues"
```

