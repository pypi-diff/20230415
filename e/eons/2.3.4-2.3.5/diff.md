# Comparing `tmp/eons-2.3.4.tar.gz` & `tmp/eons-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eons-2.3.4.tar", last modified: Fri Apr  7 00:12:49 2023, max compression
+gzip compressed data, was "eons-2.3.5.tar", last modified: Sat Apr 15 21:24:28 2023, max compression
```

## Comparing `eons-2.3.4.tar` & `eons-2.3.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:12:49.618333 eons-2.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-04-07 00:12:49.622333 eons-2.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-04-07 00:12:33.000000 eons-2.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:12:49.610333 eons-2.3.4/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:12:49.614333 eons-2.3.4/pkg/eons/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-07 00:12:41.000000 eons-2.3.4/pkg/eons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    81469 2023-04-07 00:12:41.000000 eons-2.3.4/pkg/eons/eons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:12:49.618333 eons-2.3.4/pkg/eons/resolve/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 00:12:41.000000 eons-2.3.4/pkg/eons/resolve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-07 00:12:20.000000 eons-2.3.4/pkg/eons/resolve/resolve_find_by_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-07 00:12:20.000000 eons-2.3.4/pkg/eons/resolve/resolve_import_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-07 00:12:20.000000 eons-2.3.4/pkg/eons/resolve/resolve_install_from_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-07 00:12:20.000000 eons-2.3.4/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-07 00:12:20.000000 eons-2.3.4/pkg/eons/resolve/resolve_install_with_pip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 00:12:49.614333 eons-2.3.4/pkg/eons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-04-07 00:12:49.000000 eons-2.3.4/pkg/eons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-07 00:12:49.000000 eons-2.3.4/pkg/eons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 00:12:49.000000 eons-2.3.4/pkg/eons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-07 00:12:49.000000 eons-2.3.4/pkg/eons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-07 00:12:49.000000 eons-2.3.4/pkg/eons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-07 00:12:41.000000 eons-2.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-07 00:12:49.622333 eons-2.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:24:28.065014 eons-2.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-04-15 21:24:28.065014 eons-2.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-04-15 21:24:13.000000 eons-2.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:24:28.061014 eons-2.3.5/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:24:28.061014 eons-2.3.5/pkg/eons/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-15 21:24:20.000000 eons-2.3.5/pkg/eons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81676 2023-04-15 21:24:20.000000 eons-2.3.5/pkg/eons/eons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:24:28.065014 eons-2.3.5/pkg/eons/resolve/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 21:24:20.000000 eons-2.3.5/pkg/eons/resolve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-15 21:23:54.000000 eons-2.3.5/pkg/eons/resolve/resolve_find_by_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-15 21:23:54.000000 eons-2.3.5/pkg/eons/resolve/resolve_import_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-15 21:23:54.000000 eons-2.3.5/pkg/eons/resolve/resolve_install_from_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-15 21:23:54.000000 eons-2.3.5/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-15 21:23:54.000000 eons-2.3.5/pkg/eons/resolve/resolve_install_with_pip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:24:28.061014 eons-2.3.5/pkg/eons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-04-15 21:24:28.000000 eons-2.3.5/pkg/eons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-15 21:24:28.000000 eons-2.3.5/pkg/eons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 21:24:28.000000 eons-2.3.5/pkg/eons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-15 21:24:28.000000 eons-2.3.5/pkg/eons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-15 21:24:28.000000 eons-2.3.5/pkg/eons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-15 21:24:20.000000 eons-2.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-15 21:24:28.065014 eons-2.3.5/setup.cfg
```

### Comparing `eons-2.3.4/PKG-INFO` & `eons-2.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.3.4
+Version: 2.3.5
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.3.4/README.md` & `eons-2.3.5/README.md`

 * *Files identical despite different names*

### Comparing `eons-2.3.4/pkg/eons/eons.py` & `eons-2.3.5/pkg/eons/eons.py`

 * *Files 0% similar despite different names*

```diff
@@ -804,38 +804,47 @@
 
 		next = this.next.pop(0)
 		if (not this.ValidateNext(next)):
 			raise InvalidNext(f"Failed to validate {next}")
 		return this.GetExecutor().Execute(next, precursor=this, next=this.next)
 
 
-	# Make functor.
-	# Don't worry about this; logic is abstracted to Function
-	def __call__(this, *args, **kwargs) :
-		logging.debug(f"<---- {this.name} ---->")
+	def WarmUp(this, *args, **kwargs):
 
 		this.args = args
 		this.kwargs = kwargs
-
-		logging.debug(f"{this.name}({this.args}, {this.kwargs})")
-
-		ret = None
-		nextRet = None
+		
 		try:
 			this.PopulatePrecursor()
 			this.Initialize() # nop on call 2+
 			this.PopulateMethods() # Doesn't require Fetch; depends on precursor
 			this.ParseInitialArgs() # Usually where config is read in.
 			this.ValidateStaticArgs() # nop on call 2+
 			this.PopulateNext()
 			this.ValidateArgs()
 			this.ValidateMethods()
+		except Exception as e:
+			if (this.raiseExceptions):
+				raise e
+			else:
+				logging.error(f"ERROR: {e}")
+				util.LogStack()
 
-			this.BeforeFunction()
 
+	# Make functor.
+	# Don't worry about this; logic is abstracted to Function
+	def __call__(this, *args, **kwargs) :
+		logging.debug(f"<---- {this.name} ---->")
+		ret = None
+		nextRet = None
+		try:
+			this.WarmUp(*args, **kwargs)
+			logging.debug(f"{this.name}({this.args}, {this.kwargs})")
+
+			this.BeforeFunction()
 			ret = this.Function()
 
 			if (this.DidFunctionSucceed()):
 					this.result = 1
 					# logging.info(f"{this.name} successful!")
 					nextRet = this.CallNext()
 			elif (this.enableRollback):
```

### Comparing `eons-2.3.4/pkg/eons/resolve/resolve_find_by_fetch.py` & `eons-2.3.5/pkg/eons/resolve/resolve_find_by_fetch.py`

 * *Files identical despite different names*

### Comparing `eons-2.3.4/pkg/eons/resolve/resolve_import_module.py` & `eons-2.3.5/pkg/eons/resolve/resolve_import_module.py`

 * *Files identical despite different names*

### Comparing `eons-2.3.4/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py` & `eons-2.3.5/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py`

 * *Files identical despite different names*

### Comparing `eons-2.3.4/pkg/eons.egg-info/PKG-INFO` & `eons-2.3.5/pkg/eons.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.3.4
+Version: 2.3.5
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.3.4/setup.cfg` & `eons-2.3.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eons
-version = 2.3.4
+version = 2.3.5
 author = Eons
 author_email = support@eons.llc
 description = Eons Python Framework
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/eons-dev/eons.lib
@@ -18,16 +18,16 @@
 
 [options]
 package_dir = 
 	= pkg
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	requests
 	tqdm
+	requests
 	pyyaml
 	jsonpickle
 
 [options.packages.find]
 where = pkg
 
 [egg_info]
```

