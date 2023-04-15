# Comparing `tmp/extr-0.0.5.tar.gz` & `tmp/extr-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extr-0.0.5.tar", last modified: Thu Apr 13 10:52:41 2023, max compression
+gzip compressed data, was "extr-0.0.6.tar", last modified: Sat Apr 15 10:42:23 2023, max compression
```

## Comparing `extr-0.0.5.tar` & `extr-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 10:52:41.381464 extr-0.0.5/
--rw-rw-rw-   0        0        0     2422 2023-04-13 10:52:41.379529 extr-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1586 2023-04-11 09:38:34.000000 extr-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 10:52:41.393430 extr-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      477 2023-04-13 10:52:34.000000 extr-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 10:52:41.242315 extr-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 10:52:41.300324 extr-0.0.5/src/extr/
--rw-rw-rw-   0        0        0      236 2023-04-12 10:21:01.000000 extr-0.0.5/src/extr/__init__.py
--rw-rw-rw-   0        0        0     1692 2023-04-13 10:18:22.000000 extr-0.0.5/src/extr/entities.py
--rw-rw-rw-   0        0        0      166 2023-04-12 10:31:30.000000 extr-0.0.5/src/extr/iterutils.py
--rw-rw-rw-   0        0        0     2261 2023-04-13 10:52:02.000000 extr-0.0.5/src/extr/models.py
--rw-rw-rw-   0        0        0     2510 2023-04-10 13:19:22.000000 extr-0.0.5/src/extr/regex.py
--rw-rw-rw-   0        0        0     1194 2023-04-12 10:32:54.000000 extr-0.0.5/src/extr/relations.py
-drwxrwxrwx   0        0        0        0 2023-04-13 10:52:41.371134 extr-0.0.5/src/extr.egg-info/
--rw-rw-rw-   0        0        0     2422 2023-04-13 10:52:40.000000 extr-0.0.5/src/extr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-04-13 10:52:41.000000 extr-0.0.5/src/extr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 10:52:40.000000 extr-0.0.5/src/extr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-13 10:52:41.000000 extr-0.0.5/src/extr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 10:42:23.587868 extr-0.0.6/
+-rw-rw-rw-   0        0        0     2431 2023-04-15 10:42:23.584838 extr-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1580 2023-04-15 09:22:47.000000 extr-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-15 10:42:23.593986 extr-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      538 2023-04-15 10:41:45.000000 extr-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 10:42:23.174237 extr-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 10:42:23.363259 extr-0.0.6/src/extr/
+-rw-rw-rw-   0        0        0      247 2023-04-13 10:55:50.000000 extr-0.0.6/src/extr/__init__.py
+-rw-rw-rw-   0        0        0     1692 2023-04-13 10:18:22.000000 extr-0.0.6/src/extr/entities.py
+-rw-rw-rw-   0        0        0      166 2023-04-12 10:31:30.000000 extr-0.0.6/src/extr/iterutils.py
+-rw-rw-rw-   0        0        0     2261 2023-04-13 10:55:57.000000 extr-0.0.6/src/extr/models.py
+-rw-rw-rw-   0        0        0     2510 2023-04-10 13:19:22.000000 extr-0.0.6/src/extr/regex.py
+-rw-rw-rw-   0        0        0     1194 2023-04-12 10:32:54.000000 extr-0.0.6/src/extr/relations.py
+drwxrwxrwx   0        0        0        0 2023-04-15 10:42:23.579008 extr-0.0.6/src/extr.egg-info/
+-rw-rw-rw-   0        0        0     2431 2023-04-15 10:42:22.000000 extr-0.0.6/src/extr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-04-15 10:42:23.000000 extr-0.0.6/src/extr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 10:42:22.000000 extr-0.0.6/src/extr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-15 10:42:22.000000 extr-0.0.6/src/extr.egg-info/top_level.txt
```

### Comparing `extr-0.0.5/PKG-INFO` & `extr-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: extr
-Version: 0.0.5
+Version: 0.0.6
 Summary: Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
-Home-page: UNKNOWN
+Home-page: https://github.com/dpasse/extr
 License: UNKNOWN
-Description: # Extr - NLP
-        
+Description: # Extr
         > Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
         
         <br />
         
         ## Install
         
         ```
@@ -22,17 +21,17 @@
         text = 'Ted is a Pitcher.'
         ```
         
         ### 1. Entity Extraction
         > Find Named Entities from text.
         
         ```python
-        from extr import RegEx, RegExLabel, EntityExtactor
+        from extr import RegEx, RegExLabel, EntityExtractor
         
-        entity_extractor = EntityExtactor([
+        entity_extractor = EntityExtractor([
             RegExLabel('PERSON', [
                 RegEx([r'ted'], re.IGNORECASE)
             ]),
             RegExLabel('POSITION', [
                 RegEx([r'pitcher'], re.IGNORECASE)
             ]),
         ])
```

### Comparing `extr-0.0.5/README.md` & `extr-0.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# Extr - NLP
-
+# Extr
 > Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
 
 <br />
 
 ## Install
 
 ```
@@ -16,17 +15,17 @@
 text = 'Ted is a Pitcher.'
 ```
 
 ### 1. Entity Extraction
 > Find Named Entities from text.
 
 ```python
-from extr import RegEx, RegExLabel, EntityExtactor
+from extr import RegEx, RegExLabel, EntityExtractor
 
-entity_extractor = EntityExtactor([
+entity_extractor = EntityExtractor([
     RegExLabel('PERSON', [
         RegEx([r'ted'], re.IGNORECASE)
     ]),
     RegExLabel('POSITION', [
         RegEx([r'pitcher'], re.IGNORECASE)
     ]),
 ])
```

### Comparing `extr-0.0.5/src/extr/entities.py` & `extr-0.0.6/src/extr/entities.py`

 * *Files identical despite different names*

### Comparing `extr-0.0.5/src/extr/models.py` & `extr-0.0.6/src/extr/models.py`

 * *Files identical despite different names*

### Comparing `extr-0.0.5/src/extr/regex.py` & `extr-0.0.6/src/extr/regex.py`

 * *Files identical despite different names*

### Comparing `extr-0.0.5/src/extr/relations.py` & `extr-0.0.6/src/extr/relations.py`

 * *Files identical despite different names*

### Comparing `extr-0.0.5/src/extr.egg-info/PKG-INFO` & `extr-0.0.6/src/extr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: extr
-Version: 0.0.5
+Version: 0.0.6
 Summary: Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
-Home-page: UNKNOWN
+Home-page: https://github.com/dpasse/extr
 License: UNKNOWN
-Description: # Extr - NLP
-        
+Description: # Extr
         > Named Entity Recognition (NER) and Relation Extraction (RE) library using Regular Expressions
         
         <br />
         
         ## Install
         
         ```
@@ -22,17 +21,17 @@
         text = 'Ted is a Pitcher.'
         ```
         
         ### 1. Entity Extraction
         > Find Named Entities from text.
         
         ```python
-        from extr import RegEx, RegExLabel, EntityExtactor
+        from extr import RegEx, RegExLabel, EntityExtractor
         
-        entity_extractor = EntityExtactor([
+        entity_extractor = EntityExtractor([
             RegExLabel('PERSON', [
                 RegEx([r'ted'], re.IGNORECASE)
             ]),
             RegExLabel('POSITION', [
                 RegEx([r'pitcher'], re.IGNORECASE)
             ]),
         ])
```

