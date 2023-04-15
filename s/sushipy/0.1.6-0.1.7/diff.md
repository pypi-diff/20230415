# Comparing `tmp/sushipy-0.1.6.tar.gz` & `tmp/sushipy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sushipy-0.1.6.tar", last modified: Sat Apr  1 11:59:44 2023, max compression
+gzip compressed data, was "sushipy-0.1.7.tar", last modified: Sat Apr 15 16:00:19 2023, max compression
```

## Comparing `sushipy-0.1.6.tar` & `sushipy-0.1.7.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 11:59:44.571587 sushipy-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-01 11:59:30.000000 sushipy-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-01 11:59:44.571587 sushipy-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-01 11:59:30.000000 sushipy-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-01 11:59:30.000000 sushipy-0.1.6/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-01 11:59:44.571587 sushipy-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 11:59:44.567587 sushipy-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 11:59:44.571587 sushipy-0.1.6/src/sushipy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 11:59:30.000000 sushipy-0.1.6/src/sushipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 11:59:44.571587 sushipy-0.1.6/src/sushipy/cache/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 11:59:30.000000 sushipy-0.1.6/src/sushipy/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-01 11:59:30.000000 sushipy-0.1.6/src/sushipy/cache/cache_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-01 11:59:30.000000 sushipy-0.1.6/src/sushipy/cache/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 11:59:44.571587 sushipy-0.1.6/src/sushipy/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 11:59:30.000000 sushipy-0.1.6/src/sushipy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-01 11:59:30.000000 sushipy-0.1.6/src/sushipy/config/extends.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-01 11:59:30.000000 sushipy-0.1.6/src/sushipy/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-01 11:59:30.000000 sushipy-0.1.6/src/sushipy/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-04-01 11:59:30.000000 sushipy-0.1.6/src/sushipy/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-01 11:59:30.000000 sushipy-0.1.6/src/sushipy/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-01 11:59:30.000000 sushipy-0.1.6/src/sushipy/one_compile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 11:59:44.571587 sushipy-0.1.6/src/sushipy/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-01 11:59:30.000000 sushipy-0.1.6/src/sushipy/scripts/git_init.ps1
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-01 11:59:30.000000 sushipy-0.1.6/src/sushipy/scripts/git_init.sh
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-01 11:59:30.000000 sushipy-0.1.6/src/sushipy/stores.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 11:59:44.571587 sushipy-0.1.6/src/sushipy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 11:59:30.000000 sushipy-0.1.6/src/sushipy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-01 11:59:30.000000 sushipy-0.1.6/src/sushipy/utils/find_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-01 11:59:30.000000 sushipy-0.1.6/src/sushipy/utils/verbose_print.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 11:59:44.571587 sushipy-0.1.6/src/sushipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-01 11:59:44.000000 sushipy-0.1.6/src/sushipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-01 11:59:44.000000 sushipy-0.1.6/src/sushipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 11:59:44.000000 sushipy-0.1.6/src/sushipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-01 11:59:44.000000 sushipy-0.1.6/src/sushipy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 11:59:44.571587 sushipy-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-01 11:59:30.000000 sushipy-0.1.6/tests/test_execute.py
+drwxrwxrwx   0        0        0        0 2023-04-15 16:00:19.743575 sushipy-0.1.7/
+-rw-rw-rw-   0        0        0     1087 2023-03-24 14:21:03.000000 sushipy-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     1936 2023-04-15 16:00:19.743575 sushipy-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1604 2023-03-29 18:16:15.000000 sushipy-0.1.7/README.md
+-rw-rw-rw-   0        0        0      108 2023-04-05 19:52:34.000000 sushipy-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       36 2023-04-15 15:59:54.000000 sushipy-0.1.7/requirements.txt
+-rw-rw-rw-   0        0        0      531 2023-04-15 16:00:19.745574 sushipy-0.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-15 16:00:19.652576 sushipy-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 16:00:19.693576 sushipy-0.1.7/src/sushipy/
+-rw-rw-rw-   0        0        0        0 2023-02-04 16:09:33.000000 sushipy-0.1.7/src/sushipy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 16:00:19.720575 sushipy-0.1.7/src/sushipy/cache/
+-rw-rw-rw-   0        0        0        0 2023-01-29 15:04:23.000000 sushipy-0.1.7/src/sushipy/cache/__init__.py
+-rw-rw-rw-   0        0        0      206 2023-04-15 15:59:54.000000 sushipy-0.1.7/src/sushipy/cache/cache_template.py
+-rw-rw-rw-   0        0        0     1215 2023-03-30 14:52:20.000000 sushipy-0.1.7/src/sushipy/cache/main.py
+drwxrwxrwx   0        0        0        0 2023-04-15 16:00:19.731075 sushipy-0.1.7/src/sushipy/config/
+-rw-rw-rw-   0        0        0        0 2023-02-04 17:47:51.000000 sushipy-0.1.7/src/sushipy/config/__init__.py
+-rw-rw-rw-   0        0        0     2203 2023-04-15 15:59:54.000000 sushipy-0.1.7/src/sushipy/config/auto_detect.py
+-rw-rw-rw-   0        0        0     3584 2023-04-05 20:02:07.000000 sushipy-0.1.7/src/sushipy/config/extends.py
+-rw-rw-rw-   0        0        0     4877 2023-04-13 16:25:20.000000 sushipy-0.1.7/src/sushipy/execute.py
+-rw-rw-rw-   0        0        0     2822 2023-04-14 13:41:03.000000 sushipy-0.1.7/src/sushipy/git.py
+-rw-rw-rw-   0        0        0     4243 2023-04-15 15:59:54.000000 sushipy-0.1.7/src/sushipy/index.py
+-rw-rw-rw-   0        0        0     1752 2023-04-15 15:59:54.000000 sushipy-0.1.7/src/sushipy/main.py
+-rw-rw-rw-   0        0        0     2050 2023-04-14 13:39:24.000000 sushipy-0.1.7/src/sushipy/one_compile.py
+drwxrwxrwx   0        0        0        0 2023-04-15 16:00:19.734575 sushipy-0.1.7/src/sushipy/scripts/
+-rw-rw-rw-   0        0        0      406 2023-04-01 11:57:52.000000 sushipy-0.1.7/src/sushipy/scripts/git_init.ps1
+-rw-rw-rw-   0        0        0      330 2023-04-01 11:57:52.000000 sushipy-0.1.7/src/sushipy/scripts/git_init.sh
+-rw-rw-rw-   0        0        0      453 2023-03-30 14:53:23.000000 sushipy-0.1.7/src/sushipy/stores.py
+drwxrwxrwx   0        0        0        0 2023-04-15 16:00:19.739075 sushipy-0.1.7/src/sushipy/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-10 16:59:00.000000 sushipy-0.1.7/src/sushipy/utils/__init__.py
+-rw-rw-rw-   0        0        0      236 2023-02-10 16:59:00.000000 sushipy-0.1.7/src/sushipy/utils/find_dict.py
+-rw-rw-rw-   0        0        0      685 2023-03-29 18:15:30.000000 sushipy-0.1.7/src/sushipy/utils/verbose_print.py
+drwxrwxrwx   0        0        0        0 2023-04-15 16:00:19.711075 sushipy-0.1.7/src/sushipy.egg-info/
+-rw-rw-rw-   0        0        0     1936 2023-04-15 16:00:19.000000 sushipy-0.1.7/src/sushipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      735 2023-04-15 16:00:19.000000 sushipy-0.1.7/src/sushipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 16:00:19.000000 sushipy-0.1.7/src/sushipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-15 16:00:19.000000 sushipy-0.1.7/src/sushipy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 16:00:19.742076 sushipy-0.1.7/tests/
+-rw-rw-rw-   0        0        0     1665 2023-04-15 15:59:54.000000 sushipy-0.1.7/tests/test_execute.py
```

### Comparing `sushipy-0.1.6/LICENSE` & `sushipy-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sushipy-0.1.6/PKG-INFO` & `sushipy-0.1.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-Metadata-Version: 2.1
-Name: sushipy
-Version: 0.1.6
-Home-page: https://github.com/dev-sushi/sushi
-Author: ksawery29
-Author-email: sushicontact1@gmail.com
-Project-URL: Bug Tracker, https://github.com/dev-sushi/sushi/issues
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<p align='center'>
-    <img src="https://user-images.githubusercontent.com/47505116/215187622-ea13d72c-178d-48bb-aba4-1398abf3347d.png" alt="Sushi logo">
-    <br/><br/>
-    <img src="https://img.shields.io/pypi/dm/sushipy.svg" alt="Downloads Badge"/>
-    <br/>
-    <img src="https://sonarcloud.io/api/project_badges/measure?project=dev-sushi_sushi&metric=security_rating" alt="Sonar security rating"/>
-    <img src="https://sonarcloud.io/api/project_badges/measure?project=dev-sushi_sushi&metric=sqale_rating" alt="Sonar maintainability rating"/>
-    <img src="https://sonarcloud.io/api/project_badges/measure?project=dev-sushi_sushi&metric=reliability_rating" alt="Sonar reliability rating"/>
-</p>
-
----
-
-Sushi is a library that allows you to run functions from other languages without needing to translate the code.
-
-## How it works
-
-Sushi compiles or interprets the code to create a runnable file which then can be executed, displaying the output in the terminal. Removing the translation step allows for code to run at its native language speed.
-
-## Contributing
-
-If you would like to contribute, here is a common recommended method:
-
-1. Fork the repository on GitHub.
-2. Clone your fork to your local machine.
-3. Create a new branch for your changes.
-4. Make any changes you want to the code or documentation.
-5. Push the changes to your fork on GitHub.
-6. Submit a pull request (be sure to include a good description of your changes!)
-
-## Wiki
-
-The wiki is currently hosted [here](dev-sushi.github.io/docs/).
-
-## License
-
-Sushi is licensed under the MIT license.
+Metadata-Version: 2.1
+Name: sushipy
+Version: 0.1.7
+Home-page: https://github.com/dev-sushi/sushi
+Author: ksawery29
+Author-email: sushicontact1@gmail.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/dev-sushi/sushi/issues
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align='center'>
+    <img src="https://user-images.githubusercontent.com/47505116/215187622-ea13d72c-178d-48bb-aba4-1398abf3347d.png" alt="Sushi logo">
+    <br/><br/>
+    <img src="https://img.shields.io/pypi/dm/sushipy.svg" alt="Downloads Badge"/>
+    <br/>
+    <img src="https://sonarcloud.io/api/project_badges/measure?project=dev-sushi_sushi&metric=security_rating" alt="Sonar security rating"/>
+    <img src="https://sonarcloud.io/api/project_badges/measure?project=dev-sushi_sushi&metric=sqale_rating" alt="Sonar maintainability rating"/>
+    <img src="https://sonarcloud.io/api/project_badges/measure?project=dev-sushi_sushi&metric=reliability_rating" alt="Sonar reliability rating"/>
+</p>
+
+---
+
+Sushi is a library that allows you to run functions from other languages without needing to translate the code.
+
+## How it works
+
+Sushi compiles or interprets the code to create a runnable file which then can be executed, displaying the output in the terminal. Removing the translation step allows for code to run at its native language speed.
+
+## Contributing
+
+If you would like to contribute, here is a common recommended method:
+
+1. Fork the repository on GitHub.
+2. Clone your fork to your local machine.
+3. Create a new branch for your changes.
+4. Make any changes you want to the code or documentation.
+5. Push the changes to your fork on GitHub.
+6. Submit a pull request (be sure to include a good description of your changes!)
+
+## Wiki
+
+The wiki is currently hosted [here](dev-sushi.github.io/docs/).
+
+## License
+
+Sushi is licensed under the MIT license.
```

### Comparing `sushipy-0.1.6/readme.md` & `sushipy-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `sushipy-0.1.6/src/sushipy/cache/main.py` & `sushipy-0.1.7/src/sushipy/cache/main.py`

 * *Files identical despite different names*

### Comparing `sushipy-0.1.6/src/sushipy/config/extends.py` & `sushipy-0.1.7/src/sushipy/config/extends.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,16 @@
         repo = Repo.clone_from(repourl, f"{tempdir}/sushi/")
         repo.git.checkout("main")
 
         # show what command will be executed from extended config
         temp_config = configparser.ConfigParser()
         temp_config.read(f"{tempdir}/sushi/{filename}")
 
-        self._review_config(filename)
+        if config.getboolean("main", "safe_mode") is True:
+            self._review_config(filename)
 
         # add new config to cache
         with open(f"{tempdir}/sushi/{filename}", "r", encoding="UTF-8") as f:
             Cache.update(
                 Cache, "EXTENDS_CONFIG = None", f'EXTENDS_CONFIG = """{f.read()}"""'
             )
```

### Comparing `sushipy-0.1.6/src/sushipy/execute.py` & `sushipy-0.1.7/src/sushipy/execute.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import configparser
 import inspect
 import re
 import shlex
 import subprocess
 from dataclasses import dataclass
-from os import system
+from os import remove, system
 from os.path import isfile
 
 from .cache.main import Cache
 from .stores import ONE_COMPILE
 from .utils.verbose_print import verbose_print
 
 # pylint: disable=import-error
@@ -116,40 +116,46 @@
         self.function(uuid)
 
     def function(self, uuid):
         """runs function from another language"""
 
         path = main_config["lib_path"].split("/")[0]
 
-        if sushicache.LAST_EXECUTED_CODE == self.temp_file:
+        if sushicache.LAST_EXECUTED_CODE == self.temp_file and ONE_COMPILE is False:
             system(f"./{path}/out")
             return
 
         # create temporary file
         temp_extension = config["temp_file"]["extension"]
 
-        with open(
-            file=f"{path}/temp.{temp_extension}", mode="w", encoding="UTF-8"
-        ) as f:
-            f.write(self.temp_file)
-        f.close()
-        # should print the function name for debugging purposes
-        verbose_print("[bold green]sushi[/bold green]   executing function ")
-        subprocess.call(
-            shlex.split(
-                launch_config["exec_command"].replace(
-                    "[file-name]", f"lib/temp.{temp_extension}"
-                )
-            ),
-            shell=False,
-        )
+        def execute_prelaunch():
+            with open(
+                file=f"{path}/temp.{temp_extension}", mode="w", encoding="UTF-8"
+            ) as f:
+                f.write(self.temp_file)
+            f.close()
+
+            # should print the function name for debugging purposes
+            verbose_print("[bold green]sushi[/bold green]   executing function ")
+            subprocess.call(
+                shlex.split(
+                    launch_config["exec_command"].replace(
+                        "[file-name]", f"lib/temp.{temp_extension}"
+                    )
+                ),
+                shell=False,
+            )
 
-        Cache.update(
-            Cache,
-            f"LAST_EXECUTED_CODE = {sushicache.LAST_EXECUTED_CODE}",
-            f'LAST_EXECUTED_CODE = """{TEMP_FILE}"""',
-        )
+            Cache.update(
+                Cache,
+                f"LAST_EXECUTED_CODE = {sushicache.LAST_EXECUTED_CODE}",
+                f'LAST_EXECUTED_CODE = """{TEMP_FILE}"""',
+            )
+
+        # we should skip it if using one (time) compile
+        if ONE_COMPILE is False:
+            execute_prelaunch()
 
         print(uuid)
         # remove temp file
-        # remove(f"{path}/temp.{temp_extension}")
+        remove(f"{path}/temp.{temp_extension}")
         subprocess.call([f"./{path}/out", uuid], shell=False)
```

### Comparing `sushipy-0.1.6/src/sushipy/git.py` & `sushipy-0.1.7/src/sushipy/git.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,95 @@
-"""Tracks library change with git"""
-
-import configparser
-import os
-import subprocess
-import sys
-from contextlib import suppress
-from os import chdir
-from os.path import isfile
-from sys import platform
-
-from rich import print as rich_print
-
-from .cache.main import Cache
-from .utils.verbose_print import verbose_print
-
-# pylint: disable=import-error
-if isfile("sushicache.py"):
-    import sushicache
-# pylint: enable=import-error
-
-config = configparser.ConfigParser()
-config.read("sushi.conf")
-
-
-class GitTracking:
-    """git tracking"""
-
-    def _find_changes(self) -> None:
-        """returns false if no changes"""
-
-        chdir("lib")
-        result = subprocess.run(
-            ["git", "--git-dir=.sushi-git", "status"],
-            capture_output=True,
-            text=True,
-            check=True,
-        )
-        result = result.stdout.split("\n")
-
-        return result[1] == "nothing to commit, working tree clean"
-
-    def _configure_git(self) -> None:
-        with suppress(KeyError):
-            if config.getboolean("main", "safe_mode") is True:
-                rich_print(
-                    "To continue, sushi needs to execute one shell script. "
-                    + "If you agree to continue, press any key. Otherwise press N"
-                )
-
-                input_data = input()
-                if input_data.capitalize() == "N":
-                    sys.exit(0)
-
-        def v_print(script_name: str):
-            verbose_print(
-                f"[bold green]sushi[/bold green]   executing script: {script_name}"
-            )
-
-        # run script
-        if platform in ("linux", "linux2", "darwin"):
-            v_print("git_init.sh")
-
-            current_path = os.path.dirname(__file__)
-            path = os.path.abspath(str(current_path) + "/scripts/git_init.sh")
-            os.system(f"chmod +x {path}")
-            subprocess.call(
-                [path, "lib"],
-                stdout=subprocess.DEVNULL,
-                shell=False,
-            )
-
-        elif platform == "win32":
-            v_print("git_init.ps1")
-            print("windows in progress")
-
-        Cache.update(Cache, "GIT_CONFIGURED = False", "GIT_CONFIGURED = True")
-
-    def __init__(self) -> None:
-        with suppress(NameError):
-            if sushicache.GIT_CONFIGURED is True:
-                return
-
-        self._configure_git()
+"""Tracks library change with git"""
+
+import configparser
+import os
+import subprocess
+import sys
+from contextlib import suppress
+from os import chdir
+from os.path import isfile
+from sys import platform
+
+from rich import print as rich_print
+
+from .cache.main import Cache
+from .utils.verbose_print import verbose_print
+
+# pylint: disable=import-error
+if isfile("sushicache.py"):
+    import sushicache
+# pylint: enable=import-error
+
+config = configparser.ConfigParser()
+config.read("sushi.conf")
+
+
+class GitTracking:
+    """git tracking"""
+
+    def _find_changes(self) -> None:
+        """returns False if no changes"""
+
+        if not isfile("sushicache.py"):
+            return False
+
+        chdir("lib")
+        result = subprocess.run(
+            ["git", "--git-dir=.sushi-git", "status"],
+            capture_output=True,
+            text=True,
+            check=True,
+        )
+        result = result.stdout.split("\n")
+
+        return result[1] == "nothing to commit, working tree clean"
+
+    def _configure_git(self) -> None:
+        with suppress(KeyError):
+            if config.getboolean("main", "safe_mode") is True:
+                rich_print(
+                    "To continue, sushi needs to execute one shell script. "
+                    + "If you agree to continue, press any key. Otherwise press N"
+                )
+
+                input_data = input()
+                if input_data.capitalize() == "N":
+                    sys.exit(0)
+
+        def v_print(script_name: str):
+            verbose_print(
+                f"[bold green]sushi[/bold green]   executing script: {script_name}"
+            )
+
+        # run script
+        if platform in ("linux", "linux2", "darwin"):
+            v_print("git_init.sh")
+
+            current_path = os.path.dirname(__file__)
+            path = os.path.abspath(str(current_path) + "/scripts/git_init.sh")
+            os.system(f"chmod +x {path}")
+            subprocess.call(
+                [path, "lib"],
+                stdout=subprocess.DEVNULL,
+                shell=False,
+            )
+
+        elif platform == "win32":
+            v_print("git_init.ps1")
+            print("windows in progress! report any issues on github")
+
+            current_path = os.path.dirname(__file__)
+            path = os.path.abspath(str(current_path) + "/scripts/git_init.ps1")
+            subprocess.call(
+                [path, "lib"],
+                stdout=subprocess.DEVNULL,
+                shell=False,
+            )
+
+        Cache.update(Cache, "GIT_CONFIGURED = False", "GIT_CONFIGURED = True")
+
+    def __init__(self) -> None:
+        with suppress(NameError):
+            if sushicache.GIT_CONFIGURED is True:
+                return
+
+        self._configure_git()
```

### Comparing `sushipy-0.1.6/src/sushipy/main.py` & `sushipy-0.1.7/src/sushipy/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from rich import print as rich_print
 
 from .cache.main import Cache
 from .config import extends
 from .git import GitTracking
 from .index import find
+from .one_compile import OneCompile
 from .utils.verbose_print import verbose_print
 
 config = configparser.ConfigParser()
 config.read("sushi.conf")
 
 
 # pylint: disable=import-error
@@ -28,14 +29,18 @@
 class Sushi:
     """sushi"""
 
     def _check_config(self) -> None:
         if not path.isfile("sushi.conf"):
             rich_print("[bold red]sushi[/bold red]   configuration file doesnt exists")
             sys.exit(1)
+        elif config.getboolean("main", "safe_mode") is False:
+            verbose_print(
+                "[bold yellow]sushi[/bold yellow]   running with safe_mode turned off!"
+            )
 
     def _extend_check(self) -> None:
         # check if configs needs to be extended
 
         try:
             config["extends"]["repo"]
         except KeyError:
@@ -44,13 +49,20 @@
             # skip extend config if it was already extended
             if sushicache.EXTENDS_CONFIG is None:
                 obj = extends.ConfigExtends()
                 obj.install()
 
     def __init__(self) -> None:
         verbose_print("[bold green]sushi[/bold green]   checking sushi config ")
+
         # cleaner way to run multiple functions
-        functions = [self._check_config, self._extend_check, Cache, GitTracking]
+        functions = [
+            Cache,
+            self._check_config,
+            self._extend_check,
+            GitTracking,
+            OneCompile,
+        ]
         for f in functions:
             f()
 
         find()
```

### Comparing `sushipy-0.1.6/src/sushipy/one_compile.py` & `sushipy-0.1.7/src/sushipy/one_compile.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,67 +1,76 @@
-"""one compile"""
-
-import configparser
-import uuid
-from contextlib import suppress
-from os.path import isfile
-
-from .cache.main import Cache
-
-config = configparser.ConfigParser()
-config.read("sushi.conf")
-
-# pylint: disable=import-error
-if isfile("sushicache.py"):
-    import sushicache
-
-    DATA = sushicache.INDEXED_FUNCTIONS
-# pylint: enable=import-error
-
-
-class OneCompile:
-    """one compile"""
-
-    def setup(self) -> None:
-        """setup onecompile"""
-
-        # TODO: cleanup
-        if_data = self._extract_if()
-        data = [{"uuid": str(uuid.uuid4()), "name": DATA[0]["name"]}]
-        out = self._parse_if(if_data["if"], data[0]["uuid"], data[0]["name"])
-
-        if len(DATA) > 1:
-            for x in range(len(DATA)):
-                with suppress(IndexError):
-                    out += self._parse_if(
-                        if_data["else"], str(uuid.uuid4()), DATA[x + 1]["name"]
-                    )
-
-        Cache.update(
-            Cache,
-            f'CUSTOM_TEMP_FILE = """{sushicache.CUSTOM_TEMP_FILE}"""',
-            f'CUSTOM_TEMP_FILE = """{out}"""',
-        )
-
-        return data
-
-    def _extract_if(self):
-        # extracts if statements
-        launch = config["launch"]["if_statement"]
-        else_start = "$SUSHI_ELSE_START"
-
-        split_string = launch.split(else_start)
-
-        return {"if": split_string[0], "else": split_string[1]}
-
-    def _parse_if(self, data, uuid_data, code):
-        translate_date = {
-            "$SUSHI_ARG_NUM": "1",
-            "$SUSHI_SEMICOLON": ";",
-            "$SUSHI_UUID": uuid_data,
-            "$SUSHI_CODE": code,
-        }
-
-        for i, j in translate_date.items():
-            data = data.replace(i, j)
-
-        return data
+"""one compile"""
+
+import configparser
+import uuid
+from contextlib import suppress
+from os.path import isfile
+
+from .cache.main import Cache
+
+config = configparser.ConfigParser()
+config.read("sushi.conf")
+
+# pylint: disable=import-error
+if isfile("sushicache.py"):
+    import sushicache
+
+# pylint: enable=import-error
+
+
+class OneCompile:
+    """one compile"""
+
+    def setup(self) -> None:
+        """setup onecompile"""
+
+        cache_data = sushicache.INDEXED_FUNCTIONS
+
+        # TODO: cleanup
+        if_data = self._extract_if()
+        data = [{"uuid": str(uuid.uuid4()), "name": cache_data[0]["name"]}]
+        out = self._parse_if(if_data["if"], data[0]["uuid"], data[0]["name"])
+
+        if len(cache_data) > 1:
+            for x in range(len(cache_data)):
+                with suppress(IndexError):
+                    out += self._parse_if(
+                        if_data["else"], str(uuid.uuid4()), cache_data[x + 1]["name"]
+                    )
+
+        Cache.update(
+            Cache,
+            f'CUSTOM_TEMP_FILE = """{sushicache.CUSTOM_TEMP_FILE}"""',
+            f'CUSTOM_TEMP_FILE = """{out}"""',
+        )
+
+        return data
+
+    def _extract_if(self):
+        # extracts if statements
+        launch = config["launch"]["if_statement"]
+        else_start = "$SUSHI_ELSE_START"
+
+        split_string = launch.split(else_start)
+
+        return {"if": split_string[0], "else": split_string[1]}
+
+    def _parse_if(self, data, uuid_data, code):
+        translate_date = {
+            "$SUSHI_ARG_NUM": "1",
+            "$SUSHI_SEMICOLON": ";",
+            "$SUSHI_UUID": uuid_data,
+            "$SUSHI_CODE": code,
+        }
+
+        for i, j in translate_date.items():
+            data = data.replace(i, j)
+
+        return data
+
+    def __init__(self) -> None:
+        # TODO: implement other cache system
+        try:
+            if sushicache.ONE_COMPILE_CONFIGURED is False:
+                self.setup()
+        except NameError:
+            return
```

### Comparing `sushipy-0.1.6/src/sushipy/utils/verbose_print.py` & `sushipy-0.1.7/src/sushipy/utils/verbose_print.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-"""verbose print"""
-
-import configparser
-
-from rich import print as rich_print
-
-# TODO: maybe move to stores.py
-
-config = configparser.ConfigParser()
-config.read("sushi.conf")
-
-verbose_flag = config["launch"].getboolean("verbose", fallback=False)
-
-
-def verbose_print(message: str):
-    """
-    Prints a verbose message using rich library if the 'verbose' flag is set to True.
-
-    Args:
-        message (str): The message to be printed.
-        verbose (bool): A flag to determine if the message should be printed or not.
-
-    Example:
-        verbose_print("This is a verbose message", verbose=True)
-    """
-    if verbose_flag:
-        rich_print(message)
+"""verbose print"""
+
+import configparser
+
+from rich import print as rich_print
+
+# TODO: maybe move to stores.py
+
+config = configparser.ConfigParser()
+config.read("sushi.conf")
+
+verbose_flag = config["launch"].getboolean("verbose", fallback=False)
+
+
+def verbose_print(message: str):
+    """
+    Prints a verbose message using rich library if the 'verbose' flag is set to True.
+
+    Args:
+        message (str): The message to be printed.
+        verbose (bool): A flag to determine if the message should be printed or not.
+
+    Example:
+        verbose_print("This is a verbose message", verbose=True)
+    """
+    if verbose_flag:
+        rich_print(message)
```

### Comparing `sushipy-0.1.6/src/sushipy.egg-info/PKG-INFO` & `sushipy-0.1.7/src/sushipy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-Metadata-Version: 2.1
-Name: sushipy
-Version: 0.1.6
-Home-page: https://github.com/dev-sushi/sushi
-Author: ksawery29
-Author-email: sushicontact1@gmail.com
-Project-URL: Bug Tracker, https://github.com/dev-sushi/sushi/issues
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<p align='center'>
-    <img src="https://user-images.githubusercontent.com/47505116/215187622-ea13d72c-178d-48bb-aba4-1398abf3347d.png" alt="Sushi logo">
-    <br/><br/>
-    <img src="https://img.shields.io/pypi/dm/sushipy.svg" alt="Downloads Badge"/>
-    <br/>
-    <img src="https://sonarcloud.io/api/project_badges/measure?project=dev-sushi_sushi&metric=security_rating" alt="Sonar security rating"/>
-    <img src="https://sonarcloud.io/api/project_badges/measure?project=dev-sushi_sushi&metric=sqale_rating" alt="Sonar maintainability rating"/>
-    <img src="https://sonarcloud.io/api/project_badges/measure?project=dev-sushi_sushi&metric=reliability_rating" alt="Sonar reliability rating"/>
-</p>
-
----
-
-Sushi is a library that allows you to run functions from other languages without needing to translate the code.
-
-## How it works
-
-Sushi compiles or interprets the code to create a runnable file which then can be executed, displaying the output in the terminal. Removing the translation step allows for code to run at its native language speed.
-
-## Contributing
-
-If you would like to contribute, here is a common recommended method:
-
-1. Fork the repository on GitHub.
-2. Clone your fork to your local machine.
-3. Create a new branch for your changes.
-4. Make any changes you want to the code or documentation.
-5. Push the changes to your fork on GitHub.
-6. Submit a pull request (be sure to include a good description of your changes!)
-
-## Wiki
-
-The wiki is currently hosted [here](dev-sushi.github.io/docs/).
-
-## License
-
-Sushi is licensed under the MIT license.
+Metadata-Version: 2.1
+Name: sushipy
+Version: 0.1.7
+Home-page: https://github.com/dev-sushi/sushi
+Author: ksawery29
+Author-email: sushicontact1@gmail.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/dev-sushi/sushi/issues
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align='center'>
+    <img src="https://user-images.githubusercontent.com/47505116/215187622-ea13d72c-178d-48bb-aba4-1398abf3347d.png" alt="Sushi logo">
+    <br/><br/>
+    <img src="https://img.shields.io/pypi/dm/sushipy.svg" alt="Downloads Badge"/>
+    <br/>
+    <img src="https://sonarcloud.io/api/project_badges/measure?project=dev-sushi_sushi&metric=security_rating" alt="Sonar security rating"/>
+    <img src="https://sonarcloud.io/api/project_badges/measure?project=dev-sushi_sushi&metric=sqale_rating" alt="Sonar maintainability rating"/>
+    <img src="https://sonarcloud.io/api/project_badges/measure?project=dev-sushi_sushi&metric=reliability_rating" alt="Sonar reliability rating"/>
+</p>
+
+---
+
+Sushi is a library that allows you to run functions from other languages without needing to translate the code.
+
+## How it works
+
+Sushi compiles or interprets the code to create a runnable file which then can be executed, displaying the output in the terminal. Removing the translation step allows for code to run at its native language speed.
+
+## Contributing
+
+If you would like to contribute, here is a common recommended method:
+
+1. Fork the repository on GitHub.
+2. Clone your fork to your local machine.
+3. Create a new branch for your changes.
+4. Make any changes you want to the code or documentation.
+5. Push the changes to your fork on GitHub.
+6. Submit a pull request (be sure to include a good description of your changes!)
+
+## Wiki
+
+The wiki is currently hosted [here](dev-sushi.github.io/docs/).
+
+## License
+
+Sushi is licensed under the MIT license.
```

### Comparing `sushipy-0.1.6/src/sushipy.egg-info/SOURCES.txt` & `sushipy-0.1.7/src/sushipy.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 LICENSE
+README.md
 pyproject.toml
 readme.md
+requirements.txt
 setup.cfg
 src/sushipy/__init__.py
 src/sushipy/execute.py
 src/sushipy/git.py
 src/sushipy/index.py
 src/sushipy/main.py
 src/sushipy/one_compile.py
@@ -13,14 +15,15 @@
 src/sushipy.egg-info/SOURCES.txt
 src/sushipy.egg-info/dependency_links.txt
 src/sushipy.egg-info/top_level.txt
 src/sushipy/cache/__init__.py
 src/sushipy/cache/cache_template.py
 src/sushipy/cache/main.py
 src/sushipy/config/__init__.py
+src/sushipy/config/auto_detect.py
 src/sushipy/config/extends.py
 src/sushipy/scripts/git_init.ps1
 src/sushipy/scripts/git_init.sh
 src/sushipy/utils/__init__.py
 src/sushipy/utils/find_dict.py
 src/sushipy/utils/verbose_print.py
 tests/test_execute.py
```

### Comparing `sushipy-0.1.6/tests/test_execute.py` & `sushipy-0.1.7/tests/test_execute.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,12 +54,12 @@
         print(result)
         os.chdir("../")
 
         return result
 
     def test_noarg(self):
         result = self.run_example("noarg-temp/")
-        assert result[2] == "Hello from sushi!"
+        assert result[3] == "Hello from sushi!"
 
     def test_arg(self):
         result = self.run_example("arg-temp/")
-        assert result[2] == "You provided 1"
+        assert result[3] == "You provided 1"
```

