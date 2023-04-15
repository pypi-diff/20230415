# Comparing `tmp/carter-py-0.1.tar.gz` & `tmp/carter-py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carter-py-0.1.tar", last modified: Sat Apr 15 14:05:24 2023, max compression
+gzip compressed data, was "carter-py-0.1.1.tar", last modified: Sat Apr 15 14:26:25 2023, max compression
```

## Comparing `carter-py-0.1.tar` & `carter-py-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 14:05:24.934877 carter-py-0.1/
--rw-rw-rw-   0        0        0     6622 2023-04-15 14:05:24.933876 carter-py-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5956 2023-04-15 11:16:43.000000 carter-py-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 14:05:24.925868 carter-py-0.1/carter_py.egg-info/
--rw-rw-rw-   0        0        0     6622 2023-04-15 14:05:24.000000 carter-py-0.1/carter_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-04-15 14:05:24.000000 carter-py-0.1/carter_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 14:05:24.000000 carter-py-0.1/carter_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      128 2023-04-15 14:05:24.000000 carter-py-0.1/carter_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-15 14:05:24.000000 carter-py-0.1/carter_py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 14:05:24.931874 carter-py-0.1/carterpy/
--rw-rw-rw-   0        0        0       67 2023-04-15 11:17:48.000000 carter-py-0.1/carterpy/__init__.py
--rw-rw-rw-   0        0        0     2768 2023-04-15 01:28:44.000000 carter-py-0.1/carterpy/async_carter.py
--rw-rw-rw-   0        0        0     2682 2023-04-15 10:31:16.000000 carter-py-0.1/carterpy/carter.py
--rw-rw-rw-   0        0        0     2905 2023-04-15 13:55:27.000000 carter-py-0.1/carterpy/classes.py
--rw-rw-rw-   0        0        0      455 2023-04-12 20:13:09.000000 carter-py-0.1/carterpy/utils.py
--rw-rw-rw-   0        0        0     1075 2023-04-12 19:53:47.000000 carter-py-0.1/license.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 14:05:24.934877 carter-py-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1032 2023-04-15 11:55:49.000000 carter-py-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 14:26:25.374497 carter-py-0.1.1/
+-rw-rw-rw-   0        0        0     6530 2023-04-15 14:26:25.374497 carter-py-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5862 2023-04-15 14:16:25.000000 carter-py-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 14:26:25.367490 carter-py-0.1.1/carter_py.egg-info/
+-rw-rw-rw-   0        0        0     6530 2023-04-15 14:26:25.000000 carter-py-0.1.1/carter_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2023-04-15 14:26:25.000000 carter-py-0.1.1/carter_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 14:26:25.000000 carter-py-0.1.1/carter_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      128 2023-04-15 14:26:25.000000 carter-py-0.1.1/carter_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-15 14:26:25.000000 carter-py-0.1.1/carter_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 14:26:25.372496 carter-py-0.1.1/carterpy/
+-rw-rw-rw-   0        0        0       67 2023-04-15 11:17:48.000000 carter-py-0.1.1/carterpy/__init__.py
+-rw-rw-rw-   0        0        0     2768 2023-04-15 01:28:44.000000 carter-py-0.1.1/carterpy/async_carter.py
+-rw-rw-rw-   0        0        0     2682 2023-04-15 10:31:16.000000 carter-py-0.1.1/carterpy/carter.py
+-rw-rw-rw-   0        0        0     2989 2023-04-15 14:24:34.000000 carter-py-0.1.1/carterpy/classes.py
+-rw-rw-rw-   0        0        0      455 2023-04-12 20:13:09.000000 carter-py-0.1.1/carterpy/utils.py
+-rw-rw-rw-   0        0        0     1075 2023-04-12 19:53:47.000000 carter-py-0.1.1/license.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 14:26:25.374497 carter-py-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1034 2023-04-15 14:15:46.000000 carter-py-0.1.1/setup.py
```

### Comparing `carter-py-0.1/PKG-INFO` & `carter-py-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carter-py
-Version: 0.1
+Version: 0.1.1
 Summary: A wrapper for the Carter API
 Home-page: https://github.com/LazyLyrics/carterpy
 Author: LazyLyrics
 Author-email: lazylyrics@icloud.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -12,37 +12,35 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: license.txt
 
-# `carterpy`: A Python Wrapper for the Carter API
+# carter-py: A Python Wrapper for the Carter API
 
-`carterpy` is a Python package that provides a simple wrapper for the Carter API. It allows you to easily send text messages to the API and receive responses with minimal setup, and with the ability to add more complex functionality in upcoming releases.
+`carter-py` is a Python package that provides a simple wrapper for the Carter API. It allows you to easily send text messages to the API and receive responses with minimal setup, and with the ability to add more complex functionality in upcoming releases.
 
 ## Installation
 
-To install `carterpy`, you can use pip, Python's package manager. Simply run the following command:
-
 ```bash
-pip install `carterpy`
+pip install `carter-py`
 ```
 
-This will install the latest version of `carterpy` and its dependencies.
+This will install the latest version of `carter-py` and its dependencies.
 
-**Note**: `carterpy` has two classes, a Carter class and an AsyncCarter class. The AsyncCarter class is used for asynchronous usage of the API. The Carter class is used for synchronous usage of the API. An example of asynchronous usage can be found below.
+**Note**: `carter-py` has two classes, a Carter class and an AsyncCarter class. The AsyncCarter class is used for asynchronous usage of the API. The Carter class is used for synchronous usage of the API. An example of asynchronous usage can be found below.
 
 ## Usage
 
-To use `carterpy`, you will need to obtain an API key from the Carter website. Once you have your API key, you can use it to create a Carter object and start sending messages. Here's an example:
+To use `carter-py`, you will need to obtain an API key from the Carter website. Once you have your API key, you can use it to create a Carter object and start sending messages. Here's an example:
 
 ```python
 
-from `carterpy` import Carter
+from `carter-py` import Carter
 
 
 # Replace YOUR_API_KEY with your actual API key
 
 carter = Carter("YOUR_API_KEY")
 
 # Send a message to the API
@@ -94,15 +92,15 @@
     time_taken (int): The time taken to receive the response, in milliseconds.
     timestamp (string): The timestamp of the interaction in isoformat.
     ok (bool): Whether the response was successful or not.
     status_code (int): The status code of the response.
     status_message (str): The status message of the response.
 ```
 
-Some properties may be None if the interaction was not successful. Always check the `ok` property before using the other properties, if there was an error with `carterpy` then all data related to output (`output_text, output_audio, forced_behaviours, status_code, status_message`) will be `None`. If there was an error with the API, then the `ok` property will be `False` and the `status_code` and `status_message` properties will be populated with the error information, but output data will still be None.
+Some properties may be None if the interaction was not successful. Always check the `ok` property before using the other properties, if there was an error with `carter-py` then all data related to output (`output_text, output_audio, forced_behaviours, status_code, status_message`) will be `None`. If there was an error with the API, then the `ok` property will be `False` and the `status_code` and `status_message` properties will be populated with the error information, but output data will still be None.
 
 ### History
 
 Each successful interaction with your character is stored in `Carter.history`. This is a list of Interaction objects with the most recent first. You can use this to keep track of the interactions that have taken place.
 
 ```python
 # with carter object already created
@@ -116,24 +114,24 @@
 # Output:
 # How are you?
 # Hello, world!
 ```
 
 ### Upcoming features
 
-- Soon you'll be able to register skills with your agent, this will allow you to trigger functions in your code when `carterpy` detects forced behaviours in the response. This could trigger some other functionality in your code, and even customise the response to add extra data.
+- Soon you'll be able to register skills with your agent, this will allow you to trigger functions in your code when `carter-py` detects forced behaviours in the response. This could trigger some other functionality in your code, and even customise the response to add extra data.
 - Improved logging, including the ability to pass your logger to the `Carter` object for debugging.
 
-### `carterjs`
+### carter-js
 
-`carterpy` is a Python wrapper for the Carter API. If you're looking for a JavaScript wrapper, check out [`carterjs`](https://github.com/LazyLyrics/carter-js)
+`carter-py` is a Python wrapper for the Carter API. If you're looking for a JavaScript wrapper, check out [`carter-js`](https://github.com/LazyLyrics/carter-js)
 
 ### Contributing
 
-If you would like to contribute to `carterpy`, you can do so by opening an issue or pull request on the GitHub repository.
+If you would like to contribute to `carter-py`, you can do so by opening an issue or pull request on the GitHub repository.
 
 ## Asynchronous Usage
 
 ```python
 import asyncio
 from carterpy import AsyncCarter
```

### Comparing `carter-py-0.1/README.md` & `carter-py-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-# `carterpy`: A Python Wrapper for the Carter API
+# carter-py: A Python Wrapper for the Carter API
 
-`carterpy` is a Python package that provides a simple wrapper for the Carter API. It allows you to easily send text messages to the API and receive responses with minimal setup, and with the ability to add more complex functionality in upcoming releases.
+`carter-py` is a Python package that provides a simple wrapper for the Carter API. It allows you to easily send text messages to the API and receive responses with minimal setup, and with the ability to add more complex functionality in upcoming releases.
 
 ## Installation
 
-To install `carterpy`, you can use pip, Python's package manager. Simply run the following command:
-
 ```bash
-pip install `carterpy`
+pip install `carter-py`
 ```
 
-This will install the latest version of `carterpy` and its dependencies.
+This will install the latest version of `carter-py` and its dependencies.
 
-**Note**: `carterpy` has two classes, a Carter class and an AsyncCarter class. The AsyncCarter class is used for asynchronous usage of the API. The Carter class is used for synchronous usage of the API. An example of asynchronous usage can be found below.
+**Note**: `carter-py` has two classes, a Carter class and an AsyncCarter class. The AsyncCarter class is used for asynchronous usage of the API. The Carter class is used for synchronous usage of the API. An example of asynchronous usage can be found below.
 
 ## Usage
 
-To use `carterpy`, you will need to obtain an API key from the Carter website. Once you have your API key, you can use it to create a Carter object and start sending messages. Here's an example:
+To use `carter-py`, you will need to obtain an API key from the Carter website. Once you have your API key, you can use it to create a Carter object and start sending messages. Here's an example:
 
 ```python
 
-from `carterpy` import Carter
+from `carter-py` import Carter
 
 
 # Replace YOUR_API_KEY with your actual API key
 
 carter = Carter("YOUR_API_KEY")
 
 # Send a message to the API
@@ -76,15 +74,15 @@
     time_taken (int): The time taken to receive the response, in milliseconds.
     timestamp (string): The timestamp of the interaction in isoformat.
     ok (bool): Whether the response was successful or not.
     status_code (int): The status code of the response.
     status_message (str): The status message of the response.
 ```
 
-Some properties may be None if the interaction was not successful. Always check the `ok` property before using the other properties, if there was an error with `carterpy` then all data related to output (`output_text, output_audio, forced_behaviours, status_code, status_message`) will be `None`. If there was an error with the API, then the `ok` property will be `False` and the `status_code` and `status_message` properties will be populated with the error information, but output data will still be None.
+Some properties may be None if the interaction was not successful. Always check the `ok` property before using the other properties, if there was an error with `carter-py` then all data related to output (`output_text, output_audio, forced_behaviours, status_code, status_message`) will be `None`. If there was an error with the API, then the `ok` property will be `False` and the `status_code` and `status_message` properties will be populated with the error information, but output data will still be None.
 
 ### History
 
 Each successful interaction with your character is stored in `Carter.history`. This is a list of Interaction objects with the most recent first. You can use this to keep track of the interactions that have taken place.
 
 ```python
 # with carter object already created
@@ -98,24 +96,24 @@
 # Output:
 # How are you?
 # Hello, world!
 ```
 
 ### Upcoming features
 
-- Soon you'll be able to register skills with your agent, this will allow you to trigger functions in your code when `carterpy` detects forced behaviours in the response. This could trigger some other functionality in your code, and even customise the response to add extra data.
+- Soon you'll be able to register skills with your agent, this will allow you to trigger functions in your code when `carter-py` detects forced behaviours in the response. This could trigger some other functionality in your code, and even customise the response to add extra data.
 - Improved logging, including the ability to pass your logger to the `Carter` object for debugging.
 
-### `carterjs`
+### carter-js
 
-`carterpy` is a Python wrapper for the Carter API. If you're looking for a JavaScript wrapper, check out [`carterjs`](https://github.com/LazyLyrics/carter-js)
+`carter-py` is a Python wrapper for the Carter API. If you're looking for a JavaScript wrapper, check out [`carter-js`](https://github.com/LazyLyrics/carter-js)
 
 ### Contributing
 
-If you would like to contribute to `carterpy`, you can do so by opening an issue or pull request on the GitHub repository.
+If you would like to contribute to `carter-py`, you can do so by opening an issue or pull request on the GitHub repository.
 
 ## Asynchronous Usage
 
 ```python
 import asyncio
 from carterpy import AsyncCarter
```

### Comparing `carter-py-0.1/carter_py.egg-info/PKG-INFO` & `carter-py-0.1.1/carter_py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carter-py
-Version: 0.1
+Version: 0.1.1
 Summary: A wrapper for the Carter API
 Home-page: https://github.com/LazyLyrics/carterpy
 Author: LazyLyrics
 Author-email: lazylyrics@icloud.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -12,37 +12,35 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: license.txt
 
-# `carterpy`: A Python Wrapper for the Carter API
+# carter-py: A Python Wrapper for the Carter API
 
-`carterpy` is a Python package that provides a simple wrapper for the Carter API. It allows you to easily send text messages to the API and receive responses with minimal setup, and with the ability to add more complex functionality in upcoming releases.
+`carter-py` is a Python package that provides a simple wrapper for the Carter API. It allows you to easily send text messages to the API and receive responses with minimal setup, and with the ability to add more complex functionality in upcoming releases.
 
 ## Installation
 
-To install `carterpy`, you can use pip, Python's package manager. Simply run the following command:
-
 ```bash
-pip install `carterpy`
+pip install `carter-py`
 ```
 
-This will install the latest version of `carterpy` and its dependencies.
+This will install the latest version of `carter-py` and its dependencies.
 
-**Note**: `carterpy` has two classes, a Carter class and an AsyncCarter class. The AsyncCarter class is used for asynchronous usage of the API. The Carter class is used for synchronous usage of the API. An example of asynchronous usage can be found below.
+**Note**: `carter-py` has two classes, a Carter class and an AsyncCarter class. The AsyncCarter class is used for asynchronous usage of the API. The Carter class is used for synchronous usage of the API. An example of asynchronous usage can be found below.
 
 ## Usage
 
-To use `carterpy`, you will need to obtain an API key from the Carter website. Once you have your API key, you can use it to create a Carter object and start sending messages. Here's an example:
+To use `carter-py`, you will need to obtain an API key from the Carter website. Once you have your API key, you can use it to create a Carter object and start sending messages. Here's an example:
 
 ```python
 
-from `carterpy` import Carter
+from `carter-py` import Carter
 
 
 # Replace YOUR_API_KEY with your actual API key
 
 carter = Carter("YOUR_API_KEY")
 
 # Send a message to the API
@@ -94,15 +92,15 @@
     time_taken (int): The time taken to receive the response, in milliseconds.
     timestamp (string): The timestamp of the interaction in isoformat.
     ok (bool): Whether the response was successful or not.
     status_code (int): The status code of the response.
     status_message (str): The status message of the response.
 ```
 
-Some properties may be None if the interaction was not successful. Always check the `ok` property before using the other properties, if there was an error with `carterpy` then all data related to output (`output_text, output_audio, forced_behaviours, status_code, status_message`) will be `None`. If there was an error with the API, then the `ok` property will be `False` and the `status_code` and `status_message` properties will be populated with the error information, but output data will still be None.
+Some properties may be None if the interaction was not successful. Always check the `ok` property before using the other properties, if there was an error with `carter-py` then all data related to output (`output_text, output_audio, forced_behaviours, status_code, status_message`) will be `None`. If there was an error with the API, then the `ok` property will be `False` and the `status_code` and `status_message` properties will be populated with the error information, but output data will still be None.
 
 ### History
 
 Each successful interaction with your character is stored in `Carter.history`. This is a list of Interaction objects with the most recent first. You can use this to keep track of the interactions that have taken place.
 
 ```python
 # with carter object already created
@@ -116,24 +114,24 @@
 # Output:
 # How are you?
 # Hello, world!
 ```
 
 ### Upcoming features
 
-- Soon you'll be able to register skills with your agent, this will allow you to trigger functions in your code when `carterpy` detects forced behaviours in the response. This could trigger some other functionality in your code, and even customise the response to add extra data.
+- Soon you'll be able to register skills with your agent, this will allow you to trigger functions in your code when `carter-py` detects forced behaviours in the response. This could trigger some other functionality in your code, and even customise the response to add extra data.
 - Improved logging, including the ability to pass your logger to the `Carter` object for debugging.
 
-### `carterjs`
+### carter-js
 
-`carterpy` is a Python wrapper for the Carter API. If you're looking for a JavaScript wrapper, check out [`carterjs`](https://github.com/LazyLyrics/carter-js)
+`carter-py` is a Python wrapper for the Carter API. If you're looking for a JavaScript wrapper, check out [`carter-js`](https://github.com/LazyLyrics/carter-js)
 
 ### Contributing
 
-If you would like to contribute to `carterpy`, you can do so by opening an issue or pull request on the GitHub repository.
+If you would like to contribute to `carter-py`, you can do so by opening an issue or pull request on the GitHub repository.
 
 ## Asynchronous Usage
 
 ```python
 import asyncio
 from carterpy import AsyncCarter
```

### Comparing `carter-py-0.1/carterpy/async_carter.py` & `carter-py-0.1.1/carterpy/async_carter.py`

 * *Files identical despite different names*

### Comparing `carter-py-0.1/carterpy/carter.py` & `carter-py-0.1.1/carterpy/carter.py`

 * *Files identical despite different names*

### Comparing `carter-py-0.1/carterpy/classes.py` & `carter-py-0.1.1/carterpy/classes.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         self.type = type
         self.id = uuid.uuid1()
         self.payload = payload
         self.time_taken = time_taken
         self.timestamp = iso_now()
         self.triggered_skills = []
         self.executed_skills = []
+        self.carter_data = response_data["carter_data"] if response_data is not None else None
 
         # set response params
         if response_data is not None:
             self.ok = response_data["ok"]
             self.status_code = response_data["status_code"]
             self.status_message = response_data["status_message"]
             carter_data = response_data["carter_data"]
@@ -68,12 +69,12 @@
     def __str__(self):
         if self.ok:
             return f"{self.type.capitalize()} interaction {self.id} - {self.input_text} -> {self.output_text}"
         else:
             return f"{self.type.capitalize()} interaction {self.id} - Failed with status code {self.status_code} and message {self.status_message}"
 
     def print_verbose(self):
+        print("=====================================")
+        print(f"{self.type.upper()} INTERACTION {self.id}")
         for key, value in self.__dict__.items():
-            print("=====================================")
-            print(f"{self.type.upper()} INTERACTION {self.id}")
             print(f"{key}: {value}")
-            print("=====================================")
+        print("=====================================")
```

### Comparing `carter-py-0.1/license.txt` & `carter-py-0.1.1/license.txt`

 * *Files identical despite different names*

### Comparing `carter-py-0.1/setup.py` & `carter-py-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="carter-py",
-    version="0.1",
+    version="0.1.1",
     packages=find_packages(),
     install_requires = [
     "aiohttp==3.8.4",
     "aioresponses==0.7.4",
     "asynctest==0.13.0",
     "python-dotenv==1.0.0",
     "Requests==2.28.2",
```

