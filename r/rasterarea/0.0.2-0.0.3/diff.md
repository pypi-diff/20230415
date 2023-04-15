# Comparing `tmp/rasterarea-0.0.2.tar.gz` & `tmp/rasterarea-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rasterarea-0.0.2.tar", last modified: Wed Apr  5 22:43:01 2023, max compression
+gzip compressed data, was "rasterarea-0.0.3.tar", last modified: Sat Apr 15 03:47:27 2023, max compression
```

## Comparing `rasterarea-0.0.2.tar` & `rasterarea-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:43:01.609341 rasterarea-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-05 22:42:52.000000 rasterarea-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-05 22:42:52.000000 rasterarea-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-05 22:43:01.609341 rasterarea-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-05 22:42:52.000000 rasterarea-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:43:01.609341 rasterarea-0.0.2/rasterarea/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-05 22:42:52.000000 rasterarea-0.0.2/rasterarea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-04-05 22:42:52.000000 rasterarea-0.0.2/rasterarea/rasterarea.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 22:43:01.609341 rasterarea-0.0.2/rasterarea.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-05 22:43:01.000000 rasterarea-0.0.2/rasterarea.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-05 22:43:01.000000 rasterarea-0.0.2/rasterarea.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-05 22:43:01.000000 rasterarea-0.0.2/rasterarea.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 22:43:01.000000 rasterarea-0.0.2/rasterarea.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-05 22:43:01.000000 rasterarea-0.0.2/rasterarea.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-05 22:43:01.000000 rasterarea-0.0.2/rasterarea.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-05 22:42:52.000000 rasterarea-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-05 22:43:01.609341 rasterarea-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-05 22:42:52.000000 rasterarea-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:47:27.216307 rasterarea-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-15 03:47:18.000000 rasterarea-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-15 03:47:18.000000 rasterarea-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-15 03:47:27.216307 rasterarea-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-15 03:47:18.000000 rasterarea-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:47:27.216307 rasterarea-0.0.3/rasterarea/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-15 03:47:18.000000 rasterarea-0.0.3/rasterarea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-15 03:47:18.000000 rasterarea-0.0.3/rasterarea/foliummap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-04-15 03:47:18.000000 rasterarea-0.0.3/rasterarea/ipyleafletmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-04-15 03:47:18.000000 rasterarea-0.0.3/rasterarea/rasterarea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:47:27.216307 rasterarea-0.0.3/rasterarea.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-15 03:47:27.000000 rasterarea-0.0.3/rasterarea.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-15 03:47:27.000000 rasterarea-0.0.3/rasterarea.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-15 03:47:27.000000 rasterarea-0.0.3/rasterarea.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 03:47:27.000000 rasterarea-0.0.3/rasterarea.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-15 03:47:27.000000 rasterarea-0.0.3/rasterarea.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-15 03:47:27.000000 rasterarea-0.0.3/rasterarea.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-15 03:47:18.000000 rasterarea-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-15 03:47:27.216307 rasterarea-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-15 03:47:18.000000 rasterarea-0.0.3/setup.py
```

### Comparing `rasterarea-0.0.2/LICENSE` & `rasterarea-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rasterarea-0.0.2/PKG-INFO` & `rasterarea-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rasterarea
-Version: 0.0.2
+Version: 0.0.3
 Summary: This package provides a more accurate way to claculate the area of rasters.
 Home-page: https://github.com/Feng96/rasterarea
 Author: Yinan Feng
 Author-email: 1041267458@qq.com
 License: MIT license
 Keywords: rasterarea
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `rasterarea-0.0.2/README.md` & `rasterarea-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `rasterarea-0.0.2/rasterarea/rasterarea.py` & `rasterarea-0.0.3/rasterarea/ipyleafletmap.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-"""Main module."""
-
-import random
-import string
 import ipyleaflet
 
 class Map(ipyleaflet.Map):
     
     def __init__(self, center=[20, 0], zoom=2, **kwargs) -> None:
 
         if "scroll_wheel_zoom" not in kwargs:
@@ -111,72 +107,97 @@
             attribution (str): The attribution of the tile layer.
             name (str, optional): The name of the tile layer. Defaults to "OpenStreetMap".
             kwargs: Keyword arguments to pass to the tile layer.
         """
         tile_layer = ipyleaflet.TileLayer(url=url, attribution=attribution, name=name, **kwargs)
         self.add_layer(tile_layer)
 
-    def add_basemap(self, basemap):
-        """Adds a basemap to the map.
+    def add_basemap(self, basemap, **kwargs):
 
-        Args:
-            basemap (str): The name of the basemap to add.
-        """
         import xyzservices.providers as xyz
-        try:
-            layer = eval(f"xyz.{basemap}")
-            url = layer.build_url()
-            attribution = layer.attribution
-            self.add_tile_layer(url=url, attribution=attribution, name=basemap)
 
-        except:
-            raise ValueError(f"Invalid basemap name: {basemap}")
-    
+        if basemap.lower() == "roadmap":
+            url = 'http://mt0.google.com/vt/lyrs=m&hl=en&x={x}&y={y}&z={z}'
+            self.add_tile_layer(url, name=basemap, **kwargs)
+        elif basemap.lower() == "satellite":
+            url = 'http://mt0.google.com/vt/lyrs=y&hl=en&x={x}&y={y}&z={z}'
+            self.add_tile_layer(url, name=basemap, **kwargs)
+        else:
+            try:
+                basemap = eval(f"xyz.{basemap}")
+                url = basemap.build_url()
+                attribution = basemap.attribution
+                self.add_tile_layer(url, name=basemap.name, attribution=attribution, **kwargs)
+            except:
+                raise ValueError(f"Basemap '{basemap}' not found.")
 
-    def add_geojson(self, data, **kwargs):
+    def add_geojson(self, data, name='GeoJSON', **kwargs):
         """Adds a GeoJSON layer to the map.
 
         Args:
             data (dict): The GeoJSON data.
-            kwargs: Keyword arguments to pass to the GeoJSON layer.
         """
-        import json
-
         if isinstance(data, str):
+            import json
             with open(data, "r") as f:
                 data = json.load(f)
-
-        geojson = ipyleaflet.GeoJSON(data=data, **kwargs)
+        geojson = ipyleaflet.GeoJSON(data=data,name=name, **kwargs)
         self.add_layer(geojson)
+
     
-        
-def generate_password(length=8):
-    """Generate a random password
+    def add_shp(self, data, name='Shapefile', **kwargs):
+        """Adds a Shapefile layer to the map.
 
-    Args:
-        length (int, optional): _description_. Defaults to 8.
+        Args:
+            data (str): The path to the Shapefile.
+        """
+        import geopandas as gpd
+        gdf = gpd.read_file(data)
+        geojson = gdf.__geo_interface__
+        self.add_geojson(geojson, name=name, **kwargs)
 
-    Returns:
-        _type_: _description_
-    """
-    # Define the set of characters to choose from
-    characters = string.ascii_letters + string.digits + string.punctuation
+    def add_vector(self, data, name='Vector', **kwargs):
+        """Adds a vector layer to the map.
 
-    # Generate the password
-    password = "".join(random.choice(characters) for i in range(length))
+        Args:
+            data (str): The path to the vector file.
+        """
+        import geopandas as gpd
+        gdf = gpd.read_file(data)
+        geojson = gdf.__geo_interface__
+        self.add_geojson(geojson, name=name, **kwargs)
 
-    return password
+    def add_raster(self, url, name='Raster', fit_bounds=True, **kwargs):
+        """Adds a raster layer to the map.
 
+        Args:
+            url (str): The URL of the raster layer.
+            name (str, optional): The name of the raster layer. Defaults to 'Raster'.
+            fit_bounds (bool, optional): Whether to fit the map bounds to the raster layer. Defaults to True.
+        """
+        import httpx
 
-def gnerate_lucky_number(length = 1):
-    """Generate your lucky number 
+        titiler_endpoint = "https://titiler.xyz"
 
-    Args:
-        length (int, optional): _description_. Defaults to 1.
+        r = httpx.get(
+            f"{titiler_endpoint}/cog/info",
+            params = {
+                "url": url,
+            }
+        ).json()
+
+        bounds = r["bounds"]
+
+        r = httpx.get(
+            f"{titiler_endpoint}/cog/tilejson.json",
+            params = {
+                "url": url,
+            }
+        ).json()
 
-    Returns:
-        _type_: _description_
-    """    
-    result_str = ''.join(random.choice(string.digits) for i in range(length))
-    return int(result_str)
+        tile = r["tiles"][0]
 
+        self.add_tile_layer(url=tile, name=name, **kwargs)
 
+        if fit_bounds:
+            bbox = [[bounds[1], bounds[0]], [bounds[3], bounds[2]]]
+            self.fit_bounds(bbox)
```

### Comparing `rasterarea-0.0.2/rasterarea.egg-info/PKG-INFO` & `rasterarea-0.0.3/rasterarea.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rasterarea
-Version: 0.0.2
+Version: 0.0.3
 Summary: This package provides a more accurate way to claculate the area of rasters.
 Home-page: https://github.com/Feng96/rasterarea
 Author: Yinan Feng
 Author-email: 1041267458@qq.com
 License: MIT license
 Keywords: rasterarea
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `rasterarea-0.0.2/setup.py` & `rasterarea-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='rasterarea',
     name='rasterarea',
     packages=find_packages(include=['rasterarea', 'rasterarea.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/Feng96/rasterarea',
-    version='0.0.2',
+    version='0.0.3',
     zip_safe=False,
 )
```

