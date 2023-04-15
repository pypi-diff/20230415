# Comparing `tmp/chat-spiral-0.0.3.tar.gz` & `tmp/chat-spiral-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat-spiral-0.0.3.tar", last modified: Fri Apr 14 15:31:48 2023, max compression
+gzip compressed data, was "chat-spiral-0.0.4.tar", last modified: Sat Apr 15 02:18:49 2023, max compression
```

## Comparing `chat-spiral-0.0.3.tar` & `chat-spiral-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 15:31:48.453131 chat-spiral-0.0.3/
--rw-rw-rw-   0        0        0     1092 2023-04-09 17:15:16.000000 chat-spiral-0.0.3/LICENSE
--rw-rw-rw-   0        0        0    12666 2023-04-14 15:31:48.449142 chat-spiral-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    12143 2023-04-14 15:30:44.000000 chat-spiral-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 15:31:48.432188 chat-spiral-0.0.3/chat_spiral.egg-info/
--rw-rw-rw-   0        0        0    12666 2023-04-14 15:31:48.000000 chat-spiral-0.0.3/chat_spiral.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2023-04-14 15:31:48.000000 chat-spiral-0.0.3/chat_spiral.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 15:31:48.000000 chat-spiral-0.0.3/chat_spiral.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-14 15:31:48.000000 chat-spiral-0.0.3/chat_spiral.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-14 15:31:48.000000 chat-spiral-0.0.3/chat_spiral.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 15:31:48.453131 chat-spiral-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      891 2023-04-14 15:31:00.000000 chat-spiral-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 15:31:48.447147 chat-spiral-0.0.3/spiral/
--rw-rw-rw-   0        0        0        0 2023-04-14 04:22:39.000000 chat-spiral-0.0.3/spiral/__init__.py
--rw-rw-rw-   0        0        0     5385 2023-04-14 04:47:37.000000 chat-spiral-0.0.3/spiral/chat_history.py
--rw-rw-rw-   0        0        0     1330 2023-04-14 04:47:37.000000 chat-spiral-0.0.3/spiral/chat_llm.py
--rw-rw-rw-   0        0        0    51040 2023-04-14 15:31:34.000000 chat-spiral-0.0.3/spiral/flow.py
--rw-rw-rw-   0        0        0     4899 2023-04-14 15:31:34.000000 chat-spiral-0.0.3/spiral/memory.py
--rw-rw-rw-   0        0        0    14376 2023-04-11 23:37:20.000000 chat-spiral-0.0.3/spiral/message.py
--rw-rw-rw-   0        0        0     2266 2023-04-14 15:31:34.000000 chat-spiral-0.0.3/spiral/tools.py
+drwxrwxrwx   0        0        0        0 2023-04-15 02:18:49.264073 chat-spiral-0.0.4/
+-rw-rw-rw-   0        0        0     1092 2023-04-15 01:05:52.000000 chat-spiral-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0    12666 2023-04-15 02:18:49.263098 chat-spiral-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    12143 2023-04-15 01:05:52.000000 chat-spiral-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 02:18:49.200752 chat-spiral-0.0.4/chat_spiral.egg-info/
+-rw-rw-rw-   0        0        0    12666 2023-04-15 02:18:48.000000 chat-spiral-0.0.4/chat_spiral.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-04-15 02:18:49.000000 chat-spiral-0.0.4/chat_spiral.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 02:18:48.000000 chat-spiral-0.0.4/chat_spiral.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-04-15 02:18:48.000000 chat-spiral-0.0.4/chat_spiral.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-15 02:18:48.000000 chat-spiral-0.0.4/chat_spiral.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 02:18:49.264073 chat-spiral-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      891 2023-04-15 02:17:11.000000 chat-spiral-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 02:18:49.261117 chat-spiral-0.0.4/spiral/
+-rw-rw-rw-   0        0        0       21 2023-04-15 01:05:52.000000 chat-spiral-0.0.4/spiral/__init__.py
+-rw-rw-rw-   0        0        0     5385 2023-04-15 01:05:52.000000 chat-spiral-0.0.4/spiral/chat_history.py
+-rw-rw-rw-   0        0        0     1330 2023-04-15 01:05:52.000000 chat-spiral-0.0.4/spiral/chat_llm.py
+-rw-rw-rw-   0        0        0    51040 2023-04-15 01:05:52.000000 chat-spiral-0.0.4/spiral/flow.py
+-rw-rw-rw-   0        0        0     7551 2023-04-15 01:05:52.000000 chat-spiral-0.0.4/spiral/memory.py
+-rw-rw-rw-   0        0        0    14377 2023-04-15 01:05:52.000000 chat-spiral-0.0.4/spiral/message.py
+-rw-rw-rw-   0        0        0     2266 2023-04-15 01:05:52.000000 chat-spiral-0.0.4/spiral/tools.py
```

### Comparing `chat-spiral-0.0.3/LICENSE` & `chat-spiral-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chat-spiral-0.0.3/PKG-INFO` & `chat-spiral-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-spiral
-Version: 0.0.3
+Version: 0.0.4
 Summary: A framework for creating chat spirals for Large Language Models finetuned for conversations. Currently work-in-progress.
 Home-page: https://github.com/Tiger767/spiral
 Author: Travis Hammond
 License: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `chat-spiral-0.0.3/README.md` & `chat-spiral-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `chat-spiral-0.0.3/chat_spiral.egg-info/PKG-INFO` & `chat-spiral-0.0.4/chat_spiral.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-spiral
-Version: 0.0.3
+Version: 0.0.4
 Summary: A framework for creating chat spirals for Large Language Models finetuned for conversations. Currently work-in-progress.
 Home-page: https://github.com/Tiger767/spiral
 Author: Travis Hammond
 License: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `chat-spiral-0.0.3/setup.py` & `chat-spiral-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="chat-spiral",
-    version="0.0.3",
+    version="0.0.4",
     author="Travis Hammond",
     description="A framework for creating chat spirals for Large Language Models finetuned for conversations. Currently work-in-progress.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Tiger767/spiral",
     packages=setuptools.find_packages(),
     install_requires=[
```

### Comparing `chat-spiral-0.0.3/spiral/chat_history.py` & `chat-spiral-0.0.4/spiral/chat_history.py`

 * *Files identical despite different names*

### Comparing `chat-spiral-0.0.3/spiral/chat_llm.py` & `chat-spiral-0.0.4/spiral/chat_llm.py`

 * *Files identical despite different names*

### Comparing `chat-spiral-0.0.3/spiral/flow.py` & `chat-spiral-0.0.4/spiral/flow.py`

 * *Files identical despite different names*

### Comparing `chat-spiral-0.0.3/spiral/message.py` & `chat-spiral-0.0.4/spiral/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -382,15 +382,15 @@
         """
         pattern = (
             re.escape(content_format)
             .replace("\\{", "{")
             .replace("\\}", "}")
             .format(**{name: "(?P<{}>[\s\S]*)".format(name) for name in names})
         )
-        result = re.match(pattern, content)
+        result = re.search(pattern, content)
         if result is None:
             raise ExtractionError(
                 f"Could not extract variables from JSON message content.\nContent format: {content_format}\nPattern: {pattern}\nContent: {content}"
             )
         variables = result.groupdict()
 
         json_variables = {}
```

### Comparing `chat-spiral-0.0.3/spiral/tools.py` & `chat-spiral-0.0.4/spiral/tools.py`

 * *Files identical despite different names*

