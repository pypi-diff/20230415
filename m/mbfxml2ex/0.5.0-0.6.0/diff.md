# Comparing `tmp/mbfxml2ex-0.5.0.tar.gz` & `tmp/mbfxml2ex-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbfxml2ex-0.5.0.tar", last modified: Thu Sep 29 08:47:51 2022, max compression
+gzip compressed data, was "mbfxml2ex-0.6.0.tar", last modified: Sat Apr 15 01:54:12 2023, max compression
```

## Comparing `mbfxml2ex-0.5.0.tar` & `mbfxml2ex-0.6.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-09-29 08:47:51.408048 mbfxml2ex-0.5.0/
--rw-r--r--   0 hsor001  (1210695619) 1403514002    11357 2022-09-28 14:14:25.000000 mbfxml2ex-0.5.0/LICENSE
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1500 2022-09-29 08:47:51.407741 mbfxml2ex-0.5.0/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002      842 2022-09-29 08:44:51.000000 mbfxml2ex-0.5.0/README.rst
--rw-r--r--   0 hsor001  (1210695619) 1403514002       38 2022-09-29 08:47:51.408197 mbfxml2ex-0.5.0/setup.cfg
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1844 2022-09-29 08:12:42.000000 mbfxml2ex-0.5.0/setup.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-09-29 08:47:51.395980 mbfxml2ex-0.5.0/src/
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-09-29 08:47:51.403070 mbfxml2ex-0.5.0/src/mbfxml2ex/
--rw-r--r--   0 hsor001  (1210695619) 1403514002       22 2022-09-29 08:47:20.000000 mbfxml2ex-0.5.0/src/mbfxml2ex/__init__.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     4582 2022-09-28 14:14:25.000000 mbfxml2ex-0.5.0/src/mbfxml2ex/app.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    14239 2022-09-28 14:14:25.000000 mbfxml2ex-0.5.0/src/mbfxml2ex/classes.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002      396 2022-09-28 14:14:25.000000 mbfxml2ex-0.5.0/src/mbfxml2ex/conversions.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002      279 2022-09-28 14:14:25.000000 mbfxml2ex-0.5.0/src/mbfxml2ex/exceptions.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    12063 2022-09-28 14:14:25.000000 mbfxml2ex-0.5.0/src/mbfxml2ex/parsers.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     4528 2022-09-28 14:14:25.000000 mbfxml2ex-0.5.0/src/mbfxml2ex/templates.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002      967 2022-09-28 14:14:25.000000 mbfxml2ex-0.5.0/src/mbfxml2ex/utilities.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    17170 2022-09-29 08:02:42.000000 mbfxml2ex-0.5.0/src/mbfxml2ex/zinc.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2022-09-29 08:47:51.407198 mbfxml2ex-0.5.0/src/mbfxml2ex.egg-info/
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1500 2022-09-29 08:47:51.000000 mbfxml2ex-0.5.0/src/mbfxml2ex.egg-info/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002      517 2022-09-29 08:47:51.000000 mbfxml2ex-0.5.0/src/mbfxml2ex.egg-info/SOURCES.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2022-09-29 08:47:51.000000 mbfxml2ex-0.5.0/src/mbfxml2ex.egg-info/dependency_links.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002       59 2022-09-29 08:47:51.000000 mbfxml2ex-0.5.0/src/mbfxml2ex.egg-info/entry_points.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2022-09-28 14:31:10.000000 mbfxml2ex-0.5.0/src/mbfxml2ex.egg-info/not-zip-safe
--rw-r--r--   0 hsor001  (1210695619) 1403514002       77 2022-09-29 08:47:51.000000 mbfxml2ex-0.5.0/src/mbfxml2ex.egg-info/requires.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002       10 2022-09-29 08:47:51.000000 mbfxml2ex-0.5.0/src/mbfxml2ex.egg-info/top_level.txt
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-15 01:54:12.649579 mbfxml2ex-0.6.0/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    11357 2020-11-16 23:57:54.000000 mbfxml2ex-0.6.0/LICENSE
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     1905 2023-04-15 01:54:12.649241 mbfxml2ex-0.6.0/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      839 2023-04-15 01:52:52.000000 mbfxml2ex-0.6.0/README.rst
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       38 2023-04-15 01:54:12.649666 mbfxml2ex-0.6.0/setup.cfg
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     1841 2023-04-15 01:52:52.000000 mbfxml2ex-0.6.0/setup.py
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-15 01:54:12.639069 mbfxml2ex-0.6.0/src/
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-15 01:54:12.644934 mbfxml2ex-0.6.0/src/mbfxml2ex/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       22 2023-04-15 01:52:52.000000 mbfxml2ex-0.6.0/src/mbfxml2ex/__init__.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     4582 2022-08-24 04:27:06.000000 mbfxml2ex-0.6.0/src/mbfxml2ex/app.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    14236 2023-04-04 10:04:31.000000 mbfxml2ex-0.6.0/src/mbfxml2ex/classes.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      396 2021-01-19 04:46:50.000000 mbfxml2ex-0.6.0/src/mbfxml2ex/conversions.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      279 2021-01-19 03:54:40.000000 mbfxml2ex-0.6.0/src/mbfxml2ex/exceptions.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    12063 2022-08-24 03:39:52.000000 mbfxml2ex-0.6.0/src/mbfxml2ex/parsers.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     4528 2020-11-26 23:56:34.000000 mbfxml2ex-0.6.0/src/mbfxml2ex/templates.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      967 2021-01-19 06:27:17.000000 mbfxml2ex-0.6.0/src/mbfxml2ex/utilities.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    17146 2023-04-15 01:43:54.000000 mbfxml2ex-0.6.0/src/mbfxml2ex/zinc.py
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-15 01:54:12.648829 mbfxml2ex-0.6.0/src/mbfxml2ex.egg-info/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     1905 2023-04-15 01:54:12.000000 mbfxml2ex-0.6.0/src/mbfxml2ex.egg-info/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      517 2023-04-15 01:54:12.000000 mbfxml2ex-0.6.0/src/mbfxml2ex.egg-info/SOURCES.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-04-15 01:54:12.000000 mbfxml2ex-0.6.0/src/mbfxml2ex.egg-info/dependency_links.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       59 2023-04-15 01:54:12.000000 mbfxml2ex-0.6.0/src/mbfxml2ex.egg-info/entry_points.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2020-11-27 00:32:53.000000 mbfxml2ex-0.6.0/src/mbfxml2ex.egg-info/not-zip-safe
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       71 2023-04-15 01:54:12.000000 mbfxml2ex-0.6.0/src/mbfxml2ex.egg-info/requires.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       10 2023-04-15 01:54:12.000000 mbfxml2ex-0.6.0/src/mbfxml2ex.egg-info/top_level.txt
```

### Comparing `mbfxml2ex-0.5.0/LICENSE` & `mbfxml2ex-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mbfxml2ex-0.5.0/PKG-INFO` & `mbfxml2ex-0.6.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,73 +1,70 @@
 Metadata-Version: 2.1
 Name: mbfxml2ex
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python client for generating Ex format model descriptions from MBF XML.
-Home-page: https://github.com/hsorby/mbfxml2ex
+Home-page: https://github.com/ABI-Software/mbfxml2ex
 Author: Auckland Bioengineering Institute
 Author-email: h.sorby@auckland.ac.nz
 License: Apache Software License
-Keywords: MBF OpenCMISS-Zinc
+Description: 
+        MBF XML 2 Ex
+        ============
+        
+        This program converts MBF XML to Ex format suitable for CMLibs-Zinc.
+        
+        
+        Install
+        -------
+        
+        ::
+        
+          pip install mbfxml2ex
+        
+        Usage
+        -----
+        
+        ::
+        
+          mbfxml2exconverter /path/to/input.xml
+        
+        For more information use the help::
+        
+          mbfxml2exconverter --help
+        
+        Developing
+        ----------
+        
+        When developing install the required packages for running the tests with::
+        
+          pip install .[test]
+        
+        Then run the tests with::
+        
+          nosetests
+        
+        from the repository root directory.
+        
+        To see the coverage statistics for the package run::
+        
+          nosetests --with-coverage --cover-package=mbfxml2ex
+        
+        For a nice HTML rendering of the coverage statistics run::
+        
+          nosetests --with-coverage --cover-package=mbfxml2ex --cover-html
+        
+        To view the HTML coverage output::
+        
+          cd cover
+          python -m http.server 9432
+        
+        Then, in a web browser navigate to http://localhost:9432
+        
+Keywords: MBF CMLibs Zinc
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Utilities
 Description-Content-Type: text/x-rst
 Provides-Extra: test
-License-File: LICENSE
-
-
-MBF XML 2 Ex
-============
-
-This program converts MBF XML to Ex format suitable for OpenCMISS-Zinc.
-
-
-Install
--------
-
-::
-
-  pip install mbfxml2ex
-
-Usage
------
-
-::
-
-  mbfxml2exconverter /path/to/input.xml
-
-For more information use the help::
-
-  mbfxml2exconverter --help
-
-Developing
-----------
-
-When developing install the required packages for running the tests with::
-
-  pip install .[test]
-
-Then run the tests with::
-
-  nosetests
-
-from the repository root directory.
-
-To see the coverage statistics for the package run::
-
-  nosetests --with-coverage --cover-package=mbfxml2ex
-
-For a nice HTML rendering of the coverage statistics run::
-
-  nosetests --with-coverage --cover-package=mbfxml2ex --cover-html
-
-To view the HTML coverage output::
-
-  cd cover
-  python -m http.server 9432
-
-Then, in a web browser navigate to http://localhost:9432
-
-
```

### Comparing `mbfxml2ex-0.5.0/README.rst` & `mbfxml2ex-0.6.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 MBF XML 2 Ex
 ============
 
-This program converts MBF XML to Ex format suitable for OpenCMISS-Zinc.
+This program converts MBF XML to Ex format suitable for CMLibs-Zinc.
 
 
 Install
 -------
 
 ::
```

### Comparing `mbfxml2ex-0.5.0/setup.py` & `mbfxml2ex-0.6.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 if not version:
     raise RuntimeError('Cannot find version information')
 
 # Get the long description from the README file
 with open(os.path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
-dependencies = ['opencmiss.zinc >= 3.5.1', 'opencmiss.utils >= 0.4.0']
+dependencies = ['cmlibs.zinc >= 4.0.0', 'cmlibs.utils >= 0.4.0']
 
 test_deps = [
     'coverage',
     'nose',
     'packaging',
 ]
 extras = {
@@ -48,16 +48,16 @@
     extras_require=extras,
     entry_points={
         'console_scripts': [
             'mbfxml2exconverter=mbfxml2ex.app:main',
         ]
     },
     license="Apache Software License",
-    keywords="MBF OpenCMISS-Zinc",
-    url="https://github.com/hsorby/mbfxml2ex",
+    keywords="MBF CMLibs Zinc",
+    url="https://github.com/ABI-Software/mbfxml2ex",
     download_url="",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering :: Medical Science Apps.",
         "Topic :: Utilities",
```

### Comparing `mbfxml2ex-0.5.0/src/mbfxml2ex/app.py` & `mbfxml2ex-0.6.0/src/mbfxml2ex/app.py`

 * *Files identical despite different names*

### Comparing `mbfxml2ex-0.5.0/src/mbfxml2ex/classes.py` & `mbfxml2ex-0.6.0/src/mbfxml2ex/classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import itertools
 
-from opencmiss.utils.zinc.general import AbstractNodeDataObject
+from cmlibs.utils.zinc.general import AbstractNodeDataObject
 
 from mbfxml2ex.conversions import hex_to_rgb
 from mbfxml2ex.exceptions import MBFImagesException
 
 
 class MBFPoint(AbstractNodeDataObject):
```

### Comparing `mbfxml2ex-0.5.0/src/mbfxml2ex/parsers.py` & `mbfxml2ex-0.6.0/src/mbfxml2ex/parsers.py`

 * *Files identical despite different names*

### Comparing `mbfxml2ex-0.5.0/src/mbfxml2ex/templates.py` & `mbfxml2ex-0.6.0/src/mbfxml2ex/templates.py`

 * *Files identical despite different names*

### Comparing `mbfxml2ex-0.5.0/src/mbfxml2ex/utilities.py` & `mbfxml2ex-0.6.0/src/mbfxml2ex/utilities.py`

 * *Files identical despite different names*

### Comparing `mbfxml2ex-0.5.0/src/mbfxml2ex/zinc.py` & `mbfxml2ex-0.6.0/src/mbfxml2ex/zinc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from opencmiss.utils.zinc.finiteelement import create_cube_element
-from opencmiss.zinc.context import Context
-from opencmiss.zinc.element import Element
-from opencmiss.zinc.element import Elementbasis
-from opencmiss.zinc.field import FieldGroup
+from cmlibs.utils.zinc.finiteelement import create_cube_element
+from cmlibs.zinc.context import Context
+from cmlibs.zinc.element import Element
+from cmlibs.zinc.element import Elementbasis
+from cmlibs.zinc.field import FieldGroup
 
-from opencmiss.utils.zinc.field import create_field_finite_element, create_field_coordinates, find_or_create_field_group
-from opencmiss.utils.zinc.general import create_node as create_zinc_node
-from opencmiss.utils.zinc.general import ChangeManager
+from cmlibs.utils.zinc.field import create_field_finite_element, create_field_coordinates, find_or_create_field_group
+from cmlibs.utils.zinc.general import create_node as create_zinc_node
+from cmlibs.utils.zinc.general import ChangeManager
 
 from mbfxml2ex.classes import MBFPropertyVolumeRLE, MBFPropertyPunctum, MBFPropertySet, get_text_properties
 from mbfxml2ex.exceptions import MissingImplementationException, MBFDataException
 from mbfxml2ex.utilities import extract_vessel_node_locations
 from mbfxml2ex.templates import field_header_3d_template, grid_field_3d_template, field_data_template
 
 node_id = 0
```

### Comparing `mbfxml2ex-0.5.0/src/mbfxml2ex.egg-info/PKG-INFO` & `mbfxml2ex-0.6.0/src/mbfxml2ex.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,73 +1,70 @@
 Metadata-Version: 2.1
 Name: mbfxml2ex
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python client for generating Ex format model descriptions from MBF XML.
-Home-page: https://github.com/hsorby/mbfxml2ex
+Home-page: https://github.com/ABI-Software/mbfxml2ex
 Author: Auckland Bioengineering Institute
 Author-email: h.sorby@auckland.ac.nz
 License: Apache Software License
-Keywords: MBF OpenCMISS-Zinc
+Description: 
+        MBF XML 2 Ex
+        ============
+        
+        This program converts MBF XML to Ex format suitable for CMLibs-Zinc.
+        
+        
+        Install
+        -------
+        
+        ::
+        
+          pip install mbfxml2ex
+        
+        Usage
+        -----
+        
+        ::
+        
+          mbfxml2exconverter /path/to/input.xml
+        
+        For more information use the help::
+        
+          mbfxml2exconverter --help
+        
+        Developing
+        ----------
+        
+        When developing install the required packages for running the tests with::
+        
+          pip install .[test]
+        
+        Then run the tests with::
+        
+          nosetests
+        
+        from the repository root directory.
+        
+        To see the coverage statistics for the package run::
+        
+          nosetests --with-coverage --cover-package=mbfxml2ex
+        
+        For a nice HTML rendering of the coverage statistics run::
+        
+          nosetests --with-coverage --cover-package=mbfxml2ex --cover-html
+        
+        To view the HTML coverage output::
+        
+          cd cover
+          python -m http.server 9432
+        
+        Then, in a web browser navigate to http://localhost:9432
+        
+Keywords: MBF CMLibs Zinc
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Utilities
 Description-Content-Type: text/x-rst
 Provides-Extra: test
-License-File: LICENSE
-
-
-MBF XML 2 Ex
-============
-
-This program converts MBF XML to Ex format suitable for OpenCMISS-Zinc.
-
-
-Install
--------
-
-::
-
-  pip install mbfxml2ex
-
-Usage
------
-
-::
-
-  mbfxml2exconverter /path/to/input.xml
-
-For more information use the help::
-
-  mbfxml2exconverter --help
-
-Developing
-----------
-
-When developing install the required packages for running the tests with::
-
-  pip install .[test]
-
-Then run the tests with::
-
-  nosetests
-
-from the repository root directory.
-
-To see the coverage statistics for the package run::
-
-  nosetests --with-coverage --cover-package=mbfxml2ex
-
-For a nice HTML rendering of the coverage statistics run::
-
-  nosetests --with-coverage --cover-package=mbfxml2ex --cover-html
-
-To view the HTML coverage output::
-
-  cd cover
-  python -m http.server 9432
-
-Then, in a web browser navigate to http://localhost:9432
-
-
```

### Comparing `mbfxml2ex-0.5.0/src/mbfxml2ex.egg-info/SOURCES.txt` & `mbfxml2ex-0.6.0/src/mbfxml2ex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

