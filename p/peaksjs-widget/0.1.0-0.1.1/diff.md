# Comparing `tmp/peaksjs_widget-0.1.0.tar.gz` & `tmp/peaksjs_widget-0.1.1.tar.gz`

## Comparing `peaksjs_widget-0.1.0.tar` & `peaksjs_widget-0.1.1.tar`

### file list

```diff
@@ -1,64 +1,67 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/.coveragerc
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/.eslintignore
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/.eslintrc.js
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/.npmignore
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/.prettierignore
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/.prettierrc
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/MANIFEST.in
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/babel.config.js
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/codecov.yml
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/install.json
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/jest.config.js
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/package.json
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/peaksjs_widget.json
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/pytest.ini
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/readthedocs.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/setup.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/tsconfig.eslint.json
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/tsconfig.json
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/webpack.config.js
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/css/widget.css
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/docs/Makefile
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/docs/environment.yml
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/docs/make.bat
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/docs/source/conf.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/docs/source/develop-install.rst
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/docs/source/index.rst
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/docs/source/installing.rst
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/docs/source/introduction.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/docs/source/_static/helper.js
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/docs/source/examples/index.rst
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/docs/source/examples/introduction.nblink
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/examples/introduction.ipynb
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/peaksjs_widget/__init__.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/peaksjs_widget/_frontend.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/peaksjs_widget/_version.py
--rw-r--r--   0        0        0     9021 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/peaksjs_widget/widget.py
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/peaksjs_widget/labextension/package.json
--rw-r--r--   0        0        0   102446 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/peaksjs_widget/labextension/static/328.d9fe65c100b4dcbbfa98.js
--rw-r--r--   0        0        0    89409 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/peaksjs_widget/labextension/static/338.69191a97db768e419662.js
--rw-r--r--   0        0        0    14424 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/peaksjs_widget/labextension/static/367.bfc59354caf4baff2151.js
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/peaksjs_widget/labextension/static/480.8b1740af9701e944ef3b.js
--rw-r--r--   0        0        0    19823 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/peaksjs_widget/labextension/static/537.215758051d710979d9cd.js
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/peaksjs_widget/labextension/static/568.79131bbd8f289d6200e2.js
--rw-r--r--   0        0        0    58773 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/peaksjs_widget/labextension/static/882.113942f81a9ff27461d8.js
--rw-r--r--   0        0        0     7474 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/peaksjs_widget/labextension/static/remoteEntry.415c909ebb05c6f881e3.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/peaksjs_widget/labextension/static/style.js
--rw-r--r--   0        0        0    11510 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/peaksjs_widget/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/peaksjs_widget/nbextension/extension.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/peaksjs_widget/tests/__init__.py
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/peaksjs_widget/tests/conftest.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/peaksjs_widget/tests/test_example.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/peaksjs_widget/tests/test_nbextension_path.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/src/extension.ts
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/src/index.ts
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/src/plugin.ts
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/src/version.ts
--rw-r--r--   0        0        0    18758 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/src/widget.ts
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/src/__tests__/index.spec.ts
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/src/__tests__/utils.ts
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/.gitignore
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/README.md
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6533 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/.coveragerc
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/.eslintignore
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/.eslintrc.js
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/.npmignore
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/.prettierignore
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/.prettierrc
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/MANIFEST.in
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/babel.config.js
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/codecov.yml
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/install.json
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/jest.config.js
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/package.json
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/peaksjs_widget.json
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/pytest.ini
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/readthedocs.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/setup.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/tsconfig.eslint.json
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/tsconfig.json
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/webpack.config.js
+-rw-r--r--   0        0        0    51071 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/widget-review.png
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/css/widget.css
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/docs/Makefile
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/docs/environment.yml
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/docs/make.bat
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/docs/source/conf.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/docs/source/develop-install.rst
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/docs/source/index.rst
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/docs/source/installing.rst
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/docs/source/introduction.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/docs/source/_static/helper.js
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/docs/source/examples/index.rst
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/docs/source/examples/introduction.nblink
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/examples/introduction.ipynb
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/peaksjs_widget/__init__.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/peaksjs_widget/_frontend.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/peaksjs_widget/_version.py
+-rw-r--r--   0        0        0     9021 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/peaksjs_widget/widget.py
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/peaksjs_widget/labextension/package.json
+-rw-r--r--   0        0        0   102446 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/peaksjs_widget/labextension/static/328.d9fe65c100b4dcbbfa98.js
+-rw-r--r--   0        0        0    89409 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/peaksjs_widget/labextension/static/338.69191a97db768e419662.js
+-rw-r--r--   0        0        0    14424 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/peaksjs_widget/labextension/static/367.ec0c7a47e82bf367aa00.js
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/peaksjs_widget/labextension/static/480.8b1740af9701e944ef3b.js
+-rw-r--r--   0        0        0    19823 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/peaksjs_widget/labextension/static/537.215758051d710979d9cd.js
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/peaksjs_widget/labextension/static/568.79131bbd8f289d6200e2.js
+-rw-r--r--   0        0        0    58773 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/peaksjs_widget/labextension/static/882.113942f81a9ff27461d8.js
+-rw-r--r--   0        0        0     7474 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/peaksjs_widget/labextension/static/remoteEntry.aec976a06d0c424b3978.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/peaksjs_widget/labextension/static/style.js
+-rw-r--r--   0        0        0    11510 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/peaksjs_widget/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/peaksjs_widget/nbextension/extension.js
+-rw-r--r--   0        0        0   286219 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/peaksjs_widget/nbextension/index.js
+-rw-r--r--   0        0        0  1022755 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/peaksjs_widget/nbextension/index.js.map
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/peaksjs_widget/tests/__init__.py
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/peaksjs_widget/tests/conftest.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/peaksjs_widget/tests/test_example.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/peaksjs_widget/tests/test_nbextension_path.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/src/extension.ts
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/src/index.ts
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/src/plugin.ts
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/src/version.ts
+-rw-r--r--   0        0        0    18758 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/src/widget.ts
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/src/__tests__/index.spec.ts
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/src/__tests__/utils.ts
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/README.md
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6685 2020-02-02 00:00:00.000000 peaksjs_widget-0.1.1/PKG-INFO
```

### Comparing `peaksjs_widget-0.1.0/.eslintrc.js` & `peaksjs_widget-0.1.1/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `peaksjs_widget-0.1.0/MANIFEST.in` & `peaksjs_widget-0.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `peaksjs_widget-0.1.0/package.json` & `peaksjs_widget-0.1.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "'0.1.1'"}*

```diff
@@ -92,9 +92,9 @@
         "test": "jest",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.1.1"
 }
```

### Comparing `peaksjs_widget-0.1.0/tsconfig.json` & `peaksjs_widget-0.1.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `peaksjs_widget-0.1.0/webpack.config.js` & `peaksjs_widget-0.1.1/webpack.config.js`

 * *Files identical despite different names*

### Comparing `peaksjs_widget-0.1.0/docs/Makefile` & `peaksjs_widget-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `peaksjs_widget-0.1.0/docs/make.bat` & `peaksjs_widget-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `peaksjs_widget-0.1.0/docs/source/conf.py` & `peaksjs_widget-0.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `peaksjs_widget-0.1.0/docs/source/develop-install.rst` & `peaksjs_widget-0.1.1/docs/source/develop-install.rst`

 * *Files identical despite different names*

### Comparing `peaksjs_widget-0.1.0/docs/source/index.rst` & `peaksjs_widget-0.1.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `peaksjs_widget-0.1.0/docs/source/installing.rst` & `peaksjs_widget-0.1.1/docs/source/installing.rst`

 * *Files identical despite different names*

### Comparing `peaksjs_widget-0.1.0/examples/introduction.ipynb` & `peaksjs_widget-0.1.1/examples/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `peaksjs_widget-0.1.0/peaksjs_widget/__init__.py` & `peaksjs_widget-0.1.1/peaksjs_widget/__init__.py`

 * *Files identical despite different names*

### Comparing `peaksjs_widget-0.1.0/peaksjs_widget/widget.py` & `peaksjs_widget-0.1.1/peaksjs_widget/widget.py`

 * *Files identical despite different names*

### Comparing `peaksjs_widget-0.1.0/peaksjs_widget/labextension/package.json` & `peaksjs_widget-0.1.1/peaksjs_widget/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9677734375%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.aec976a06d0c424b3978.js'}}",*

 * * "'version'": "'0.1.1'"}*

```diff
@@ -51,15 +51,15 @@
         "dist/*.js",
         "css/*.css"
     ],
     "homepage": "https://github.com/ktonal/peaksjs-widget",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.415c909ebb05c6f881e3.js"
+            "load": "static/remoteEntry.aec976a06d0c424b3978.js"
         },
         "extension": "lib/plugin",
         "outputDir": "peaksjs_widget/labextension/",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -96,9 +96,9 @@
         "test": "jest",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.1.1"
 }
```

### Comparing `peaksjs_widget-0.1.0/peaksjs_widget/labextension/static/328.d9fe65c100b4dcbbfa98.js` & `peaksjs_widget-0.1.1/peaksjs_widget/labextension/static/328.d9fe65c100b4dcbbfa98.js`

 * *Files identical despite different names*

### Comparing `peaksjs_widget-0.1.0/peaksjs_widget/labextension/static/338.69191a97db768e419662.js` & `peaksjs_widget-0.1.1/peaksjs_widget/labextension/static/338.69191a97db768e419662.js`

 * *Files identical despite different names*

### Comparing `peaksjs_widget-0.1.0/peaksjs_widget/labextension/static/367.bfc59354caf4baff2151.js` & `peaksjs_widget-0.1.1/peaksjs_widget/labextension/static/367.ec0c7a47e82bf367aa00.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -509,11 +509,11 @@
                         i = r
                     }
                 }
             }
         },
         147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"peaksjs-widget","version":"0.1.0","description":"ipywidget to interact with audio waveforms through peaks.js","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/ktonal/peaksjs-widget","bugs":{"url":"https://github.com/ktonal/peaksjs-widget/issues"},"license":"BSD-3-Clause","author":{"name":"AntoineDaurat","email":"ktonalberlin@gmail.com"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/ktonal/peaksjs-widget"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf peaksjs_widget/labextension","clean:nbextension":"rimraf peaksjs_widget/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^6","@jupyter-widgets/controls":"^5","underscore":"^1.13.6","konva":"^8.3.10","peaks.js":"^2.0.2","waveform-data":">= 4.3.0 < 5"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"peaksjs_widget/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"peaksjs-widget","version":"0.1.1","description":"ipywidget to interact with audio waveforms through peaks.js","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/ktonal/peaksjs-widget","bugs":{"url":"https://github.com/ktonal/peaksjs-widget/issues"},"license":"BSD-3-Clause","author":{"name":"AntoineDaurat","email":"ktonalberlin@gmail.com"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/ktonal/peaksjs-widget"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf peaksjs_widget/labextension","clean:nbextension":"rimraf peaksjs_widget/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^6","@jupyter-widgets/controls":"^5","underscore":"^1.13.6","konva":"^8.3.10","peaks.js":"^2.0.2","waveform-data":">= 4.3.0 < 5"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"peaksjs_widget/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `peaksjs_widget-0.1.0/peaksjs_widget/labextension/static/480.8b1740af9701e944ef3b.js` & `peaksjs_widget-0.1.1/peaksjs_widget/labextension/static/480.8b1740af9701e944ef3b.js`

 * *Files identical despite different names*

### Comparing `peaksjs_widget-0.1.0/peaksjs_widget/labextension/static/537.215758051d710979d9cd.js` & `peaksjs_widget-0.1.1/peaksjs_widget/labextension/static/537.215758051d710979d9cd.js`

 * *Files identical despite different names*

### Comparing `peaksjs_widget-0.1.0/peaksjs_widget/labextension/static/568.79131bbd8f289d6200e2.js` & `peaksjs_widget-0.1.1/peaksjs_widget/labextension/static/568.79131bbd8f289d6200e2.js`

 * *Files identical despite different names*

### Comparing `peaksjs_widget-0.1.0/peaksjs_widget/labextension/static/882.113942f81a9ff27461d8.js` & `peaksjs_widget-0.1.1/peaksjs_widget/labextension/static/882.113942f81a9ff27461d8.js`

 * *Files identical despite different names*

### Comparing `peaksjs_widget-0.1.0/peaksjs_widget/labextension/static/remoteEntry.415c909ebb05c6f881e3.js` & `peaksjs_widget-0.1.1/peaksjs_widget/labextension/static/remoteEntry.aec976a06d0c424b3978.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, s, l, u, d, f, c, p, h, v, b, g, m = {
+    var e, r, t, n, a, o, i, s, l, d, u, f, c, p, h, v, b, g, m = {
             303: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(367), t.e(568)]).then((() => () => t(568))),
                         "./extension": () => Promise.all([t.e(367), t.e(480)]).then((() => () => t(480)))
                     },
                     a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -45,24 +45,24 @@
             enumerable: !0,
             get: r[t]
         })
     }, y.f = {}, y.e = e => Promise.all(Object.keys(y.f).reduce(((r, t) => (y.f[t](e, r), r)), [])), y.u = e => e + "." + {
         219: "5232dd76676b5cc17f72",
         328: "d9fe65c100b4dcbbfa98",
         338: "69191a97db768e419662",
-        367: "bfc59354caf4baff2151",
+        367: "ec0c7a47e82bf367aa00",
         480: "8b1740af9701e944ef3b",
         537: "215758051d710979d9cd",
         568: "79131bbd8f289d6200e2",
         882: "113942f81a9ff27461d8"
     } [e] + ".js?v=" + {
         219: "5232dd76676b5cc17f72",
         328: "d9fe65c100b4dcbbfa98",
         338: "69191a97db768e419662",
-        367: "bfc59354caf4baff2151",
+        367: "ec0c7a47e82bf367aa00",
         480: "8b1740af9701e944ef3b",
         537: "215758051d710979d9cd",
         568: "79131bbd8f289d6200e2",
         882: "113942f81a9ff27461d8"
     } [e], y.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
@@ -71,18 +71,18 @@
             if ("object" == typeof window) return window
         }
     }(), y.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "peaksjs-widget:", y.l = (t, n, a, o) => {
         if (e[t]) e[t].push(n);
         else {
             var i, s;
             if (void 0 !== a)
-                for (var l = document.getElementsByTagName("script"), u = 0; u < l.length; u++) {
-                    var d = l[u];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + a) {
-                        i = d;
+                for (var l = document.getElementsByTagName("script"), d = 0; d < l.length; d++) {
+                    var u = l[d];
+                    if (u.getAttribute("src") == t || u.getAttribute("data-webpack") == r + a) {
+                        i = u;
                         break
                     }
                 }
             i || (s = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, y.nc && i.setAttribute("nonce", y.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
             var f = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(c);
                     var a = e[t];
@@ -118,15 +118,15 @@
                         (!s || !s.loaded && (!n != !s.eager ? n : i > s.from)) && (a[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (s("konva", "8.4.3", (() => Promise.all([y.e(328), y.e(882)]).then((() => () => y(882))))), s("peaks.js", "2.1.0", (() => Promise.all([y.e(328), y.e(338), y.e(219)]).then((() => () => y(338))))), s("peaksjs-widget", "0.1.0", (() => Promise.all([y.e(367), y.e(568)]).then((() => () => y(568))))), s("waveform-data", "4.3.0", (() => y.e(537).then((() => () => y(537)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (s("konva", "8.4.3", (() => Promise.all([y.e(328), y.e(882)]).then((() => () => y(882))))), s("peaks.js", "2.1.0", (() => Promise.all([y.e(328), y.e(338), y.e(219)]).then((() => () => y(338))))), s("peaksjs-widget", "0.1.1", (() => Promise.all([y.e(367), y.e(568)]).then((() => () => y(568))))), s("waveform-data", "4.3.0", (() => y.e(537).then((() => () => y(537)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         y.g.importScripts && (e = y.g.location + "");
         var r = y.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -175,31 +175,31 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 a = n < 0;
             a && (n = -n - 1);
             for (var i = 0, s = 1, l = !0;; s++, i++) {
-                var u, d, f = s < e.length ? (typeof e[s])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(u = r[i]))[0])) return !l || ("u" == f ? s > n && !a : "" == f != a);
-                if ("u" == d) {
+                var d, u, f = s < e.length ? (typeof e[s])[0] : "";
+                if (i >= r.length || "o" == (u = (typeof(d = r[i]))[0])) return !l || ("u" == f ? s > n && !a : "" == f != a);
+                if ("u" == u) {
                     if (!l || "u" != f) return !1
                 } else if (l)
-                    if (f == d)
+                    if (f == u)
                         if (s <= n) {
-                            if (u != e[s]) return !1
+                            if (d != e[s]) return !1
                         } else {
-                            if (a ? u > e[s] : u < e[s]) return !1;
-                            u != e[s] && (l = !1)
+                            if (a ? d > e[s] : d < e[s]) return !1;
+                            d != e[s] && (l = !1)
                         }
                 else if ("s" != f && "n" != f) {
                     if (a || s <= n) return !1;
                     l = !1, s--
                 } else {
-                    if (s <= n || d < f != a) return !1;
+                    if (s <= n || u < f != a) return !1;
                     l = !1
                 } else "s" != f && "n" != f && (l = !1, s--)
             }
         }
         var c = [],
             p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
@@ -210,25 +210,25 @@
     }, i = (e, r) => {
         var t = y.S[e];
         if (!t || !y.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, s = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", u = (e, r, t, n) => {
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", d = (e, r, t, n) => {
         var a = s(e, t);
         return o(n, a) || "undefined" != typeof console && console.warn && console.warn(l(e, t, a, n)), f(e[t][a])
-    }, d = (e, r, t) => {
+    }, u = (e, r, t) => {
         var a = e[r];
         return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
     }, f = e => (e.loaded = 1, e.get()), p = (c = e => function(r, t, n, a) {
         var o = y.I(r);
         return o && o.then ? o.then(e.bind(e, r, y.S[r], t, n, a)) : e(r, y.S[r], t, n, a)
-    })(((e, r, t, n) => (i(e, t), u(r, 0, t, n)))), h = c(((e, r, t, n, a) => {
-        var o = r && y.o(r, t) && d(r, t, n);
+    })(((e, r, t, n) => (i(e, t), d(r, 0, t, n)))), h = c(((e, r, t, n, a) => {
+        var o = r && y.o(r, t) && u(r, t, n);
         return o ? f(o) : a()
     })), v = {}, b = {
         600: () => h("default", "konva", [1, 8, 3, 10], (() => Promise.all([y.e(328), y.e(882)]).then((() => () => y(882))))),
         985: () => p("default", "@jupyter-widgets/base", [1, 6]),
         989: () => h("default", "peaks.js", [1, 2, 0, 2], (() => Promise.all([y.e(328), y.e(338), y.e(219)]).then((() => () => y(338))))),
         219: () => h("default", "waveform-data", [, [-1, 5],
             [0, 4, 3, 0], 2
```

### Comparing `peaksjs_widget-0.1.0/peaksjs_widget/labextension/static/third-party-licenses.json` & `peaksjs_widget-0.1.1/peaksjs_widget/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `peaksjs_widget-0.1.0/peaksjs_widget/tests/conftest.py` & `peaksjs_widget-0.1.1/peaksjs_widget/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `peaksjs_widget-0.1.0/src/extension.ts` & `peaksjs_widget-0.1.1/src/extension.ts`

 * *Files identical despite different names*

### Comparing `peaksjs_widget-0.1.0/src/plugin.ts` & `peaksjs_widget-0.1.1/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `peaksjs_widget-0.1.0/src/version.ts` & `peaksjs_widget-0.1.1/src/version.ts`

 * *Files identical despite different names*

### Comparing `peaksjs_widget-0.1.0/src/widget.ts` & `peaksjs_widget-0.1.1/src/widget.ts`

 * *Files identical despite different names*

### Comparing `peaksjs_widget-0.1.0/src/__tests__/index.spec.ts` & `peaksjs_widget-0.1.1/src/__tests__/index.spec.ts`

 * *Files identical despite different names*

### Comparing `peaksjs_widget-0.1.0/src/__tests__/utils.ts` & `peaksjs_widget-0.1.1/src/__tests__/utils.ts`

 * *Files identical despite different names*

### Comparing `peaksjs_widget-0.1.0/.gitignore` & `peaksjs_widget-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `peaksjs_widget-0.1.0/LICENSE.txt` & `peaksjs_widget-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `peaksjs_widget-0.1.0/README.md` & `peaksjs_widget-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 
 # peaksjs-widget
 
 [![Build Status](https://travis-ci.org/ktonal/peaksjs-widget.svg?branch=master)](https://travis-ci.org/ktonal/peaksjs_widget)
 [![codecov](https://codecov.io/gh/ktonal/peaksjs-widget/branch/master/graph/badge.svg)](https://codecov.io/gh/ktonal/peaksjs-widget)
 
-
 ipywidget to interact with audio waveforms through peaks.js
 
+![preview](widget-review.png)
+
 ## Installation
 
 You can install using `pip`:
 
-```bash
+```shell script
 pip install peaksjs_widget
 ```
 
 If you are using Jupyter Notebook 5.2 or earlier, you may also need to enable
 the nbextension:
-```bash
+```shell script
 jupyter nbextension enable --py [--sys-prefix|--user|--system] peaksjs_widget
 ```
 
 ## Shortcuts
 
 you can interact with the waveform/widgets with following shortcuts:
 
@@ -44,21 +45,21 @@
     * `Ctrl + alt + click` on a point: edit point's label
 
 you can also drag points and segments' boundaries with the mouse to edit their position
 
 ## Development Installation
 
 Create a dev environment:
-```bash
+```shell script
 conda create -n peaksjs_widget-dev -c conda-forge nodejs yarn python jupyterlab
 conda activate peaksjs_widget-dev
 ```
 
 Install the python. This will also build the TS package.
-```bash
+```shell script
 pip install -e ".[test, examples]"
 ```
 
 When developing your extensions, you need to manually enable your extensions with the
 notebook / lab frontend. For lab, this is done by the command:
 
 ```
@@ -79,15 +80,15 @@
 of those flags here.
 
 ### How to see your changes
 #### Typescript:
 If you use JupyterLab to develop then you can watch the source directory and run JupyterLab at the same time in different
 terminals to watch for changes in the extension's source and automatically rebuild the widget.
 
-```bash
+```shell script
 # Watch the source directory in one terminal, automatically rebuilding when needed
 yarn run watch
 # Run JupyterLab in another terminal
 jupyter lab
 ```
 
 After a change wait for the build to finish and then refresh your browser and the changes should take effect.
@@ -96,19 +97,24 @@
 If you make a change to the python code then you will need to restart the notebook kernel to have it take effect.
 
 ## Updating the version
 
 To update the version, install tbump and use it to bump the version.
 By default it will also create a tag.
 
-```bash
+```shell script
 pip install tbump
 tbump <new-version>
 ```
 
 ## Publish the package
-
-```bash
+on npm
+````shell script
+npm login 
+npm publish
+````
+on pypi
+```shell script
 rm -rf dist/
 pyproject-build .
-twine upload dist/* -u k-tonal
+twine upload dist/peaksjs* -u k-tonal
 ```
```

### Comparing `peaksjs_widget-0.1.0/pyproject.toml` & `peaksjs_widget-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "ipywidgets>=7.0.0",
     "pydub",
     "numpy",
 ]
-version = "0.1.0"
+version = "0.1.1"
 
 [project.optional-dependencies]
 docs = [
     "jupyter_sphinx",
     "nbsphinx",
     "nbsphinx-link",
     "pypandoc",
@@ -57,15 +57,15 @@
 ]
 
 [project.urls]
 Homepage = "https://github.com/ktonal/peaksjs-widget"
 
 [tool.hatch.build]
 artifacts = [
-#    "peaksjs_widget/nbextension/index.*",
+    "peaksjs_widget/nbextension/index.*",
     "peaksjs_widget/labextension/*.tgz",
     "peaksjs_widget/labextension",
 ]
 
 [tool.hatch.build.targets.wheel.shared-data]
 "peaksjs_widget/nbextension" = "share/jupyter/nbextensions/peaksjs_widget"
 "peaksjs_widget/labextension" = "share/jupyter/labextensions/peaksjs_widget"
@@ -100,15 +100,15 @@
 version_template = "version = \"{major}.{minor}.{patch}\""
 
 [[tool.tbump.file]]
 src = "peaksjs_widget/_version.py"
 version_template = "version_info = ({major}, {minor}, {patch})"
 
 [tool.tbump.version]
-current = "0.1.0"
+current = "0.1.1"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `peaksjs_widget-0.1.0/PKG-INFO` & `peaksjs_widget-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peaksjs_widget
-Version: 0.1.0
+Version: 0.1.1
 Summary: ipywidget to interact with audio waveforms through peaks.js
 Project-URL: Homepage, https://github.com/ktonal/peaksjs-widget
 Author-email: AntoineDaurat <ktonalberlin@gmail.com>
 License: Copyright (c) 2023 AntoineDaurat
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
@@ -65,28 +65,29 @@
 
 
 # peaksjs-widget
 
 [![Build Status](https://travis-ci.org/ktonal/peaksjs-widget.svg?branch=master)](https://travis-ci.org/ktonal/peaksjs_widget)
 [![codecov](https://codecov.io/gh/ktonal/peaksjs-widget/branch/master/graph/badge.svg)](https://codecov.io/gh/ktonal/peaksjs-widget)
 
-
 ipywidget to interact with audio waveforms through peaks.js
 
+![preview](widget-review.png)
+
 ## Installation
 
 You can install using `pip`:
 
-```bash
+```shell script
 pip install peaksjs_widget
 ```
 
 If you are using Jupyter Notebook 5.2 or earlier, you may also need to enable
 the nbextension:
-```bash
+```shell script
 jupyter nbextension enable --py [--sys-prefix|--user|--system] peaksjs_widget
 ```
 
 ## Shortcuts
 
 you can interact with the waveform/widgets with following shortcuts:
 
@@ -109,21 +110,21 @@
     * `Ctrl + alt + click` on a point: edit point's label
 
 you can also drag points and segments' boundaries with the mouse to edit their position
 
 ## Development Installation
 
 Create a dev environment:
-```bash
+```shell script
 conda create -n peaksjs_widget-dev -c conda-forge nodejs yarn python jupyterlab
 conda activate peaksjs_widget-dev
 ```
 
 Install the python. This will also build the TS package.
-```bash
+```shell script
 pip install -e ".[test, examples]"
 ```
 
 When developing your extensions, you need to manually enable your extensions with the
 notebook / lab frontend. For lab, this is done by the command:
 
 ```
@@ -144,15 +145,15 @@
 of those flags here.
 
 ### How to see your changes
 #### Typescript:
 If you use JupyterLab to develop then you can watch the source directory and run JupyterLab at the same time in different
 terminals to watch for changes in the extension's source and automatically rebuild the widget.
 
-```bash
+```shell script
 # Watch the source directory in one terminal, automatically rebuilding when needed
 yarn run watch
 # Run JupyterLab in another terminal
 jupyter lab
 ```
 
 After a change wait for the build to finish and then refresh your browser and the changes should take effect.
@@ -161,19 +162,24 @@
 If you make a change to the python code then you will need to restart the notebook kernel to have it take effect.
 
 ## Updating the version
 
 To update the version, install tbump and use it to bump the version.
 By default it will also create a tag.
 
-```bash
+```shell script
 pip install tbump
 tbump <new-version>
 ```
 
 ## Publish the package
-
-```bash
+on npm
+````shell script
+npm login 
+npm publish
+````
+on pypi
+```shell script
 rm -rf dist/
 pyproject-build .
-twine upload dist/* -u k-tonal
+twine upload dist/peaksjs* -u k-tonal
 ```
```

