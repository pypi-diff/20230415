# Comparing `tmp/nekograd-0.0.1.tar.gz` & `tmp/nekograd-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nekograd-0.0.1.tar", last modified: Sun Mar 26 00:36:53 2023, max compression
+gzip compressed data, was "nekograd-0.1.0.tar", last modified: Sat Apr 15 09:08:18 2023, max compression
```

## Comparing `nekograd-0.0.1.tar` & `nekograd-0.1.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:36:53.218232 nekograd-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-26 00:36:37.000000 nekograd-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-26 00:36:37.000000 nekograd-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-03-26 00:36:53.218232 nekograd-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-26 00:36:37.000000 nekograd-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:36:53.214232 nekograd-0.0.1/nekograd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 00:36:37.000000 nekograd-0.0.1/nekograd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-26 00:36:37.000000 nekograd-0.0.1/nekograd/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:36:53.214232 nekograd-0.0.1/nekograd/data/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-26 00:36:37.000000 nekograd-0.0.1/nekograd/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-03-26 00:36:37.000000 nekograd-0.0.1/nekograd/data/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-03-26 00:36:37.000000 nekograd-0.0.1/nekograd/data/split.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-26 00:36:37.000000 nekograd-0.0.1/nekograd/data/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-26 00:36:37.000000 nekograd-0.0.1/nekograd/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:36:53.214232 nekograd-0.0.1/nekograd/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 00:36:37.000000 nekograd-0.0.1/nekograd/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-26 00:36:37.000000 nekograd-0.0.1/nekograd/metrics/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-03-26 00:36:37.000000 nekograd-0.0.1/nekograd/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:36:53.218232 nekograd-0.0.1/nekograd/model/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-26 00:36:37.000000 nekograd-0.0.1/nekograd/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-03-26 00:36:37.000000 nekograd-0.0.1/nekograd/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-26 00:36:37.000000 nekograd-0.0.1/nekograd/model/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-03-26 00:36:37.000000 nekograd-0.0.1/nekograd/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:36:53.218232 nekograd-0.0.1/nekograd/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 00:36:37.000000 nekograd-0.0.1/nekograd/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-03-26 00:36:37.000000 nekograd-0.0.1/nekograd/torch/criterion.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-26 00:36:37.000000 nekograd-0.0.1/nekograd/torch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:36:53.214232 nekograd-0.0.1/nekograd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-03-26 00:36:53.000000 nekograd-0.0.1/nekograd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-03-26 00:36:53.000000 nekograd-0.0.1/nekograd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 00:36:53.000000 nekograd-0.0.1/nekograd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-26 00:36:53.000000 nekograd-0.0.1/nekograd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-26 00:36:53.000000 nekograd-0.0.1/nekograd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-26 00:36:37.000000 nekograd-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-26 00:36:53.218232 nekograd-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-03-26 00:36:37.000000 nekograd-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:36:53.218232 nekograd-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-03-26 00:36:37.000000 nekograd-0.0.1/tests/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:08:18.100280 nekograd-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-15 09:08:08.000000 nekograd-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-15 09:08:08.000000 nekograd-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-15 09:08:18.100280 nekograd-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-15 09:08:08.000000 nekograd-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:08:18.096280 nekograd-0.1.0/nekograd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:08:18.096280 nekograd-0.1.0/nekograd/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/data/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/data/split.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/data/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:08:18.096280 nekograd-0.1.0/nekograd/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/metrics/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/metrics/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:08:18.100280 nekograd-0.1.0/nekograd/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/model/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/model/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:08:18.100280 nekograd-0.1.0/nekograd/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/torch/criterion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-15 09:08:08.000000 nekograd-0.1.0/nekograd/torch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:08:18.096280 nekograd-0.1.0/nekograd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-15 09:08:18.000000 nekograd-0.1.0/nekograd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-15 09:08:18.000000 nekograd-0.1.0/nekograd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 09:08:18.000000 nekograd-0.1.0/nekograd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-15 09:08:18.000000 nekograd-0.1.0/nekograd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 09:08:18.000000 nekograd-0.1.0/nekograd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-15 09:08:08.000000 nekograd-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 09:08:18.100280 nekograd-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-15 09:08:08.000000 nekograd-0.1.0/setup.py
```

### Comparing `nekograd-0.0.1/LICENSE` & `nekograd-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nekograd-0.0.1/PKG-INFO` & `nekograd-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nekograd
-Version: 0.0.1
+Version: 0.1.0
 Home-page: https://github.com/arseniybelkov/nekograd
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nekograd
```

### Comparing `nekograd-0.0.1/README.md` & `nekograd-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nekograd-0.0.1/nekograd/data/module.py` & `nekograd-0.1.0/nekograd/data/module.py`

 * *Files identical despite different names*

### Comparing `nekograd-0.0.1/nekograd/data/split.py` & `nekograd-0.1.0/nekograd/data/split.py`

 * *Files identical despite different names*

### Comparing `nekograd-0.0.1/nekograd/data/transforms.py` & `nekograd-0.1.0/nekograd/data/transforms.py`

 * *Files identical despite different names*

### Comparing `nekograd-0.0.1/nekograd/metrics/utils.py` & `nekograd-0.1.0/nekograd/metrics/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from functools import wraps
 from typing import Callable, Sequence, Union
 
 import numpy as np
 from torch import Tensor
 
-from ..torch.utils import to_np
-
+from ..torch.utils import to_np, np2tensor
 
 ArrayLike = Union[np.ndarray, Tensor]
 
 
 def ravel(metric):
     @wraps(metric)
     def wrapper(t: np.ndarray, p: np.ndarray, *args, **kwargs):
@@ -75,25 +74,33 @@
     return wrapper
 
 
 def batched(aggregate: Callable = np.mean):
     def decorator(metric):
         @wraps(metric)
         def wrapper(
-            ts: Sequence[np.ndarray], ps: Sequence[np.ndarray], *args, **kwargs
+                ts: Sequence[np.ndarray], ps: Sequence[np.ndarray], *args, **kwargs
         ):
             return aggregate([metric(t, p, *args, **kwargs) for t, p in zip(ts, ps)])
 
         return wrapper
 
     return decorator
 
 
 def argmax(axis: int = 0):
     def decorator(metric):
         @wraps(metric)
         def wrapper(t: np.ndarray, p: np.ndarray, *args, **kwargs):
-            return metric(t, p.argmax(axis), *args, **kwargs)
+            return metric(t, np.argmax(p, axis), *args, **kwargs)
 
         return wrapper
 
     return decorator
+
+
+def to_tensor(metric):
+    @wraps(metric)
+    def wrapper(t: np.ndarray, p: np.ndarray, *args, **kwargs):
+        return metric(np2tensor(t), np2tensor(p), *args, **kwargs)
+
+    return wrapper
```

### Comparing `nekograd-0.0.1/nekograd/torch/criterion.py` & `nekograd-0.1.0/nekograd/torch/criterion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from inspect import isfunction
 from typing import Callable, Dict, List, Union
 
 import torch
 from cytoolz.functoolz import juxt
+from more_itertools import zip_equal
 
 
 class CriterionDict(torch.nn.Module):
     """
     Parameters
     ----------
     criterions: Callable
@@ -67,15 +68,15 @@
         self.scale = scale
         self.alphas = alphas
         self.criterions = criterions
         self.loss_keys = loss_keys
 
     def forward(self, *args, **kwargs) -> Dict[str, torch.Tensor]:
         loss = {"loss": 0}
-        for _loss, alpha, loss_key in zip(
+        for _loss, alpha, loss_key in zip_equal(
             juxt(self.criterions)(*args, **kwargs), self.alphas, self.loss_keys
         ):
             if isinstance(_loss, (int, float)):
                 _loss = torch.tensor(_loss, dtype=torch.float32).cuda()
             loss["loss"] += _loss * alpha
             loss.update({loss_key: _loss * alpha if self.scale else _loss})
         return loss
```

### Comparing `nekograd-0.0.1/nekograd/torch/utils.py` & `nekograd-0.1.0/nekograd/torch/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from itertools import chain
-from typing import Dict, Sequence, Any, List
+from typing import Dict, Sequence, Any, List, Union
 
 import numpy as np
 import torch
 import torch.nn as nn
 
 
 def switch_grad(*models: nn.Module, mode: bool = False) -> None:
@@ -31,7 +31,13 @@
         return tensor2np(x)
     elif isinstance(x, Dict):
         return tensor_dict2np(x)
     elif isinstance(x, Sequence):
         return tensor_sequence2np(x)
     else:
         return np.asarray(x)
+
+
+def np2tensor(x: Union[torch.Tensor, np.ndarray]) -> torch.Tensor:
+    if isinstance(x, torch.Tensor):
+        return x
+    return torch.from_numpy(np.asarray(x))
```

### Comparing `nekograd-0.0.1/nekograd.egg-info/PKG-INFO` & `nekograd-0.1.0/nekograd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nekograd
-Version: 0.0.1
+Version: 0.1.0
 Home-page: https://github.com/arseniybelkov/nekograd
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nekograd
```

### Comparing `nekograd-0.0.1/nekograd.egg-info/SOURCES.txt` & `nekograd-0.1.0/nekograd.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -13,16 +13,18 @@
 nekograd/data/__init__.py
 nekograd/data/module.py
 nekograd/data/split.py
 nekograd/data/transforms.py
 nekograd/data/utils.py
 nekograd/metrics/__init__.py
 nekograd/metrics/binary.py
+nekograd/metrics/checks.py
 nekograd/metrics/utils.py
 nekograd/model/__init__.py
 nekograd/model/base.py
 nekograd/model/commands.py
 nekograd/model/model.py
+nekograd/model/policy.py
+nekograd/model/utils.py
 nekograd/torch/__init__.py
 nekograd/torch/criterion.py
-nekograd/torch/utils.py
-tests/test_model.py
+nekograd/torch/utils.py
```

### Comparing `nekograd-0.0.1/setup.py` & `nekograd-0.1.0/setup.py`

 * *Files identical despite different names*

