# Comparing `tmp/pyexhange_r3ne-0.1.8.tar.gz` & `tmp/pyexhange_r3ne-0.1.9.tar.gz`

## Comparing `pyexhange_r3ne-0.1.8.tar` & `pyexhange_r3ne-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.8/.gitattributes
--rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.8/Run.bat
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.8/config.json.example
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.8/pyexhange.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.8/requirements.txt
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.8/test.py
--rwxr-xr-x   0        0        0       71 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.8/upload.bat
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.8/data/placeholder
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.8/modules/price.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.8/modules/send.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.8/modules/trade.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.8/modules/wallet.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.8/modules/utils/coingecko.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.8/modules/utils/data.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.8/modules/utils/exchanges.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.8/modules/utils/finhub.py
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.8/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.8/LICENCE.rst
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.8/README.md
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.9/.gitattributes
+-rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.9/Run.bat
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.9/compensation.json
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.9/config.json.example
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.9/pyexhange.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.9/requirements.txt
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.9/test.py
+-rwxr-xr-x   0        0        0       71 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.9/upload.bat
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.9/data/placeholder
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.9/modules/price.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.9/modules/send.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.9/modules/trade.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.9/modules/wallet.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.9/modules/utils/coingecko.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.9/modules/utils/data.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.9/modules/utils/exchanges.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.9/modules/utils/finhub.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.9/LICENCE.rst
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.9/README.md
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 pyexhange_r3ne-0.1.9/PKG-INFO
```

### Comparing `pyexhange_r3ne-0.1.8/modules/price.py` & `pyexhange_r3ne-0.1.9/modules/price.py`

 * *Files identical despite different names*

### Comparing `pyexhange_r3ne-0.1.8/modules/send.py` & `pyexhange_r3ne-0.1.9/modules/send.py`

 * *Files identical despite different names*

### Comparing `pyexhange_r3ne-0.1.8/modules/trade.py` & `pyexhange_r3ne-0.1.9/modules/trade.py`

 * *Files identical despite different names*

### Comparing `pyexhange_r3ne-0.1.8/modules/wallet.py` & `pyexhange_r3ne-0.1.9/modules/wallet.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,11 +13,14 @@
 
     user, currency = args
     currency = currency.upper()
     curdata = get_data(currency)
 
     if curdata == None:
         curdata = {"price": 0, "symbol":"CRYPTO"}
-    amount = data.load(user, curdata['symbol'])
+    if currency == "USD":
+        amount = data.load(user, "USD")
+    else:
+        amount = data.load(user, curdata['symbol'])
 
     output = {"status": "success", "amount": amount,"price": curdata['price'] * amount, "currency": curdata['symbol']}
     return output
```

### Comparing `pyexhange_r3ne-0.1.8/modules/utils/data.py` & `pyexhange_r3ne-0.1.9/modules/utils/data.py`

 * *Files identical despite different names*

### Comparing `pyexhange_r3ne-0.1.8/modules/utils/finhub.py` & `pyexhange_r3ne-0.1.9/modules/utils/finhub.py`

 * *Files identical despite different names*

### Comparing `pyexhange_r3ne-0.1.8/.gitignore` & `pyexhange_r3ne-0.1.9/.gitignore`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,162 +1,162 @@
-# Byte-compiled / optimized / DLL files
-__pycache__/
-*.py[cod]
-*$py.class
-
-# C extensions
-*.so
-
-# Distribution / packaging
-.Python
-build/
-develop-eggs/
-dist/
-downloads/
-eggs/
-.eggs/
-lib/
-lib64/
-parts/
-sdist/
-var/
-wheels/
-share/python-wheels/
-*.egg-info/
-.installed.cfg
-*.egg
-MANIFEST
-
-# PyInstaller
-#  Usually these files are written by a python script from a template
-#  before PyInstaller builds the exe, so as to inject date/other infos into it.
-*.manifest
-*.spec
-
-# Installer logs
-pip-log.txt
-pip-delete-this-directory.txt
-
-# Unit test / coverage reports
-htmlcov/
-.tox/
-.nox/
-.coverage
-.coverage.*
-.cache
-nosetests.xml
-coverage.xml
-*.cover
-*.py,cover
-.hypothesis/
-.pytest_cache/
-cover/
-
-# Translations
-*.mo
-*.pot
-
-# Django stuff:
-*.log
-local_settings.py
-db.sqlite3
-db.sqlite3-journal
-
-# Flask stuff:
-instance/
-.webassets-cache
-
-# Scrapy stuff:
-.scrapy
-
-# Sphinx documentation
-docs/_build/
-
-# PyBuilder
-.pybuilder/
-target/
-
-# Jupyter Notebook
-.ipynb_checkpoints
-
-# IPython
-profile_default/
-ipython_config.py
-
-# pyenv
-#   For a library or package, you might want to ignore these files since the code is
-#   intended to run in multiple environments; otherwise, check them in:
-# .python-version
-
-# pipenv
-#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
-#   However, in case of collaboration, if having platform-specific dependencies or dependencies
-#   having no cross-platform support, pipenv may install dependencies that don't work, or not
-#   install all needed dependencies.
-#Pipfile.lock
-
-# poetry
-#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
-#   This is especially recommended for binary packages to ensure reproducibility, and is more
-#   commonly ignored for libraries.
-#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
-#poetry.lock
-
-# pdm
-#   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
-#pdm.lock
-#   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
-#   in version control.
-#   https://pdm.fming.dev/#use-with-ide
-.pdm.toml
-
-# PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
-__pypackages__/
-
-# Celery stuff
-celerybeat-schedule
-celerybeat.pid
-
-# SageMath parsed files
-*.sage.py
-
-# Environments
-.env
-.venv
-env/
-venv/
-ENV/
-env.bak/
-venv.bak/
-
-# Spyder project settings
-.spyderproject
-.spyproject
-
-# Rope project settings
-.ropeproject
-
-# mkdocs documentation
-/site
-
-# mypy
-.mypy_cache/
-.dmypy.json
-dmypy.json
-
-# Pyre type checker
-.pyre/
-
-# pytype static type analyzer
-.pytype/
-
-# Cython debug symbols
-cython_debug/
-
-# PyCharm
-#  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
-#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
-#  and can be added to the global gitignore or merged into this file.  For a more nuclear
-#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
-config.json
-data/*.json
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
+# Distribution / packaging
+.Python
+build/
+develop-eggs/
+dist/
+downloads/
+eggs/
+.eggs/
+lib/
+lib64/
+parts/
+sdist/
+var/
+wheels/
+share/python-wheels/
+*.egg-info/
+.installed.cfg
+*.egg
+MANIFEST
+
+# PyInstaller
+#  Usually these files are written by a python script from a template
+#  before PyInstaller builds the exe, so as to inject date/other infos into it.
+*.manifest
+*.spec
+
+# Installer logs
+pip-log.txt
+pip-delete-this-directory.txt
+
+# Unit test / coverage reports
+htmlcov/
+.tox/
+.nox/
+.coverage
+.coverage.*
+.cache
+nosetests.xml
+coverage.xml
+*.cover
+*.py,cover
+.hypothesis/
+.pytest_cache/
+cover/
+
+# Translations
+*.mo
+*.pot
+
+# Django stuff:
+*.log
+local_settings.py
+db.sqlite3
+db.sqlite3-journal
+
+# Flask stuff:
+instance/
+.webassets-cache
+
+# Scrapy stuff:
+.scrapy
+
+# Sphinx documentation
+docs/_build/
+
+# PyBuilder
+.pybuilder/
+target/
+
+# Jupyter Notebook
+.ipynb_checkpoints
+
+# IPython
+profile_default/
+ipython_config.py
+
+# pyenv
+#   For a library or package, you might want to ignore these files since the code is
+#   intended to run in multiple environments; otherwise, check them in:
+# .python-version
+
+# pipenv
+#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
+#   However, in case of collaboration, if having platform-specific dependencies or dependencies
+#   having no cross-platform support, pipenv may install dependencies that don't work, or not
+#   install all needed dependencies.
+#Pipfile.lock
+
+# poetry
+#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
+#   This is especially recommended for binary packages to ensure reproducibility, and is more
+#   commonly ignored for libraries.
+#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
+#poetry.lock
+
+# pdm
+#   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
+#pdm.lock
+#   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
+#   in version control.
+#   https://pdm.fming.dev/#use-with-ide
+.pdm.toml
+
+# PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
+__pypackages__/
+
+# Celery stuff
+celerybeat-schedule
+celerybeat.pid
+
+# SageMath parsed files
+*.sage.py
+
+# Environments
+.env
+.venv
+env/
+venv/
+ENV/
+env.bak/
+venv.bak/
+
+# Spyder project settings
+.spyderproject
+.spyproject
+
+# Rope project settings
+.ropeproject
+
+# mkdocs documentation
+/site
+
+# mypy
+.mypy_cache/
+.dmypy.json
+dmypy.json
+
+# Pyre type checker
+.pyre/
+
+# pytype static type analyzer
+.pytype/
+
+# Cython debug symbols
+cython_debug/
+
+# PyCharm
+#  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
+#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
+#  and can be added to the global gitignore or merged into this file.  For a more nuclear
+#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
+#.idea/
+config.json
+data/*.json
```

### Comparing `pyexhange_r3ne-0.1.8/LICENCE.rst` & `pyexhange_r3ne-0.1.9/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `pyexhange_r3ne-0.1.8/README.md` & `pyexhange_r3ne-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyexhange_r3ne-0.1.8/pyproject.toml` & `pyexhange_r3ne-0.1.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["hatchling", "finnhub-python"]
+requires = ["hatchling", "finnhub-python", "pycoingecko"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyexhange_r3ne"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="R3ne.net", email="mail@r3ne.net" },
 ]
 description = "Python code that allows users to create and manage their own virtual wallets to get the trading experiense with out real money."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pyexhange_r3ne-0.1.8/PKG-INFO` & `pyexhange_r3ne-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyexhange_r3ne
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python code that allows users to create and manage their own virtual wallets to get the trading experiense with out real money.
 Project-URL: Homepage, https://github.com/JAAKKQ/pyexhange
 Project-URL: Bug Tracker, https://github.com/JAAKKQ/pyexhange/issues
 Author-email: "R3ne.net" <mail@r3ne.net>
 License-File: LICENCE.rst
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

