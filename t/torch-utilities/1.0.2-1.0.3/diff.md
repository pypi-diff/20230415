# Comparing `tmp/torch_utilities-1.0.2.tar.gz` & `tmp/torch_utilities-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_utilities-1.0.2.tar", last modified: Tue Apr 11 21:00:36 2023, max compression
+gzip compressed data, was "torch_utilities-1.0.3.tar", last modified: Sat Apr 15 13:53:30 2023, max compression
```

## Comparing `torch_utilities-1.0.2.tar` & `torch_utilities-1.0.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-04-11 21:00:36.848624 torch_utilities-1.0.2/
--rw-rw-r--   0 deema     (1000) deema     (1000)     1074 2023-04-11 20:08:44.000000 torch_utilities-1.0.2/LICENSE
--rw-rw-r--   0 deema     (1000) deema     (1000)     5061 2023-04-11 21:00:36.848624 torch_utilities-1.0.2/PKG-INFO
--rw-rw-r--   0 deema     (1000) deema     (1000)     4724 2023-04-11 20:36:41.000000 torch_utilities-1.0.2/README.md
--rw-rw-r--   0 deema     (1000) deema     (1000)       80 2023-04-11 20:08:44.000000 torch_utilities-1.0.2/pyproject.toml
--rw-rw-r--   0 deema     (1000) deema     (1000)      837 2023-04-11 21:00:36.848624 torch_utilities-1.0.2/setup.cfg
-drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-04-11 21:00:36.848624 torch_utilities-1.0.2/tests/
--rw-rw-r--   0 deema     (1000) deema     (1000)      196 2023-04-11 20:08:44.000000 torch_utilities-1.0.2/tests/__init__.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     3514 2023-04-11 20:08:44.000000 torch_utilities-1.0.2/tests/generate_test_data.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    10294 2023-04-11 20:08:44.000000 torch_utilities-1.0.2/tests/test_audio.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     2179 2023-04-11 20:08:44.000000 torch_utilities-1.0.2/tests/test_augmentation.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     5321 2023-04-11 20:08:44.000000 torch_utilities-1.0.2/tests/test_common.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     5870 2023-04-11 20:08:44.000000 torch_utilities-1.0.2/tests/test_data_loading.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     4081 2023-04-11 20:08:44.000000 torch_utilities-1.0.2/tests/test_io.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     1228 2023-04-11 20:08:44.000000 torch_utilities-1.0.2/tests/test_metrics.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     9425 2023-04-11 20:08:44.000000 torch_utilities-1.0.2/tests/test_model_trainer.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    33857 2023-04-11 20:08:44.000000 torch_utilities-1.0.2/tests/test_modules.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     3675 2023-04-11 20:08:44.000000 torch_utilities-1.0.2/tests/test_pytorch.py
-drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-04-11 21:00:36.848624 torch_utilities-1.0.2/torch_utilities/
--rw-rw-r--   0 deema     (1000) deema     (1000)      373 2023-04-11 20:08:44.000000 torch_utilities-1.0.2/torch_utilities/__init__.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    19083 2023-04-11 20:08:44.000000 torch_utilities-1.0.2/torch_utilities/audio.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     6376 2023-04-11 20:08:44.000000 torch_utilities-1.0.2/torch_utilities/augmentation.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     6300 2023-04-11 20:08:44.000000 torch_utilities-1.0.2/torch_utilities/common.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    13302 2023-04-11 20:08:44.000000 torch_utilities-1.0.2/torch_utilities/data_loading.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     4664 2023-04-11 20:08:44.000000 torch_utilities-1.0.2/torch_utilities/io.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     3777 2023-04-11 20:08:44.000000 torch_utilities-1.0.2/torch_utilities/metrics.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    28901 2023-04-11 20:57:07.000000 torch_utilities-1.0.2/torch_utilities/model_trainer.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    42064 2023-04-11 20:08:44.000000 torch_utilities-1.0.2/torch_utilities/modules.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    11611 2023-04-11 20:08:44.000000 torch_utilities-1.0.2/torch_utilities/pytorch.py
-drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-04-11 21:00:36.848624 torch_utilities-1.0.2/torch_utilities.egg-info/
--rw-rw-r--   0 deema     (1000) deema     (1000)     5061 2023-04-11 21:00:36.000000 torch_utilities-1.0.2/torch_utilities.egg-info/PKG-INFO
--rw-rw-r--   0 deema     (1000) deema     (1000)     1057 2023-04-11 21:00:36.000000 torch_utilities-1.0.2/torch_utilities.egg-info/SOURCES.txt
--rw-rw-r--   0 deema     (1000) deema     (1000)        1 2023-04-11 21:00:36.000000 torch_utilities-1.0.2/torch_utilities.egg-info/dependency_links.txt
--rw-rw-r--   0 deema     (1000) deema     (1000)      147 2023-04-11 21:00:36.000000 torch_utilities-1.0.2/torch_utilities.egg-info/entry_points.txt
--rw-rw-r--   0 deema     (1000) deema     (1000)      154 2023-04-11 21:00:36.000000 torch_utilities-1.0.2/torch_utilities.egg-info/requires.txt
--rw-rw-r--   0 deema     (1000) deema     (1000)       22 2023-04-11 21:00:36.000000 torch_utilities-1.0.2/torch_utilities.egg-info/top_level.txt
+drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-04-15 13:53:30.153149 torch_utilities-1.0.3/
+-rw-rw-r--   0 deema     (1000) deema     (1000)     1074 2023-04-12 21:50:16.000000 torch_utilities-1.0.3/LICENSE
+-rw-rw-r--   0 deema     (1000) deema     (1000)     4980 2023-04-15 13:53:30.153149 torch_utilities-1.0.3/PKG-INFO
+-rw-rw-r--   0 deema     (1000) deema     (1000)     4643 2023-04-15 12:37:07.000000 torch_utilities-1.0.3/README.md
+-rw-rw-r--   0 deema     (1000) deema     (1000)       80 2023-04-12 21:50:16.000000 torch_utilities-1.0.3/pyproject.toml
+-rw-rw-r--   0 deema     (1000) deema     (1000)      837 2023-04-15 13:53:30.153149 torch_utilities-1.0.3/setup.cfg
+drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-04-15 13:53:30.153149 torch_utilities-1.0.3/tests/
+-rw-rw-r--   0 deema     (1000) deema     (1000)      196 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/tests/__init__.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     3514 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/tests/generate_test_data.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)    10294 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/tests/test_audio.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     2179 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/tests/test_augmentation.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     5321 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/tests/test_common.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     5870 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/tests/test_data_loading.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     4081 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/tests/test_io.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     1228 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/tests/test_metrics.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     9425 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/tests/test_model_trainer.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)    37202 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/tests/test_modules.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     3675 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/tests/test_pytorch.py
+drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-04-15 13:53:30.153149 torch_utilities-1.0.3/torch_utilities/
+-rw-rw-r--   0 deema     (1000) deema     (1000)      373 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/torch_utilities/__init__.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)    19083 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/torch_utilities/audio.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     6376 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/torch_utilities/augmentation.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     6300 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/torch_utilities/common.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)    13302 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/torch_utilities/data_loading.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     4664 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/torch_utilities/io.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     3777 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/torch_utilities/metrics.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)    29223 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/torch_utilities/model_trainer.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)    44684 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/torch_utilities/modules.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)    11611 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/torch_utilities/pytorch.py
+drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-04-15 13:53:30.153149 torch_utilities-1.0.3/torch_utilities.egg-info/
+-rw-rw-r--   0 deema     (1000) deema     (1000)     4980 2023-04-15 13:53:30.000000 torch_utilities-1.0.3/torch_utilities.egg-info/PKG-INFO
+-rw-rw-r--   0 deema     (1000) deema     (1000)     1057 2023-04-15 13:53:30.000000 torch_utilities-1.0.3/torch_utilities.egg-info/SOURCES.txt
+-rw-rw-r--   0 deema     (1000) deema     (1000)        1 2023-04-15 13:53:30.000000 torch_utilities-1.0.3/torch_utilities.egg-info/dependency_links.txt
+-rw-rw-r--   0 deema     (1000) deema     (1000)      147 2023-04-15 13:53:30.000000 torch_utilities-1.0.3/torch_utilities.egg-info/entry_points.txt
+-rw-rw-r--   0 deema     (1000) deema     (1000)      154 2023-04-15 13:53:30.000000 torch_utilities-1.0.3/torch_utilities.egg-info/requires.txt
+-rw-rw-r--   0 deema     (1000) deema     (1000)       22 2023-04-15 13:53:30.000000 torch_utilities-1.0.3/torch_utilities.egg-info/top_level.txt
```

### Comparing `torch_utilities-1.0.2/LICENSE` & `torch_utilities-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.2/PKG-INFO` & `torch_utilities-1.0.3/torch_utilities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: torch_utilities
-Version: 1.0.2
+Name: torch-utilities
+Version: 1.0.3
 Summary: Simplifying audio and deep learning with PyTorch.
 Home-page: https://github.com/FedericoDiMarzo/torch_utilities
 Author: Federico Di Marzo
 Author-email: federicodimarzo@protonmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -17,16 +17,14 @@
 
 ## Installation
 You can install **Torch Utilities** using pip
 ```bash
 pip install torch_utilities
 ```
 
-A pypi package will be provided in the future when the API will be more stable.
-
 ## Running The Tests
 To verify the correctness of the code and run the tests, simply run the following line in a bash console:
 ```bash
 python torch_utilities/scripts/run_tests.py
 ```
 This will run a suite of tests to ensure that the module is functioning as expected. If any tests fail, it may indicate that there is a bug in the code or that some aspect of the API has changed. In such cases, we encourage you to open an issue on the repository so that we can help resolve the problem.
```

### Comparing `torch_utilities-1.0.2/README.md` & `torch_utilities-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 
 ## Installation
 You can install **Torch Utilities** using pip
 ```bash
 pip install torch_utilities
 ```
 
-A pypi package will be provided in the future when the API will be more stable.
-
 ## Running The Tests
 To verify the correctness of the code and run the tests, simply run the following line in a bash console:
 ```bash
 python torch_utilities/scripts/run_tests.py
 ```
 This will run a suite of tests to ensure that the module is functioning as expected. If any tests fail, it may indicate that there is a bug in the code or that some aspect of the API has changed. In such cases, we encourage you to open an issue on the repository so that we can help resolve the problem.
```

### Comparing `torch_utilities-1.0.2/setup.cfg` & `torch_utilities-1.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = torch_utilities
-version = 1.0.2
+version = 1.0.3
 author = Federico Di Marzo
 author_email = federicodimarzo@protonmail.com
 description = Simplifying audio and deep learning with PyTorch.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/FedericoDiMarzo/torch_utilities
```

### Comparing `torch_utilities-1.0.2/tests/generate_test_data.py` & `torch_utilities-1.0.3/tests/generate_test_data.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.2/tests/test_audio.py` & `torch_utilities-1.0.3/tests/test_audio.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.2/tests/test_augmentation.py` & `torch_utilities-1.0.3/tests/test_augmentation.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.2/tests/test_common.py` & `torch_utilities-1.0.3/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.2/tests/test_data_loading.py` & `torch_utilities-1.0.3/tests/test_data_loading.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.2/tests/test_io.py` & `torch_utilities-1.0.3/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.2/tests/test_metrics.py` & `torch_utilities-1.0.3/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.2/tests/test_model_trainer.py` & `torch_utilities-1.0.3/tests/test_model_trainer.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.2/tests/test_modules.py` & `torch_utilities-1.0.3/tests/test_modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import numpy as np
 import unittest
 import torch
 
 set_module_root("../torch_utils")
 import torch_utilities as tu
 from torch_utilities import repeat_test, set_device
-from torch_utilities.modules import get_time_value, get_freq_value
+from torch_utilities.modules import get_time_value, get_freq_value, get_causal_longformer_mask
 
 # = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = =
 
 
 def _setup() -> None:
     torch.manual_seed(984)
     np.random.seed(876)
@@ -461,20 +461,20 @@
                 enable_weight_norm,
                 merge_after_conv,
                 dtype,
                 in_freqs,
             ) = p
             if in_freqs % 2 == 1:
                 stride_f = 1
-                
+
             if (not merge_after_conv) and (stride_f != 1):
                 # excluding cases where the merge is before the stride
                 # and the stride is different than 1
                 return
-             
+
             with self.subTest(p=p):
                 conv = self.get_instance(p)
                 x = self.get_input(p)
                 y = conv(x)
                 batch_size, _, frames = x.shape[:3]
                 out_freqs = in_freqs // stride_f
                 expected_shape = (batch_size, out_channels, frames, out_freqs)
@@ -1037,9 +1037,125 @@
                 y = csc(x)
                 B, C, T, F = x.shape
                 self.assertEqual(y.shape, (B, out_channels, T, in_freqs * stride_f))
 
 
 # = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = =
 
+
+class TestSlidingCausalMultiheadAttention(unittest.TestCase):
+    @classmethod
+    def setUpClass(cls):
+        _setup()
+
+    def setUp(self):
+        self.channels = (2,)
+        self.sequence_len = (10,)
+        self.embed_dim = (32, 64)
+        self.stride = (5, 2)
+        self.num_heads = (1,)
+        self.dropout = (0,)
+        self.bias = (True,)
+        self.receptive_field = (None,)
+        self.attn_mask = (None,)
+        # ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~
+        self.params = product(
+            self.channels,
+            self.sequence_len,
+            self.embed_dim,
+            self.stride,
+            self.num_heads,
+            self.dropout,
+            self.bias,
+            self.receptive_field,
+            self.attn_mask,
+        )
+
+    def get_instance(self, p: Tuple) -> tu.SlidingCausalMultiheadAttention:
+        (
+            channels,
+            sequence_len,
+            embed_dim,
+            stride,
+            num_heads,
+            dropout,
+            bias,
+            receptive_field,
+            attn_mask,
+        ) = p
+        instance = tu.SlidingCausalMultiheadAttention(
+            channels=channels,
+            sequence_len=sequence_len,
+            embed_dim=embed_dim,
+            stride=stride,
+            num_heads=num_heads,
+            dropout=dropout,
+            bias=bias,
+            receptive_field=receptive_field,
+            attn_mask=attn_mask,
+        )
+        return instance
+
+    def get_input(self, p: Tuple) -> Tensor:
+        (
+            channels,
+            sequence_len,
+            embed_dim,
+            stride,
+            num_heads,
+            dropout,
+            bias,
+            receptive_field,
+            attn_mask,
+        ) = p
+        x = _get_input(channels, embed_dim, None)
+        return x
+
+    def test_inner_modules(self):
+        for p in self.params:
+            (
+                channels,
+                sequence_len,
+                embed_dim,
+                stride,
+                num_heads,
+                dropout,
+                bias,
+                receptive_field,
+                attn_mask,
+            ) = p
+            with self.subTest(p=p):
+                att = self.get_instance(p)
+                self.assertEqual(type(att.mh_attention), nn.MultiheadAttention)
+                self.assertEqual(type(att.unfold), tu.UnfoldSpectrogram)
+                self.assertEqual(type(att.fold), tu.FoldSpectrogram)
+
+                # default attention mask
+                if attn_mask is None and receptive_field is None:
+                    expected = get_causal_longformer_mask(sequence_len, sequence_len // 2)
+                    max_err = (expected - att.attn_mask).abs().max()
+                    self.assertLess(max_err, 1e-12)
+
+    def test_forward(self):
+        for p in self.params:
+            (
+                channels,
+                sequence_len,
+                embed_dim,
+                stride,
+                num_heads,
+                dropout,
+                bias,
+                receptive_field,
+                attn_mask,
+            ) = p
+            with self.subTest(p=p):
+                att = self.get_instance(p)
+                x = self.get_input(p)
+                y = att(x)
+                self.assertEqual(x.shape, y.shape)
+
+
+# = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = =
+
 if __name__ == "__main__":
     unittest.main(verbosity=2)
```

### Comparing `torch_utilities-1.0.2/tests/test_pytorch.py` & `torch_utilities-1.0.3/tests/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.2/torch_utilities/audio.py` & `torch_utilities-1.0.3/torch_utilities/audio.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.2/torch_utilities/augmentation.py` & `torch_utilities-1.0.3/torch_utilities/augmentation.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.2/torch_utilities/common.py` & `torch_utilities-1.0.3/torch_utilities/common.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.2/torch_utilities/data_loading.py` & `torch_utilities-1.0.3/torch_utilities/data_loading.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.2/torch_utilities/io.py` & `torch_utilities-1.0.3/torch_utilities/io.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.2/torch_utilities/metrics.py` & `torch_utilities-1.0.3/torch_utilities/metrics.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.2/torch_utilities/model_trainer.py` & `torch_utilities-1.0.3/torch_utilities/model_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,16 @@
         train_dl: DataLoader,
         valid_dl: DataLoader,
         optimizer_class: Type[Optimizer],
         losses: List[Callable],
         net_ins_indices: Optional[List[int]] = None,
         losses_names: Optional[List[str]] = None,
         save_buffer_maxlen: int = 10,
-        gradient_clip_value: Optional[float] = None,
         enable_profiling: bool = False,
+        reset_epoch: bool = False,
     ) -> None:
         """
         Abstract class to structure a model training.
 
         The directory pointed by model_path should
         have the following structure:
 
@@ -74,20 +74,21 @@
                 dataloader out = [T0, T1, T2]
                 net_ins_indices = [2, 1]
                 net_ins = [T2, T1]
         losses_names : Optional[List[str]]
             Names of the losses, by default ["loss0", "loss1", ...]
         save_buffer_maxlen : int, optional
             N best checkpoints saved (based on a lower total loss),
-            by default 5
-        gradient_clip_value : Optional[float]
-            Maximum gradient update value, by default no gradient clipping
+            by default 10
         enable_profiling : bool, optional
             If True runs one full run of the train dataset and
             logs to tensorboard the profiling information, by default False
+        reset_epoch : bool, optional
+            If set to True resets the epoch to 0 after loading the checkpoints,
+            by default False
 
 
         config.yml [training] parameters
         ----------
         max_epochs : int, optional
             Max number of epochs, by default 100
         learning_rate : float, optional
@@ -97,42 +98,47 @@
         weight_decay : float, optional
             Optimizer weight_decay, by default 0
         losses_weights : List[float], optional
             Per-loss gains, by default all ones
         log_every : int, optional
             Frequency of the logs (over the dataset iterations),
             by default 100
+        gradient_clip_value : float, optional
+            Maximum gradient update value, by default no gradient clipping
         """
         self.device = tu.get_device()
 
         # explicit attributes
         self.model_path = model_path
         self.model = model
         self.train_dl = train_dl
         self.valid_dl = valid_dl
         self.losses = losses
         self.net_ins_indices = net_ins_indices or [0]
         self.losses_names = losses_names or self._default_losses_names()
         self.optimizer_class = optimizer_class
-        self.gradient_clip_value = gradient_clip_value
         self.enable_profiling = enable_profiling
+        self.reset_epoch = reset_epoch
 
         # configuration attributes
         self.config_path = self.model_path / "config.yml"
         self.config = tu.Config(self.config_path)
         self.learning_rate = self._from_config("learning_rate", float, 1e-5)
         self.weight_decay = self._from_config("weight_decay", float, 0)
         self.log_every = self._from_config("log_every", int, 100)
         self.max_epochs = self._from_config("max_epochs", int, 100)
         self.overfit_mode = self._from_config("overfit_mode", bool, False)
         self.losses_weights = self._from_config(
             "losses_weights", np.array, np.ones(len(self.losses))
         )
         self.losses_weights = self.losses_weights.astype(float)
 
+        gcv = self._from_config("gradient_clip_value", float, -1)
+        self.gradient_clip_value = gcv if (gcv > 0) else None
+
         # other dirs
         self.checkpoints_dir = model_path / "checkpoints"
         self.checkpoint_monitoring_file = self.checkpoints_dir / "ckpt.yml"
         self.logs_dir = model_path / "logs"
         [d.mkdir(exist_ok=True) for d in (self.checkpoints_dir, self.logs_dir)]
 
         # model and running_losses setup
@@ -155,15 +161,15 @@
         self.dummy_input_train = self._get_dummy_data(True)
         self.dummy_input_valid = self._get_dummy_data(False)
         self.last_total_loss = 1e10
         self.last_computed_metric = -1e10  # used to select the best checkpoints
         self.profiler = self._get_profiler()  # null context manager if enable_profiling==False
 
     # = = = = = = = = = = = = = = = = = = = = = =
-    #             Getters/Setters
+    #         Public getters/setters
     # = = = = = = = = = = = = = = = = = = = = = =
     def get_model(self) -> nn.Module:
         """
         Gets the model instance.
 
         Returns
         -------
@@ -239,14 +245,25 @@
         ----------
         value : float
             New learning rate
         """
         for g in self.optimizer.param_groups:
             g["weight_decay"] = value
 
+    def get_tensorboard_writer(self) -> SummaryWriter:
+        """
+        Getter to the tensorboard log writer
+
+        Returns
+        -------
+        SummaryWriter
+            tensorboard log writer
+        """
+        return self.log_writer
+
     # = = = = = = = = = = = = = = = = = = = = = =
     #             Training loop
     # = = = = = = = = = = = = = = = = = = = = = =
     def start_training(self) -> None:
         """
         Trains a model.
         """
@@ -503,15 +520,15 @@
         """
         m = self.model(self.config_path)
         m.to(self.device)
 
         # load checkpoint if it exists
         if self._prev_train_exists():
             epoch, model_state, optim_state = self._load_checkpoint()
-            self.start_epoch = epoch
+            self.start_epoch = 0 if self.reset_epoch else epoch
             self.optim_state = optim_state
             m.load_state_dict(model_state)
 
         return m
 
     def _prev_train_exists(self) -> bool:
         """
@@ -657,25 +674,14 @@
                 # ignore errors for optimizer mismatches
                 optim.load_state_dict(self.optim_state)
         return optim
 
     # = = = = = = = = = = = = = = = = = = = = = =
     #                Logging
     # = = = = = = = = = = = = = = = = = = = = = =
-    def get_tensorboard_writer(self) -> SummaryWriter:
-        """
-        Getter to the tensorboard log writer
-
-        Returns
-        -------
-        SummaryWriter
-            tensorboard log writer
-        """
-        return self.log_writer
-
     @abc.abstractclassmethod
     def tensorboard_logs(self, raw_data: List[Tensor], epoch: int) -> None:
         """
         Additional tensorboard logging.
 
         Parameters
         ----------
@@ -806,14 +812,15 @@
         # adding also the parameters
         txt += f" parameters: {self._get_model_parameters() * 1e-3} K"
 
         self.log_writer.add_text("config.yaml", txt, 0)
 
     # = = = = = = = = = = = = = = = = = = = = = =
     #                Profiler
+    # = = = = = = = = = = = = = = = = = = = = = =
     def _get_profiler(self) -> torch.profiler.profile:
         """
         Return the profiler context manager.
 
         Returns
         -------
         torch.profiler.profile
```

### Comparing `torch_utilities-1.0.2/torch_utilities/modules.py` & `torch_utilities-1.0.3/torch_utilities/modules.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,14 +27,16 @@
     "CausalSubConv2d",
     # conv2d compositions
     "CausalConv2dNormAct",
     "CausalSmoothedTConv",
     "DenseConvBlock",
     # recurrent variants
     "GruNormAct",
+    # attention variants
+    "SlidingCausalMultiheadAttention",
 ]
 
 # private utility functions = = = = = = = = = = = = = =
 
 
 def get_time_value(param):
     """
@@ -118,36 +120,36 @@
     k_t, k_f = [f(kernel_size) for f in (get_time_value, get_freq_value)]
     dilation = [(k_t**x, k_f**x) for x in range(depth)]
     if disable_dilation_f:
         dilation = [(d[0], 1) for d in dilation]
     return dilation
 
 
-def get_causal_longformer_mask(size_len: int, width: int) -> Tensor:
+def get_causal_longformer_mask(sequence_len: int, receptive_field: int) -> Tensor:
     """
     Obtain a causal mask inspired by the Longformer to use
     within self attention layers.
 
     https://arxiv.org/abs/2004.05150
 
     Parameters
     ----------
-    size_len : int
+    sequence_len : int
         Length of the sequence
-    width : int
-        Number of previous neighbours to pay attention to
+    receptive_field : int
+        Number of previous frames to pay attention to
 
     Returns
     -------
     Tensor
-        Attention mask
+        Attention mask of shape (sequence_len, sequence_len)
     """
-    _diag = lambda i: torch.diag(torch.ones(size_len - i), -i)
+    _diag = lambda i: torch.diag(torch.ones(sequence_len - i), -i)
     mask = _diag(0)
-    for i in range(1, width):
+    for i in range(1, receptive_field):
         mask += _diag(i)
     return mask
 
 
 # utilitiy layers  = = = = = = = = = = = = = = = = = = =
 class LambdaLayer(Module):
     def __init__(self, f: Callable):
@@ -318,15 +320,15 @@
             Input of shape (B, C, T, F)
 
         Returns
         -------
         Tensor
             Unfolded input of shape (B, C*num_blocks, block_size, F)
         """
-        assert self._input_shape_is_valid(x), r"x.shape[2] - block_size % stride != 0"
+        assert self._input_shape_is_valid(x), r"(x.shape[2] - block_size) % stride != 0"
         ch = x.shape[1]
         x = self._reshape_0(x)
         x = self._unfold(x)
         x = self._reshape_1(x)
         x = self._reshape_2(x)
         x = self._reshape_3(x, ch)
         return x
@@ -464,16 +466,16 @@
         super().__init__()
         self.layers = nn.Sequential(*modules)
 
     def forward(self, x: Tensor) -> Tensor:
         y = self.layers(x)
         # keeping the channels of the output
         c_out = y.shape[1]
-        y = x[:,:c_out] + y[:,:c_out]
-        
+        y = x[:, :c_out] + y[:, :c_out]
+
         return y
 
 
 # dense variants = = = = = = = = = = = = = = = = = = = =
 class GroupedLinear(Module):
     def __init__(
         self,
@@ -1311,32 +1313,100 @@
         y = y.transpose(1, 2)
         y = self.activation(y)
         if self.residual_merge is not None:
             y = self.residual_merge(x, y)
         return y, h
 
 
-# attention variants  = = = = = = = = = = = = = = = = = 
-class SlidingSelfAttention(Module):
+# attention variants  = = = = = = = = = = = = = = = = =
+class SlidingCausalMultiheadAttention(Module):
     def __init__(
         self,
-        hidden_size: int,
+        channels: int,
         sequence_len: int,
-        receptive_field: int,
-        depth: int,
-        heads: int,
-        dropout: float = 0.1,
+        embed_dim: int,
+        stride: int,
+        num_heads: int,
+        dropout: float = 0.0,
+        bias: bool = True,
+        receptive_field: Optional[int] = None,
+        attn_mask: Optional[Tensor] = None,
     ) -> None:
-        # TODO: implement it
+        """
+        Causal multi head attention module applied on an
+        unfolded version of the input.
+
+        Parameters
+        ----------
+        channels : int
+            Number of input channels
+        embed_dim : int
+            Dimension of the embeddings (F)
+        sequence_len : int
+            Lenght of the sequence blocks resulting from the unfolding
+        stride : int
+            Hop size between the blocks
+        num_heads : int
+            Number of heads for the attention
+        dropout : float, optional
+            Dropout amount, by default 0.0
+        bias : bool, optional
+            Enables/disables the biases in the projections, by default True
+        receptive_field : Optional[int], optional
+            Used for the default causal Longformer mask, indicates the number of frames
+            employed in the computation of the attention, by default half of the sequence_len
+        attn_mask : Optional[Tensor], optional
+            Mask provided to the attention layer, by default a causal version of the Longformer
+            mask is provided https://arxiv.org/abs/2004.05150
+        """
         super().__init__()
 
         # attributes
-        self.receptive_field = receptive_field
+        self.channels = channels
+        self.embed_dim = embed_dim
+        self.num_heads = num_heads
+        self.sequence_len = sequence_len
         self.stride = stride
-        self.hidden_size = hidden_size
-        self.heads = heads
         self.dropout = dropout
+        self.bias = bias
+        self.receptive_field = receptive_field or (self.sequence_len // 2)
+        self.attn_mask = attn_mask or get_causal_longformer_mask(
+            self.sequence_len, self.receptive_field
+        )
 
         # inner modules
+        self.reshape_0 = lambda x: x.flatten(0, 1)
+        self.reshape_1 = lambda x, b: x.reshape(b, -1, x.shape[1], x.shape[2])
+
+        self.unfold = UnfoldSpectrogram(self.sequence_len, self.stride)
+        self.fold = FoldSpectrogram(self.sequence_len, self.stride, self.channels)
+
+        self.mh_attention = nn.MultiheadAttention(
+            embed_dim=self.embed_dim,
+            num_heads=self.num_heads,
+            dropout=self.dropout,
+            bias=self.bias,
+            batch_first=True,
+        )
+
+    def forward(self, x: Tensor) -> Tensor:
+        """
+        Parameters
+        ----------
+        x : Tensor
+            Input of shape (B, C, T, F)
+
+        Returns
+        -------
+        Tensor
+            Output of shape (B, C, T, F)
+        """
+        B = x.shape[0]
+        x = self.unfold(x)
+        x = self.reshape_0(x)
+        x = self.mh_attention(x, x, x, attn_mask=self.attn_mask)[0]
+        x = self.reshape_1(x, B)
+        x = self.fold(x)
+        return x
 
 
 # = = = = = = = = = = = = = = = = = = = = = = = = = = =
```

### Comparing `torch_utilities-1.0.2/torch_utilities/pytorch.py` & `torch_utilities-1.0.3/torch_utilities/pytorch.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.2/torch_utilities.egg-info/PKG-INFO` & `torch_utilities-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: torch-utilities
-Version: 1.0.2
+Name: torch_utilities
+Version: 1.0.3
 Summary: Simplifying audio and deep learning with PyTorch.
 Home-page: https://github.com/FedericoDiMarzo/torch_utilities
 Author: Federico Di Marzo
 Author-email: federicodimarzo@protonmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -17,16 +17,14 @@
 
 ## Installation
 You can install **Torch Utilities** using pip
 ```bash
 pip install torch_utilities
 ```
 
-A pypi package will be provided in the future when the API will be more stable.
-
 ## Running The Tests
 To verify the correctness of the code and run the tests, simply run the following line in a bash console:
 ```bash
 python torch_utilities/scripts/run_tests.py
 ```
 This will run a suite of tests to ensure that the module is functioning as expected. If any tests fail, it may indicate that there is a bug in the code or that some aspect of the API has changed. In such cases, we encourage you to open an issue on the repository so that we can help resolve the problem.
```

### Comparing `torch_utilities-1.0.2/torch_utilities.egg-info/SOURCES.txt` & `torch_utilities-1.0.3/torch_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

