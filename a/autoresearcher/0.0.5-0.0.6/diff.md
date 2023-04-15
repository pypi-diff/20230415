# Comparing `tmp/autoresearcher-0.0.5.tar.gz` & `tmp/autoresearcher-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoresearcher-0.0.5.tar", last modified: Tue Apr 11 04:06:25 2023, max compression
+gzip compressed data, was "autoresearcher-0.0.6.tar", last modified: Sat Apr 15 17:25:05 2023, max compression
```

## Comparing `autoresearcher-0.0.5.tar` & `autoresearcher-0.0.6.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 04:06:25.556544 autoresearcher-0.0.5/
--rw-r--r--   0 marapelzer   (501) staff       (20)     1070 2023-04-11 00:23:06.000000 autoresearcher-0.0.5/LICENSE
--rw-r--r--   0 marapelzer   (501) staff       (20)     3130 2023-04-11 04:06:25.556053 autoresearcher-0.0.5/PKG-INFO
--rw-r--r--   0 marapelzer   (501) staff       (20)     2678 2023-04-11 04:05:37.000000 autoresearcher-0.0.5/README.md
-drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 04:06:25.546365 autoresearcher-0.0.5/autoresearcher/
--rw-r--r--   0 marapelzer   (501) staff       (20)       77 2023-04-11 03:55:00.000000 autoresearcher-0.0.5/autoresearcher/__init__.py
-drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 04:06:25.549205 autoresearcher-0.0.5/autoresearcher/data_sources/
--rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:55:00.000000 autoresearcher-0.0.5/autoresearcher/data_sources/__init__.py
-drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 04:06:25.550921 autoresearcher-0.0.5/autoresearcher/data_sources/web_apis/
--rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:55:00.000000 autoresearcher-0.0.5/autoresearcher/data_sources/web_apis/__init__.py
--rw-r--r--   0 marapelzer   (501) staff       (20)      585 2023-04-11 03:55:00.000000 autoresearcher-0.0.5/autoresearcher/data_sources/web_apis/base_web_api_data_loader.py
--rw-r--r--   0 marapelzer   (501) staff       (20)     1627 2023-04-11 03:55:00.000000 autoresearcher-0.0.5/autoresearcher/data_sources/web_apis/semantic_scholar_loader.py
-drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 04:06:25.552070 autoresearcher-0.0.5/autoresearcher/llms/
--rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:55:00.000000 autoresearcher-0.0.5/autoresearcher/llms/__init__.py
--rw-r--r--   0 marapelzer   (501) staff       (20)     1204 2023-04-11 03:55:00.000000 autoresearcher-0.0.5/autoresearcher/llms/openai.py
-drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 04:06:25.553254 autoresearcher-0.0.5/autoresearcher/utils/
--rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:55:00.000000 autoresearcher-0.0.5/autoresearcher/utils/__init__.py
--rw-r--r--   0 marapelzer   (501) staff       (20)      366 2023-04-11 03:55:00.000000 autoresearcher-0.0.5/autoresearcher/utils/get_citations.py
--rw-r--r--   0 marapelzer   (501) staff       (20)     1632 2023-04-11 03:55:00.000000 autoresearcher-0.0.5/autoresearcher/utils/prompts.py
-drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 04:06:25.554194 autoresearcher-0.0.5/autoresearcher/workflows/
--rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:55:00.000000 autoresearcher-0.0.5/autoresearcher/workflows/__init__.py
-drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 04:06:25.555153 autoresearcher-0.0.5/autoresearcher/workflows/literature_review/
--rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-11 03:55:00.000000 autoresearcher-0.0.5/autoresearcher/workflows/literature_review/__init__.py
--rw-r--r--   0 marapelzer   (501) staff       (20)     5684 2023-04-11 03:56:51.000000 autoresearcher-0.0.5/autoresearcher/workflows/literature_review/literature_review.py
-drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-11 04:06:25.548819 autoresearcher-0.0.5/autoresearcher.egg-info/
--rw-r--r--   0 marapelzer   (501) staff       (20)     3130 2023-04-11 04:06:25.000000 autoresearcher-0.0.5/autoresearcher.egg-info/PKG-INFO
--rw-r--r--   0 marapelzer   (501) staff       (20)      796 2023-04-11 04:06:25.000000 autoresearcher-0.0.5/autoresearcher.egg-info/SOURCES.txt
--rw-r--r--   0 marapelzer   (501) staff       (20)        1 2023-04-11 04:06:25.000000 autoresearcher-0.0.5/autoresearcher.egg-info/dependency_links.txt
--rw-r--r--   0 marapelzer   (501) staff       (20)      109 2023-04-11 04:06:25.000000 autoresearcher-0.0.5/autoresearcher.egg-info/requires.txt
--rw-r--r--   0 marapelzer   (501) staff       (20)       15 2023-04-11 04:06:25.000000 autoresearcher-0.0.5/autoresearcher.egg-info/top_level.txt
--rw-r--r--   0 marapelzer   (501) staff       (20)      103 2023-04-11 03:55:00.000000 autoresearcher-0.0.5/pyproject.toml
--rw-r--r--   0 marapelzer   (501) staff       (20)       38 2023-04-11 04:06:25.556671 autoresearcher-0.0.5/setup.cfg
--rw-r--r--   0 marapelzer   (501) staff       (20)      935 2023-04-11 04:01:14.000000 autoresearcher-0.0.5/setup.py
+drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-15 17:25:05.778550 autoresearcher-0.0.6/
+-rw-r--r--   0 marapelzer   (501) staff       (20)     1070 2023-04-11 00:23:06.000000 autoresearcher-0.0.6/LICENSE
+-rw-r--r--   0 marapelzer   (501) staff       (20)        9 2023-04-14 15:47:19.000000 autoresearcher-0.0.6/MANIFEST.in
+-rw-r--r--   0 marapelzer   (501) staff       (20)     3132 2023-04-15 17:25:05.778239 autoresearcher-0.0.6/PKG-INFO
+-rw-r--r--   0 marapelzer   (501) staff       (20)     2680 2023-04-11 05:07:01.000000 autoresearcher-0.0.6/README.md
+drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-15 17:25:05.767184 autoresearcher-0.0.6/autoresearcher/
+-rw-r--r--   0 marapelzer   (501) staff       (20)       77 2023-04-15 00:53:20.000000 autoresearcher-0.0.6/autoresearcher/__init__.py
+drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-15 17:25:05.770323 autoresearcher-0.0.6/autoresearcher/data_sources/
+-rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-11 04:54:36.000000 autoresearcher-0.0.6/autoresearcher/data_sources/__init__.py
+drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-15 17:25:05.772205 autoresearcher-0.0.6/autoresearcher/data_sources/web_apis/
+-rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-11 04:54:36.000000 autoresearcher-0.0.6/autoresearcher/data_sources/web_apis/__init__.py
+-rw-r--r--   0 marapelzer   (501) staff       (20)      585 2023-04-11 04:54:36.000000 autoresearcher-0.0.6/autoresearcher/data_sources/web_apis/base_web_api_data_loader.py
+-rw-r--r--   0 marapelzer   (501) staff       (20)     1627 2023-04-11 04:54:36.000000 autoresearcher-0.0.6/autoresearcher/data_sources/web_apis/semantic_scholar_loader.py
+-rw-r--r--   0 marapelzer   (501) staff       (20)     1641 2023-04-14 15:47:19.000000 autoresearcher-0.0.6/autoresearcher/data_sources/web_apis/wikipedia_loader.py
+drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-15 17:25:05.774455 autoresearcher-0.0.6/autoresearcher/llms/
+-rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-11 04:54:36.000000 autoresearcher-0.0.6/autoresearcher/llms/__init__.py
+-rw-r--r--   0 marapelzer   (501) staff       (20)     1204 2023-04-11 04:54:36.000000 autoresearcher-0.0.6/autoresearcher/llms/openai.py
+drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-15 17:25:05.776720 autoresearcher-0.0.6/autoresearcher/utils/
+-rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-11 04:54:36.000000 autoresearcher-0.0.6/autoresearcher/utils/__init__.py
+-rw-r--r--   0 marapelzer   (501) staff       (20)      206 2023-04-15 17:23:31.000000 autoresearcher-0.0.6/autoresearcher/utils/count_tokens.py
+-rw-r--r--   0 marapelzer   (501) staff       (20)      436 2023-04-15 17:23:31.000000 autoresearcher-0.0.6/autoresearcher/utils/get_citations.py
+-rw-r--r--   0 marapelzer   (501) staff       (20)     1632 2023-04-11 04:54:36.000000 autoresearcher-0.0.6/autoresearcher/utils/prompts.py
+drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-15 17:25:05.777274 autoresearcher-0.0.6/autoresearcher/workflows/
+-rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-11 04:54:36.000000 autoresearcher-0.0.6/autoresearcher/workflows/__init__.py
+drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-15 17:25:05.777771 autoresearcher-0.0.6/autoresearcher/workflows/literature_review/
+-rw-r--r--   0 marapelzer   (501) staff       (20)        0 2023-04-11 04:54:36.000000 autoresearcher-0.0.6/autoresearcher/workflows/literature_review/__init__.py
+-rw-r--r--   0 marapelzer   (501) staff       (20)     6083 2023-04-15 17:23:31.000000 autoresearcher-0.0.6/autoresearcher/workflows/literature_review/literature_review.py
+drwxr-xr-x   0 marapelzer   (501) staff       (20)        0 2023-04-15 17:25:05.769816 autoresearcher-0.0.6/autoresearcher.egg-info/
+-rw-r--r--   0 marapelzer   (501) staff       (20)     3132 2023-04-15 17:25:05.000000 autoresearcher-0.0.6/autoresearcher.egg-info/PKG-INFO
+-rw-r--r--   0 marapelzer   (501) staff       (20)      902 2023-04-15 17:25:05.000000 autoresearcher-0.0.6/autoresearcher.egg-info/SOURCES.txt
+-rw-r--r--   0 marapelzer   (501) staff       (20)        1 2023-04-15 17:25:05.000000 autoresearcher-0.0.6/autoresearcher.egg-info/dependency_links.txt
+-rw-r--r--   0 marapelzer   (501) staff       (20)      125 2023-04-15 17:25:05.000000 autoresearcher-0.0.6/autoresearcher.egg-info/requires.txt
+-rw-r--r--   0 marapelzer   (501) staff       (20)       15 2023-04-15 17:25:05.000000 autoresearcher-0.0.6/autoresearcher.egg-info/top_level.txt
+-rw-r--r--   0 marapelzer   (501) staff       (20)      103 2023-04-11 04:54:36.000000 autoresearcher-0.0.6/pyproject.toml
+-rw-r--r--   0 marapelzer   (501) staff       (20)       38 2023-04-15 17:25:05.778647 autoresearcher-0.0.6/setup.cfg
+-rw-r--r--   0 marapelzer   (501) staff       (20)      963 2023-04-15 17:24:55.000000 autoresearcher-0.0.6/setup.py
```

### Comparing `autoresearcher-0.0.5/LICENSE` & `autoresearcher-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `autoresearcher-0.0.5/PKG-INFO` & `autoresearcher-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: autoresearcher
-Version: 0.0.5
+Version: 0.0.6
 Summary: Automating scientic workflows with AI
 Home-page: https://github.com/eimenhmdt/autoresearcher
 Author: Eimen Hamedat
 Author-email: eimen.hamedat@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🤖🧪 AutoResearcher
 
 ---
 
-⚡ Automating scientic workflows with AI ⚡
+⚡ Automating scientific workflows with AI ⚡
 
 [![Discord](https://img.shields.io/discord/1094636825647267910?label=AutoResearcher&logo=discord&style=flat-square)](https://discord.gg/PnQDR5h9)
 
 ---
 
 ## What is AutoResearcher?
```

### Comparing `autoresearcher-0.0.5/README.md` & `autoresearcher-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # 🤖🧪 AutoResearcher
 
 ---
 
-⚡ Automating scientic workflows with AI ⚡
+⚡ Automating scientific workflows with AI ⚡
 
 [![Discord](https://img.shields.io/discord/1094636825647267910?label=AutoResearcher&logo=discord&style=flat-square)](https://discord.gg/PnQDR5h9)
 
 ---
 
 ## What is AutoResearcher?
```

### Comparing `autoresearcher-0.0.5/autoresearcher/data_sources/web_apis/base_web_api_data_loader.py` & `autoresearcher-0.0.6/autoresearcher/data_sources/web_apis/base_web_api_data_loader.py`

 * *Files identical despite different names*

### Comparing `autoresearcher-0.0.5/autoresearcher/data_sources/web_apis/semantic_scholar_loader.py` & `autoresearcher-0.0.6/autoresearcher/data_sources/web_apis/semantic_scholar_loader.py`

 * *Files identical despite different names*

### Comparing `autoresearcher-0.0.5/autoresearcher/llms/openai.py` & `autoresearcher-0.0.6/autoresearcher/llms/openai.py`

 * *Files identical despite different names*

### Comparing `autoresearcher-0.0.5/autoresearcher/utils/prompts.py` & `autoresearcher-0.0.6/autoresearcher/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `autoresearcher-0.0.5/autoresearcher/workflows/literature_review/literature_review.py` & `autoresearcher-0.0.6/autoresearcher/workflows/literature_review/literature_review.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 from termcolor import colored
 from autoresearcher.llms.openai import openai_call
 from autoresearcher.utils.get_citations import get_citation_by_doi
 from autoresearcher.utils.prompts import literature_review_prompt, extract_answer_prompt, keyword_combination_prompt
+from autoresearcher.utils.count_tokens import count_tokens
 from autoresearcher.data_sources.web_apis.semantic_scholar_loader import SemanticScholarLoader
 
 def literature_review(research_question, output_file=None):
 
     SemanticScholar = SemanticScholarLoader()
 
     # Generate keyword combinations for a given research question
@@ -40,30 +41,39 @@
                 answers.append(answer_with_citation)
                 print(colored(f"Answer found!", "green"))
                 print(colored(f"{answer_with_citation}", "cyan"))
 
         return answers
 
     # Combine answers into a concise literature review using OpenAI API
-    def combine_answers(answers, research_question, use_gpt4=False, temperature=0.1, max_tokens=1800):
+    def combine_answers(answers, research_question, use_gpt4=False, temperature=0.1):
         answer_list = "\n\n".join(answers)
         prompt = literature_review_prompt.format(research_question=research_question, answer_list=answer_list)
+        
+        # Calculate the tokens in the input
+        input_tokens = count_tokens(prompt)
+        
+        # Calculate the remaining tokens for the response
+        remaining_tokens = 4080 - input_tokens
+        max_tokens = max(remaining_tokens, 0)
         literature_review = openai_call(prompt, use_gpt4=use_gpt4, temperature=temperature, max_tokens=max_tokens)
 
         return literature_review
 
     # Extract bibliographical citations from answers
     def extract_citations(answers):
         citations = []
         for answer in answers:
             citation_start = answer.rfind("SOURCE: ")
             if citation_start != -1:
                 citation = answer[citation_start + len("SOURCE: "):]
                 citations.append(citation)
         return citations
+    
+    
 
     print(colored(f"Research question: {research_question}", "yellow", attrs=["bold", "blink"]))
     print(colored("Auto Researcher initiated!", "yellow"))
 
     # Generate keyword combinations
     print(colored("Generating keyword combinations...", "yellow"))
     keyword_combinations = generate_keyword_combinations(research_question)
@@ -103,18 +113,18 @@
             f.write(literature_review)
         print(colored(f"Literature review saved to {output_file}", "green"))
 
     return literature_review
 
 if __name__ == "__main__":
     import sys
-
+    
     if len(sys.argv) > 2:
         research_question = sys.argv[1]
         output_file = sys.argv[2]
     elif len(sys.argv) > 1:
         research_question = sys.argv[1]
         output_file = None
     else:
-        raise ValueError("No research question provided.")
+        raise ValueError("No research question provided. Usage: python literature_review.py 'My research question' 'optional_output_file.txt'")
 
-    literature_review(research_question, output_file)
+    literature_review(research_question, output_file)
```

### Comparing `autoresearcher-0.0.5/autoresearcher.egg-info/PKG-INFO` & `autoresearcher-0.0.6/autoresearcher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: autoresearcher
-Version: 0.0.5
+Version: 0.0.6
 Summary: Automating scientic workflows with AI
 Home-page: https://github.com/eimenhmdt/autoresearcher
 Author: Eimen Hamedat
 Author-email: eimen.hamedat@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🤖🧪 AutoResearcher
 
 ---
 
-⚡ Automating scientic workflows with AI ⚡
+⚡ Automating scientific workflows with AI ⚡
 
 [![Discord](https://img.shields.io/discord/1094636825647267910?label=AutoResearcher&logo=discord&style=flat-square)](https://discord.gg/PnQDR5h9)
 
 ---
 
 ## What is AutoResearcher?
```

### Comparing `autoresearcher-0.0.5/autoresearcher.egg-info/SOURCES.txt` & `autoresearcher-0.0.6/autoresearcher.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 autoresearcher/__init__.py
 autoresearcher.egg-info/PKG-INFO
 autoresearcher.egg-info/SOURCES.txt
 autoresearcher.egg-info/dependency_links.txt
 autoresearcher.egg-info/requires.txt
 autoresearcher.egg-info/top_level.txt
 autoresearcher/data_sources/__init__.py
 autoresearcher/data_sources/web_apis/__init__.py
 autoresearcher/data_sources/web_apis/base_web_api_data_loader.py
 autoresearcher/data_sources/web_apis/semantic_scholar_loader.py
+autoresearcher/data_sources/web_apis/wikipedia_loader.py
 autoresearcher/llms/__init__.py
 autoresearcher/llms/openai.py
 autoresearcher/utils/__init__.py
+autoresearcher/utils/count_tokens.py
 autoresearcher/utils/get_citations.py
 autoresearcher/utils/prompts.py
 autoresearcher/workflows/__init__.py
 autoresearcher/workflows/literature_review/__init__.py
 autoresearcher/workflows/literature_review/literature_review.py
```

### Comparing `autoresearcher-0.0.5/setup.py` & `autoresearcher-0.0.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="autoresearcher",
-    version="0.0.5",
+    version="0.0.6",
     author="Eimen Hamedat",
     author_email="eimen.hamedat@gmail.com",
     description="Automating scientic workflows with AI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/eimenhmdt/autoresearcher",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(),
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     include_package_data=True,
     install_requires=[
         "openai==0.27.0",
         "python-dotenv==1.0.0",
         "requests==2.26.0",
         "termcolor==1.1.0",
         "jellyfish==0.11.2",
+        "tiktoken==0.3.3",
         "setuptools>=42",
         "wheel"
     ],
-)
+)
```

