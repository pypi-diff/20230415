# Comparing `tmp/badgie-0.2.0.tar.gz` & `tmp/badgie-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badgie-0.2.0.tar", last modified: Wed Apr 12 06:02:46 2023, max compression
+gzip compressed data, was "badgie-0.3.0.tar", last modified: Fri Apr 14 23:35:30 2023, max compression
```

## Comparing `badgie-0.2.0.tar` & `badgie-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 06:02:46.109152 badgie-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-04-12 06:02:42.000000 badgie-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3726 2023-04-12 06:02:46.109152 badgie-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2834 2023-04-12 06:02:42.000000 badgie-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 06:02:46.105151 badgie-0.2.0/badgie/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 06:02:42.000000 badgie-0.2.0/badgie/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3145 2023-04-12 06:02:42.000000 badgie-0.2.0/badgie/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-12 06:02:42.000000 badgie-0.2.0/badgie/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 06:02:46.109152 badgie-0.2.0/badgie/badges/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 06:02:42.000000 badgie-0.2.0/badgie/badges/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      875 2023-04-12 06:02:42.000000 badgie-0.2.0/badgie/badges/_base.py
--rw-rw-rw-   0 root         (0) root         (0)      761 2023-04-12 06:02:42.000000 badgie-0.2.0/badgie/badges/brettops.py
--rw-rw-rw-   0 root         (0) root         (0)      715 2023-04-12 06:02:42.000000 badgie-0.2.0/badgie/badges/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-04-12 06:02:42.000000 badgie-0.2.0/badgie/badges/precommit.py
--rw-rw-rw-   0 root         (0) root         (0)      202 2023-04-12 06:02:42.000000 badgie-0.2.0/badgie/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      211 2023-04-12 06:02:42.000000 badgie-0.2.0/badgie/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1426 2023-04-12 06:02:42.000000 badgie-0.2.0/badgie/parser.py
--rw-rw-rw-   0 root         (0) root         (0)      853 2023-04-12 06:02:42.000000 badgie-0.2.0/badgie/sources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 06:02:46.107152 badgie-0.2.0/badgie.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3726 2023-04-12 06:02:46.000000 badgie-0.2.0/badgie.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      473 2023-04-12 06:02:46.000000 badgie-0.2.0/badgie.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 06:02:46.000000 badgie-0.2.0/badgie.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-04-12 06:02:46.000000 badgie-0.2.0/badgie.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-12 06:02:46.000000 badgie-0.2.0/badgie.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-12 06:02:46.000000 badgie-0.2.0/badgie.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-04-12 06:02:46.109152 badgie-0.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1391 2023-04-12 06:02:42.000000 badgie-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 23:35:30.916654 badgie-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-04-14 23:35:27.000000 badgie-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3700 2023-04-14 23:35:30.916654 badgie-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2808 2023-04-14 23:35:27.000000 badgie-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 23:35:30.912654 badgie-0.3.0/badgie/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-14 23:35:28.000000 badgie-0.3.0/badgie/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 23:35:30.915654 badgie-0.3.0/badgie/badges/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/badges/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/badges/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      913 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/badges/brettops.py
+-rw-rw-rw-   0 root         (0) root         (0)     1257 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/badges/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)      511 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/badges/precommit.py
+-rw-rw-rw-   0 root         (0) root         (0)     4458 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      202 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      302 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1524 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 23:35:30.915654 badgie-0.3.0/badgie/providers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/providers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1432 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/providers/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      747 2023-04-14 23:35:27.000000 badgie-0.3.0/badgie/sources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 23:35:30.913653 badgie-0.3.0/badgie.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3700 2023-04-14 23:35:30.000000 badgie-0.3.0/badgie.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      559 2023-04-14 23:35:30.000000 badgie-0.3.0/badgie.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 23:35:30.000000 badgie-0.3.0/badgie.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-14 23:35:30.000000 badgie-0.3.0/badgie.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-14 23:35:30.000000 badgie-0.3.0/badgie.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-14 23:35:30.000000 badgie-0.3.0/badgie.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-04-14 23:35:30.916654 badgie-0.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1429 2023-04-14 23:35:28.000000 badgie-0.3.0/setup.py
```

### Comparing `badgie-0.2.0/LICENSE` & `badgie-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `badgie-0.2.0/PKG-INFO` & `badgie-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badgie
-Version: 0.2.0
+Version: 0.3.0
 Summary: Add all the badges with Badgie!
 Home-page: https://gitlab.com/brettops/tools/badgie
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
 Keywords: badge template markdown
 Platform: UNKNOWN
@@ -24,14 +24,15 @@
 License-File: LICENSE
 
 # Badgie
 
 <!-- BADGIE TIME -->
 
 [![brettops tool](https://img.shields.io/badge/brettops-tool-209cdf?labelColor=162d50)](https://brettops.io)
+[![latest release](https://img.shields.io/gitlab/v/release/brettops/tools/badgie)](https://gitlab.com/brettops/tools/badgie/-/releases)
 [![pipeline status](https://gitlab.com/brettops/tools/badgie/badges/main/pipeline.svg)](https://gitlab.com/brettops/tools/badgie/-/commits/main)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 <!-- END BADGIE TIME -->
 
 Add all the badges with Badgie!
 
@@ -131,19 +132,14 @@
 
 [![pipeline status](brettops/containers/verible/badges/main/pipeline.svg)](brettops/containers/verible/-/commits/main)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 <!-- END BADGIE TIME -->
 ```
 
-## Configuring Badgie
-
-When Badgie can't auto-determine a value, or when doing so _really_ doesn't make
-sense, Badgie can be configured to do something else.
-
 ## Caveats
 
 Badgie makes decisions on the assumption that you do sensible things with your
-repository structure. It does not try to work around bad practices and MRs that
+repository structure. It does not try to work around bad practices. MRs that
 encourage this will be rejected.
```

### Comparing `badgie-0.2.0/README.md` & `badgie-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Badgie
 
 <!-- BADGIE TIME -->
 
 [![brettops tool](https://img.shields.io/badge/brettops-tool-209cdf?labelColor=162d50)](https://brettops.io)
+[![latest release](https://img.shields.io/gitlab/v/release/brettops/tools/badgie)](https://gitlab.com/brettops/tools/badgie/-/releases)
 [![pipeline status](https://gitlab.com/brettops/tools/badgie/badges/main/pipeline.svg)](https://gitlab.com/brettops/tools/badgie/-/commits/main)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 <!-- END BADGIE TIME -->
 
 Add all the badges with Badgie!
 
@@ -106,17 +107,12 @@
 
 [![pipeline status](brettops/containers/verible/badges/main/pipeline.svg)](brettops/containers/verible/-/commits/main)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 <!-- END BADGIE TIME -->
 ```
 
-## Configuring Badgie
-
-When Badgie can't auto-determine a value, or when doing so _really_ doesn't make
-sense, Badgie can be configured to do something else.
-
 ## Caveats
 
 Badgie makes decisions on the assumption that you do sensible things with your
-repository structure. It does not try to work around bad practices and MRs that
+repository structure. It does not try to work around bad practices. MRs that
 encourage this will be rejected.
```

### Comparing `badgie-0.2.0/badgie/badges/_base.py` & `badgie-0.3.0/badgie/badges/_base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,42 @@
-import logging
+import sys
 from dataclasses import dataclass
 from typing import Optional
 
-from ..models import Remote
+from termcolor import colored
+
+from ..models import Project, Remote
 
 
 @dataclass(frozen=True)
 class Badge:
-    project_url: str
-    project_ref: str
+    project: Project
     remote: Optional[Remote] = None
 
     def __post_init__(self):
-        logging.info("add %s", self.__class__.name)
+        print(
+            colored(
+                "- adding a {name} badge".format(
+                    name=colored(self.__class__.name, "blue", attrs=["bold"])
+                )
+            ),
+            file=sys.stderr,
+        )
 
     def get_badge_image_url(self):
         raise NotImplementedError
 
     def get_link_title(self):
         try:
             return self.link_title
         except AttributeError:
             return ""
 
     def get_link_url(self):
-        return self.project_url
+        return self.project.url
 
     def get_markdown(self):
         return f"[![{self.get_link_title()}]({self.get_badge_image_url()})]({self.get_link_url()})"
 
 
 _BADGES = {}
```

### Comparing `badgie-0.2.0/badgie.egg-info/PKG-INFO` & `badgie-0.3.0/badgie.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badgie
-Version: 0.2.0
+Version: 0.3.0
 Summary: Add all the badges with Badgie!
 Home-page: https://gitlab.com/brettops/tools/badgie
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
 Keywords: badge template markdown
 Platform: UNKNOWN
@@ -24,14 +24,15 @@
 License-File: LICENSE
 
 # Badgie
 
 <!-- BADGIE TIME -->
 
 [![brettops tool](https://img.shields.io/badge/brettops-tool-209cdf?labelColor=162d50)](https://brettops.io)
+[![latest release](https://img.shields.io/gitlab/v/release/brettops/tools/badgie)](https://gitlab.com/brettops/tools/badgie/-/releases)
 [![pipeline status](https://gitlab.com/brettops/tools/badgie/badges/main/pipeline.svg)](https://gitlab.com/brettops/tools/badgie/-/commits/main)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 <!-- END BADGIE TIME -->
 
 Add all the badges with Badgie!
 
@@ -131,19 +132,14 @@
 
 [![pipeline status](brettops/containers/verible/badges/main/pipeline.svg)](brettops/containers/verible/-/commits/main)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 <!-- END BADGIE TIME -->
 ```
 
-## Configuring Badgie
-
-When Badgie can't auto-determine a value, or when doing so _really_ doesn't make
-sense, Badgie can be configured to do something else.
-
 ## Caveats
 
 Badgie makes decisions on the assumption that you do sensible things with your
-repository structure. It does not try to work around bad practices and MRs that
+repository structure. It does not try to work around bad practices. MRs that
 encourage this will be rejected.
```

### Comparing `badgie-0.2.0/setup.py` & `badgie-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
 # injected version
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 
 # markdown readme
 long_description = open("README.md").read()
 
 # read requirements from requirements.in
 install_requires = open("requirements.in").read().splitlines()
 
@@ -16,17 +16,18 @@
     author_email="brett@brettops.io",
     description="Add all the badges with Badgie!",
     license="MIT",
     url="https://gitlab.com/brettops/tools/badgie",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
+    package_data={"badgie": ["py.typed"]},
     entry_points={
         "console_scripts": [
-            "badgie = badgie.__main__:main",
+            "badgie = badgie.cli:main",
         ],
     },
     install_requires=install_requires,
     python_requires=">=3.9",
     keywords="badge template markdown",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
```

