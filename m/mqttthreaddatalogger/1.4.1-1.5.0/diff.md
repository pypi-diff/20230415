# Comparing `tmp/mqttthreaddatalogger-1.4.1.tar.gz` & `tmp/mqttthreaddatalogger-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\OneDrive\Documents\Python\Pypi projets\mqttthreaddatalogger\dist\tmpljflbdzu\mqttthreaddatalogger-1.4.1.tar", last modified: Mon Apr 11 19:24:01 2022, max compression
+gzip compressed data, was "mqttthreaddatalogger-1.5.0.tar", last modified: Sat Apr 15 19:24:03 2023, max compression
```

## Comparing `mqttthreaddatalogger-1.4.1.tar` & `mqttthreaddatalogger-1.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-04-11 19:24:01.467858 mqttthreaddatalogger-1.4.1/
--rw-rw-rw-   0        0        0     1094 2021-02-10 19:27:17.000000 mqttthreaddatalogger-1.4.1/LICENCE
--rw-rw-rw-   0        0        0     2027 2022-04-11 19:24:01.466858 mqttthreaddatalogger-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     1539 2022-04-11 19:22:58.000000 mqttthreaddatalogger-1.4.1/README.md
-drwxrwxrwx   0        0        0        0 2022-04-11 19:24:01.403894 mqttthreaddatalogger-1.4.1/mqttthreaddatalogger/
--rw-rw-rw-   0        0        0       78 2021-05-20 20:55:44.000000 mqttthreaddatalogger-1.4.1/mqttthreaddatalogger/__init__.py
--rw-rw-rw-   0        0        0     5082 2022-04-11 19:16:33.000000 mqttthreaddatalogger-1.4.1/mqttthreaddatalogger/mqttthreaddatalogger.py
-drwxrwxrwx   0        0        0        0 2022-04-11 19:24:01.463860 mqttthreaddatalogger-1.4.1/mqttthreaddatalogger.egg-info/
--rw-rw-rw-   0        0        0     2027 2022-04-11 19:24:00.000000 mqttthreaddatalogger-1.4.1/mqttthreaddatalogger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2022-04-11 19:24:00.000000 mqttthreaddatalogger-1.4.1/mqttthreaddatalogger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-11 19:24:00.000000 mqttthreaddatalogger-1.4.1/mqttthreaddatalogger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2022-04-11 19:24:00.000000 mqttthreaddatalogger-1.4.1/mqttthreaddatalogger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2022-04-11 19:24:00.000000 mqttthreaddatalogger-1.4.1/mqttthreaddatalogger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-04-11 19:24:01.467858 mqttthreaddatalogger-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0      811 2022-04-11 19:17:25.000000 mqttthreaddatalogger-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 19:24:03.981209 mqttthreaddatalogger-1.5.0/
+-rw-rw-rw-   0        0        0     1094 2021-02-10 19:27:17.000000 mqttthreaddatalogger-1.5.0/LICENCE
+-rw-rw-rw-   0        0        0     1986 2023-04-15 19:24:03.981209 mqttthreaddatalogger-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1539 2022-04-11 19:22:58.000000 mqttthreaddatalogger-1.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 19:24:03.970912 mqttthreaddatalogger-1.5.0/mqttthreaddatalogger/
+-rw-rw-rw-   0        0        0       78 2021-05-20 20:55:44.000000 mqttthreaddatalogger-1.5.0/mqttthreaddatalogger/__init__.py
+-rw-rw-rw-   0        0        0     5114 2023-04-15 19:19:25.000000 mqttthreaddatalogger-1.5.0/mqttthreaddatalogger/mqttthreaddatalogger.py
+drwxrwxrwx   0        0        0        0 2023-04-15 19:24:03.981209 mqttthreaddatalogger-1.5.0/mqttthreaddatalogger.egg-info/
+-rw-rw-rw-   0        0        0     1986 2023-04-15 19:24:03.000000 mqttthreaddatalogger-1.5.0/mqttthreaddatalogger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-04-15 19:24:03.000000 mqttthreaddatalogger-1.5.0/mqttthreaddatalogger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 19:24:03.000000 mqttthreaddatalogger-1.5.0/mqttthreaddatalogger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-15 19:24:03.000000 mqttthreaddatalogger-1.5.0/mqttthreaddatalogger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-15 19:24:03.000000 mqttthreaddatalogger-1.5.0/mqttthreaddatalogger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 19:24:03.981209 mqttthreaddatalogger-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-04-15 19:23:19.000000 mqttthreaddatalogger-1.5.0/setup.py
```

### Comparing `mqttthreaddatalogger-1.4.1/LICENCE` & `mqttthreaddatalogger-1.5.0/LICENCE`

 * *Files identical despite different names*

### Comparing `mqttthreaddatalogger-1.4.1/PKG-INFO` & `mqttthreaddatalogger-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: mqttthreaddatalogger
-Version: 1.4.1
+Version: 1.5.0
 Summary: Connexion mqtt et enregistrement des données dans un fichier csv
 Author: Didier Orlandi
 Author-email: didier.orlandi@wanadoo.fr
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
@@ -48,9 +46,7 @@
 time.sleep(1)<br />
 #publication d'un message vers MQTT  <br />
 #m.client.publish("votretopic/test/in/",payload="{\"pression\":1024}",qos=0)<br />
 <br />
 
 
 
-
-
```

### Comparing `mqttthreaddatalogger-1.4.1/README.md` & `mqttthreaddatalogger-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `mqttthreaddatalogger-1.4.1/mqttthreaddatalogger/mqttthreaddatalogger.py` & `mqttthreaddatalogger-1.5.0/mqttthreaddatalogger/mqttthreaddatalogger.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,16 +91,17 @@
     def on_message(self, client, userdata, msg):
         data = msg.payload.decode("utf-8").strip('\r\n') # decode et enlève les \r \n
         #print("message reçu")
         tab = []
         try:
             y = json.loads(data)
             for i in range(0,len(self.Key)):
-                txt = self.Key[i].split("#")# split pour le nom des champs 
-                value = eval('y'+txt[0])# la valeur string est évaluée
+                txt = self.Key[i].split("#")# split pour le nom des champs
+                value = y[txt]
+                #value = eval('y'+txt[0])# la valeur string est évaluée
                 try: 
                     value = float(value)# essaye de convertir en float
                 except:
                     pass  # rien à faire
                 tab.append(value)
             #print("ma key ", tab)
         except:
```

### Comparing `mqttthreaddatalogger-1.4.1/mqttthreaddatalogger.egg-info/PKG-INFO` & `mqttthreaddatalogger-1.5.0/mqttthreaddatalogger.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: mqttthreaddatalogger
-Version: 1.4.1
+Version: 1.5.0
 Summary: Connexion mqtt et enregistrement des données dans un fichier csv
 Author: Didier Orlandi
 Author-email: didier.orlandi@wanadoo.fr
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
@@ -48,9 +46,7 @@
 time.sleep(1)<br />
 #publication d'un message vers MQTT  <br />
 #m.client.publish("votretopic/test/in/",payload="{\"pression\":1024}",qos=0)<br />
 <br />
 
 
 
-
-
```

### Comparing `mqttthreaddatalogger-1.4.1/setup.py` & `mqttthreaddatalogger-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mqttthreaddatalogger", # Replace with your own username
-    version="1.4.1",
+    version="1.5.0",
     author="Didier Orlandi",
     author_email="didier.orlandi@wanadoo.fr",
     description="Connexion mqtt et enregistrement des données dans un fichier csv",
     long_description=long_description,
     long_description_content_type="text/markdown",
     #url="https://github.com/",
     packages=setuptools.find_packages(),
```

