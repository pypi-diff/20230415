# Comparing `tmp/SPLayout-0.4.4.tar.gz` & `tmp/SPLayout-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SPLayout-0.4.4.tar", last modified: Fri Apr 14 12:44:47 2023, max compression
+gzip compressed data, was "dist\SPLayout-0.4.5.tar", last modified: Sat Apr 15 14:29:30 2023, max compression
```

## Comparing `SPLayout-0.4.4.tar` & `SPLayout-0.4.5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 12:44:47.000000 SPLayout-0.4.4/
--rw-rw-rw-   0        0        0     2146 2023-04-14 12:44:47.000000 SPLayout-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     2433 2023-02-23 14:51:36.000000 SPLayout-0.4.4/README.md
--rw-rw-rw-   0        0        0     1473 2023-02-23 14:51:44.000000 SPLayout-0.4.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-14 12:44:47.000000 SPLayout-0.4.4/SPLayout.egg-info/
--rw-rw-rw-   0        0        0     2146 2023-04-14 12:44:47.000000 SPLayout-0.4.4/SPLayout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1491 2023-04-14 12:44:47.000000 SPLayout-0.4.4/SPLayout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 12:44:47.000000 SPLayout-0.4.4/SPLayout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-14 12:44:47.000000 SPLayout-0.4.4/SPLayout.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-14 12:44:47.000000 SPLayout-0.4.4/SPLayout.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 12:44:47.000000 SPLayout-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0      687 2023-02-23 14:06:17.000000 SPLayout-0.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 12:44:47.000000 SPLayout-0.4.4/splayout/
--rw-rw-rw-   0        0        0     1987 2023-04-14 12:44:18.000000 SPLayout-0.4.4/splayout/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 12:44:47.000000 SPLayout-0.4.4/splayout/adjointmethod/
--rw-rw-rw-   0        0        0      293 2023-02-24 04:21:26.000000 SPLayout-0.4.4/splayout/adjointmethod/__init__.py
--rw-rw-rw-   0        0        0    10984 2023-02-23 12:33:21.000000 SPLayout-0.4.4/splayout/adjointmethod/adjointshapeopt.py
--rw-rw-rw-   0        0        0    10647 2023-02-24 04:32:00.000000 SPLayout-0.4.4/splayout/adjointmethod/adjointtopologyopt.py
--rw-rw-rw-   0        0        0    10586 2023-02-23 12:35:47.000000 SPLayout-0.4.4/splayout/adjointmethod/shaperegion2d.py
--rw-rw-rw-   0        0        0    10652 2023-02-23 12:35:57.000000 SPLayout-0.4.4/splayout/adjointmethod/shaperegion3d.py
--rw-rw-rw-   0        0        0    11374 2023-02-23 12:36:38.000000 SPLayout-0.4.4/splayout/adjointmethod/topologyregion2d.py
--rw-rw-rw-   0        0        0    11149 2023-02-24 02:38:35.000000 SPLayout-0.4.4/splayout/adjointmethod/topologyregion3d.py
-drwxrwxrwx   0        0        0        0 2023-04-14 12:44:47.000000 SPLayout-0.4.4/splayout/algorithms/
--rw-rw-rw-   0        0        0      312 2023-02-23 13:06:11.000000 SPLayout-0.4.4/splayout/algorithms/__init__.py
--rw-rw-rw-   0        0        0     5781 2022-01-04 05:22:28.000000 SPLayout-0.4.4/splayout/algorithms/binarybatalgorithm.py
--rw-rw-rw-   0        0        0     6360 2022-01-04 06:04:34.000000 SPLayout-0.4.4/splayout/algorithms/binarygeneticalgorithm.py
--rw-rw-rw-   0        0        0     5831 2022-01-04 06:03:59.000000 SPLayout-0.4.4/splayout/algorithms/binaryparticleswarmalgorithm.py
--rw-rw-rw-   0        0        0     4305 2023-02-23 12:22:49.000000 SPLayout-0.4.4/splayout/algorithms/directbinarysearchalgorithm.py
--rw-rw-rw-   0        0        0     7333 2023-02-23 11:24:29.000000 SPLayout-0.4.4/splayout/algorithms/particleswarmalgorithm.py
-drwxrwxrwx   0        0        0        0 2023-04-14 12:44:47.000000 SPLayout-0.4.4/splayout/components/
--rw-rw-rw-   0        0        0     3728 2023-02-23 12:38:12.000000 SPLayout-0.4.4/splayout/components/AEMDgrating.py
--rw-rw-rw-   0        0        0      714 2023-02-23 13:44:58.000000 SPLayout-0.4.4/splayout/components/__init__.py
--rw-rw-rw-   0        0        0     4403 2023-02-23 12:38:42.000000 SPLayout-0.4.4/splayout/components/bend.py
--rw-rw-rw-   0        0        0     9026 2023-02-23 12:39:10.000000 SPLayout-0.4.4/splayout/components/doubleconnector.py
--rw-rw-rw-   0        0        0     6092 2023-02-23 12:42:22.000000 SPLayout-0.4.4/splayout/components/filledpattern.py
--rw-rw-rw-   0        0        0    49359 2023-02-23 12:42:22.000000 SPLayout-0.4.4/splayout/components/microring.py
--rw-rw-rw-   0        0        0    21403 2023-02-23 12:42:22.000000 SPLayout-0.4.4/splayout/components/pixelsregion.py
--rw-rw-rw-   0        0        0     7433 2023-02-23 12:41:22.000000 SPLayout-0.4.4/splayout/components/polygon.py
--rw-rw-rw-   0        0        0    14219 2023-02-23 12:42:22.000000 SPLayout-0.4.4/splayout/components/quarbend.py
--rw-rw-rw-   0        0        0    18098 2023-02-23 12:42:22.000000 SPLayout-0.4.4/splayout/components/sbend.py
--rw-rw-rw-   0        0        0    13136 2023-02-23 12:41:22.000000 SPLayout-0.4.4/splayout/components/selfdefinecomponent.py
--rw-rw-rw-   0        0        0    28052 2023-02-23 12:43:30.000000 SPLayout-0.4.4/splayout/components/simpleasymmetricdirectionalcoupler.py
--rw-rw-rw-   0        0        0     7270 2023-02-23 12:41:22.000000 SPLayout-0.4.4/splayout/components/slowlyvaryingtaper.py
--rw-rw-rw-   0        0        0     6668 2023-02-23 14:27:24.000000 SPLayout-0.4.4/splayout/components/taper.py
--rw-rw-rw-   0        0        0     1269 2023-02-23 12:41:22.000000 SPLayout-0.4.4/splayout/components/text.py
--rw-rw-rw-   0        0        0     8908 2023-02-23 12:42:22.000000 SPLayout-0.4.4/splayout/components/waveguide.py
-drwxrwxrwx   0        0        0        0 2023-04-14 12:44:47.000000 SPLayout-0.4.4/splayout/lumericalcommun/
--rw-rw-rw-   0        0        0       72 2023-02-23 12:26:37.000000 SPLayout-0.4.4/splayout/lumericalcommun/__init__.py
--rw-rw-rw-   0        0        0    75510 2023-04-14 12:41:11.000000 SPLayout-0.4.4/splayout/lumericalcommun/fdtdapi.py
--rw-rw-rw-   0        0        0    44213 2023-02-23 12:42:48.000000 SPLayout-0.4.4/splayout/lumericalcommun/modeapi.py
-drwxrwxrwx   0        0        0        0 2023-04-14 12:44:47.000000 SPLayout-0.4.4/splayout/utils/
--rw-rw-rw-   0        0        0       20 2023-02-23 12:27:14.000000 SPLayout-0.4.4/splayout/utils/__init__.py
--rw-rw-rw-   0        0        0     7931 2023-02-23 12:43:16.000000 SPLayout-0.4.4/splayout/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-15 14:29:30.000000 SPLayout-0.4.5/
+-rw-rw-rw-   0        0        0     2146 2023-04-15 14:29:30.000000 SPLayout-0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2433 2023-02-23 14:51:36.000000 SPLayout-0.4.5/README.md
+-rw-rw-rw-   0        0        0     1473 2023-02-23 14:51:44.000000 SPLayout-0.4.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-15 14:29:30.000000 SPLayout-0.4.5/SPLayout.egg-info/
+-rw-rw-rw-   0        0        0     2146 2023-04-15 14:29:30.000000 SPLayout-0.4.5/SPLayout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1491 2023-04-15 14:29:30.000000 SPLayout-0.4.5/SPLayout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 14:29:30.000000 SPLayout-0.4.5/SPLayout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-15 14:29:30.000000 SPLayout-0.4.5/SPLayout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-15 14:29:30.000000 SPLayout-0.4.5/SPLayout.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 14:29:30.000000 SPLayout-0.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      687 2023-02-23 14:06:17.000000 SPLayout-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 14:29:30.000000 SPLayout-0.4.5/splayout/
+-rw-rw-rw-   0        0        0     1987 2023-04-15 14:27:55.000000 SPLayout-0.4.5/splayout/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 14:29:30.000000 SPLayout-0.4.5/splayout/adjointmethod/
+-rw-rw-rw-   0        0        0      293 2023-02-24 04:21:26.000000 SPLayout-0.4.5/splayout/adjointmethod/__init__.py
+-rw-rw-rw-   0        0        0    10984 2023-02-23 12:33:21.000000 SPLayout-0.4.5/splayout/adjointmethod/adjointshapeopt.py
+-rw-rw-rw-   0        0        0    10647 2023-02-24 04:32:00.000000 SPLayout-0.4.5/splayout/adjointmethod/adjointtopologyopt.py
+-rw-rw-rw-   0        0        0    10586 2023-02-23 12:35:47.000000 SPLayout-0.4.5/splayout/adjointmethod/shaperegion2d.py
+-rw-rw-rw-   0        0        0    10652 2023-02-23 12:35:57.000000 SPLayout-0.4.5/splayout/adjointmethod/shaperegion3d.py
+-rw-rw-rw-   0        0        0    11374 2023-02-23 12:36:38.000000 SPLayout-0.4.5/splayout/adjointmethod/topologyregion2d.py
+-rw-rw-rw-   0        0        0    11149 2023-02-24 02:38:35.000000 SPLayout-0.4.5/splayout/adjointmethod/topologyregion3d.py
+drwxrwxrwx   0        0        0        0 2023-04-15 14:29:30.000000 SPLayout-0.4.5/splayout/algorithms/
+-rw-rw-rw-   0        0        0      312 2023-02-23 13:06:11.000000 SPLayout-0.4.5/splayout/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     5781 2022-01-04 05:22:28.000000 SPLayout-0.4.5/splayout/algorithms/binarybatalgorithm.py
+-rw-rw-rw-   0        0        0     6360 2022-01-04 06:04:34.000000 SPLayout-0.4.5/splayout/algorithms/binarygeneticalgorithm.py
+-rw-rw-rw-   0        0        0     5831 2022-01-04 06:03:59.000000 SPLayout-0.4.5/splayout/algorithms/binaryparticleswarmalgorithm.py
+-rw-rw-rw-   0        0        0     4305 2023-02-23 12:22:49.000000 SPLayout-0.4.5/splayout/algorithms/directbinarysearchalgorithm.py
+-rw-rw-rw-   0        0        0     7333 2023-02-23 11:24:29.000000 SPLayout-0.4.5/splayout/algorithms/particleswarmalgorithm.py
+drwxrwxrwx   0        0        0        0 2023-04-15 14:29:30.000000 SPLayout-0.4.5/splayout/components/
+-rw-rw-rw-   0        0        0     3728 2023-02-23 12:38:12.000000 SPLayout-0.4.5/splayout/components/AEMDgrating.py
+-rw-rw-rw-   0        0        0      714 2023-02-23 13:44:58.000000 SPLayout-0.4.5/splayout/components/__init__.py
+-rw-rw-rw-   0        0        0     4403 2023-02-23 12:38:42.000000 SPLayout-0.4.5/splayout/components/bend.py
+-rw-rw-rw-   0        0        0     9026 2023-02-23 12:39:10.000000 SPLayout-0.4.5/splayout/components/doubleconnector.py
+-rw-rw-rw-   0        0        0     6092 2023-02-23 12:42:22.000000 SPLayout-0.4.5/splayout/components/filledpattern.py
+-rw-rw-rw-   0        0        0    49359 2023-02-23 12:42:22.000000 SPLayout-0.4.5/splayout/components/microring.py
+-rw-rw-rw-   0        0        0    21403 2023-02-23 12:42:22.000000 SPLayout-0.4.5/splayout/components/pixelsregion.py
+-rw-rw-rw-   0        0        0     7433 2023-02-23 12:41:22.000000 SPLayout-0.4.5/splayout/components/polygon.py
+-rw-rw-rw-   0        0        0    14219 2023-02-23 12:42:22.000000 SPLayout-0.4.5/splayout/components/quarbend.py
+-rw-rw-rw-   0        0        0    18098 2023-02-23 12:42:22.000000 SPLayout-0.4.5/splayout/components/sbend.py
+-rw-rw-rw-   0        0        0    13136 2023-02-23 12:41:22.000000 SPLayout-0.4.5/splayout/components/selfdefinecomponent.py
+-rw-rw-rw-   0        0        0    28052 2023-02-23 12:43:30.000000 SPLayout-0.4.5/splayout/components/simpleasymmetricdirectionalcoupler.py
+-rw-rw-rw-   0        0        0     7270 2023-02-23 12:41:22.000000 SPLayout-0.4.5/splayout/components/slowlyvaryingtaper.py
+-rw-rw-rw-   0        0        0     6668 2023-02-23 14:27:24.000000 SPLayout-0.4.5/splayout/components/taper.py
+-rw-rw-rw-   0        0        0     1269 2023-02-23 12:41:22.000000 SPLayout-0.4.5/splayout/components/text.py
+-rw-rw-rw-   0        0        0     8908 2023-02-23 12:42:22.000000 SPLayout-0.4.5/splayout/components/waveguide.py
+drwxrwxrwx   0        0        0        0 2023-04-15 14:29:30.000000 SPLayout-0.4.5/splayout/lumericalcommun/
+-rw-rw-rw-   0        0        0       72 2023-02-23 12:26:37.000000 SPLayout-0.4.5/splayout/lumericalcommun/__init__.py
+-rw-rw-rw-   0        0        0    77831 2023-04-15 14:25:50.000000 SPLayout-0.4.5/splayout/lumericalcommun/fdtdapi.py
+-rw-rw-rw-   0        0        0    44213 2023-02-23 12:42:48.000000 SPLayout-0.4.5/splayout/lumericalcommun/modeapi.py
+drwxrwxrwx   0        0        0        0 2023-04-15 14:29:30.000000 SPLayout-0.4.5/splayout/utils/
+-rw-rw-rw-   0        0        0       20 2023-02-23 12:27:14.000000 SPLayout-0.4.5/splayout/utils/__init__.py
+-rw-rw-rw-   0        0        0     7931 2023-02-23 12:43:16.000000 SPLayout-0.4.5/splayout/utils/utils.py
```

### Comparing `SPLayout-0.4.4/PKG-INFO` & `SPLayout-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: SPLayout
-Version: 0.4.4
+Version: 0.4.5
 Summary: Silicon Photonics Design Tools for GDSII Files.
 Home-page: https://github.com/Hideousmon/SPLayout
 Author: Zhenyu ZHAO
 Author-email: mailtozyzhao@163.com
 License: UNKNOWN
 Description: SPLayout
         ========
```

### Comparing `SPLayout-0.4.4/README.md` & `SPLayout-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/README.rst` & `SPLayout-0.4.5/README.rst`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/SPLayout.egg-info/PKG-INFO` & `SPLayout-0.4.5/SPLayout.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: SPLayout
-Version: 0.4.4
+Version: 0.4.5
 Summary: Silicon Photonics Design Tools for GDSII Files.
 Home-page: https://github.com/Hideousmon/SPLayout
 Author: Zhenyu ZHAO
 Author-email: mailtozyzhao@163.com
 License: UNKNOWN
 Description: SPLayout
         ========
```

### Comparing `SPLayout-0.4.4/SPLayout.egg-info/SOURCES.txt` & `SPLayout-0.4.5/SPLayout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/setup.py` & `SPLayout-0.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/splayout/__init__.py` & `SPLayout-0.4.5/splayout/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.4.4"
+__version__ = "0.4.5"
 
 ## Submodules
 from . import utils
 from . import components
 from . import algorithms
 from . import lumericalcommun
 from . import adjointmethod
```

### Comparing `SPLayout-0.4.4/splayout/adjointmethod/adjointshapeopt.py` & `SPLayout-0.4.5/splayout/adjointmethod/adjointshapeopt.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/splayout/adjointmethod/adjointtopologyopt.py` & `SPLayout-0.4.5/splayout/adjointmethod/adjointtopologyopt.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/splayout/adjointmethod/shaperegion2d.py` & `SPLayout-0.4.5/splayout/adjointmethod/shaperegion2d.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/splayout/adjointmethod/shaperegion3d.py` & `SPLayout-0.4.5/splayout/adjointmethod/shaperegion3d.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/splayout/adjointmethod/topologyregion2d.py` & `SPLayout-0.4.5/splayout/adjointmethod/topologyregion2d.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/splayout/adjointmethod/topologyregion3d.py` & `SPLayout-0.4.5/splayout/adjointmethod/topologyregion3d.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/splayout/algorithms/binarybatalgorithm.py` & `SPLayout-0.4.5/splayout/algorithms/binarybatalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/splayout/algorithms/binarygeneticalgorithm.py` & `SPLayout-0.4.5/splayout/algorithms/binarygeneticalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/splayout/algorithms/binaryparticleswarmalgorithm.py` & `SPLayout-0.4.5/splayout/algorithms/binaryparticleswarmalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/splayout/algorithms/directbinarysearchalgorithm.py` & `SPLayout-0.4.5/splayout/algorithms/directbinarysearchalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/splayout/algorithms/particleswarmalgorithm.py` & `SPLayout-0.4.5/splayout/algorithms/particleswarmalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/splayout/components/AEMDgrating.py` & `SPLayout-0.4.5/splayout/components/AEMDgrating.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/splayout/components/__init__.py` & `SPLayout-0.4.5/splayout/components/__init__.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/splayout/components/bend.py` & `SPLayout-0.4.5/splayout/components/bend.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/splayout/components/doubleconnector.py` & `SPLayout-0.4.5/splayout/components/doubleconnector.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/splayout/components/filledpattern.py` & `SPLayout-0.4.5/splayout/components/filledpattern.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/splayout/components/microring.py` & `SPLayout-0.4.5/splayout/components/microring.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/splayout/components/pixelsregion.py` & `SPLayout-0.4.5/splayout/components/pixelsregion.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/splayout/components/polygon.py` & `SPLayout-0.4.5/splayout/components/polygon.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/splayout/components/quarbend.py` & `SPLayout-0.4.5/splayout/components/quarbend.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/splayout/components/sbend.py` & `SPLayout-0.4.5/splayout/components/sbend.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/splayout/components/selfdefinecomponent.py` & `SPLayout-0.4.5/splayout/components/selfdefinecomponent.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/splayout/components/simpleasymmetricdirectionalcoupler.py` & `SPLayout-0.4.5/splayout/components/simpleasymmetricdirectionalcoupler.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/splayout/components/slowlyvaryingtaper.py` & `SPLayout-0.4.5/splayout/components/slowlyvaryingtaper.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/splayout/components/taper.py` & `SPLayout-0.4.5/splayout/components/taper.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/splayout/components/text.py` & `SPLayout-0.4.5/splayout/components/text.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/splayout/components/waveguide.py` & `SPLayout-0.4.5/splayout/components/waveguide.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/splayout/lumericalcommun/fdtdapi.py` & `SPLayout-0.4.5/splayout/lumericalcommun/fdtdapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1354,14 +1354,73 @@
                 scripts += "select(\"" + name + "\");"
                 scripts += "set(\"enabled\",1);"
             self.fdtd.eval(scripts)
         else:
             self.fdtd.eval("select(\"" + item_name + "\");")
             self.fdtd.eval("set(\"enabled\",1);")
 
+    def reset_wavelengths_of_sources(self, wavelength_start, wavelength_end):
+        """
+        Reset the wavelength_start and wavelength_end of the sources.
+
+        Parameters
+        ----------
+        wavelength_start : Float
+            The start wavelength of the source (unit: μm).
+        wavelength_end : Float
+            The end wavelength of the source (unit: μm).
+
+        Notes
+        -----
+        This function should be called when any source is added.
+        """
+        if (self.global_source_set_flag == 1):
+            self.fdtd.setglobalsource('wavelength start', wavelength_start * 1e-6)
+            self.fdtd.setglobalsource('wavelength stop', wavelength_end * 1e-6)
+            self.wavelength_start = wavelength_start * 1e-6
+            self.wavelength_end = wavelength_end * 1e-6
+        else:
+            raise Exception("Reset wavelengths of sources should be used when any source is added.")
+
+    def reset_wavelength_points_of_monitors(self, points):
+        """
+        Reset wavelength points of the monitors.
+
+        Parameters
+        ----------
+        points : Int
+            The number of the frequency points that will be monitored.
+
+        Notes
+        -----
+        This function should be called when any monitor is added.
+        """
+        if (self.global_monitor_set_flag == 1):
+            self.fdtd.setglobalmonitor('frequency points', points)
+            self.frequency_points = points
+        else:
+            raise Exception("Reset wavelength points of monitors should be used when any monitor is added.")
+
+    def reset_wavelength_points_of_selected_monitor(self, monitor_name, points):
+        """
+        Reset wavelength points of the monitors.
+
+        Parameters
+        ----------
+        monitor_name : String
+            Name of the monitor in Lumerical FDTD.
+        points : Int
+            The number of the frequency points that will be monitored.
+        """
+        self.fdtd.eval("select(\"" + monitor_name + "\");")
+        self.fdtd.eval("set(\"override global monitor settings\",1);")
+        self.fdtd.eval("set(\"use source limits\",1);")
+        self.fdtd.eval("set(\"use wavelength spacing\",1);")
+        self.fdtd.eval("set(\"frequency points\"," + str(int(points)) + ");")
+
     def remove(self, item_name):
         """
         Remove an item of the simulation.
 
         Parameters
         ----------
         item_name : String or list
```

### Comparing `SPLayout-0.4.4/splayout/lumericalcommun/modeapi.py` & `SPLayout-0.4.5/splayout/lumericalcommun/modeapi.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.4.4/splayout/utils/utils.py` & `SPLayout-0.4.5/splayout/utils/utils.py`

 * *Files identical despite different names*

