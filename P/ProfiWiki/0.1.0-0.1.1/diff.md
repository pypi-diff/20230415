# Comparing `tmp/profiwiki-0.1.0.tar.gz` & `tmp/profiwiki-0.1.1.tar.gz`

## Comparing `profiwiki-0.1.0.tar` & `profiwiki-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,33 @@
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 profiwiki-0.1.0/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 profiwiki-0.1.0/.pydevproject
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 profiwiki-0.1.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 profiwiki-0.1.0/.github/workflows/upload-to-pypi.yml
--rwxr-xr-x   0        0        0      938 2020-02-02 00:00:00.000000 profiwiki-0.1.0/2018/bashit
--rwxr-xr-x   0        0        0     3234 2020-02-02 00:00:00.000000 profiwiki-0.1.0/2018/gencompose
--rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 profiwiki-0.1.0/2018/mw1_27_7
--rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 profiwiki-0.1.0/2018/mw1_30_1
--rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 profiwiki-0.1.0/2018/mw1_31_1
--rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 profiwiki-0.1.0/2018/mw1_33_1
--rwxr-xr-x   0        0        0    24022 2020-02-02 00:00:00.000000 profiwiki-0.1.0/2018/profiwiki-install.sh
--rwxr-xr-x   0        0        0    11669 2020-02-02 00:00:00.000000 profiwiki-0.1.0/2018/testinstall
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 profiwiki-0.1.0/2018/wiki-config.sh
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 profiwiki-0.1.0/2018/image/phpinfo.php
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 profiwiki-0.1.0/2018/image/profiwiki.php
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 profiwiki-0.1.0/profiwiki/__init__.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 profiwiki-0.1.0/profiwiki/docker.py
--rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 profiwiki-0.1.0/profiwiki/profiwiki_cmd.py
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 profiwiki-0.1.0/profiwiki/profiwiki_core.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 profiwiki-0.1.0/profiwiki/version.py
--rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 profiwiki-0.1.0/scripts/install
--rwxr-xr-x   0        0        0      217 2020-02-02 00:00:00.000000 profiwiki-0.1.0/scripts/test
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 profiwiki-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 profiwiki-0.1.0/tests/basetest.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 profiwiki-0.1.0/tests/test_profiwiki.py
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 profiwiki-0.1.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 profiwiki-0.1.0/LICENSE
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 profiwiki-0.1.0/README.md
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 profiwiki-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 profiwiki-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 profiwiki-0.1.1/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 profiwiki-0.1.1/.pydevproject
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 profiwiki-0.1.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 profiwiki-0.1.1/.github/workflows/upload-to-pypi.yml
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 profiwiki-0.1.1/.vscode/settings.json
+-rwxr-xr-x   0        0        0      938 2020-02-02 00:00:00.000000 profiwiki-0.1.1/2018/bashit
+-rwxr-xr-x   0        0        0     3234 2020-02-02 00:00:00.000000 profiwiki-0.1.1/2018/gencompose
+-rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 profiwiki-0.1.1/2018/mw1_27_7
+-rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 profiwiki-0.1.1/2018/mw1_30_1
+-rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 profiwiki-0.1.1/2018/mw1_31_1
+-rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 profiwiki-0.1.1/2018/mw1_33_1
+-rwxr-xr-x   0        0        0    24022 2020-02-02 00:00:00.000000 profiwiki-0.1.1/2018/profiwiki-install.sh
+-rwxr-xr-x   0        0        0    11669 2020-02-02 00:00:00.000000 profiwiki-0.1.1/2018/testinstall
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 profiwiki-0.1.1/2018/wiki-config.sh
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 profiwiki-0.1.1/2018/image/phpinfo.php
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 profiwiki-0.1.1/2018/image/profiwiki.php
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 profiwiki-0.1.1/profiwiki/__init__.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 profiwiki-0.1.1/profiwiki/docker.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 profiwiki-0.1.1/profiwiki/patch.py
+-rw-r--r--   0        0        0     5831 2020-02-02 00:00:00.000000 profiwiki-0.1.1/profiwiki/profiwiki_cmd.py
+-rw-r--r--   0        0        0     9016 2020-02-02 00:00:00.000000 profiwiki-0.1.1/profiwiki/profiwiki_core.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 profiwiki-0.1.1/profiwiki/version.py
+-rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 profiwiki-0.1.1/scripts/install
+-rwxr-xr-x   0        0        0      217 2020-02-02 00:00:00.000000 profiwiki-0.1.1/scripts/test
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 profiwiki-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 profiwiki-0.1.1/tests/basetest.py
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 profiwiki-0.1.1/tests/test_patch.py
+-rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 profiwiki-0.1.1/tests/test_profiwiki.py
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 profiwiki-0.1.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 profiwiki-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 profiwiki-0.1.1/README.md
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 profiwiki-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 profiwiki-0.1.1/PKG-INFO
```

### Comparing `profiwiki-0.1.0/.github/workflows/build.yml` & `profiwiki-0.1.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.0/.github/workflows/upload-to-pypi.yml` & `profiwiki-0.1.1/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.0/2018/bashit` & `profiwiki-0.1.1/2018/bashit`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.0/2018/gencompose` & `profiwiki-0.1.1/2018/gencompose`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.0/2018/profiwiki-install.sh` & `profiwiki-0.1.1/2018/profiwiki-install.sh`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.0/2018/testinstall` & `profiwiki-0.1.1/2018/testinstall`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.0/profiwiki/docker.py` & `profiwiki-0.1.1/profiwiki/docker.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,46 +10,57 @@
 class ProfiWikiContainer():
     """
     a profiwiki docker container wrapper
     """
     def __init__(self,dc:DockerContainer):
         """
         Args:
-            dc: the Docc
+            dc(DockerContainer): the to wrap
         """
         self.dc=dc
     
     def log_action(self,action:str):
-        print(f"{action} {self.dc.kind} {self.dc.name}",flush=True)
+        """
+        log the given action
+        
+        Args:
+            action(str): the d
+        """
+        if self.dc:
+            print(f"{action} {self.dc.kind} {self.dc.name}",flush=True)
+        else:
+            print(f"{action}",flush=True)
         
     def upload(self,text:str,path:str):
         """
         upload the given text to the given path
         """
         with tempfile.NamedTemporaryFile() as tmp:
-            self.log_action(f"uploading {tmp.name} to ")
+            self.log_action(f"uploading {tmp.name} as {path} to ")
             with open(tmp.name,"w") as text_file:
                 text_file.write(text)
             self.dc.container.copy_to(tmp.name,path)
         
-        
-    def killremove(self):
+    def killremove(self,volumes:bool=False):
         """
         kill and remove me
+        
+        Args:
+            volumes(bool): if True remove anonymous volumes associated with the container, default=True (to avoid e.g. passwords to get remembered / stuck
         """
         if self.dc:
             self.log_action("killing and removing")
             self.dc.container.kill()
-            self.dc.container.remove()
+            self.dc.container.remove(volumes=volumes)
 
     def start_cron(self):
         """
         Starting periodic command scheduler: cron.
-        """        
-        self.dc.container.execute(["sh","-c","service","cron","start"],tty=True)
+        """  
+        self.dc.container.execute(["/usr/sbin/service","cron","start"],tty=True)
         
     def install_plantuml(self):
         """
         install plantuml to this container
         """
         # https://gabrieldemarmiesse.github.io/python-on-whales/docker_objects/containers/
         self.dc.container.execute(["apt-get","update"],tty=True)
@@ -83,10 +94,11 @@
         self.upload(script,"/root/install_fontawesome")
         # make executable
         self.dc.container.execute(["chmod","+x",script_path])
         self.dc.container.execute([script_path],tty=True)
         try:
             self.dc.container.execute(["service","apache2","restart"])
         except DockerException as e:
+            # we expect a SIGTERM
             if not e.return_code==143:
                 raise e
         pass
```

### Comparing `profiwiki-0.1.0/profiwiki/version.py` & `profiwiki-0.1.1/profiwiki/version.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 
 @author: wf
 '''
 import profiwiki
 
 class Version(object):
     '''
-    Version handling for pysotsog
+    Version handling for ProfiWiki
     '''
     name="pyProfiWiki"
     description="""BITPlan's professional Semantic Mediawiki"""
     version=profiwiki.__version__
     date = '2023-04-01'
-    updated = '2023-04-01'
+    updated = '2023-04-08'
     authors='Wolfgang Fahl'
     doc_url="https://wiki.bitplan.com/index.php/ProfiWiki"
     chat_url="https://github.com/BITPlan/ProfiWiki/discussions"
     cm_url="https://github.com/BITPlan/ProfiWiki"
     license=f'''Copyright 2015-2023 contributors. All rights reserved.
   Licensed under the Apache License 2.0
   http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `profiwiki-0.1.0/tests/basetest.py` & `profiwiki-0.1.1/tests/basetest.py`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.0/.gitignore` & `profiwiki-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.0/LICENSE` & `profiwiki-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.0/README.md` & `profiwiki-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `profiwiki-0.1.0/pyproject.toml` & `profiwiki-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 maintainers = [
   { name = "Wolfgang Fahl", email = "wf@bitplan.com" },
 ]
 readme = "README.md"
 license= "Apache-2.0"
 dependencies = [
   #https://pypi.org/project/pymediawikidocker/
-  "pymediawikidocker",
+  "pymediawikidocker>=0.9.8",
   #https://pypi.org/project/py-3rdparty-mediawiki/
   "py-3rdparty-mediawiki"
 ]
 
 requires-python = ">=3.8"
 classifiers=[
     "Development Status :: 4 - Beta",
@@ -44,14 +44,17 @@
 Home = "https://github.com/BITPlan/ProfiWiki"
 Documentation = "https://wiki.bitplan.com/index.php/ProfiWiki"
 Source = "https://github.com/BITPlan/ProfiWiki"
 
 [project.optional-dependencies]
 test = [
   "green",
+  "pydevd",
+  # https://pypi.python.org/pypi/ptvsd
+  "ptvsd"
 ]
 
 [tool.hatch.build.targets.wheel]
 packages = [
   "profiwiki",
 ]
```

### Comparing `profiwiki-0.1.0/PKG-INFO` & `profiwiki-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProfiWiki
-Version: 0.1.0
+Version: 0.1.1
 Project-URL: Home, https://github.com/BITPlan/ProfiWiki
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/ProfiWiki
 Project-URL: Source, https://github.com/BITPlan/ProfiWiki
 Author-email: Wolfgang Fahl <wf@bitplan.com>
 Maintainer-email: Wolfgang Fahl <wf@bitplan.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -19,17 +19,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Requires-Dist: py-3rdparty-mediawiki
-Requires-Dist: pymediawikidocker
+Requires-Dist: pymediawikidocker>=0.9.8
 Provides-Extra: test
 Requires-Dist: green; extra == 'test'
+Requires-Dist: ptvsd; extra == 'test'
+Requires-Dist: pydevd; extra == 'test'
 Description-Content-Type: text/markdown
 
 # BITPlan ProfiWiki
 BITPlan's Professional SemanticMediaWiki
 
 [![Join the discussion at https://github.com/BITPlan/ProfiWiki/discussions](https://img.shields.io/github/discussions/BITPlan/ProfiWiki)](https://github.com/BITPlan/ProfiWiki/discussions)
 [![pypi](https://img.shields.io/pypi/pyversions/ProfiWiki)](https://pypi.org/project/ProfiWiki/)
```

