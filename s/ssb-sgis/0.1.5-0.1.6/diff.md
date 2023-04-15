# Comparing `tmp/ssb_sgis-0.1.5.tar.gz` & `tmp/ssb_sgis-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_sgis-0.1.5.tar", max compression
+gzip compressed data, was "ssb_sgis-0.1.6.tar", max compression
```

## Comparing `ssb_sgis-0.1.5.tar` & `ssb_sgis-0.1.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1074 2023-04-12 19:35:11.603711 ssb_sgis-0.1.5/LICENSE
--rw-r--r--   0        0        0     7070 2023-04-12 19:35:11.603711 ssb_sgis-0.1.5/README.md
--rw-r--r--   0        0        0     2477 2023-04-12 19:35:28.572292 ssb_sgis-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1651 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/__init__.py
--rw-r--r--   0        0        0     2634 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/dapla.py
--rw-r--r--   0        0        0      666 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/geopandas_tools/__init__.py
--rw-r--r--   0        0        0     8776 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/geopandas_tools/buffer_dissolve_explode.py
--rw-r--r--   0        0        0    27649 2023-04-12 19:35:28.576292 ssb_sgis-0.1.5/src/sgis/geopandas_tools/general.py
--rw-r--r--   0        0        0     5456 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/geopandas_tools/geometry_types.py
--rw-r--r--   0        0        0    34762 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/geopandas_tools/line_operations.py
--rw-r--r--   0        0        0    16647 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/geopandas_tools/neighbors.py
--rw-r--r--   0        0        0    14435 2023-04-12 19:35:28.576292 ssb_sgis-0.1.5/src/sgis/geopandas_tools/overlay.py
--rw-r--r--   0        0        0     6316 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/geopandas_tools/point_operations.py
--rw-r--r--   0        0        0     5046 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/geopandas_tools/polygon_operations.py
--rw-r--r--   0        0        0     2468 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/helpers.py
--rw-r--r--   0        0        0        0 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/maps/__init__.py
--rw-r--r--   0        0        0    23159 2023-04-12 19:35:28.576292 ssb_sgis-0.1.5/src/sgis/maps/explore.py
--rw-r--r--   0        0        0    20458 2023-04-12 19:35:28.576292 ssb_sgis-0.1.5/src/sgis/maps/legend.py
--rw-r--r--   0        0        0    16402 2023-04-12 19:35:28.576292 ssb_sgis-0.1.5/src/sgis/maps/map.py
--rw-r--r--   0        0        0    12564 2023-04-12 19:35:28.576292 ssb_sgis-0.1.5/src/sgis/maps/maps.py
--rw-r--r--   0        0        0    13220 2023-04-12 19:35:28.576292 ssb_sgis-0.1.5/src/sgis/maps/thematicmap.py
--rw-r--r--   0        0        0        0 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/networkanalysis/__init__.py
--rw-r--r--   0        0        0     5171 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/networkanalysis/_get_route.py
--rw-r--r--   0        0        0     2521 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/networkanalysis/_od_cost_matrix.py
--rw-r--r--   0        0        0     4819 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/networkanalysis/_points.py
--rw-r--r--   0        0        0     4426 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/networkanalysis/_service_area.py
--rw-r--r--   0        0        0    11360 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/networkanalysis/directednetwork.py
--rw-r--r--   0        0        0    23953 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/networkanalysis/network.py
--rw-r--r--   0        0        0     6124 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/networkanalysis/network_norway.py
--rw-r--r--   0        0        0    58054 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/networkanalysis/networkanalysis.py
--rw-r--r--   0        0        0    12655 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/networkanalysis/networkanalysisrules.py
--rw-r--r--   0        0        0        0 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/py.typed
--rw-r--r--   0        0        0     3765 2023-04-12 19:35:11.639712 ssb_sgis-0.1.5/src/sgis/read_parquet.py
--rw-r--r--   0        0        0     8434 1970-01-01 00:00:00.000000 ssb_sgis-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-15 12:26:09.075918 ssb_sgis-0.1.6/LICENSE
+-rw-r--r--   0        0        0     7260 2023-04-15 12:26:26.071902 ssb_sgis-0.1.6/README.md
+-rw-r--r--   0        0        0     2477 2023-04-15 12:26:26.075902 ssb_sgis-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1651 2023-04-15 12:26:09.107918 ssb_sgis-0.1.6/src/sgis/__init__.py
+-rw-r--r--   0        0        0     2634 2023-04-15 12:26:09.107918 ssb_sgis-0.1.6/src/sgis/dapla.py
+-rw-r--r--   0        0        0      666 2023-04-15 12:26:09.107918 ssb_sgis-0.1.6/src/sgis/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:26:09.107918 ssb_sgis-0.1.6/src/sgis/geopandas_tools/__init__.py
+-rw-r--r--   0        0        0     8776 2023-04-15 12:26:09.107918 ssb_sgis-0.1.6/src/sgis/geopandas_tools/buffer_dissolve_explode.py
+-rw-r--r--   0        0        0    27590 2023-04-15 12:26:26.075902 ssb_sgis-0.1.6/src/sgis/geopandas_tools/general.py
+-rw-r--r--   0        0        0     5480 2023-04-15 12:26:26.075902 ssb_sgis-0.1.6/src/sgis/geopandas_tools/geometry_types.py
+-rw-r--r--   0        0        0    34748 2023-04-15 12:26:26.075902 ssb_sgis-0.1.6/src/sgis/geopandas_tools/line_operations.py
+-rw-r--r--   0        0        0    16647 2023-04-15 12:26:09.111918 ssb_sgis-0.1.6/src/sgis/geopandas_tools/neighbors.py
+-rw-r--r--   0        0        0    14435 2023-04-15 12:26:09.111918 ssb_sgis-0.1.6/src/sgis/geopandas_tools/overlay.py
+-rw-r--r--   0        0        0     6316 2023-04-15 12:26:09.111918 ssb_sgis-0.1.6/src/sgis/geopandas_tools/point_operations.py
+-rw-r--r--   0        0        0     5046 2023-04-15 12:26:09.111918 ssb_sgis-0.1.6/src/sgis/geopandas_tools/polygon_operations.py
+-rw-r--r--   0        0        0     2468 2023-04-15 12:26:09.111918 ssb_sgis-0.1.6/src/sgis/helpers.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:26:09.111918 ssb_sgis-0.1.6/src/sgis/maps/__init__.py
+-rw-r--r--   0        0        0    19148 2023-04-15 12:26:26.075902 ssb_sgis-0.1.6/src/sgis/maps/explore.py
+-rw-r--r--   0        0        0    20499 2023-04-15 12:26:26.075902 ssb_sgis-0.1.6/src/sgis/maps/legend.py
+-rw-r--r--   0        0        0    16402 2023-04-15 12:26:09.111918 ssb_sgis-0.1.6/src/sgis/maps/map.py
+-rw-r--r--   0        0        0    12747 2023-04-15 12:26:26.075902 ssb_sgis-0.1.6/src/sgis/maps/maps.py
+-rw-r--r--   0        0        0    14092 2023-04-15 12:26:26.075902 ssb_sgis-0.1.6/src/sgis/maps/thematicmap.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:26:09.111918 ssb_sgis-0.1.6/src/sgis/networkanalysis/__init__.py
+-rw-r--r--   0        0        0     7628 2023-04-15 12:26:26.075902 ssb_sgis-0.1.6/src/sgis/networkanalysis/_get_route.py
+-rw-r--r--   0        0        0     2455 2023-04-15 12:26:26.075902 ssb_sgis-0.1.6/src/sgis/networkanalysis/_od_cost_matrix.py
+-rw-r--r--   0        0        0     4182 2023-04-15 12:26:26.075902 ssb_sgis-0.1.6/src/sgis/networkanalysis/_points.py
+-rw-r--r--   0        0        0     4426 2023-04-15 12:26:09.111918 ssb_sgis-0.1.6/src/sgis/networkanalysis/_service_area.py
+-rw-r--r--   0        0        0    11354 2023-04-15 12:26:26.075902 ssb_sgis-0.1.6/src/sgis/networkanalysis/directednetwork.py
+-rw-r--r--   0        0        0    23771 2023-04-15 12:26:26.075902 ssb_sgis-0.1.6/src/sgis/networkanalysis/network.py
+-rw-r--r--   0        0        0     6124 2023-04-15 12:26:09.111918 ssb_sgis-0.1.6/src/sgis/networkanalysis/network_norway.py
+-rw-r--r--   0        0        0    67522 2023-04-15 12:26:26.075902 ssb_sgis-0.1.6/src/sgis/networkanalysis/networkanalysis.py
+-rw-r--r--   0        0        0    12692 2023-04-15 12:26:26.079902 ssb_sgis-0.1.6/src/sgis/networkanalysis/networkanalysisrules.py
+-rw-r--r--   0        0        0        0 2023-04-15 12:26:09.111918 ssb_sgis-0.1.6/src/sgis/py.typed
+-rw-r--r--   0        0        0     3765 2023-04-15 12:26:09.111918 ssb_sgis-0.1.6/src/sgis/read_parquet.py
+-rw-r--r--   0        0        0     8624 1970-01-01 00:00:00.000000 ssb_sgis-0.1.6/PKG-INFO
```

### Comparing `ssb_sgis-0.1.5/LICENSE` & `ssb_sgis-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.5/README.md` & `ssb_sgis-0.1.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 ## Network analysis examples
 
 Preparing for network analysis:
 
 ```python
 import sgis as sg
-
+import pandas as pd
 
 roads = sg.read_parquet_url(
     "https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet"
 )
 
 nw = (
     sg.DirectedNetwork(roads)
@@ -59,22 +59,31 @@
 
     NetworkAnalysis(
         network=DirectedNetwork(6364 km, percent_bidirectional=87),
         rules=NetworkAnalysisRules(weight=minutes, search_tolerance=250, search_factor=0, split_lines=False, ...),
         log=True, detailed_log=True,
     )
 
-Get number of times each line segment was visited.
+Get number of times each line segment was visited, with optional weighting.
 
 ```python
-frequencies = nwa.get_route_frequencies(points.sample(75), points.sample(75))
+origins = points.iloc[:75]
+destinations = points.iloc[75:150]
+
+# creating uniform weights of 10
+od_pairs = pd.MultiIndex.from_product([origins.index, destinations.index])
+weights = pd.DataFrame(index=od_pairs)
+weights["weight"] = 10
 
+frequencies = nwa.get_route_frequencies(origins, destinations, weight_df=weights)
+
+# plot the results
 m = sg.ThematicMap(sg.buff(frequencies, 15), column="frequency", black=True)
 m.cmap = "plasma"
-m.title = "Number of times each road was used."
+m.title = "Number of times each road was used,\nweighted * 10"
 m.plot()
 ```
 
 ![png](docs/examples/network_analysis_examples_files/network_analysis_examples_5_0.png)
 
 Fast many-to-many travel times/distances.
 
@@ -103,14 +112,15 @@
 
 ```python
 service_areas = nwa.service_area(
     points.iloc[[0]],
     breaks=np.arange(1, 11),
 )
 
+# plot the results
 m = sg.ThematicMap(service_areas, column="minutes", black=True, size=10)
 m.k = 10
 m.title = "Roads that can be reached within 1 to 10 minutes"
 m.plot()
 ```
 
 ![png](docs/examples/network_analysis_examples_files/network_analysis_examples_9_0.png)
@@ -126,16 +136,14 @@
 m.title = "Four fastest routes from A to B"
 m.legend.title = "Rank"
 m.plot()
 ```
 
 ![png](docs/examples/network_analysis_examples_files/network_analysis_examples_11_0.png)
 
-More network analysis examples can be found here: https://github.com/statisticsnorway/ssb-sgis/blob/main/docs/network_analysis_demo_template.md
-
 Road data for Norway can be downloaded here: https://kartkatalog.geonorge.no/metadata/nvdb-ruteplan-nettverksdatasett/8d0f9066-34f9-4423-be12-8e8523089313
 
 ## Developer information
 
 ### Git LFS
 
 The data in the testdata directory is stored with [Git LFS](https://git-lfs.com/).
```

### Comparing `ssb_sgis-0.1.5/pyproject.toml` & `ssb_sgis-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-sgis"
-version = "0.1.5"
+version = "0.1.6"
 description = "GIS functions used at Statistics Norway."
 authors = ["Statistics Norway <ort@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "sgis", from = "src"}]
 homepage = "https://github.com/statisticsnorway/ssb-sgis"
 repository = "https://github.com/statisticsnorway/ssb-sgis"
```

### Comparing `ssb_sgis-0.1.5/src/sgis/__init__.py` & `ssb_sgis-0.1.6/src/sgis/__init__.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.5/src/sgis/dapla.py` & `ssb_sgis-0.1.6/src/sgis/dapla.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.5/src/sgis/exceptions.py` & `ssb_sgis-0.1.6/src/sgis/exceptions.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.5/src/sgis/geopandas_tools/buffer_dissolve_explode.py` & `ssb_sgis-0.1.6/src/sgis/geopandas_tools/buffer_dissolve_explode.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.5/src/sgis/geopandas_tools/general.py` & `ssb_sgis-0.1.6/src/sgis/geopandas_tools/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -364,16 +364,16 @@
 
     >>> import sgis as sg
     >>> from shapely.geometry import Polygon
     >>> poly1 = sg.to_gdf(Polygon([(0, 0), (0, 1), (1, 1), (1, 0)]))
     >>> poly1["poly1"] = 1
     >>> line = sg.to_lines(poly1)
     >>> line
-        poly1                                           geometry
-    0      1  LINESTRING (0.00000 0.00000, 0.00000 1.00000, ...
+                                                geometry  poly1
+    0  LINESTRING (0.00000 0.00000, 0.00000 1.00000, ...      1
 
     Convert two overlapping polygons to linestrings.
 
     >>> poly2 = sg.to_gdf(Polygon([(0.5, 0.5), (0.5, 1.5), (1.5, 1.5), (1.5, 0.5)]))
     >>> poly2["poly2"] = 1
     >>> lines = sg.to_lines(poly1, poly2)
     >>> lines
@@ -381,21 +381,19 @@
     0    1.0    NaN  LINESTRING (0.00000 0.00000, 0.00000 1.00000, ...
     1    1.0    NaN  LINESTRING (0.50000 1.00000, 1.00000 1.00000, ...
     2    1.0    NaN  LINESTRING (1.00000 0.50000, 1.00000 0.00000, ...
     3    NaN    1.0      LINESTRING (0.50000 0.50000, 0.50000 1.00000)
     4    NaN    1.0  LINESTRING (0.50000 1.00000, 0.50000 1.50000, ...
     5    NaN    1.0      LINESTRING (1.00000 0.50000, 0.50000 0.50000)
 
-    Plot before and after (plots not showing in terminal).
+    Plot before and after.
 
     >>> sg.qtm(poly1, poly2)
-    <Axes: >
     >>> lines["l"] = lines.length
     >>> sg.qtm(lines, "l")
-    <Axes: >
     """
 
     if any(any(gdf.geom_type.isin(["Point", "MultiPoint"])) for gdf in gdfs):
         raise ValueError("Cannot convert points to lines.")
 
     def _shapely_geometry_to_lines(geom):
         if geom.area == 0:
```

### Comparing `ssb_sgis-0.1.5/src/sgis/geopandas_tools/geometry_types.py` & `ssb_sgis-0.1.6/src/sgis/geopandas_tools/geometry_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
     >>> gdf = gdf.dissolve()
     >>> gdf
                                                 geometry
     0  GEOMETRYCOLLECTION (POINT (0.00000 0.00000), L...
 
     >>> to_single_geom_type(gdf, "line")
-                    geometry
+                                            geometry
     2  LINESTRING (1.00000 1.00000, 2.00000 2.00000)
     """
     if not isinstance(gdf, (GeoDataFrame, GeoSeries)):
         raise TypeError(f"'gdf' should be GeoDataFrame or GeoSeries, got {type(gdf)}")
 
     # explode collections to single-typed geometries
     collections = gdf.loc[gdf.geom_type == "GeometryCollection"]
```

### Comparing `ssb_sgis-0.1.5/src/sgis/geopandas_tools/line_operations.py` & `ssb_sgis-0.1.6/src/sgis/geopandas_tools/line_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -694,15 +694,15 @@
     >>> roads.connected.value_counts()
     1.0    85638
     0.0     7757
     Name: connected, dtype: int64
 
     Fill gaps shorter than 1.1 meters.
 
-    >>> filled = sg.close_network_holes_to_deadends(roads, max_distance=1.1, max_angle=30)
+    >>> filled = sg.close_network_holes_to_deadends(roads, max_distance=1.1)
     >>> roads = sg.get_largest_component(roads)
     >>> roads.connected.value_counts()
     1.0    100315
     0.0       180
     Name: connected, dtype: int64
 
     It's not always wise to fill gaps. In the case of this data, these small gaps are
```

### Comparing `ssb_sgis-0.1.5/src/sgis/geopandas_tools/neighbors.py` & `ssb_sgis-0.1.6/src/sgis/geopandas_tools/neighbors.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.5/src/sgis/geopandas_tools/overlay.py` & `ssb_sgis-0.1.6/src/sgis/geopandas_tools/overlay.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.5/src/sgis/geopandas_tools/point_operations.py` & `ssb_sgis-0.1.6/src/sgis/geopandas_tools/point_operations.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.5/src/sgis/geopandas_tools/polygon_operations.py` & `ssb_sgis-0.1.6/src/sgis/geopandas_tools/polygon_operations.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.5/src/sgis/helpers.py` & `ssb_sgis-0.1.6/src/sgis/helpers.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.5/src/sgis/maps/explore.py` & `ssb_sgis-0.1.6/src/sgis/maps/legend.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,722 +1,586 @@
-"""Interactive map of one or more GeoDataFrames with layers that can be toggles on/off.
+"""Attributes of the legend of the ThematicMap class.
+
+The Legend class is best accessed through the 'legend' attribute of the ThematicMap
+class.
 
-This module holds the Explore class, which is the basis for the explore, samplemap and
-clipmap functions from the 'maps' module.
 """
 import warnings
-from statistics import mean
 
-import branca as bc
-import folium
 import matplotlib
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-from geopandas import GeoDataFrame
-from shapely.geometry import LineString
+from matplotlib.lines import Line2D
+from pandas import Series
 
-from ..geopandas_tools.general import clean_geoms, random_points_in_polygons
-from ..geopandas_tools.geometry_types import get_geom_type
-from .map import Map
+from ..geopandas_tools.general import points_in_bounds
 
 
 # the geopandas._explore raises a deprication warning. Ignoring for now.
 warnings.filterwarnings(
     action="ignore", category=matplotlib.MatplotlibDeprecationWarning
 )
 pd.options.mode.chained_assignment = None
 
 
-# gray for NaNs
-NAN_COLOR = "#969696"
-
-
-# cols to not show when hovering over geometries (tooltip)
-COLS_TO_DROP = ["color", "col_as_int", "geometry"]
+class Legend:
+    """Holds the general attributes of the legend in the ThematicMap class.
 
+    This class holds attributes of the 'legend' attribute of the ThematicMap class.
+    The fontsize, title_fontsize and markersize attributes are adjusted
+    according to the size attribute of the ThematicMap.
+
+    If a numeric column is used, additional attributes can be found in the
+    ContinousLegend class.
+
+    Attributes:
+        title: Legend title. Defaults to the column name if used in the
+            ThematicMap class.
+        position: The legend's x and y position in the plot, specified as a tuple of
+            x and y position between 0 and 1. E.g. position=(0.8, 0.2) for a position
+            in the bottom right corner, (0.2, 0.8) for the upper left corner.
+        fontsize: Text size of the legend labels. Defaults to the size of
+            the ThematicMap class.
+        title_fontsize: Text size of the legend title. Defaults to the
+            size * 1.2 of the ThematicMap class.
+        markersize: Size of the color circles in the legend. Defaults to the size of
+            the ThematicMap class.
+        framealpha: Transparency of the legend background.
+        edgecolor: Color of the legend border. Defaults to #0f0f0f (almost black).
+        kwargs: Stores additional keyword arguments taken by the matplotlib legend
+            method. Specify this as e.g. m.legend.kwargs["labelcolor"] = "red", where
+            'm' is the name of the ThematicMap instance. See here:
+            https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.legend.html
+
+    Examples
+    --------
+    Create ten random points with a numeric column from 0 to 9.
+
+    >>> import sgis as sg
+    >>> points = sg.random_points(10)
+    >>> points["number"] = range(10)
+    >>> points
+                    geometry  number
+    0  POINT (0.59780 0.50425)       0
+    1  POINT (0.07019 0.26167)       1
+    2  POINT (0.56475 0.15422)       2
+    3  POINT (0.87293 0.60316)       3
+    4  POINT (0.47373 0.20040)       4
+    5  POINT (0.98661 0.15614)       5
+    6  POINT (0.30951 0.77057)       6
+    7  POINT (0.47802 0.52824)       7
+    8  POINT (0.12215 0.96588)       8
+    9  POINT (0.02938 0.93467)       9
+
+    Creating the ThematicMap instance will also create the legend. Since we
+    specify a numeric column, a ContinousLegend instance is created.
+
+    >>> m = sg.ThematicMap(points, column="number")
+    >>> m.legend
+    <sgis.maps.legend.ContinousLegend object at 0x00000222206738D0>
+
+    Changing the attributes that apply to both numeric and categorical columns.
+
+    >>> m.legend.title = "Meters"
+    >>> m.legend.title_fontsize = 11
+    >>> m.legend.fontsize = 9
+    >>> m.legend.markersize = 7.5
+    >>> m.legend.position = (0.35, 0.28)
+    >>> m.plot()
+
+    Additional matplotlib keyword arguments can be specified as kwargs.
+
+    >>> m.legend.kwargs["labelcolor"] = "red"
+
+    Since we are using a numeric column, the legend is of type ContinousLegend.
+    We can therefore also access the attributes that only apply to numeric columns.
+
+    >>> m.label_sep = "to"
+    >>> m.label_suffix = "num"
+    >>> m.rounding = 2
+    >>> m.plot()
 
-# from geopandas
-_MAP_KWARGS = [
-    "location",
-    "prefer_canvas",
-    "no_touch",
-    "disable_3d",
-    "png_enabled",
-    "zoom_control",
-    "crs",
-    "zoom_start",
-    "left",
-    "top",
-    "position",
-    "min_zoom",
-    "max_zoom",
-    "min_lat",
-    "max_lat",
-    "min_lon",
-    "max_lon",
-    "max_bounds",
-]
-
+    """
 
-class Explore(Map):
     def __init__(
         self,
-        *gdfs,
-        column: str | None = None,
-        popup: bool = True,
-        max_zoom: int = 30,
-        show_in_browser: bool = False,
+        title: str | None = None,
+        labels: list[str] | None = None,
+        position: tuple[float] | None = None,
+        markersize: int | None = None,
+        fontsize: int | None = None,
+        title_fontsize: int | None = None,
+        framealpha: float = 1.0,
+        edgecolor: str = "#0f0f0f",
         **kwargs,
     ):
-        super().__init__(*gdfs, column=column, **kwargs)
-        self.popup = popup
-        self.max_zoom = max_zoom
-        self.show_in_browser = show_in_browser
-
-        if any(get_geom_type(gdf) == "mixed" for gdf in self.gdfs):
-            self._make_all_polygon()
-
-        if self._is_categorical:
-            if len(self.gdfs) == 1:
-                self._split_categories()
-        else:
-            if not self._cmap:
-                self._cmap = "viridis"
-            self.cmap_start = kwargs.pop("cmap_start", 0)
-            self.cmap_stop = kwargs.pop("cmap_stop", 256)
-
-    def explore(self, column: str | None = None, **kwargs) -> None:
-        """Interactive map of the GeoDataFrames with layers that can be toggles on/off.
-
-        It displays all the GeoDataFrames and displays them together in an interactive
-        map with a common legend. The layers can be toggled on and off.
-
-        Args:
-            column: The column to color the geometries by. Defaults to the column
-                that was specified last.
-            **kwargs: Keyword arguments to pass to geopandas.GeoDataFrame.explore, for
-                instance 'cmap' to change the colors, 'scheme' to change how the data
-                is grouped. This defaults to 'fisherjenks' for numeric data.
-
-        See also:
-            samplemap: same functionality, but shows only a random area of a given size.
-            clipmap: same functionality, but shows only the areas clipped by a given
-            mask.
-
-        Examples
-        --------
-        >>> from sgis import read_parquet_url
-        >>> roads = read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
-        >>> points = read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
-
-        Simple explore of two GeoDataFrames.
-
-        >>> from sgis import Explore
-        >>> ex = Explore(roads, points)
-        >>> ex.explore()
-
-        With column.
-
-        >>> roads["meters"] = roads.length
-        >>> points["meters"] = points.length
-        >>> ex = Explore(roads, points, column="meters")
-        >>> ex.samplemap()
-        """
-        if column:
-            self._column = column
-            self._update_column()
-            kwargs.pop("column", None)
-        self.to_show = self._gdfs
-        self._explore(**kwargs)
-
-    def samplemap(
-        self,
-        size: int = 1000,
-        column: str | None = None,
-        sample_from_first: bool = True,
-        **kwargs,
-    ) -> None:
-        """Shows an interactive map of a random area of the GeoDataFrames.
-
-        It takes a random sample point of the GeoDataFrames, and shows all geometries
-        within a given radius of this point. Displays an interactive map with a common
-        legend. The layers can be toggled on and off.
-
-        The radius to plot can be changed with the 'size' parameter.
-
-        For more info about the labeling and coloring of the map, see the explore
-        method.
-
-        Args:
-            size: the radius to buffer the sample point by before clipping with the
-                data.
-            column: The column to color the geometries by. Defaults to the column
-                that was specified last.
-            sample_from_first: If True (default), the sample point is taken from
-                the first specified GeoDataFrame. If False, all GeoDataFrames are
-                considered.
-            **kwargs: Keyword arguments to pass to geopandas.GeoDataFrame.explore, for
-                instance 'cmap' to change the colors, 'scheme' to change how the data
-                is grouped. This defaults to 'fisherjenks' for numeric data.
-
-        See also:
-            explore: same functionality, but shows the entire area of the geometries.
-            clipmap: same functionality, but shows only the areas clipped by a given
-            mask.
-        """
-        if column:
-            self._column = column
-            self._update_column()
-            kwargs.pop("column", None)
+        self.title = title
 
-        self.previous_sample_count = 0
-
-        if sample_from_first:
-            sample = self._gdfs[0].sample(1)
+        if "size" in kwargs:
+            size = kwargs.pop("size")
+            self._get_legend_sizes(size, kwargs)
         else:
-            sample = self._gdf.sample(1)
-
-        # convert lines to polygons
-        if get_geom_type(sample) == "line":
-            sample["geometry"] = sample.buffer(1)
-
-        if get_geom_type(sample) == "polygon":
-            random_point = random_points_in_polygons(sample, 1)
-
-        # if point or mixed geometries
+            self._title_fontsize = title_fontsize
+            self._fontsize = fontsize
+            self._markersize = markersize
+
+        self.framealpha = framealpha
+        self.edgecolor = edgecolor
+        self.width = kwargs.pop("width", 0.1)
+        self.height = kwargs.pop("height", 0.1)
+        self.title_color = kwargs.pop("title_color", None)
+        self.labelspacing = kwargs.pop("labelspacing", 0.8)
+
+        self.labels = labels
+        self._position = position
+        self.kwargs = kwargs
+        self._position_has_been_set = True if position else False
+
+    def _get_legend_sizes(self, size, kwargs):
+        """Adjust fontsize and markersize to size kwarg."""
+
+        if "title_fontsize" in kwargs:
+            self._title_fontsize = kwargs["title_fontsize"]
+            self._title_fontsize_has_been_set = True
         else:
-            random_point = sample.centroid
-
-        gdfs: tuple[GeoDataFrame] = ()
-        for gdf in self._gdfs:
-            gdf = gdf.clip(random_point.buffer(size))
-            gdfs = gdfs + (gdf,)
-        self._gdfs = gdfs
-        self._gdf = pd.concat(gdfs, ignore_index=True)
-        self._explore(**kwargs)
-
-    def clipmap(
-        self,
-        mask,
-        column: str | None = None,
-        **kwargs,
-    ) -> None:
-        """Shows an interactive map of a of the GeoDataFrames clipped by the mask.
-
-        It clips all the GeoDataFrames in the Explore instance to the mask extent,
-        and displays the resulting geometries in an interactive map with a common
-        legends. The layers can be toggled on and off.
-
-        For more info about the labeling and coloring of the map, see the explore
-        method.
-
-        Args:
-            mask: the geometry to clip the data by.
-            column: The column to color the geometries by. Defaults to the column
-                that was specified last.
-            **kwargs: Keyword arguments to pass to geopandas.GeoDataFrame.explore, for
-                instance 'cmap' to change the colors, 'scheme' to change how the data
-                is grouped. This defaults to 'fisherjenks' for numeric data.
-
-        See also:
-            explore: same functionality, but shows the entire area of the geometries.
-            samplemap: same functionality, but shows only a random area of a given size.
-        """
-        if column:
-            self._column = column
-            self._update_column()
-            kwargs.pop("column", None)
-
-        gdfs: tuple[GeoDataFrame] = ()
-        for gdf in self._gdfs:
-            gdf = gdf.clip(mask)
-            collections = gdf.loc[gdf.geom_type == "GeometryCollection"]
-            if len(collections):
-                collections = collections.explode(index_parts=False)
-                gdf = pd.concat([gdf, collections], ignore_index=False)
-            gdfs = gdfs + (gdf,)
-        self._gdfs = gdfs
-        self._gdf = pd.concat(gdfs, ignore_index=True)
-        self._explore(**kwargs)
+            self._title_fontsize = size * 1.2
 
-    def _explore(self, **kwargs):
-        self.kwargs = self.kwargs | kwargs
-
-        if self._is_categorical:
-            self._create_categorical_map()
+        if "fontsize" in kwargs:
+            self._fontsize = kwargs["fontsize"]
+            self._fontsize_has_been_set = True
         else:
-            self._create_continous_map()
+            self._fontsize = size
 
-        if self.show_in_browser:
-            self.map.show_in_browser()
+        if "markersize" in kwargs:
+            self._markersize = kwargs["markersize"]
+            self._markersize_has_been_set = True
         else:
-            display(self.map)
+            self._markersize = size
 
-    def _split_categories(self):
-        new_gdfs, new_labels = [], []
-        for cat in self._unique_values:
-            gdf = self.gdf.loc[self.gdf[self.column] == cat]
-            new_gdfs.append(gdf)
-            new_labels.append(cat)
-        self._gdfs = new_gdfs
-        self._gdf = pd.concat(new_gdfs, ignore_index=True)
-        self.labels = new_labels
-
-    def _make_all_polygon(self):
-        """Buffer gdf if mixed geometry types
-
-        Because Folium does not handle GeometryCollection well
-        """
-
-        new_gdfs = []
-        for gdf in self.gdfs:
-            if get_geom_type(gdf) == "mixed":
-                gdf[gdf._geometry_column_name] = gdf.buffer(0.1)
-            new_gdfs.append(gdf)
-        self._gdfs = new_gdfs
-        self._gdf = pd.concat(new_gdfs, ignore_index=True)
-        self._nan_idx = self._gdf[self._column].isna()
-
-    def _update_column(self):
-        self._is_categorical = self._check_if_categorical()
-        self._fill_missings()
-        self._gdf = pd.concat(self._gdfs, ignore_index=True)
-
-    def _create_categorical_map(self):
-        self._get_categorical_colors()
-
-        self.map = self._explore_return(
-            self._gdf,
-            return_="empty_map",
-            max_zoom=self.max_zoom,
-            popup=self.popup,
-            **self.kwargs,
-        )
+    def _prepare_categorical_legend(self, categories_colors: dict, nan_label: str):
+        for attr in self.__dict__.keys():
+            if attr in self.kwargs:
+                self[attr] = self.kwargs.pop(attr)
+
+        # swap column values with label values if labels is dict
+        if self.labels and isinstance(self.labels, dict):
+            categories_colors = {
+                self.labels[cat]: color for cat, color in categories_colors.items()
+            }
+        # swap column values with label list and hope it's in the correct order
+        elif self.labels:
+            categories_colors = {
+                label: color
+                for label, color in zip(
+                    self.labels, categories_colors.values(), strict=True
+                )
+            }
 
-        for gdf, label in zip(self._gdfs, self.labels, strict=True):
-            if not len(gdf):
-                continue
-            f = folium.FeatureGroup(name=label)
-
-            gjs = self._explore_return(
-                gdf,
-                color=gdf["color"],
-                return_="geojson",
-                tooltip=self._tooltip_cols(gdf),
-                **{
-                    key: value
-                    for key, value in self.kwargs.items()
-                    if key not in ["title"]
-                },
+        self._patches, self._categories = [], []
+        for category, color in categories_colors.items():
+            if category == nan_label:
+                self._categories.append(nan_label)
+            else:
+                self._categories.append(category)
+            self._patches.append(
+                Line2D(
+                    [0],
+                    [0],
+                    linestyle="none",
+                    marker="o",
+                    alpha=self.kwargs.get("alpha", 1),
+                    markersize=self._markersize,
+                    markerfacecolor=color,
+                    markeredgewidth=0,
+                )
             )
-            f.add_child(gjs)
-            self.map.add_child(f)
-        _categorical_legend(
-            self.map,
-            self._column,
-            self._categories_colors_dict.keys(),
-            self._categories_colors_dict.values(),
-        )
-        folium.TileLayer("stamentoner").add_to(self.map)
-        folium.TileLayer("cartodbdark_matter").add_to(self.map)
-        self.map.add_child(folium.LayerControl())
-
-    def _create_continous_map(self):
-        self._prepare_continous_map()
-        if self.scheme:
-            classified = self._classify_from_bins(self._gdf, bins=self.bins)
-            classified_sequential = self._push_classification(classified)
-            n_colors = len(np.unique(classified_sequential)) - any(self._nan_idx)
-            unique_colors = self._get_continous_colors(n=n_colors)
-
-        self.map = self._explore_return(
-            self._gdf,
-            return_="empty_map",
-            max_zoom=self.max_zoom,
-            popup=self.popup,
+
+    def _actually_add_legend(self, ax):
+        legend = ax.legend(
+            self._patches,
+            self._categories,
+            fontsize=self._fontsize,
+            title=self.title,
+            title_fontsize=self._title_fontsize,
+            bbox_to_anchor=self._position + (self.width, self.height),
+            fancybox=False,
+            framealpha=self.framealpha,
+            edgecolor=self.edgecolor,
+            labelspacing=self.labelspacing,
             **self.kwargs,
         )
 
-        colorbar = bc.colormap.StepColormap(
-            unique_colors,
-            vmin=self._gdf[self._column].min(),
-            vmax=self._gdf[self._column].max(),
-            caption=self._column,
-            index=self.bins,
-            #  **colormap_kwds,
-        )
+        if self.title_color:
+            plt.setp(legend.get_title(), color=self.title_color)
 
-        for gdf, label in zip(self._gdfs, self.labels, strict=True):
-            if not len(gdf):
-                continue
-            f = folium.FeatureGroup(name=label)
-
-            classified = self._classify_from_bins(gdf, bins=self.bins)
-            colorarray = unique_colors[classified]
-
-            gjs = self._explore_return(
-                gdf,
-                tooltip=self._tooltip_cols(gdf),
-                color=colorarray,
-                return_="geojson",
-                **{key: value for key, value in self.kwargs.items() if key != "title"},
-            )
-            f.add_child(gjs)
-            self.map.add_child(f)
+        return ax
 
-        self.map.add_child(colorbar)
-        folium.TileLayer("stamentoner").add_to(self.map)
-        folium.TileLayer("cartodbdark_matter").add_to(self.map)
-        self.map.add_child(folium.LayerControl())
-
-    def _tooltip_cols(self, gdf: GeoDataFrame) -> list:
-        if "tooltip" in self.kwargs:
-            tooltip = self.kwargs.pop("tooltip")
-            return tooltip
-        return [col for col in gdf.columns if col not in COLS_TO_DROP]
-
-    def _explore_return(
-        self,
-        df,
-        return_: str,
-        column=None,
-        color=None,
-        attr=None,
-        tiles="OpenStreetMap",
-        tooltip=True,
-        popup=False,
-        highlight=True,
-        width="100%",
-        height="100%",
-        control_scale=True,
-        marker_type=None,
-        marker_kwds={},
-        style_kwds={},
-        highlight_kwds={},
-        tooltip_kwds={},
-        popup_kwds={},
-        map_kwds={},
-        **kwargs,
-    ):
-        """Contains the nessecary parts of the geopandas _explore function.
-
-        Also has a return_ parameter that controls what is returned. This should be
-        replaced by separate functions, and irrelevant parameters should be removed.
-        """
-        # xyservices is an optional dependency
-        try:
-            import xyzservices
+    def _get_best_legend_position(self, gdf, k: int):
+        minx, miny, maxx, maxy = gdf.total_bounds
+        diffx = maxx - minx
+        diffy = maxy - miny
 
-            has_xyzservices = True
-        except ImportError:
-            has_xyzservices = False
-
-        gdf = df.copy()
-
-        # convert LinearRing to LineString
-        rings_mask = df.geom_type == "LinearRing"
-        if rings_mask.any():
-            gdf.geometry[rings_mask] = gdf.geometry[rings_mask].apply(
-                lambda g: LineString(g)
-            )
+        points = points_in_bounds(gdf, 30)
+        gdf = gdf.loc[:, ~gdf.columns.str.contains("index|level_")]
+        joined = points.sjoin_nearest(gdf, distance_col="nearest")
 
-        if gdf.crs is None:
-            kwargs["crs"] = "Simple"
-            tiles = None
-        elif not gdf.crs.equals(4326):
-            gdf = gdf.to_crs(4326)
-
-        # create folium.Map object
-        # Get bounds to specify location and map extent
-        bounds = gdf.total_bounds
-        location = kwargs.pop("location", None)
-        if location is None:
-            x = mean([bounds[0], bounds[2]])
-            y = mean([bounds[1], bounds[3]])
-            location = (y, x)
-            if "zoom_start" in kwargs.keys():
-                fit = False
-            else:
-                fit = True
-        else:
-            fit = False
+        max_distance = max(joined.nearest)
 
-        # get a subset of kwargs to be passed to folium.Map
-        for i in _MAP_KWARGS:
-            if i in map_kwds:
-                raise ValueError(
-                    f"'{i}' cannot be specified in 'map_kwds'. "
-                    f"Use the '{i}={map_kwds[i]}' argument instead."
-                )
-        map_kwds = {
-            **map_kwds,
-            **{i: kwargs[i] for i in kwargs.keys() if i in _MAP_KWARGS},
-        }
-
-        if has_xyzservices:
-            # match provider name string to xyzservices.TileProvider
-            if isinstance(tiles, str):
-                try:
-                    tiles = xyzservices.providers.query_name(tiles)
-                except ValueError:
-                    pass
-
-            if isinstance(tiles, xyzservices.TileProvider):
-                attr = attr if attr else tiles.html_attribution
-                map_kwds["min_zoom"] = tiles.get("min_zoom", 0)
-                map_kwds["max_zoom"] = tiles.get("max_zoom", 30)
-                tiles = tiles.build_url(scale_factor="{r}")
-
-            m = folium.Map(
-                location=location,
-                control_scale=control_scale,
-                tiles=tiles,
-                attr=attr,
-                width=width,
-                height=height,
-                **map_kwds,
-            )
+        best_position = joined.loc[joined.nearest == max_distance].drop_duplicates(
+            "geometry"
+        )
 
-            # fit bounds to get a proper zoom level
-            if fit:
-                m.fit_bounds([[bounds[1], bounds[0]], [bounds[3], bounds[2]]])
-
-        for map_kwd in _MAP_KWARGS:
-            kwargs.pop(map_kwd, None)
-
-        # set default style
-        if "fillOpacity" not in style_kwds:
-            style_kwds["fillOpacity"] = 0.5
-        if "weight" not in style_kwds:
-            style_kwds["weight"] = 2
-        if "style_function" in style_kwds:
-            style_kwds_function = style_kwds["style_function"]
-            if not callable(style_kwds_function):
-                raise ValueError("'style_function' has to be a callable")
-            style_kwds.pop("style_function")
-        else:
+        bestx, besty = (
+            best_position.geometry.x.iloc[0],
+            best_position.geometry.y.iloc[0],
+        )
 
-            def _no_style(x):
-                return {}
+        bestx_01 = (bestx - minx) / (diffx)
+        besty_01 = (besty - miny) / (diffy)
 
-            style_kwds_function = _no_style
+        bestx_01 = 0.1 if bestx_01 < 0.5 else 0.90
+        besty_01 = 0.0375 * k if besty_01 < 0.5 else 1
 
-        gdf["__folium_color"] = color
+        return bestx_01, besty_01
 
-        stroke_color = style_kwds.pop("color", None)
-        if not stroke_color:
+    def __getitem__(self, item):
+        return getattr(self, item)
 
-            def _style_column(x):
-                base_style = {
-                    "fillColor": x["properties"]["__folium_color"],
-                    "color": x["properties"]["__folium_color"],
-                    **style_kwds,
-                }
-                return {
-                    **base_style,
-                    **style_kwds_function(x),
-                }
+    def __setitem__(self, key, value):
+        setattr(self, key, value)
 
-            style_function = _style_column
+    def get(self, key, default=None):
+        try:
+            return self[key]
+        except (KeyError, ValueError, IndexError, AttributeError):
+            return default
+
+    @property
+    def position(self):
+        return self._position
+
+    @position.setter
+    def position(self, new_value: bool):
+        self._position = new_value
+        self._position_has_been_set = True
+
+    @property
+    def title_fontsize(self):
+        return self._title_fontsize
+
+    @title_fontsize.setter
+    def title_fontsize(self, new_value: bool):
+        self._title_fontsize = new_value
+        self._title_fontsize_has_been_set = True
+
+    @property
+    def fontsize(self):
+        return self._fontsize
+
+    @fontsize.setter
+    def fontsize(self, new_value: bool):
+        self._fontsize = new_value
+        self._fontsize_has_been_set = True
+
+    @property
+    def markersize(self):
+        return self._markersize
+
+    @markersize.setter
+    def markersize(self, new_value: bool):
+        self._markersize = new_value
+        self._markersize_has_been_set = True
+
+
+class ContinousLegend(Legend):
+    """Holds the legend attributes specific to numeric columns.
+
+    The attributes consern the labeling of the groups in the legend.
+    Labels can be set manually with the 'labels' attribute, or the format
+    of the labels can be changed with the remaining attributes.
+
+    Attributes:
+        labels: To manually set labels. If set, all other labeling attributes are
+            ignored. Should be given as a list of strings with the same length as
+            the number of color groups.
+        pretty_labels: If False (default), the minimum and maximum values of each
+            color group will be used as legend labels. If True, the labels will end
+            with the maximum value, but start at 1 + the maximum value of the previous
+            group. The labels will be correct but inaccurate.
+        label_suffix: The text to put after each number in the legend labels.
+            Defaults to None.
+        label_sep: Text to put in between the two numbers in each color group in
+            the legend. Defaults to '-'.
+        rounding: Number of decimals in the labels. By default, the rounding
+            depends on the column's maximum value and standard deviation.
+            OBS: The bins will not be rounded, meaning the labels might be wrong
+            if not bins are set manually.
+        thousand_sep: Separator between each thousand for large numbers. Defaults to
+            None, meaning no separator.
+        decimal_mark: Text to use as decimal point. Defaults to None, meaning '.' (dot)
+            unless 'thousand_sep' is '.'. In this case, ',' (comma) will be used as
+            decimal mark.
+
+    Examples
+    --------
+    Create ten random points with a numeric column from 0 to 9.
+
+    >>> import sgis as sg
+    >>> points = sg.random_points(10)
+    >>> points["number"] = range(10)
+    >>> points
+                    geometry  number
+    0  POINT (0.59780 0.50425)       0
+    1  POINT (0.07019 0.26167)       1
+    2  POINT (0.56475 0.15422)       2
+    3  POINT (0.87293 0.60316)       3
+    4  POINT (0.47373 0.20040)       4
+    5  POINT (0.98661 0.15614)       5
+    6  POINT (0.30951 0.77057)       6
+    7  POINT (0.47802 0.52824)       7
+    8  POINT (0.12215 0.96588)       8
+    9  POINT (0.02938 0.93467)       9
+
+    Creating the ThematicMap instance with a numeric column.
+
+    >>> m = sg.ThematicMap(points, column="number")
+
+    Changing the attributes that apply to both numeric and categorical columns.
+
+    >>> m.legend.title = "Meters"
+    >>> m.legend.position = (0.35, 0.28)
+
+    Change the attributes that only apply to numeric columns.
+
+    >>> m.label_sep = "to"
+    >>> m.label_suffix = "num"
+    >>> m.rounding = 2
+    >>> m.plot()
+
+    Setting labels manually. For better control, it might be wise to also set the bins
+    manually. The following bins will create a plot with the color groups
+    0-2, 3-5, 6-7 and 8-9. The legend labels can then be set accordingly.
+
+    >>> m = sg.ThematicMap(points, column="number")
+    >>> m.bins = [0, 2, 5, 7, 9]
+    >>> m.legend.labels = ["0 to 2 num", "3 to 5 num", "6 to 7 num", "8 to 9 num"]
+    >>> m.plot()
+
+    We will get the same groups if we exclude the first and last bin values. The
+    minimum and maximum values will be filled anyway.
+
+    >>> m = sg.ThematicMap(points, column="number")
+    >>> m.bins = [2, 5, 7]
+    >>> m.legend.labels = ["0 to 2 num", "3 to 5 num", "6 to 7 num", "8 to 9 num"]
+    >>> m.plot()
 
-        if highlight:
-            if "fillOpacity" not in highlight_kwds:
-                highlight_kwds["fillOpacity"] = 0.75
+    """
 
-            def _style_highlight(x):
-                return {**highlight_kwds}
+    def __init__(
+        self,
+        labels: list[str] | None = None,
+        pretty_labels: bool = False,
+        label_suffix: str | None = None,
+        label_sep: str = "-",
+        rounding: int | None = None,
+        thousand_sep: str | None = None,
+        decimal_mark: str | None = None,
+        **kwargs,
+    ):
+        super().__init__(**kwargs)
 
-            highlight_function = _style_highlight
+        self.pretty_labels = pretty_labels
+        self.thousand_sep = thousand_sep
+        self.decimal_mark = decimal_mark
+
+        self.label_sep = label_sep
+        self.label_suffix = "" if not label_suffix else label_suffix
+        self._rounding = rounding
+        self._rounding_has_been_set = True if rounding else False
+
+    def _get_rounding(self, array: Series | np.ndarray) -> int:
+        def isinteger(x):
+            return np.equal(np.mod(x, 1), 0)
+
+        if np.all(isinteger(array)):
+            return 0
+
+        closest_to_zero_idx = np.argmin(np.abs(array))
+        closest_to_zero = np.abs(array[closest_to_zero_idx])
+
+        between_1_and_0 = 1 > closest_to_zero > 0
+        if between_1_and_0:
+            return int(abs(np.log10(abs(closest_to_zero)))) + 1
+
+        std_ = np.std(array)
+        max_ = np.max(array)
+        if max_ > 30 and std_ > 5:
+            return 0
+        if max_ > 5 and std_ > 1:
+            return 1
+        if max_ > 1 and std_ > 0.1:
+            return 2
+        return int(abs(np.log10(std_))) + 1
+
+    @staticmethod
+    def _set_rounding(bins, rounding: int | float):
+        if rounding == 0:
+            return [int(round(bin, 0)) for bin in bins]
         else:
-            highlight_function = None
-
-        # define default for points
-        if marker_type is None:
-            marker_type = "circle_marker"
-
-        marker = marker_type
-        if isinstance(marker_type, str):
-            if marker_type == "marker":
-                marker = folium.Marker(**marker_kwds)
-            elif marker_type == "circle":
-                marker = folium.Circle(**marker_kwds)
-            elif marker_type == "circle_marker":
-                marker_kwds["radius"] = marker_kwds.get("radius", 2)
-                marker_kwds["fill"] = marker_kwds.get("fill", True)
-                marker = folium.CircleMarker(**marker_kwds)
-            else:
-                raise ValueError(
-                    "Only 'marker', 'circle', and 'circle_marker' are "
-                    "supported as marker values"
-                )
+            return [round(bin, rounding) for bin in bins]
 
-        gdf = clean_geoms(gdf)
+    def _remove_max_legend_value(self):
+        if not self._legend:
+            raise ValueError("Cannot modify legend before it is created.")
 
-        # prepare tooltip and popup
-        if isinstance(gdf, GeoDataFrame):
-            # add named index to the tooltip
-            if gdf.index.name is not None:
-                gdf = gdf.reset_index()
-            # specify fields to show in the tooltip
-            tooltip = _tooltip_popup("tooltip", tooltip, gdf, **tooltip_kwds)
-            popup = _tooltip_popup("popup", popup, gdf, **popup_kwds)
-        else:
-            tooltip = None
-            popup = None
+    def _prepare_continous_legend(
+        self,
+        bins: list[float],
+        colors: list[str],
+        nan_label: str,
+        bin_values: dict,
+    ):
+        # TODO: clean up this messy method
 
-        if "geojson" in return_:
-            # add dataframe to map
-            gjs = folium.GeoJson(
-                gdf.__geo_interface__,
-                tooltip=tooltip,
-                popup=popup,
-                marker=marker,
-                style_function=style_function,
-                highlight_function=highlight_function,
-                **kwargs,
+        for attr in self.__dict__.keys():
+            if attr in self.kwargs:
+                self[attr] = self.kwargs.pop(attr)
+
+        self._patches, self._categories = [], []
+
+        for color in colors:
+            self._patches.append(
+                Line2D(
+                    [0],
+                    [0],
+                    linestyle="none",
+                    marker="o",
+                    alpha=self.kwargs.get("alpha", 1),
+                    markersize=self._markersize,
+                    markerfacecolor=color,
+                    markeredgewidth=0,
+                )
             )
-            return gjs
 
-        return m
+        if self.labels:
+            if len(self.labels) != len(colors):
+                raise ValueError(
+                    "Label list must be same length as the number of groups. "
+                    f"Got k={len(colors)} and labels={len(colors)}."
+                    f"labels: {', '.join(self.labels)}"
+                    f"colors: {', '.join(colors)}"
+                )
+            self._categories = self.labels
 
+        elif len(bins) == len(colors):
+            for i, _ in enumerate(bins):
+                min_ = np.min(bin_values[i])
+                max_ = np.max(bin_values[i])
+                min_rounded = self._set_rounding([min_], self._rounding)[0]
+                max_rounded = self._set_rounding([max_], self._rounding)[0]
+                if min_ == max_:
+                    self._categories.append(f"{min_rounded} {self.label_suffix}")
+                else:
+                    self._categories.append(
+                        f"{min_rounded} {self.label_suffix} {self.label_sep} "
+                        f"{max_rounded} {self.label_suffix}"
+                    )
 
-def _tooltip_popup(type, fields, gdf, **kwds):
-    """get tooltip or popup"""
-    import folium
-
-    # specify fields to show in the tooltip
-    if fields is False or fields is None or fields == 0:
-        return None
-    else:
-        if fields is True:
-            fields = gdf.columns.drop(gdf.geometry.name).to_list()
-        elif isinstance(fields, int):
-            fields = gdf.columns.drop(gdf.geometry.name).to_list()[:fields]
-        elif isinstance(fields, str):
-            fields = [fields]
-
-    for field in ["__plottable_column", "__folium_color"]:
-        if field in fields:
-            fields.remove(field)
-
-    # Cast fields to str
-    fields = list(map(str, fields))
-    if type == "tooltip":
-        return folium.GeoJsonTooltip(fields, **kwds)
-    elif type == "popup":
-        return folium.GeoJsonPopup(fields, **kwds)
+        else:
+            for i, (cat1, cat2) in enumerate(zip(bins[:-1], bins[1:], strict=True)):
+                if nan_label in str(cat1) or nan_label in str(cat2):
+                    self._categories.append(nan_label)
+                    continue
+
+                min_ = np.min(bin_values[i])
+                max_ = np.max(bin_values[i])
+                min_rounded = self._set_rounding([min_], self._rounding)[0]
+                max_rounded = self._set_rounding([max_], self._rounding)[0]
+                if self.pretty_labels:
+                    if i != 0 and self._rounding == 0:
+                        cat1 = int(cat1 + 1)
+                    elif i != 0:
+                        cat1 = cat1 + float(f"1e-{self._rounding}")
+
+                    cat1 = self._format_number(cat1)
+                    cat2 = self._format_number(cat2)
+
+                    if min_ == max_:
+                        label = self._two_value_label(cat1, cat2)
+                        self._categories.append(label)
+                        continue
+
+                    label = self._two_value_label(cat1, cat2)
+                    self._categories.append(label)
+
+                elif min_ == max_:
+                    min_rounded = self._format_number(min_rounded)
+                    label = self._one_value_label(min_rounded)
+                    self._categories.append(label)
+                else:
+                    min_rounded = self._format_number(min_rounded)
+                    max_rounded = self._format_number(max_rounded)
+                    label = self._two_value_label(min_rounded, max_rounded)
+                    self._categories.append(label)
+
+    def _actually_add_legend(self, ax):
+        legend = ax.legend(
+            self._patches,
+            self._categories,
+            fontsize=self._fontsize,
+            title=self.title,
+            title_fontsize=self._title_fontsize,
+            bbox_to_anchor=self._position + (self.width, self.height),
+            fancybox=False,
+            framealpha=self.framealpha,
+            edgecolor=self.edgecolor,
+            labelspacing=self.labelspacing,
+            **self.kwargs,
+        )
 
+        if self.title_color:
+            plt.setp(legend.get_title(), color=self.title_color)
 
-def _categorical_legend(m, title, categories, colors):
-    """
-    Add categorical legend to a map
+        return ax
 
-    The implementation is using the code originally written by Michel Metran
-    (@michelmetran) and released on GitHub
-    (https://github.com/michelmetran/package_folium) under MIT license.
-
-    Copyright (c) 2020 Michel Metran
-
-    Parameters
-    ----------
-    m : folium.Map
-        Existing map instance on which to draw the plot
-    title : str
-        title of the legend (e.g. column name)
-    categories : list-like
-        list of categories
-    colors : list-like
-        list of colors (in the same order as categories)
-    """
+    def _two_value_label(self, value1, value2):
+        return (
+            f"{value1} {self.label_suffix} {self.label_sep} "
+            f"{value2} {self.label_suffix}"
+        )
 
-    # Header to Add
-    head = """
-    {% macro header(this, kwargs) %}
-    <script src="https://code.jquery.com/ui/1.12.1/jquery-ui.js"></script>
-    <script>$( function() {
-        $( ".maplegend" ).draggable({
-            start: function (event, ui) {
-                $(this).css({
-                    right: "auto",
-                    top: "auto",
-                    bottom: "auto"
-                });
-            }
-        });
-    });
-    </script>
-    <style type='text/css'>
-      .maplegend {
-        position: absolute;
-        z-index:9999;
-        background-color: rgba(255, 255, 255, .8);
-        border-radius: 5px;
-        box-shadow: 0 0 15px rgba(0,0,0,0.2);
-        padding: 10px;
-        font: 12px/14px Arial, Helvetica, sans-serif;
-        right: 10px;
-        bottom: 20px;
-      }
-      .maplegend .legend-title {
-        text-align: left;
-        margin-bottom: 5px;
-        font-weight: bold;
-        }
-      .maplegend .legend-scale ul {
-        margin: 0;
-        margin-bottom: 0px;
-        padding: 0;
-        float: left;
-        list-style: none;
-        }
-      .maplegend .legend-scale ul li {
-        list-style: none;
-        margin-left: 0;
-        line-height: 16px;
-        margin-bottom: 2px;
-        }
-      .maplegend ul.legend-labels li span {
-        display: block;
-        float: left;
-        height: 14px;
-        width: 14px;
-        margin-right: 5px;
-        margin-left: 0;
-        border: 0px solid #ccc;
-        }
-      .maplegend .legend-source {
-        color: #777;
-        clear: both;
-        }
-      .maplegend a {
-        color: #777;
-        }
-    </style>
-    {% endmacro %}
-    """
-    import branca as bc
+    def _one_value_label(self, value1):
+        return f"{value1} {self.label_suffix}"
 
-    # Add CSS (on Header)
-    macro = bc.element.MacroElement()
-    macro._template = bc.element.Template(head)
-    m.get_root().add_child(macro)
-
-    body = f"""
-    <div id='maplegend {title}' class='maplegend'>
-        <div class='legend-title'>{title}</div>
-        <div class='legend-scale'>
-            <ul class='legend-labels'>"""
-
-    # Loop Categories
-    for label, color in zip(categories, colors, strict=True):
-        body += f"""
-                <li><span style='background:{color}'></span>{label}</li>"""
-
-    body += """
-            </ul>
-        </div>
-    </div>
-    """
+    def _format_number(self, number):
+        if not self.thousand_sep and not self.decimal_mark:
+            return number
+
+        if self.thousand_sep:
+            number = f"{number:,}".replace(",", "*temp_thousand*")
+
+        if self.decimal_mark:
+            number = str(number).replace(".", "*temp_decimal*")
+
+        if self.thousand_sep == "." and not self.decimal_mark:
+            number = number.replace(".", ",").replace(
+                "*temp_thousand*", self.thousand_sep
+            )
+        elif not self.thousand_sep:
+            number = number.replace("*temp_decimal*", self.decimal_mark)
+        elif not self.decimal_mark:
+            number = number.replace("*temp_thousand*", self.thousand_sep)
+        else:
+            number = number.replace("*temp_thousand*", self.thousand_sep).replace(
+                "*temp_decimal*", self.decimal_mark
+            )
+        return number
 
-    # Add Body
-    body = bc.element.Element(body, "legend")
-    m.get_root().html.add_child(body)
+    @property
+    def rounding(self):
+        return self._rounding
+
+    @rounding.setter
+    def rounding(self, new_value: bool):
+        self._rounding = new_value
+        self._rounding_has_been_set = True
```

### Comparing `ssb_sgis-0.1.5/src/sgis/maps/map.py` & `ssb_sgis-0.1.6/src/sgis/maps/map.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.5/src/sgis/maps/maps.py` & `ssb_sgis-0.1.6/src/sgis/maps/maps.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,20 +33,24 @@
     *gdfs: GeoDataFrame,
     column: str | None = None,
     labels: tuple[str] | None = None,
     max_zoom: int = 30,
     show_in_browser: bool = False,
     **kwargs,
 ) -> None:
-    """Interactive map of GeoDataFrames with layers that can be toggles on/off.
+    """Interactive map of GeoDataFrames with layers that can be toggled on/off.
 
     It takes all the given GeoDataFrames and displays them together in an
     interactive map with a common legend. If 'column' is not specified, each
     GeoDataFrame is given a unique color.
 
+    If the column is of type string and only one GeoDataFrame is given, the unique
+    values will be split into separate GeoDataFrames so that each value can be toggled
+    on/off.
+
     The coloring can be changed with the 'cmap' parameter. The default colormap is a
     custom, strongly colored palette. If a numerical colum is given, the 'viridis'
     palette is used.
 
     Note:
         The maximum zoom level only works on the OpenStreetMap background map.
```

### Comparing `ssb_sgis-0.1.5/src/sgis/maps/thematicmap.py` & `ssb_sgis-0.1.6/src/sgis/maps/thematicmap.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,34 +142,64 @@
 
     def plot(self, **kwargs) -> None:
         """Creates the final plot.
 
         This method should be run after customising the map, but before saving.
         """
 
+        __test = kwargs.pop("__test", False)
         include_legend = bool(kwargs.pop("legend", self.legend))
 
-        self._prepare_plot(**kwargs)
-
         if "color" in kwargs:
-            kwargs["column"] = self.column
+            kwargs.pop("column", None)
             self.legend = None
             include_legend = False
         elif hasattr(self, "color"):
-            kwargs["column"] = self.column
+            kwargs.pop("column", None)
             kwargs["color"] = self.color
             self.legend = None
             include_legend = False
+
         elif self._is_categorical:
             kwargs = self._prepare_categorical_plot(kwargs)
+            self.legend._prepare_categorical_legend(
+                categories_colors=self._categories_colors_dict,
+                nan_label=self.nan_label,
+            )
+
         else:
             kwargs = self._prepare_continous_plot(kwargs)
+            if self.legend:
+                if not self.legend._rounding_has_been_set:
+                    self.legend._rounding = self.legend._get_rounding(
+                        array=self._gdf.loc[~self._nan_idx, self._column]
+                    )
+
+                self.legend._prepare_continous_legend(
+                    bins=self.bins,
+                    colors=self._unique_colors,
+                    nan_label=self.nan_label,
+                    bin_values=self._bins_unique_values,
+                )
+
+        if self.legend and not self.legend._position_has_been_set:
+            self.legend._position = self.legend._get_best_legend_position(
+                self._gdf, k=self._k + bool(len(self._nan_idx))
+            )
+
+        if __test:
+            return
+
+        self._prepare_plot(**kwargs)
 
         if self.legend:
-            self._actually_add_legend()
+            self.ax = self.legend._actually_add_legend(ax=self.ax)
+
+        #        if self.legend:
+        #           self._actually_add_legend()
 
         self._gdf.plot(legend=include_legend, ax=self.ax, **kwargs)
 
     def save(self, path: str) -> None:
         """Save figure as image file.
 
         To be run after the plot method.
@@ -253,19 +283,14 @@
     def _actually_add_legend(self) -> None:
         """Add legend to the axis and fill it with colors and labels."""
         if not self.legend._position_has_been_set:
             self.legend._position = self.legend._get_best_legend_position(
                 self._gdf, k=self._k + bool(len(self._nan_idx))
             )
 
-        if not self._is_categorical and not self.legend._rounding_has_been_set:
-            self.legend._rounding = self.legend._get_rounding(
-                array=self._gdf.loc[~self._nan_idx, self._column]
-            )
-
         if self._is_categorical:
             self.ax = self.legend._actually_add_categorical_legend(
                 ax=self.ax,
                 categories_colors=self._categories_colors_dict,
                 nan_label=self.nan_label,
             )
         else:
```

### Comparing `ssb_sgis-0.1.5/src/sgis/networkanalysis/_od_cost_matrix.py` & `ssb_sgis-0.1.6/src/sgis/networkanalysis/_od_cost_matrix.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,43 +12,41 @@
     origins: GeoDataFrame,
     destinations: GeoDataFrame,
     weight: str,
     *,
     lines: bool = False,
     rowwise: bool = False,
 ) -> DataFrame | GeoDataFrame:
-    if rowwise and len(origins) != len(destinations):
-        raise ValueError(
-            "'origins' and 'destinations' must have the same length when rowwise=True"
-        )
-
-    results = graph.distances(
+    distances: list[list[str]] = graph.distances(
         weights="weight",
         source=origins["temp_idx"],
         target=destinations["temp_idx"],
     )
 
     ori_idx, des_idx, costs = [], [], []
     for i, f_idx in enumerate(origins["temp_idx"]):
-        for ii, t_idx in enumerate(destinations["temp_idx"]):
+        for j, t_idx in enumerate(destinations["temp_idx"]):
             ori_idx.append(f_idx)
             des_idx.append(t_idx)
-            costs.append(results[i][ii])
+            costs.append(distances[i][j])
 
     results = (
         pd.DataFrame(data={"origin": ori_idx, "destination": des_idx, weight: costs})
         .replace([np.inf, -np.inf], np.nan)
         .reset_index(drop=True)
     )
 
     # calculating all-to-all distances is much faster than looping rowwise,
     # so filtering to rowwise afterwards instead
     if rowwise:
         rowwise_df = DataFrame(
-            {"origin": origins["temp_idx"], "destination": destinations["temp_idx"]}
+            {
+                "origin": origins["temp_idx"].reset_index(drop=True),
+                "destination": destinations["temp_idx"].reset_index(drop=True),
+            }
         )
         results = rowwise_df.merge(results, on=["origin", "destination"], how="left")
 
     wkt_dict_origin = {
         idx: geom.wkt
         for idx, geom in zip(origins["temp_idx"], origins.geometry, strict=True)
     }
```

### Comparing `ssb_sgis-0.1.5/src/sgis/networkanalysis/_points.py` & `ssb_sgis-0.1.6/src/sgis/networkanalysis/_points.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,32 +32,14 @@
         self.gdf["temp_idx"] = self.gdf["temp_idx"].astype(str)
 
         self.idx_dict = {
             temp_idx: idx
             for temp_idx, idx in zip(self.gdf.temp_idx, self.gdf.index, strict=True)
         }
 
-    def _get_n_missing(
-        self,
-        results: GeoDataFrame | DataFrame,
-        col: str,
-    ) -> None:
-        """
-        Get number of missing values for each point after a network analysis.
-
-        Args:
-            results: (Geo)DataFrame resulting from od_cost_matrix, get_route,
-                get_k_routes, get_route_frequencies or service_area.
-            col: id column of the results. Either 'origin' or 'destination'.
-        """
-        self.gdf["missing"] = self.gdf["temp_idx"].map(
-            results.groupby(col).count().iloc[:, 0]
-            - results.dropna().groupby(col).count().iloc[:, 0]
-        )
-
     @staticmethod
     def _convert_distance_to_weight(distances, rules):
         """Meters to minutes based on 'weight_to_nodes_' attribute of the rules."""
         if not rules.nodedist_multiplier and not rules.nodedist_kmh:
             return [0 for _ in distances]
 
         if rules.nodedist_multiplier and rules.nodedist_kmh:
```

### Comparing `ssb_sgis-0.1.5/src/sgis/networkanalysis/_service_area.py` & `ssb_sgis-0.1.6/src/sgis/networkanalysis/_service_area.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.5/src/sgis/networkanalysis/directednetwork.py` & `ssb_sgis-0.1.6/src/sgis/networkanalysis/directednetwork.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 from shapely.constructive import reverse
 
 from ..helpers import return_two_vals, unit_is_meters
 from .network import Network
 
 
 class DirectedNetwork(Network):
-    """Subclass of Network with methods for making the network directed.
+    """Class for preparing line data for directed network analysis.
 
     Can be used as the 'network' parameter in the NetworkAnalysis class for directed
     network analysis.
 
     The DirectedNetwork class differs from the Network base class in two ways:
     1) using a DirectedNetwork in the NetworkAnalysis class means the network graph
     will be directed, meaning you can only travel in one direction on each line.
-    2) the class offers methods for making the network directed, mainly the
+    2) the class holds methods for making the network directed, mainly the
     'make_directed_network' method, which reverses lines going the wrong direction
     and duplicates and flips lines going both directions. It also creates a 'minute'
     column.
 
     Args:
         gdf: a GeoDataFrame of line geometries.
         **kwargs: keyword arguments taken by the base class Network.
```

### Comparing `ssb_sgis-0.1.5/src/sgis/networkanalysis/network.py` & `ssb_sgis-0.1.6/src/sgis/networkanalysis/network.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     1.0    85638
     Name: connected, dtype: int64
 
     Filling small gaps/holes in the network.
 
     >>> len(nw.gdf)
     85638
-    >>> nw = nw.close_network_holes(max_distance=1.5, fillna=0)
+    >>> nw = nw.close_network_holes(max_distance=1.5, max_angle=90, fillna=0)
     >>> len(nw.gdf)
     86929
 
     Cutting long lines into pieces. This is only relevant for service area analysis and
     similar analyses.
 
     >>> nw.gdf.length.max()
@@ -608,14 +608,29 @@
         )
 
         if any(removed):
             return False
 
         return True
 
+    def get_edges(self) -> list[tuple[str, str]]:
+        return [
+            (str(source), str(target))
+            for source, target in zip(
+                self.gdf["source"], self.gdf["target"], strict=True
+            )
+        ]
+
+    @staticmethod
+    def _create_edge_ids(
+        edges: list[tuple[str, str]], weights: list[float]
+    ) -> list[str]:
+        """Edge identifiers represented with source and target ids and the weight."""
+        return [f"{s}_{t}_{w}" for (s, t), w in zip(edges, weights, strict=True)]
+
     def _update_nodes_if(self):
         if not self._nodes_are_up_to_date():
             self._make_node_ids()
 
     @property
     def nodes(self):
         """GeoDataFrame with the network nodes (line endpoints).
@@ -649,31 +664,7 @@
 
     def __iter__(self):
         """So the attributes can be iterated through."""
         return iter(self.__dict__.items())
 
     def __len__(self):
         return len(self.gdf)
-
-
-# TODO: put these a better place:
-
-
-def _edge_ids(
-    gdf: GeoDataFrame | list[tuple[int, int]], weight: str | list[float]
-) -> list[str]:
-    """Quite messy way to deal with different input types."""
-    if isinstance(gdf, GeoDataFrame):
-        return _edge_id_template(
-            zip(gdf["source"], gdf["target"], strict=True),
-            weight_arr=gdf[weight],
-        )
-    if isinstance(gdf, list):
-        return _edge_id_template(gdf, weight_arr=weight)
-
-
-def _edge_id_template(*source_target_arrs, weight_arr):
-    """Edge identifiers represented with source and target ids and the weight."""
-    return [
-        f"{s}_{t}_{w}"
-        for (s, t), w in zip(*source_target_arrs, weight_arr, strict=True)
-    ]
```

### Comparing `ssb_sgis-0.1.5/src/sgis/networkanalysis/network_norway.py` & `ssb_sgis-0.1.6/src/sgis/networkanalysis/network_norway.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.5/src/sgis/networkanalysis/networkanalysis.py` & `ssb_sgis-0.1.6/src/sgis/networkanalysis/networkanalysis.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 import pandas as pd
 from geopandas import GeoDataFrame
 from igraph import Graph
 from pandas import DataFrame
 
 from ..geopandas_tools.general import _push_geom_col
 from ..geopandas_tools.line_operations import split_lines_by_nearest_point
-from ._get_route import _get_route
+from ._get_route import _get_k_routes, _get_route, _get_route_frequencies
 from ._od_cost_matrix import _od_cost_matrix
 from ._points import Destinations, Origins
 from ._service_area import _service_area
 from .directednetwork import DirectedNetwork
-from .network import Network, _edge_ids
+from .network import Network
 from .networkanalysisrules import NetworkAnalysisRules
 
 
 class NetworkAnalysis:
     """Class for doing network analysis.
 
     The class takes a (Directed)Network and rules for the analyses
@@ -67,45 +67,46 @@
     Attributes:
         network: The Network instance.
         rules: The NetworkAnalysisRules instance.
         log: A DataFrame with information about each analysis run.
 
     See also
     --------
-    DirectedNetwork : for customising and optimising line data before directed network
+    DirectedNetwork : For customising and optimising line data before directed network
         analysis.
-    Network : for customising and optimising line data before undirected network
+
+    Network : For customising and optimising line data before undirected network
         analysis.
 
     Examples
     --------
     Read example data.
 
-    >>> from sgis import read_parquet_url
-    >>> roads = read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_eidskog_2022.parquet")
-    >>> points = read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_eidskog.parquet")
+    >>> import sgis as sg
+    >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_eidskog_2022.parquet")
+    >>> points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_eidskog.parquet")
 
     Creating a NetworkAnalysis class instance.
 
-    >>> from sgis import DirectedNetwork, NetworkAnalysisRules, NetworkAnalysis
     >>> nw = (
-    ...     DirectedNetwork(roads)
+    ...     sg.DirectedNetwork(roads)
     ...     .remove_isolated()
     ...     .make_directed_network(
     ...         direction_col="oneway",
     ...         direction_vals_bft=("B", "FT", "TF"),
     ...         minute_cols=("drivetime_fw", "drivetime_bw"),
     ...     )
     ... )
-    >>> rules = NetworkAnalysisRules(weight="minutes")
-    >>> nwa = NetworkAnalysis(network=nw, rules=rules, detailed_log=False)
+    >>> rules = sg.NetworkAnalysisRules(weight="minutes")
+    >>> nwa = sg.NetworkAnalysis(network=nw, rules=rules, detailed_log=False)
     >>> nwa
     NetworkAnalysis(
         network=DirectedNetwork(6364 km, percent_bidirectional=87),
-        rules=NetworkAnalysisRules(weight='minutes', search_tolerance=250, search_factor=10, split_lines=False, ...)
+        rules=NetworkAnalysisRules(weight='minutes', search_tolerance=250, search_factor=10, split_lines=False, ...),
+        log=True, detailed_log=True,
     )
 
     od_cost_matrix: fast many-to-many travel time/distance calculation.
 
     >>> od = nwa.od_cost_matrix(points, points)
     >>> od
             origin  destination    minutes
@@ -116,15 +117,14 @@
     4            0            4  14.742294
     ...        ...          ...        ...
     999995     999          995  11.038673
     999996     999          996  17.820664
     999997     999          997  10.288465
     999998     999          998  14.798257
     999999     999          999   0.000000
-
     [1000000 rows x 3 columns]
 
     get_route: get the geometry of the routes.
 
     >>> routes = nwa.get_route(points.sample(10), points.sample(10))
     >>> routes
         origin  destination    minutes                                           geometry
@@ -135,35 +135,34 @@
     4      112          939  10.308372  MULTILINESTRING Z ((264112.512 6640728.679 79....
     ..     ...          ...        ...                                                ...
     95     606            2  11.325834  MULTILINESTRING Z ((270054.367 6653367.774 144...
     96     606          511  15.045134  MULTILINESTRING Z ((258569.800 6652168.600 57....
     97     606          901  16.998595  MULTILINESTRING Z ((265040.505 6641218.021 100...
     98     606          766  10.094371  MULTILINESTRING Z ((265639.400 6649020.000 85....
     99     606          320   7.317098  MULTILINESTRING Z ((262711.480 6648807.500 3.8...
-
     [100 rows x 4 columns]
 
     get_route_frequencies: get the number of times each line segment was used.
 
     >>> frequencies = nwa.get_route_frequencies(points.sample(25), points.sample(25))
     >>> frequencies[[["source", "target", "frequency", "geometry"]]
            source target  frequency                                           geometry
-    116897  28500  13496        1.0  LINESTRING Z (256638.500 6653339.300 153.857, ...
-    155781  23913  23908        1.0  LINESTRING Z (256843.774 6653563.678 143.702, ...
-    155780  76957  23913        1.0  LINESTRING Z (256866.300 6653559.400 142.457, ...
-    155779  76956  76957        1.0  LINESTRING Z (256875.300 6653557.100 142.157, ...
-    155778  74816  76956        1.0  LINESTRING Z (256882.738 6653554.580 141.657, ...
+    160188  77264  79112        1.0  LINESTRING Z (268641.225 6651871.624 111.355, ...
+    138956  30221  45403        1.0  LINESTRING Z (273091.100 6652396.000 170.471, ...
+    138958  30224  30221        1.0  LINESTRING Z (273117.500 6652391.500 169.771, ...
+    138960  16513  30224        1.0  LINESTRING Z (273176.813 6652379.896 169.414, ...
+    138962  40610  16513        1.0  LINESTRING Z (273207.300 6652372.100 168.871, ...
     ...       ...    ...        ...                                                ...
-    156631  77375  77374       90.0  LINESTRING Z (265454.387 6651000.044 88.806, 2...
-    149793  72649  77375       90.0  LINESTRING Z (265455.009 6651007.750 88.612, 2...
-    158249  78124  78123       95.0  LINESTRING Z (265563.150 6650547.620 89.382, 2...
-    158248  78123  72820       95.0  LINESTRING Z (265567.158 6650542.836 89.522, 2...
-    156601  77353  78124       95.0  LINESTRING Z (265530.470 6650587.640 88.527, 2...
+    151464  73800  73801      108.0  LINESTRING Z (265362.800 6647137.100 131.660, ...
+    151465  73801  73802      108.0  LINESTRING Z (265368.600 6647142.900 131.660, ...
+    151466  73802  73632      108.0  LINESTRING Z (265371.400 6647147.900 131.660, ...
+    151463  73799  73800      129.0  LINESTRING Z (265359.600 6647135.400 131.660, ...
+    152170  74418  74246      135.0  LINESTRING Z (264579.835 6651954.573 113.209, ...
 
-    [9268 rows x 4 columns]
+    [8915 rows x 4 columns]
 
     service_area: get the area that can be reached within one or more breaks.
 
     >>> service_areas = nwa.service_area(
     ...         points.iloc[:3],
     ...         breaks=[5, 10, 15],
     ...     )
@@ -183,16 +182,16 @@
 
     >>> nwa.log
                   endtime  minutes_elapsed                 method  origins_count  destinations_count  percent_missing  cost_mean  isolated_removed  ...   cost_p25 cost_median   cost_p75  cost_std  lines rowwise     breaks  dissolve
     0 2023-03-29 15:19:51              0.5         od_cost_matrix           1000              1000.0           0.9966  15.270462              True  ...  10.565738   14.772737  19.337235  6.654981  False   False        NaN       NaN
     1 2023-03-29 15:20:21              0.5              get_route             10                10.0           0.0000  15.001443              True  ...  10.093613   14.641413  19.725085  6.869095    NaN   False        NaN       NaN
     2 2023-03-29 15:20:40              0.3  get_route_frequencies             25                25.0           0.0000   0.067199              True  ...   0.013309    0.038496   0.085692  0.087247    NaN     NaN        NaN       NaN
     3 2023-03-29 15:20:50              0.2           service_area              3                 NaN           0.0000  10.000000              True  ...   5.000000   10.000000  15.000000  4.330127    NaN     NaN  5, 10, 15      True
-
     [4 rows x 23 columns]
+
     """
 
     def __init__(
         self,
         network: Network | DirectedNetwork,
         rules: NetworkAnalysisRules,
         log: bool = True,
@@ -270,54 +269,56 @@
             A DataFrame with the weight column and the columns 'origin' and
             'destination', containing the indices of the origins and destinations
             GeoDataFrames. If lines is True, also returns a geometry column with
             straight lines between origin and destination.
 
         Examples
         --------
+        Create the NetworkAnalysis instance.
+
+        >>> import sgis as sg
+        >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_eidskog_2022.parquet")
+        >>> nw = sg.DirectedNetwork(roads).remove_isolated().make_directed_network_norway()
+        >>> rules = sg.NetworkAnalysisRules(weight="minutes")
+        >>> nwa = sg.NetworkAnalysis(network=nw, rules=rules, detailed_log=False)
+
         Create some origin and destination points.
-        See the class examples for how to prepare the network.
 
-        import sgis as sg
-        >>> points = sg.read_parquet_url(
-        ...     "https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet"
-        ... )
+        >>> points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
 
-        >>> origins = points.loc[:99]
+        >>> origins = points.loc[:99, ["geometry"]]
         >>> origins
                                   geometry
         0   POINT (263122.700 6651184.900)
         1   POINT (272456.100 6653369.500)
         2   POINT (270082.300 6653032.700)
         3   POINT (259804.800 6650339.700)
         4   POINT (272876.200 6652889.100)
         ..                             ...
         95  POINT (270348.000 6651899.400)
         96  POINT (264845.600 6649005.800)
         97  POINT (263162.000 6650732.200)
         98  POINT (272322.700 6653729.100)
         99  POINT (265622.800 6644644.200)
-
         [100 rows x 1 columns]
 
-        >>> destinations = points.loc[100:199]
+        >>> destinations = points.loc[100:199, ["geometry"]]
         >>> destinations
                                    geometry
         100  POINT (265997.900 6647899.400)
         101  POINT (263835.200 6648677.700)
         102  POINT (265764.000 6644063.900)
         103  POINT (265970.700 6651258.500)
         104  POINT (264624.300 6649937.700)
         ..                              ...
         195  POINT (258175.600 6653694.300)
         196  POINT (258772.200 6652487.600)
         197  POINT (273135.300 6653198.100)
         198  POINT (270582.300 6652163.800)
         199  POINT (264980.800 6647231.300)
-
         [100 rows x 1 columns]
 
         Travel time from 100 to 100 points.
 
         >>> od = nwa.od_cost_matrix(origins, destinations)
         >>> od
               origin  destination    minutes
@@ -328,15 +329,14 @@
         4          0          104   5.882124
         ...      ...          ...        ...
         9995      99          195  20.488644
         9996      99          196  16.721241
         9997      99          197  19.977029
         9998      99          198  15.233163
         9999      99          199   6.439002
-
         [10000 rows x 3 columns]
 
         Join the results onto the 'origins' GeoDataFrame via the index.
 
         >>> joined = origins.join(od.set_index("origin"))
         >>> joined
                                   geometry  destination    minutes
@@ -347,15 +347,14 @@
         0   POINT (263122.700 6651184.900)          104   5.882124
         ..                             ...          ...        ...
         99  POINT (265622.800 6644644.200)          195  20.488644
         99  POINT (265622.800 6644644.200)          196  16.721241
         99  POINT (265622.800 6644644.200)          197  19.977029
         99  POINT (265622.800 6644644.200)          198  15.233163
         99  POINT (265622.800 6644644.200)          199   6.439002
-
         [10000 rows x 3 columns]
 
         Get travel times below 10 minutes.
 
         >>> less_than_10_min = od.loc[od.minutes < 10]
         >>> joined = origins.join(less_than_10_min.set_index("origin"))
         >>> joined
@@ -367,15 +366,14 @@
         0   POINT (263122.700 6651184.900)        106.0  9.811828
         ..                             ...          ...       ...
         99  POINT (265622.800 6644644.200)        173.0  4.305523
         99  POINT (265622.800 6644644.200)        174.0  6.094040
         99  POINT (265622.800 6644644.200)        177.0  5.944194
         99  POINT (265622.800 6644644.200)        183.0  8.449906
         99  POINT (265622.800 6644644.200)        199.0  6.439002
-
         [2195 rows x 3 columns]
 
         Get the three fastest routes from each origin.
 
         >>> three_fastest = od.loc[od.groupby("origin")["minutes"].rank() <= 3]
         >>> joined = origins.join(three_fastest.set_index("origin"))
         >>> joined
@@ -387,15 +385,14 @@
         1   POINT (272456.100 6653369.500)        184.0  2.754545
         ..                             ...          ...       ...
         98  POINT (272322.700 6653729.100)        184.0  3.175472
         98  POINT (272322.700 6653729.100)        189.0  3.179428
         99  POINT (265622.800 6644644.200)        102.0  1.648705
         99  POINT (265622.800 6644644.200)        134.0  1.116209
         99  POINT (265622.800 6644644.200)        156.0  1.368926
-
         [294 rows x 3 columns]
 
         Assign aggregated values directly onto the origins via the index.
 
         >>> origins["minutes_mean"] = od.groupby("origin")["minutes"].mean()
         >>> origins
                                   geometry  minutes_mean
@@ -406,14 +403,15 @@
         4   POINT (272876.200 6652889.100)     17.565747
         ..                             ...           ...
         95  POINT (270348.000 6651899.400)     15.427027
         96  POINT (264845.600 6649005.800)     11.239592
         97  POINT (263162.000 6650732.200)     11.904372
         98  POINT (272322.700 6653729.100)     17.579399
         99  POINT (265622.800 6644644.200)     12.185800
+        [100 rows x 2 columns]
 
         Use set_index to use column as identifier insted of the index.
 
         >>> origins["letter"] = np.random.choice([*"abc"], len(origins))
         >>> od = nwa.od_cost_matrix(origins.set_index("letter"), destinations)
         >>> od
              origin  destination    minutes
@@ -424,15 +422,14 @@
         4         a          104   5.882124
         ...     ...          ...        ...
         9995      b          195  20.488644
         9996      b          196  16.721241
         9997      b          197  19.977029
         9998      b          198  15.233163
         9999      b          199   6.439002
-
         [10000 rows x 3 columns]
 
         Travel time from 1000 to 1000 points rowwise.
 
         >>> points_reversed = points.iloc[::-1].reset_index(drop=True)
         >>> od = nwa.od_cost_matrix(points, points_reversed, rowwise=True)
         >>> od
@@ -444,34 +441,31 @@
         4         4            4  16.521346
         ..      ...          ...        ...
         995     995          995  16.794610
         996     996          996   9.611700
         997     997          997  19.968743
         998     998          998   9.484374
         999     999          999  14.892648
-
         [1000 rows x 3 columns]
+
         """
         if self._log:
             time_ = perf_counter()
 
-        self._prepare_network_analysis(origins, destinations)
+        self._prepare_network_analysis(origins, destinations, rowwise)
 
         results = _od_cost_matrix(
             graph=self.graph,
             origins=self.origins.gdf,
             destinations=self.destinations.gdf,
             weight=self.rules.weight,
             lines=lines,
             rowwise=rowwise,
         )
 
-        self.origins._get_n_missing(results, "origin")
-        self.destinations._get_n_missing(results, "destination")
-
         results["origin"] = results["origin"].map(self.origins.idx_dict)
         results["destination"] = results["destination"].map(self.destinations.idx_dict)
 
         if lines:
             results = _push_geom_col(results)
 
         if self.rules.split_lines:
@@ -515,20 +509,25 @@
             containing the indices of the origins and destinations GeoDataFrames.
 
         Raises:
             ValueError: if no paths were found.
 
         Examples
         --------
+        Create the NetworkAnalysis instance.
+
+        >>> import sgis as sg
+        >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_eidskog_2022.parquet")
+        >>> nw = sg.DirectedNetwork(roads).remove_isolated().make_directed_network_norway()
+        >>> rules = sg.NetworkAnalysisRules(weight="minutes")
+        >>> nwa = sg.NetworkAnalysis(network=nw, rules=rules, detailed_log=False)
+
         Get routes from 1 to 1000 points.
 
-        import sgis as sg
-        >>> points = sg.read_parquet_url(
-        ...     "https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet"
-        ... )
+        >>> points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
 
         >>> routes = nwa.get_route(points.iloc[[0]], points)
         >>> routes
             origin  destination    minutes                                           geometry
         0         1            2  12.930588  MULTILINESTRING Z ((272281.367 6653079.745 160...
         1         1            3  10.867076  MULTILINESTRING Z ((270054.367 6653367.774 144...
         2         1            4   8.075722  MULTILINESTRING Z ((259735.774 6650362.886 24....
@@ -542,34 +541,28 @@
         996       1         1000  14.657289  MULTILINESTRING Z ((264475.675 6644245.782 114...
 
         [997 rows x 4 columns]
         """
         if self._log:
             time_ = perf_counter()
 
-        self._prepare_network_analysis(origins, destinations)
+        self._prepare_network_analysis(origins, destinations, rowwise)
 
         results = _get_route(
             graph=self.graph,
             origins=self.origins.gdf,
             destinations=self.destinations.gdf,
             weight=self.rules.weight,
             roads=self.network.gdf,
             rowwise=rowwise,
         )
 
-        self.origins._get_n_missing(results, "origin")
-        self.destinations._get_n_missing(results, "destination")
-
         results["origin"] = results["origin"].map(self.origins.idx_dict)
         results["destination"] = results["destination"].map(self.destinations.idx_dict)
 
-        if isinstance(results, GeoDataFrame):
-            results = _push_geom_col(results)
-
         if self.rules.split_lines:
             self._unsplit_network()
 
         if self._log:
             minutes_elapsed = round((perf_counter() - time_) / 60, 1)
             self._runlog(
                 "get_route",
@@ -624,18 +617,23 @@
 
         Raises:
             ValueError: if no paths were found.
             ValueError: if drop_middle_percent is not between 0 and 100.
 
         Examples
         --------
-        import sgis as sg
-        >>> points = sg.read_parquet_url(
-        ...     "https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet"
-        ... )
+        Create the NetworkAnalysis instance.
+
+        >>> import sgis as sg
+        >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_eidskog_2022.parquet")
+        >>> nw = sg.DirectedNetwork(roads).remove_isolated().make_directed_network_norway()
+        >>> rules = sg.NetworkAnalysisRules(weight="minutes")
+        >>> nwa = sg.NetworkAnalysis(network=nw, rules=rules, detailed_log=False)
+
+        >>> points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
         >>> point1 = points.iloc[[0]]
         >>> point2 = points.iloc[[1]]
 
         Getting 10 fastest routes from one point to another point.
 
         >>> k_routes = nwa.get_k_routes(
         ...             point1,
@@ -652,16 +650,17 @@
         4       0            1  14.962593   5  MULTILINESTRING Z ((271257.900 6654378.100 193...
         5       0            1  15.423934   6  MULTILINESTRING Z ((272281.367 6653079.745 160...
         6       0            1  16.217271   7  MULTILINESTRING Z ((272281.367 6653079.745 160...
         7       0            1  16.483982   8  MULTILINESTRING Z ((272281.367 6653079.745 160...
         8       0            1  16.513253   9  MULTILINESTRING Z ((272281.367 6653079.745 160...
         9       0            1  16.551196  10  MULTILINESTRING Z ((272281.367 6653079.745 160...
 
-        We got all 10 routes because only the middle 1 percent of the routes are removed in
-        each iteration. Let's compare with dropping middle 50 and middle 100 percent.
+        We got all 10 routes because only the middle 1 percent of the routes are
+        removed in each iteration. Let's compare with dropping middle 50 and middle
+        100 percent.
 
         >>> k_routes = nwa.get_k_routes(
         ...             point1,
         ...             point2,
         ...             k=10,
         ...             drop_middle_percent=50
         ...         )
@@ -685,30 +684,27 @@
         """
         if not 0 <= drop_middle_percent <= 100:
             raise ValueError("'drop_middle_percent' should be between 0 and 100")
 
         if self._log:
             time_ = perf_counter()
 
-        self._prepare_network_analysis(origins, destinations)
+        self._prepare_network_analysis(origins, destinations, rowwise)
 
-        results = _get_route(
+        results = _get_k_routes(
             graph=self.graph,
             origins=self.origins.gdf,
             destinations=self.destinations.gdf,
             weight=self.rules.weight,
             roads=self.network.gdf,
             rowwise=rowwise,
             k=k,
             drop_middle_percent=drop_middle_percent,
         )
 
-        self.origins._get_n_missing(results, "origin")
-        self.destinations._get_n_missing(results, "destination")
-
         results["origin"] = results["origin"].map(self.origins.idx_dict)
         results["destination"] = results["destination"].map(self.destinations.idx_dict)
 
         if isinstance(results, GeoDataFrame):
             results = _push_geom_col(results)
 
         if self.rules.split_lines:
@@ -725,84 +721,189 @@
 
         return results
 
     def get_route_frequencies(
         self,
         origins: GeoDataFrame,
         destinations: GeoDataFrame,
+        weight_df: DataFrame | None = None,
+        rowwise: bool = False,
         frequency_col: str = "frequency",
     ) -> GeoDataFrame:
         """Finds the number of times each line segment was visited in all trips.
 
         Finds the route with the lowest cost (minutes, meters, etc.) from a set of
         origins to a set of destinations and summarises the number of times each
         segment was used. The aggregation is done on the line indices, which is much
         faster than getting the geometries and then dissolving.
 
+        The trip frequencies can be weighted (multiplied) based on 'weight_df'. See
+        example below.
+
         Args:
-            origins: GeoDataFrame of points from where the routes will originate
-            destinations: GeoDataFrame of points from where the routes will terminate
+            origins: GeoDataFrame of points from where the routes will originate.
+            destinations: GeoDataFrame of points from where the routes will terminate.
+            weight_df: A long formated DataFrame where each row contains the indices of
+                an origin-destination pair and the number to multiply the frequency for
+                this route by. The DataFrame can either contain three columns (origin
+                index, destination index and weight. In that order) or only a weight
+                column and a MultiIndex where level 0 is origin index and level 1 is
+                destination index.
             frequency_col: Name of column with the number of times each road was
                 visited. Defaults to 'frequency'.
 
         Returns:
             A GeoDataFrame with all line segments that were visited at least once,
             with a column with the number of times the line segment was used in the
             individual routes.
 
         Note:
             The resulting lines will keep all columns of the 'gdf' of the Network.
 
         Raises:
-            ValueError: if no paths were found.
+            ValueError: If no paths were found.
+            ValueError: If weight_df is not a DataFrame with one or three columns.
+            ValueError: If weight_df is given and the index of origins/destinations
+                is not unique.
 
         Examples
         --------
+        Create the NetworkAnalysis instance.
+
+        >>> import sgis as sg
+        >>> import pandas as pd
+        >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_eidskog_2022.parquet")
+        >>> nw = sg.DirectedNetwork(roads).remove_isolated().make_directed_network_norway()
+        >>> rules = sg.NetworkAnalysisRules(weight="minutes")
+        >>> nwa = sg.NetworkAnalysis(network=nw, rules=rules, detailed_log=False)
+
         Get number of times each road was visited for trips from 25 to 25 points.
 
-        import sgis as sg
-        >>> points = sg.read_parquet_url(
-        ...     "https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet"
+        >>> points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
+
+        >>> origins = points.iloc[:25]
+        >>> destinations = points.iloc[25:50]
+        >>> frequencies = nwa.get_route_frequencies(origins, destinations)
+        >>> frequencies[["source", "target", "frequency", "geometry"]]
+               source target  frequency                                           geometry
+        160188  77264  79112        1.0  LINESTRING Z (268641.225 6651871.624 111.355, ...
+        153682  68376   4136        1.0  LINESTRING Z (268542.700 6652162.400 121.266, ...
+        153679  75263  75502        1.0  LINESTRING Z (268665.600 6652165.400 117.466, ...
+        153678  75262  75263        1.0  LINESTRING Z (268660.000 6652167.100 117.466, ...
+        153677  47999  75262        1.0  LINESTRING Z (268631.500 6652176.800 118.166, ...
+        ...       ...    ...        ...                                                ...
+        151465  73801  73802      103.0  LINESTRING Z (265368.600 6647142.900 131.660, ...
+        151464  73800  73801      103.0  LINESTRING Z (265362.800 6647137.100 131.660, ...
+        151466  73802  73632      103.0  LINESTRING Z (265371.400 6647147.900 131.660, ...
+        151463  73799  73800      123.0  LINESTRING Z (265359.600 6647135.400 131.660, ...
+        152170  74418  74246      130.0  LINESTRING Z (264579.835 6651954.573 113.209, ...
+
+        [8556 rows x 4 columns]
+
+        The frequencies can be weighted for each origin-destination pair by specifying
+        'weight_df'. This can be a DataFrame with three columns, where the first two
+        contain the indices of the origin and destination (in that order), and the
+        third the number to multiply the frequency by. 'weight_df' can also be a
+        DataFrame with a 2-leveled MultiIndex, where level 0 is the origin index and
+        level 1 is the destination.
+
+        Constructing a DataFrame with all od-pair combinations and give all rows a
+        weight of 10.
+
+        >>> od_pairs = pd.MultiIndex.from_product(
+        ...     [origins.index, destinations.index], names=["origin", "destination"]
         ... )
+        >>> weight_df = pd.DataFrame(index=od_pairs).reset_index()
+        >>> weight_df["weight"] = 10
+        >>> weight_df
+             origin  destination  weight
+        0         0           25      10
+        1         0           26      10
+        2         0           27      10
+        3         0           28      10
+        4         0           29      10
+        ..      ...          ...     ...
+        620      24           45      10
+        621      24           46      10
+        622      24           47      10
+        623      24           48      10
+        624      24           49      10
+
+        [625 rows x 3 columns]
+
+        All frequencies will now be multiplied by 10.
 
-        >>> frequencies = nwa.get_route_frequencies(points.sample(25), points.sample(25))
+        >>> frequencies = nwa.get_route_frequencies(origins, destinations, weight_df, weight_df=weight_df)
         >>> frequencies[["source", "target", "frequency", "geometry"]]
-               source target   frequency                                          geometry
-        137866  19095  44962    1.0      LINESTRING Z (265476.114 6645475.318 160.724, ...
-        138905  30597  16266    1.0      LINESTRING Z (272648.400 6652234.800 178.170, ...
-        138903  16266  45388    1.0      LINESTRING Z (272642.602 6652236.229 178.687, ...
-        138894  43025  30588    1.0      LINESTRING Z (272446.600 6652253.700 162.970, ...
-        138892  30588  16021    1.0      LINESTRING Z (272414.400 6652263.100 161.170, ...
-        ...       ...    ...    ...                                                    ...
-        158287  78157  78156  176.0      LINESTRING Z (263975.482 6653605.092 132.739, ...
-        149697  72562  72563  180.0      LINESTRING Z (265179.202 6651549.723 81.532, 2...
-        149698  72563  72564  180.0      LINESTRING Z (265178.761 6651549.956 81.561, 2...
-        149695  72560  72561  180.0      LINESTRING Z (265457.755 6651249.238 76.502, 2...
-        149696  72561  72562  180.0      LINESTRING Z (265180.086 6651549.259 81.473, 2...
 
-        [12231 rows x 4 columns]
+               source target  frequency                                           geometry
+        160188  77264  79112       10.0  LINESTRING Z (268641.225 6651871.624 111.355, ...
+        153682  68376   4136       10.0  LINESTRING Z (268542.700 6652162.400 121.266, ...
+        153679  75263  75502       10.0  LINESTRING Z (268665.600 6652165.400 117.466, ...
+        153678  75262  75263       10.0  LINESTRING Z (268660.000 6652167.100 117.466, ...
+        153677  47999  75262       10.0  LINESTRING Z (268631.500 6652176.800 118.166, ...
+        ...       ...    ...        ...                                                ...
+        151465  73801  73802     1030.0  LINESTRING Z (265368.600 6647142.900 131.660, ...
+        151464  73800  73801     1030.0  LINESTRING Z (265362.800 6647137.100 131.660, ...
+        151466  73802  73632     1030.0  LINESTRING Z (265371.400 6647147.900 131.660, ...
+        151463  73799  73800     1230.0  LINESTRING Z (265359.600 6647135.400 131.660, ...
+        152170  74418  74246     1300.0  LINESTRING Z (264579.835 6651954.573 113.209, ...
+
+        [8556 rows x 4 columns]
+
+        'weight_df' can also be a DataFrame with one column (the weight) and a
+        MultiIndex.
+
+        >>> weight_df = pd.DataFrame(index=od_pairs)
+        >>> weight_df["weight"] = 10
+        >>> weight_df
+               weight
+        0  25      10
+           26      10
+           27      10
+           28      10
+           29      10
+        ...       ...
+        24 45      10
+           46      10
+           47      10
+           48      10
+           49      10
+
         """
         if self._log:
             time_ = perf_counter()
 
-        self._prepare_network_analysis(origins, destinations)
+        if weight_df is not None:
+            weight_df = self._prepare_weight_df(weight_df, origins, destinations)
 
-        results = _get_route(
+        self._prepare_network_analysis(origins, destinations, rowwise)
+
+        if weight_df is not None:
+            ori_idx_mapper = {v: k for k, v in self.origins.idx_dict.items()}
+            des_idx_mapper = {v: k for k, v in self.destinations.idx_dict.items()}
+            multiindex_mapper = lambda x: (
+                ori_idx_mapper.get(x[0]),
+                des_idx_mapper.get(x[1]),
+            )
+            weight_df.index = weight_df.index.map(multiindex_mapper)
+
+        results = _get_route_frequencies(
             graph=self.graph,
             origins=self.origins.gdf,
             destinations=self.destinations.gdf,
-            weight=self.rules.weight,
             roads=self.network.gdf,
-            summarise=True,
+            weight_df=weight_df,
+            rowwise=rowwise,
         )
 
         if isinstance(results, GeoDataFrame):
             results = _push_geom_col(results)
 
-        results = results.rename(columns={"n": frequency_col}).sort_values(
+        results = results.rename(columns={"frequency": frequency_col}).sort_values(
             frequency_col
         )
 
         if self.rules.split_lines:
             self._unsplit_network()
 
         if self._log:
@@ -845,21 +946,25 @@
 
         See also:
             precice_service_area: Equivelent method where lines are also cut to get
                 precice results.
 
         Examples
         --------
-        import sgis as sg
-        >>> points = sg.read_parquet_url(
-        ...     "https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet"
-        ... )
+        Create the NetworkAnalysis instance.
+
+        >>> import sgis as sg
+        >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_eidskog_2022.parquet")
+        >>> nw = sg.DirectedNetwork(roads).remove_isolated().make_directed_network_norway()
+        >>> rules = sg.NetworkAnalysisRules(weight="minutes")
+        >>> nwa = sg.NetworkAnalysis(network=nw, rules=rules, detailed_log=False)
 
         10 minute service area for three origin points.
 
+        >>> points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
         >>> service_areas = nwa.service_area(
         ...         points.loc[:2],
         ...         breaks=10,
         ... )
         >>> service_areas
            origin  minutes                                           geometry
         0       0       10  MULTILINESTRING Z ((264348.673 6648271.134 17....
@@ -886,18 +991,14 @@
             time_ = perf_counter()
 
         self._prepare_network_analysis(origins)
 
         # sort the breaks as an np.ndarray
         breaks = self._sort_breaks(breaks)
 
-        self.network.gdf["source_target_weight"] = _edge_ids(
-            self.network.gdf, self.rules.weight
-        )
-
         results = _service_area(
             graph=self.graph,
             origins=self.origins.gdf,
             breaks=breaks,
             weight=self.rules.weight,
             lines=self.network.gdf,
             nodes=self.network.nodes,
@@ -973,21 +1074,26 @@
             network.gdf as well.
 
         See also:
             service_area: Faster method where lines are not cut to get precice results.
 
         Examples
         --------
-        import sgis as sg
-        >>> points = sg.read_parquet_url(
-        ...     "https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet"
-        ... )
+        Create the NetworkAnalysis instance.
+
+        >>> import sgis as sg
+        >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_eidskog_2022.parquet")
+        >>> nw = sg.DirectedNetwork(roads).remove_isolated().make_directed_network_norway()
+        >>> rules = sg.NetworkAnalysisRules(weight="minutes")
+        >>> nwa = sg.NetworkAnalysis(network=nw, rules=rules, detailed_log=False)
 
         10 minute service area for one origin point.
 
+        >>> points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
+
         >>> sa = nwa.precice_service_area(
         ...         points.iloc[[0]],
         ...         breaks=10,
         ...     )
         >>> sa
             idx  minutes                                           geometry
         0    1       10  MULTILINESTRING Z ((264348.673 6648271.134 17....
@@ -1012,18 +1118,14 @@
             time_ = perf_counter()
 
         self._prepare_network_analysis(origins)
 
         # sort the breaks as an np.ndarray
         breaks = self._sort_breaks(breaks)
 
-        self.network.gdf["source_target_weight"] = _edge_ids(
-            self.network.gdf, self.rules.weight
-        )
-
         results = _service_area(
             graph=self.graph,
             origins=self.origins.gdf,
             breaks=breaks,
             weight=self.rules.weight,
             lines=self.network.gdf,
             nodes=self.network.nodes,
@@ -1066,14 +1168,72 @@
                 minutes_elapsed,
                 breaks=breaks,
                 dissolve=dissolve,
             )
 
         return results
 
+    @staticmethod
+    def _prepare_weight_df(weight_df, origins, destinations):
+        """Copy weight_df, convert to MultiIndex (if needed), then validate it.
+
+        The weight_df needs to have a very specific shape and index. If a 3-columned df
+        is given, convert the first two to a MultiIndex.
+
+        Then make sure this index matches the index of origins and destinations.
+        """
+        error_message = (
+            "'weight_df' should be a DataFrame with the columns "
+            "'origin', 'destination' and 'weight', where the first "
+            "two contain the indices of the origins and destinations "
+            "and the weight column contains the number to multiply "
+            "the trip frequency for this origin-destination pair."
+        )
+
+        if not isinstance(weight_df, DataFrame):
+            raise ValueError(error_message)
+
+        weight_df = weight_df.copy()
+
+        if len(weight_df.columns) == 3:
+            weight_df = weight_df.set_index(list(weight_df.columns[:2]))
+
+        if len(weight_df.columns) != 1 and isinstance(weight_df.index, pd.MultiIndex):
+            raise ValueError(error_message)
+
+        if not weight_df.index.is_unique:
+            raise ValueError("'weight_df' must contain only unique OD combinations.")
+
+        if not origins.index.is_unique:
+            raise ValueError(
+                "The index of 'origins' must be unque when using a 'weight_df'."
+            )
+        if not destinations.index.is_unique:
+            raise ValueError(
+                "The index of 'destinations' must be unque when using a 'weight_df'."
+            )
+
+        # check if any/all indices are in origins/destinations.
+        # Doing 'any' to give better error message
+        level_0 = weight_df.index.get_level_values(0)
+        if not level_0.isin(origins.index).any():
+            raise ValueError("None of the 'origins' indices are in 'weight_df'.")
+
+        level_1 = weight_df.index.get_level_values(1)
+        if not level_1.isin(destinations.index).any():
+            raise ValueError("None of the 'destinations' indices are in 'weight_df'.")
+
+        if not level_0.isin(origins.index).all():
+            raise ValueError("Not all 'origins' indices are in 'weight_df'.")
+
+        if not level_1.isin(destinations.index).all():
+            raise ValueError("Not all 'destinations' indices are in 'weight_df'.")
+
+        return weight_df
+
     def _log_df_template(self, method: str, minutes_elapsed: float) -> DataFrame:
         """Creates a DataFrame with one row and the main columns.
 
         To be run after each network analysis.
 
         Args:
             method: the name of the network analysis method used
@@ -1145,21 +1305,30 @@
                 if isinstance(value, (list, tuple)):
                     value = [str(x) for x in value]
                     value = ", ".join(value)
                 df[key] = value
 
         self.log = pd.concat([self.log, df], ignore_index=True)
 
-    def _prepare_network_analysis(self, origins, destinations=None) -> None:
+    def _prepare_network_analysis(
+        self, origins, destinations=None, rowwise=False
+    ) -> None:
         """Prepares the weight column, node ids, origins, destinations and graph.
 
         Updates the graph only if it is not yet created and no parts of the analysis
         has changed. this method is run inside od_cost_matrix, get_route and
         service_area.
         """
+
+        if rowwise and len(origins) != len(destinations):
+            raise ValueError(
+                "'origins' and 'destinations' must have the same length when "
+                "rowwise=True"
+            )
+
         self.network.gdf = self.rules._validate_weight(self.network.gdf)
 
         self.origins = Origins(origins)
         self.origins._make_temp_idx(
             start=max(self.network.nodes.node_id.astype(int)) + 1
         )
 
@@ -1171,26 +1340,31 @@
 
         else:
             self.destinations = None
 
         if not self._graph_is_up_to_date() or not self.network._nodes_are_up_to_date():
             self.network._update_nodes_if()
 
-            edges, weights = self._get_edges_and_weights()
+            edges, weights, ids = self._get_edges_and_weights()
 
             self.graph = self._make_graph(
-                edges=edges, weights=weights, directed=self.network._as_directed
+                edges=edges,
+                weights=weights,
+                edge_ids=ids,
+                directed=self.network._as_directed,
             )
 
             self._add_missing_vertices()
 
         self._update_wkts()
         self.rules._update_rules()
 
-    def _get_edges_and_weights(self) -> tuple[list[tuple[str, str]], list[float]]:
+    def _get_edges_and_weights(
+        self,
+    ) -> tuple[list[tuple[str, str]], list[float], list[str]]:
         """Creates lists of edges and weights which will be used to make the graph.
 
         Edges and weights between origins and nodes and nodes and destinations are
         also added.
         """
         if self.rules.split_lines:
             self._split_lines()
@@ -1199,43 +1373,45 @@
                 start=max(self.network.nodes.node_id.astype(int)) + 1
             )
             if self.destinations is not None:
                 self.destinations._make_temp_idx(
                     start=max(self.origins.gdf.temp_idx.astype(int)) + 1
                 )
 
-        edges = [
-            (str(source), str(target))
-            for source, target in zip(
-                self.network.gdf["source"], self.network.gdf["target"], strict=True
-            )
-        ]
+        edges: list[tuple[str, str]] = self.network.get_edges()
 
         weights = list(self.network.gdf[self.rules.weight])
 
+        self.network.gdf["source_target_weight"] = self.network._create_edge_ids(
+            edges, weights
+        )
+
         edges_start, weights_start = self.origins._get_edges_and_weights(
             nodes=self.network.nodes,
             rules=self.rules,
         )
 
         edges = edges + edges_start
         weights = weights + weights_start
 
         if self.destinations is None:
-            return edges, weights
+            edge_ids = self.network._create_edge_ids(edges, weights)
+            return edges, weights, edge_ids
 
         edges_end, weights_end = self.destinations._get_edges_and_weights(
             nodes=self.network.nodes,
             rules=self.rules,
         )
 
         edges = edges + edges_end
         weights = weights + weights_end
 
-        return edges, weights
+        edge_ids = self.network._create_edge_ids(edges, weights)
+
+        return edges, weights, edge_ids
 
     def _split_lines(self) -> None:
         if self.destinations is not None:
             points = pd.concat(
                 [self.origins.gdf, self.destinations.gdf], ignore_index=True
             )
         else:
@@ -1300,23 +1476,24 @@
                 ]
             )
 
     @staticmethod
     def _make_graph(
         edges: list[tuple[str, ...]] | np.ndarray[tuple[str, ...]],
         weights: list[float] | np.ndarray[float],
+        edge_ids: np.ndarray,
         directed: bool,
     ) -> Graph:
         """Creates an igraph Graph from a list of edges and weights."""
         assert len(edges) == len(weights)
 
         graph = igraph.Graph.TupleList(edges, directed=directed)
 
         graph.es["weight"] = weights
-        graph.es["source_target_weight"] = _edge_ids(edges, weights)
+        graph.es["source_target_weight"] = edge_ids
         graph.es["edge_tuples"] = edges
         graph.es["source"] = [edge[0] for edge in edges]
         graph.es["target"] = [edge[1] for edge in edges]
 
         assert min(graph.es["weight"]) >= 0
 
         return graph
@@ -1335,14 +1512,15 @@
 
         for points in ["origins", "destinations"]:
             if not hasattr(self.wkts, points):
                 return False
             if self._points_have_changed(self[points].gdf, what=points):
                 return False
 
+        #        if not self.gdf["source_target_weight"].
         return True
 
     def _points_have_changed(self, points: GeoDataFrame, what: str) -> bool:
         """Check if the origins or destinations have changed.
 
         This method is best stored in the NetworkAnalysis class,
         since the point classes are instantiated each time an analysis is run.
```

### Comparing `ssb_sgis-0.1.5/src/sgis/networkanalysis/networkanalysisrules.py` & `ssb_sgis-0.1.6/src/sgis/networkanalysis/networkanalysisrules.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,19 +66,19 @@
 
     >>> nw = (sg.DirectedNetwork(roads)
     ...       .remove_isolated()
     ...       .make_directed_network_norway()
     ... )
     >>> rules = sg.NetworkAnalysisRules(weight="minutes")
     >>> nwa = sg.NetworkAnalysis(network=nw, rules=rules)
-
     >>> nwa
     NetworkAnalysis(
         network=DirectedNetwork(6364 km, percent_bidirectional=87),
-        rules=NetworkAnalysisRules(weight=minutes, search_tolerance=250, search_factor=0, split_lines=False, ...)
+        rules=NetworkAnalysisRules(weight=minutes, search_tolerance=250, search_factor=0, split_lines=False, ...),
+        log=True, detailed_log=True,
     )
 
     Setting 'split_lines' to True, means the points will be connected to the closest
     part of the closest network line. If False, the lines are connected to the closest
     endpoint of the lines. split_lines defaults to False, since splitting lines takes
     some time and doesn't make a huge difference in most cases.
```

### Comparing `ssb_sgis-0.1.5/src/sgis/read_parquet.py` & `ssb_sgis-0.1.6/src/sgis/read_parquet.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.5/PKG-INFO` & `ssb_sgis-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-sgis
-Version: 0.1.5
+Version: 0.1.6
 Summary: GIS functions used at Statistics Norway.
 Home-page: https://github.com/statisticsnorway/ssb-sgis
 License: MIT
 Author: Statistics Norway
 Author-email: ort@ssb.no
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 3 - Alpha
@@ -64,15 +64,15 @@
 
 ## Network analysis examples
 
 Preparing for network analysis:
 
 ```python
 import sgis as sg
-
+import pandas as pd
 
 roads = sg.read_parquet_url(
     "https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet"
 )
 
 nw = (
     sg.DirectedNetwork(roads)
@@ -93,22 +93,31 @@
 
     NetworkAnalysis(
         network=DirectedNetwork(6364 km, percent_bidirectional=87),
         rules=NetworkAnalysisRules(weight=minutes, search_tolerance=250, search_factor=0, split_lines=False, ...),
         log=True, detailed_log=True,
     )
 
-Get number of times each line segment was visited.
+Get number of times each line segment was visited, with optional weighting.
 
 ```python
-frequencies = nwa.get_route_frequencies(points.sample(75), points.sample(75))
+origins = points.iloc[:75]
+destinations = points.iloc[75:150]
+
+# creating uniform weights of 10
+od_pairs = pd.MultiIndex.from_product([origins.index, destinations.index])
+weights = pd.DataFrame(index=od_pairs)
+weights["weight"] = 10
 
+frequencies = nwa.get_route_frequencies(origins, destinations, weight_df=weights)
+
+# plot the results
 m = sg.ThematicMap(sg.buff(frequencies, 15), column="frequency", black=True)
 m.cmap = "plasma"
-m.title = "Number of times each road was used."
+m.title = "Number of times each road was used,\nweighted * 10"
 m.plot()
 ```
 
 ![png](docs/examples/network_analysis_examples_files/network_analysis_examples_5_0.png)
 
 Fast many-to-many travel times/distances.
 
@@ -137,14 +146,15 @@
 
 ```python
 service_areas = nwa.service_area(
     points.iloc[[0]],
     breaks=np.arange(1, 11),
 )
 
+# plot the results
 m = sg.ThematicMap(service_areas, column="minutes", black=True, size=10)
 m.k = 10
 m.title = "Roads that can be reached within 1 to 10 minutes"
 m.plot()
 ```
 
 ![png](docs/examples/network_analysis_examples_files/network_analysis_examples_9_0.png)
@@ -160,16 +170,14 @@
 m.title = "Four fastest routes from A to B"
 m.legend.title = "Rank"
 m.plot()
 ```
 
 ![png](docs/examples/network_analysis_examples_files/network_analysis_examples_11_0.png)
 
-More network analysis examples can be found here: https://github.com/statisticsnorway/ssb-sgis/blob/main/docs/network_analysis_demo_template.md
-
 Road data for Norway can be downloaded here: https://kartkatalog.geonorge.no/metadata/nvdb-ruteplan-nettverksdatasett/8d0f9066-34f9-4423-be12-8e8523089313
 
 ## Developer information
 
 ### Git LFS
 
 The data in the testdata directory is stored with [Git LFS](https://git-lfs.com/).
```

