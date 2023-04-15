# Comparing `tmp/TelegramNotificator-1.0.3.tar.gz` & `tmp/TelegramNotificator-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TelegramNotificator-1.0.3.tar", last modified: Sat Apr 15 02:45:07 2023, max compression
+gzip compressed data, was "TelegramNotificator-1.0.4.tar", last modified: Sat Apr 15 02:59:21 2023, max compression
```

## Comparing `TelegramNotificator-1.0.3.tar` & `TelegramNotificator-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 02:45:07.990819 TelegramNotificator-1.0.3/
--rw-rw-rw-   0        0        0     1063 2023-04-15 02:05:41.000000 TelegramNotificator-1.0.3/LICENCE
--rw-rw-rw-   0        0        0      723 2023-04-15 02:45:07.989817 TelegramNotificator-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      707 2023-04-15 01:22:00.000000 TelegramNotificator-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 02:45:07.982816 TelegramNotificator-1.0.3/TelegramNotificator.egg-info/
--rw-rw-rw-   0        0        0      723 2023-04-15 02:45:07.000000 TelegramNotificator-1.0.3/TelegramNotificator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-04-15 02:45:07.000000 TelegramNotificator-1.0.3/TelegramNotificator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 02:45:07.000000 TelegramNotificator-1.0.3/TelegramNotificator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-15 02:45:07.000000 TelegramNotificator-1.0.3/TelegramNotificator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-15 02:45:07.000000 TelegramNotificator-1.0.3/TelegramNotificator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 02:45:07.990819 TelegramNotificator-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      933 2023-04-15 02:44:27.000000 TelegramNotificator-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 02:45:07.986818 TelegramNotificator-1.0.3/telegram_notificator/
--rw-rw-rw-   0        0        0       52 2023-04-15 01:11:28.000000 TelegramNotificator-1.0.3/telegram_notificator/__init__.py
--rw-rw-rw-   0        0        0      523 2023-04-15 01:04:48.000000 TelegramNotificator-1.0.3/telegram_notificator/telegram_notificator.py
+drwxrwxrwx   0        0        0        0 2023-04-15 02:59:21.442502 TelegramNotificator-1.0.4/
+-rw-rw-rw-   0        0        0     1063 2023-04-15 02:05:41.000000 TelegramNotificator-1.0.4/LICENCE
+-rw-rw-rw-   0        0        0      723 2023-04-15 02:59:21.439497 TelegramNotificator-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      659 2023-04-15 02:50:22.000000 TelegramNotificator-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 02:59:21.382216 TelegramNotificator-1.0.4/TelegramNotificator.egg-info/
+-rw-rw-rw-   0        0        0      723 2023-04-15 02:59:21.000000 TelegramNotificator-1.0.4/TelegramNotificator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-04-15 02:59:21.000000 TelegramNotificator-1.0.4/TelegramNotificator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 02:59:21.000000 TelegramNotificator-1.0.4/TelegramNotificator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-15 02:59:21.000000 TelegramNotificator-1.0.4/TelegramNotificator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-15 02:59:21.000000 TelegramNotificator-1.0.4/TelegramNotificator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 02:59:21.442502 TelegramNotificator-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      933 2023-04-15 02:58:56.000000 TelegramNotificator-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 02:59:21.385215 TelegramNotificator-1.0.4/telegram_notificator/
+-rw-rw-rw-   0        0        0      523 2023-04-15 02:58:12.000000 TelegramNotificator-1.0.4/telegram_notificator/__init__.py
+-rw-rw-rw-   0        0        0      524 2023-04-15 02:58:43.000000 TelegramNotificator-1.0.4/telegram_notificator/telegram_notificator.py
```

### Comparing `TelegramNotificator-1.0.3/LICENCE` & `TelegramNotificator-1.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `TelegramNotificator-1.0.3/PKG-INFO` & `TelegramNotificator-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TelegramNotificator
-Version: 1.0.3
+Version: 1.0.4
 Summary: A basic telegram notifications sender.
 Author: Cryptoroid
 Author-email: 
 License: MIT
 Keywords: telegram,message,notification,alert,send message,telegram message,telegram bot
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `TelegramNotificator-1.0.3/README.md` & `TelegramNotificator-1.0.4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 **Send telegram notifications or alerts from your python programs.**
 
 
 <div align="left">
 
 ## Installation
   
-Install the libriry requests as follow:
+Install the library TelegramNotificator as follow:
 
 ```
-pip install requests
+pip install TelegramNotificator
 ```
 
-Then copy the telegram_notificator file to your project folder and us it as the following example:
+Then simply use it like this:
 
 ```python
-from telegram_notificator import telegram_notificator as tn
+from telegram_notificator import TelegramNotificator as tn
 
 def telegram = tn(YOUR_TELEGRAM_BOT_TOKEN, YOUR_TELEGRAM_CHAT_ID)
 
 telegram.send_message('Hello world!')
 ```
 
 To get your `YOUR_TELEGRAM_BOT_TOKEN` and `YOUR_TELEGRAM_CHAT_ID` details just do a search about how to create a telegram bot using [BotFather](https://t.me/botfather).
```

### Comparing `TelegramNotificator-1.0.3/TelegramNotificator.egg-info/PKG-INFO` & `TelegramNotificator-1.0.4/TelegramNotificator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TelegramNotificator
-Version: 1.0.3
+Version: 1.0.4
 Summary: A basic telegram notifications sender.
 Author: Cryptoroid
 Author-email: 
 License: MIT
 Keywords: telegram,message,notification,alert,send message,telegram message,telegram bot
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `TelegramNotificator-1.0.3/setup.py` & `TelegramNotificator-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 # Setting up
 setup(
     name="TelegramNotificator",
-    version='1.0.3',
+    version='1.0.4',
     author="Cryptoroid",
     author_email="",
     license='MIT',
     description='A basic telegram notifications sender.',
     long_description_content_type="text/markdown",
     long_description='Send telegram notifications or alerts from your python programs.',
     packages=find_packages(),
```

### Comparing `TelegramNotificator-1.0.3/telegram_notificator/telegram_notificator.py` & `TelegramNotificator-1.0.4/telegram_notificator/__init__.py`

 * *Files identical despite different names*

