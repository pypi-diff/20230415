# Comparing `tmp/arxiv_bot-0.0.3.tar.gz` & `tmp/arxiv_bot-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arxiv_bot-0.0.3.tar", max compression
+gzip compressed data, was "arxiv_bot-0.0.4.tar", max compression
```

## Comparing `arxiv_bot-0.0.3.tar` & `arxiv_bot-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0       12 2023-02-05 03:03:40.410331 arxiv_bot-0.0.3/README.md
--rw-r--r--   0        0        0      107 2023-03-01 06:15:05.389266 arxiv_bot-0.0.3/arxiv_bot/__init__.py
--rw-r--r--   0        0        0        0 2023-02-27 04:42:53.940169 arxiv_bot-0.0.3/arxiv_bot/knowledge_base/__init__.py
--rw-r--r--   0        0        0      193 2023-02-27 10:27:55.374860 arxiv_bot-0.0.3/arxiv_bot/knowledge_base/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      175 2023-03-01 06:21:23.731532 arxiv_bot-0.0.3/arxiv_bot/knowledge_base/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    14645 2023-02-27 10:27:55.376048 arxiv_bot-0.0.3/arxiv_bot/knowledge_base/__pycache__/constructor.cpython-311.pyc
--rw-r--r--   0        0        0    14741 2023-03-01 06:07:46.313553 arxiv_bot-0.0.3/arxiv_bot/knowledge_base/__pycache__/constructors.cpython-311.pyc
--rw-r--r--   0        0        0    14290 2023-03-17 15:27:14.374433 arxiv_bot-0.0.3/arxiv_bot/knowledge_base/__pycache__/constructors.cpython-39.pyc
--rw-r--r--   0        0        0    10129 2023-03-01 06:15:26.092472 arxiv_bot-0.0.3/arxiv_bot/knowledge_base/__pycache__/database.cpython-311.pyc
--rw-r--r--   0        0        0     6626 2023-03-03 15:51:03.434969 arxiv_bot-0.0.3/arxiv_bot/knowledge_base/__pycache__/database.cpython-39.pyc
--rw-r--r--   0        0        0    16357 2023-03-18 08:26:23.667260 arxiv_bot-0.0.3/arxiv_bot/knowledge_base/constructors.py
--rw-r--r--   0        0        0     7915 2023-03-03 15:50:05.968405 arxiv_bot-0.0.3/arxiv_bot/knowledge_base/database.py
--rw-r--r--   0        0        0     1643 2023-02-27 10:51:36.468949 arxiv_bot-0.0.3/arxiv_bot/templates.py
--rw-r--r--   0        0        0      823 2023-03-18 08:27:38.129863 arxiv_bot-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 arxiv_bot-0.0.3/setup.py
--rw-r--r--   0        0        0      763 1970-01-01 00:00:00.000000 arxiv_bot-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       12 2023-02-05 03:03:40.410331 arxiv_bot-0.0.4/README.md
+-rw-r--r--   0        0        0      107 2023-03-01 06:15:05.389266 arxiv_bot-0.0.4/arxiv_bot/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-27 04:42:53.940169 arxiv_bot-0.0.4/arxiv_bot/knowledge_base/__init__.py
+-rw-r--r--   0        0        0      193 2023-02-27 10:27:55.374860 arxiv_bot-0.0.4/arxiv_bot/knowledge_base/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      175 2023-03-01 06:21:23.731532 arxiv_bot-0.0.4/arxiv_bot/knowledge_base/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    14645 2023-02-27 10:27:55.376048 arxiv_bot-0.0.4/arxiv_bot/knowledge_base/__pycache__/constructor.cpython-311.pyc
+-rw-r--r--   0        0        0    14741 2023-03-01 06:07:46.313553 arxiv_bot-0.0.4/arxiv_bot/knowledge_base/__pycache__/constructors.cpython-311.pyc
+-rw-r--r--   0        0        0    14290 2023-03-17 15:27:14.374433 arxiv_bot-0.0.4/arxiv_bot/knowledge_base/__pycache__/constructors.cpython-39.pyc
+-rw-r--r--   0        0        0    10129 2023-03-01 06:15:26.092472 arxiv_bot-0.0.4/arxiv_bot/knowledge_base/__pycache__/database.cpython-311.pyc
+-rw-r--r--   0        0        0     6626 2023-03-03 15:51:03.434969 arxiv_bot-0.0.4/arxiv_bot/knowledge_base/__pycache__/database.cpython-39.pyc
+-rw-r--r--   0        0        0    16354 2023-04-14 09:08:50.697609 arxiv_bot-0.0.4/arxiv_bot/knowledge_base/constructors.py
+-rw-r--r--   0        0        0     6955 2023-04-14 09:52:17.541131 arxiv_bot-0.0.4/arxiv_bot/knowledge_base/database.py
+-rw-r--r--   0        0        0        0 2023-04-14 05:45:40.130729 arxiv_bot-0.0.4/arxiv_bot/manager/bot.py
+-rw-r--r--   0        0        0     1643 2023-02-27 10:51:36.468949 arxiv_bot-0.0.4/arxiv_bot/templates.py
+-rw-r--r--   0        0        0      848 2023-04-15 11:57:17.214180 arxiv_bot-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      929 1970-01-01 00:00:00.000000 arxiv_bot-0.0.4/setup.py
+-rw-r--r--   0        0        0      809 1970-01-01 00:00:00.000000 arxiv_bot-0.0.4/PKG-INFO
```

### Comparing `arxiv_bot-0.0.3/arxiv_bot/knowledge_base/__pycache__/constructor.cpython-311.pyc` & `arxiv_bot-0.0.4/arxiv_bot/knowledge_base/__pycache__/constructor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `arxiv_bot-0.0.3/arxiv_bot/knowledge_base/__pycache__/constructors.cpython-311.pyc` & `arxiv_bot-0.0.4/arxiv_bot/knowledge_base/__pycache__/constructors.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `arxiv_bot-0.0.3/arxiv_bot/knowledge_base/__pycache__/constructors.cpython-39.pyc` & `arxiv_bot-0.0.4/arxiv_bot/knowledge_base/__pycache__/constructors.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `arxiv_bot-0.0.3/arxiv_bot/knowledge_base/__pycache__/database.cpython-311.pyc` & `arxiv_bot-0.0.4/arxiv_bot/knowledge_base/__pycache__/database.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `arxiv_bot-0.0.3/arxiv_bot/knowledge_base/__pycache__/database.cpython-39.pyc` & `arxiv_bot-0.0.4/arxiv_bot/knowledge_base/__pycache__/database.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `arxiv_bot-0.0.3/arxiv_bot/knowledge_base/constructors.py` & `arxiv_bot-0.0.4/arxiv_bot/knowledge_base/constructors.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             raise Exception(f'No paper found for query: {query}')
     return paper_id
 
 def init_extractor(
     template: str,
     openai_api_key: Union[str, None] = None,
     max_tokens: int = 1000,
-    chunk_size: int = 650,
+    chunk_size: int = 300,
     chunk_overlap: int = 40
 ):
     if openai_api_key is None and 'OPENAI_API_KEY' not in os.environ:
         raise Exception('No OpenAI API key provided')
     openai_api_key = openai_api_key or os.environ['OPENAI_API_KEY']
     # instantiate the OpenAI API wrapper
     llm = OpenAI(
@@ -100,15 +100,15 @@
     )
     text_splitter = tiktoken_splitter(
         chunk_size=chunk_size,
         chunk_overlap=chunk_overlap
     )
     return extractor, text_splitter
 
-def tiktoken_splitter(chunk_size=650, chunk_overlap=40):
+def tiktoken_splitter(chunk_size=300, chunk_overlap=40):
     tokenizer = tiktoken.get_encoding('p50k_base')
     # create length function
     def len_fn(text):
         tokens = tokenizer.encode(
             text, disallowed_special=()
         )
         return len(tokens)
@@ -283,15 +283,15 @@
         result = result[0]
         # remove 'v1', 'v2', etc. from the end of the pdf_url
         result.pdf_url = re.sub(r'v\d+$', '', result.pdf_url)
         self.authors = [author.name for author in result.authors]
         self.categories = result.categories
         self.comment = result.comment
         self.journal_ref = result.journal_ref
-        self.pdf_url = result.pdf_url
+        self.source = result.pdf_url
         self.primary_category = result.primary_category
         self.published = result.published.strftime('%Y%m%d')
         self.summary = result.summary
         self.title = result.title
         self.updated = result.updated.strftime('%Y%m%d')
         logging.debug(f"Downloaded metadata for paper '{self.id}'")
 
@@ -331,15 +331,15 @@
         :rtype: dict
         """
         fields = self.__dict__()
         # drop content field because it's big
         fields.pop('content')
         return fields
     
-    def chunker(self, chunk_size=650):
+    def chunker(self, chunk_size=300):
         # clean and split into initial smaller chunks
         clean_paper = self._clean_text(self.content)
         splitter = tiktoken_splitter(chunk_size=chunk_size)
         
         langchain_dataset = []
 
         paper_chunks = splitter.split_text(clean_paper)
@@ -357,15 +357,15 @@
         return text
 
     def __dict__(self):
         return {
             'id': self.id,
             'title': self.title,
             'summary': self.summary,
-            'pdf_url': self.pdf_url,
+            'source': self.source,
             'authors': self.authors,
             'categories': self.categories,
             'comment': self.comment,
             'journal_ref': self.journal_ref,
             'primary_category': self.primary_category,
             'published': self.published,
             'updated': self.updated,
```

### Comparing `arxiv_bot-0.0.3/arxiv_bot/knowledge_base/database.py` & `arxiv_bot-0.0.4/arxiv_bot/knowledge_base/database.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 from typing import Optional
 from uuid import uuid4
 from tqdm.auto import tqdm
 
 import torch
 from transformers import AutoTokenizer, AutoModelForMaskedLM
+from pinecone_text.sparse.splade_encoder import SpladeEncoder
 
 import pinecone
 import openai
 
 
 dense_models = {
     'text-embedding-ada-002': {
@@ -165,47 +166,23 @@
     def __init__(
         self,
         model_name: Optional[str] = 'naver/splade-cocondenser-ensembledistil',
         device: Optional[str] = None
     ):
         # initialize model
         self.device = device or ('cuda' if torch.cuda.is_available() else 'cpu')
-        self.model = AutoModelForMaskedLM.from_pretrained(model_name)
-        # move to cuda if enabled
-        self.model.to(self.device)
-        # set to inference mode
-        self.model.eval()
-        # initialize tokenizer
-        self.tokenizer = AutoTokenizer.from_pretrained(model_name)
+        self.model = SpladeEncoder(device=device)
 
     def __call__(self, texts: list):
         if type(texts) == str:
             texts = [texts]
-        # tokenize
-        tokens = self.tokenizer(
-            texts, add_special_tokens=False,
-            return_tensors='pt', truncation=True,
-            padding=True
-        ).to(self.device)
-        # create sparse embedding
-        with torch.no_grad():
-            output = self.model(**tokens)
-            sparse_emb = torch.max(
-                torch.log(
-                    1 + torch.relu(output.logits)
-                ) * tokens.attention_mask.unsqueeze(-1),
-            dim=1)[0].squeeze()
-        # extract indices and their values
-        indices = []
-        values = []
-        for i in range(sparse_emb.shape[0]):
-            indices.append(sparse_emb[i].nonzero().squeeze().cpu().tolist())
-            values.append(sparse_emb[i][indices[i]].cpu().tolist())
+        # encode
+        embeds = self.model.encode_documents(texts)
         # return sparse embedding in pinecone format
-        return [{'indices': idx, 'values': vals} for idx, vals in zip(indices, values)]
+        return embeds
 
 class DenseOpenAI:
     def __init__(self, model_name: str, api_key: Optional[str] = None):
         self.api_key = api_key or os.environ['OPENAI_API_KEY']
         self.model_name = model_name
     
     def __call__(self, texts: list):
```

### Comparing `arxiv_bot-0.0.3/arxiv_bot/templates.py` & `arxiv_bot-0.0.4/arxiv_bot/templates.py`

 * *Files identical despite different names*

### Comparing `arxiv_bot-0.0.3/pyproject.toml` & `arxiv_bot-0.0.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arxiv-bot"
-version = "0.0.3"
+version = "0.0.4"
 description = "ArXiv component of AI assistant"
 authors = ["James Briggs <james@aurelio.ai>"]
 readme = "README.md"
 packages = [
     {include = "arxiv_bot"},
     {include = "arxiv_bot/knowledge_base"}
 ]
@@ -15,14 +15,15 @@
 arxiv = "^1.4.3"
 pypdf2 = "^3.0.1"
 openai = "^0.26.5"
 pinecone-client = ">=2.2.1,<3.0"
 tiktoken = "^0.2.0"
 transformers = "^4.26.1"
 tqdm = "^4.64.1"
+pinecone-text = "^0.4.2"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.hatch.version]
```

### Comparing `arxiv_bot-0.0.3/setup.py` & `arxiv_bot-0.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['arxiv_bot', 'arxiv_bot.knowledge_base', 'knowledge_base']
+['arxiv_bot', 'arxiv_bot.knowledge_base', 'arxiv_bot.manager', 'knowledge_base']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['arxiv>=1.4.3,<2.0.0',
  'langchain>=0.0.96,<0.0.97',
  'openai>=0.26.5,<0.27.0',
  'pinecone-client>=2.2.1,<3.0',
+ 'pinecone-text>=0.4.2,<0.5.0',
  'pypdf2>=3.0.1,<4.0.0',
  'tiktoken>=0.2.0,<0.3.0',
  'tqdm>=4.64.1,<5.0.0',
  'transformers>=4.26.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'arxiv-bot',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': 'ArXiv component of AI assistant',
     'long_description': '# Arxiv Bot\n',
     'author': 'James Briggs',
     'author_email': 'james@aurelio.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `arxiv_bot-0.0.3/PKG-INFO` & `arxiv_bot-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: arxiv-bot
-Version: 0.0.3
+Version: 0.0.4
 Summary: ArXiv component of AI assistant
 Author: James Briggs
 Author-email: james@aurelio.ai
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arxiv (>=1.4.3,<2.0.0)
 Requires-Dist: langchain (>=0.0.96,<0.0.97)
 Requires-Dist: openai (>=0.26.5,<0.27.0)
 Requires-Dist: pinecone-client (>=2.2.1,<3.0)
+Requires-Dist: pinecone-text (>=0.4.2,<0.5.0)
 Requires-Dist: pypdf2 (>=3.0.1,<4.0.0)
 Requires-Dist: tiktoken (>=0.2.0,<0.3.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Requires-Dist: transformers (>=4.26.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Arxiv Bot
```

