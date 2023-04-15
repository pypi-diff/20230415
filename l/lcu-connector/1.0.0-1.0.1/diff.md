# Comparing `tmp/lcu-connector-1.0.0.tar.gz` & `tmp/lcu-connector-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcu-connector-1.0.0.tar", last modified: Sat Apr 15 04:39:34 2023, max compression
+gzip compressed data, was "lcu-connector-1.0.1.tar", last modified: Sat Apr 15 05:24:21 2023, max compression
```

## Comparing `lcu-connector-1.0.0.tar` & `lcu-connector-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 04:39:34.388344 lcu-connector-1.0.0/
--rw-rw-rw-   0        0        0     1091 2023-04-15 04:30:40.000000 lcu-connector-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2661 2023-04-15 04:39:34.388344 lcu-connector-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1976 2023-04-15 04:30:40.000000 lcu-connector-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 04:39:34.383393 lcu-connector-1.0.0/lcu_connector/
--rw-rw-rw-   0        0        0       34 2023-04-15 04:30:40.000000 lcu-connector-1.0.0/lcu_connector/__init__.py
--rw-rw-rw-   0        0        0     4121 2023-04-15 04:30:40.000000 lcu-connector-1.0.0/lcu_connector/connection.py
--rw-rw-rw-   0        0        0     3938 2023-04-15 04:30:40.000000 lcu-connector-1.0.0/lcu_connector/connector.py
--rw-rw-rw-   0        0        0      830 2023-04-15 04:30:40.000000 lcu-connector-1.0.0/lcu_connector/exceptions.py
--rw-rw-rw-   0        0        0     4546 2023-04-15 04:30:40.000000 lcu-connector-1.0.0/lcu_connector/riot.py
-drwxrwxrwx   0        0        0        0 2023-04-15 04:39:34.387338 lcu-connector-1.0.0/lcu_connector.egg-info/
--rw-rw-rw-   0        0        0     2661 2023-04-15 04:39:34.000000 lcu-connector-1.0.0/lcu_connector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-04-15 04:39:34.000000 lcu-connector-1.0.0/lcu_connector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 04:39:34.000000 lcu-connector-1.0.0/lcu_connector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-15 04:39:34.000000 lcu-connector-1.0.0/lcu_connector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-15 04:39:34.000000 lcu-connector-1.0.0/lcu_connector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1145 2023-04-15 04:30:40.000000 lcu-connector-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-15 04:39:34.388344 lcu-connector-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1063 2023-04-15 04:39:06.000000 lcu-connector-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 05:24:21.563248 lcu-connector-1.0.1/
+-rw-rw-rw-   0        0        0     1091 2023-04-15 04:30:40.000000 lcu-connector-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2821 2023-04-15 05:24:21.562269 lcu-connector-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1976 2023-04-15 04:30:40.000000 lcu-connector-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 05:24:21.559307 lcu-connector-1.0.1/lcu_connector/
+-rw-rw-rw-   0        0        0       34 2023-04-15 04:30:40.000000 lcu-connector-1.0.1/lcu_connector/__init__.py
+-rw-rw-rw-   0        0        0     4121 2023-04-15 04:30:40.000000 lcu-connector-1.0.1/lcu_connector/connection.py
+-rw-rw-rw-   0        0        0     3938 2023-04-15 05:06:52.000000 lcu-connector-1.0.1/lcu_connector/connector.py
+-rw-rw-rw-   0        0        0      830 2023-04-15 04:30:40.000000 lcu-connector-1.0.1/lcu_connector/exceptions.py
+-rw-rw-rw-   0        0        0     4544 2023-04-15 05:19:53.000000 lcu-connector-1.0.1/lcu_connector/riot.py
+drwxrwxrwx   0        0        0        0 2023-04-15 05:24:21.562269 lcu-connector-1.0.1/lcu_connector.egg-info/
+-rw-rw-rw-   0        0        0     2821 2023-04-15 05:24:21.000000 lcu-connector-1.0.1/lcu_connector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-04-15 05:24:21.000000 lcu-connector-1.0.1/lcu_connector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       45 2023-04-15 05:24:21.000000 lcu-connector-1.0.1/lcu_connector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-15 05:24:21.000000 lcu-connector-1.0.1/lcu_connector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-15 05:24:21.000000 lcu-connector-1.0.1/lcu_connector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1145 2023-04-15 04:30:40.000000 lcu-connector-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-15 05:24:21.563248 lcu-connector-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1341 2023-04-15 05:20:56.000000 lcu-connector-1.0.1/setup.py
```

### Comparing `lcu-connector-1.0.0/LICENSE` & `lcu-connector-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lcu-connector-1.0.0/PKG-INFO` & `lcu-connector-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: lcu-connector
-Version: 1.0.0
+Version: 1.0.1
 Summary: Easy-to-use wrapper for the League Client API.
 Author: Gabriel Viana
 Author-email: ssiriusbeck@gmail.com
-License: MIT
-Project-URL: Source, https://github.com/pySiriusDev/LCU-Connector
-Project-URL: Download, https://github.com/pySiriusDev/LCU-Connector/releases
+Project-URL: Source, https://github.com/pySiriusDev/lcu-connector
+Project-URL: Download, https://github.com/pySiriusDev/lcu-connector/releases
 Project-URL: Instagram, https://instagram.com/biellviana
 Project-URL: Twitter, https://twitter.com/_siriusbeck
 Keywords: league client,league client api,league client api wrapper,api wrapperleague of legends,league of legends api,lcu-driver,lcu driver,lcu-connector,lcu connector
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # LCU Connector
 
 This library serves to make the connection with the League Client API in a simple way, although there are others, such as [lcu-driver](https://github.com/sousa-andre/lcu-driver) (which by the way is very good), but with lcu-driver, for example, I couldn't work and structure my code the way I wanted it to, so I decided to make my own wrapper.
```

### Comparing `lcu-connector-1.0.0/README.md` & `lcu-connector-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `lcu-connector-1.0.0/lcu_connector/connection.py` & `lcu-connector-1.0.1/lcu_connector/connection.py`

 * *Files identical despite different names*

### Comparing `lcu-connector-1.0.0/lcu_connector/connector.py` & `lcu-connector-1.0.1/lcu_connector/connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
         Args:
             headers (Dict): The value to set the headers property to.
         """
         self.__headers = headers
 
 
-class Connector(BaseConnector, Connection):
+class Connector(Connection, BaseConnector):
     """Represents a connector for a Riot Games client.
 
     Inherits from:
         BaseConnector
         Connection
 
     Attributes:
```

### Comparing `lcu-connector-1.0.0/lcu_connector/exceptions.py` & `lcu-connector-1.0.1/lcu_connector/exceptions.py`

 * *Files identical despite different names*

### Comparing `lcu-connector-1.0.0/lcu_connector/riot.py` & `lcu-connector-1.0.1/lcu_connector/riot.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
 
 class RiotSSL:
     def __init__(self) -> None:
         """Initialize an instance of the class with a Path object pointing to the './riotgames.pem' file
         and calls the private method '__update_path()'. This method is typically called when a new instance of the class is created.
         """
-        self.__file = Path('./riotgames.pem')
+        self.__file = Path('riotgames.pem')
         self.__update_path()
 
     def __update_path(self) -> None:
         """Update the file path, if the file does not exist, the method retrieves the file from the specified URL
         and writes it to the file path.
         """
         if not self.__file.exists():
```

### Comparing `lcu-connector-1.0.0/lcu_connector.egg-info/PKG-INFO` & `lcu-connector-1.0.1/lcu_connector.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: lcu-connector
-Version: 1.0.0
+Version: 1.0.1
 Summary: Easy-to-use wrapper for the League Client API.
 Author: Gabriel Viana
 Author-email: ssiriusbeck@gmail.com
-License: MIT
-Project-URL: Source, https://github.com/pySiriusDev/LCU-Connector
-Project-URL: Download, https://github.com/pySiriusDev/LCU-Connector/releases
+Project-URL: Source, https://github.com/pySiriusDev/lcu-connector
+Project-URL: Download, https://github.com/pySiriusDev/lcu-connector/releases
 Project-URL: Instagram, https://instagram.com/biellviana
 Project-URL: Twitter, https://twitter.com/_siriusbeck
 Keywords: league client,league client api,league client api wrapper,api wrapperleague of legends,league of legends api,lcu-driver,lcu driver,lcu-connector,lcu connector
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # LCU Connector
 
 This library serves to make the connection with the League Client API in a simple way, although there are others, such as [lcu-driver](https://github.com/sousa-andre/lcu-driver) (which by the way is very good), but with lcu-driver, for example, I couldn't work and structure my code the way I wanted it to, so I decided to make my own wrapper.
```

### Comparing `lcu-connector-1.0.0/pyproject.toml` & `lcu-connector-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lcu-connector-1.0.0/setup.py` & `lcu-connector-1.0.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,45 @@
 from setuptools import setup
 
 
-with open('README.md') as file:
-    readme = file.read()
-
+with open("README.md", "r") as fh:
+    readme = fh.read()
 
 setup(
-    name='lcu-connector',
-    version='1.0.0',
-    author='Gabriel Viana',
+    name="lcu-connector",
+    version="1.0.1",
+    author="Gabriel Viana",
     author_email='ssiriusbeck@gmail.com',
-    description='Easy-to-use wrapper for the League Client API.',
+    description="Easy-to-use wrapper for the League Client API.",
     long_description=readme,
-    long_description_content_type='text/markdown',
-    packages=['lcu_connector'],
-    install_requires=['requests', 'psutil'],
+    long_description_content_type="text/markdown",
+    packages=["lcu_connector"],
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    python_requires='>=3.11',
+    install_requires=[
+        'requests',
+        'psutil'
+    ],
+    dependency_links=['https://github.com/pySiriusDev/lcu-connector'],
+    project_urls={
+        'Source': 'https://github.com/pySiriusDev/lcu-connector',
+        'Download': 'https://github.com/pySiriusDev/lcu-connector/releases',
+        'Instagram': 'https://instagram.com/biellviana',
+        'Twitter': 'https://twitter.com/_siriusbeck'
+    },
     keywords=[
         'league client',
         'league client api',
         'league client api wrapper',
         'api wrapper'
         'league of legends',
         'league of legends api',
         'lcu-driver',
         'lcu driver',
         'lcu-connector',
         'lcu connector'
-    ],
-    license='MIT',
-    project_urls={
-        'Source': 'https://github.com/pySiriusDev/LCU-Connector',
-        'Download': 'https://github.com/pySiriusDev/LCU-Connector/releases',
-        'Instagram': 'https://instagram.com/biellviana',
-        'Twitter': 'https://twitter.com/_siriusbeck'
-    }
-)
+    ]
+)
```

