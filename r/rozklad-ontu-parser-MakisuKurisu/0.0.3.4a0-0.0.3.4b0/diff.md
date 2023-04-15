# Comparing `tmp/rozklad_ontu_parser_makisukurisu-0.0.3.4a0.tar.gz` & `tmp/rozklad_ontu_parser_makisukurisu-0.0.3.4b0.tar.gz`

## Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.4a0.tar` & `rozklad_ontu_parser_makisukurisu-0.0.3.4b0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4a0/requirements.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4a0/run_lint.bat
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4a0/run_lint.sh
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4a0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4a0/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4a0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4a0/ontu_parser/__init__.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4a0/ontu_parser/example.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4a0/ontu_parser/classes/__init__.py
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4a0/ontu_parser/classes/base.py
--rw-r--r--   0        0        0    13351 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4a0/ontu_parser/classes/dataclasses.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4a0/ontu_parser/classes/enums.py
--rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4a0/ontu_parser/classes/parser.py
--rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4a0/ontu_parser/classes/sender.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4a0/.gitignore
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4a0/LICENSE
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4a0/pyproject.toml
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4a0/readme.md
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4a0/PKG-INFO
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/requirements.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/run_lint.bat
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/run_lint.sh
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/__init__.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/example.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/__init__.py
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/base.py
+-rw-r--r--   0        0        0    13351 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/dataclasses.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/enums.py
+-rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/parser.py
+-rw-r--r--   0        0        0     7002 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/sender.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/.gitignore
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/LICENSE
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/pyproject.toml
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/readme.md
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 rozklad_ontu_parser_makisukurisu-0.0.3.4b0/PKG-INFO
```

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.4a0/.github/ISSUE_TEMPLATE/feature_request.md` & `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.4a0/.github/workflows/pylint.yml` & `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.4a0/.github/workflows/python-publish.yml` & `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.4a0/ontu_parser/example.py` & `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/example.py`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.4a0/ontu_parser/classes/base.py` & `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/base.py`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.4a0/ontu_parser/classes/dataclasses.py` & `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/dataclasses.py`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.4a0/ontu_parser/classes/enums.py` & `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/enums.py`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.4a0/ontu_parser/classes/parser.py` & `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/parser.py`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.4a0/ontu_parser/classes/sender.py` & `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/ontu_parser/classes/sender.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,19 +184,15 @@
             )
 
         try:
             response: requests.Response = session.request(
                 method=method,
                 url=self.link,
                 cookies=self.cookies.value,
-                data=data,
-                proxies={
-                    "http": "http://127.0.0.1:8888",
-                    "https": "http://127.0.0.1:8888",
-                }
+                data=data
             )
         except Exception as exception:
             raise ValueError(
                 f'could not get response from {self.link}, got exception: {exception}',
                 self.link,
                 exception
             ) from exception
```

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.4a0/LICENSE` & `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/LICENSE`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.4a0/pyproject.toml` & `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "rozklad_ontu_parser_MakisuKurisu"
-version = "0.0.3.4a"
+version = "0.0.3.4b"
 authors = [
   {  name="Pavlo Pohorieltsev", email="667strets@gmail.com"  },
 ]
 description = "Package for parsing data from rozklad.ontu.edu.ua"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.4a0/readme.md` & `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/readme.md`

 * *Files identical despite different names*

### Comparing `rozklad_ontu_parser_makisukurisu-0.0.3.4a0/PKG-INFO` & `rozklad_ontu_parser_makisukurisu-0.0.3.4b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rozklad_ontu_parser_MakisuKurisu
-Version: 0.0.3.4a0
+Version: 0.0.3.4b0
 Summary: Package for parsing data from rozklad.ontu.edu.ua
 Project-URL: Homepage, https://github.com/makisukurisu/rozklad-ontu-parser
 Project-URL: Bug Tracker, https://github.com/makisukurisu/rozklad-ontu-parser/issues
 Author-email: Pavlo Pohorieltsev <667strets@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
```

