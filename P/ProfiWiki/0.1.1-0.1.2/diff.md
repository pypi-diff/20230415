# Comparing `tmp/profiwiki-0.1.1.tar.gz` & `tmp/profiwiki-0.1.2.tar.gz`

## Comparing `profiwiki-0.1.1.tar` & `profiwiki-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 profiwiki-0.1.1/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 profiwiki-0.1.1/.pydevproject
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 profiwiki-0.1.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 profiwiki-0.1.1/.github/workflows/upload-to-pypi.yml
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 profiwiki-0.1.1/.vscode/settings.json
--rwxr-xr-x   0        0        0      938 2020-02-02 00:00:00.000000 profiwiki-0.1.1/2018/bashit
--rwxr-xr-x   0        0        0     3234 2020-02-02 00:00:00.000000 profiwiki-0.1.1/2018/gencompose
--rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 profiwiki-0.1.1/2018/mw1_27_7
--rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 profiwiki-0.1.1/2018/mw1_30_1
--rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 profiwiki-0.1.1/2018/mw1_31_1
--rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 profiwiki-0.1.1/2018/mw1_33_1
--rwxr-xr-x   0        0        0    24022 2020-02-02 00:00:00.000000 profiwiki-0.1.1/2018/profiwiki-install.sh
--rwxr-xr-x   0        0        0    11669 2020-02-02 00:00:00.000000 profiwiki-0.1.1/2018/testinstall
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 profiwiki-0.1.1/2018/wiki-config.sh
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 profiwiki-0.1.1/2018/image/phpinfo.php
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 profiwiki-0.1.1/2018/image/profiwiki.php
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 profiwiki-0.1.1/profiwiki/__init__.py
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 profiwiki-0.1.1/profiwiki/docker.py
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 profiwiki-0.1.1/profiwiki/patch.py
--rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 profiwiki-0.1.1/profiwiki/profiwiki_cmd.py
--rw-r--r--   0        0        0     9016 2020-02-02 00:00:00.000000 profiwiki-0.1.1/profiwiki/profiwiki_core.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 profiwiki-0.1.1/profiwiki/version.py
--rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 profiwiki-0.1.1/scripts/install
--rwxr-xr-x   0        0        0      217 2020-02-02 00:00:00.000000 profiwiki-0.1.1/scripts/test
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 profiwiki-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 profiwiki-0.1.1/tests/basetest.py
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 profiwiki-0.1.1/tests/test_patch.py
--rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 profiwiki-0.1.1/tests/test_profiwiki.py
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 profiwiki-0.1.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 profiwiki-0.1.1/LICENSE
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 profiwiki-0.1.1/README.md
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 profiwiki-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 profiwiki-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 profiwiki-0.1.2/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 profiwiki-0.1.2/.pydevproject
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 profiwiki-0.1.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 profiwiki-0.1.2/.github/workflows/upload-to-pypi.yml
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 profiwiki-0.1.2/.vscode/settings.json
+-rwxr-xr-x   0        0        0      938 2020-02-02 00:00:00.000000 profiwiki-0.1.2/2018/bashit
+-rwxr-xr-x   0        0        0     3234 2020-02-02 00:00:00.000000 profiwiki-0.1.2/2018/gencompose
+-rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 profiwiki-0.1.2/2018/mw1_27_7
+-rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 profiwiki-0.1.2/2018/mw1_30_1
+-rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 profiwiki-0.1.2/2018/mw1_31_1
+-rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 profiwiki-0.1.2/2018/mw1_33_1
+-rwxr-xr-x   0        0        0    24022 2020-02-02 00:00:00.000000 profiwiki-0.1.2/2018/profiwiki-install.sh
+-rwxr-xr-x   0        0        0    11669 2020-02-02 00:00:00.000000 profiwiki-0.1.2/2018/testinstall
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 profiwiki-0.1.2/2018/wiki-config.sh
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 profiwiki-0.1.2/2018/image/phpinfo.php
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 profiwiki-0.1.2/2018/image/profiwiki.php
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 profiwiki-0.1.2/profiwiki/__init__.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 profiwiki-0.1.2/profiwiki/docker.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 profiwiki-0.1.2/profiwiki/patch.py
+-rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 profiwiki-0.1.2/profiwiki/profiwiki_cmd.py
+-rw-r--r--   0        0        0     9016 2020-02-02 00:00:00.000000 profiwiki-0.1.2/profiwiki/profiwiki_core.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 profiwiki-0.1.2/profiwiki/version.py
+-rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 profiwiki-0.1.2/scripts/install
+-rwxr-xr-x   0        0        0      217 2020-02-02 00:00:00.000000 profiwiki-0.1.2/scripts/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 profiwiki-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 profiwiki-0.1.2/tests/basetest.py
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 profiwiki-0.1.2/tests/test_patch.py
+-rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 profiwiki-0.1.2/tests/test_profiwiki.py
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 profiwiki-0.1.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 profiwiki-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 profiwiki-0.1.2/README.md
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 profiwiki-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 profiwiki-0.1.2/PKG-INFO
```

### Comparing `profiwiki-0.1.1/.github/workflows/build.yml` & `profiwiki-0.1.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.1/.github/workflows/upload-to-pypi.yml` & `profiwiki-0.1.2/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.1/2018/bashit` & `profiwiki-0.1.2/2018/bashit`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.1/2018/gencompose` & `profiwiki-0.1.2/2018/gencompose`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.1/2018/profiwiki-install.sh` & `profiwiki-0.1.2/2018/profiwiki-install.sh`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.1/2018/testinstall` & `profiwiki-0.1.2/2018/testinstall`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.1/profiwiki/docker.py` & `profiwiki-0.1.2/profiwiki/docker.py`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.1/profiwiki/patch.py` & `profiwiki-0.1.2/profiwiki/patch.py`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.1/profiwiki/profiwiki_cmd.py` & `profiwiki-0.1.2/profiwiki/profiwiki_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         parser = ArgumentParser(description=description, formatter_class=RawDescriptionHelpFormatter)
         config.addArgs(parser)
         parser.add_argument("--about", help="show about info [default: %(default)s]", action="store_true")
         parser.add_argument("--all",help="do all necessary steps for a full setup",action="store_true")
         parser.add_argument("--bash",help="bash into container",action="store_true")
         parser.add_argument("--create",action="store_true",help="create the wiki") 
         parser.add_argument("--check",action="store_true",help="check the wiki")  
+        parser.add_argument("--update",action="store_true",help="start the update script -e.g. to fix SMW key")  
         parser.add_argument("--cron",action="store_true",help="start cron service")        
         parser.add_argument("--down", action="store_true", help="shutdown the wiki [default: %(default)s]")
         parser.add_argument("--patch", action="store_true", help="apply LocalSettings.php patches [default: %(default)s]")
         parser.add_argument("--list",action="store_true",help="list the available profi wikis [default: %(default)s]")
         parser.add_argument("-fu","--forceuser",action="store_true",help="force overwrite of wikiuser")
         parser.add_argument("-fa", "--fontawesome",   action="store_true", help="install fontawesome")
         parser.add_argument("-rp", "--randompassword",   action="store_true", help="create random password and create wikiuser while at it")
```

### Comparing `profiwiki-0.1.1/profiwiki/profiwiki_core.py` & `profiwiki-0.1.2/profiwiki/profiwiki_core.py`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.1/profiwiki/version.py` & `profiwiki-0.1.2/profiwiki/version.py`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.1/tests/basetest.py` & `profiwiki-0.1.2/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.1/tests/test_patch.py` & `profiwiki-0.1.2/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.1/tests/test_profiwiki.py` & `profiwiki-0.1.2/tests/test_profiwiki.py`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.1/.gitignore` & `profiwiki-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.1/LICENSE` & `profiwiki-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.1/README.md` & `profiwiki-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.1/pyproject.toml` & `profiwiki-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.1/PKG-INFO` & `profiwiki-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProfiWiki
-Version: 0.1.1
+Version: 0.1.2
 Project-URL: Home, https://github.com/BITPlan/ProfiWiki
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/ProfiWiki
 Project-URL: Source, https://github.com/BITPlan/ProfiWiki
 Author-email: Wolfgang Fahl <wf@bitplan.com>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

