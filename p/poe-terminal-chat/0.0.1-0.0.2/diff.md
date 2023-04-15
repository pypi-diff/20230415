# Comparing `tmp/poe_terminal_chat-0.0.1.tar.gz` & `tmp/poe_terminal_chat-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poe_terminal_chat-0.0.1.tar", last modified: Sat Apr 15 14:51:20 2023, max compression
+gzip compressed data, was "poe_terminal_chat-0.0.2.tar", last modified: Sat Apr 15 15:43:22 2023, max compression
```

## Comparing `poe_terminal_chat-0.0.1.tar` & `poe_terminal_chat-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 14:51:20.743716 poe_terminal_chat-0.0.1/
--rw-rw-rw-   0        0        0     1087 2023-04-15 14:49:57.000000 poe_terminal_chat-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      212 2023-04-15 14:51:20.743716 poe_terminal_chat-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-15 12:06:49.000000 poe_terminal_chat-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 14:51:20.741200 poe_terminal_chat-0.0.1/poe_terminal_chat.egg-info/
--rw-rw-rw-   0        0        0      212 2023-04-15 14:51:20.000000 poe_terminal_chat-0.0.1/poe_terminal_chat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-04-15 14:51:20.000000 poe_terminal_chat-0.0.1/poe_terminal_chat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 14:51:20.000000 poe_terminal_chat-0.0.1/poe_terminal_chat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-15 14:51:20.000000 poe_terminal_chat-0.0.1/poe_terminal_chat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       54 2023-04-15 14:51:20.000000 poe_terminal_chat-0.0.1/poe_terminal_chat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-15 14:51:20.000000 poe_terminal_chat-0.0.1/poe_terminal_chat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 14:51:20.744719 poe_terminal_chat-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      684 2023-04-15 14:41:00.000000 poe_terminal_chat-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 15:43:22.508199 poe_terminal_chat-0.0.2/
+-rw-rw-rw-   0        0        0     1087 2023-04-15 14:49:57.000000 poe_terminal_chat-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      211 2023-04-15 15:43:22.507690 poe_terminal_chat-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-15 12:06:49.000000 poe_terminal_chat-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 15:43:22.493648 poe_terminal_chat-0.0.2/poe_terminal_chat/
+-rw-rw-rw-   0        0        0        0 2023-04-15 12:08:35.000000 poe_terminal_chat-0.0.2/poe_terminal_chat/__init__.py
+-rw-rw-rw-   0        0        0     1006 2023-04-15 14:36:02.000000 poe_terminal_chat-0.0.2/poe_terminal_chat/command_line.py
+-rw-rw-rw-   0        0        0      506 2023-04-15 14:29:11.000000 poe_terminal_chat-0.0.2/poe_terminal_chat/poeterminal.py
+-rw-rw-rw-   0        0        0      862 2023-04-15 14:38:03.000000 poe_terminal_chat-0.0.2/poe_terminal_chat/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-15 15:43:22.506690 poe_terminal_chat-0.0.2/poe_terminal_chat.egg-info/
+-rw-rw-rw-   0        0        0      211 2023-04-15 15:43:22.000000 poe_terminal_chat-0.0.2/poe_terminal_chat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-04-15 15:43:22.000000 poe_terminal_chat-0.0.2/poe_terminal_chat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 15:43:22.000000 poe_terminal_chat-0.0.2/poe_terminal_chat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-04-15 15:43:22.000000 poe_terminal_chat-0.0.2/poe_terminal_chat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       54 2023-04-15 15:43:22.000000 poe_terminal_chat-0.0.2/poe_terminal_chat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-15 15:43:22.000000 poe_terminal_chat-0.0.2/poe_terminal_chat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 15:43:22.508199 poe_terminal_chat-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      686 2023-04-15 15:42:55.000000 poe_terminal_chat-0.0.2/setup.py
```

### Comparing `poe_terminal_chat-0.0.1/LICENSE` & `poe_terminal_chat-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `poe_terminal_chat-0.0.1/setup.py` & `poe_terminal_chat-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup
 
 setup(
         name="poe_terminal_chat",
-        version="0.0.1",
+        version="0.0.2",
         descrption="poe(a third part AI assistant) terminal chat, can have accesses of chatgpt and claude",
         url="https://github.com/Mushrr/poe_terminal_chat",
-        author="Mushrr",
+        author="Mushr",
         author_email="huangxingjiegkd@163.com",
         license="MIT",
         packages=["poe_terminal_chat"],
         entry_points = {
-            'console_scripts': ['poechat=poe_terminal_chat.src.entry:main']
+            'console_scripts': ['poechat=poe_terminal_chat.command_line:main']
             },
         install_requires=[
             "poe-api>=0.2.10",
             "requests>=2.28.2",
             "python-dotenv>=1.0.0"
             ]
         )
```

