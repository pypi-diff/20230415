# Comparing `tmp/pyfbsdk-stub-generator-0.0.3.tar.gz` & `tmp/pyfbsdk-stub-generator-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c:\Users\nils\Documents\GitHub\pyfbsdk-stub-generator\dist\.tmp-41m6kua8\pyfbsdk-stub-generator-0.0.3.tar", last modified: Fri Jan 13 15:40:39 2023, max compression
+gzip compressed data, was "pyfbsdk-stub-generator-0.0.4.tar", last modified: Sat Apr 15 19:56:13 2023, max compression
```

## Comparing `pyfbsdk-stub-generator-0.0.3.tar` & `pyfbsdk-stub-generator-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-01-13 15:40:39.000000 pyfbsdk-stub-generator-0.0.3/
--rw-rw-rw-   0        0        0     1092 2022-07-10 09:49:23.000000 pyfbsdk-stub-generator-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1749 2023-01-13 15:40:39.000000 pyfbsdk-stub-generator-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1279 2022-07-10 09:49:23.000000 pyfbsdk-stub-generator-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-01-13 15:40:39.000000 pyfbsdk-stub-generator-0.0.3/pyfbsdk_stub_generator/
--rw-rw-rw-   0        0        0      939 2022-12-18 12:00:22.000000 pyfbsdk-stub-generator-0.0.3/pyfbsdk_stub_generator/__init__.py
--rw-rw-rw-   0        0        0      285 2022-12-21 11:45:02.000000 pyfbsdk-stub-generator-0.0.3/pyfbsdk_stub_generator/additions_pyfbsdk.py
--rw-rw-rw-   0        0        0    12306 2022-12-17 20:27:21.000000 pyfbsdk-stub-generator-0.0.3/pyfbsdk_stub_generator/manual_documentation.py
--rw-rw-rw-   0        0        0    23650 2022-12-25 22:11:46.000000 pyfbsdk-stub-generator-0.0.3/pyfbsdk_stub_generator/motionbuilder_documentation_parser.py
--rw-rw-rw-   0        0        0    49212 2022-12-26 18:04:32.000000 pyfbsdk-stub-generator-0.0.3/pyfbsdk_stub_generator/stub_generator.py
-drwxrwxrwx   0        0        0        0 2023-01-13 15:40:39.000000 pyfbsdk-stub-generator-0.0.3/pyfbsdk_stub_generator.egg-info/
--rw-rw-rw-   0        0        0     1749 2023-01-13 15:40:39.000000 pyfbsdk-stub-generator-0.0.3/pyfbsdk_stub_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-01-13 15:40:39.000000 pyfbsdk-stub-generator-0.0.3/pyfbsdk_stub_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-13 15:40:39.000000 pyfbsdk-stub-generator-0.0.3/pyfbsdk_stub_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-01-13 15:40:39.000000 pyfbsdk-stub-generator-0.0.3/pyfbsdk_stub_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-07-10 09:49:23.000000 pyfbsdk-stub-generator-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      596 2023-01-13 15:40:39.000000 pyfbsdk-stub-generator-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-15 19:56:13.829535 pyfbsdk-stub-generator-0.0.4/
+-rw-rw-rw-   0        0        0     1235 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       46 2023-04-15 19:55:38.000000 pyfbsdk-stub-generator-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2051 2023-04-15 19:56:13.829535 pyfbsdk-stub-generator-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1561 2023-04-15 19:07:58.000000 pyfbsdk-stub-generator-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 19:56:13.727218 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/
+-rw-rw-rw-   0        0        0      932 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 19:56:13.763292 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/base_content/
+-rw-rw-rw-   0        0        0      330 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/base_content/pyfbsdk.pyi
+-rw-rw-rw-   0        0        0     7750 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/module_types.py
+-rw-rw-rw-   0        0        0     9182 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/native_generator.py
+drwxrwxrwx   0        0        0        0 2023-04-15 19:56:13.769515 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/
+-rw-rw-rw-   0        0        0      568 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 19:56:13.776239 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/fb_property/
+-rw-rw-rw-   0        0        0        0 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/fb_property/__init__.py
+-rw-rw-rw-   0        0        0     1847 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/fb_property/fb_property_plugin.py
+drwxrwxrwx   0        0        0        0 2023-04-15 19:56:13.787889 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/manual_documentation/
+-rw-rw-rw-   0        0        0       57 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/manual_documentation/__init__.py
+-rw-rw-rw-   0        0        0     1033 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/manual_documentation/doc_bases.py
+drwxrwxrwx   0        0        0        0 2023-04-15 19:56:13.793253 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/manual_documentation/modules/
+-rw-rw-rw-   0        0        0        0 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/manual_documentation/modules/__init__.py
+-rw-rw-rw-   0        0        0     4036 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/manual_documentation/modules/pyfbsdk.py
+-rw-rw-rw-   0        0        0     2978 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/manual_documentation/plugin_manual_docs.py
+drwxrwxrwx   0        0        0        0 2023-04-15 19:56:13.799613 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/online_documentation/
+-rw-rw-rw-   0        0        0       66 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/online_documentation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 19:56:13.824315 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/
+-rw-rw-rw-   0        0        0        0 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/__init__.py
+-rw-rw-rw-   0        0        0     1251 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/documentation_cache.py
+-rw-rw-rw-   0        0        0      492 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/documentation_urls.py
+-rw-rw-rw-   0        0        0    11801 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/page_parser.py
+-rw-rw-rw-   0        0        0     2557 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/table_of_contents.py
+-rw-rw-rw-   0        0        0    16475 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/online_documentation/plugin_online_documentation.py
+-rw-rw-rw-   0        0        0     2666 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/plugins/plugin.py
+-rw-rw-rw-   0        0        0     6559 2023-04-15 16:24:26.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/stub_generator.py
+drwxrwxrwx   0        0        0        0 2023-04-15 19:56:13.758281 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator.egg-info/
+-rw-rw-rw-   0        0        0     2051 2023-04-15 19:56:13.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1649 2023-04-15 19:56:13.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 19:56:13.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 19:56:13.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-04-15 19:56:13.000000 pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2022-06-24 08:36:30.000000 pyfbsdk-stub-generator-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      724 2023-04-15 19:56:13.834870 pyfbsdk-stub-generator-0.0.4/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyfbsdk-stub-generator-0.0.3/PKG-INFO` & `pyfbsdk-stub-generator-0.0.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,27 @@
-Metadata-Version: 2.1
-Name: pyfbsdk-stub-generator
-Version: 0.0.3
-Summary: Generate pyfbsdk stub files for better intellisense when working with MotionBuilder
-Home-page: https://github.com/nils-soderman/pyfbsdk-stub-generator
-Author: Nils Soderman
-Keywords: pyfbsdk,motionbuilder,mobu,autodesk,stub,stubfile,generator,gen
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # MotionBuilder pyfbsdk stub-file generator
-Script for generating more complete python stub files for Autodesk MotionBuilder's pyfbsdk modules.
+Script for generating python stub files for Autodesk MotionBuilder's pyfbsdk module.
+
+These stub files include all classes & functions that can be accessed through the pyfbsdk module.
+They also include type hints and docstrings for most entities.
 
 
 <br>
 
-# Usage
 
-## Pre-generated files
+# Pre-generated files
 The GitHub repository already contains some pre-generated stub files that are ready to be used, simply get them from the [generated-stub-files](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files) folder:
-* [MotionBuilder 2023](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files/motionbuilder-2023)
 * [MotionBuilder 2022](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files/motionbuilder-2022)
+* [MotionBuilder 2023](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files/motionbuilder-2023)
+* [MotionBuilder 2024](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files/motionbuilder-2024)
 
 <br>
 
+# Usage
+
 ## Generate stub files
 If you want to generate your own stub files for your MotionBuilder version:
 
 1. Install the module through pip:
 ```cmd
 python -m pip install pyfbsdk-stub-generator
 ```
@@ -42,8 +35,8 @@
 
 <br>
 
 # Application Spesific Setup
 
 ## Visual Studio Code
 
-These stub files comes bundeled with the [MotionBuilder Utils](https://marketplace.visualstudio.com/items?itemName=NilsSoderman.mobu-utils) VSCode extention.
+These stub files comes bundeled with the [MotionBuilder Utils](https://marketplace.visualstudio.com/items?itemName=NilsSoderman.mobu-utils) VSCode extention.
```

### Comparing `pyfbsdk-stub-generator-0.0.3/pyfbsdk_stub_generator/__init__.py` & `pyfbsdk-stub-generator-0.0.4/pyfbsdk_stub_generator/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import os
 
+
 def Generate(Directory: str, FileExtension = "pyi") -> str:
     """ 
     Generate a stub file for the pyfbsdk module. \\
     This may take a while since the online MoBu sdk documentation will have to be parsed.
 
     ## Parameters:
         - directory: The absolute path to the directory where the pyfbsdk stub file should be created
         - fileExtension: The file extension
-        
+
     ## Returns:
     The filepath to the generated file 
     """
     # Make sure code is running in a motionbuilder python interpreter with access to the pyfbsdk module
     try:
         import pyfbsdk
     except ModuleNotFoundError as e:
         raise ImportError(f"{Generate.__name__} can only be called upon from within MotionBuilder.") from e
-    
-    from .stub_generator import GeneratePYFBSDKStub
+
+    from .stub_generator import GeneratePyfbsdkStubFile
 
     Filepath = os.path.join(Directory, f"pyfbsdk.{FileExtension}")
-     
-    return GeneratePYFBSDKStub(Filepath)
+
+    return GeneratePyfbsdkStubFile(Filepath)
```

### Comparing `pyfbsdk-stub-generator-0.0.3/pyfbsdk_stub_generator.egg-info/PKG-INFO` & `pyfbsdk-stub-generator-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 Metadata-Version: 2.1
 Name: pyfbsdk-stub-generator
-Version: 0.0.3
+Version: 0.0.4
 Summary: Generate pyfbsdk stub files for better intellisense when working with MotionBuilder
 Home-page: https://github.com/nils-soderman/pyfbsdk-stub-generator
 Author: Nils Soderman
+License: UNLICENSE
 Keywords: pyfbsdk,motionbuilder,mobu,autodesk,stub,stubfile,generator,gen
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MotionBuilder pyfbsdk stub-file generator
-Script for generating more complete python stub files for Autodesk MotionBuilder's pyfbsdk modules.
+Script for generating python stub files for Autodesk MotionBuilder's pyfbsdk module.
+
+These stub files include all classes & functions that can be accessed through the pyfbsdk module.
+They also include type hints and docstrings for most entities.
 
 
 <br>
 
-# Usage
 
-## Pre-generated files
+# Pre-generated files
 The GitHub repository already contains some pre-generated stub files that are ready to be used, simply get them from the [generated-stub-files](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files) folder:
-* [MotionBuilder 2023](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files/motionbuilder-2023)
 * [MotionBuilder 2022](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files/motionbuilder-2022)
+* [MotionBuilder 2023](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files/motionbuilder-2023)
+* [MotionBuilder 2024](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files/motionbuilder-2024)
 
 <br>
 
+# Usage
+
 ## Generate stub files
 If you want to generate your own stub files for your MotionBuilder version:
 
 1. Install the module through pip:
 ```cmd
 python -m pip install pyfbsdk-stub-generator
 ```
```

