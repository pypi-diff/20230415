# Comparing `tmp/vtreat-1.2.7.tar.gz` & `tmp/vtreat-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtreat-1.2.7.tar", last modified: Fri Apr  7 18:42:46 2023, max compression
+gzip compressed data, was "vtreat-1.2.8.tar", last modified: Sat Apr 15 19:04:00 2023, max compression
```

## Comparing `vtreat-1.2.7.tar` & `vtreat-1.2.8.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-07 18:42:46.476559 vtreat-1.2.7/
--rw-r--r--   0 johnmount   (501) staff       (20)     1494 2019-07-23 14:11:34.000000 vtreat-1.2.7/LICENSE
--rw-r--r--   0 johnmount   (501) staff       (20)     3207 2023-04-07 18:42:46.476269 vtreat-1.2.7/PKG-INFO
--rw-r--r--   0 johnmount   (501) staff       (20)    35907 2022-01-27 17:04:33.000000 vtreat-1.2.7/README.md
--rw-r--r--   0 johnmount   (501) staff       (20)       38 2023-04-07 18:42:46.476656 vtreat-1.2.7/setup.cfg
--rw-r--r--   0 johnmount   (501) staff       (20)     3812 2022-12-14 00:59:42.000000 vtreat-1.2.7/setup.py
-drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-07 18:42:46.472226 vtreat-1.2.7/vtreat/
--rw-r--r--   0 johnmount   (501) staff       (20)     2643 2022-12-14 00:59:35.000000 vtreat-1.2.7/vtreat/__init__.py
--rw-r--r--   0 johnmount   (501) staff       (20)     3699 2022-01-27 17:04:33.000000 vtreat-1.2.7/vtreat/cross_plan.py
--rw-r--r--   0 johnmount   (501) staff       (20)     3632 2022-09-12 18:41:57.000000 vtreat-1.2.7/vtreat/effect_scaler.py
--rw-r--r--   0 johnmount   (501) staff       (20)     8158 2022-01-27 17:04:33.000000 vtreat-1.2.7/vtreat/stats_utils.py
--rw-r--r--   0 johnmount   (501) staff       (20)     1074 2022-01-27 17:04:33.000000 vtreat-1.2.7/vtreat/transform.py
--rw-r--r--   0 johnmount   (501) staff       (20)     8629 2022-01-27 17:04:33.000000 vtreat-1.2.7/vtreat/util.py
--rw-r--r--   0 johnmount   (501) staff       (20)    29728 2022-01-27 17:04:33.000000 vtreat-1.2.7/vtreat/vtreat_api.py
--rw-r--r--   0 johnmount   (501) staff       (20)     8031 2022-12-24 16:28:04.000000 vtreat-1.2.7/vtreat/vtreat_db_adapter.py
--rw-r--r--   0 johnmount   (501) staff       (20)    62607 2022-01-27 17:04:33.000000 vtreat-1.2.7/vtreat/vtreat_impl.py
-drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-07 18:42:46.475857 vtreat-1.2.7/vtreat.egg-info/
--rw-r--r--   0 johnmount   (501) staff       (20)     3207 2023-04-07 18:42:46.000000 vtreat-1.2.7/vtreat.egg-info/PKG-INFO
--rw-r--r--   0 johnmount   (501) staff       (20)      367 2023-04-07 18:42:46.000000 vtreat-1.2.7/vtreat.egg-info/SOURCES.txt
--rw-r--r--   0 johnmount   (501) staff       (20)        1 2023-04-07 18:42:46.000000 vtreat-1.2.7/vtreat.egg-info/dependency_links.txt
--rw-r--r--   0 johnmount   (501) staff       (20)       52 2023-04-07 18:42:46.000000 vtreat-1.2.7/vtreat.egg-info/requires.txt
--rw-r--r--   0 johnmount   (501) staff       (20)        7 2023-04-07 18:42:46.000000 vtreat-1.2.7/vtreat.egg-info/top_level.txt
+drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-15 19:04:00.382947 vtreat-1.2.8/
+-rw-r--r--   0 johnmount   (501) staff       (20)     1494 2019-07-23 14:11:34.000000 vtreat-1.2.8/LICENSE
+-rw-r--r--   0 johnmount   (501) staff       (20)     3207 2023-04-15 19:04:00.382660 vtreat-1.2.8/PKG-INFO
+-rw-r--r--   0 johnmount   (501) staff       (20)    35907 2022-01-27 17:04:33.000000 vtreat-1.2.8/README.md
+-rw-r--r--   0 johnmount   (501) staff       (20)       38 2023-04-15 19:04:00.383031 vtreat-1.2.8/setup.cfg
+-rw-r--r--   0 johnmount   (501) staff       (20)     3812 2023-04-15 19:03:51.000000 vtreat-1.2.8/setup.py
+drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-15 19:04:00.380672 vtreat-1.2.8/vtreat/
+-rw-r--r--   0 johnmount   (501) staff       (20)     2643 2023-04-15 19:03:35.000000 vtreat-1.2.8/vtreat/__init__.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     3699 2022-01-27 17:04:33.000000 vtreat-1.2.8/vtreat/cross_plan.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     3632 2022-09-12 18:41:57.000000 vtreat-1.2.8/vtreat/effect_scaler.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     4602 2023-04-15 17:53:59.000000 vtreat-1.2.8/vtreat/partial_pooling_estimator.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     8158 2022-01-27 17:04:33.000000 vtreat-1.2.8/vtreat/stats_utils.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     1074 2022-01-27 17:04:33.000000 vtreat-1.2.8/vtreat/transform.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     8932 2023-04-15 18:09:20.000000 vtreat-1.2.8/vtreat/util.py
+-rw-r--r--   0 johnmount   (501) staff       (20)    29728 2022-01-27 17:04:33.000000 vtreat-1.2.8/vtreat/vtreat_api.py
+-rw-r--r--   0 johnmount   (501) staff       (20)     8031 2022-12-24 16:28:04.000000 vtreat-1.2.8/vtreat/vtreat_db_adapter.py
+-rw-r--r--   0 johnmount   (501) staff       (20)    63169 2023-04-15 18:43:59.000000 vtreat-1.2.8/vtreat/vtreat_impl.py
+drwxr-xr-x   0 johnmount   (501) staff       (20)        0 2023-04-15 19:04:00.382276 vtreat-1.2.8/vtreat.egg-info/
+-rw-r--r--   0 johnmount   (501) staff       (20)     3207 2023-04-15 19:04:00.000000 vtreat-1.2.8/vtreat.egg-info/PKG-INFO
+-rw-r--r--   0 johnmount   (501) staff       (20)      403 2023-04-15 19:04:00.000000 vtreat-1.2.8/vtreat.egg-info/SOURCES.txt
+-rw-r--r--   0 johnmount   (501) staff       (20)        1 2023-04-15 19:04:00.000000 vtreat-1.2.8/vtreat.egg-info/dependency_links.txt
+-rw-r--r--   0 johnmount   (501) staff       (20)       52 2023-04-15 19:04:00.000000 vtreat-1.2.8/vtreat.egg-info/requires.txt
+-rw-r--r--   0 johnmount   (501) staff       (20)        7 2023-04-15 19:04:00.000000 vtreat-1.2.8/vtreat.egg-info/top_level.txt
```

### Comparing `vtreat-1.2.7/LICENSE` & `vtreat-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vtreat-1.2.7/PKG-INFO` & `vtreat-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtreat
-Version: 1.2.7
+Version: 1.2.8
 Summary: vtreat is a pandas.DataFrame processor/conditioner that prepares real-world data for predictive modeling in a statistically sound manner. 
 Home-page: https://github.com/WinVector/pyvtreat
 Author: John Mount, Nina Zumel
 Author-email: jmount@win-vector.com
 License: License :: OSI Approved :: BSD 3-clause License
 Platform: any
 Classifier: Intended Audience :: Science/Research
```

### Comparing `vtreat-1.2.7/README.md` & `vtreat-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `vtreat-1.2.7/setup.py` & `vtreat-1.2.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 as a [`Python`/`Pandas` package](https://github.com/WinVector/vtreat),
 and also as an [`R` package](https://github.com/WinVector/vtreat).
 """
 
 
 setuptools.setup(
     name='vtreat',
-    version='1.2.7',
+    version='1.2.8',
     author='John Mount, Nina Zumel',
     author_email='jmount@win-vector.com',
     url='https://github.com/WinVector/pyvtreat',
     packages=setuptools.find_packages(where='.', exclude=['tests', 'Examples']),
     install_requires=[
         'numpy',
         'pandas',
```

### Comparing `vtreat-1.2.7/vtreat/__init__.py` & `vtreat-1.2.8/vtreat/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # noinspection PyUnresolvedReferences
 import numpy
 
 from vtreat.vtreat_api import *
 
 __docformat__ = "restructuredtext"
-__version__ = "1.2.7"
+__version__ = "1.2.8"
 
 __doc__ = """
 This<https://github.com/WinVector/pyvtreat> is the Python version of the vtreat data preparation system
 (also available as an R package<https://winvector.github.io/vtreat/>.
 
 vtreat is a DataFrame processor/conditioner that prepares
 real-world data for supervised machine learning or predictive modeling
```

### Comparing `vtreat-1.2.7/vtreat/cross_plan.py` & `vtreat-1.2.8/vtreat/cross_plan.py`

 * *Files identical despite different names*

### Comparing `vtreat-1.2.7/vtreat/effect_scaler.py` & `vtreat-1.2.8/vtreat/effect_scaler.py`

 * *Files identical despite different names*

### Comparing `vtreat-1.2.7/vtreat/stats_utils.py` & `vtreat-1.2.8/vtreat/stats_utils.py`

 * *Files identical despite different names*

### Comparing `vtreat-1.2.7/vtreat/transform.py` & `vtreat-1.2.8/vtreat/transform.py`

 * *Files identical despite different names*

### Comparing `vtreat-1.2.7/vtreat/util.py` & `vtreat-1.2.8/vtreat/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import hashlib
 
 import numpy
 import pandas
 
 import vtreat.stats_utils
+from vtreat.partial_pooling_estimator import pooled_effect_estimate
 
 
 def safe_to_numeric_array(x):
     """
     Convert array to numeric. Note, will parse strings (due to numpy)!
 
     :param x: array to process
@@ -134,25 +135,36 @@
         avg_var = numpy.nanmean(sf["_var"])
     sf.loc[bad_vars, "_var"] = avg_var
     if sf.shape[0] > 1:
         sf["_vb"] = statistics.variance(sf["_group_mean"]) + eps
     else:
         sf["_vb"] = eps
     sf["_gm"] = global_mean
-    # hierarchical model is in:
-    # http://www.win-vector.com/blog/2017/09/partial-pooling-for-lower-variance-variable-encoding/
-    # using naive empirical estimates of variances
-    # adjusted from ni to ni-1 and +eps variance to make
-    # rare levels look like new levels.
-    sf["_hest"] = (
-        (sf["_ni"] - 1) * sf["_group_mean"] / sf["_var"] + sf["_gm"] / sf["_vb"]
-    ) / ((sf["_ni"] - 1) / sf["_var"] + 1 / sf["_vb"])
+    sf.sort_values(["x"], inplace=True, ignore_index=True)
     return sf
 
 
+def pooled_impact_estimate(x, y):
+    """
+    compute some pooled grouped by x vector summaries of numeric y vector (no missing values in y)
+    http://www.win-vector.com/blog/2017/09/partial-pooling-for-lower-variance-variable-encoding/
+    https://github.com/WinVector/Examples/blob/main/PartialPooling/PartialPooling.ipynb
+    """
+    n = len(x)
+    assert n > 0
+    assert n == len(y)
+    obs = pandas.DataFrame({
+        "location_id": x,
+        "observation": safe_to_numeric_array(y),
+    })
+    res = pooled_effect_estimate(obs)
+    res.rename(columns={"location_id": "x"}, inplace=True)
+    return res
+
+
 def score_variables(
         cross_frame: pandas.DataFrame,
         *,
         variables: Optional[Iterable[str]],
         outcome,
         is_classification: bool = False) -> Optional[pandas.DataFrame]:
     """
@@ -295,10 +307,7 @@
     """
     Get a hash code representing a data frame.
 
     :param d: data frame
     :return: hash code as a string
     """
     return hashlib.sha256(pandas.util.hash_pandas_object(d).values).hexdigest()
-
-
-
```

### Comparing `vtreat-1.2.7/vtreat/vtreat_api.py` & `vtreat-1.2.8/vtreat/vtreat_api.py`

 * *Files identical despite different names*

### Comparing `vtreat-1.2.7/vtreat/vtreat_db_adapter.py` & `vtreat-1.2.8/vtreat/vtreat_db_adapter.py`

 * *Files identical despite different names*

### Comparing `vtreat-1.2.7/vtreat/vtreat_impl.py` & `vtreat-1.2.8/vtreat/vtreat_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -473,22 +473,25 @@
     :param x: training explanatory values
     :param y: training dependent values
     :param extra_args: optional extra arguments for fit_ methods
     :param params: control parameter dictionary
     :return:
     """
 
-    sf = vtreat.util.grouped_by_x_statistics(x, y)
-    if sf.shape[0] <= 1:
+    if (len(x) <= 1) or (len(set(x)) <= 1):
         return None
     if params["use_hierarchical_estimate"]:
-        sf["_impact_code"] = sf["_hest"] - sf["_gm"]
+        cf = vtreat.util.pooled_impact_estimate(x, y)
+        cf["_impact_code"] = cf["estimate"] - cf["grand_mean"]
     else:
-        sf["_impact_code"] = sf["_group_mean"] - sf["_gm"]
-    sf = sf.loc[:, ["x", "_impact_code"]].copy()
+        cf = vtreat.util.grouped_by_x_statistics(x, y)
+        cf["_impact_code"] = cf["_group_mean"] - cf["_gm"]
+    if cf.shape[0] <= 1:
+        return None
+    sf = cf.loc[:, ["x", "_impact_code"]].reset_index(drop=True, inplace=False)
     newcol = incoming_column_name + "_impact_code"
     sf.columns = [incoming_column_name, newcol]
     return YAwareMappedCodeTransform(
         incoming_column_name=incoming_column_name,
         derived_column_name=newcol,
         treatment="impact_code",
         code_book=sf,
@@ -513,19 +516,21 @@
     :param x: training explanatory values
     :param y: training dependent values
     :param extra_args: optional extra arguments for fit_ methods
     :param params: control parameter dictionary
     :return:
     """
 
-    sf = vtreat.util.grouped_by_x_statistics(x, y)
-    if sf.shape[0] <= 1:
+    if (len(x) <= 1) or (len(set(x)) <= 1):
         return None
+    sf = vtreat.util.grouped_by_x_statistics(x, y)
     sf["_deviation_code"] = numpy.sqrt(sf["_var"])
     sf = sf.loc[:, ["x", "_deviation_code"]].copy()
+    if sf.shape[0] <= 1:
+        return None
     newcol = incoming_column_name + "_deviation_code"
     sf.columns = [incoming_column_name, newcol]
     return YAwareMappedCodeTransform(
         incoming_column_name=incoming_column_name,
         derived_column_name=newcol,
         treatment="deviation_code",
         code_book=sf,
@@ -549,28 +554,37 @@
     :param incoming_column_name:
     :param x: training explanatory values
     :param y: training dependent values
     :param extra_args: required extra arguments for fit_ methods
     :param params: control parameter dictionary
     :return:
     """
+    if (len(x) <= 1) or (len(set(x)) <= 1):
+        return None
     outcome_target = (
         extra_args["outcome_target"],
     )  # TODO: document why this is a tuple
     var_suffix = extra_args["var_suffix"]
     y = numpy.asarray(numpy.asarray(y) == outcome_target, dtype=float)
-    sf = vtreat.util.grouped_by_x_statistics(x, y)
-    if sf.shape[0] <= 1:
-        return None
     eps = 1.0e-3
     if params["use_hierarchical_estimate"]:
-        sf["_logit_code"] = numpy.log((sf["_hest"] + eps) / (sf["_gm"] + eps))
+        cf = vtreat.util.pooled_impact_estimate(x, y)
+        cf["_logit_code"] = (
+            numpy.log((numpy.maximum(cf["estimate"], 0.0) + eps)
+                      / (numpy.maximum(cf["grand_mean"], 0.0) + eps))
+        )
     else:
-        sf["_logit_code"] = numpy.log((sf["_group_mean"] + eps) / (sf["_gm"] + eps))
-    sf = sf.loc[:, ["x", "_logit_code"]].copy()
+        cf = vtreat.util.grouped_by_x_statistics(x, y)
+        cf["_logit_code"] = (
+            numpy.log((numpy.maximum(cf["_group_mean"], 0.0) + eps)
+                      / (numpy.maximum(cf["_gm"], 0.0) + eps))
+        )
+    if cf.shape[0] <= 1:
+        return None
+    sf = cf.loc[:, ["x", "_logit_code"]].reset_index(drop=True, inplace=False)
     newcol = incoming_column_name + "_logit_code" + var_suffix
     sf.columns = [incoming_column_name, newcol]
     return YAwareMappedCodeTransform(
         incoming_column_name=incoming_column_name,
         derived_column_name=newcol,
         treatment="logit_code",
         code_book=sf,
@@ -720,16 +734,16 @@
     bad_posns = vtreat.util.is_bad(sf["x"])
     sf.loc[bad_posns, "x"] = bad_sentinel
     sf.reset_index(inplace=True, drop=True)
     n = sf.shape[0]
     sf["_ni"] = 1.0
     sf = pandas.DataFrame(sf.groupby("x")["_ni"].sum())
     sf.reset_index(inplace=True, drop=False)
-    sf["_hest"] = sf["_ni"] / n
-    sf = sf.loc[:, ["x", "_hest"]].copy()
+    sf["_prev"] = sf["_ni"] / n
+    sf = sf.loc[:, ["x", "_prev"]].copy()
     newcol = incoming_column_name + "_prevalence_code"
     sf.columns = [incoming_column_name, newcol]
     sf[incoming_column_name] = sf[incoming_column_name].astype(str)
     sf.reset_index(inplace=True, drop=True)
     return MappedCodeTransform(
         incoming_column_name=incoming_column_name,
         derived_column_name=newcol,
```

### Comparing `vtreat-1.2.7/vtreat.egg-info/PKG-INFO` & `vtreat-1.2.8/vtreat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtreat
-Version: 1.2.7
+Version: 1.2.8
 Summary: vtreat is a pandas.DataFrame processor/conditioner that prepares real-world data for predictive modeling in a statistically sound manner. 
 Home-page: https://github.com/WinVector/pyvtreat
 Author: John Mount, Nina Zumel
 Author-email: jmount@win-vector.com
 License: License :: OSI Approved :: BSD 3-clause License
 Platform: any
 Classifier: Intended Audience :: Science/Research
```

