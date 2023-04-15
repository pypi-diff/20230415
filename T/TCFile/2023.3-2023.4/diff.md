# Comparing `tmp/TCFile-2023.3.tar.gz` & `tmp/TCFile-2023.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TCFile-2023.3.tar", last modified: Mon Mar  6 12:23:27 2023, max compression
+gzip compressed data, was "TCFile-2023.4.tar", last modified: Tue Apr  4 15:05:53 2023, max compression
```

## Comparing `TCFile-2023.3.tar` & `TCFile-2023.4.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0      259 2023-02-21 06:15:39.309633 TCFile-2023.3/.gitignore
--rw-r--r--   0        0        0     1090 2021-08-09 08:30:36.870133 TCFile-2023.3/LICENSE
--rw-r--r--   0        0        0      829 2023-02-21 06:45:10.368182 TCFile-2023.3/README.md
--rw-r--r--   0        0        0     3405 2023-03-06 12:19:52.724243 TCFile-2023.3/TCFile/TCFhandler/TCFile.py
--rw-r--r--   0        0        0       26 2023-02-21 05:09:10.170046 TCFile-2023.3/TCFile/TCFhandler/__init__.py
--rw-r--r--   0        0        0       25 2023-02-21 05:09:10.171047 TCFile-2023.3/TCFile/__init__.py
--rw-r--r--   0        0        0      919 2023-02-21 05:09:10.171047 TCFile-2023.3/TCFile/tests/TCFhandler.py
--rw-r--r--   0        0        0       16 2023-02-21 05:09:10.172048 TCFile-2023.3/TCFile/tests/__init__.py
--rw-r--r--   0        0        0     2040 2023-02-21 02:03:07.116288 TCFile-2023.3/docs/structure_TCF.md
--rw-r--r--   0        0        0     1088 2023-03-06 12:21:32.216416 TCFile-2023.3/pyproject.toml
--rw-r--r--   0        0        0     1720 1970-01-01 00:00:00.000000 TCFile-2023.3/PKG-INFO
+-rw-r--r--   0        0        0       42 2023-04-04 15:05:45.921389 TCFile-2023.4/.gitattributes
+-rw-r--r--   0        0        0      689 2023-04-04 15:05:45.921389 TCFile-2023.4/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      241 2023-04-04 15:05:45.921389 TCFile-2023.4/.gitignore
+-rw-r--r--   0        0        0     1069 2023-04-04 15:05:45.921389 TCFile-2023.4/LICENSE
+-rw-r--r--   0        0        0      819 2023-04-04 15:05:45.921389 TCFile-2023.4/README.md
+-rw-r--r--   0        0        0      929 2023-04-04 15:05:45.921389 TCFile-2023.4/TCFile-tests/TCFhandler.py
+-rw-r--r--   0        0        0      134 2023-04-04 15:05:45.997389 TCFile-2023.4/TCFile-tests/test_snapshot.TCF
+-rw-r--r--   0        0        0     3406 2023-04-04 15:05:45.997389 TCFile-2023.4/TCFile/TCFhandler/TCFile.py
+-rw-r--r--   0        0        0       26 2023-04-04 15:05:45.997389 TCFile-2023.4/TCFile/TCFhandler/__init__.py
+-rw-r--r--   0        0        0       25 2023-04-04 15:05:45.997389 TCFile-2023.4/TCFile/__init__.py
+-rw-r--r--   0        0        0     1956 2023-04-04 15:05:45.997389 TCFile-2023.4/docs/structure_TCF.md
+-rw-r--r--   0        0        0     1049 2023-04-04 15:05:45.997389 TCFile-2023.4/pyproject.toml
+-rw-r--r--   0        0        0     1751 1970-01-01 00:00:00.000000 TCFile-2023.4/PKG-INFO
```

### Comparing `TCFile-2023.3/TCFile/TCFhandler/TCFile.py` & `TCFile-2023.4/TCFile/TCFhandler/TCFile.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,103 +1,105 @@
-from typing import Sequence
-from PIL import Image
-import numpy as np
-import h5py
-
-class TCFile(Sequence):
-    '''
-    interface class to TCF files.
-    This class returns data as if list containg multiple data.
-    Preview of the data is stored in attributes.
-    * Note: It can read 3D, 2DMIP, BF.
-
-    Attributes
-    ----------
-    length : int
-        time series length of the TCF file
-    dataShape : numpy.array[int]
-        shape of single shot data
-    dataResolution : numpy.array[float]
-        (unit: μm) resolution of data. It represents unit resolution per pixel
-    dt : float
-        (unit: s) Time steps of data. Zero if it is single shot data
-    tcfname : str
-    imgtype : str
-    '''
-
-    def __init__(self, tcfname:str, imgtype:str):
-        '''
-        Paramters
-        ---------
-        tcfname : str
-            location of the target TCF file
-        imgtype : str
-            image type to see
-
-        Raises
-        ------
-        ValueError
-            If imgtype is unsupported given tcf file.
-        '''
-        # validation of input parameters
-        if '3D' == imgtype:
-            dim = 3
-        elif '2DMIP' == imgtype or 'BF' == imgtype:
-            dim = 2
-        else:
-            raise ValueError('The imgtype is not supported')
-
-        with h5py.File(tcfname) as f:
-            # validation of the given file
-            if 'Data' not in f:
-                raise ValueError('It is not tcf file')
-            elif imgtype not in f['Data']:
-                raise ValueError('The imgtype is not supported')
-            # load attributes
-            getAttr = lambda attrName: f[f'Data/{imgtype}'].attrs[attrName][0]
-        
-            self.length = getAttr('DataCount')
-            self.dataShape = list(getAttr(f'Size{axis}') for axis in  ('X', 'Y', 'Z')[:dim])
-            self.dataShape.reverse()
-            self.dataResolution = list(getAttr(f'Resolution{axis}') for axis in  ('X', 'Y', 'Z')[:dim])
-            self.dataResolution.reverse()
-            self.dt = getAttr('TimeInterval')
-        
-        self.tcfname = tcfname
-        self.imgtype = imgtype
-    
-    def __getitem__ (self, key:int) -> np.ndarray:
-        '''
-        Return
-        ------
-        data : numpy.ndarray[uint8]
-            raw data of refractive index mutliplided by 1e4.
-
-        Raises
-        ------
-        TypeError
-            If key is not int
-        IndexError
-            If key is out of bound
-        '''
-        length = len(self)
-        if not isinstance(key, int):
-            raise TypeError(f'{self.__class__} indices must be integer, not {type(key)}')
-        if key < -length or key >= length:
-            raise IndexError(f'{self.__class__} index out of range')
-        key = (key + length) % length
-
-        with h5py.File(self.tcfname) as f:
-            data = f[f'Data/{self.imgtype}/{key:06d}'][()] 
-        
-        if ('3D' == self.imgtype or '2DMIP' == self.imgtype) and not np.issubdtype(data.dtype, np.floating):
-            # To preserve the storage, some TCF file save data as a UInt16 integer scaled by 1e4
-            data = data.astype(np.float32)
-            data /= 1e4
-        elif 'BF' == self.imgtype:
-            data = Image.fromarray(data, mode = 'RGB')
-
-        return data
-
-    def __len__(self):
-        return self.length
-
+from typing import Sequence
+from PIL import Image
+import numpy as np
+import h5py
+
+class TCFile(Sequence):
+    '''
+    interface class to TCF files.
+    This class returns data as if list containg multiple data.
+    Preview of the data is stored in attributes.
+    * Note: It can read 3D, 2DMIP, BF.
+
+    Attributes
+    ----------
+    length : int
+        time series length of the TCF file
+    dataShape : numpy.array[int]
+        shape of single shot data
+    dataResolution : numpy.array[float]
+        (unit: μm) resolution of data. It represents unit resolution per pixel
+    dt : float
+        (unit: s) Time steps of data. Zero if it is single shot data
+    tcfname : str
+    imgtype : str
+    '''
+
+    def __init__(self, tcfname:str, imgtype:str):
+        '''
+        Paramters
+        ---------
+        tcfname : str
+            location of the target TCF file
+        imgtype : str
+            image type to see
+
+        Raises
+        ------
+        ValueError
+            If imgtype is unsupported given tcf file.
+        '''
+        # validation of input parameters
+        if '3D' == imgtype:
+            dim = 3
+        elif '2DMIP' == imgtype or 'BF' == imgtype:
+            dim = 2
+        else:
+            raise ValueError('The imgtype is not supported')
+
+        with h5py.File(tcfname) as f:
+            # validation of the given file
+            if 'Data' not in f:
+                raise ValueError('It is not tcf file')
+            elif imgtype not in f['Data']:
+                raise ValueError('The imgtype is not supported')
+            # load attributes
+            getAttr = lambda attrName: f[f'Data/{imgtype}'].attrs.get(attrName)[0]
+        
+            self.length = getAttr('DataCount')
+            self.dataShape = list(getAttr(f'Size{axis}') for axis in  ('X', 'Y', 'Z')[:dim])
+            self.dataShape.reverse()
+            self.dataResolution = list(getAttr(f'Resolution{axis}') for axis in  ('X', 'Y', 'Z')[:dim])
+            self.dataResolution.reverse()
+            self.dt = f[f'Data/{imgtype}'].attrs.get('TimeInterval',default=[None])[0]
+            if self.dt is None:
+                self.dt = 0
+        
+        self.tcfname = tcfname
+        self.imgtype = imgtype
+    
+    def __getitem__ (self, key:int) -> np.ndarray:
+        '''
+        Return
+        ------
+        data : numpy.ndarray[uint8]
+            raw data of refractive index mutliplided by 1e4.
+
+        Raises
+        ------
+        TypeError
+            If key is not int
+        IndexError
+            If key is out of bound
+        '''
+        length = len(self)
+        if not isinstance(key, int):
+            raise TypeError(f'{self.__class__} indices must be integer, not {type(key)}')
+        if key < -length or key >= length:
+            raise IndexError(f'{self.__class__} index out of range')
+        key = (key + length) % length
+
+        with h5py.File(self.tcfname) as f:
+            data = f[f'Data/{self.imgtype}/{key:06d}'][()]
+        
+        if ('3D' == self.imgtype or '2DMIP' == self.imgtype) and not np.issubdtype(data.dtype, np.floating):
+            # To preserve the storage, some TCF file save data as a UInt16 integer scaled by 1e4
+            data = data.astype(np.float32)
+            data /= 1e4
+        elif 'BF' == self.imgtype:
+            data = Image.fromarray(data, mode = 'RGB')
+
+        return data
+
+    def __len__(self):
+        return self.length
+
```

### Comparing `TCFile-2023.3/PKG-INFO` & `TCFile-2023.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TCFile
-Version: 2023.3
+Version: 2023.4
 Summary: Python package for handling TCF data. It works with Tomcube data
 Author-email: Dohyeon Lee <dleh428@kaist.ac.kr>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -41,15 +41,15 @@
 Please use this package with full understanding.
 Any suggestions and comments are welcome! 
 
 ## Use case
 
 ```python
 
-from TCFile import *
+from ..TCFile import *
 
 tcfile = TCFile('test.TCF','3D') # for now, it only read 3D RI data
 print(f"number of snapshots : {len(tcfile)}")
 
 ## Usage 1: handling a data for each snapshot
 data = tcfile[0]
 print(f"shape of data : {data.shape}")
@@ -58,10 +58,11 @@
     # do some operations on the data ...
     pass
 ```
 
 ## Test (for development and contribution)
 
 ```bash
-pytest TCFile/tests/TCFhandler.py
+conda install PIL h5py numpy
+pytest TCFile-tests/TCFhandler.py
 ```
```

