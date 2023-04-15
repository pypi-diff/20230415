# Comparing `tmp/TelegramNotificator-1.0.2.tar.gz` & `tmp/TelegramNotificator-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TelegramNotificator-1.0.2.tar", last modified: Sat Apr 15 02:40:58 2023, max compression
+gzip compressed data, was "TelegramNotificator-1.0.3.tar", last modified: Sat Apr 15 02:45:07 2023, max compression
```

## Comparing `TelegramNotificator-1.0.2.tar` & `TelegramNotificator-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 02:40:58.436481 TelegramNotificator-1.0.2/
--rw-rw-rw-   0        0        0      700 2023-04-15 02:40:58.436481 TelegramNotificator-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      707 2023-04-15 01:22:00.000000 TelegramNotificator-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 02:40:58.420853 TelegramNotificator-1.0.2/TelegramNotificator.egg-info/
--rw-rw-rw-   0        0        0      700 2023-04-15 02:40:58.000000 TelegramNotificator-1.0.2/TelegramNotificator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-04-15 02:40:58.000000 TelegramNotificator-1.0.2/TelegramNotificator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 02:40:58.000000 TelegramNotificator-1.0.2/TelegramNotificator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-15 02:40:58.000000 TelegramNotificator-1.0.2/TelegramNotificator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-15 02:40:58.000000 TelegramNotificator-1.0.2/TelegramNotificator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 02:40:58.436481 TelegramNotificator-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      933 2023-04-15 02:39:44.000000 TelegramNotificator-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 02:40:58.436481 TelegramNotificator-1.0.2/telegram_notificator/
--rw-rw-rw-   0        0        0       52 2023-04-15 01:11:28.000000 TelegramNotificator-1.0.2/telegram_notificator/__init__.py
--rw-rw-rw-   0        0        0      523 2023-04-15 01:04:48.000000 TelegramNotificator-1.0.2/telegram_notificator/telegram_notificator.py
+drwxrwxrwx   0        0        0        0 2023-04-15 02:45:07.990819 TelegramNotificator-1.0.3/
+-rw-rw-rw-   0        0        0     1063 2023-04-15 02:05:41.000000 TelegramNotificator-1.0.3/LICENCE
+-rw-rw-rw-   0        0        0      723 2023-04-15 02:45:07.989817 TelegramNotificator-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      707 2023-04-15 01:22:00.000000 TelegramNotificator-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 02:45:07.982816 TelegramNotificator-1.0.3/TelegramNotificator.egg-info/
+-rw-rw-rw-   0        0        0      723 2023-04-15 02:45:07.000000 TelegramNotificator-1.0.3/TelegramNotificator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-04-15 02:45:07.000000 TelegramNotificator-1.0.3/TelegramNotificator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 02:45:07.000000 TelegramNotificator-1.0.3/TelegramNotificator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-15 02:45:07.000000 TelegramNotificator-1.0.3/TelegramNotificator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-15 02:45:07.000000 TelegramNotificator-1.0.3/TelegramNotificator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 02:45:07.990819 TelegramNotificator-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      933 2023-04-15 02:44:27.000000 TelegramNotificator-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 02:45:07.986818 TelegramNotificator-1.0.3/telegram_notificator/
+-rw-rw-rw-   0        0        0       52 2023-04-15 01:11:28.000000 TelegramNotificator-1.0.3/telegram_notificator/__init__.py
+-rw-rw-rw-   0        0        0      523 2023-04-15 01:04:48.000000 TelegramNotificator-1.0.3/telegram_notificator/telegram_notificator.py
```

### Comparing `TelegramNotificator-1.0.2/PKG-INFO` & `TelegramNotificator-1.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: TelegramNotificator
-Version: 1.0.2
+Version: 1.0.3
 Summary: A basic telegram notifications sender.
 Author: Cryptoroid
 Author-email: 
 License: MIT
 Keywords: telegram,message,notification,alert,send message,telegram message,telegram bot
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
+License-File: LICENCE
 
 Send telegram notifications or alerts from your python programs.
```

### Comparing `TelegramNotificator-1.0.2/README.md` & `TelegramNotificator-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `TelegramNotificator-1.0.2/TelegramNotificator.egg-info/PKG-INFO` & `TelegramNotificator-1.0.3/TelegramNotificator.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: TelegramNotificator
-Version: 1.0.2
+Version: 1.0.3
 Summary: A basic telegram notifications sender.
 Author: Cryptoroid
 Author-email: 
 License: MIT
 Keywords: telegram,message,notification,alert,send message,telegram message,telegram bot
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
+License-File: LICENCE
 
 Send telegram notifications or alerts from your python programs.
```

### Comparing `TelegramNotificator-1.0.2/setup.py` & `TelegramNotificator-1.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 # Setting up
 setup(
     name="TelegramNotificator",
-    version='1.0.2',
+    version='1.0.3',
     author="Cryptoroid",
     author_email="",
     license='MIT',
     description='A basic telegram notifications sender.',
     long_description_content_type="text/markdown",
     long_description='Send telegram notifications or alerts from your python programs.',
     packages=find_packages(),
```

### Comparing `TelegramNotificator-1.0.2/telegram_notificator/telegram_notificator.py` & `TelegramNotificator-1.0.3/telegram_notificator/telegram_notificator.py`

 * *Files identical despite different names*

