# Comparing `tmp/rwkv-paddle-0.7.3.tar.gz` & `tmp/rwkv-paddle-0.7.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwkv-paddle-0.7.3.tar", last modified: Sat Apr 15 08:23:51 2023, max compression
+gzip compressed data, was "rwkv-paddle-0.7.3.1.tar", last modified: Sat Apr 15 08:57:33 2023, max compression
```

## Comparing `rwkv-paddle-0.7.3.tar` & `rwkv-paddle-0.7.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 wsl       (1000) wsl       (1000)        0 2023-04-15 08:23:51.901076 rwkv-paddle-0.7.3/
--rwxrwxrwx   0 wsl       (1000) wsl       (1000)    11357 2023-04-15 08:23:25.000000 rwkv-paddle-0.7.3/LICENSE
--rwxrwxrwx   0 wsl       (1000) wsl       (1000)       31 2023-04-15 08:23:25.000000 rwkv-paddle-0.7.3/MANIFEST.in
--rwxrwxrwx   0 wsl       (1000) wsl       (1000)     5094 2023-04-15 08:23:51.898070 rwkv-paddle-0.7.3/PKG-INFO
--rwxrwxrwx   0 wsl       (1000) wsl       (1000)     4595 2023-04-15 08:23:25.000000 rwkv-paddle-0.7.3/README.md
--rwxrwxrwx   0 wsl       (1000) wsl       (1000)      528 2023-04-15 08:23:25.000000 rwkv-paddle-0.7.3/pyproject.toml
--rwxrwxrwx   0 wsl       (1000) wsl       (1000)       38 2023-04-15 08:23:51.902077 rwkv-paddle-0.7.3/setup.cfg
-drwxrwxrwx   0 wsl       (1000) wsl       (1000)        0 2023-04-15 08:23:51.725833 rwkv-paddle-0.7.3/src/
-drwxrwxrwx   0 wsl       (1000) wsl       (1000)        0 2023-04-15 08:23:51.798916 rwkv-paddle-0.7.3/src/rwkv_paddle/
--rwxrwxrwx   0 wsl       (1000) wsl       (1000)        0 2023-04-15 08:23:25.000000 rwkv-paddle-0.7.3/src/rwkv_paddle/__init__.py
-drwxrwxrwx   0 wsl       (1000) wsl       (1000)        0 2023-04-15 08:23:51.887546 rwkv-paddle-0.7.3/src/rwkv_paddle/cuda/
--rwxrwxrwx   0 wsl       (1000) wsl       (1000)     4996 2023-04-15 08:23:25.000000 rwkv-paddle-0.7.3/src/rwkv_paddle/cuda/operators.cu
--rwxrwxrwx   0 wsl       (1000) wsl       (1000)     6222 2023-04-15 08:23:25.000000 rwkv-paddle-0.7.3/src/rwkv_paddle/cuda/wrapper.cpp
--rwxrwxrwx   0 wsl       (1000) wsl       (1000)    33465 2023-04-15 08:23:25.000000 rwkv-paddle-0.7.3/src/rwkv_paddle/model.py
--rwxrwxrwx   0 wsl       (1000) wsl       (1000)     6850 2023-04-15 08:23:25.000000 rwkv-paddle-0.7.3/src/rwkv_paddle/serialization.py
--rwxrwxrwx   0 wsl       (1000) wsl       (1000)     4898 2023-04-15 08:23:25.000000 rwkv-paddle-0.7.3/src/rwkv_paddle/utils.py
-drwxrwxrwx   0 wsl       (1000) wsl       (1000)        0 2023-04-15 08:23:51.855546 rwkv-paddle-0.7.3/src/rwkv_paddle.egg-info/
--rwxrwxrwx   0 wsl       (1000) wsl       (1000)     5094 2023-04-15 08:23:51.000000 rwkv-paddle-0.7.3/src/rwkv_paddle.egg-info/PKG-INFO
--rwxrwxrwx   0 wsl       (1000) wsl       (1000)      416 2023-04-15 08:23:51.000000 rwkv-paddle-0.7.3/src/rwkv_paddle.egg-info/SOURCES.txt
--rwxrwxrwx   0 wsl       (1000) wsl       (1000)        1 2023-04-15 08:23:51.000000 rwkv-paddle-0.7.3/src/rwkv_paddle.egg-info/dependency_links.txt
--rwxrwxrwx   0 wsl       (1000) wsl       (1000)       19 2023-04-15 08:23:51.000000 rwkv-paddle-0.7.3/src/rwkv_paddle.egg-info/requires.txt
--rwxrwxrwx   0 wsl       (1000) wsl       (1000)       12 2023-04-15 08:23:51.000000 rwkv-paddle-0.7.3/src/rwkv_paddle.egg-info/top_level.txt
+drwxrwxrwx   0 wsl       (1000) wsl       (1000)        0 2023-04-15 08:57:33.007759 rwkv-paddle-0.7.3.1/
+-rwxrwxrwx   0 wsl       (1000) wsl       (1000)    11357 2023-04-15 08:23:25.000000 rwkv-paddle-0.7.3.1/LICENSE
+-rwxrwxrwx   0 wsl       (1000) wsl       (1000)       31 2023-04-15 08:23:25.000000 rwkv-paddle-0.7.3.1/MANIFEST.in
+-rwxrwxrwx   0 wsl       (1000) wsl       (1000)     5122 2023-04-15 08:57:33.004758 rwkv-paddle-0.7.3.1/PKG-INFO
+-rwxrwxrwx   0 wsl       (1000) wsl       (1000)     4621 2023-04-15 08:57:23.000000 rwkv-paddle-0.7.3.1/README.md
+-rwxrwxrwx   0 wsl       (1000) wsl       (1000)      530 2023-04-15 08:57:23.000000 rwkv-paddle-0.7.3.1/pyproject.toml
+-rwxrwxrwx   0 wsl       (1000) wsl       (1000)       38 2023-04-15 08:57:33.007759 rwkv-paddle-0.7.3.1/setup.cfg
+drwxrwxrwx   0 wsl       (1000) wsl       (1000)        0 2023-04-15 08:57:32.809489 rwkv-paddle-0.7.3.1/src/
+drwxrwxrwx   0 wsl       (1000) wsl       (1000)        0 2023-04-15 08:57:32.888028 rwkv-paddle-0.7.3.1/src/rwkv_paddle/
+-rwxrwxrwx   0 wsl       (1000) wsl       (1000)        0 2023-04-15 08:23:25.000000 rwkv-paddle-0.7.3.1/src/rwkv_paddle/__init__.py
+drwxrwxrwx   0 wsl       (1000) wsl       (1000)        0 2023-04-15 08:57:32.986759 rwkv-paddle-0.7.3.1/src/rwkv_paddle/cuda/
+-rwxrwxrwx   0 wsl       (1000) wsl       (1000)     4996 2023-04-15 08:23:25.000000 rwkv-paddle-0.7.3.1/src/rwkv_paddle/cuda/operators.cu
+-rwxrwxrwx   0 wsl       (1000) wsl       (1000)     6222 2023-04-15 08:23:25.000000 rwkv-paddle-0.7.3.1/src/rwkv_paddle/cuda/wrapper.cpp
+-rwxrwxrwx   0 wsl       (1000) wsl       (1000)    33465 2023-04-15 08:23:25.000000 rwkv-paddle-0.7.3.1/src/rwkv_paddle/model.py
+-rwxrwxrwx   0 wsl       (1000) wsl       (1000)     6850 2023-04-15 08:23:25.000000 rwkv-paddle-0.7.3.1/src/rwkv_paddle/serialization.py
+-rwxrwxrwx   0 wsl       (1000) wsl       (1000)     4898 2023-04-15 08:23:25.000000 rwkv-paddle-0.7.3.1/src/rwkv_paddle/utils.py
+drwxrwxrwx   0 wsl       (1000) wsl       (1000)        0 2023-04-15 08:57:32.954198 rwkv-paddle-0.7.3.1/src/rwkv_paddle.egg-info/
+-rwxrwxrwx   0 wsl       (1000) wsl       (1000)     5122 2023-04-15 08:57:32.000000 rwkv-paddle-0.7.3.1/src/rwkv_paddle.egg-info/PKG-INFO
+-rwxrwxrwx   0 wsl       (1000) wsl       (1000)      416 2023-04-15 08:57:32.000000 rwkv-paddle-0.7.3.1/src/rwkv_paddle.egg-info/SOURCES.txt
+-rwxrwxrwx   0 wsl       (1000) wsl       (1000)        1 2023-04-15 08:57:32.000000 rwkv-paddle-0.7.3.1/src/rwkv_paddle.egg-info/dependency_links.txt
+-rwxrwxrwx   0 wsl       (1000) wsl       (1000)       19 2023-04-15 08:57:32.000000 rwkv-paddle-0.7.3.1/src/rwkv_paddle.egg-info/requires.txt
+-rwxrwxrwx   0 wsl       (1000) wsl       (1000)       12 2023-04-15 08:57:32.000000 rwkv-paddle-0.7.3.1/src/rwkv_paddle.egg-info/top_level.txt
```

### Comparing `rwkv-paddle-0.7.3/LICENSE` & `rwkv-paddle-0.7.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rwkv-paddle-0.7.3/PKG-INFO` & `rwkv-paddle-0.7.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwkv-paddle
-Version: 0.7.3
+Version: 0.7.3.1
 Summary: The RWKV Language Model on PaddlePaddle
 Author: HighCWu
 Project-URL: Homepage, https://github.com/HighCWu/rwkv-paddle
 Project-URL: Bug Tracker, https://github.com/HighCWu/rwkv-paddle/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -18,17 +18,19 @@
 
 https://github.com/BlinkDL/ChatRWKV
 
 https://github.com/BlinkDL/RWKV-LM
 
 PS: Some strategies are not supported on PaddlePaddle. The best supported strategies are 'cuda fp16' and 'cpu fp32'.
 
-PS: PaddlePaddle version should be greater than 2.4.0
+PS: PaddlePaddle version should be greater than 2.4.0.
 
 ```python
+import os
+
 # set these before import RWKV
 os.environ['RWKV_JIT_ON'] = '0' # RWKV JIT Mode is not supported on paddlepaddle now
 os.environ["RWKV_CUDA_ON"] = '0' # '1' to compile CUDA kernel (10x faster), requires c++ compiler & cuda libraries
 
 ########################################################################################################
 #
 # Use '/' in model path, instead of '\'. Use ctx4096 models if you need long ctx.
@@ -63,16 +65,16 @@
 # 'cuda fp16i8 *10+' = first 10 layers cuda fp16i8, then fp16i8 stream the rest to it (increase 10 for better speed)
 #
 # Extreme STREAM: 3G VRAM is enough to run RWKV 14B (slow. will be faster in future)
 # 'cuda fp16i8 *0+ -> cpu fp32 *1' = stream all layers cuda fp16i8, last 1 layer [ln_out+head] cpu fp32
 #
 # ########################################################################################################
 
-from rwkv.model import RWKV
-from rwkv.utils import PIPELINE, PIPELINE_ARGS
+from rwkv_paddle.model import RWKV
+from rwkv_paddle.utils import PIPELINE, PIPELINE_ARGS
 
 # download models: https://huggingface.co/BlinkDL
 model = RWKV(model='/fsx/BlinkDL/HF-MODEL/rwkv-4-pile-169m/RWKV-4-Pile-169M-20220807-8023', strategy='cpu fp32')
 pipeline = PIPELINE(model, "20B_tokenizer.json") # 20B_tokenizer.json is in https://github.com/HighCWu/rwkv-paddle
 
 ctx = "\nIn a shocking finding, scientist discovered a herd of dragons living in a remote, previously unexplored valley, in Tibet. Even more surprising to the researchers was the fact that the dragons spoke perfect Chinese."
 print(ctx, end='')
```

### Comparing `rwkv-paddle-0.7.3/README.md` & `rwkv-paddle-0.7.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 
 https://github.com/BlinkDL/ChatRWKV
 
 https://github.com/BlinkDL/RWKV-LM
 
 PS: Some strategies are not supported on PaddlePaddle. The best supported strategies are 'cuda fp16' and 'cpu fp32'.
 
-PS: PaddlePaddle version should be greater than 2.4.0
+PS: PaddlePaddle version should be greater than 2.4.0.
 
 ```python
+import os
+
 # set these before import RWKV
 os.environ['RWKV_JIT_ON'] = '0' # RWKV JIT Mode is not supported on paddlepaddle now
 os.environ["RWKV_CUDA_ON"] = '0' # '1' to compile CUDA kernel (10x faster), requires c++ compiler & cuda libraries
 
 ########################################################################################################
 #
 # Use '/' in model path, instead of '\'. Use ctx4096 models if you need long ctx.
@@ -49,16 +51,16 @@
 # 'cuda fp16i8 *10+' = first 10 layers cuda fp16i8, then fp16i8 stream the rest to it (increase 10 for better speed)
 #
 # Extreme STREAM: 3G VRAM is enough to run RWKV 14B (slow. will be faster in future)
 # 'cuda fp16i8 *0+ -> cpu fp32 *1' = stream all layers cuda fp16i8, last 1 layer [ln_out+head] cpu fp32
 #
 # ########################################################################################################
 
-from rwkv.model import RWKV
-from rwkv.utils import PIPELINE, PIPELINE_ARGS
+from rwkv_paddle.model import RWKV
+from rwkv_paddle.utils import PIPELINE, PIPELINE_ARGS
 
 # download models: https://huggingface.co/BlinkDL
 model = RWKV(model='/fsx/BlinkDL/HF-MODEL/rwkv-4-pile-169m/RWKV-4-Pile-169M-20220807-8023', strategy='cpu fp32')
 pipeline = PIPELINE(model, "20B_tokenizer.json") # 20B_tokenizer.json is in https://github.com/HighCWu/rwkv-paddle
 
 ctx = "\nIn a shocking finding, scientist discovered a herd of dragons living in a remote, previously unexplored valley, in Tibet. Even more surprising to the researchers was the fact that the dragons spoke perfect Chinese."
 print(ctx, end='')
```

### Comparing `rwkv-paddle-0.7.3/pyproject.toml` & `rwkv-paddle-0.7.3.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rwkv-paddle"
-version = "0.7.3"
+version = "0.7.3.1"
 authors = [
   { name="HighCWu" },
 ]
 description = "The RWKV Language Model on PaddlePaddle"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `rwkv-paddle-0.7.3/src/rwkv_paddle/cuda/operators.cu` & `rwkv-paddle-0.7.3.1/src/rwkv_paddle/cuda/operators.cu`

 * *Files identical despite different names*

### Comparing `rwkv-paddle-0.7.3/src/rwkv_paddle/cuda/wrapper.cpp` & `rwkv-paddle-0.7.3.1/src/rwkv_paddle/cuda/wrapper.cpp`

 * *Files identical despite different names*

### Comparing `rwkv-paddle-0.7.3/src/rwkv_paddle/model.py` & `rwkv-paddle-0.7.3.1/src/rwkv_paddle/model.py`

 * *Files identical despite different names*

### Comparing `rwkv-paddle-0.7.3/src/rwkv_paddle/serialization.py` & `rwkv-paddle-0.7.3.1/src/rwkv_paddle/serialization.py`

 * *Files identical despite different names*

### Comparing `rwkv-paddle-0.7.3/src/rwkv_paddle/utils.py` & `rwkv-paddle-0.7.3.1/src/rwkv_paddle/utils.py`

 * *Files identical despite different names*

### Comparing `rwkv-paddle-0.7.3/src/rwkv_paddle.egg-info/PKG-INFO` & `rwkv-paddle-0.7.3.1/src/rwkv_paddle.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwkv-paddle
-Version: 0.7.3
+Version: 0.7.3.1
 Summary: The RWKV Language Model on PaddlePaddle
 Author: HighCWu
 Project-URL: Homepage, https://github.com/HighCWu/rwkv-paddle
 Project-URL: Bug Tracker, https://github.com/HighCWu/rwkv-paddle/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -18,17 +18,19 @@
 
 https://github.com/BlinkDL/ChatRWKV
 
 https://github.com/BlinkDL/RWKV-LM
 
 PS: Some strategies are not supported on PaddlePaddle. The best supported strategies are 'cuda fp16' and 'cpu fp32'.
 
-PS: PaddlePaddle version should be greater than 2.4.0
+PS: PaddlePaddle version should be greater than 2.4.0.
 
 ```python
+import os
+
 # set these before import RWKV
 os.environ['RWKV_JIT_ON'] = '0' # RWKV JIT Mode is not supported on paddlepaddle now
 os.environ["RWKV_CUDA_ON"] = '0' # '1' to compile CUDA kernel (10x faster), requires c++ compiler & cuda libraries
 
 ########################################################################################################
 #
 # Use '/' in model path, instead of '\'. Use ctx4096 models if you need long ctx.
@@ -63,16 +65,16 @@
 # 'cuda fp16i8 *10+' = first 10 layers cuda fp16i8, then fp16i8 stream the rest to it (increase 10 for better speed)
 #
 # Extreme STREAM: 3G VRAM is enough to run RWKV 14B (slow. will be faster in future)
 # 'cuda fp16i8 *0+ -> cpu fp32 *1' = stream all layers cuda fp16i8, last 1 layer [ln_out+head] cpu fp32
 #
 # ########################################################################################################
 
-from rwkv.model import RWKV
-from rwkv.utils import PIPELINE, PIPELINE_ARGS
+from rwkv_paddle.model import RWKV
+from rwkv_paddle.utils import PIPELINE, PIPELINE_ARGS
 
 # download models: https://huggingface.co/BlinkDL
 model = RWKV(model='/fsx/BlinkDL/HF-MODEL/rwkv-4-pile-169m/RWKV-4-Pile-169M-20220807-8023', strategy='cpu fp32')
 pipeline = PIPELINE(model, "20B_tokenizer.json") # 20B_tokenizer.json is in https://github.com/HighCWu/rwkv-paddle
 
 ctx = "\nIn a shocking finding, scientist discovered a herd of dragons living in a remote, previously unexplored valley, in Tibet. Even more surprising to the researchers was the fact that the dragons spoke perfect Chinese."
 print(ctx, end='')
```

