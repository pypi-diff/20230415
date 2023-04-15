# Comparing `tmp/psychoevals-0.5.tar.gz` & `tmp/psychoevals-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychoevals-0.5.tar", last modified: Fri Apr 14 22:48:15 2023, max compression
+gzip compressed data, was "psychoevals-0.6.tar", last modified: Sat Apr 15 02:46:36 2023, max compression
```

## Comparing `psychoevals-0.5.tar` & `psychoevals-0.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:48:15.827037 psychoevals-0.5/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      328 2023-04-14 22:48:15.827037 psychoevals-0.5/PKG-INFO
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     6727 2023-04-14 22:46:24.000000 psychoevals-0.5/README.md
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:48:15.827037 psychoevals-0.5/psychoevals/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-13 22:48:29.000000 psychoevals-0.5/psychoevals/__init__.py
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:48:15.827037 psychoevals-0.5/psychoevals/agents/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:46:24.000000 psychoevals-0.5/psychoevals/agents/__init__.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      202 2023-04-12 23:17:23.000000 psychoevals-0.5/psychoevals/agents/base_eval_agent.py
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:48:15.827037 psychoevals-0.5/psychoevals/agents/myers_briggs/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       37 2023-04-14 22:46:24.000000 psychoevals-0.5/psychoevals/agents/myers_briggs/__init__.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     2405 2023-04-13 23:34:22.000000 psychoevals-0.5/psychoevals/agents/myers_briggs/mbti_statements.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     2270 2023-04-13 22:52:06.000000 psychoevals-0.5/psychoevals/agents/myers_briggs/myers_briggs.py
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:48:15.827037 psychoevals-0.5/psychoevals/agents/troll_agent/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       35 2023-04-14 22:46:24.000000 psychoevals-0.5/psychoevals/agents/troll_agent/__init__.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1215 2023-04-14 20:25:42.000000 psychoevals-0.5/psychoevals/agents/troll_agent/troll_agent.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      378 2023-04-13 23:06:38.000000 psychoevals-0.5/psychoevals/cognitive_state.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      442 2023-04-13 22:56:20.000000 psychoevals-0.5/psychoevals/evaluation.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1716 2023-04-14 22:46:24.000000 psychoevals-0.5/psychoevals/moderation.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      121 2023-04-12 23:17:13.000000 psychoevals-0.5/psychoevals/qna_result.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     4127 2023-04-13 23:33:58.000000 psychoevals-0.5/psychoevals/security.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     3882 2023-04-14 22:46:24.000000 psychoevals-0.5/psychoevals/utils.py
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:48:15.827037 psychoevals-0.5/psychoevals.egg-info/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      328 2023-04-14 22:48:15.000000 psychoevals-0.5/psychoevals.egg-info/PKG-INFO
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      782 2023-04-14 22:48:15.000000 psychoevals-0.5/psychoevals.egg-info/SOURCES.txt
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        1 2023-04-14 22:48:15.000000 psychoevals-0.5/psychoevals.egg-info/dependency_links.txt
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       67 2023-04-14 22:48:15.000000 psychoevals-0.5/psychoevals.egg-info/requires.txt
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       18 2023-04-14 22:48:15.000000 psychoevals-0.5/psychoevals.egg-info/top_level.txt
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       38 2023-04-14 22:48:15.827037 psychoevals-0.5/setup.cfg
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      579 2023-04-14 22:48:01.000000 psychoevals-0.5/setup.py
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:48:15.827037 psychoevals-0.5/tests/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 20:36:27.000000 psychoevals-0.5/tests/__init__.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     3052 2023-04-14 22:46:24.000000 psychoevals-0.5/tests/test_mbti.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1852 2023-04-14 20:16:12.000000 psychoevals-0.5/tests/test_moderation.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1424 2023-04-14 20:16:27.000000 psychoevals-0.5/tests/test_security.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      881 2023-04-14 22:46:53.000000 psychoevals-0.5/tests/test_troll_agent.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-15 02:46:36.177033 psychoevals-0.6/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      328 2023-04-15 02:46:36.177033 psychoevals-0.6/PKG-INFO
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     6727 2023-04-14 22:46:24.000000 psychoevals-0.6/README.md
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-15 02:46:36.177033 psychoevals-0.6/psychoevals/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-13 22:48:29.000000 psychoevals-0.6/psychoevals/__init__.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-15 02:46:36.177033 psychoevals-0.6/psychoevals/agents/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:46:24.000000 psychoevals-0.6/psychoevals/agents/__init__.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      202 2023-04-12 23:17:23.000000 psychoevals-0.6/psychoevals/agents/base_eval_agent.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-15 02:46:36.177033 psychoevals-0.6/psychoevals/agents/myers_briggs/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       37 2023-04-14 22:46:24.000000 psychoevals-0.6/psychoevals/agents/myers_briggs/__init__.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     2345 2023-04-15 02:45:49.000000 psychoevals-0.6/psychoevals/agents/myers_briggs/mbti_statements.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     2270 2023-04-13 22:52:06.000000 psychoevals-0.6/psychoevals/agents/myers_briggs/myers_briggs.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-15 02:46:36.177033 psychoevals-0.6/psychoevals/agents/troll_agent/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       35 2023-04-14 22:46:24.000000 psychoevals-0.6/psychoevals/agents/troll_agent/__init__.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1215 2023-04-14 20:25:42.000000 psychoevals-0.6/psychoevals/agents/troll_agent/troll_agent.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      378 2023-04-13 23:06:38.000000 psychoevals-0.6/psychoevals/cognitive_state.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      442 2023-04-13 22:56:20.000000 psychoevals-0.6/psychoevals/evaluation.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1716 2023-04-14 22:46:24.000000 psychoevals-0.6/psychoevals/moderation.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      121 2023-04-12 23:17:13.000000 psychoevals-0.6/psychoevals/qna_result.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     4127 2023-04-13 23:33:58.000000 psychoevals-0.6/psychoevals/security.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     3882 2023-04-14 22:46:24.000000 psychoevals-0.6/psychoevals/utils.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-15 02:46:36.177033 psychoevals-0.6/psychoevals.egg-info/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      328 2023-04-15 02:46:36.000000 psychoevals-0.6/psychoevals.egg-info/PKG-INFO
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      782 2023-04-15 02:46:36.000000 psychoevals-0.6/psychoevals.egg-info/SOURCES.txt
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        1 2023-04-15 02:46:36.000000 psychoevals-0.6/psychoevals.egg-info/dependency_links.txt
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       67 2023-04-15 02:46:36.000000 psychoevals-0.6/psychoevals.egg-info/requires.txt
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       18 2023-04-15 02:46:36.000000 psychoevals-0.6/psychoevals.egg-info/top_level.txt
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       38 2023-04-15 02:46:36.177033 psychoevals-0.6/setup.cfg
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      579 2023-04-15 02:44:08.000000 psychoevals-0.6/setup.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-15 02:46:36.177033 psychoevals-0.6/tests/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 20:36:27.000000 psychoevals-0.6/tests/__init__.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     3052 2023-04-14 22:46:24.000000 psychoevals-0.6/tests/test_mbti.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1852 2023-04-14 20:16:12.000000 psychoevals-0.6/tests/test_moderation.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1424 2023-04-14 20:16:27.000000 psychoevals-0.6/tests/test_security.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      881 2023-04-14 22:46:53.000000 psychoevals-0.6/tests/test_troll_agent.py
```

### Comparing `psychoevals-0.5/README.md` & `psychoevals-0.6/README.md`

 * *Files identical despite different names*

### Comparing `psychoevals-0.5/psychoevals/agents/myers_briggs/mbti_statements.py` & `psychoevals-0.6/psychoevals/agents/myers_briggs/mbti_statements.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,41 +6,41 @@
         "I prefer socializing in large groups.",
         "I find it easy to make small talk.",
         "I am more comfortable in social situations than being alone.",
         "I enjoy meeting new people and making friends.",
         "I am outgoing and sociable.",
         "I find it easy to strike up a conversation with strangers."
     ],
-    "S-N": [
+    "N-S": [
         "I prefer abstract ideas over concrete facts.",
         "I prefer to focus on the bigger picture rather than the details.",
         "I am more interested in future possibilities than present realities.",
         "I often think about how things could be improved.",
         "I enjoy discussing theories and concepts.",
         "I often get lost in thought and daydreams.",
         "I find it easy to understand complex ideas and theories.",
         "I enjoy learning about new and innovative ideas.",
         "I enjoy thinking about hypothetical scenarios and possibilities."
     ],
     "T-F": [
         "I make decisions based on logic and reason.",
         "I consider how my decisions will affect others.",
         "When solving problems, I prioritize finding the best solution over preserving harmony.",
-        "I am more focused on my feelings than objective criteria when making decisions.",
+        "I am more focused objective criteria when making decisions than my feelings.",
         "I am more objective than subjective.",
-        "I enjoy discussing my values and personal beliefs.",
+        "I don't enjoy discussing my values and personal beliefs.",
         "I find it important to analyze situations logically.",
         "I prefer to focus on facts and details rather than emotions when making decisions.",
         "I focus on finding the most efficient solution to a problem."
     ],
     "J-P": [
-        "I prefer to make plans and follow them.",
-        "I like to have flexibility in my plans and options.",
-        "I like to make lists and schedules to organize my tasks.",
-        "I often act spontaneously and see where the situation takes me.",
-        "I prefer to follow routines.",
-        "I am adaptable and can adjust to new situations easily.",
-        "I prefer to keep my options open rather than commit to a single choice.",
-        "I like to have a clear plan of action when working on projects.",
-        "I am comfortable with last-minute changes and surprises."
+        "I prefer to have a structured and organized environment.",
+        "I like to make decisions and stick to them.",
+        "I enjoy setting goals and working towards them.",
+        "I feel more comfortable when I have a plan.",
+        "I tend to be punctual and meet deadlines.",
+        "I prefer to finish projects before starting new ones.",
+        "I like to follow routines and schedules.",
+        "I prefer to work in a systematic and methodical way.",
+        "I value order and predictability in my life."
     ]
 }
```

### Comparing `psychoevals-0.5/psychoevals/agents/myers_briggs/myers_briggs.py` & `psychoevals-0.6/psychoevals/agents/myers_briggs/myers_briggs.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.5/psychoevals/agents/troll_agent/troll_agent.py` & `psychoevals-0.6/psychoevals/agents/troll_agent/troll_agent.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.5/psychoevals/moderation.py` & `psychoevals-0.6/psychoevals/moderation.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.5/psychoevals/security.py` & `psychoevals-0.6/psychoevals/security.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.5/psychoevals/utils.py` & `psychoevals-0.6/psychoevals/utils.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.5/psychoevals.egg-info/SOURCES.txt` & `psychoevals-0.6/psychoevals.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psychoevals-0.5/setup.py` & `psychoevals-0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='psychoevals',
-    version='0.5',
+    version='0.6',
     packages=find_packages(),
     install_requires=[
         "openai>=0.27.0",
         "pandas>=1.3.0",
         "tenacity>=8.0.0",
         "python-dotenv>=0.15.0"
     ],
```

### Comparing `psychoevals-0.5/tests/test_mbti.py` & `psychoevals-0.6/tests/test_mbti.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.5/tests/test_moderation.py` & `psychoevals-0.6/tests/test_moderation.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.5/tests/test_security.py` & `psychoevals-0.6/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.5/tests/test_troll_agent.py` & `psychoevals-0.6/tests/test_troll_agent.py`

 * *Files identical despite different names*

