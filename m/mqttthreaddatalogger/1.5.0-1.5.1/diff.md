# Comparing `tmp/mqttthreaddatalogger-1.5.0.tar.gz` & `tmp/mqttthreaddatalogger-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqttthreaddatalogger-1.5.0.tar", last modified: Sat Apr 15 19:24:03 2023, max compression
+gzip compressed data, was "mqttthreaddatalogger-1.5.1.tar", last modified: Sat Apr 15 19:31:37 2023, max compression
```

## Comparing `mqttthreaddatalogger-1.5.0.tar` & `mqttthreaddatalogger-1.5.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 19:24:03.981209 mqttthreaddatalogger-1.5.0/
--rw-rw-rw-   0        0        0     1094 2021-02-10 19:27:17.000000 mqttthreaddatalogger-1.5.0/LICENCE
--rw-rw-rw-   0        0        0     1986 2023-04-15 19:24:03.981209 mqttthreaddatalogger-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1539 2022-04-11 19:22:58.000000 mqttthreaddatalogger-1.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 19:24:03.970912 mqttthreaddatalogger-1.5.0/mqttthreaddatalogger/
--rw-rw-rw-   0        0        0       78 2021-05-20 20:55:44.000000 mqttthreaddatalogger-1.5.0/mqttthreaddatalogger/__init__.py
--rw-rw-rw-   0        0        0     5114 2023-04-15 19:19:25.000000 mqttthreaddatalogger-1.5.0/mqttthreaddatalogger/mqttthreaddatalogger.py
-drwxrwxrwx   0        0        0        0 2023-04-15 19:24:03.981209 mqttthreaddatalogger-1.5.0/mqttthreaddatalogger.egg-info/
--rw-rw-rw-   0        0        0     1986 2023-04-15 19:24:03.000000 mqttthreaddatalogger-1.5.0/mqttthreaddatalogger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-04-15 19:24:03.000000 mqttthreaddatalogger-1.5.0/mqttthreaddatalogger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 19:24:03.000000 mqttthreaddatalogger-1.5.0/mqttthreaddatalogger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-15 19:24:03.000000 mqttthreaddatalogger-1.5.0/mqttthreaddatalogger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-15 19:24:03.000000 mqttthreaddatalogger-1.5.0/mqttthreaddatalogger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 19:24:03.981209 mqttthreaddatalogger-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-04-15 19:23:19.000000 mqttthreaddatalogger-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 19:31:37.662910 mqttthreaddatalogger-1.5.1/
+-rw-rw-rw-   0        0        0     1094 2021-02-10 19:27:17.000000 mqttthreaddatalogger-1.5.1/LICENCE
+-rw-rw-rw-   0        0        0     1986 2023-04-15 19:31:37.662910 mqttthreaddatalogger-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1539 2022-04-11 19:22:58.000000 mqttthreaddatalogger-1.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 19:31:37.640877 mqttthreaddatalogger-1.5.1/mqttthreaddatalogger/
+-rw-rw-rw-   0        0        0       78 2021-05-20 20:55:44.000000 mqttthreaddatalogger-1.5.1/mqttthreaddatalogger/__init__.py
+-rw-rw-rw-   0        0        0     5150 2023-04-15 19:30:12.000000 mqttthreaddatalogger-1.5.1/mqttthreaddatalogger/mqttthreaddatalogger.py
+drwxrwxrwx   0        0        0        0 2023-04-15 19:31:37.662910 mqttthreaddatalogger-1.5.1/mqttthreaddatalogger.egg-info/
+-rw-rw-rw-   0        0        0     1986 2023-04-15 19:31:37.000000 mqttthreaddatalogger-1.5.1/mqttthreaddatalogger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-04-15 19:31:37.000000 mqttthreaddatalogger-1.5.1/mqttthreaddatalogger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 19:31:37.000000 mqttthreaddatalogger-1.5.1/mqttthreaddatalogger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-15 19:31:37.000000 mqttthreaddatalogger-1.5.1/mqttthreaddatalogger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-15 19:31:37.000000 mqttthreaddatalogger-1.5.1/mqttthreaddatalogger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 19:31:37.662910 mqttthreaddatalogger-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-04-15 19:31:01.000000 mqttthreaddatalogger-1.5.1/setup.py
```

### Comparing `mqttthreaddatalogger-1.5.0/LICENCE` & `mqttthreaddatalogger-1.5.1/LICENCE`

 * *Files identical despite different names*

### Comparing `mqttthreaddatalogger-1.5.0/PKG-INFO` & `mqttthreaddatalogger-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqttthreaddatalogger
-Version: 1.5.0
+Version: 1.5.1
 Summary: Connexion mqtt et enregistrement des données dans un fichier csv
 Author: Didier Orlandi
 Author-email: didier.orlandi@wanadoo.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
```

### Comparing `mqttthreaddatalogger-1.5.0/README.md` & `mqttthreaddatalogger-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `mqttthreaddatalogger-1.5.0/mqttthreaddatalogger/mqttthreaddatalogger.py` & `mqttthreaddatalogger-1.5.1/mqttthreaddatalogger/mqttthreaddatalogger.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,16 @@
     def on_message(self, client, userdata, msg):
         data = msg.payload.decode("utf-8").strip('\r\n') # decode et enlève les \r \n
         #print("message reçu")
         tab = []
         try:
             y = json.loads(data)
             for i in range(0,len(self.Key)):
-                txt = self.Key[i].split("#")# split pour le nom des champs
+                #txt = self.Key[i].split("#")# split pour le nom des champs
+                txt = self.Key[i]
                 value = y[txt]
                 #value = eval('y'+txt[0])# la valeur string est évaluée
                 try: 
                     value = float(value)# essaye de convertir en float
                 except:
                     pass  # rien à faire
                 tab.append(value)
```

### Comparing `mqttthreaddatalogger-1.5.0/mqttthreaddatalogger.egg-info/PKG-INFO` & `mqttthreaddatalogger-1.5.1/mqttthreaddatalogger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqttthreaddatalogger
-Version: 1.5.0
+Version: 1.5.1
 Summary: Connexion mqtt et enregistrement des données dans un fichier csv
 Author: Didier Orlandi
 Author-email: didier.orlandi@wanadoo.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
```

### Comparing `mqttthreaddatalogger-1.5.0/setup.py` & `mqttthreaddatalogger-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mqttthreaddatalogger", # Replace with your own username
-    version="1.5.0",
+    version="1.5.1",
     author="Didier Orlandi",
     author_email="didier.orlandi@wanadoo.fr",
     description="Connexion mqtt et enregistrement des données dans un fichier csv",
     long_description=long_description,
     long_description_content_type="text/markdown",
     #url="https://github.com/",
     packages=setuptools.find_packages(),
```

