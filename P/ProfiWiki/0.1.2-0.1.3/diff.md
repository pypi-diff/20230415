# Comparing `tmp/profiwiki-0.1.2.tar.gz` & `tmp/profiwiki-0.1.3.tar.gz`

## Comparing `profiwiki-0.1.2.tar` & `profiwiki-0.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 profiwiki-0.1.2/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 profiwiki-0.1.2/.pydevproject
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 profiwiki-0.1.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 profiwiki-0.1.2/.github/workflows/upload-to-pypi.yml
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 profiwiki-0.1.2/.vscode/settings.json
--rwxr-xr-x   0        0        0      938 2020-02-02 00:00:00.000000 profiwiki-0.1.2/2018/bashit
--rwxr-xr-x   0        0        0     3234 2020-02-02 00:00:00.000000 profiwiki-0.1.2/2018/gencompose
--rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 profiwiki-0.1.2/2018/mw1_27_7
--rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 profiwiki-0.1.2/2018/mw1_30_1
--rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 profiwiki-0.1.2/2018/mw1_31_1
--rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 profiwiki-0.1.2/2018/mw1_33_1
--rwxr-xr-x   0        0        0    24022 2020-02-02 00:00:00.000000 profiwiki-0.1.2/2018/profiwiki-install.sh
--rwxr-xr-x   0        0        0    11669 2020-02-02 00:00:00.000000 profiwiki-0.1.2/2018/testinstall
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 profiwiki-0.1.2/2018/wiki-config.sh
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 profiwiki-0.1.2/2018/image/phpinfo.php
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 profiwiki-0.1.2/2018/image/profiwiki.php
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 profiwiki-0.1.2/profiwiki/__init__.py
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 profiwiki-0.1.2/profiwiki/docker.py
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 profiwiki-0.1.2/profiwiki/patch.py
--rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 profiwiki-0.1.2/profiwiki/profiwiki_cmd.py
--rw-r--r--   0        0        0     9016 2020-02-02 00:00:00.000000 profiwiki-0.1.2/profiwiki/profiwiki_core.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 profiwiki-0.1.2/profiwiki/version.py
--rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 profiwiki-0.1.2/scripts/install
--rwxr-xr-x   0        0        0      217 2020-02-02 00:00:00.000000 profiwiki-0.1.2/scripts/test
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 profiwiki-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 profiwiki-0.1.2/tests/basetest.py
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 profiwiki-0.1.2/tests/test_patch.py
--rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 profiwiki-0.1.2/tests/test_profiwiki.py
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 profiwiki-0.1.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 profiwiki-0.1.2/LICENSE
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 profiwiki-0.1.2/README.md
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 profiwiki-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 profiwiki-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 profiwiki-0.1.3/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 profiwiki-0.1.3/.pydevproject
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 profiwiki-0.1.3/.github/workflows/build.yml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 profiwiki-0.1.3/.github/workflows/upload-to-pypi.yml
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 profiwiki-0.1.3/.vscode/settings.json
+-rwxr-xr-x   0        0        0      938 2020-02-02 00:00:00.000000 profiwiki-0.1.3/2018/bashit
+-rwxr-xr-x   0        0        0     3234 2020-02-02 00:00:00.000000 profiwiki-0.1.3/2018/gencompose
+-rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 profiwiki-0.1.3/2018/mw1_27_7
+-rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 profiwiki-0.1.3/2018/mw1_30_1
+-rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 profiwiki-0.1.3/2018/mw1_31_1
+-rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 profiwiki-0.1.3/2018/mw1_33_1
+-rwxr-xr-x   0        0        0    24022 2020-02-02 00:00:00.000000 profiwiki-0.1.3/2018/profiwiki-install.sh
+-rwxr-xr-x   0        0        0    11669 2020-02-02 00:00:00.000000 profiwiki-0.1.3/2018/testinstall
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 profiwiki-0.1.3/2018/wiki-config.sh
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 profiwiki-0.1.3/2018/image/phpinfo.php
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 profiwiki-0.1.3/2018/image/profiwiki.php
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 profiwiki-0.1.3/profiwiki/__init__.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 profiwiki-0.1.3/profiwiki/docker.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 profiwiki-0.1.3/profiwiki/patch.py
+-rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 profiwiki-0.1.3/profiwiki/profiwiki_cmd.py
+-rw-r--r--   0        0        0     9074 2020-02-02 00:00:00.000000 profiwiki-0.1.3/profiwiki/profiwiki_core.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 profiwiki-0.1.3/profiwiki/version.py
+-rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 profiwiki-0.1.3/scripts/install
+-rwxr-xr-x   0        0        0      217 2020-02-02 00:00:00.000000 profiwiki-0.1.3/scripts/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 profiwiki-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 profiwiki-0.1.3/tests/basetest.py
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 profiwiki-0.1.3/tests/test_patch.py
+-rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 profiwiki-0.1.3/tests/test_profiwiki.py
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 profiwiki-0.1.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 profiwiki-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 profiwiki-0.1.3/README.md
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 profiwiki-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 profiwiki-0.1.3/PKG-INFO
```

### Comparing `profiwiki-0.1.2/.github/workflows/build.yml` & `profiwiki-0.1.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.2/.github/workflows/upload-to-pypi.yml` & `profiwiki-0.1.3/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.2/2018/bashit` & `profiwiki-0.1.3/2018/bashit`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.2/2018/gencompose` & `profiwiki-0.1.3/2018/gencompose`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.2/2018/profiwiki-install.sh` & `profiwiki-0.1.3/2018/profiwiki-install.sh`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.2/2018/testinstall` & `profiwiki-0.1.3/2018/testinstall`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.2/profiwiki/docker.py` & `profiwiki-0.1.3/profiwiki/docker.py`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.2/profiwiki/patch.py` & `profiwiki-0.1.3/profiwiki/patch.py`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.2/profiwiki/profiwiki_cmd.py` & `profiwiki-0.1.3/profiwiki/profiwiki_cmd.py`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.2/profiwiki/profiwiki_core.py` & `profiwiki-0.1.3/profiwiki/profiwiki_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,16 +67,19 @@
         self.config.fromArgs(args)
         self.wiki_id=f"{self.config.container_base_name}"
         if args.bash:
             cmd=f"docker exec -it {self.config.container_base_name}-mw /bin/bash"
             print(cmd)
             return
         mwApp=self.getMwApp(withGenerate=args.forceRebuild)
+        if self.config.verbose:
+            print(f"ProfiWiki {mwApp.config.container_base_name} using port {mwApp.config.port} sqlport {mwApp.config.sqlPort}")
+   
         if args.randompassword:
-            self.password=self.config.random_password()
+            mwApp.config.password=self.config.random_password()
             self.wikiUser=self.createOrModifyWikiUser(mwApp,force_overwrite=args.forceuser)
         if args.wikiuser and not self.wikiUser:
             self.createOrModifyWikiUser(mwApp,force_overwrite=args.forceuser)
         if args.all:
             if not self.wikiUser:
                 self.wikiUser=self.createOrModifyWikiUser(mwApp,force_overwrite=args.forceuser)
             self.create(mwApp, args.forceRebuild)
@@ -133,16 +136,14 @@
             withGenerate(bool): if True regenerate the configuration files
             
         Returns:
             MediaWikiCluster: the MediaWiki Cluser
         """
         if self.mwCluster is not None:
             return self.mwCluster
-        if self.config.verbose:
-            print(f"ProfiWiki {self.config.prefix} using port {self.config.port}")
         mwCluster=MediaWikiCluster(config=self.config)
         # generate
         mwCluster.createApps(withGenerate=withGenerate)
         self.mwCluster=mwCluster
         return mwCluster
     
     def getMwApp(self,withGenerate:bool=True):
```

### Comparing `profiwiki-0.1.2/profiwiki/version.py` & `profiwiki-0.1.3/profiwiki/version.py`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.2/tests/basetest.py` & `profiwiki-0.1.3/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.2/tests/test_patch.py` & `profiwiki-0.1.3/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.2/tests/test_profiwiki.py` & `profiwiki-0.1.3/tests/test_profiwiki.py`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.2/.gitignore` & `profiwiki-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.2/LICENSE` & `profiwiki-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.2/README.md` & `profiwiki-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.2/pyproject.toml` & `profiwiki-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.2/PKG-INFO` & `profiwiki-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProfiWiki
-Version: 0.1.2
+Version: 0.1.3
 Project-URL: Home, https://github.com/BITPlan/ProfiWiki
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/ProfiWiki
 Project-URL: Source, https://github.com/BITPlan/ProfiWiki
 Author-email: Wolfgang Fahl <wf@bitplan.com>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

