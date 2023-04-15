# Comparing `tmp/llama_api_server-0.2.0.tar.gz` & `tmp/llama_api_server-0.2.1.tar.gz`

## Comparing `llama_api_server-0.2.0.tar` & `llama_api_server-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/.gitattributes
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/Makefile
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/SECURITY.md
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/requirements.txt
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/version.txt
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/llama_api_server/__init__.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/llama_api_server/__main__.py
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/llama_api_server/app.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/llama_api_server/config.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/llama_api_server/model_pool.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/llama_api_server/utils.py
--rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/llama_api_server/models/llama_cpp.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/llama_api_server/models/pyllama.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/llama_api_server/models/pyllama_quant.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/LICENSE
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/README.md
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 llama_api_server-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/.gitattributes
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/Makefile
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/SECURITY.md
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/requirements.txt
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/version.txt
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/llama_api_server/__init__.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/llama_api_server/__main__.py
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/llama_api_server/app.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/llama_api_server/config.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/llama_api_server/model_pool.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/llama_api_server/utils.py
+-rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/llama_api_server/models/llama_cpp.py
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/llama_api_server/models/pyllama.py
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/llama_api_server/models/pyllama_quant.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/README.md
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/PKG-INFO
```

### Comparing `llama_api_server-0.2.0/SECURITY.md` & `llama_api_server-0.2.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.2.0/requirements.txt` & `llama_api_server-0.2.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.2.0/.github/FUNDING.yml` & `llama_api_server-0.2.1/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md` & `llama_api_server-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md` & `llama_api_server-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.2.0/.github/workflows/release.yml` & `llama_api_server-0.2.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.2.0/llama_api_server/app.py` & `llama_api_server-0.2.1/llama_api_server/app.py`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.2.0/llama_api_server/model_pool.py` & `llama_api_server-0.2.1/llama_api_server/model_pool.py`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.2.0/llama_api_server/models/llama_cpp.py` & `llama_api_server-0.2.1/llama_api_server/models/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.2.0/llama_api_server/models/pyllama.py` & `llama_api_server-0.2.1/llama_api_server/models/pyllama.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         except ImportError:
             raise ImportError(
                 'To run model with pyllama, please run "python -m pip install pyllama transformers" first'
             )
         local_rank = 0
         world_size = 1
         max_seq_len = params.get("max_seq_len", None) or 2048
-        max_batch_size = params.get("max_batch_size", None) or 16
+        max_batch_size = params.get("max_batch_size", None) or 2
         ckpt_dir = params["ckpt_dir"]
         tokenizer_path = params["tokenizer_path"]
         device = params.get("device", "cuda")
         checkpoints = sorted(Path(ckpt_dir).glob("*.pth"))
         assert world_size == len(
             checkpoints
         ), f"Loading a checkpoint for MP={len(checkpoints)} but world size is {world_size}"
@@ -49,18 +49,17 @@
     def completions(self, args):
         prompt = args["prompt"]
         top_p = args["top_p"]
         suffix = args["suffix"]
         echo = args["echo"]
         temp = args["temperature"]
         max_tokens = args["max_tokens"]
-        result = prompt if echo else ""
-        result += self.model.generate(
+        result = self.model.generate(
             [prompt], max_gen_len=max_tokens, temperature=temp, top_p=top_p
-        )
+        )[0]
         finish_reason = "length"
         c_prompt_tokens = n_past = 0
         return {
             "id": get_uuid(),
             "object": "text_completion",
             "created": get_timestamp(),
             "model": args["model"],
```

### Comparing `llama_api_server-0.2.0/llama_api_server/models/pyllama_quant.py` & `llama_api_server-0.2.1/llama_api_server/models/pyllama_quant.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,28 +32,27 @@
 
         prompt = args["prompt"]
         top_p = args["top_p"]
         suffix = args["suffix"]
         echo = args["echo"]
         temp = args["temperature"]
         max_tokens = args["max_tokens"]
-        result = prompt if echo else ""
 
         input_ids = self.tokenizer.encode(prompt, return_tensors="pt").to(self.dev)
 
         with torch.no_grad():
             generated_ids = self.model.generate(
                 input_ids,
                 do_sample=True,
                 min_length=1,
-                max_length=max_tokens,
+                max_new_tokens=max_tokens,
                 top_p=top_p,
                 temperature=temp,
             )
-        result += self.tokenizer.decode([el.item() for el in generated_ids[0]])
+        result = self.tokenizer.decode([el.item() for el in generated_ids[0]])
         finish_reason = "length"
         c_prompt_tokens = len(input_ids)
         c_completion_tokens = len(generated_ids)
         return {
             "id": get_uuid(),
             "object": "text_completion",
             "created": get_timestamp(),
```

### Comparing `llama_api_server-0.2.0/.gitignore` & `llama_api_server-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.2.0/LICENSE` & `llama_api_server-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.2.0/README.md` & `llama_api_server-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-llama-api-server
+🎭🦙 llama-api-server
 =======
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Release](https://github.com/iaalm/llama-api-server/actions/workflows/release.yml/badge.svg)](https://github.com/iaalm/llama-api-server/actions/workflows/release.yml)
 
 This project is under active deployment. Breaking changes could be made any time.
 
 Llama as a Service! This project try to build a REST-ful API server compatible to OpenAI API using open source backends like llama.
 
-## Get started
+# 🚀Get started
 
-### Prepare model
+## Prepare model
 
-#### llama.cpp
+### llama.cpp
 If you you don't have quantized llama.cpp, you need to follow [instruction](https://github.com/ggerganov/llama.cpp#usage) to prepare model.
 
-#### pyllama
+### pyllama
 If you you don't have quantize pyllama, you need to follow [instruction](https://github.com/juncongmoo/pyllama#-quantize-llama-to-run-in-a-4gb-gpu) to prepare model.
 
 
-### Install
+## Install
 ```
 pip install llama-api-server
 
 # to run wth pyllama
 pip install llama-api-server[pyllama]
 
 echo > config.yml << EOF
@@ -38,64 +38,67 @@
       params:
         path: /absolute/path/to/your/pyllama-7B4b.pt
     text-davinci-003:
       type: pyllama
       params:
         ckpt_dir: /absolute/path/to/your/7B/
         tokenizer_path: /absolute/path/to/your/tokenizer.model
+      # keep to 1 instance to speed up loading of model
+      min_instance: 1
+      max_instance: 1
   embeddings:
     text-embedding-ada-002:
       type: llama_cpp
       params:
         path: /absolute/path/to/your/7B/ggml-model-q4_0.bin
 EOF
 
 echo "SOME_TOKEN" > tokens.txt
 
 # start web server
 python -m llama_api_server
 ```
 
-### Call with openai-python
+## Call with openai-python
 ```
 export OPENAI_API_KEY=SOME_TOKEN
 export OPENAI_API_BASE=http://127.0.0.1:5000/v1
 
 openai api completions.create -e text-ada-002 -p "hello?"
 
 curl -X POST http://127.0.0.1:5000/v1/embeddings -H 'Content-Type: application/json' -d '{"model":"text-embedding-ada-002", "input":"It is good."}'  -H "Authorization: Bearer SOME_TOKEN"
 ```
 
-## Roadmap
+# 🛣️Roadmap
 
-#### Tested with
+### Tested with
 - [X] openai-python
     - [X] OPENAI\_API\_TYPE=default
     - [X] OPENAI\_API\_TYPE=azure
 
-#### Supported APIs
+### Supported APIs
 - [X] Completions
     - [X] set `temperature`, `top_p`, and `top_k`
     - [X] set `max_tokens`
     - [ ] set `stop`
     - [ ] set `stream`
     - [ ] set `n`
     - [ ] set `presence_penalty` and `frequency_penalty`
     - [ ] set `logit_bias`
 - [X] Embeddings
     - [X] batch process
 - [ ] Chat
 - [ ] List model
 
-#### Supported backed
+### Supported backends
 - [X] [llama.cpp](https://github.com/ggerganov/llama.cpp) via [llamacpp-python](https://github.com/thomasantony/llamacpp-python)
 - [X] [llama](https://github.com/facebookresearch/llama) via [pyllama](https://github.com/juncongmoo/pyllama)
     - [X] Without Quantization
     - [X] With Quantization
 
-#### Others
+### Others
 - [X] Performance parameters like `n_batch` and `n_thread`
 - [X] Token auth
 - [ ] Documents
 - [ ] Intergration tests
 - [ ] A tool to download/prepare pretrain model
 - [ ] Make config.ini and token file configable
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `llama_api_server-0.2.0/pyproject.toml` & `llama_api_server-0.2.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "llama_api_server"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = [
     {name = "iaalm", email= "iaalmsimon@gmail.com"}
 ]
 license = {text = "MIT"}
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `llama_api_server-0.2.0/PKG-INFO` & `llama_api_server-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama_api_server
-Version: 0.2.0
+Version: 0.2.1
 Project-URL: homepage, https://github.com/iaalm/llama-api-server
 Project-URL: repository, https://github.com/iaalm/llama-api-server
 Author-email: iaalm <iaalmsimon@gmail.com>
 License: MIT
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -20,36 +20,36 @@
 Requires-Dist: numpy
 Requires-Dist: pyyaml
 Provides-Extra: pyllama
 Requires-Dist: pyllama>=0.0.9; extra == 'pyllama'
 Requires-Dist: transformers>=4.27.4; extra == 'pyllama'
 Description-Content-Type: text/markdown
 
-llama-api-server
+🎭🦙 llama-api-server
 =======
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Release](https://github.com/iaalm/llama-api-server/actions/workflows/release.yml/badge.svg)](https://github.com/iaalm/llama-api-server/actions/workflows/release.yml)
 
 This project is under active deployment. Breaking changes could be made any time.
 
 Llama as a Service! This project try to build a REST-ful API server compatible to OpenAI API using open source backends like llama.
 
-## Get started
+# 🚀Get started
 
-### Prepare model
+## Prepare model
 
-#### llama.cpp
+### llama.cpp
 If you you don't have quantized llama.cpp, you need to follow [instruction](https://github.com/ggerganov/llama.cpp#usage) to prepare model.
 
-#### pyllama
+### pyllama
 If you you don't have quantize pyllama, you need to follow [instruction](https://github.com/juncongmoo/pyllama#-quantize-llama-to-run-in-a-4gb-gpu) to prepare model.
 
 
-### Install
+## Install
 ```
 pip install llama-api-server
 
 # to run wth pyllama
 pip install llama-api-server[pyllama]
 
 echo > config.yml << EOF
@@ -64,64 +64,67 @@
       params:
         path: /absolute/path/to/your/pyllama-7B4b.pt
     text-davinci-003:
       type: pyllama
       params:
         ckpt_dir: /absolute/path/to/your/7B/
         tokenizer_path: /absolute/path/to/your/tokenizer.model
+      # keep to 1 instance to speed up loading of model
+      min_instance: 1
+      max_instance: 1
   embeddings:
     text-embedding-ada-002:
       type: llama_cpp
       params:
         path: /absolute/path/to/your/7B/ggml-model-q4_0.bin
 EOF
 
 echo "SOME_TOKEN" > tokens.txt
 
 # start web server
 python -m llama_api_server
 ```
 
-### Call with openai-python
+## Call with openai-python
 ```
 export OPENAI_API_KEY=SOME_TOKEN
 export OPENAI_API_BASE=http://127.0.0.1:5000/v1
 
 openai api completions.create -e text-ada-002 -p "hello?"
 
 curl -X POST http://127.0.0.1:5000/v1/embeddings -H 'Content-Type: application/json' -d '{"model":"text-embedding-ada-002", "input":"It is good."}'  -H "Authorization: Bearer SOME_TOKEN"
 ```
 
-## Roadmap
+# 🛣️Roadmap
 
-#### Tested with
+### Tested with
 - [X] openai-python
     - [X] OPENAI\_API\_TYPE=default
     - [X] OPENAI\_API\_TYPE=azure
 
-#### Supported APIs
+### Supported APIs
 - [X] Completions
     - [X] set `temperature`, `top_p`, and `top_k`
     - [X] set `max_tokens`
     - [ ] set `stop`
     - [ ] set `stream`
     - [ ] set `n`
     - [ ] set `presence_penalty` and `frequency_penalty`
     - [ ] set `logit_bias`
 - [X] Embeddings
     - [X] batch process
 - [ ] Chat
 - [ ] List model
 
-#### Supported backed
+### Supported backends
 - [X] [llama.cpp](https://github.com/ggerganov/llama.cpp) via [llamacpp-python](https://github.com/thomasantony/llamacpp-python)
 - [X] [llama](https://github.com/facebookresearch/llama) via [pyllama](https://github.com/juncongmoo/pyllama)
     - [X] Without Quantization
     - [X] With Quantization
 
-#### Others
+### Others
 - [X] Performance parameters like `n_batch` and `n_thread`
 - [X] Token auth
 - [ ] Documents
 - [ ] Intergration tests
 - [ ] A tool to download/prepare pretrain model
 - [ ] Make config.ini and token file configable
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

