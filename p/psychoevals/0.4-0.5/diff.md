# Comparing `tmp/psychoevals-0.4.tar.gz` & `tmp/psychoevals-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychoevals-0.4.tar", last modified: Fri Apr 14 22:39:35 2023, max compression
+gzip compressed data, was "psychoevals-0.5.tar", last modified: Fri Apr 14 22:48:15 2023, max compression
```

## Comparing `psychoevals-0.4.tar` & `psychoevals-0.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:39:35.357039 psychoevals-0.4/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      328 2023-04-14 22:39:35.357039 psychoevals-0.4/PKG-INFO
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     6066 2023-04-14 21:19:33.000000 psychoevals-0.4/README.md
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:39:35.357039 psychoevals-0.4/psychoevals/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-13 22:48:29.000000 psychoevals-0.4/psychoevals/__init__.py
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:39:35.357039 psychoevals-0.4/psychoevals/agents/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:34:56.000000 psychoevals-0.4/psychoevals/agents/__init__.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      202 2023-04-12 23:17:23.000000 psychoevals-0.4/psychoevals/agents/base_eval_agent.py
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:39:35.357039 psychoevals-0.4/psychoevals/agents/myers_briggs/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       37 2023-04-14 22:36:25.000000 psychoevals-0.4/psychoevals/agents/myers_briggs/__init__.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     2405 2023-04-13 23:34:22.000000 psychoevals-0.4/psychoevals/agents/myers_briggs/mbti_statements.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     2270 2023-04-13 22:52:06.000000 psychoevals-0.4/psychoevals/agents/myers_briggs/myers_briggs.py
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:39:35.357039 psychoevals-0.4/psychoevals/agents/troll_agent/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       35 2023-04-14 22:37:10.000000 psychoevals-0.4/psychoevals/agents/troll_agent/__init__.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1215 2023-04-14 20:25:42.000000 psychoevals-0.4/psychoevals/agents/troll_agent/troll_agent.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      378 2023-04-13 23:06:38.000000 psychoevals-0.4/psychoevals/cognitive_state.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      442 2023-04-13 22:56:20.000000 psychoevals-0.4/psychoevals/evaluation.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1716 2023-04-14 21:54:45.000000 psychoevals-0.4/psychoevals/moderation.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      121 2023-04-12 23:17:13.000000 psychoevals-0.4/psychoevals/qna_result.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     4127 2023-04-13 23:33:58.000000 psychoevals-0.4/psychoevals/security.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     3882 2023-04-14 21:54:37.000000 psychoevals-0.4/psychoevals/utils.py
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:39:35.357039 psychoevals-0.4/psychoevals.egg-info/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      328 2023-04-14 22:39:35.000000 psychoevals-0.4/psychoevals.egg-info/PKG-INFO
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      782 2023-04-14 22:39:35.000000 psychoevals-0.4/psychoevals.egg-info/SOURCES.txt
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        1 2023-04-14 22:39:35.000000 psychoevals-0.4/psychoevals.egg-info/dependency_links.txt
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       67 2023-04-14 22:39:35.000000 psychoevals-0.4/psychoevals.egg-info/requires.txt
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       18 2023-04-14 22:39:35.000000 psychoevals-0.4/psychoevals.egg-info/top_level.txt
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       38 2023-04-14 22:39:35.357039 psychoevals-0.4/setup.cfg
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      579 2023-04-14 22:39:29.000000 psychoevals-0.4/setup.py
-drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:39:35.357039 psychoevals-0.4/tests/
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 20:36:27.000000 psychoevals-0.4/tests/__init__.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     3052 2023-04-14 22:36:16.000000 psychoevals-0.4/tests/test_mbti.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1852 2023-04-14 20:16:12.000000 psychoevals-0.4/tests/test_moderation.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1424 2023-04-14 20:16:27.000000 psychoevals-0.4/tests/test_security.py
--rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      881 2023-04-14 22:37:17.000000 psychoevals-0.4/tests/test_troll_agent.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:48:15.827037 psychoevals-0.5/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      328 2023-04-14 22:48:15.827037 psychoevals-0.5/PKG-INFO
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     6727 2023-04-14 22:46:24.000000 psychoevals-0.5/README.md
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:48:15.827037 psychoevals-0.5/psychoevals/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-13 22:48:29.000000 psychoevals-0.5/psychoevals/__init__.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:48:15.827037 psychoevals-0.5/psychoevals/agents/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:46:24.000000 psychoevals-0.5/psychoevals/agents/__init__.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      202 2023-04-12 23:17:23.000000 psychoevals-0.5/psychoevals/agents/base_eval_agent.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:48:15.827037 psychoevals-0.5/psychoevals/agents/myers_briggs/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       37 2023-04-14 22:46:24.000000 psychoevals-0.5/psychoevals/agents/myers_briggs/__init__.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     2405 2023-04-13 23:34:22.000000 psychoevals-0.5/psychoevals/agents/myers_briggs/mbti_statements.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     2270 2023-04-13 22:52:06.000000 psychoevals-0.5/psychoevals/agents/myers_briggs/myers_briggs.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:48:15.827037 psychoevals-0.5/psychoevals/agents/troll_agent/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       35 2023-04-14 22:46:24.000000 psychoevals-0.5/psychoevals/agents/troll_agent/__init__.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1215 2023-04-14 20:25:42.000000 psychoevals-0.5/psychoevals/agents/troll_agent/troll_agent.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      378 2023-04-13 23:06:38.000000 psychoevals-0.5/psychoevals/cognitive_state.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      442 2023-04-13 22:56:20.000000 psychoevals-0.5/psychoevals/evaluation.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1716 2023-04-14 22:46:24.000000 psychoevals-0.5/psychoevals/moderation.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      121 2023-04-12 23:17:13.000000 psychoevals-0.5/psychoevals/qna_result.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     4127 2023-04-13 23:33:58.000000 psychoevals-0.5/psychoevals/security.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     3882 2023-04-14 22:46:24.000000 psychoevals-0.5/psychoevals/utils.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:48:15.827037 psychoevals-0.5/psychoevals.egg-info/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      328 2023-04-14 22:48:15.000000 psychoevals-0.5/psychoevals.egg-info/PKG-INFO
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      782 2023-04-14 22:48:15.000000 psychoevals-0.5/psychoevals.egg-info/SOURCES.txt
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        1 2023-04-14 22:48:15.000000 psychoevals-0.5/psychoevals.egg-info/dependency_links.txt
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       67 2023-04-14 22:48:15.000000 psychoevals-0.5/psychoevals.egg-info/requires.txt
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       18 2023-04-14 22:48:15.000000 psychoevals-0.5/psychoevals.egg-info/top_level.txt
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)       38 2023-04-14 22:48:15.827037 psychoevals-0.5/setup.cfg
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      579 2023-04-14 22:48:01.000000 psychoevals-0.5/setup.py
+drwxr-xr-x   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 22:48:15.827037 psychoevals-0.5/tests/
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)        0 2023-04-14 20:36:27.000000 psychoevals-0.5/tests/__init__.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     3052 2023-04-14 22:46:24.000000 psychoevals-0.5/tests/test_mbti.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1852 2023-04-14 20:16:12.000000 psychoevals-0.5/tests/test_moderation.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)     1424 2023-04-14 20:16:27.000000 psychoevals-0.5/tests/test_security.py
+-rw-r--r--   0 jhwang5   (1000) jhwang5   (1000)      881 2023-04-14 22:46:53.000000 psychoevals-0.5/tests/test_troll_agent.py
```

### Comparing `psychoevals-0.4/README.md` & `psychoevals-0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,41 @@
-# PsychoEvals
+# PsychoEvals: Prompt Security and Psychometrics Framework for LLMs
 
-PsychoEvals is a Python library for evaluating and securing the behavior of large language models (LLMs), such as OpenAI's GPT series. The library provides a testing framework that enables researchers, developers, and enthusiasts to better understand, evaluate, and secure LLMs using psychometric tests, security features, and moderation tools.
+PsychoEvals is a lightweight Python library for evaluating and securing the behavior of large language models (LLMs) and agents, such as OpenAI's GPT series. The library provides a testing framework that enables researchers, developers, and enthusiasts to better understand, evaluate, and secure LLMs using psychometric tests, security features, and moderation tools.
 
-## 4 Canonical Use Cases
+🚀 4 Canonical Use Cases
 
 * Apply a battery of 'troll' questions to provoke a NSFW answer from your Chatbot prompt
 * Apply psychometric tests on Agent prompts (aka `CognitiveState`)
 * Secure your LLM response from basic prompt hijacking and injection attacks
 * Moderate the response from your LLM for any issues based on some criteria (hate, violence, etc)
 
-## Install
+💾 Install
 
-To install: 
+1) pip install the module. 
 `pip install psychoevals`
 
-Example:
+2) create a virtual env, i.e. 
+`python -m venv .venv`
+
+3) activate the virtual env
+`source .venv/bin/activate`
+
+4) create a new file called .env and put your `OPENAI_API_KEY` in it
+```bash
+OPENAI_API_KEY=<your key>
+```
+
+5) install dependencies
+```
+pip3 install -r requirements.txt
 ```
+
+Usage Example:
+```python
 from psychoevals.moderation import moderate, basic_moderation_handler
 
 text_sequence_normal = "Sample text with non-offensive content."
 text_sequence_violent = "I will kill them."
 
 # demonstrates the use of Global flag. If any category is flagged, it's flagged and transformed.
 # basic_moderation_handler is a function you pass to trigger a custom response 
@@ -28,15 +44,15 @@
     return f"Processing the following text: {text_sequence}"
 
 assert(process_text_global(text_sequence_normal) != "Flagged")
 ```
 
 ## Motivation
 
-As LLM-based agents become more prevalent, it is essential to have a standardized and accessible way to evaluate their pseudo "psychiatric" attributes and properties. Additionally, it is crucial to secure these models against malicious input and to moderate their responses to ensure safe usage. PsychoGPT aims to fill these gaps by providing a comprehensive framework that addresses both evaluation and security concerns.
+As LLM-based agents become more prevalent, it is essential to have a standardized and accessible way to evaluate their pseudo "psychiatric" attributes and properties. Additionally, it is crucial to secure these models against malicious input and to moderate their responses to ensure safe usage. PsychoEvals aims to fill these gaps by providing a comprehensive framework that addresses both evaluation and security concerns.
 
 Use cases:
 * Character profiling of agents in real time 
 * Preventing prompt injection attempts
 * Quantifying "weirdness" in prompts
 * Psychometric profiling of agents and their evolutions over time
 * Real time detection of psychiatric episodes of agents
@@ -59,45 +75,45 @@
 3. Create a new branch for your feature or bugfix.
 4. Implement your changes, making sure to follow the project's coding style and guidelines.
 5. Commit your changes and push them to your forked repository.
 6. Create a pull request, describing the changes you've made and the problem they solve.
 
 ## How It Works
 
-PsychoGPT is built around three core modules: agents, security, and moderation.
+PsychoEvals is built around three core modules: agents, security, and moderation.
 
 ### Agents Quickstart
 
-```
+```python
 # TrollAgent applies a battery of tests to provoke a NSFW answer from the prompt
 troll_agent = TrollAgent() # Instantiate the TrollAgent 
 cognitive_state = CognitiveState(<agent's prompt state>) # Instantiate a Sandbox for Your Agent's Prompt
 evaluation = troll_agent.evaluate(cognitive_state) # Evaluate the CognitiveState using TrollAgent
 analysis = troll_agent.analyze(evaluation) # Analyze the evaluation
 assert(len(analysis["nsfw_responses"]) == 0) # assert no NSFW responses
 ```
 
 The agents module provides a range of evaluation tools, such as psychometric tests, that can be used to assess the behavior and characteristics of LLMs. Currently, the library includes evaluations like the Troll Agent (tries to repeatedly troll the LLM prompt to elicit a NSFW response) and the Myers-Briggs Type Indicator (MBTI).
 
 ### Security Quickstart
 
-```
+```python
 from psychoevals.security import secure_prompt 
 ...
 # Function using secure_prompt decorator with the custom filter
 @secure_prompt(policy_filters=[policy_filter], handler=http_response_handler)
 def process_text(text_sequence: str) -> str:
     return f"Processing the following text: {text_sequence}"
 ```
 
 The security module offers a set of tools and decorators designed to protect LLMs from prompt injection attacks and other malicious input. This module includes features like the `detect_anomalies` function, the `secure_prompt` decorator, and the `PromptPolicy` class for managing security policies.
 
 ### Moderation Quickstart
 
-```
+```python
 from psychoevals.moderation import moderate, basic_moderation_handler
 
 text_sequence_normal = "Sample text with non-offensive content."
 text_sequence_violent = "I will kill them."
 
 # demonstrates the use of Global flag. If any category is flagged, it's flagged and transformed.
 @moderate(handler=basic_moderation_handler, global_threshold=True)
@@ -124,7 +140,16 @@
 - `prompt_filter_generator` create custom prompt filters against custom PromptPolicies 
 - `PromptPolicy` class for managing and applying security policies
 
 ## List of Moderation Tools
 
 - `moderate` decorator for flagging and handling content violations
 - Customizable content moderation thresholds and policies
+
+## How to Cite
+@misc{nextworddev2023psychoevals,
+  title={PsychoEvals: A Psychometrics Evaluation Testing Framework for Large Language Models},
+  author={John, Nextworddev},
+  year={2023},
+  url={https://github.com/nextworddev/psychoevals},
+}
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `psychoevals-0.4/psychoevals/agents/myers_briggs/mbti_statements.py` & `psychoevals-0.5/psychoevals/agents/myers_briggs/mbti_statements.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.4/psychoevals/agents/myers_briggs/myers_briggs.py` & `psychoevals-0.5/psychoevals/agents/myers_briggs/myers_briggs.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.4/psychoevals/agents/troll_agent/troll_agent.py` & `psychoevals-0.5/psychoevals/agents/troll_agent/troll_agent.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.4/psychoevals/moderation.py` & `psychoevals-0.5/psychoevals/moderation.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.4/psychoevals/security.py` & `psychoevals-0.5/psychoevals/security.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.4/psychoevals/utils.py` & `psychoevals-0.5/psychoevals/utils.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.4/psychoevals.egg-info/SOURCES.txt` & `psychoevals-0.5/psychoevals.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psychoevals-0.4/setup.py` & `psychoevals-0.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='psychoevals',
-    version='0.4',
+    version='0.5',
     packages=find_packages(),
     install_requires=[
         "openai>=0.27.0",
         "pandas>=1.3.0",
         "tenacity>=8.0.0",
         "python-dotenv>=0.15.0"
     ],
```

### Comparing `psychoevals-0.4/tests/test_mbti.py` & `psychoevals-0.5/tests/test_mbti.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.4/tests/test_moderation.py` & `psychoevals-0.5/tests/test_moderation.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.4/tests/test_security.py` & `psychoevals-0.5/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `psychoevals-0.4/tests/test_troll_agent.py` & `psychoevals-0.5/tests/test_troll_agent.py`

 * *Files identical despite different names*

