# Comparing `tmp/allocine-seances-0.0.2.tar.gz` & `tmp/allocine-seances-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allocine-seances-0.0.2.tar", last modified: Sat Apr 15 18:24:26 2023, max compression
+gzip compressed data, was "allocine-seances-0.0.3.tar", last modified: Sat Apr 15 18:29:08 2023, max compression
```

## Comparing `allocine-seances-0.0.2.tar` & `allocine-seances-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 18:24:26.534231 allocine-seances-0.0.2/
--rw-rw-rw-   0        0        0     1088 2023-04-15 16:16:47.000000 allocine-seances-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     4595 2023-04-15 18:24:26.534231 allocine-seances-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2767 2023-04-15 17:20:12.000000 allocine-seances-0.0.2/README.md
--rw-rw-rw-   0        0        0      721 2023-04-15 18:23:32.000000 allocine-seances-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-15 18:24:26.534231 allocine-seances-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-15 18:24:26.518610 allocine-seances-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:24:26.518610 allocine-seances-0.0.2/src/allocineAPI/
--rw-rw-rw-   0        0        0      638 2023-04-14 22:38:09.000000 allocine-seances-0.0.2/src/allocineAPI/URLs.py
--rw-rw-rw-   0        0        0        0 2023-04-15 16:02:27.000000 allocine-seances-0.0.2/src/allocineAPI/__init__.py
--rw-rw-rw-   0        0        0     5585 2023-04-14 23:10:17.000000 allocine-seances-0.0.2/src/allocineAPI/allocineAPI.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:24:26.534231 allocine-seances-0.0.2/src/allocine_seances.egg-info/
--rw-rw-rw-   0        0        0     4595 2023-04-15 18:24:26.000000 allocine-seances-0.0.2/src/allocine_seances.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      334 2023-04-15 18:24:26.000000 allocine-seances-0.0.2/src/allocine_seances.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 18:24:26.000000 allocine-seances-0.0.2/src/allocine_seances.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-15 18:24:26.000000 allocine-seances-0.0.2/src/allocine_seances.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-15 18:24:26.000000 allocine-seances-0.0.2/src/allocine_seances.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 18:29:08.535679 allocine-seances-0.0.3/
+-rw-rw-rw-   0        0        0     1088 2023-04-15 16:16:47.000000 allocine-seances-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4595 2023-04-15 18:29:08.534683 allocine-seances-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2767 2023-04-15 17:20:12.000000 allocine-seances-0.0.3/README.md
+-rw-rw-rw-   0        0        0      721 2023-04-15 18:28:52.000000 allocine-seances-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-15 18:29:08.535679 allocine-seances-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-15 18:29:08.507677 allocine-seances-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:29:08.513678 allocine-seances-0.0.3/src/allocineAPI/
+-rw-rw-rw-   0        0        0        0 2023-04-15 16:02:27.000000 allocine-seances-0.0.3/src/allocineAPI/__init__.py
+-rw-rw-rw-   0        0        0     6200 2023-04-15 18:28:42.000000 allocine-seances-0.0.3/src/allocineAPI/allocineAPI.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:29:08.532678 allocine-seances-0.0.3/src/allocine_seances.egg-info/
+-rw-rw-rw-   0        0        0     4595 2023-04-15 18:29:08.000000 allocine-seances-0.0.3/src/allocine_seances.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-04-15 18:29:08.000000 allocine-seances-0.0.3/src/allocine_seances.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 18:29:08.000000 allocine-seances-0.0.3/src/allocine_seances.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-15 18:29:08.000000 allocine-seances-0.0.3/src/allocine_seances.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-15 18:29:08.000000 allocine-seances-0.0.3/src/allocine_seances.egg-info/top_level.txt
```

### Comparing `allocine-seances-0.0.2/LICENSE` & `allocine-seances-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `allocine-seances-0.0.2/PKG-INFO` & `allocine-seances-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allocine-seances
-Version: 0.0.2
+Version: 0.0.3
 Summary: Récupération des scéances de cinémas sur allociné
 Author-email: lefevre-dev <louislefevre.dev@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `allocine-seances-0.0.2/README.md` & `allocine-seances-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `allocine-seances-0.0.2/pyproject.toml` & `allocine-seances-0.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "allocine-seances"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="lefevre-dev", email="louislefevre.dev@gmail.com" },
 ]
 description = "Récupération des scéances de cinémas sur allociné"
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
```

### Comparing `allocine-seances-0.0.2/src/allocineAPI/allocineAPI.py` & `allocine-seances-0.0.3/src/allocineAPI/allocineAPI.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json
 import requests
 from bs4 import BeautifulSoup
-from URLs import URLs
 
 
 class allocineAPI:
     TOP_VILLE_TITLE = "Top villes"
     DEPARTEMENTS_TITLE = "Départements"
     CIRCUIT_TITLE = "Les cinémas par circuit"
 
@@ -135,14 +134,37 @@
                 "duration": duration,
                 "VF": list_vf,
                 "VO": list_vo
             })
         return formated_data
 
 
+class URLs:
+
+    BASE_URL = "https://www.allocine.fr/"
+    SEANCES = "salle/"
+    CINEMA = "cinema/"
+    SHOWTIMES = "_/showtimes/theater-"
+
+    @staticmethod
+    def seance_url():
+        return URLs.BASE_URL + URLs.SEANCES
+
+    @staticmethod
+    def cinemas_url(id_location):
+        if "circuit" in id_location:
+            return URLs.BASE_URL + URLs.SEANCES + id_location
+        else:
+            return URLs.BASE_URL + URLs.SEANCES + URLs.CINEMA + id_location
+
+    @staticmethod
+    def showtime_url(id_cinema, day_shift):
+        return URLs.BASE_URL + URLs.SHOWTIMES + id_cinema + "/d-" + str(day_shift)
+
+
 if __name__ == '__main__':
 
     api = allocineAPI()
 
     # ret = api.get_top_villes()
     # for elt in ret: print(elt)
```

### Comparing `allocine-seances-0.0.2/src/allocine_seances.egg-info/PKG-INFO` & `allocine-seances-0.0.3/src/allocine_seances.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allocine-seances
-Version: 0.0.2
+Version: 0.0.3
 Summary: Récupération des scéances de cinémas sur allociné
 Author-email: lefevre-dev <louislefevre.dev@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

