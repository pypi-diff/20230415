# Comparing `tmp/allocine-seances-0.0.3.tar.gz` & `tmp/allocine-seances-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allocine-seances-0.0.3.tar", last modified: Sat Apr 15 18:29:08 2023, max compression
+gzip compressed data, was "allocine-seances-0.0.4.tar", last modified: Sat Apr 15 18:36:10 2023, max compression
```

## Comparing `allocine-seances-0.0.3.tar` & `allocine-seances-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 18:29:08.535679 allocine-seances-0.0.3/
--rw-rw-rw-   0        0        0     1088 2023-04-15 16:16:47.000000 allocine-seances-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     4595 2023-04-15 18:29:08.534683 allocine-seances-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2767 2023-04-15 17:20:12.000000 allocine-seances-0.0.3/README.md
--rw-rw-rw-   0        0        0      721 2023-04-15 18:28:52.000000 allocine-seances-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-15 18:29:08.535679 allocine-seances-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-15 18:29:08.507677 allocine-seances-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 18:29:08.513678 allocine-seances-0.0.3/src/allocineAPI/
--rw-rw-rw-   0        0        0        0 2023-04-15 16:02:27.000000 allocine-seances-0.0.3/src/allocineAPI/__init__.py
--rw-rw-rw-   0        0        0     6200 2023-04-15 18:28:42.000000 allocine-seances-0.0.3/src/allocineAPI/allocineAPI.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:29:08.532678 allocine-seances-0.0.3/src/allocine_seances.egg-info/
--rw-rw-rw-   0        0        0     4595 2023-04-15 18:29:08.000000 allocine-seances-0.0.3/src/allocine_seances.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-04-15 18:29:08.000000 allocine-seances-0.0.3/src/allocine_seances.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 18:29:08.000000 allocine-seances-0.0.3/src/allocine_seances.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-15 18:29:08.000000 allocine-seances-0.0.3/src/allocine_seances.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-15 18:29:08.000000 allocine-seances-0.0.3/src/allocine_seances.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 18:36:10.165266 allocine-seances-0.0.4/
+-rw-rw-rw-   0        0        0     1088 2023-04-15 16:16:47.000000 allocine-seances-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     4607 2023-04-15 18:36:10.164264 allocine-seances-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2779 2023-04-15 18:32:35.000000 allocine-seances-0.0.4/README.md
+-rw-rw-rw-   0        0        0      721 2023-04-15 18:35:45.000000 allocine-seances-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-15 18:36:10.165266 allocine-seances-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-15 18:36:10.136269 allocine-seances-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:36:10.143264 allocine-seances-0.0.4/src/allocineAPI/
+-rw-rw-rw-   0        0        0        0 2023-04-15 16:02:27.000000 allocine-seances-0.0.4/src/allocineAPI/__init__.py
+-rw-rw-rw-   0        0        0     6200 2023-04-15 18:28:42.000000 allocine-seances-0.0.4/src/allocineAPI/allocineAPI.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:36:10.163265 allocine-seances-0.0.4/src/allocine_seances.egg-info/
+-rw-rw-rw-   0        0        0     4607 2023-04-15 18:36:10.000000 allocine-seances-0.0.4/src/allocine_seances.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-04-15 18:36:10.000000 allocine-seances-0.0.4/src/allocine_seances.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 18:36:10.000000 allocine-seances-0.0.4/src/allocine_seances.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-15 18:36:10.000000 allocine-seances-0.0.4/src/allocine_seances.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-15 18:36:10.000000 allocine-seances-0.0.4/src/allocine_seances.egg-info/top_level.txt
```

### Comparing `allocine-seances-0.0.3/LICENSE` & `allocine-seances-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `allocine-seances-0.0.3/PKG-INFO` & `allocine-seances-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allocine-seances
-Version: 0.0.3
+Version: 0.0.4
 Summary: Récupération des scéances de cinémas sur allociné
 Author-email: lefevre-dev <louislefevre.dev@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,15 +41,15 @@
 La méthode ```get_cinema(id_location)``` retourne un id de cinéma pour un emplacement donné.
 
 La méthode ```get_showtime(id_cinema, day_shift)``` retourne la liste des séances pour un cinema donné et un jour. le paramètre day_shift (entier positif) représente le décalage en jour par rapport à la date actuelle.
 
 # Import
 
 ```python
-from allocineAPI import allocineAPI
+from allocineAPI.allocineAPI import allocineAPI
 
 api = allocineAPI()
 ```
 # Liste des méthodes
 ## Listes des villes
 ```python
 ret = api.get_top_villes()
```

### Comparing `allocine-seances-0.0.3/README.md` & `allocine-seances-0.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 La méthode ```get_cinema(id_location)``` retourne un id de cinéma pour un emplacement donné.
 
 La méthode ```get_showtime(id_cinema, day_shift)``` retourne la liste des séances pour un cinema donné et un jour. le paramètre day_shift (entier positif) représente le décalage en jour par rapport à la date actuelle.
 
 # Import
 
 ```python
-from allocineAPI import allocineAPI
+from allocineAPI.allocineAPI import allocineAPI
 
 api = allocineAPI()
 ```
 # Liste des méthodes
 ## Listes des villes
 ```python
 ret = api.get_top_villes()
```

### Comparing `allocine-seances-0.0.3/pyproject.toml` & `allocine-seances-0.0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "allocine-seances"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="lefevre-dev", email="louislefevre.dev@gmail.com" },
 ]
 description = "Récupération des scéances de cinémas sur allociné"
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
```

### Comparing `allocine-seances-0.0.3/src/allocineAPI/allocineAPI.py` & `allocine-seances-0.0.4/src/allocineAPI/allocineAPI.py`

 * *Files identical despite different names*

### Comparing `allocine-seances-0.0.3/src/allocine_seances.egg-info/PKG-INFO` & `allocine-seances-0.0.4/src/allocine_seances.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allocine-seances
-Version: 0.0.3
+Version: 0.0.4
 Summary: Récupération des scéances de cinémas sur allociné
 Author-email: lefevre-dev <louislefevre.dev@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,15 +41,15 @@
 La méthode ```get_cinema(id_location)``` retourne un id de cinéma pour un emplacement donné.
 
 La méthode ```get_showtime(id_cinema, day_shift)``` retourne la liste des séances pour un cinema donné et un jour. le paramètre day_shift (entier positif) représente le décalage en jour par rapport à la date actuelle.
 
 # Import
 
 ```python
-from allocineAPI import allocineAPI
+from allocineAPI.allocineAPI import allocineAPI
 
 api = allocineAPI()
 ```
 # Liste des méthodes
 ## Listes des villes
 ```python
 ret = api.get_top_villes()
```

