# Comparing `tmp/vernac-0.0.2.tar.gz` & `tmp/vernac-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vernac-0.0.2.tar", last modified: Thu Apr 13 18:56:40 2023, max compression
+gzip compressed data, was "vernac-0.0.3.tar", last modified: Fri Apr 14 23:15:21 2023, max compression
```

## Comparing `vernac-0.0.2.tar` & `vernac-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,28 @@
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-13 18:56:40.753269 vernac-0.0.2/
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1867 2023-04-13 17:01:30.000000 vernac-0.0.2/.gitignore
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1074 2023-04-13 16:57:19.000000 vernac-0.0.2/LICENSE
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     2123 2023-04-13 18:56:40.753269 vernac-0.0.2/PKG-INFO
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1840 2023-04-13 18:44:27.000000 vernac-0.0.2/README.md
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1153 2023-04-13 16:59:44.000000 vernac-0.0.2/dev-requirements.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       34 2023-04-13 16:59:44.000000 vernac-0.0.2/local-dev-requirements.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      574 2023-04-13 18:49:35.000000 vernac-0.0.2/pyproject.toml
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       38 2023-04-13 18:56:40.753269 vernac-0.0.2/setup.cfg
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-13 18:56:40.753269 vernac-0.0.2/src/
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-13 18:56:40.753269 vernac-0.0.2/src/vernac/
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     5980 2023-04-13 16:59:08.000000 vernac-0.0.2/src/vernac/compile.py
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-13 18:56:40.753269 vernac-0.0.2/src/vernac.egg-info/
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     2123 2023-04-13 18:56:40.000000 vernac-0.0.2/src/vernac.egg-info/PKG-INFO
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      319 2023-04-13 18:56:40.000000 vernac-0.0.2/src/vernac.egg-info/SOURCES.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)        1 2023-04-13 18:56:40.000000 vernac-0.0.2/src/vernac.egg-info/dependency_links.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       54 2023-04-13 18:56:40.000000 vernac-0.0.2/src/vernac.egg-info/entry_points.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       65 2023-04-13 18:56:40.000000 vernac-0.0.2/src/vernac.egg-info/requires.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)        7 2023-04-13 18:56:40.000000 vernac-0.0.2/src/vernac.egg-info/top_level.txt
+drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-14 23:15:21.041238 vernac-0.0.3/
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1980 2023-04-14 22:56:26.000000 vernac-0.0.3/.gitignore
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1074 2023-04-13 16:57:19.000000 vernac-0.0.3/LICENSE
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     2478 2023-04-14 23:15:21.041238 vernac-0.0.3/PKG-INFO
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     2195 2023-04-14 04:14:58.000000 vernac-0.0.3/README.md
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     2985 2023-04-14 03:58:04.000000 vernac-0.0.3/dev-requirements.txt
+drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-14 23:15:21.041238 vernac-0.0.3/examples/
+drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-14 23:15:21.041238 vernac-0.0.3/examples/reliable/
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      283 2023-04-14 17:41:58.000000 vernac-0.0.3/examples/reliable/benchmark.vn
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      138 2023-04-14 17:41:58.000000 vernac-0.0.3/examples/reliable/fizzbuzz.vn
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      142 2023-04-14 17:41:58.000000 vernac-0.0.3/examples/reliable/mergesort.vn
+drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-14 23:15:21.041238 vernac-0.0.3/examples/unreliable/
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      433 2023-04-14 22:59:31.000000 vernac-0.0.3/examples/unreliable/count_gpt_titles.vn
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      921 2023-04-14 18:05:37.000000 vernac-0.0.3/examples/unreliable/hntoday.vn
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      312 2023-04-14 18:34:26.000000 vernac-0.0.3/examples/unreliable/snake.vn
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       34 2023-04-13 16:59:44.000000 vernac-0.0.3/local-dev-requirements.txt
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      587 2023-04-13 18:57:07.000000 vernac-0.0.3/pyproject.toml
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       38 2023-04-14 23:15:21.041238 vernac-0.0.3/setup.cfg
+drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-14 23:15:21.041238 vernac-0.0.3/src/
+drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-14 23:15:21.041238 vernac-0.0.3/src/vernac/
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     6625 2023-04-14 23:04:53.000000 vernac-0.0.3/src/vernac/compile.py
+drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-04-14 23:15:21.041238 vernac-0.0.3/src/vernac.egg-info/
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     2478 2023-04-14 23:15:21.000000 vernac-0.0.3/src/vernac.egg-info/PKG-INFO
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      511 2023-04-14 23:15:21.000000 vernac-0.0.3/src/vernac.egg-info/SOURCES.txt
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)        1 2023-04-14 23:15:21.000000 vernac-0.0.3/src/vernac.egg-info/dependency_links.txt
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       54 2023-04-14 23:15:21.000000 vernac-0.0.3/src/vernac.egg-info/entry_points.txt
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       71 2023-04-14 23:15:21.000000 vernac-0.0.3/src/vernac.egg-info/requires.txt
+-rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)        7 2023-04-14 23:15:21.000000 vernac-0.0.3/src/vernac.egg-info/top_level.txt
```

### Comparing `vernac-0.0.2/.gitignore` & `vernac-0.0.3/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -126,7 +126,13 @@
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
 # asdf tool versions (individual to each developer)
 .tool-versions
+
+# direnv config (often contains secrets)
+.envrc
+
+# VS Code (not sure about this; can always add later)
+.vscode/
```

### Comparing `vernac-0.0.2/LICENSE` & `vernac-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vernac-0.0.2/PKG-INFO` & `vernac-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: vernac
-Version: 0.0.2
-Project-URL: homepage, https://github.com/bsilverthorn/vernac
-Project-URL: repository, https://github.com/bsilverthorn/vernac
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 Vernac: programming (in) language 📖
 ====================================
 
 Vernac is a tool for writing software in "vernacular"—plain language.
 
 Vernac isn't for turning English into code; it's for turning English into _programs_:
 
@@ -43,30 +33,51 @@
 
 Its value is in bundling together known prompts and annoying packaging steps so you can go from English to an executable program in one step.
 
 The dream is that you check the _English_ into git, not the code.
 
 Every modern programmer already uses ChatGPT to generate code, then copies the code into their own source file. That’s a bit like writing your application in assembly and occasionally pasting in output from your compiler. Stay in the highest-level language you have for as long as you can! Today, in the GPT era, our highest-level language is English.
 
+Usage
+-----
+
+### Install
+
+- `pip install vernac` or (recommended →) `pipx install vernac`
+
+### Run
+
+- `export OPENAI_API_KEY=<key>`
+- `vernac <source_in> -o <executable_out>`
+
+The executable bundles its dependencies _except_ for a Python interpreter.
+
 Missing features
 ----------------
 
 - Modules
 - Documentation
 - API lookup
 - Error messages
 - Configuration
 - Implicit self-tests
 - Explicit self-tests
 - IDE plugins
 - Integration with other languages
+- Shebang mode
+- Non-OpenAI models
 - Anything non-Linux or non-Python
 - Anything to prevent your programs from behaving differently every time you recompile
 - …
 
+Related work
+------------
+
+- https://github.com/PrefectHQ/marvin
+
 FAQs
 ----
 
 ### What about non-English languages?
 
 They are likely to work, but less likely than English.
```

### Comparing `vernac-0.0.2/pyproject.toml` & `vernac-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 homepage = "https://github.com/bsilverthorn/vernac"
 repository = "https://github.com/bsilverthorn/vernac"
 
 [project.optional-dependencies]
 dev = [
     "ipython",
     "pip-tools",
+    "build",
     "twine",
 ]
 
 [project.scripts]
 vernac = "vernac.compile:script_main"
 
 [tool.setuptools_scm]
```

### Comparing `vernac-0.0.2/src/vernac/compile.py` & `vernac-0.0.3/src/vernac/compile.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import os
+import os.path
 import math
 import re
+import sys
 import argparse
 import subprocess
 
 from typing import (
     cast,
     BinaryIO,
     Iterable,
 )
-from subprocess import check_call
+from subprocess import (
+    check_output,
+    CalledProcessError,
+)
 from tempfile import TemporaryDirectory
 
 import openai
 import tomli_w
 
 from rich import print
 from rich.progress import (
@@ -26,15 +31,14 @@
 from openai import ChatCompletion
 
 progress = Progress(
     SpinnerColumn(),
     TextColumn("[progress.description]{task.description}"),
     BarColumn(),
     TaskProgressColumn(),
-    transient=True,
 )
 openai.api_key = os.getenv("OPENAI_API_KEY")
 
 def normalize_progress(x, scale=100, divisor=32, max_y=0.99):
     return scale * min(
         max_y,
         (1 - math.exp(-x / divisor)),
@@ -74,17 +78,19 @@
     return completion
 
 def strip_markdown_fence(markdown: str) -> str:
     pattern = r"```\s*\w*\s*\n(?P<inner>.*?)```"
     match = re.search(pattern, markdown, re.DOTALL)
 
     if match:
-        return match.group("inner")
+        inner = match.group("inner")
     else:
-        return markdown
+        inner = markdown
+
+    return inner.strip() + "\n"
 
 def get_dependencies(python: str) -> list[str]:
     system_prompt = (
         "You are an expert programmer working on contract. "
         "The user, your client, will share a Python program. "
         "Respond with a list of Python packages that must be installed to run the program. "
         "Standard library packages do not need to be installed and should be ignored. "
@@ -99,17 +105,17 @@
         [
             {"role": "system", "content": system_prompt},
             {"role": "user", "content": user_prompt},
         ],
         model="gpt-4",
         task_title="Analyzing",
     )
-    dependencies = chat_completion.splitlines()
+    dependencies = set(chat_completion.splitlines()) - sys.stdlib_module_names
 
-    return dependencies
+    return list(dependencies)
 
 def compile(english: str):
     system_prompt = (
         "You are an expert programmer working on contract. "
         "The user, your client, will provide a description of program functionality. "
         "Respond with Python 3 source code implementing that description. " 
         "Respond only with the source code inside a Markdown code block. "
@@ -133,15 +139,15 @@
     data = {
         "build-system": {
             "requires": ["setuptools", "setuptools-scm"],
             "build-backend": "setuptools.build_meta"
         },
         "project": {
             "name": "compiled_by_vernac",
-            "requires-python": "~=3.11",
+            "requires-python": ">=3.10",
             "dependencies": deps,
             "version": "0.0.1",
             "scripts": {
                 "main": "compiled_by_vernac.main:main"
             },
         },
     }
@@ -157,50 +163,66 @@
     with open(to_dir("src/compiled_by_vernac/main.py"), "w") as file:
         file.write(python)
 
     with open(to_dir("pyproject.toml"), "wb") as file:
         generate_pyproject(file, deps)
 
 def shiv_package(dir_path: str, out_path: str):
-    check_call(
-        [
-            "shiv",
-            "-o", out_path,
-            "-c", "main",
-            dir_path,
-        ],
-        stdout=subprocess.DEVNULL,
-        stderr=subprocess.DEVNULL,
-    )
+    # crudely guess the shiv bin location
+    python_dir = os.path.dirname(sys.executable)
+    shiv_path = os.path.join(python_dir, "shiv")
+
+    # run shiv to package
+    try:
+        check_output(
+            [
+                shiv_path,
+                "-o", out_path,
+                "-c", "main",
+                dir_path,
+            ],
+            stderr=subprocess.STDOUT,
+        )
+    except CalledProcessError as error:
+        print(error.output)
+
+        raise
 
 def package(python: str, out_path: str, deps: list[str]):
     task = progress.add_task("Packaging", total=2)
 
     with TemporaryDirectory(prefix="vernac") as tmpdir:
         package_in_dir(python=python, dir_path=tmpdir, deps=deps)
 
         progress.update(task, advance=1)
 
         shiv_package(dir_path=tmpdir, out_path=out_path)
 
         progress.update(task, advance=1)
 
-def main(in_path: str, out_path: str):
+def main(in_path: str, out_path: str, verbose: bool = False):
 
     with progress:
         task = progress.add_task("Reading", total=1)
 
         with open(in_path, "r") as f:
             src = f.read()
 
         progress.update(task, advance=1)
 
         python = compile(src)
+
+        if verbose:
+            print("# Source", "\n\n```\n", python, "```")
+
         deps = get_dependencies(python)
 
+        if verbose:
+            print("\n# Dependencies\n", deps)
+
         package(python, out_path, deps)
 
 def parse_args():
     parser = argparse.ArgumentParser()
 
     parser.add_argument(
         dest="in_path",
@@ -210,14 +232,19 @@
     parser.add_argument(
         "-o",
         dest="out_path",
         type=str,
         metavar="PATH",
         required=True,
     )
+    parser.add_argument(
+        "-v",
+        dest="verbose",
+        action="store_true",
+    )
 
     args = parser.parse_args()
 
     return args
 
 def script_main():
     main(**vars(parse_args()))
```

### Comparing `vernac-0.0.2/src/vernac.egg-info/PKG-INFO` & `vernac-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vernac
-Version: 0.0.2
+Version: 0.0.3
 Project-URL: homepage, https://github.com/bsilverthorn/vernac
 Project-URL: repository, https://github.com/bsilverthorn/vernac
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
@@ -43,30 +43,51 @@
 
 Its value is in bundling together known prompts and annoying packaging steps so you can go from English to an executable program in one step.
 
 The dream is that you check the _English_ into git, not the code.
 
 Every modern programmer already uses ChatGPT to generate code, then copies the code into their own source file. That’s a bit like writing your application in assembly and occasionally pasting in output from your compiler. Stay in the highest-level language you have for as long as you can! Today, in the GPT era, our highest-level language is English.
 
+Usage
+-----
+
+### Install
+
+- `pip install vernac` or (recommended →) `pipx install vernac`
+
+### Run
+
+- `export OPENAI_API_KEY=<key>`
+- `vernac <source_in> -o <executable_out>`
+
+The executable bundles its dependencies _except_ for a Python interpreter.
+
 Missing features
 ----------------
 
 - Modules
 - Documentation
 - API lookup
 - Error messages
 - Configuration
 - Implicit self-tests
 - Explicit self-tests
 - IDE plugins
 - Integration with other languages
+- Shebang mode
+- Non-OpenAI models
 - Anything non-Linux or non-Python
 - Anything to prevent your programs from behaving differently every time you recompile
 - …
 
+Related work
+------------
+
+- https://github.com/PrefectHQ/marvin
+
 FAQs
 ----
 
 ### What about non-English languages?
 
 They are likely to work, but less likely than English.
```

