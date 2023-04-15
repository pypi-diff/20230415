# Comparing `tmp/mongopersistence-0.2.0.tar.gz` & `tmp/mongopersistence-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongopersistence-0.2.0.tar", max compression
+gzip compressed data, was "mongopersistence-0.3.0.tar", max compression
```

## Comparing `mongopersistence-0.2.0.tar` & `mongopersistence-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-04-08 15:03:17.174512 mongopersistence-0.2.0/LICENSE
--rw-r--r--   0        0        0     2219 2023-04-08 15:03:17.174657 mongopersistence-0.2.0/README.md
--rw-r--r--   0        0        0       57 2023-04-08 15:15:28.419882 mongopersistence-0.2.0/mongopersistence/__init__.py
--rw-r--r--   0        0        0     9918 2023-04-09 19:21:09.184267 mongopersistence-0.2.0/mongopersistence/persistence.py
--rw-r--r--   0        0        0      406 2023-04-09 20:27:18.310535 mongopersistence-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2784 1970-01-01 00:00:00.000000 mongopersistence-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-15 11:26:21.541175 mongopersistence-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2492 2023-04-15 11:26:21.541350 mongopersistence-0.3.0/README.md
+-rw-r--r--   0        0        0       80 2023-04-15 11:26:21.541580 mongopersistence-0.3.0/mongopersistence/__init__.py
+-rw-r--r--   0        0        0    13729 2023-04-15 11:26:21.541800 mongopersistence-0.3.0/mongopersistence/persistence.py
+-rw-r--r--   0        0        0      874 2023-04-15 11:26:21.542619 mongopersistence-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3055 1970-01-01 00:00:00.000000 mongopersistence-0.3.0/PKG-INFO
```

### Comparing `mongopersistence-0.2.0/LICENSE` & `mongopersistence-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mongopersistence-0.2.0/README.md` & `mongopersistence-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,89 @@
+Metadata-Version: 2.1
+Name: mongopersistence
+Version: 0.3.0
+Summary: Package to add persistence to your telegram bot using pymongo
+License: MIT
+Author: LucaSforza
+Author-email: lucasforza1234@icloud.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: motor (>=3.1.2,<4.0.0)
+Requires-Dist: python-telegram-bot (>=20.1,<21.0)
+Description-Content-Type: text/markdown
 
 # MongoPersistence
 
 Package to add persistence to your telegram bot in a mongodb database.
 
-ATTENTION: MongoPersistence is a new project, it should work, but if you encounter any bugs please report them in the [Issues](https://github.com/LucaSforza/MongoPersistence/issues) section and if you have an idea how to fix it please consider opening a [PR](https://github.com/LucaSforza/MongoPersistence/pulls).
+ATTENTION: MongoPersistence is a new project, it should work, but if you encounter any bugs, please report them in
+the [Issues](https://github.com/LucaSforza/MongoPersistence/issues) section and if you have an idea how to fix it, please
+consider opening a [PR](https://github.com/LucaSforza/MongoPersistence/pulls).
+
 ## Usage
 
-First make sure you have created a database using mongodb.
+First, make sure you've created a database using mongodb.
 If you haven't already, click [here](https://www.mongodb.com) to get started.
 
 Then create a collection in your database for each type of data you want to make persistent.
 
 ```python
-from mongopersistence import *
 from telegram.ext import Application
 
-dbhelper = DBMongoHelper(
-    'your-mongodb-key',
-    'your-database-name',
-    name_col_user_data='my-collection-for-user-data'
+from mongopersistence import MongoPersistence
+
+persistence = MongoPersistence(
+    mongo_url="mongodb://username:password@your-ip:27017/",
+    db_name="your-database-name",
+    name_col_user_data="my-collection-for-user-data",  # optional
+    name_col_chat_data="my-collection-for-chat-data",  # optional
+    name_col_bot_data="my-collection-for-bot-data",  # optional
+    name_col_conversations_data="my-collection-for-conversations",  # optional
+    create_col_if_not_exist=True,  # optional
+    ignore_general_data=["cache"],
+    ignore_user_data=["foo", "bar"],
 )
 
-application = Application.builder().token('your-token'
-        ).persistence(MongoPersistence(dbhelper)
-        ).build()
+application = (
+    Application
+    .builder()
+    .token("your-token")
+    .persistence(persistence).build()
+)
 ```
 
-With this code you will add persistence only to user_data and since the `load_on_flush` attribute has not been specified then the data will be loaded only when the bot is shut down.
+With this code you will add persistence only to user_data and since the `load_on_flush` attribute has not been specified
+then the data will be loaded only when the bot is shut down.
+
+If you want the data to be loaded continuously instead, define:
 
-If you want the data to be loaded continuously instead define:
 ```python
- MongoPersistence(dbhelper,load_on_flush=False,update_interval=60)
+MongoPersistence(..., load_on_flush=False, update_interval=60)
 ```
 
 `update_interval` can also be undefined and the default is `60`.
 
-One of the advantages of setting `load_on_flush = False` is that if you modify the database (either directly from the site or through the code of your other app) then it will automatically be updated to the modified data type inside your bot, without having to shut it down first !
-
-The last thing to specify is to be CAREFUL in adding permission to your IP on the [mongodb site](https://www.mongodb.com), otherwise you will encounter an error running the bot.
-
+One of the advantages of setting `load_on_flush = False` is that if you modify the database (either directly from the
+site or through the code of your other app) then it will automatically be updated to the modified data type inside your
+bot, without having to shut it down first !
+
+The last thing to specify is to be CAREFUL
+in adding permission to your IP on the [mongodb site](https://www.mongodb.com).
+Otherwise, you will encounter an error running the bot.
 
 ## Installation
 
 Install mongopersistence with pip
 
 ```bash
-  pip install mongopersistence
+pip install mongopersistence
 ```
-    
+
 ## Roadmap
 
 Search all the TODOs in this repo to see how you can contribute to this package, but in general:
 
 - Add support for make persistent callback data.
 
-- Add a feature that allows you to ignore dictionary elements using string lists so they don't become persistent.
-
```

