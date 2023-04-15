# Comparing `tmp/simple-hierarchical-transformer-0.0.8.tar.gz` & `tmp/simple-hierarchical-transformer-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-hierarchical-transformer-0.0.8.tar", last modified: Wed Apr 12 02:05:23 2023, max compression
+gzip compressed data, was "simple-hierarchical-transformer-0.0.9.tar", last modified: Wed Apr 12 02:50:51 2023, max compression
```

## Comparing `simple-hierarchical-transformer-0.0.8.tar` & `simple-hierarchical-transformer-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:05:23.357913 simple-hierarchical-transformer-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-12 02:05:10.000000 simple-hierarchical-transformer-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-12 02:05:23.357913 simple-hierarchical-transformer-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-04-12 02:05:10.000000 simple-hierarchical-transformer-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 02:05:23.357913 simple-hierarchical-transformer-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-12 02:05:10.000000 simple-hierarchical-transformer-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:05:23.357913 simple-hierarchical-transformer-0.0.8/simple_hierarchical_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-12 02:05:10.000000 simple-hierarchical-transformer-0.0.8/simple_hierarchical_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-12 02:05:10.000000 simple-hierarchical-transformer-0.0.8/simple_hierarchical_transformer/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    16463 2023-04-12 02:05:10.000000 simple-hierarchical-transformer-0.0.8/simple_hierarchical_transformer/simple_hierarchical_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:05:23.357913 simple-hierarchical-transformer-0.0.8/simple_hierarchical_transformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-12 02:05:23.000000 simple-hierarchical-transformer-0.0.8/simple_hierarchical_transformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-12 02:05:23.000000 simple-hierarchical-transformer-0.0.8/simple_hierarchical_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 02:05:23.000000 simple-hierarchical-transformer-0.0.8/simple_hierarchical_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-12 02:05:23.000000 simple-hierarchical-transformer-0.0.8/simple_hierarchical_transformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-12 02:05:23.000000 simple-hierarchical-transformer-0.0.8/simple_hierarchical_transformer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:50:51.295391 simple-hierarchical-transformer-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-12 02:50:38.000000 simple-hierarchical-transformer-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-12 02:50:51.295391 simple-hierarchical-transformer-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-04-12 02:50:38.000000 simple-hierarchical-transformer-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 02:50:51.295391 simple-hierarchical-transformer-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-12 02:50:38.000000 simple-hierarchical-transformer-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:50:51.295391 simple-hierarchical-transformer-0.0.9/simple_hierarchical_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-12 02:50:38.000000 simple-hierarchical-transformer-0.0.9/simple_hierarchical_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-12 02:50:38.000000 simple-hierarchical-transformer-0.0.9/simple_hierarchical_transformer/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16574 2023-04-12 02:50:38.000000 simple-hierarchical-transformer-0.0.9/simple_hierarchical_transformer/simple_hierarchical_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:50:51.295391 simple-hierarchical-transformer-0.0.9/simple_hierarchical_transformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-12 02:50:51.000000 simple-hierarchical-transformer-0.0.9/simple_hierarchical_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-12 02:50:51.000000 simple-hierarchical-transformer-0.0.9/simple_hierarchical_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 02:50:51.000000 simple-hierarchical-transformer-0.0.9/simple_hierarchical_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-12 02:50:51.000000 simple-hierarchical-transformer-0.0.9/simple_hierarchical_transformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-12 02:50:51.000000 simple-hierarchical-transformer-0.0.9/simple_hierarchical_transformer.egg-info/top_level.txt
```

### Comparing `simple-hierarchical-transformer-0.0.8/LICENSE` & `simple-hierarchical-transformer-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-hierarchical-transformer-0.0.8/PKG-INFO` & `simple-hierarchical-transformer-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-hierarchical-transformer
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple Hierarchical Transformer
 Home-page: https://github.com/lucidrains/simple-hierarchical-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,hierarchical
 Classifier: Development Status :: 4 - Beta
```

### Comparing `simple-hierarchical-transformer-0.0.8/README.md` & `simple-hierarchical-transformer-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## Simple Hierarchical Transformer (wip)
+## Simple Hierarchical Transformer
 
 Experiments around a simple idea for inducing multiple hierarchical predictive coding models within a GPT. It is so simple, it may not work. But then again, deep learning progress is built on the bedrocks of simple ideas. Worth a shot.
 
 So far, the idea has passed the litmus test from a research friend. Will bring it to completion in the next week or so. If it does not work out, I'll leave the negative experimental results as well as the repository around, and maybe some PhD student can build upon it.
 
 <a href="https://api.wandb.ai/links/lucidrains/w8vdkz75">Ongoing experiments</a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-## Simple Hierarchical Transformer (wip) Experiments around a simple idea for
+## Simple Hierarchical Transformer Experiments around a simple idea for
 inducing multiple hierarchical predictive coding models within a GPT. It is so
 simple, it may not work. But then again, deep learning progress is built on the
 bedrocks of simple ideas. Worth a shot. So far, the idea has passed the litmus
 test from a research friend. Will bring it to completion in the next week or
 so. If it does not work out, I'll leave the negative experimental results as
 well as the repository around, and maybe some PhD student can build upon it.
 Ongoing_experiments Update: I think it is working ð¤ ## Appreciation -
```

### Comparing `simple-hierarchical-transformer-0.0.8/setup.py` & `simple-hierarchical-transformer-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'simple-hierarchical-transformer',
   packages = find_packages(exclude=[]),
-  version = '0.0.8',
+  version = '0.0.9',
   license='MIT',
   description = 'Simple Hierarchical Transformer',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/simple-hierarchical-transformer',
   keywords = [
```

### Comparing `simple-hierarchical-transformer-0.0.8/simple_hierarchical_transformer/attention.py` & `simple-hierarchical-transformer-0.0.9/simple_hierarchical_transformer/attention.py`

 * *Files identical despite different names*

### Comparing `simple-hierarchical-transformer-0.0.8/simple_hierarchical_transformer/simple_hierarchical_transformer.py` & `simple-hierarchical-transformer-0.0.9/simple_hierarchical_transformer/simple_hierarchical_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -484,15 +484,16 @@
     @property
     def device(self):
         return next(self.parameters()).device
     
     def forward(
         self,
         ids,
-        return_loss = False
+        return_loss = False,
+        ablate_hierarchical_merge = False
     ):
         """
         einops notation:
 
         b - batch
         n - sequence length
         c - compression factor
@@ -536,14 +537,17 @@
                 next_tokens.append(h)
 
             tokens = next_tokens
 
             # pool the information all hierarchies
             # and then update the tokens that will be used to make the final autoregressive prediction
 
+            if ablate_hierarchical_merge:
+                continue
+
             pooled = merge(tokens)
             predict_tokens = tokens[self.predict_hierarchy_index]
             predict_tokens = predict_tokens + pooled
             tokens[self.predict_hierarchy_index] = predict_tokens
 
         # final norm and logits
```

### Comparing `simple-hierarchical-transformer-0.0.8/simple_hierarchical_transformer.egg-info/PKG-INFO` & `simple-hierarchical-transformer-0.0.9/simple_hierarchical_transformer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-hierarchical-transformer
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple Hierarchical Transformer
 Home-page: https://github.com/lucidrains/simple-hierarchical-transformer
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,hierarchical
 Classifier: Development Status :: 4 - Beta
```

