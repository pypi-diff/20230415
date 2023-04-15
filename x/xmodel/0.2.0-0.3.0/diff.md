# Comparing `tmp/xmodel-0.2.0.tar.gz` & `tmp/xmodel-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmodel-0.2.0.tar", max compression
+gzip compressed data, was "xmodel-0.3.0.tar", max compression
```

## Comparing `xmodel-0.2.0.tar` & `xmodel-0.3.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0     1211 2023-04-13 18:35:37.993890 xmodel-0.2.0/LICENSE
--rw-r--r--   0        0        0      697 2023-04-13 18:35:37.993890 xmodel-0.2.0/README.md
--rw-r--r--   0        0        0     1965 2023-04-13 18:35:37.997890 xmodel-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    20864 2023-04-13 18:35:37.997890 xmodel-0.2.0/xmodel/__init__.py
--rw-r--r--   0        0        0       18 2023-04-13 18:35:37.997890 xmodel-0.2.0/xmodel/_private/__init__.py
--rw-r--r--   0        0        0       33 2023-04-13 18:35:37.997890 xmodel-0.2.0/xmodel/_private/api/__init__.py
--rw-r--r--   0        0        0     7004 2023-04-13 18:35:37.997890 xmodel-0.2.0/xmodel/_private/api/state.py
--rw-r--r--   0        0        0      828 2023-04-13 18:35:37.997890 xmodel-0.2.0/xmodel/_private/api/utils.py
--rw-r--r--   0        0        0      191 2023-04-13 18:35:37.997890 xmodel-0.2.0/xmodel/base/__init__.py
--rw-r--r--   0        0        0    48954 2023-04-13 18:35:37.997890 xmodel-0.2.0/xmodel/base/api.py
--rw-r--r--   0        0        0    35399 2023-04-13 18:35:37.997890 xmodel-0.2.0/xmodel/base/fields.py
--rw-r--r--   0        0        0    29421 2023-04-13 18:35:37.997890 xmodel-0.2.0/xmodel/base/model.py
--rw-r--r--   0        0        0    21759 2023-04-13 18:35:37.997890 xmodel-0.2.0/xmodel/base/structure.py
--rw-r--r--   0        0        0        1 2023-04-13 18:35:38.001890 xmodel-0.2.0/xmodel/common/__init__.py
--rw-r--r--   0        0        0    13351 2023-04-13 18:35:38.001890 xmodel-0.2.0/xmodel/common/children.py
--rw-r--r--   0        0        0     1943 2023-04-13 18:35:38.001890 xmodel-0.2.0/xmodel/common/lazy.py
--rw-r--r--   0        0        0      963 2023-04-13 18:35:38.001890 xmodel-0.2.0/xmodel/common/types.py
--rw-r--r--   0        0        0     1635 2023-04-13 18:35:38.001890 xmodel-0.2.0/xmodel/common/unwrap.py
--rw-r--r--   0        0        0     2555 2023-04-13 18:35:38.001890 xmodel-0.2.0/xmodel/common/utils.py
--rw-r--r--   0        0        0     7716 2023-04-13 18:35:38.001890 xmodel-0.2.0/xmodel/converters.py
--rw-r--r--   0        0        0       89 2023-04-13 18:35:38.001890 xmodel-0.2.0/xmodel/errors.py
--rw-r--r--   0        0        0      804 2023-04-13 18:35:38.001890 xmodel-0.2.0/xmodel/json.py
--rw-r--r--   0        0        0      273 2023-04-13 18:35:38.001890 xmodel-0.2.0/xmodel/remote/__init__.py
--rw-r--r--   0        0        0    30701 2023-04-13 18:35:38.001890 xmodel-0.2.0/xmodel/remote/api.py
--rw-r--r--   0        0        0     7828 2023-04-13 18:35:38.001890 xmodel-0.2.0/xmodel/remote/client.py
--rw-r--r--   0        0        0      301 2023-04-13 18:35:38.001890 xmodel-0.2.0/xmodel/remote/errors.py
--rw-r--r--   0        0        0     2235 2023-04-13 18:35:38.001890 xmodel-0.2.0/xmodel/remote/model.py
--rw-r--r--   0        0        0     3112 2023-04-13 18:35:38.001890 xmodel-0.2.0/xmodel/remote/options.py
--rw-r--r--   0        0        0    12775 2023-04-13 18:35:38.001890 xmodel-0.2.0/xmodel/remote/response_state.py
--rw-r--r--   0        0        0     6709 2023-04-13 18:35:38.001890 xmodel-0.2.0/xmodel/remote/structure.py
--rw-r--r--   0        0        0     7935 2023-04-13 18:35:38.001890 xmodel-0.2.0/xmodel/remote/weak_cache_pool.py
--rw-r--r--   0        0        0     1645 1970-01-01 00:00:00.000000 xmodel-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-04-15 03:16:28.299921 xmodel-0.3.0/LICENSE
+-rw-r--r--   0        0        0      697 2023-04-15 03:16:28.299921 xmodel-0.3.0/README.md
+-rw-r--r--   0        0        0     1965 2023-04-15 03:16:28.299921 xmodel-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    20864 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/__init__.py
+-rw-r--r--   0        0        0       18 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/_private/__init__.py
+-rw-r--r--   0        0        0       33 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/_private/api/__init__.py
+-rw-r--r--   0        0        0     7004 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/_private/api/state.py
+-rw-r--r--   0        0        0      828 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/_private/api/utils.py
+-rw-r--r--   0        0        0      191 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/base/__init__.py
+-rw-r--r--   0        0        0    48954 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/base/api.py
+-rw-r--r--   0        0        0    35396 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/base/fields.py
+-rw-r--r--   0        0        0    29418 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/base/model.py
+-rw-r--r--   0        0        0    21759 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/base/structure.py
+-rw-r--r--   0        0        0        1 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/common/__init__.py
+-rw-r--r--   0        0        0    13348 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/common/children.py
+-rw-r--r--   0        0        0     1943 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/common/lazy.py
+-rw-r--r--   0        0        0      963 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/common/types.py
+-rw-r--r--   0        0        0     1635 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/common/unwrap.py
+-rw-r--r--   0        0        0     2555 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/common/utils.py
+-rw-r--r--   0        0        0     7716 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/converters.py
+-rw-r--r--   0        0        0       89 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/errors.py
+-rw-r--r--   0        0        0      804 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/json.py
+-rw-r--r--   0        0        0      273 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/remote/__init__.py
+-rw-r--r--   0        0        0    30698 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/remote/api.py
+-rw-r--r--   0        0        0     7828 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/remote/client.py
+-rw-r--r--   0        0        0      301 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/remote/errors.py
+-rw-r--r--   0        0        0     2235 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/remote/model.py
+-rw-r--r--   0        0        0     3112 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/remote/options.py
+-rw-r--r--   0        0        0    12775 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/remote/response_state.py
+-rw-r--r--   0        0        0     6709 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/remote/structure.py
+-rw-r--r--   0        0        0     7935 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/remote/weak_cache_pool.py
+-rw-r--r--   0        0        0      240 2023-04-15 03:16:28.303921 xmodel-0.3.0/xmodel/util.py
+-rw-r--r--   0        0        0     1645 1970-01-01 00:00:00.000000 xmodel-0.3.0/PKG-INFO
```

### Comparing `xmodel-0.2.0/LICENSE` & `xmodel-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xmodel-0.2.0/README.md` & `xmodel-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `xmodel-0.2.0/pyproject.toml` & `xmodel-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xmodel"
-version = "0.2.0"
+version = "0.3.0"
 description = "Models for working with JSON, ie: JsonModel"
 authors = ["Josh Orr <josh@orr.blue>"]
 packages = [{include = "xmodel"}]
 readme = "README.md"
 license = "The Unlicense (Unlicense)"
 repository = "https://github.com/xyngular/py-xmodel"
```

### Comparing `xmodel-0.2.0/xmodel/__init__.py` & `xmodel-0.3.0/xmodel/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -497,8 +497,8 @@
     'BaseStructure',
     'Field',
     'Converter',
     'XModelError',
     'JsonModel'
 ]
 
-__version__ = '0.2.0'
+__version__ = '0.3.0'
```

### Comparing `xmodel-0.2.0/xmodel/_private/api/state.py` & `xmodel-0.3.0/xmodel/_private/api/state.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.2.0/xmodel/_private/api/utils.py` & `xmodel-0.3.0/xmodel/_private/api/utils.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.2.0/xmodel/base/api.py` & `xmodel-0.3.0/xmodel/base/api.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.2.0/xmodel/base/fields.py` & `xmodel-0.3.0/xmodel/base/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from xsentinels.default import Default
 import dataclasses
 from enum import Enum, auto as EnumAuto  # noqa
 from xmodel.errors import XModelError
 from copy import copy
 import typing_inspect
 import inspect
-from xloop import xloop as loop
+from xmodel.util import loop
 
 if TYPE_CHECKING:
     from xmodel import BaseModel
     from xmodel import BaseApi
 
 T = TypeVar("T")
```

### Comparing `xmodel-0.2.0/xmodel/base/model.py` & `xmodel-0.3.0/xmodel/base/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from abc import ABC
 import inspect
 import typing_inspect
 from xmodel.common.types import JsonDict
 
 from xsentinels.null import Null, NullType
 from xsentinels.default import Default
-from xloop import xloop as loop
+from xmodel.util import loop
 
 from xmodel.base.fields import Field, Converter
 from xmodel import _private
 from xmodel.errors import XModelError
 
 if TYPE_CHECKING:
     # Allows IDE to get type reference without a circular import issue.
```

### Comparing `xmodel-0.2.0/xmodel/base/structure.py` & `xmodel-0.3.0/xmodel/base/structure.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.2.0/xmodel/common/children.py` & `xmodel-0.3.0/xmodel/common/children.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import typing_inspect
 import inspect
 from dataclasses import dataclass
 
 from xinject.context import XContext
 from xsentinels.default import Default
 from xsentinels.null import Null
-from xloop import xloop as loop
+from xmodel.util import loop
 
 from xmodel import BaseModel
 from xmodel.errors import XModelError
 from xmodel.base.fields import Field
 from xmodel import _private
```

### Comparing `xmodel-0.2.0/xmodel/common/lazy.py` & `xmodel-0.3.0/xmodel/common/lazy.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.2.0/xmodel/common/types.py` & `xmodel-0.3.0/xmodel/common/types.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.2.0/xmodel/common/unwrap.py` & `xmodel-0.3.0/xmodel/common/unwrap.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.2.0/xmodel/common/utils.py` & `xmodel-0.3.0/xmodel/common/utils.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.2.0/xmodel/converters.py` & `xmodel-0.3.0/xmodel/converters.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.2.0/xmodel/json.py` & `xmodel-0.3.0/xmodel/json.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.2.0/xmodel/remote/api.py` & `xmodel-0.3.0/xmodel/remote/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 )
 
 import typing_inspect
 
 from xinject import Dependency
 from xsentinels import Default
 from xurls.url import Query
-from xloop import xloop as loop
+from xmodel.util import loop
 
 from xmodel.errors import XModelError
 from xmodel.base.api import BaseApi
 from xmodel.remote.model import RemoteModel
 from xmodel.common.types import FieldNames, JsonDict
 from xmodel.remote.client import RemoteClient
 from xmodel.remote.response_state import ResponseState
```

### Comparing `xmodel-0.2.0/xmodel/remote/client.py` & `xmodel-0.3.0/xmodel/remote/client.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.2.0/xmodel/remote/model.py` & `xmodel-0.3.0/xmodel/remote/model.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.2.0/xmodel/remote/options.py` & `xmodel-0.3.0/xmodel/remote/options.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.2.0/xmodel/remote/response_state.py` & `xmodel-0.3.0/xmodel/remote/response_state.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.2.0/xmodel/remote/structure.py` & `xmodel-0.3.0/xmodel/remote/structure.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.2.0/xmodel/remote/weak_cache_pool.py` & `xmodel-0.3.0/xmodel/remote/weak_cache_pool.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.2.0/PKG-INFO` & `xmodel-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmodel
-Version: 0.2.0
+Version: 0.3.0
 Summary: Models for working with JSON, ie: JsonModel
 Home-page: https://github.com/xyngular/py-xmodel
 License: The Unlicense (Unlicense)
 Author: Josh Orr
 Author-email: josh@orr.blue
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

