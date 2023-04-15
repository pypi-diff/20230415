# Comparing `tmp/wheel_axle-0.0.6.dev20230415194546.tar.gz` & `tmp/wheel_axle-0.0.6.dev20230415195445.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wheel_axle-0.0.6.dev20230415194546.tar", last modified: Sat Apr 15 19:46:06 2023, max compression
+gzip compressed data, was "wheel_axle-0.0.6.dev20230415195445.tar", last modified: Sat Apr 15 19:55:06 2023, max compression
```

## Comparing `wheel_axle-0.0.6.dev20230415194546.tar` & `wheel_axle-0.0.6.dev20230415195445.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:46:06.345655 wheel_axle-0.0.6.dev20230415194546/
--rw-rw-r--   0 runner    (1001) docker     (123)       38 2023-04-15 19:46:00.000000 wheel_axle-0.0.6.dev20230415194546/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-15 19:46:06.345655 wheel_axle-0.0.6.dev20230415194546/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 19:46:06.345655 wheel_axle-0.0.6.dev20230415194546/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     6585 2023-04-15 19:46:00.000000 wheel_axle-0.0.6.dev20230415194546/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:46:06.345655 wheel_axle-0.0.6.dev20230415194546/wheel_axle/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:46:06.345655 wheel_axle-0.0.6.dev20230415194546/wheel_axle/bdist_axle/
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-04-15 19:46:00.000000 wheel_axle-0.0.6.dev20230415194546/wheel_axle/bdist_axle/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-04-15 19:46:00.000000 wheel_axle-0.0.6.dev20230415194546/wheel_axle/bdist_axle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-15 19:45:42.000000 wheel_axle-0.0.6.dev20230415194546/wheel_axle/bdist_axle/_file_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:46:06.345655 wheel_axle-0.0.6.dev20230415194546/wheel_axle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-15 19:46:06.000000 wheel_axle-0.0.6.dev20230415194546/wheel_axle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-15 19:46:06.000000 wheel_axle-0.0.6.dev20230415194546/wheel_axle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 19:46:06.000000 wheel_axle-0.0.6.dev20230415194546/wheel_axle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-15 19:46:06.000000 wheel_axle-0.0.6.dev20230415194546/wheel_axle.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 19:46:06.000000 wheel_axle-0.0.6.dev20230415194546/wheel_axle.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-15 19:46:06.000000 wheel_axle-0.0.6.dev20230415194546/wheel_axle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-15 19:46:06.000000 wheel_axle-0.0.6.dev20230415194546/wheel_axle.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 19:46:06.000000 wheel_axle-0.0.6.dev20230415194546/wheel_axle.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:55:06.769187 wheel_axle-0.0.6.dev20230415195445/
+-rw-rw-r--   0 runner    (1001) docker     (123)       38 2023-04-15 19:55:00.000000 wheel_axle-0.0.6.dev20230415195445/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-04-15 19:55:06.769187 wheel_axle-0.0.6.dev20230415195445/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 19:55:06.769187 wheel_axle-0.0.6.dev20230415195445/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6582 2023-04-15 19:55:00.000000 wheel_axle-0.0.6.dev20230415195445/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:55:06.769187 wheel_axle-0.0.6.dev20230415195445/wheel_axle/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:55:06.769187 wheel_axle-0.0.6.dev20230415195445/wheel_axle/bdist_axle/
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-04-15 19:55:00.000000 wheel_axle-0.0.6.dev20230415195445/wheel_axle/bdist_axle/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-04-15 19:55:00.000000 wheel_axle-0.0.6.dev20230415195445/wheel_axle/bdist_axle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-15 19:54:42.000000 wheel_axle-0.0.6.dev20230415195445/wheel_axle/bdist_axle/_file_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 19:55:06.769187 wheel_axle-0.0.6.dev20230415195445/wheel_axle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-04-15 19:55:06.000000 wheel_axle-0.0.6.dev20230415195445/wheel_axle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-15 19:55:06.000000 wheel_axle-0.0.6.dev20230415195445/wheel_axle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 19:55:06.000000 wheel_axle-0.0.6.dev20230415195445/wheel_axle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-15 19:55:06.000000 wheel_axle-0.0.6.dev20230415195445/wheel_axle.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 19:55:06.000000 wheel_axle-0.0.6.dev20230415195445/wheel_axle.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-15 19:55:06.000000 wheel_axle-0.0.6.dev20230415195445/wheel_axle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-15 19:55:06.000000 wheel_axle-0.0.6.dev20230415195445/wheel_axle.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 19:55:06.000000 wheel_axle-0.0.6.dev20230415195445/wheel_axle.egg-info/zip-safe
```

### Comparing `wheel_axle-0.0.6.dev20230415194546/PKG-INFO` & `wheel_axle-0.0.6.dev20230415195445/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wheel_axle
-Version: 0.0.6.dev20230415194546
+Version: 0.0.6.dev20230415195445
 Summary: Axle is Python wheel enhancement library
 Home-page: https://github.com/karellen/wheel-axle
 Author: Karellen, Inc.
 Author-email: supervisor@karellen.co
 Maintainer: Arcadiy Ivanov
 Maintainer-email: arcadiy@karellen.co
 License: Apache License, Version 2.0
@@ -33,17 +33,17 @@
 [![Gitter](https://img.shields.io/gitter/room/karellen/Lobby?logo=gitter)](https://app.gitter.im/#/room/#karellen_Lobby:gitter.im)
 [![Build Status](https://img.shields.io/github/actions/workflow/status/karellen/wheel-axle/build.yml?branch=master)](https://github.com/karellen/wheel-axle/actions/workflows/build.yml)
 [![Coverage Status](https://img.shields.io/coveralls/github/karellen/wheel-axle/master?logo=coveralls)](https://coveralls.io/r/karellen/wheel-axle?branch=master)
 
 [![Wheel Axle Version](https://img.shields.io/pypi/v/wheel-axle?logo=pypi)](https://pypi.org/project/wheel-axle/)
 [![Wheel Axle Python Versions](https://img.shields.io/pypi/pyversions/wheel-axle?logo=pypi)](https://pypi.org/project/wheel-axle/)
 
-[![Wheel Axle Downloads Per Day](https://img.shields.io/pypi/dd/wheel-axle?logo=pypi)](https://pypistats.org/packages/wheel-axle/)
-[![Wheel Axle Downloads Per Week](https://img.shields.io/pypi/dw/wheel-axle?logo=pypi)](https://pypistats.org/packages/wheel-axle/)
-[![Wheel Axle Downloads Per Month](https://img.shields.io/pypi/dm/wheel-axle?logo=pypi)](https://pypistats.org/packages/wheel-axle/)
+[![Wheel Axle Downloads Per Day](https://img.shields.io/pypi/dd/wheel-axle?logo=pypi)](https://pypistats.org/packages/wheel-axle)
+[![Wheel Axle Downloads Per Week](https://img.shields.io/pypi/dw/wheel-axle?logo=pypi)](https://pypistats.org/packages/wheel-axle)
+[![Wheel Axle Downloads Per Month](https://img.shields.io/pypi/dm/wheel-axle?logo=pypi)](https://pypistats.org/packages/wheel-axle)
 
 ## Problem
 
 1. `bdist_wheel` does not support symlinks.
 2. `bdist_wheel` does not support overwriting in a convenient way:
     * whether the distribution is pure-Python
     * distribution ABI tag
```

### Comparing `wheel_axle-0.0.6.dev20230415194546/setup.py` & `wheel_axle-0.0.6.dev20230415195445/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
         _install.run(self)
 
         self.post_install_script()
 
 if __name__ == '__main__':
     setup(
         name = 'wheel_axle',
-        version = '0.0.6.dev20230415194546',
+        version = '0.0.6.dev20230415195445',
         description = 'Axle is Python wheel enhancement library',
-        long_description = '# Wheel Axle - Python Wheel enhancement library\n\n[![Gitter](https://img.shields.io/gitter/room/karellen/Lobby?logo=gitter)](https://app.gitter.im/#/room/#karellen_Lobby:gitter.im)\n[![Build Status](https://img.shields.io/github/actions/workflow/status/karellen/wheel-axle/build.yml?branch=master)](https://github.com/karellen/wheel-axle/actions/workflows/build.yml)\n[![Coverage Status](https://img.shields.io/coveralls/github/karellen/wheel-axle/master?logo=coveralls)](https://coveralls.io/r/karellen/wheel-axle?branch=master)\n\n[![Wheel Axle Version](https://img.shields.io/pypi/v/wheel-axle?logo=pypi)](https://pypi.org/project/wheel-axle/)\n[![Wheel Axle Python Versions](https://img.shields.io/pypi/pyversions/wheel-axle?logo=pypi)](https://pypi.org/project/wheel-axle/)\n\n[![Wheel Axle Downloads Per Day](https://img.shields.io/pypi/dd/wheel-axle?logo=pypi)](https://pypistats.org/packages/wheel-axle/)\n[![Wheel Axle Downloads Per Week](https://img.shields.io/pypi/dw/wheel-axle?logo=pypi)](https://pypistats.org/packages/wheel-axle/)\n[![Wheel Axle Downloads Per Month](https://img.shields.io/pypi/dm/wheel-axle?logo=pypi)](https://pypistats.org/packages/wheel-axle/)\n\n## Problem\n\n1. `bdist_wheel` does not support symlinks.\n2. `bdist_wheel` does not support overwriting in a convenient way:\n    * whether the distribution is pure-Python\n    * distribution ABI tag\n    * Extend Python tag override capability\n\n## Solution\n\n**WARNING: THIS IS EXPERIMENTAL BETA SOFTWARE. THERE ARE NO WARRANTIES OF ANY KIND. USE AT YOUR OWN RISK.\nADDITIONAL INCLUDED DISCLAIMERS ALSO APPLY.**\n\nWheel-Axle (`Axle`, `bdist_axle`) is a drop-in replacement/augmentation utility for `wheel` (`bdist_wheel`)\nthat extends and builds spec-compliant wheels.\n\nDuring the build, `Axle` is able to capture and record symlinks in the following schema paths (locations):\n\n* purelib\n* platlib\n* scripts\n* headers\n* data\n\nAdditionally, `Axle` is able to customize the tags via additional command line options.\n\nWhile the generated wheel is fully spec-compliant, additional symlinks functionality is not possible without its\ncompanion library [Wheel Axle Runtime](https://github.com/karellen/wheel-axle-runtime). Thus, every wheel generated by\nthe `bdist_axle` automatically becomes dependent on `wheel-axle-runtime` that provides post-install logic required.\n\n## Implementation\n\nThe body of the library is as ugly and messy as `distutils`/`setuptools` are, and consists of, mainly, in\nhacking/overwriting various `setuptools` commands to detect, handle and record symlinks and their targets. Once that\nproblem is solved, the list of symlinks is recorded in the `.dist-info/symlinks.txt`\nin the following CSV format:\n\n1. symlink name\n2. symlink target\n3. a boolean (0 or 1) flag indicating whether the target is a directory\n\n**NOTE: Symlinks may be relative, absolute and/or broken. Symlink targets are recorded verbatim (even when broken) and\nare NOT otherwise interpreted. THIS IS INTENTIONAL. Please\nsee [Wheel Axle Runtime Security Notice](https://github.com/karellen/wheel-axle-runtime#security)\nfor additional information.**\n\nA special `<distribution name and version>.pth` file is also added to the distribution. When the wheel is installed\nthis `.pth` file triggers the post-install logic via\n[wheel-axle-runtime](https://github.com/karellen/wheel-axle-runtime).\n\n## Usage\n\n`python setup.py bdist_wheel <arguments>` can be replaced with `python setup.py bdist_axle <arguments>`. The replacement\nis drop-in.\n\nAdditional functionality is available via the following options:\n\n```commandline\n  --root-is-pure    set to manually override whether the wheel is\n                    pure (default: None)\n  --abi-tag         set to override ABI tag (default: None)\n```\n\nUsing `--python-tag`, `--root-is-pure` and `--abi-tag` allows you to create wheels that carry platform-dependent data\nwhile otherwise containing pure-Python libraries.\n',
+        long_description = '# Wheel Axle - Python Wheel enhancement library\n\n[![Gitter](https://img.shields.io/gitter/room/karellen/Lobby?logo=gitter)](https://app.gitter.im/#/room/#karellen_Lobby:gitter.im)\n[![Build Status](https://img.shields.io/github/actions/workflow/status/karellen/wheel-axle/build.yml?branch=master)](https://github.com/karellen/wheel-axle/actions/workflows/build.yml)\n[![Coverage Status](https://img.shields.io/coveralls/github/karellen/wheel-axle/master?logo=coveralls)](https://coveralls.io/r/karellen/wheel-axle?branch=master)\n\n[![Wheel Axle Version](https://img.shields.io/pypi/v/wheel-axle?logo=pypi)](https://pypi.org/project/wheel-axle/)\n[![Wheel Axle Python Versions](https://img.shields.io/pypi/pyversions/wheel-axle?logo=pypi)](https://pypi.org/project/wheel-axle/)\n\n[![Wheel Axle Downloads Per Day](https://img.shields.io/pypi/dd/wheel-axle?logo=pypi)](https://pypistats.org/packages/wheel-axle)\n[![Wheel Axle Downloads Per Week](https://img.shields.io/pypi/dw/wheel-axle?logo=pypi)](https://pypistats.org/packages/wheel-axle)\n[![Wheel Axle Downloads Per Month](https://img.shields.io/pypi/dm/wheel-axle?logo=pypi)](https://pypistats.org/packages/wheel-axle)\n\n## Problem\n\n1. `bdist_wheel` does not support symlinks.\n2. `bdist_wheel` does not support overwriting in a convenient way:\n    * whether the distribution is pure-Python\n    * distribution ABI tag\n    * Extend Python tag override capability\n\n## Solution\n\n**WARNING: THIS IS EXPERIMENTAL BETA SOFTWARE. THERE ARE NO WARRANTIES OF ANY KIND. USE AT YOUR OWN RISK.\nADDITIONAL INCLUDED DISCLAIMERS ALSO APPLY.**\n\nWheel-Axle (`Axle`, `bdist_axle`) is a drop-in replacement/augmentation utility for `wheel` (`bdist_wheel`)\nthat extends and builds spec-compliant wheels.\n\nDuring the build, `Axle` is able to capture and record symlinks in the following schema paths (locations):\n\n* purelib\n* platlib\n* scripts\n* headers\n* data\n\nAdditionally, `Axle` is able to customize the tags via additional command line options.\n\nWhile the generated wheel is fully spec-compliant, additional symlinks functionality is not possible without its\ncompanion library [Wheel Axle Runtime](https://github.com/karellen/wheel-axle-runtime). Thus, every wheel generated by\nthe `bdist_axle` automatically becomes dependent on `wheel-axle-runtime` that provides post-install logic required.\n\n## Implementation\n\nThe body of the library is as ugly and messy as `distutils`/`setuptools` are, and consists of, mainly, in\nhacking/overwriting various `setuptools` commands to detect, handle and record symlinks and their targets. Once that\nproblem is solved, the list of symlinks is recorded in the `.dist-info/symlinks.txt`\nin the following CSV format:\n\n1. symlink name\n2. symlink target\n3. a boolean (0 or 1) flag indicating whether the target is a directory\n\n**NOTE: Symlinks may be relative, absolute and/or broken. Symlink targets are recorded verbatim (even when broken) and\nare NOT otherwise interpreted. THIS IS INTENTIONAL. Please\nsee [Wheel Axle Runtime Security Notice](https://github.com/karellen/wheel-axle-runtime#security)\nfor additional information.**\n\nA special `<distribution name and version>.pth` file is also added to the distribution. When the wheel is installed\nthis `.pth` file triggers the post-install logic via\n[wheel-axle-runtime](https://github.com/karellen/wheel-axle-runtime).\n\n## Usage\n\n`python setup.py bdist_wheel <arguments>` can be replaced with `python setup.py bdist_axle <arguments>`. The replacement\nis drop-in.\n\nAdditional functionality is available via the following options:\n\n```commandline\n  --root-is-pure    set to manually override whether the wheel is\n                    pure (default: None)\n  --abi-tag         set to override ABI tag (default: None)\n```\n\nUsing `--python-tag`, `--root-is-pure` and `--abi-tag` allows you to create wheels that carry platform-dependent data\nwhile otherwise containing pure-Python libraries.\n',
         long_description_content_type = 'text/markdown',
         classifiers = [
             'License :: OSI Approved :: Apache Software License',
             'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.9',
             'Programming Language :: Python :: 3.10',
```

### Comparing `wheel_axle-0.0.6.dev20230415194546/wheel_axle/bdist_axle/LICENSE` & `wheel_axle-0.0.6.dev20230415195445/wheel_axle/bdist_axle/LICENSE`

 * *Files identical despite different names*

### Comparing `wheel_axle-0.0.6.dev20230415194546/wheel_axle/bdist_axle/__init__.py` & `wheel_axle-0.0.6.dev20230415195445/wheel_axle/bdist_axle/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from wheel.bdist_wheel import bdist_wheel as _bdist_wheel, python_tag
 from wheel.vendored.packaging import tags
 
 from wheel_axle.bdist_axle._file_utils import copy_link, copy_tree
 from wheel_axle.runtime._symlinks import write_symlinks_file
 from wheel_axle.runtime.constants import AXLE_LOCK_FILE, SYMLINKS_FILE
 
-__version__ = "0.0.6.dev20230415194546"
+__version__ = "0.0.6.dev20230415195445"
 WHEEL_AXLE_DEPENDENCY = "wheel-axle-runtime<1.0"
 
 
 class SymlinkAwareCommmand(Command):
     def initialize_options(self):
         super().initialize_options()
         self._symlinks = []
```

### Comparing `wheel_axle-0.0.6.dev20230415194546/wheel_axle/bdist_axle/_file_utils.py` & `wheel_axle-0.0.6.dev20230415195445/wheel_axle/bdist_axle/_file_utils.py`

 * *Files identical despite different names*

### Comparing `wheel_axle-0.0.6.dev20230415194546/wheel_axle.egg-info/PKG-INFO` & `wheel_axle-0.0.6.dev20230415195445/wheel_axle.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wheel-axle
-Version: 0.0.6.dev20230415194546
+Version: 0.0.6.dev20230415195445
 Summary: Axle is Python wheel enhancement library
 Home-page: https://github.com/karellen/wheel-axle
 Author: Karellen, Inc.
 Author-email: supervisor@karellen.co
 Maintainer: Arcadiy Ivanov
 Maintainer-email: arcadiy@karellen.co
 License: Apache License, Version 2.0
@@ -33,17 +33,17 @@
 [![Gitter](https://img.shields.io/gitter/room/karellen/Lobby?logo=gitter)](https://app.gitter.im/#/room/#karellen_Lobby:gitter.im)
 [![Build Status](https://img.shields.io/github/actions/workflow/status/karellen/wheel-axle/build.yml?branch=master)](https://github.com/karellen/wheel-axle/actions/workflows/build.yml)
 [![Coverage Status](https://img.shields.io/coveralls/github/karellen/wheel-axle/master?logo=coveralls)](https://coveralls.io/r/karellen/wheel-axle?branch=master)
 
 [![Wheel Axle Version](https://img.shields.io/pypi/v/wheel-axle?logo=pypi)](https://pypi.org/project/wheel-axle/)
 [![Wheel Axle Python Versions](https://img.shields.io/pypi/pyversions/wheel-axle?logo=pypi)](https://pypi.org/project/wheel-axle/)
 
-[![Wheel Axle Downloads Per Day](https://img.shields.io/pypi/dd/wheel-axle?logo=pypi)](https://pypistats.org/packages/wheel-axle/)
-[![Wheel Axle Downloads Per Week](https://img.shields.io/pypi/dw/wheel-axle?logo=pypi)](https://pypistats.org/packages/wheel-axle/)
-[![Wheel Axle Downloads Per Month](https://img.shields.io/pypi/dm/wheel-axle?logo=pypi)](https://pypistats.org/packages/wheel-axle/)
+[![Wheel Axle Downloads Per Day](https://img.shields.io/pypi/dd/wheel-axle?logo=pypi)](https://pypistats.org/packages/wheel-axle)
+[![Wheel Axle Downloads Per Week](https://img.shields.io/pypi/dw/wheel-axle?logo=pypi)](https://pypistats.org/packages/wheel-axle)
+[![Wheel Axle Downloads Per Month](https://img.shields.io/pypi/dm/wheel-axle?logo=pypi)](https://pypistats.org/packages/wheel-axle)
 
 ## Problem
 
 1. `bdist_wheel` does not support symlinks.
 2. `bdist_wheel` does not support overwriting in a convenient way:
     * whether the distribution is pure-Python
     * distribution ABI tag
```

