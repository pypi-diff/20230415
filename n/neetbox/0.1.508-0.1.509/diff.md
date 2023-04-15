# Comparing `tmp/neetbox-0.1.508.tar.gz` & `tmp/neetbox-0.1.509.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neetbox-0.1.508.tar", max compression
+gzip compressed data, was "neetbox-0.1.509.tar", max compression
```

## Comparing `neetbox-0.1.508.tar` & `neetbox-0.1.509.tar`

### file list

```diff
@@ -1,41 +1,43 @@
--rw-r--r--   0        0        0     1067 2023-04-14 10:45:41.754661 neetbox-0.1.508/LICENSE
--rw-r--r--   0        0        0      397 2023-04-14 10:45:41.754661 neetbox-0.1.508/README.md
--rw-r--r--   0        0        0     2824 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/cli/__init__.py
--rw-r--r--   0        0        0     2910 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/cli/parse.py
--rw-r--r--   0        0        0     1154 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/config/__init__.py
--rw-r--r--   0        0        0     1385 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/config/_config.py
--rw-r--r--   0        0        0     2541 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/daemon/__init__.py
--rw-r--r--   0        0        0      608 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/daemon/_apis.py
--rw-r--r--   0        0        0     1904 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/daemon/_daemon.py
--rw-r--r--   0        0        0     4398 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/daemon/_daemon_client.py
--rw-r--r--   0        0        0      409 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/integrations/__init__.py
--rw-r--r--   0        0        0     1182 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/integrations/engine.py
--rw-r--r--   0        0        0     7527 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/integrations/environment.py
--rw-r--r--   0        0        0     8229 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/integrations/resource.py
--rw-r--r--   0        0        0      313 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/logging/__init__.py
--rw-r--r--   0        0        0     2106 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/logging/_colorama.py
--rw-r--r--   0        0        0    12181 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/logging/flfs/ansiregular.flf
--rw-r--r--   0        0        0    12181 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/logging/flfs/ansishadow.flf
--rw-r--r--   0        0        0    11585 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/logging/flfs/isometrixc2.flf
--rw-r--r--   0        0        0    23112 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/logging/flfs/nscripts.flf
--rw-r--r--   0        0        0    21669 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/logging/flfs/nvscript.flf
--rw-r--r--   0        0        0     3921 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/logging/formatting.py
--rw-r--r--   0        0        0    18647 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/logging/logger.py
--rw-r--r--   0        0        0       54 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/pipeline/__init__.py
--rw-r--r--   0        0        0      281 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/pipeline/pipe.py
--rw-r--r--   0        0        0     5594 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/pipeline/registry.py
--rw-r--r--   0        0        0        0 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/plotting/__init__.py
--rw-r--r--   0        0        0     4922 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/plotting/plot.py
--rw-r--r--   0        0        0      115 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/torch/__init__.py
--rw-r--r--   0        0        0     5227 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/torch/arch/canny.py
--rw-r--r--   0        0        0     6437 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/torch/arch/cnn.py
--rw-r--r--   0        0        0     2319 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/torch/arch/kernels.py
--rw-r--r--   0        0        0     2440 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/torch/arch/mask_boundary_finder.py
--rw-r--r--   0        0        0     3678 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/torch/nlp.py
--rw-r--r--   0        0        0     4481 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/torch/profile.py
--rw-r--r--   0        0        0        0 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/utils/__init__.py
--rw-r--r--   0        0        0     2303 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/utils/framing.py
--rw-r--r--   0        0        0     2165 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/utils/utils.py
--rw-r--r--   0        0        0     1332 2023-04-14 10:45:41.762662 neetbox-0.1.508/pyproject.toml
--rw-r--r--   0        0        0     1962 1970-01-01 00:00:00.000000 neetbox-0.1.508/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-15 10:16:55.167917 neetbox-0.1.509/LICENSE
+-rw-r--r--   0        0        0      397 2023-04-15 10:16:55.167917 neetbox-0.1.509/README.md
+-rw-r--r--   0        0        0     2827 2023-04-15 10:16:55.171917 neetbox-0.1.509/neetbox/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 10:16:55.171917 neetbox-0.1.509/neetbox/cli/__init__.py
+-rw-r--r--   0        0        0     2910 2023-04-15 10:16:55.171917 neetbox-0.1.509/neetbox/cli/parse.py
+-rw-r--r--   0        0        0     1154 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/config/__init__.py
+-rw-r--r--   0        0        0     1385 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/config/_config.py
+-rw-r--r--   0        0        0       66 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/core/__init__.py
+-rw-r--r--   0        0        0     5864 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/core/registry.py
+-rw-r--r--   0        0        0     2878 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/daemon/__init__.py
+-rw-r--r--   0        0        0      608 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/daemon/_apis.py
+-rw-r--r--   0        0        0     1938 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/daemon/_daemon.py
+-rw-r--r--   0        0        0     4851 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/daemon/_daemon_client.py
+-rw-r--r--   0        0        0     3226 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/daemon/_win_service.py
+-rw-r--r--   0        0        0      378 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/integrations/__init__.py
+-rw-r--r--   0        0        0     1182 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/integrations/engine.py
+-rw-r--r--   0        0        0     4875 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/integrations/environment.py
+-rw-r--r--   0        0        0     8493 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/integrations/resource.py
+-rw-r--r--   0        0        0      313 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/logging/__init__.py
+-rw-r--r--   0        0        0     2106 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/logging/_colorama.py
+-rw-r--r--   0        0        0    12181 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/logging/flfs/ansiregular.flf
+-rw-r--r--   0        0        0    12181 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/logging/flfs/ansishadow.flf
+-rw-r--r--   0        0        0    11585 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/logging/flfs/isometrixc2.flf
+-rw-r--r--   0        0        0    23112 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/logging/flfs/nscripts.flf
+-rw-r--r--   0        0        0    21669 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/logging/flfs/nvscript.flf
+-rw-r--r--   0        0        0     3921 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/logging/formatting.py
+-rw-r--r--   0        0        0    18647 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/logging/logger.py
+-rw-r--r--   0        0        0        0 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/pipeline/__init__.py
+-rw-r--r--   0        0        0      277 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/pipeline/pipe.py
+-rw-r--r--   0        0        0        0 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/plotting/__init__.py
+-rw-r--r--   0        0        0     4922 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/plotting/plot.py
+-rw-r--r--   0        0        0      108 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/torch/__init__.py
+-rw-r--r--   0        0        0     5227 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/torch/arch/canny.py
+-rw-r--r--   0        0        0     6437 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/torch/arch/cnn.py
+-rw-r--r--   0        0        0     2312 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/torch/arch/kernels.py
+-rw-r--r--   0        0        0     2440 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/torch/arch/mask_boundary_finder.py
+-rw-r--r--   0        0        0     3678 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/torch/nlp.py
+-rw-r--r--   0        0        0     4474 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/torch/profile.py
+-rw-r--r--   0        0        0       76 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/utils/__init__.py
+-rw-r--r--   0        0        0     2303 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/utils/framing.py
+-rw-r--r--   0        0        0     4780 2023-04-15 10:16:55.175917 neetbox-0.1.509/neetbox/utils/utils.py
+-rw-r--r--   0        0        0     1264 2023-04-15 10:16:55.175917 neetbox-0.1.509/pyproject.toml
+-rw-r--r--   0        0        0     1838 1970-01-01 00:00:00.000000 neetbox-0.1.509/PKG-INFO
```

### Comparing `neetbox-0.1.508/LICENSE` & `neetbox-0.1.509/LICENSE`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.508/neetbox/__init__.py` & `neetbox-0.1.509/neetbox/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,22 @@
 from neetbox.config._config import update_with
 from neetbox.daemon import _try_attach_daemon
 from neetbox.utils.framing import get_frame_module_traceback
 
 module = get_frame_module_traceback(1).__name__
 config_file_name = f"{module}.toml"
 
+
 def post_init():
     import setproctitle
-    project_name = get_module_level_config()['name']
+
+    project_name = get_module_level_config()["name"]
     setproctitle.setproctitle(project_name)
 
+
 def init(path=None, load=False, **kwargs) -> bool:
     if path:
         os.chdir(path=path)
     current_path = os.getcwd()
     config_file_path = os.path.join(current_path, config_file_name)
 
     if not load:
```

### Comparing `neetbox-0.1.508/neetbox/cli/parse.py` & `neetbox-0.1.509/neetbox/cli/parse.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.508/neetbox/config/__init__.py` & `neetbox-0.1.509/neetbox/config/__init__.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.508/neetbox/config/_config.py` & `neetbox-0.1.509/neetbox/config/_config.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.508/neetbox/daemon/_apis.py` & `neetbox-0.1.509/neetbox/daemon/_apis.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.508/neetbox/daemon/_daemon.py` & `neetbox-0.1.509/neetbox/daemon/_daemon.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 #
 # Author: GavinGong aka VisualDust
 # URL:    https://gong.host
 # Date:   20230414
 
-from flask import Flask, json, abort, request
+from neetbox.utils import pkg
 from neetbox.config import get_module_level_config
 from threading import Thread
 import time
 import sys
 
 _STAT_POOL = {}
 __DAEMON_SHUTDOWN_IF_NO_UPLOAD_TIMEOUT_SEC = 60 * 60
@@ -17,14 +17,15 @@
 
 
 def daemon_process(daemon_config=None):
     import setproctitle
 
     setproctitle.setproctitle(__DAEMON_NAME)
     daemon_config = daemon_config or get_module_level_config()
+    from flask import Flask, json, abort, request
     api = Flask(__DAEMON_NAME)
 
     @api.route("/hello", methods=["GET"])
     def just_send_hello():
         return json.dumps({"hello": "hello"})
 
     @api.route("/status", methods=["GET"], defaults={"name": None})
```

### Comparing `neetbox-0.1.508/neetbox/daemon/_daemon_client.py` & `neetbox-0.1.509/neetbox/daemon/_daemon_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,45 +4,55 @@
 # URL:    https://gong.host
 # Date:   20230414
 
 import requests
 import time
 import json
 from datetime import datetime
-from typing import Callable
+from typing import Callable, Any
 from threading import Thread
 from functools import partial
 from neetbox.config import get_module_level_config
 from neetbox.logging import logger
+from neetbox.core import Registry
 
-_update_queue_dict = {}
+_update_queue_dict = Registry("daemon")
 __TIME_UNIT_SEC = 0.1
 __TIME_CTR_MAX_CYCLE = 9999999
 _update_value_dict = {}
 
 
 class _WatchConfig(dict):
     def __init__(self, name, freq, initiative=False, to_log=False):
         self["name"] = name
         self["freq"] = freq
         self["initiative"] = initiative
         self["to_log"] = to_log
 
 
+class _WatchedFun:
+    def __init__(self, func, others) -> None:
+        self.func = func
+        self.others = others
+
+    def __call__(self, *args: Any, **kwds: Any) -> Any:
+        return self.func(*args, **kwds)
+
+
 def __get(name):
     _the_value = _update_value_dict.get(name, None)
     if _the_value and "value" in _the_value:
         _the_value = _the_value["value"]
     return _the_value
 
 
 def __update_and_get(name):
-    _vtuple = _update_queue_dict[name]
-    _watch_config, _vfun = _vtuple
-    _the_value = _vfun()
+    _watched_fun: _WatchedFun = _update_queue_dict[name]
+    _watch_config = _watched_fun.others
+    _the_value = _watched_fun()
     _update_value_dict[name] = {
         "value": _the_value,
         "timestamp": datetime.timestamp(datetime.now()),
         "interval": (_watch_config["freq"] * __TIME_UNIT_SEC),
     }
     return _the_value
 
@@ -50,17 +60,21 @@
 def _watch(func: Callable, name: str, freq: float, initiative=False, to_log=False):
     """Function decorator to let the daemon watch a value of the function
 
     Args:
         func (function): A function returns a tuple '(name,value)'. 'name' represents the name of the value.
     """
     name = name or func.__name__
-    _update_queue_dict[name] = (
-        _WatchConfig(name, freq=freq, initiative=initiative, to_log=to_log),
-        func,
+    _update_queue_dict._register(
+        name=name,
+        what= _WatchedFun(
+            func=func,
+            others=_WatchConfig(name, freq=freq, initiative=initiative, to_log=to_log),
+        ),
+        force=True,
     )
     if (
         initiative
     ):  # initiatively update the value dict when the function was called manually
         logger.log(
             f"added {name} to daemon monitor. It will update on each call of the function."
         )
@@ -76,22 +90,26 @@
     if not initiative:  # passively update
         freq = freq or get_module_level_config()["updateInterval"]
     else:
         freq = __TIME_CTR_MAX_CYCLE + 1
     return partial(_watch, name=name, freq=freq, initiative=initiative, to_log=to_log)
 
 
+def listen(name=None):
+    pass  # todo
+
+
 def _update_thread():
     # update values
     _ctr = 0
     while True:
         _ctr = (_ctr + 1) % __TIME_CTR_MAX_CYCLE
         time.sleep(__TIME_UNIT_SEC)
-        for _vname, _vtuple in _update_queue_dict.items():
-            _watch_config, _vfun = _vtuple
+        for _vname, _watched_fun in _update_queue_dict.items():
+            _watch_config = _watched_fun.others
             if (
                 not _watch_config["initiative"] and _ctr % _watch_config["freq"] == 0
             ):  # do update
                 _the_value = __update_and_get(_vname)
 
 
 update_thread = Thread(target=_update_thread, daemon=True)
```

### Comparing `neetbox-0.1.508/neetbox/integrations/engine.py` & `neetbox-0.1.509/neetbox/integrations/engine.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.508/neetbox/integrations/resource.py` & `neetbox-0.1.509/neetbox/integrations/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # -*- coding: utf-8 -*-
 #
 # Author: GavinGong aka VisualDust
 # URL:    https://gong.host
 # Date:   20230315
 
-from PIL import Image
 from random import random
 import os
 import asyncio
 import numpy as np
 import threading
-from neetbox.integrations import pkg
+from neetbox.utils import pkg
 from neetbox.logging import logger
 from neetbox.integrations import engine
 from typing import Dict
 import pathlib
 import urllib.request
 from tqdm import tqdm
 from typing import List, Union, Dict, Any
@@ -111,14 +110,20 @@
         if not self._ready:
             raise Exception("not ready.")
         if type(index) is int:
             return self.file_path_list[index]
 
 
 class ImagesLoader(ResourceLoader):
+    
+    def __init__(self, folder, file_types=["png", "jpg"], sub_dirs=True, async_scan=False, verbose=False):
+        pkg.is_installed('PIL', try_install_if_not='pillow')
+        from PIL import Image
+        super().__init__(folder, file_types, sub_dirs, async_scan, verbose)
+        
     def get_random_image(self):
         rand_img_path = self.file_path_list[int(random() * len(self.file_path_list))]
         image = Image.open(rand_img_path).convert("RGB")
         return image
 
     def get_random_images(self, howmany=1):
         assert howmany < len(self.file_path_list)
```

### Comparing `neetbox-0.1.508/neetbox/logging/_colorama.py` & `neetbox-0.1.509/neetbox/logging/_colorama.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.508/neetbox/logging/flfs/ansiregular.flf` & `neetbox-0.1.509/neetbox/logging/flfs/ansiregular.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.508/neetbox/logging/flfs/ansishadow.flf` & `neetbox-0.1.509/neetbox/logging/flfs/ansishadow.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.508/neetbox/logging/flfs/isometrixc2.flf` & `neetbox-0.1.509/neetbox/logging/flfs/isometrixc2.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.508/neetbox/logging/flfs/nscripts.flf` & `neetbox-0.1.509/neetbox/logging/flfs/nscripts.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.508/neetbox/logging/flfs/nvscript.flf` & `neetbox-0.1.509/neetbox/logging/flfs/nvscript.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.508/neetbox/logging/formatting.py` & `neetbox-0.1.509/neetbox/logging/formatting.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.508/neetbox/logging/logger.py` & `neetbox-0.1.509/neetbox/logging/logger.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.508/neetbox/pipeline/registry.py` & `neetbox-0.1.509/neetbox/core/registry.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,135 +9,110 @@
 from typing import Optional, Union, Sequence
 import inspect
 import json
 import functools
 from typing import Any, Callable, Dict, List, Optional, Sequence, Union
 
 
+class _RegEndpoint:
+    def __init__(self, what, tags=None):
+        """Generate a massive type which contains both the regietered object and it's tags
+
+        Args:
+            what (_type_): The object being registered
+            tags (_type_, optional): The tags. Defaults to None.
+        """
+        self.what = what
+        self.tags = tags
+
+    def __str__(self) -> str:
+        return f"{self.what} with tags: {self.tags}"
+
+
 class Registry(dict):
+
     """Register Helper Class
     A Register is a 'dict[str:any]'
     Registers are stored in a pool of type dict[str:Register]
     """
 
     # class level
     _registry_pool: Dict[str, "Registry"] = dict()  # all registeres are stored here
 
-    # instance level
-    initialized: bool = False
-
     def __new__(cls, name: str) -> "Registry":
         assert is_pure_ansi(name), "Registry name should not contain non-ansi char."
         if name in cls._registry_pool:
             return cls._registry_pool[name]
-        logger.log(f"Creating Registry for {cls}")
+        logger.log(f"Creating Registry for '{name}'")
         instance = dict.__new__(cls)
         cls._registry_pool[name] = instance
         return instance
 
     # not compatible with python below 3.8
-    def __init__(self, name: str) -> None:
-        if not self.initialized:
-            # do initializations
+    def __init__(self, name, *args, **kwargs) -> None:
+        if not "initialized" in self:
+            self["initialized"] = True
             self.name = name
-            self.initialized = True
 
     def _register(
         self,
         what: Any,
         name: Optional[str] = None,
-        force: bool = False,
+        force: bool = True,
         tags: Optional[Union[str, Sequence[str]]] = None,
     ):
-        if not (inspect.isfunction(what) or inspect.isclass(what)):
-            logger.warn("Registering {type(what)}, which is not a class or a callable.")
+        # if not (inspect.isfunction(what) or inspect.isclass(what)):
+        #     logger.warn(f"Registering {type(what)}, which is not a class or a callable.")
         name = name or what.__name__
         if type(tags) is str:
             tags = [tags]
+        _endp = _RegEndpoint(what, tags)
         if name in self.keys():
             if not force:
                 logger.warn(
                     f"{name} already exists in Registry:{self.name}. If you want to overwrite, try to register with 'force=True'"
                 )
             else:
-                logger.warn(f"Overwritting: {name} existed in Registry:{self.name}.")
-                self[name] = (what, tags)
+                logger.warn(
+                    f"Overwritting existing '{name}' in Registry '{self.name}'."
+                )
+                self[name] = _endp
         else:
-            self[name] = (what, tags)
+            self[name] = _endp
         return what
 
     def register(
         self,
         *,
         name: Optional[str] = None,
-        force: bool = False,
+        force: bool = True,
         tags: Optional[Union[str, Sequence[str]]] = None,
-    ) -> Callable:
-        return functools.partial(
-            self._register, name=name, force=force, tags=tags
-        )
-
-    def register_all(
-        self,
-        what: Union[Dict, Sequence[Callable]],
-        names: Optional[Sequence[str]] = None,
-        tags: Optional[Union[str, Sequence[str]]] = None,
-        force: bool = False,
-    ) -> None:
-        if type(what) is dict:
-            _names = what.keys()
-            what = what.values()
-        if type(what) is list:
-            _names = names if names else [None] * len(what)
-            for module, name, info in zip(what, _names, tags):
-                self._register(module, force=force, name=name, tags=tags)
-        else:
-            logger.err(
-                ValueError(
-                    f"Unsupported format of 'what'. Please use list or dict(tuple)."
-                ),
-                reraise=True,
-            )
-
-    def merge(
-        self,
-        others: Union["Registry", List["Registry"]],
-        force: bool = False,
-    ) -> None:
-        if not isinstance(others, list):
-            others = [others]
-        if not isinstance(others[0], Registry):
-            logger.err(
-                TypeError("Expect `Registry` type, but got {}".format(type(others[0]))),
-                reraise=True,
-            )
-        for other in others:
-            self.register_all(other, force=force)
+    ):
+        return functools.partial(self._register, name=name, force=force, tags=tags)
 
     @classmethod
     def find(
         cls,
         name: Optional[str] = None,
         tags: Optional[Union[str, List[str]]] = None,
-        default=None,
     ):
         if not name and not tags:
             logger.err(
                 ValueError(
                     "Please provide at least the name or the tags you want to find."
                 ),
                 reraise=True,
             )
         results = []
         # filter name
         for reg_name, reg in cls._registry_pool.items():
             private_sign = "__"
             if not reg_name.startswith(private_sign):
                 if not name:
-                    results += [(_n, _o) for _n, _o in reg.items()]
+                    results += [(_n, _o) for _n, _o in reg.items(_real_type=False)]
                 elif name in reg:
                     results.append((name, reg[name]))
 
         # filter tags
         if type(tags) is str:
             tags = [tags]
 
@@ -145,33 +120,80 @@
             # check if all tags in f_tags are listed in s_tags
             for _t in f_tags:
                 if _t not in s_tags:
                     return False
             return True
 
         results = {
-            _name: obj_tag_pair[0]
-            for _name, obj_tag_pair in results
-            if _tags_match(tags, obj_tag_pair[1])
+            _name: _endp.what
+            for _name, _endp in results
+            if _tags_match(tags, _endp.tags)
         }
         return results
 
     def __getitem__(self, __key: str) -> Any:
-        return super().__getitem__(__key)[0]
+        _v = self.__dict__[__key]
+        if type(_v) is _RegEndpoint:
+            _v = _v.what
+        return _v
 
     def __setitem__(self, k, v) -> None:
         assert is_pure_ansi(k), "Only ANSI chars are allowed for registering things."
-        if type(v) is not tuple:
-            v = (v, None)
-        if len(v) != 2:
-            raise ValueError("Only support value of format (object, list(str))")
-        super().__setitem__(k, v)
+        self.__dict__[k] = v
+
+    def clear(self):
+        return self.__dict__.clear()
+
+    def copy(self):
+        return self.__dict__.copy()
+
+    def has_key(self, k):
+        return k in self.__dict__
+
+    def update(self, *args, **kwargs):
+        return self.__dict__.update(*args, **kwargs)
+
+    def keys(self):
+        return [
+            _item[0]
+            for _item in self.__dict__.items()
+            if type(_item[1]) is _RegEndpoint
+        ]
+
+    def values(self):
+        return [
+            _item[1].what
+            for _item in self.__dict__.items()
+            if type(_item[1]) is _RegEndpoint
+        ]
+
+    def items(self, _real_type=True):
+        _legal_items = [
+            _item for _item in self.__dict__.items() if type(_item[1]) is _RegEndpoint
+        ]
+        if _real_type:
+            _legal_items = [
+                (_k, _v.what) for _k, _v in _legal_items if type(_v) is _RegEndpoint
+            ]
+        return _legal_items
+
+    def pop(self, *args):
+        return self.__dict__.pop(*args)
+
+    def __cmp__(self, dict_):
+        return self.__cmp__(self.__dict__, dict_)
+
+    def __contains__(self, item):
+        return item in self.__dict__
+
+    def __iter__(self):
+        return iter(self.__dict__)
 
     def __str__(self) -> str:
         return json.dumps(
-            self,
+            dict(self.items()),
             indent=4,
             ensure_ascii=False,
             sort_keys=False,
             separators=(",", ":"),
             default=str,
         )
```

### Comparing `neetbox-0.1.508/neetbox/plotting/plot.py` & `neetbox-0.1.509/neetbox/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.508/neetbox/torch/arch/canny.py` & `neetbox-0.1.509/neetbox/torch/arch/canny.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.508/neetbox/torch/arch/cnn.py` & `neetbox-0.1.509/neetbox/torch/arch/cnn.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.508/neetbox/torch/arch/kernels.py` & `neetbox-0.1.509/neetbox/torch/arch/kernels.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from neetbox.integrations import pkg
+from neetbox.utils import pkg
 
 
 def get_gaussian_kernel(k=3, mu=0, sigma=1, normalize=True):
     # compute 1 dimension gaussian
     gaussian_1D = np.linspace(-1, 1, k)
     # compute a grid distance from center
     x, y = np.meshgrid(gaussian_1D, gaussian_1D)
```

### Comparing `neetbox-0.1.508/neetbox/torch/arch/mask_boundary_finder.py` & `neetbox-0.1.509/neetbox/torch/arch/mask_boundary_finder.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.508/neetbox/torch/nlp.py` & `neetbox-0.1.509/neetbox/torch/nlp.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.508/neetbox/torch/profile.py` & `neetbox-0.1.509/neetbox/torch/profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 #
 # Author: GavinGong aka VisualDust
 # URL:    https://gong.host
 # Date:   20230315
 
-from neetbox.integrations import pkg
+from neetbox.utils import pkg
 import time
 from tqdm import tqdm
 import torch
 
 from neetbox.logging import logger
```

### Comparing `neetbox-0.1.508/neetbox/utils/framing.py` & `neetbox-0.1.509/neetbox/utils/framing.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.508/pyproject.toml` & `neetbox-0.1.509/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neetbox"
-version = "0.1.508"
+version = "0.1.509"
 description = "NEETBox contains useless CV code snippets."
 license = "MIT"
 authors = ["VisualDust <gavin@gong.host>"]
 maintainers = [
     "VisualDust <gavin@gong.host>",
     "PommesPeter <me@pommespeter.space>",
     "PaperCube <imzhy@hotmail.com>"
@@ -30,25 +30,21 @@
 # name = "pypi"
 # url = "https://pypi.org/simple"
 # default = true
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 numpy = ">=1"
-pillow = ">=8"
-pandas = ">=1"
 tqdm = ">=4"
 colorama = ">=0.3"
 toml = ">0.10"
-pytest = "*"
 gputil = ">=1.4"
 psutil = ">=5.0"
 injector = ">=0.20"
 pyfiglet = ">=0.8"
-python-daemon = "^3.0.1"
 flask = "^2.2.3"
 setproctitle = "^1.3.2"
 requests = "^2.28.2"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `neetbox-0.1.508/PKG-INFO` & `neetbox-0.1.509/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neetbox
-Version: 0.1.508
+Version: 0.1.509
 Summary: NEETBox contains useless CV code snippets.
 Home-page: https://neetbox.550w.host
 License: MIT
 Keywords: computer vision,tools,logging
 Author: VisualDust
 Author-email: gavin@gong.host
 Maintainer: VisualDust
@@ -25,20 +25,16 @@
 Classifier: Topic :: System :: Logging
 Classifier: Topic :: Utilities
 Requires-Dist: colorama (>=0.3)
 Requires-Dist: flask (>=2.2.3,<3.0.0)
 Requires-Dist: gputil (>=1.4)
 Requires-Dist: injector (>=0.20)
 Requires-Dist: numpy (>=1)
-Requires-Dist: pandas (>=1)
-Requires-Dist: pillow (>=8)
 Requires-Dist: psutil (>=5.0)
 Requires-Dist: pyfiglet (>=0.8)
-Requires-Dist: pytest
-Requires-Dist: python-daemon (>=3.0.1,<4.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: setproctitle (>=1.3.2,<2.0.0)
 Requires-Dist: toml (>0.10)
 Requires-Dist: tqdm (>=4)
 Project-URL: Repository, https://github.com/visualDust/neetbox
 Description-Content-Type: text/markdown
```

