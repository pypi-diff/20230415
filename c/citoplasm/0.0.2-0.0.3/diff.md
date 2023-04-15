# Comparing `tmp/citoplasm-0.0.2.tar.gz` & `tmp/citoplasm-0.0.3.tar.gz`

## Comparing `citoplasm-0.0.2.tar` & `citoplasm-0.0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 citoplasm-0.0.2/mypy.ini
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 citoplasm-0.0.2/requirements.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 citoplasm-0.0.2/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 citoplasm-0.0.2/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 citoplasm-0.0.2/.pytest_cache/README.md
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 citoplasm-0.0.2/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 citoplasm-0.0.2/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 citoplasm-0.0.2/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 citoplasm-0.0.2/citoplasm/__init__.py
--rw-r--r--   0        0        0     5763 2020-02-02 00:00:00.000000 citoplasm-0.0.2/citoplasm/cito.py
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 citoplasm-0.0.2/citoplasm/context.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 citoplasm-0.0.2/citoplasm/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 citoplasm-0.0.2/citoplasm/agent/__init__.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 citoplasm-0.0.2/citoplasm/agent/agent.py
--rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 citoplasm-0.0.2/citoplasm/agent/openai_chat_agent.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 citoplasm-0.0.2/citoplasm/functions/__init__.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 citoplasm-0.0.2/citoplasm/functions/ask.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 citoplasm-0.0.2/citoplasm/functions/chain.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 citoplasm-0.0.2/citoplasm/functions/compare.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 citoplasm-0.0.2/citoplasm/functions/verify.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 citoplasm-0.0.2/citoplasm/tools/__init__.py
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 citoplasm-0.0.2/citoplasm/tools/python.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 citoplasm-0.0.2/citoplasm/tools/search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 citoplasm-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 citoplasm-0.0.2/tests/test_chain.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 citoplasm-0.0.2/tests/test_classify.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 citoplasm-0.0.2/tests/test_qa.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 citoplasm-0.0.2/tests/test_verify.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 citoplasm-0.0.2/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 citoplasm-0.0.2/LICENSE
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 citoplasm-0.0.2/README.md
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 citoplasm-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5080 2020-02-02 00:00:00.000000 citoplasm-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 citoplasm-0.0.3/mypy.ini
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 citoplasm-0.0.3/requirements.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 citoplasm-0.0.3/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 citoplasm-0.0.3/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 citoplasm-0.0.3/.pytest_cache/README.md
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 citoplasm-0.0.3/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 citoplasm-0.0.3/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 citoplasm-0.0.3/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 citoplasm-0.0.3/citoplasm/__init__.py
+-rw-r--r--   0        0        0     5763 2020-02-02 00:00:00.000000 citoplasm-0.0.3/citoplasm/cito.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 citoplasm-0.0.3/citoplasm/context.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 citoplasm-0.0.3/citoplasm/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 citoplasm-0.0.3/citoplasm/agent/__init__.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 citoplasm-0.0.3/citoplasm/agent/agent.py
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 citoplasm-0.0.3/citoplasm/agent/openai_chat_agent.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 citoplasm-0.0.3/citoplasm/functions/__init__.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 citoplasm-0.0.3/citoplasm/functions/ask.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 citoplasm-0.0.3/citoplasm/functions/chain.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 citoplasm-0.0.3/citoplasm/functions/compare.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 citoplasm-0.0.3/citoplasm/functions/verify.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 citoplasm-0.0.3/citoplasm/tools/__init__.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 citoplasm-0.0.3/citoplasm/tools/python.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 citoplasm-0.0.3/citoplasm/tools/search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 citoplasm-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 citoplasm-0.0.3/tests/test_chain.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 citoplasm-0.0.3/tests/test_classify.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 citoplasm-0.0.3/tests/test_qa.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 citoplasm-0.0.3/tests/test_verify.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 citoplasm-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 citoplasm-0.0.3/LICENSE
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 citoplasm-0.0.3/README.md
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 citoplasm-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5080 2020-02-02 00:00:00.000000 citoplasm-0.0.3/PKG-INFO
```

### Comparing `citoplasm-0.0.2/requirements.txt` & `citoplasm-0.0.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.2/.pytest_cache/v/cache/nodeids` & `citoplasm-0.0.3/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.2/citoplasm/cito.py` & `citoplasm-0.0.3/citoplasm/cito.py`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.2/citoplasm/context.py` & `citoplasm-0.0.3/citoplasm/context.py`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.2/citoplasm/agent/openai_chat_agent.py` & `citoplasm-0.0.3/citoplasm/agent/openai_chat_agent.py`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.2/citoplasm/functions/ask.py` & `citoplasm-0.0.3/citoplasm/functions/ask.py`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.2/citoplasm/functions/chain.py` & `citoplasm-0.0.3/citoplasm/functions/chain.py`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.2/citoplasm/functions/compare.py` & `citoplasm-0.0.3/citoplasm/functions/compare.py`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.2/citoplasm/functions/verify.py` & `citoplasm-0.0.3/citoplasm/functions/verify.py`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.2/citoplasm/tools/python.py` & `citoplasm-0.0.3/citoplasm/tools/python.py`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.2/citoplasm/tools/search.py` & `citoplasm-0.0.3/citoplasm/tools/search.py`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.2/tests/test_chain.py` & `citoplasm-0.0.3/tests/test_chain.py`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.2/tests/test_classify.py` & `citoplasm-0.0.3/tests/test_classify.py`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.2/tests/test_qa.py` & `citoplasm-0.0.3/tests/test_qa.py`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.2/tests/test_verify.py` & `citoplasm-0.0.3/tests/test_verify.py`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.2/LICENSE` & `citoplasm-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.2/README.md` & `citoplasm-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `citoplasm-0.0.2/PKG-INFO` & `citoplasm-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citoplasm
-Version: 0.0.2
+Version: 0.0.3
 Summary: CITOplasm is a Python library for writing LLM code in a declarative way.
 Project-URL: Homepage, https://github.com/joshpoll/CITOplasm
 Project-URL: Bug Tracker, https://github.com/joshpoll/CITOplasm/issues
 Author-email: Joshua Maxwell Pollock <jopo@mit.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

