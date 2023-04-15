# Comparing `tmp/CoLT5-attention-0.2.0.tar.gz` & `tmp/CoLT5-attention-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoLT5-attention-0.2.0.tar", last modified: Sat Apr 15 15:09:05 2023, max compression
+gzip compressed data, was "CoLT5-attention-0.2.1.tar", last modified: Sat Apr 15 18:12:30 2023, max compression
```

## Comparing `CoLT5-attention-0.2.0.tar` & `CoLT5-attention-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:09:05.364228 CoLT5-attention-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:09:05.360228 CoLT5-attention-0.2.0/CoLT5_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-15 15:09:05.000000 CoLT5-attention-0.2.0/CoLT5_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-15 15:09:05.000000 CoLT5-attention-0.2.0/CoLT5_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 15:09:05.000000 CoLT5-attention-0.2.0/CoLT5_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-15 15:09:05.000000 CoLT5-attention-0.2.0/CoLT5_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-15 15:09:05.000000 CoLT5-attention-0.2.0/CoLT5_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-15 15:08:45.000000 CoLT5-attention-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-15 15:09:05.364228 CoLT5-attention-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-04-15 15:08:45.000000 CoLT5-attention-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:09:05.364228 CoLT5-attention-0.2.0/colt5_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-15 15:08:45.000000 CoLT5-attention-0.2.0/colt5_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-15 15:08:45.000000 CoLT5-attention-0.2.0/colt5_attention/coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-15 15:08:45.000000 CoLT5-attention-0.2.0/colt5_attention/sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)    19307 2023-04-15 15:08:45.000000 CoLT5-attention-0.2.0/colt5_attention/transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 15:09:05.364228 CoLT5-attention-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-15 15:08:45.000000 CoLT5-attention-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:12:30.292684 CoLT5-attention-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:12:30.292684 CoLT5-attention-0.2.1/CoLT5_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-15 18:12:30.000000 CoLT5-attention-0.2.1/CoLT5_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-15 18:12:30.000000 CoLT5-attention-0.2.1/CoLT5_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 18:12:30.000000 CoLT5-attention-0.2.1/CoLT5_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-15 18:12:30.000000 CoLT5-attention-0.2.1/CoLT5_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-15 18:12:30.000000 CoLT5-attention-0.2.1/CoLT5_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-15 18:12:16.000000 CoLT5-attention-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-15 18:12:30.292684 CoLT5-attention-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-04-15 18:12:16.000000 CoLT5-attention-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:12:30.292684 CoLT5-attention-0.2.1/colt5_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-15 18:12:16.000000 CoLT5-attention-0.2.1/colt5_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-15 18:12:16.000000 CoLT5-attention-0.2.1/colt5_attention/coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-15 18:12:16.000000 CoLT5-attention-0.2.1/colt5_attention/sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19887 2023-04-15 18:12:16.000000 CoLT5-attention-0.2.1/colt5_attention/transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 18:12:30.292684 CoLT5-attention-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-15 18:12:16.000000 CoLT5-attention-0.2.1/setup.py
```

### Comparing `CoLT5-attention-0.2.0/CoLT5_attention.egg-info/PKG-INFO` & `CoLT5-attention-0.2.1/CoLT5_attention.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.2.0
+Version: 0.2.1
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.2.0/LICENSE` & `CoLT5-attention-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.2.0/PKG-INFO` & `CoLT5-attention-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.2.0
+Version: 0.2.1
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.2.0/README.md` & `CoLT5-attention-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -119,14 +119,15 @@
 ## Todo
 
 - [x] add the coordinate descent method as another router
 - [x] figure out if it can be done autoregressively and try it out - moving to <a href="https://github.com/lucidrains/coordinate-descent-attention">this repo</a>
 
 - [ ] for variable sequence lengths, allow for setting k as a function of sequence lengths per sample in batch
 - [ ] create a variant of CoLT5 for high resolution feature maps (image attention) - then try out for diffusion
+- [ ] in the cross attention scenario, support for routing token that first queries the source tokens, before retrieving from memories
 
 ## Citations
 
 ```bibtex
 @inproceedings{Ainslie2023CoLT5FL,
     title   = {CoLT5: Faster Long-Range Transformers with Conditional Computation},
     author  = {Joshua Ainslie and Tao Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit Sanghai},
```

#### html2text {}

```diff
@@ -45,13 +45,15 @@
 num_tokens_kv = 1024, # only 1024 routed from 1 million ).cuda() cross_attn_out
 = cross_attn( tokens, context = memories, mask = tokens_mask, context_mask =
 memories_mask ) cross_attn_out.shape # (2, 1024, 512) - same as tokens ``` ##
 Todo - [x] add the coordinate descent method as another router - [x] figure out
 if it can be done autoregressively and try it out - moving to this_repo - [ ]
 for variable sequence lengths, allow for setting k as a function of sequence
 lengths per sample in batch - [ ] create a variant of CoLT5 for high resolution
-feature maps (image attention) - then try out for diffusion ## Citations
-```bibtex @inproceedings{Ainslie2023CoLT5FL, title = {CoLT5: Faster Long-Range
-Transformers with Conditional Computation}, author = {Joshua Ainslie and Tao
-Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury
-Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and
-Yun-Hsuan Sung and Sumit Sanghai}, year = {2023} } ```
+feature maps (image attention) - then try out for diffusion - [ ] in the cross
+attention scenario, support for routing token that first queries the source
+tokens, before retrieving from memories ## Citations ```bibtex @inproceedings
+{Ainslie2023CoLT5FL, title = {CoLT5: Faster Long-Range Transformers with
+Conditional Computation}, author = {Joshua Ainslie and Tao Lei and Michiel de
+Jong and Santiago Ontan'on and Siddhartha Brahma and Yury Zemlyanskiy and David
+Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit
+Sanghai}, year = {2023} } ```
```

### Comparing `CoLT5-attention-0.2.0/colt5_attention/coor_descent.py` & `CoLT5-attention-0.2.1/colt5_attention/coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.2.0/colt5_attention/sinkhorn.py` & `CoLT5-attention-0.2.1/colt5_attention/sinkhorn.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.2.0/colt5_attention/transformer_block.py` & `CoLT5-attention-0.2.1/colt5_attention/transformer_block.py`

 * *Files 2% similar despite different names*

```diff
@@ -524,48 +524,68 @@
         num_tokens_q = None,
         num_tokens_kv = None,
         mask = None,
         context_mask = None
     ):
         batch, device = x.shape[0], x.device
 
-        num_tokens_q = default(num_tokens_q, self.num_tokens_q)
-        num_tokens_kv = default(num_tokens_kv, self.num_tokens_kv)
-
         batch_range = torch.arange(batch, device = device)
         batch_range = rearrange(batch_range, 'b -> b 1')
 
-        # route tokens appropriately
+        # route the queries
 
-        normalized_scores_q, indices_q = self.q_router(x, num_tokens = num_tokens_q, mask = mask)
-        normalized_scores_kv, indices_kv = self.kv_router(context, num_tokens = num_tokens_kv, mask = context_mask)
+        query_length = x.shape[-2]
+        num_tokens_q = default(num_tokens_q, self.num_tokens_q)
 
-        # select the tokens to be routed
+        routed_tokens_q = x
+        should_route_queries = query_length > num_tokens_q
 
-        routed_tokens_q = x[batch_range, indices_q]
-        routed_tokens_kv = x[batch_range, indices_kv]
+        if should_route_queries:
+            normalized_scores_q, indices_q = self.q_router(x, num_tokens = num_tokens_q, mask = mask)
 
-        # calculate key padding mask
+            routed_tokens_q = x[batch_range, indices_q]
+
+        # route the long contexts
+
+        key_value_length = context.shape[-2]
+        num_tokens_kv = default(num_tokens_kv, self.num_tokens_kv)
 
-        routed_tokens_kv_mask = None
-        if exists(mask):
-            routed_tokens_kv_mask = context_mask[batch_range, indices_kv]
+        routed_tokens_kv = context
+        routed_tokens_kv_mask = context_mask
+        normalized_scores_kv = None
+
+        should_route_kv = key_value_length > num_tokens_kv
+
+        if should_route_kv:
+            normalized_scores_kv, indices_kv = self.kv_router(context, num_tokens = num_tokens_kv, mask = context_mask)
+
+            routed_tokens_kv = x[batch_range, indices_kv]
+
+            routed_tokens_kv_mask = None
+            if exists(context_mask):
+                routed_tokens_kv_mask = context_mask[batch_range, indices_kv]
 
         # do the heavier branch with only routed tokens
 
         routed_tokens_out = self.heavy_attn(
             routed_tokens_q,
             mask = routed_tokens_kv_mask,
             context = routed_tokens_kv,
             normalized_scores_kv = normalized_scores_kv
         )
 
-        routed_tokens_out = routed_tokens_out * rearrange(normalized_scores_q, '... -> ... 1')
+        if should_route_queries:
+            routed_tokens_out = routed_tokens_out * rearrange(normalized_scores_q, '... -> ... 1')
+
+        # early return if queries did not undergo routing
+
+        if not should_route_queries:
+            return routed_tokens_out
 
-        # scatter back the output
+        # otherwise, scatter back the query outputs
 
         out = torch.zeros_like(x)
 
         if self.router_type == 'sinkhorn':
             out = scatter_mean(heavy_out, routed_tokens_out, indices_q, dim = 1)
         else:
             out[batch_range, indices_q] = routed_tokens_out
```

### Comparing `CoLT5-attention-0.2.0/setup.py` & `CoLT5-attention-0.2.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'CoLT5-attention',
   packages = find_packages(),
-  version = '0.2.0',
+  version = '0.2.1',
   license='MIT',
   description = 'Conditionally Routed Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/CoLT5-attention',
   keywords = [
```

