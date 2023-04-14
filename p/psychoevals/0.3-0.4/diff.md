# Comparing `tmp/psychoevals-0.3.tar.gz` & `tmp/psychoevals-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychoevals-0.3.tar", last modified: Fri Apr 14 21:55:52 2023, max compression
+gzip compressed data, was "psychoevals-0.4.tar", last modified: Fri Apr 14 22:39:35 2023, max compression
```

## Comparing `psychoevals-0.3.tar` & `psychoevals-0.4.tar`

### file list

```diff
@@ -1,28 +1,35 @@
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 21:55:52.007039 psychoevals-0.3/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      328 2023-04-14 21:55:52.007039 psychoevals-0.3/PKG-INFO
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     6066 2023-04-14 21:19:33.000000 psychoevals-0.3/README.md
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 21:55:51.997039 psychoevals-0.3/psychoevals/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-13 22:48:29.000000 psychoevals-0.3/psychoevals/__init__.py
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 21:55:51.997039 psychoevals-0.3/psychoevals/agents/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       50 2023-04-13 22:53:06.000000 psychoevals-0.3/psychoevals/agents/__init__.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      202 2023-04-12 23:17:23.000000 psychoevals-0.3/psychoevals/agents/base_eval_agent.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      378 2023-04-13 23:06:38.000000 psychoevals-0.3/psychoevals/cognitive_state.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      442 2023-04-13 22:56:20.000000 psychoevals-0.3/psychoevals/evaluation.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1716 2023-04-14 21:54:45.000000 psychoevals-0.3/psychoevals/moderation.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      121 2023-04-12 23:17:13.000000 psychoevals-0.3/psychoevals/qna_result.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     4127 2023-04-13 23:33:58.000000 psychoevals-0.3/psychoevals/security.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     3882 2023-04-14 21:54:37.000000 psychoevals-0.3/psychoevals/utils.py
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 21:55:51.997039 psychoevals-0.3/psychoevals.egg-info/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      328 2023-04-14 21:55:51.000000 psychoevals-0.3/psychoevals.egg-info/PKG-INFO
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      550 2023-04-14 21:55:51.000000 psychoevals-0.3/psychoevals.egg-info/SOURCES.txt
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        1 2023-04-14 21:55:51.000000 psychoevals-0.3/psychoevals.egg-info/dependency_links.txt
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       67 2023-04-14 21:55:51.000000 psychoevals-0.3/psychoevals.egg-info/requires.txt
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       18 2023-04-14 21:55:51.000000 psychoevals-0.3/psychoevals.egg-info/top_level.txt
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       38 2023-04-14 21:55:52.007039 psychoevals-0.3/setup.cfg
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      579 2023-04-14 21:55:39.000000 psychoevals-0.3/setup.py
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 21:55:52.007039 psychoevals-0.3/tests/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 20:36:27.000000 psychoevals-0.3/tests/__init__.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     3039 2023-04-14 20:33:13.000000 psychoevals-0.3/tests/test_mbti.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1852 2023-04-14 20:16:12.000000 psychoevals-0.3/tests/test_moderation.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1424 2023-04-14 20:16:27.000000 psychoevals-0.3/tests/test_security.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      893 2023-04-14 20:16:18.000000 psychoevals-0.3/tests/test_troll_agent.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:39:35.357039 psychoevals-0.4/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      328 2023-04-14 22:39:35.357039 psychoevals-0.4/PKG-INFO
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     6066 2023-04-14 21:19:33.000000 psychoevals-0.4/README.md
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:39:35.357039 psychoevals-0.4/psychoevals/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-13 22:48:29.000000 psychoevals-0.4/psychoevals/__init__.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:39:35.357039 psychoevals-0.4/psychoevals/agents/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:34:56.000000 psychoevals-0.4/psychoevals/agents/__init__.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      202 2023-04-12 23:17:23.000000 psychoevals-0.4/psychoevals/agents/base_eval_agent.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:39:35.357039 psychoevals-0.4/psychoevals/agents/myers_briggs/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       37 2023-04-14 22:36:25.000000 psychoevals-0.4/psychoevals/agents/myers_briggs/__init__.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     2405 2023-04-13 23:34:22.000000 psychoevals-0.4/psychoevals/agents/myers_briggs/mbti_statements.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     2270 2023-04-13 22:52:06.000000 psychoevals-0.4/psychoevals/agents/myers_briggs/myers_briggs.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:39:35.357039 psychoevals-0.4/psychoevals/agents/troll_agent/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       35 2023-04-14 22:37:10.000000 psychoevals-0.4/psychoevals/agents/troll_agent/__init__.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1215 2023-04-14 20:25:42.000000 psychoevals-0.4/psychoevals/agents/troll_agent/troll_agent.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      378 2023-04-13 23:06:38.000000 psychoevals-0.4/psychoevals/cognitive_state.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      442 2023-04-13 22:56:20.000000 psychoevals-0.4/psychoevals/evaluation.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1716 2023-04-14 21:54:45.000000 psychoevals-0.4/psychoevals/moderation.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      121 2023-04-12 23:17:13.000000 psychoevals-0.4/psychoevals/qna_result.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     4127 2023-04-13 23:33:58.000000 psychoevals-0.4/psychoevals/security.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     3882 2023-04-14 21:54:37.000000 psychoevals-0.4/psychoevals/utils.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:39:35.357039 psychoevals-0.4/psychoevals.egg-info/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      328 2023-04-14 22:39:35.000000 psychoevals-0.4/psychoevals.egg-info/PKG-INFO
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      782 2023-04-14 22:39:35.000000 psychoevals-0.4/psychoevals.egg-info/SOURCES.txt
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        1 2023-04-14 22:39:35.000000 psychoevals-0.4/psychoevals.egg-info/dependency_links.txt
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       67 2023-04-14 22:39:35.000000 psychoevals-0.4/psychoevals.egg-info/requires.txt
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       18 2023-04-14 22:39:35.000000 psychoevals-0.4/psychoevals.egg-info/top_level.txt
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       38 2023-04-14 22:39:35.357039 psychoevals-0.4/setup.cfg
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      579 2023-04-14 22:39:29.000000 psychoevals-0.4/setup.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:39:35.357039 psychoevals-0.4/tests/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 20:36:27.000000 psychoevals-0.4/tests/__init__.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     3052 2023-04-14 22:36:16.000000 psychoevals-0.4/tests/test_mbti.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1852 2023-04-14 20:16:12.000000 psychoevals-0.4/tests/test_moderation.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1424 2023-04-14 20:16:27.000000 psychoevals-0.4/tests/test_security.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      881 2023-04-14 22:37:17.000000 psychoevals-0.4/tests/test_troll_agent.py
```

### Comparing `psychoevals-0.3/README.md` & `psychoevals-0.4/README.md`

 * *Files identical despite different names*

### Comparing `psychoevals-0.3/psychoevals/moderation.py` & `psychoevals-0.4/psychoevals/moderation.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.3/psychoevals/security.py` & `psychoevals-0.4/psychoevals/security.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.3/psychoevals/utils.py` & `psychoevals-0.4/psychoevals/utils.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.3/psychoevals.egg-info/SOURCES.txt` & `psychoevals-0.4/psychoevals.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -10,12 +10,17 @@
 psychoevals.egg-info/PKG-INFO
 psychoevals.egg-info/SOURCES.txt
 psychoevals.egg-info/dependency_links.txt
 psychoevals.egg-info/requires.txt
 psychoevals.egg-info/top_level.txt
 psychoevals/agents/__init__.py
 psychoevals/agents/base_eval_agent.py
+psychoevals/agents/myers_briggs/__init__.py
+psychoevals/agents/myers_briggs/mbti_statements.py
+psychoevals/agents/myers_briggs/myers_briggs.py
+psychoevals/agents/troll_agent/__init__.py
+psychoevals/agents/troll_agent/troll_agent.py
 tests/__init__.py
 tests/test_mbti.py
 tests/test_moderation.py
 tests/test_security.py
 tests/test_troll_agent.py
```

### Comparing `psychoevals-0.3/setup.py` & `psychoevals-0.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='psychoevals',
-    version='0.3',
+    version='0.4',
     packages=find_packages(),
     install_requires=[
         "openai>=0.27.0",
         "pandas>=1.3.0",
         "tenacity>=8.0.0",
         "python-dotenv>=0.15.0"
     ],
```

### Comparing `psychoevals-0.3/tests/test_mbti.py` & `psychoevals-0.4/tests/test_mbti.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # test_end_to_end.py
 import pandas as pd
-from psychoevals.agents import MyersBriggs
+from psychoevals.agents.myers_briggs import MyersBriggs
 from psychoevals.cognitive_state import CognitiveState
 
 def test_myers_briggs():
     mbti = MyersBriggs()
 
     # Test with a fictional character description
     extroverted_character_description = '''
```

### Comparing `psychoevals-0.3/tests/test_moderation.py` & `psychoevals-0.4/tests/test_moderation.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.3/tests/test_security.py` & `psychoevals-0.4/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.3/tests/test_troll_agent.py` & `psychoevals-0.4/tests/test_troll_agent.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from psychoevals.agents.troll_agent.troll_agent import TrollAgent
+from psychoevals.agents.troll_agent import TrollAgent
 from psychoevals.cognitive_state import CognitiveState
 
 def test_troll_agent():
     # Instantiate the TrollAgent and a CognitiveState
     troll_agent = TrollAgent()
     cognitive_state = CognitiveState("")
```

