# Comparing `tmp/PrettyColorPrinter-0.40.tar.gz` & `tmp/PrettyColorPrinter-0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrettyColorPrinter-0.40.tar", last modified: Sun Jan  1 05:47:34 2023, max compression
+gzip compressed data, was "PrettyColorPrinter-0.41.tar", last modified: Sat Apr 15 15:46:48 2023, max compression
```

## Comparing `PrettyColorPrinter-0.40.tar` & `PrettyColorPrinter-0.41.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-01-01 05:47:34.231565 PrettyColorPrinter-0.40/
--rw-rw-rw-   0        0        0     1148 2023-01-01 05:47:24.000000 PrettyColorPrinter-0.40/LICENSE.rst
--rw-rw-rw-   0        0        0      161 2023-01-01 05:47:22.000000 PrettyColorPrinter-0.40/MANIFEST.in
--rw-rw-rw-   0        0        0     5714 2023-01-01 05:47:34.231565 PrettyColorPrinter-0.40/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-01-01 05:47:34.225733 PrettyColorPrinter-0.40/PrettyColorPrinter/
--rw-rw-rw-   0        0        0     1069 2022-10-02 04:27:48.000000 PrettyColorPrinter-0.40/PrettyColorPrinter/LICENSE
--rw-rw-rw-   0        0        0     4579 2022-12-27 17:15:50.000000 PrettyColorPrinter-0.40/PrettyColorPrinter/README.MD
--rw-rw-rw-   0        0        0    53597 2023-01-01 05:42:25.000000 PrettyColorPrinter-0.40/PrettyColorPrinter/__init__.py
--rw-rw-rw-   0        0        0       45 2023-01-01 05:47:33.000000 PrettyColorPrinter-0.40/PrettyColorPrinter/requirements.txt
--rw-rw-rw-   0        0        0        2 2023-01-01 05:47:33.000000 PrettyColorPrinter-0.40/PrettyColorPrinter/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-01-01 05:47:34.230589 PrettyColorPrinter-0.40/PrettyColorPrinter.egg-info/
--rw-rw-rw-   0        0        0     5714 2023-01-01 05:47:34.000000 PrettyColorPrinter-0.40/PrettyColorPrinter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      419 2023-01-01 05:47:34.000000 PrettyColorPrinter-0.40/PrettyColorPrinter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-01 05:47:34.000000 PrettyColorPrinter-0.40/PrettyColorPrinter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-01-01 05:47:34.000000 PrettyColorPrinter-0.40/PrettyColorPrinter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-01-01 05:47:34.000000 PrettyColorPrinter-0.40/PrettyColorPrinter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4579 2022-12-27 17:15:50.000000 PrettyColorPrinter-0.40/README.md
--rw-rw-rw-   0        0        0      115 2023-01-01 05:47:34.232541 PrettyColorPrinter-0.40/setup.cfg
--rw-rw-rw-   0        0        0     1591 2023-01-01 05:47:33.000000 PrettyColorPrinter-0.40/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 15:46:48.269403 PrettyColorPrinter-0.41/
+-rw-rw-rw-   0        0        0     1148 2023-04-15 15:46:39.000000 PrettyColorPrinter-0.41/LICENSE.rst
+-rw-rw-rw-   0        0        0      161 2023-04-15 15:46:38.000000 PrettyColorPrinter-0.41/MANIFEST.in
+-rw-rw-rw-   0        0        0     5450 2023-04-15 15:46:48.269403 PrettyColorPrinter-0.41/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-15 15:46:48.264418 PrettyColorPrinter-0.41/PrettyColorPrinter/
+-rw-rw-rw-   0        0        0     1069 2023-04-15 00:18:29.000000 PrettyColorPrinter-0.41/PrettyColorPrinter/LICENSE
+-rw-rw-rw-   0        0        0     4579 2023-04-15 00:18:29.000000 PrettyColorPrinter-0.41/PrettyColorPrinter/README.MD
+-rw-rw-rw-   0        0        0    53608 2023-04-15 15:34:24.000000 PrettyColorPrinter-0.41/PrettyColorPrinter/__init__.py
+-rw-rw-rw-   0        0        0       45 2023-04-15 15:46:47.000000 PrettyColorPrinter-0.41/PrettyColorPrinter/requirements.txt
+-rw-rw-rw-   0        0        0    64025 2023-04-15 15:46:47.000000 PrettyColorPrinter-0.41/PrettyColorPrinter/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-15 15:46:48.268413 PrettyColorPrinter-0.41/PrettyColorPrinter.egg-info/
+-rw-rw-rw-   0        0        0     5450 2023-04-15 15:46:48.000000 PrettyColorPrinter-0.41/PrettyColorPrinter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      419 2023-04-15 15:46:48.000000 PrettyColorPrinter-0.41/PrettyColorPrinter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 15:46:48.000000 PrettyColorPrinter-0.41/PrettyColorPrinter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 15:46:48.000000 PrettyColorPrinter-0.41/PrettyColorPrinter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-15 15:46:48.000000 PrettyColorPrinter-0.41/PrettyColorPrinter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4579 2023-04-15 00:18:29.000000 PrettyColorPrinter-0.41/README.md
+-rw-rw-rw-   0        0        0       85 2023-04-15 15:46:48.270428 PrettyColorPrinter-0.41/setup.cfg
+-rw-rw-rw-   0        0        0     1507 2023-04-15 15:46:47.000000 PrettyColorPrinter-0.41/setup.py
```

### Comparing `PrettyColorPrinter-0.40/LICENSE.rst` & `PrettyColorPrinter-0.41/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `PrettyColorPrinter-0.40/PKG-INFO` & `PrettyColorPrinter-0.41/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,57 +1,51 @@
 Metadata-Version: 2.1
 Name: PrettyColorPrinter
-Version: 0.40
+Version: 0.41
 Summary: Pandas DataFrames / Pandas Series / Print colored Numpy arrays / lists / dicts / tuples!
 Home-page: https://github.com/hansalemaos/PrettyColorPrinter
 Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
+Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: pandas,numpy,dataframe,series,print,prettyprint,colored,coloured
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Editors :: Text Processing
-Classifier: Topic :: Text Processing :: General
-Classifier: Topic :: Text Processing :: Indexing
-Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
-
 # **Print colored Numpy arrays / pandas DataFrames / Pandas Series / lists / dicts / tuples!**
 
 ```python
 pip install PrettyColorPrinter
 ```
 
 #### **This is everything you have to do to use PrettyColorPrinter with pandas**
 
 ```python
 from PrettyColorPrinter import add_printer
 add_printer() #This function will add some methods to PandasObject
 
-#Let’s import pandas and create a DataFrame:
+#Letâ€™s import pandas and create a DataFrame:
 
 import pandas as pd
 df=pd.read_csv(r"https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_no2_long.csv")
 ```
 
 ### Update 2022/12/27
 
 You can switch between the colored version and the black/white version. 
 
 ```python
-import pandas as pd
-from PrettyColorPrinter import add_printer, switch_color_bw
-add_printer(True)
-switch_color_bw()
+import pandas as pd
+from PrettyColorPrinter import add_printer, switch_color_bw
+add_printer(True)
+switch_color_bw()
 
 ```
 
 ### Update 2022/10/08
 
 Fixed a bug with empty DataFrames
 
@@ -147,15 +141,15 @@
         return the input DataFrame to allow chaining
 ```
 
 ### Using PrettyColorPrinter without pandas
 
 **
 
-The function **pdp** can be used without pandas.   
+The function **pdp** can be used without pandas.Â   
 Doing it this way, you are not restricted to PandasObjects.
 
 **You can print lists, dicts, tuples, np.arrays, pd.DataFrames and pd.Series**
 
 **
 
 ```python
```

### Comparing `PrettyColorPrinter-0.40/PrettyColorPrinter/LICENSE` & `PrettyColorPrinter-0.41/PrettyColorPrinter/LICENSE`

 * *Files identical despite different names*

### Comparing `PrettyColorPrinter-0.40/PrettyColorPrinter/README.MD` & `PrettyColorPrinter-0.41/PrettyColorPrinter/README.MD`

 * *Files identical despite different names*

### Comparing `PrettyColorPrinter-0.40/PrettyColorPrinter/__init__.py` & `PrettyColorPrinter-0.41/PrettyColorPrinter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -763,22 +763,22 @@
             if indiprint != len(columnsprint):
                 print(TC(f"{labels}  ").bg_red.fg_black, end="")
                 print(TC("█").fg_yellow.bg_black, end="")
             if indiprint + 1 == len(columnsprint):
                 pass
                 print("", end="\n")
 
-    maxsize = [
-        df[x].astype("string").array.astype("U").dtype.itemsize // 4 for x in df.columns
-    ]
+    maxsize = (
+        df[x].astype("string").__array__().astype("U").dtype.itemsize //4 for x in df.columns
+    )
     maxsize_cols = [len(str(x)) for x in df.columns]
     maxsize = [x if x >= y else y for x, y in zip(maxsize, maxsize_cols)]
 
     maxsize_ = [x + 2 if x < max_column_size else max_column_size for x in maxsize]
-    maxindexsize = 4 + (df.index.astype("string").array.astype("U").dtype.itemsize // 4)
+    maxindexsize = 4 + (df.index.astype("string").__array__().astype("U").dtype.itemsize // 4)
     if maxindexsize < 8:
         maxindexsize = 9
 
     columnsprint = [
         str(f"{col}").replace("\n", "\\n").replace("\r", "\\r")[:size].rjust(size + 1)
         for col, size in zip(df.columns, maxsize_)
     ]
```

### Comparing `PrettyColorPrinter-0.40/PrettyColorPrinter.egg-info/PKG-INFO` & `PrettyColorPrinter-0.41/PrettyColorPrinter.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,57 +1,51 @@
 Metadata-Version: 2.1
 Name: PrettyColorPrinter
-Version: 0.40
+Version: 0.41
 Summary: Pandas DataFrames / Pandas Series / Print colored Numpy arrays / lists / dicts / tuples!
 Home-page: https://github.com/hansalemaos/PrettyColorPrinter
 Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
+Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: pandas,numpy,dataframe,series,print,prettyprint,colored,coloured
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Editors :: Text Processing
-Classifier: Topic :: Text Processing :: General
-Classifier: Topic :: Text Processing :: Indexing
-Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
-
 # **Print colored Numpy arrays / pandas DataFrames / Pandas Series / lists / dicts / tuples!**
 
 ```python
 pip install PrettyColorPrinter
 ```
 
 #### **This is everything you have to do to use PrettyColorPrinter with pandas**
 
 ```python
 from PrettyColorPrinter import add_printer
 add_printer() #This function will add some methods to PandasObject
 
-#Let’s import pandas and create a DataFrame:
+#Letâ€™s import pandas and create a DataFrame:
 
 import pandas as pd
 df=pd.read_csv(r"https://github.com/pandas-dev/pandas/raw/main/doc/data/air_quality_no2_long.csv")
 ```
 
 ### Update 2022/12/27
 
 You can switch between the colored version and the black/white version. 
 
 ```python
-import pandas as pd
-from PrettyColorPrinter import add_printer, switch_color_bw
-add_printer(True)
-switch_color_bw()
+import pandas as pd
+from PrettyColorPrinter import add_printer, switch_color_bw
+add_printer(True)
+switch_color_bw()
 
 ```
 
 ### Update 2022/10/08
 
 Fixed a bug with empty DataFrames
 
@@ -147,15 +141,15 @@
         return the input DataFrame to allow chaining
 ```
 
 ### Using PrettyColorPrinter without pandas
 
 **
 
-The function **pdp** can be used without pandas.   
+The function **pdp** can be used without pandas.Â   
 Doing it this way, you are not restricted to PandasObjects.
 
 **You can print lists, dicts, tuples, np.arrays, pd.DataFrames and pd.Series**
 
 **
 
 ```python
```

### Comparing `PrettyColorPrinter-0.40/README.md` & `PrettyColorPrinter-0.41/README.md`

 * *Files identical despite different names*

### Comparing `PrettyColorPrinter-0.40/setup.py` & `PrettyColorPrinter-0.41/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from setuptools import setup, find_packages
-import codecs
-import os
+# import codecs
+# import os
+# 
+# here = os.path.abspath(os.path.dirname(__file__))
+# 
+# with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
+#     long_description = "\n" + fh.read()\
 
-#change to dict
-here = os.path.abspath(os.path.dirname(__file__))
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
-with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
-    long_description = "\n" + fh.read()
-
-VERSION = '0.40'
-DESCRIPTION = "Pandas DataFrames / Pandas Series / Print colored Numpy arrays / lists / dicts / tuples!"
+VERSION = '''0.41'''
+DESCRIPTION = '''Pandas DataFrames / Pandas Series / Print colored Numpy arrays / lists / dicts / tuples!'''
 
 # Setting up
 setup(
     name="PrettyColorPrinter",
     version=VERSION,
     license='MIT',
     url = 'https://github.com/hansalemaos/PrettyColorPrinter',
     author="Johannes Fischer",
-    author_email="<aulasparticularesdealemaosp@gmail.com>",
+    author_email="aulasparticularesdealemaosp@gmail.com",
     description=DESCRIPTION,
-    long_description_content_type="text/markdown",
-    long_description=long_description,
+long_description = long_description,
+long_description_content_type="text/markdown",
     #packages=['cprinter', 'input_timeout', 'numpy', 'pandas', 'regex'],
     keywords=['pandas', 'numpy', 'dataframe', 'series', 'print', 'prettyprint', 'colored', 'coloured'],
-    classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.9', 'Topic :: Scientific/Engineering :: Visualization', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Text Editors :: Text Processing', 'Topic :: Text Processing :: General', 'Topic :: Text Processing :: Indexing', 'Topic :: Text Processing :: Filters', 'Topic :: Utilities'],
+    classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.10', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Utilities'],
     install_requires=['cprinter', 'input_timeout', 'numpy', 'pandas', 'regex'],
     include_package_data=True
 )
 #python setup.py sdist bdist_wheel
 #twine upload dist/*
```

