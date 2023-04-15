# Comparing `tmp/statgis-1.0.5.tar.gz` & `tmp/statgis-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statgis-1.0.5.tar", max compression
+gzip compressed data, was "statgis-1.0.6.tar", max compression
```

## Comparing `statgis-1.0.5.tar` & `statgis-1.0.6.tar`

### file list

```diff
@@ -1,37 +1,20 @@
--rw-r--r--   0        0        0     1133 2023-01-19 20:42:33.999376 statgis-1.0.5/LICENSE
--rw-r--r--   0        0        0      865 2023-01-22 18:39:16.900951 statgis-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     1469 2023-01-22 18:02:01.027304 statgis-1.0.5/README.md
--rw-r--r--   0        0        0      159 2023-01-22 04:19:42.281203 statgis-1.0.5/src/statgis/__init__.py
--rw-r--r--   0        0        0      283 2023-01-22 16:39:50.776767 statgis-1.0.5/src/statgis/gee/__init__.py
--rw-r--r--   0        0        0      656 2023-01-22 16:43:43.864697 statgis-1.0.5/src/statgis/gee/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6821 2023-01-22 06:03:24.306629 statgis-1.0.5/src/statgis/gee/__pycache__/classification.cpython-311.pyc
--rw-r--r--   0        0        0      648 2023-01-22 04:11:08.525705 statgis-1.0.5/src/statgis/gee/__pycache__/gee.cpython-311.pyc
--rw-r--r--   0        0        0     2672 2023-01-19 23:37:31.470144 statgis-1.0.5/src/statgis/gee/__pycache__/landsat_functions.cpython-311.pyc
--rw-r--r--   0        0        0     4264 2023-01-22 16:43:49.927975 statgis-1.0.5/src/statgis/gee/__pycache__/river_analysis.cpython-311.pyc
--rw-r--r--   0        0        0     4263 2023-01-22 04:11:13.247472 statgis-1.0.5/src/statgis/gee/__pycache__/riveranalysis.cpython-311.pyc
--rw-r--r--   0        0        0     3799 2023-01-22 02:31:39.794755 statgis-1.0.5/src/statgis/gee/__pycache__/sample.cpython-311.pyc
--rw-r--r--   0        0        0     1742 2023-01-22 01:07:56.799972 statgis-1.0.5/src/statgis/gee/__pycache__/sentinel_functions.cpython-311.pyc
--rw-r--r--   0        0        0     2461 2023-01-22 16:43:53.878855 statgis-1.0.5/src/statgis/gee/__pycache__/shoreline_analysis.cpython-311.pyc
--rw-r--r--   0        0        0     2460 2023-01-22 04:11:17.550919 statgis-1.0.5/src/statgis/gee/__pycache__/shorelineanalysis.cpython-311.pyc
--rw-r--r--   0        0        0     2152 2023-01-22 16:43:55.696597 statgis-1.0.5/src/statgis/gee/__pycache__/terrain_analysis.cpython-311.pyc
--rw-r--r--   0        0        0     2151 2023-01-22 04:00:53.661489 statgis-1.0.5/src/statgis/gee/__pycache__/terrainanalysis.cpython-311.pyc
--rw-r--r--   0        0        0    17438 2023-01-20 03:42:57.455096 statgis-1.0.5/src/statgis/gee/__pycache__/time_series_analysis.cpython-311.pyc
--rw-r--r--   0        0        0     6967 2023-01-20 05:12:46.421154 statgis-1.0.5/src/statgis/gee/__pycache__/zonal_statistics.cpython-311.pyc
--rw-r--r--   0        0        0     4291 2023-01-22 05:56:39.148791 statgis-1.0.5/src/statgis/gee/classification.py
--rw-r--r--   0        0        0     1426 2023-01-19 23:31:18.454505 statgis-1.0.5/src/statgis/gee/landsat_functions.py
--rw-r--r--   0        0        0     2816 2023-01-22 04:02:19.964674 statgis-1.0.5/src/statgis/gee/river_analysis.py
--rw-r--r--   0        0        0     1904 2023-01-22 18:06:53.792186 statgis-1.0.5/src/statgis/gee/sample.py
--rw-r--r--   0        0        0      932 2023-01-20 20:06:03.991306 statgis-1.0.5/src/statgis/gee/sentinel_functions.py
--rw-r--r--   0        0        0     1334 2023-01-22 03:59:26.799302 statgis-1.0.5/src/statgis/gee/shoreline_analysis.py
--rw-r--r--   0        0        0     1238 2023-01-22 18:07:52.711943 statgis-1.0.5/src/statgis/gee/terrain_analysis.py
--rw-r--r--   0        0        0     9634 2023-01-22 18:08:36.077520 statgis-1.0.5/src/statgis/gee/time_series_analysis.py
--rw-r--r--   0        0        0     4616 2023-01-22 18:26:15.538063 statgis-1.0.5/src/statgis/gee/zonal_statistics.py
--rw-r--r--   0        0        0        0 2023-01-22 04:11:57.687403 statgis-1.0.5/src/statgis/statgis.py
--rw-r--r--   0        0        0       42 2023-01-22 04:20:19.996256 statgis-1.0.5/src/statgis/statutils/__init__.py
--rw-r--r--   0        0        0      260 2023-01-22 04:21:17.105379 statgis-1.0.5/src/statgis/statutils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4338 2023-01-22 05:47:01.520052 statgis-1.0.5/src/statgis/statutils/__pycache__/plots.cpython-311.pyc
--rw-r--r--   0        0        0     2689 2023-01-22 05:53:06.185590 statgis-1.0.5/src/statgis/statutils/__pycache__/stats.cpython-311.pyc
--rw-r--r--   0        0        0     3411 2023-01-22 18:37:51.619887 statgis-1.0.5/src/statgis/statutils/plots.py
--rw-r--r--   0        0        0     1970 2023-01-22 18:38:18.763212 statgis-1.0.5/src/statgis/statutils/stats.py
--rw-r--r--   0        0        0     2268 1970-01-01 00:00:00.000000 statgis-1.0.5/setup.py
--rw-r--r--   0        0        0     2104 1970-01-01 00:00:00.000000 statgis-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1133 2023-04-15 01:57:54.839842 statgis-1.0.6/LICENSE
+-rw-r--r--   0        0        0      890 2023-04-15 20:15:51.780807 statgis-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1469 2023-04-15 01:57:54.871115 statgis-1.0.6/README.md
+-rw-r--r--   0        0        0      159 2023-04-15 01:57:55.092860 statgis-1.0.6/src/statgis/__init__.py
+-rw-r--r--   0        0        0      283 2023-04-15 01:57:55.095862 statgis-1.0.6/src/statgis/gee/__init__.py
+-rw-r--r--   0        0        0     4291 2023-04-15 01:57:55.096863 statgis-1.0.6/src/statgis/gee/classification.py
+-rw-r--r--   0        0        0     1426 2023-04-15 01:57:55.103864 statgis-1.0.6/src/statgis/gee/landsat_functions.py
+-rw-r--r--   0        0        0     2816 2023-04-15 01:57:55.401621 statgis-1.0.6/src/statgis/gee/river_analysis.py
+-rw-r--r--   0        0        0     1904 2023-04-15 01:57:55.401621 statgis-1.0.6/src/statgis/gee/sample.py
+-rw-r--r--   0        0        0      932 2023-04-15 01:57:55.401621 statgis-1.0.6/src/statgis/gee/sentinel_functions.py
+-rw-r--r--   0        0        0     1334 2023-04-15 01:57:55.401621 statgis-1.0.6/src/statgis/gee/shoreline_analysis.py
+-rw-r--r--   0        0        0     1238 2023-04-15 01:57:55.417245 statgis-1.0.6/src/statgis/gee/terrain_analysis.py
+-rw-r--r--   0        0        0    10834 2023-04-15 20:05:41.515042 statgis-1.0.6/src/statgis/gee/time_series_analysis.py
+-rw-r--r--   0        0        0     1835 2023-04-15 05:14:49.801143 statgis-1.0.6/src/statgis/gee/utils.py
+-rw-r--r--   0        0        0     4616 2023-04-15 01:57:55.417245 statgis-1.0.6/src/statgis/gee/zonal_statistics.py
+-rw-r--r--   0        0        0        0 2023-04-15 01:57:55.417245 statgis-1.0.6/src/statgis/statgis.py
+-rw-r--r--   0        0        0       42 2023-04-15 01:57:55.471047 statgis-1.0.6/src/statgis/statutils/__init__.py
+-rw-r--r--   0        0        0     3408 2023-04-15 04:08:25.691314 statgis-1.0.6/src/statgis/statutils/plots.py
+-rw-r--r--   0        0        0     1970 2023-04-15 01:57:55.526062 statgis-1.0.6/src/statgis/statutils/stats.py
+-rw-r--r--   0        0        0     2145 1970-01-01 00:00:00.000000 statgis-1.0.6/PKG-INFO
```

### Comparing `statgis-1.0.5/LICENSE` & `statgis-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `statgis-1.0.5/pyproject.toml` & `statgis-1.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "statgis"
-version = "1.0.5"
+version = "1.0.6"
 description = "Tools for improve work with geospatial data in Python"
-authors = ["Sebástian Narváez-Salcedo", "Brayan Navarro-Londoño"]
+authors = ["Sebástian Narváez-Salcedo <sanarvaezstatgis@gmail.com>", "Brayan Navarro-Londoño <brnavarrostatgis@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "<3.12,>=3.8"
 earthengine-api = ">=0.1.335"
 pandas = ">=1.3.5"
@@ -21,13 +21,12 @@
 pytest-cov = ">=4.0.0"
 jupyterlab = ">=3.5.2"
 ipykernel = ">=6.20.2"
 myst-nb = {version = "^0.17.1", python = "^3.11"}
 sphinx-autoapi = "^2.0.1"
 sphinx-rtd-theme = "^1.1.1"
 sphinxcontrib-napoleon = "^0.7"
-pydata-sphinx-theme = "^0.12.0"
 sphinx-material = "^0.0.35"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `statgis-1.0.5/README.md` & `statgis-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `statgis-1.0.5/src/statgis/gee/classification.py` & `statgis-1.0.6/src/statgis/gee/classification.py`

 * *Files identical despite different names*

### Comparing `statgis-1.0.5/src/statgis/gee/landsat_functions.py` & `statgis-1.0.6/src/statgis/gee/landsat_functions.py`

 * *Files identical despite different names*

### Comparing `statgis-1.0.5/src/statgis/gee/river_analysis.py` & `statgis-1.0.6/src/statgis/gee/river_analysis.py`

 * *Files identical despite different names*

### Comparing `statgis-1.0.5/src/statgis/gee/sample.py` & `statgis-1.0.6/src/statgis/gee/sample.py`

 * *Files identical despite different names*

### Comparing `statgis-1.0.5/src/statgis/gee/sentinel_functions.py` & `statgis-1.0.6/src/statgis/gee/sentinel_functions.py`

 * *Files identical despite different names*

### Comparing `statgis-1.0.5/src/statgis/gee/shoreline_analysis.py` & `statgis-1.0.6/src/statgis/gee/shoreline_analysis.py`

 * *Files identical despite different names*

### Comparing `statgis-1.0.5/src/statgis/gee/terrain_analysis.py` & `statgis-1.0.6/src/statgis/gee/terrain_analysis.py`

 * *Files identical despite different names*

### Comparing `statgis-1.0.5/src/statgis/gee/time_series_analysis.py` & `statgis-1.0.6/src/statgis/gee/time_series_analysis.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 """Functions to process image collections as time series"""
 import ee
 import pandas as pd
 
-
 ee.Initialize()
 
 
-def extract_dates(image_collection: ee.ImageCollection) -> pd.Series:
+def extract_dates(image_collection: ee.ImageCollection) -> pd.DatetimeIndex:
     """
     Extract dates from all images in an image collection.
 
     Parameters
     ----------
     image_collection : ee.ImageCollection
-        Colletion of image.
+        Collection of image.
 
     Returns
     -------
     dates : pd.Series
         Series with the dates of the images.
     """
     dates = (
         image_collection.reduceColumns(ee.Reducer.toList(), ["system:time_start"])
-                        .get("list")
-                        .getInfo()
+        .get("list")
+        .getInfo()
     )
 
     dates = pd.DatetimeIndex(pd.to_datetime(dates, unit="ms"))
 
     return dates
 
 
 def trend(image_collection: ee.ImageCollection, band: str) -> ee.ImageCollection:
     """
-    Calculate the linear trend and stational variation to an image collection.
+    Calculate the linear trend and seasonal variation to an image collection.
 
     Parameters
     ----------
     image_collection : ee.imageCollection
         Image collection to perform the linear trend and detrend.
 
     band : str
         Name of the band to perform the calc.
 
     Returns
     -------
     image_collection : ee.ImageCollection
-        Image collection with the Raw data, Time, Trend and Stational variation bands.
+        Image collection with the Raw data, Time, Trend and seasonal variation bands.
     """
+
     def time_func(image: ee.Image) -> ee.Image:
         """Calculate time band for linear regression"""
         time = (
             image.metadata("system:time_start")
-                 .divide(1000*60*60*24*365)
-                 .rename("time")
+            .divide(1000 * 60 * 60 * 24 * 365)
+            .rename("time")
         )
 
         return image.addBands(time)
 
     mean = image_collection.select(band).mean()
 
     image_collection = image_collection.map(time_func)
@@ -65,137 +65,168 @@
 
     fitted = image_collection.reduce(ee.Reducer.linearFit())
 
     def pred_func(image: ee.Image) -> ee.Image:
         """Calculate linear regression"""
         pred = (
             image.select("time")
-                 .multiply(fitted.select("scale"))
-                 .add(fitted.select("offset"))
-                 .rename("predicted")
-                 .toFloat()
+            .multiply(fitted.select("scale"))
+            .add(fitted.select("offset"))
+            .rename("predicted")
+            .toFloat()
         )
 
         return image.addBands(pred)
 
     def stat_func(image: ee.Image) -> ee.Image:
-        """Calculate the stational component"""
+        """Calculate the seasonal component"""
         stat = image.expression(
             "band - pred + mean",
             {
-                "band":image.select(band),
-                "pred":image.select("predicted"),
-                "mean":mean,
+                "band": image.select(band),
+                "pred": image.select("predicted"),
+                "mean": mean,
             },
         ).rename("detrended").toFloat()
 
         return image.addBands(stat)
 
     image_collection = image_collection.map(pred_func).map(stat_func)
 
     return image_collection
 
 
-def reduce_by_year(
+def resample(
     image_collection: ee.ImageCollection,
     reducer: ee.Reducer,
-    start: int,
-    end: int,
+    scale: str,
 ) -> ee.ImageCollection:
     """
-    Resample image collection to annual reduced collection.
+    Function to resample an Image Collection to a fixed timestamp.
 
     Parameters
     ----------
     image_collection : ee.ImageCollection
-        Image collection to reduce.
+        Image Collection to resample.
 
     reducer : ee.Reducer
-        Reducer to apply throught the image collection.
+        To aggregate the images
 
-    start : int
-        First year.
-
-    end : int
-        Last year.
+    scale : str
+        Time scale to aggregate the image, must be one from:
+        - annual.
+        - monthly.
+        - monthly-stat.
+        - monthly-stat-repeated.
 
     Returns
     -------
-    annual_collection : ee.ImageCollection
-        Image collection reduced to annual frequency.
+    final_collection : ee.ImageCollection
+        Collection resampled.
     """
-    annual_collection = []
 
-    for year in range(start, end+1):
-        img = (
-            image_collection.filter(ee.Filter.calendarRange(year, year, "year"))
-                            .reduce(reducer)
-                            .set("year", year)
-        )
+    dates = image_collection.reduceColumns(
+        reducer=ee.Reducer.min().combine(ee.Reducer.max(), sharedInputs=True),
+        selectors=["system:time_start"],
+    ).getInfo()
 
-        annual_collection.append(img)
+    for key, val in dates.items():
+        dates[key] = ee.Date(val).get("year").getInfo()
 
-    return ee.ImageCollection(annual_collection)
+    months = range(1, 13)
+    years = range(dates["min"], dates["max"] + 1)
 
+    band_names = image_collection.first().bandNames()
 
-def reduce_by_month(
-    image_collection: ee.ImageCollection,
-    reducer: ee.Reducer,
-) -> ee.ImageCollection:
-    """
-    Reduce image collection to monthly statistic.
+    final_collection = []
 
-    Parameters
-    ----------
-    image_collection : ee.ImageCollection
-        Image collection to reduce.
+    if scale == "annual":
+        for year in years:
+            date = ee.Date.fromYMD(year, 1, 1).millis()
 
-    reducer : ee.Reducer
-        Reducer to apply throught image collection.
+            image = (
+                image_collection.filter(ee.Filter.calendarRange(year, year, "year"))
+                .reduce(reducer, 4)
+                .set("year", year)
+                .set("system:time_start", date)
+            )
 
-    Returns
-    -------
-    monthly_collection : ee.ImageCollection
-        Image collection reduced to monthly frequency.
-    """
-    monthly_collection = []
+            final_collection.append(image)
 
-    for month in range(1, 13):
-        img = (
-            image_collection.filter(ee.Filter.calendarRange(month, month, "month"))
-                            .reduce(reducer)
-                            .rename("seasonal")
-                            .set("month", month)
-        )
+    elif scale == "monthly":
+        for year in years:
+            for month in months:
+                date = ee.Date.fromYMD(year, month, 1).millis()
+
+                image = (
+                    image_collection.filter(ee.Filter.calendarRange(year, year, "year"))
+                    .filter(ee.Filter.calendarRange(month, month, "month"))
+                    .reduce(reducer, 4)
+                    .set("year", year)
+                    .set("month", month)
+                    .set("system:time_start", date)
+                )
+
+                final_collection.append(image)
+
+    elif scale == "monthly-stat":
+        for month in months:
+            image = (
+                image_collection.filter(ee.Filter.calendarRange(month, month, "month"))
+                .reduce(reducer, 4)
+                .set("month", month)
+            )
+
+            final_collection.append(image)
 
-        monthly_collection.append(img)
+    elif scale == "monthly-stat-repeated":
+        for year in years:
+            for month in months:
+                date = ee.Date.fromYMD(year, month, 1).millis()
 
-    return ee.ImageCollection(monthly_collection)
+                image = (
+                    image_collection.filter(ee.Filter.calendarRange(month, month, "month"))
+                    .reduce(reducer, 4)
+                    .set("year", year)
+                    .set("month", month)
+                    .set("system:time_start", date)
+                )
+
+                final_collection.append(image)
+
+    else:
+        Exception("ERROR")
+
+    final_collection = ee.ImageCollection(final_collection).map(lambda img: img.rename(band_names))
+
+    return final_collection
 
 
 def calculate_anomalies(
-    image_collection: ee.ImageCollection, monthly_mean: ee.ImageCollection
+    image_collection: ee.ImageCollection,
+    monthly_mean: ee.ImageCollection
 ) -> ee.ImageCollection:
     """
     Calculate the anomalies of a ImageCollection subtracting the monthly mean values.
 
     Parameters
     ----------
     image_collection : ee.ImageCollection
         Image collection trended by the trend function to calc the anomalies.
 
     monthly_mean : ee.ImageCollection
         Image collection with the monthly means of ImageCollection calculated by the
-        `reduce_by_month` function.
+        `resample()` function.
 
     Returns
     -------
     anomalies : ee.ImageCollection
-        ImageCollection with stational means added and anomalies calcualted.
+        ImageCollection with seasonal means added and anomalies calculated.
     """
+
     def calc_anomaly(image: ee.Image) -> ee.Image:
         """Function for calculate anomalies."""
         anomaly = image.expression(
             "stat - mean",
             {"stat": image.select("detrended"), "mean": image.select("seasonal")},
         ).rename("anomaly")
 
@@ -236,61 +267,61 @@
     )
     m12 = image_collection.filter(ee.Filter.calendarRange(12, 12, "month")).map(
         lambda x: x.addBands(monthly_mean.filter(ee.Filter.eq("month", 12)).first())
     )
 
     anomalies = (
         m01.merge(m02)
-           .merge(m03)
-           .merge(m04)
-           .merge(m05)
-           .merge(m06)
-           .merge(m07)
-           .merge(m08)
-           .merge(m09)
-           .merge(m10)
-           .merge(m11)
-           .merge(m12)
+        .merge(m03)
+        .merge(m04)
+        .merge(m05)
+        .merge(m06)
+        .merge(m07)
+        .merge(m08)
+        .merge(m09)
+        .merge(m10)
+        .merge(m11)
+        .merge(m12)
     )
 
     anomalies = anomalies.sort("system:time_start")
     anomalies = anomalies.map(calc_anomaly)
 
     return anomalies
 
 
 def time_series_processing(
     image_collection: ee.ImageCollection, band: str
-) -> list:
+) -> tuple[ee.ImageCollection, ee.ImageCollection]:
     """
     This function take an ee.ImageCollection and calculate the linear trend, the
     detrended component, the seasonal mean and anomalies for the selected band.
     To calculate the linear trend the function use `ee.Reducer.linearFit()`, next,
     calculate the detrended component subtracting the linear_fitted values to the
-    original series and restoring its mean, the monthly means are calculeted by
+    original series and restoring its mean, the monthly means are calculated by
     selecting all the image in the specific month and reduce it by its mean, finally,
     subtracting the monthly means to the detrended component anomalies are obtained.
-    This function work as a "wrapper" function of `trend()`, `reduce_by_month()` and
+    This function work as a "wrapper" function of `trend()`, `resample()` and
     `calc_anomalies()`.
 
     Parameters
     ----------
     image_collection : ee.ImageCollection
-        Image collection to proces.
+        Image collection to process.
 
     band : str
         Name of the band of interest.
 
     Returns
     -------
     data : ee.ImageCollection
-        Image collection with the raw data, the linear trend, deternded component,
+        Image collection with the raw data, the linear trend, detrended component,
         seasonal mean and the anomalies.
 
     monthly_mean : ee.ImageCollection
         Image collection with the twelves monthly means calculated.
     """
     trended = trend(image_collection, band)
-    monthly_mean = reduce_by_month(trended.select("detrended"), ee.Reducer.mean())
+    monthly_mean = resample(trended.select("detrended"), ee.Reducer.mean(), "monthly-stat")
     data = calculate_anomalies(trended, monthly_mean)
 
     return data, monthly_mean
```

### Comparing `statgis-1.0.5/src/statgis/gee/zonal_statistics.py` & `statgis-1.0.6/src/statgis/gee/zonal_statistics.py`

 * *Files identical despite different names*

### Comparing `statgis-1.0.5/src/statgis/statutils/plots.py` & `statgis-1.0.6/src/statgis/statutils/plots.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-"""Submodule for genarate statistical plots"""
+"""Submodule for generate statistical plots"""
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from typing import Union
 from matplotlib.axes import Axes
 from matplotlib.ticker import NullLocator
 from numpy.typing import ArrayLike
 from .stats import corr_matrix
 
 
 def plot_corr_matrix(
     data: pd.DataFrame,
     variables: Union[ArrayLike, None] = None,
     half: bool = False,
-    hide_insignificants: bool = False,
+    hide_insignificant: bool = False,
     significant_threshold: float = 0.05,
     show_labels: bool = True,
     show_colorbar: bool = False,
     palette: str = "Spectral",
     text_color: str = "black",
     ax: Union[Axes, None] = None,
 ) -> Axes:
@@ -30,56 +30,56 @@
         Dataframe with the variables to evaluate their correlation.
 
     variables : ArrayLike | None = None
         The variables of interest, if it is not defined, all variables in
         the dataframe will be evaluated.
 
     half : bool (optional)
-        If True, only show the corerlation of the first half of the matrix,
+        If True, only show the correlation of the first half of the matrix,
         excluding the repeated correlation.
 
-    hide_insignifcants : bool (optional)
+    hide_insignificant : bool (optional)
         If True, hide all the correlation with a p-value greater than the
         significant threshold.
 
     significant_threshold : float (optional)
         Threshold of significant correlation.
 
     show_labels : bool (optional)
         Show the correlation value.
 
     show_colorbar : bool (optional)
-        Show colorbar
+        Show color-bar
 
     palette : str (optional)
         Color palette for correlation plot.
 
     text_color : str (optional)
         Color of text correlation labels.
 
     ax : matplotlib.axes.Axes | None (optional)
         Axes to draw the correlation matrix.
     returns
     -------
     ax : matplotlib.axes.Axes
-        Correltion matrix.
+        Correlation matrix.
     """
     # If variables are not defined get all columns from data
     if variables is None:
         variables = data.columns
 
     # Get the number of variables
-    N = len(variables)
+    n = len(variables)
 
     # Reverse variables for plot
     reverse = variables[::-1]
 
     # Get the correlation matrix
     corr = corr_matrix(
-        data, variables, half, hide_insignificants, significant_threshold
+        data, variables, half, hide_insignificant, significant_threshold
     )
 
     # If there not axes create one
     if ax is None:
         fig = plt.figure()
         ax = fig.add_subplot(1, 1, 1)
 
@@ -87,21 +87,21 @@
     im = ax.pcolormesh(
         variables, reverse, corr, cmap=palette, edgecolor="w", vmin=-1, vmax=1
     )
 
     # Invert y axis
     ax.invert_yaxis()
 
-    # Add the colorbar
+    # Add the color-bar
     if show_colorbar:
         cax = ax.inset_axes([1.04, 0.1, 0.05, 0.8])
-        bar = plt.colorbar(im, cax=cax, label="Correlation")
+        plt.colorbar(im, cax=cax, label="Correlation")
 
     if show_labels:
-        x, y = np.meshgrid(np.arange(N), np.arange(N))
+        x, y = np.meshgrid(np.arange(n), np.arange(n))
         x = x.reshape(-1)
         y = y.reshape(-1)
         t = corr.values.reshape(-1)
 
         for xi, yi, ti in zip(x, y, t):
             if np.isfinite(ti):
                 ax.text(
@@ -112,8 +112,8 @@
                     ha="center",
                     va="center",
                 )
 
     ax.xaxis.set_minor_locator(NullLocator())
     ax.yaxis.set_minor_locator(NullLocator())
 
-    return ax
+    return ax
```

### Comparing `statgis-1.0.5/src/statgis/statutils/stats.py` & `statgis-1.0.6/src/statgis/statutils/stats.py`

 * *Files identical despite different names*

### Comparing `statgis-1.0.5/PKG-INFO` & `statgis-1.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: statgis
-Version: 1.0.5
+Version: 1.0.6
 Summary: Tools for improve work with geospatial data in Python
 License: MIT
 Author: Sebástian Narváez-Salcedo
+Author-email: sanarvaezstatgis@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

