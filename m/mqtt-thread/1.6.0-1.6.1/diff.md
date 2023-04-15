# Comparing `tmp/mqtt_thread-1.6.0.tar.gz` & `tmp/mqtt_thread-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqtt_thread-1.6.0.tar", last modified: Sat Feb 25 23:17:19 2023, max compression
+gzip compressed data, was "mqtt_thread-1.6.1.tar", last modified: Sat Apr 15 21:08:01 2023, max compression
```

## Comparing `mqtt_thread-1.6.0.tar` & `mqtt_thread-1.6.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-02-25 23:17:19.148523 mqtt_thread-1.6.0/
--rw-rw-rw-   0        0        0     1088 2021-02-01 10:36:06.000000 mqtt_thread-1.6.0/LICENCE
--rw-rw-rw-   0        0        0     3720 2023-02-25 23:17:19.148523 mqtt_thread-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     3320 2023-02-25 23:15:51.000000 mqtt_thread-1.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-02-25 23:17:19.132561 mqtt_thread-1.6.0/mqtt_thread/
--rw-rw-rw-   0        0        0     6878 2023-02-25 23:05:38.000000 mqtt_thread-1.6.0/mqtt_thread/MQTT_Thread.py
--rw-rw-rw-   0        0        0     5772 2023-02-22 15:29:07.000000 mqtt_thread-1.6.0/mqtt_thread/MQTT_Thread_bak.py
--rw-rw-rw-   0        0        0       51 2021-02-01 20:48:52.000000 mqtt_thread-1.6.0/mqtt_thread/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-25 23:17:19.148523 mqtt_thread-1.6.0/mqtt_thread.egg-info/
--rw-rw-rw-   0        0        0     3720 2023-02-25 23:17:19.000000 mqtt_thread-1.6.0/mqtt_thread.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-02-25 23:17:19.000000 mqtt_thread-1.6.0/mqtt_thread.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-25 23:17:19.000000 mqtt_thread-1.6.0/mqtt_thread.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-02-25 23:17:19.000000 mqtt_thread-1.6.0/mqtt_thread.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-02-25 23:17:19.000000 mqtt_thread-1.6.0/mqtt_thread.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-25 23:17:19.148523 mqtt_thread-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0      764 2023-02-25 22:56:53.000000 mqtt_thread-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 21:08:01.403636 mqtt_thread-1.6.1/
+-rw-rw-rw-   0        0        0     1088 2021-02-01 10:36:06.000000 mqtt_thread-1.6.1/LICENCE
+-rw-rw-rw-   0        0        0     3720 2023-04-15 21:08:01.391015 mqtt_thread-1.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3320 2023-02-25 23:15:51.000000 mqtt_thread-1.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 21:08:01.379370 mqtt_thread-1.6.1/mqtt_thread/
+-rw-rw-rw-   0        0        0     7041 2023-04-15 21:06:43.000000 mqtt_thread-1.6.1/mqtt_thread/MQTT_Thread.py
+-rw-rw-rw-   0        0        0     5772 2023-02-22 15:29:07.000000 mqtt_thread-1.6.1/mqtt_thread/MQTT_Thread_bak.py
+-rw-rw-rw-   0        0        0       51 2021-02-01 20:48:52.000000 mqtt_thread-1.6.1/mqtt_thread/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 21:08:01.391015 mqtt_thread-1.6.1/mqtt_thread.egg-info/
+-rw-rw-rw-   0        0        0     3720 2023-04-15 21:08:01.000000 mqtt_thread-1.6.1/mqtt_thread.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-04-15 21:08:01.000000 mqtt_thread-1.6.1/mqtt_thread.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 21:08:01.000000 mqtt_thread-1.6.1/mqtt_thread.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-15 21:08:01.000000 mqtt_thread-1.6.1/mqtt_thread.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-15 21:08:01.000000 mqtt_thread-1.6.1/mqtt_thread.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 21:08:01.403636 mqtt_thread-1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      764 2023-04-15 21:07:15.000000 mqtt_thread-1.6.1/setup.py
```

### Comparing `mqtt_thread-1.6.0/LICENCE` & `mqtt_thread-1.6.1/LICENCE`

 * *Files identical despite different names*

### Comparing `mqtt_thread-1.6.0/PKG-INFO` & `mqtt_thread-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqtt_thread
-Version: 1.6.0
+Version: 1.6.1
 Summary: Connection MQTT with thread
 Author: Didier Orlandi
 Author-email: didier.orlandi@wanadoo.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `mqtt_thread-1.6.0/README.md` & `mqtt_thread-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `mqtt_thread-1.6.0/mqtt_thread/MQTT_Thread.py` & `mqtt_thread-1.6.1/mqtt_thread/MQTT_Thread.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,18 @@
                 if tab != []:
                     tab.append(self.temps)
                     date = [datetime.datetime.now().strftime("%d/%m/%y %H:%M:%S")]
                     tab1 = date + tab
                     self.lastLinedata = tab1
                     if self.record:
                         #print(tab)
-                        enregistreFichier(self.nomFichier+str(i)+"csv",self.lastLinedata)
+                        if (len(self.Key)==1):
+                            enregistreFichier(self.nomFichier,self.lastLinedata)
+                        else:
+                            enregistreFichier(self.nomFichier+"_"+str(i),self.lastLinedata)
 
         except:
             if self.verbose:
                 print("pas de clé demandée sur -> ",self.msg)
         else:
             if self.verbose:
                 print(self.msg)
```

### Comparing `mqtt_thread-1.6.0/mqtt_thread/MQTT_Thread_bak.py` & `mqtt_thread-1.6.1/mqtt_thread/MQTT_Thread_bak.py`

 * *Files identical despite different names*

### Comparing `mqtt_thread-1.6.0/mqtt_thread.egg-info/PKG-INFO` & `mqtt_thread-1.6.1/mqtt_thread.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqtt-thread
-Version: 1.6.0
+Version: 1.6.1
 Summary: Connection MQTT with thread
 Author: Didier Orlandi
 Author-email: didier.orlandi@wanadoo.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `mqtt_thread-1.6.0/setup.py` & `mqtt_thread-1.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mqtt_thread", # Replace with your own username
-    version="1.6.0",
+    version="1.6.1",
     author="Didier Orlandi",
     author_email="didier.orlandi@wanadoo.fr",
     description="Connection MQTT with thread",
     long_description=long_description,
     long_description_content_type="text/markdown",
     #url="https://github.com/",
     packages=setuptools.find_packages(),
```

