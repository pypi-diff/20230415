# Comparing `tmp/bluetooth_data_tools-0.3.1.tar.gz` & `tmp/bluetooth_data_tools-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluetooth_data_tools-0.3.1.tar", max compression
+gzip compressed data, was "bluetooth_data_tools-0.4.0.tar", max compression
```

## Comparing `bluetooth_data_tools-0.3.1.tar` & `bluetooth_data_tools-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,13 @@
--rw-r--r--   0        0        0    11345 2022-12-19 19:23:47.496223 bluetooth_data_tools-0.3.1/LICENSE
--rw-r--r--   0        0        0     3598 2022-12-19 19:23:47.496223 bluetooth_data_tools-0.3.1/README.md
--rw-r--r--   0        0        0     2357 2022-12-19 19:23:48.672227 bluetooth_data_tools-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1905 2022-12-19 19:23:48.596226 bluetooth_data_tools-0.3.1/src/bluetooth_data_tools/__init__.py
--rw-r--r--   0        0        0     5388 2022-12-19 19:23:47.500223 bluetooth_data_tools-0.3.1/src/bluetooth_data_tools/gap.py
--rw-r--r--   0        0        0        0 2022-12-19 19:23:47.500223 bluetooth_data_tools-0.3.1/src/bluetooth_data_tools/py.typed
--rw-r--r--   0        0        0     4495 1970-01-01 00:00:00.000000 bluetooth_data_tools-0.3.1/setup.py
--rw-r--r--   0        0        0     4935 1970-01-01 00:00:00.000000 bluetooth_data_tools-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11345 2023-04-15 03:39:10.527391 bluetooth_data_tools-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3598 2023-04-15 03:39:10.527391 bluetooth_data_tools-0.4.0/README.md
+-rw-r--r--   0        0        0     1168 2023-04-15 03:39:10.527391 bluetooth_data_tools-0.4.0/build_ext.py
+-rw-r--r--   0        0        0     2471 2023-04-15 03:39:11.275388 bluetooth_data_tools-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1981 2023-04-15 03:39:11.235388 bluetooth_data_tools-0.4.0/src/bluetooth_data_tools/__init__.py
+-rw-r--r--   0        0        0      311 2023-04-15 03:39:10.531391 bluetooth_data_tools-0.4.0/src/bluetooth_data_tools/_utils_impl.pyx
+-rw-r--r--   0        0        0      860 2023-04-15 03:39:10.531391 bluetooth_data_tools-0.4.0/src/bluetooth_data_tools/gap.pxd
+-rw-r--r--   0        0        0     6685 2023-04-15 03:39:10.531391 bluetooth_data_tools-0.4.0/src/bluetooth_data_tools/gap.py
+-rw-r--r--   0        0        0        0 2023-04-15 03:39:10.531391 bluetooth_data_tools-0.4.0/src/bluetooth_data_tools/py.typed
+-rw-r--r--   0        0        0      499 2023-04-15 03:39:10.531391 bluetooth_data_tools-0.4.0/src/bluetooth_data_tools/utils.py
+-rw-r--r--   0        0        0      684 2023-04-15 03:39:10.531391 bluetooth_data_tools-0.4.0/src/bluetooth_data_tools/utils_wrapper.h
+-rw-r--r--   0        0        0     4539 1970-01-01 00:00:00.000000 bluetooth_data_tools-0.4.0/setup.py
+-rw-r--r--   0        0        0     4886 1970-01-01 00:00:00.000000 bluetooth_data_tools-0.4.0/PKG-INFO
```

### Comparing `bluetooth_data_tools-0.3.1/LICENSE` & `bluetooth_data_tools-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bluetooth_data_tools-0.3.1/README.md` & `bluetooth_data_tools-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `bluetooth_data_tools-0.3.1/pyproject.toml` & `bluetooth_data_tools-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bluetooth-data-tools"
-version = "0.3.1"
+version = "0.4.0"
 description = "Tools for converting bluetooth data and packets"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/bdraco/bluetooth-data-tools"
 documentation = "https://bluetooth-data-tools.readthedocs.io"
 classifiers = [
@@ -14,20 +14,24 @@
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries",
 ]
 packages = [
     { include = "bluetooth_data_tools", from = "src" },
 ]
 
+[tool.poetry.build]
+generate-setup-file = true
+script = "build_ext.py"
+
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/bdraco/bluetooth-data-tools/issues"
 "Changelog" = "https://github.com/bdraco/bluetooth-data-tools/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 
 # Documentation Dependencies
 Sphinx = {version = "^5.0", optional = true}
 sphinx-rtd-theme = {version = "^1.0", optional = true}
 myst-parser = {version = "^0.18", optional = true}
 
 [tool.poetry.extras]
@@ -86,9 +90,9 @@
 allow_untyped_defs = true
 
 [[tool.mypy.overrides]]
 module = "docs.*"
 ignore_errors = true
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ['setuptools>=65.4.1', 'wheel', 'Cython', "poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `bluetooth_data_tools-0.3.1/src/bluetooth_data_tools/__init__.py` & `bluetooth_data_tools-0.4.0/src/bluetooth_data_tools/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 
 from .gap import (
     BLEGAPAdvertisement,
     BLEGAPType,
     decode_advertisement_data,
     parse_advertisement_data,
 )
+from .utils import int_to_bluetooth_address
 
-__version__ = "0.3.1"
+__version__ = "0.4.0"
 
 L_PACK = Struct(">L")
 
 __all__ = [
     "address_to_bytes",
     "manufacturer_data_to_raw",
     "newest_manufacturer_data",
     "human_readable_name",
+    "int_to_bluetooth_address",
     "short_address",
     "BLEGAPType",
     "BLEGAPAdvertisement",
     "decode_advertisement_data",
     "parse_advertisement_data",
 ]
```

### Comparing `bluetooth_data_tools-0.3.1/src/bluetooth_data_tools/gap.py` & `bluetooth_data_tools-0.4.0/src/bluetooth_data_tools/gap.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,42 @@
 """GATT Advertisement and Scan Response Data (GAP)."""
-
-
-from __future__ import annotations
-
 import logging
-from collections.abc import Iterable
-from dataclasses import dataclass
 from enum import IntEnum
+from typing import Dict, Iterable, List, Tuple
 from uuid import UUID
 
 BLE_UUID = "0000-1000-8000-00805f9b34fb"
 _LOGGER = logging.getLogger(__name__)
 
 
-@dataclass
 class BLEGAPAdvertisement:
+    """GATT Advertisement and Scan Response Data (GAP)."""
 
-    local_name: str | None
-    service_uuids: list[str]
-    service_data: dict[str, bytes]
-    manufacturer_data: dict[int, bytes]
-    tx_power: int | None
+    __slots__ = (
+        "local_name",
+        "service_uuids",
+        "service_data",
+        "manufacturer_data",
+        "tx_power",
+    )
+
+    def __init__(
+        self,
+        local_name: str | None,
+        service_uuids: List[str],
+        service_data: Dict[str, bytes],
+        manufacturer_data: Dict[int, bytes],
+        tx_power: int | None,
+    ) -> None:
+        """Initialize GAP Advertisement."""
+        self.local_name = local_name
+        self.service_uuids = service_uuids
+        self.service_data = service_data
+        self.manufacturer_data = manufacturer_data
+        self.tx_power = tx_power
 
 
 class BLEGAPType(IntEnum):
     """Advertising data types."""
 
     TYPE_UNKNOWN = 0x00
     TYPE_FLAGS = 0x01
@@ -59,18 +71,20 @@
     TYPE_URI = 0x24
     TYPE_3D_INFORMATION_DATA = 0x3D
     TYPE_MANUFACTURER_SPECIFIC_DATA = 0xFF
 
 
 _BLEGAPType_MAP = {gap_ad.value: gap_ad for gap_ad in BLEGAPType}
 
+_bytes = bytes
+
 
 def decode_advertisement_data(
-    encoded_struct: bytes,
-) -> Iterable[tuple[BLEGAPType, bytes]]:
+    encoded_struct: _bytes,
+) -> Iterable[Tuple[BLEGAPType, bytes]]:
     """Decode a BLE GAP AD structure."""
     offset = 0
     total_length = len(encoded_struct)
     while offset < total_length:
         try:
             length = encoded_struct[offset]
             if not length:
@@ -94,55 +108,73 @@
             )
             return
 
         yield _BLEGAPType_MAP.get(type_, BLEGAPType.TYPE_UNKNOWN), value
         offset += 1 + length
 
 
+TYPE_SHORT_LOCAL_NAME = BLEGAPType.TYPE_SHORT_LOCAL_NAME.value
+TYPE_COMPLETE_LOCAL_NAME = BLEGAPType.TYPE_COMPLETE_LOCAL_NAME.value
+TYPE_MANUFACTURER_SPECIFIC_DATA = BLEGAPType.TYPE_MANUFACTURER_SPECIFIC_DATA.value
+TYPE_16BIT_SERVICE_UUID_COMPLETE = BLEGAPType.TYPE_16BIT_SERVICE_UUID_COMPLETE.value
+TYPE_16BIT_SERVICE_UUID_MORE_AVAILABLE = (
+    BLEGAPType.TYPE_16BIT_SERVICE_UUID_MORE_AVAILABLE.value
+)
+TYPE_128BIT_SERVICE_UUID_COMPLETE = BLEGAPType.TYPE_128BIT_SERVICE_UUID_COMPLETE.value
+TYPE_128BIT_SERVICE_UUID_MORE_AVAILABLE = (
+    BLEGAPType.TYPE_128BIT_SERVICE_UUID_MORE_AVAILABLE.value
+)
+TYPE_SERVICE_DATA = BLEGAPType.TYPE_SERVICE_DATA.value
+TYPE_SERVICE_DATA_32BIT_UUID = BLEGAPType.TYPE_SERVICE_DATA_32BIT_UUID.value
+TYPE_SERVICE_DATA_128BIT_UUID = BLEGAPType.TYPE_SERVICE_DATA_128BIT_UUID.value
+TYPE_TX_POWER_LEVEL = BLEGAPType.TYPE_TX_POWER_LEVEL.value
+
+
 def parse_advertisement_data(
     data: Iterable[bytes],
 ) -> BLEGAPAdvertisement:
     """Parse advertisement data."""
-    manufacturer_data: dict[int, bytes] = {}
-    service_data: dict[str, bytes] = {}
-    service_uuids: list[str] = []
+    manufacturer_data: Dict[int, bytes] = {}
+    service_data: Dict[str, bytes] = {}
+    service_uuids: List[str] = []
     local_name: str | None = None
     tx_power: int | None = None
 
     for gap_data in data:
         for gap_type, gap_value in decode_advertisement_data(gap_data):
-            if gap_type == BLEGAPType.TYPE_SHORT_LOCAL_NAME and not local_name:
+            gap_type_num = gap_type.value
+            if gap_type_num == TYPE_SHORT_LOCAL_NAME and not local_name:
                 local_name = gap_value.decode("utf-8", errors="replace")
-            elif gap_type == BLEGAPType.TYPE_COMPLETE_LOCAL_NAME:
+            elif gap_type_num == TYPE_COMPLETE_LOCAL_NAME:
                 local_name = gap_value.decode("utf-8", errors="replace")
-            elif gap_type == BLEGAPType.TYPE_MANUFACTURER_SPECIFIC_DATA:
+            elif gap_type_num == TYPE_MANUFACTURER_SPECIFIC_DATA:
                 manufacturer_id = int.from_bytes(gap_value[:2], "little")
                 manufacturer_data[manufacturer_id] = gap_value[2:]
-            elif gap_type in {
-                BLEGAPType.TYPE_16BIT_SERVICE_UUID_COMPLETE,
-                BLEGAPType.TYPE_16BIT_SERVICE_UUID_MORE_AVAILABLE,
+            elif gap_type_num in {
+                TYPE_16BIT_SERVICE_UUID_COMPLETE,
+                TYPE_16BIT_SERVICE_UUID_MORE_AVAILABLE,
             }:
                 uuid_int = int.from_bytes(gap_value[:2], "little")
                 service_uuids.append(f"0000{uuid_int:04x}-{BLE_UUID}")
-            elif gap_type in {
-                BLEGAPType.TYPE_128BIT_SERVICE_UUID_MORE_AVAILABLE,
-                BLEGAPType.TYPE_128BIT_SERVICE_UUID_COMPLETE,
+            elif gap_type_num in {
+                TYPE_128BIT_SERVICE_UUID_MORE_AVAILABLE,
+                TYPE_128BIT_SERVICE_UUID_COMPLETE,
             }:
                 uuid_str = str(UUID(int=int.from_bytes(gap_value[:16], "little")))
                 service_uuids.append(uuid_str)
-            elif gap_type == BLEGAPType.TYPE_SERVICE_DATA:
+            elif gap_type_num == TYPE_SERVICE_DATA:
                 uuid_int = int.from_bytes(gap_value[:2], "little")
                 service_data[f"0000{uuid_int:04x}-{BLE_UUID}"] = gap_value[2:]
-            elif gap_type == BLEGAPType.TYPE_SERVICE_DATA_32BIT_UUID:
+            elif gap_type_num == TYPE_SERVICE_DATA_32BIT_UUID:
                 uuid_int = int.from_bytes(gap_value[:4], "little")
                 service_data[f"{uuid_int:08x}-{BLE_UUID}"] = gap_value[4:]
-            elif gap_type == BLEGAPType.TYPE_SERVICE_DATA_128BIT_UUID:
+            elif gap_type_num == TYPE_SERVICE_DATA_128BIT_UUID:
                 uuid_str = str(UUID(int=int.from_bytes(gap_value[:16], "little")))
                 service_data[uuid_str] = gap_value[16:]
-            elif gap_type == BLEGAPType.TYPE_TX_POWER_LEVEL:
+            elif gap_type_num == TYPE_TX_POWER_LEVEL:
                 tx_power = int.from_bytes(gap_value, "little", signed=True)
 
     return BLEGAPAdvertisement(
         local_name,
         service_uuids,
         service_data,
         manufacturer_data,
```

### Comparing `bluetooth_data_tools-0.3.1/setup.py` & `bluetooth_data_tools-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,24 +13,25 @@
 extras_require = \
 {'docs': ['Sphinx>=5.0,<6.0',
           'sphinx-rtd-theme>=1.0,<2.0',
           'myst-parser>=0.18,<0.19']}
 
 setup_kwargs = {
     'name': 'bluetooth-data-tools',
-    'version': '0.3.1',
+    'version': '0.4.0',
     'description': 'Tools for converting bluetooth data and packets',
     'long_description': '# Bluetooth Data Tools\n\n<p align="center">\n  <a href="https://github.com/bdraco/bluetooth-data-tools/actions?query=workflow%3ACI">\n    <img src="https://img.shields.io/github/workflow/status/bdraco/bluetooth-data-tools/CI/main?label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://bluetooth-data-tools.readthedocs.io">\n    <img src="https://img.shields.io/readthedocs/bluetooth-data-tools.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">\n  </a>\n  <a href="https://codecov.io/gh/bdraco/bluetooth-data-tools">\n    <img src="https://img.shields.io/codecov/c/github/bdraco/bluetooth-data-tools.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/bluetooth-data-tools/">\n    <img src="https://img.shields.io/pypi/v/bluetooth-data-tools.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/bluetooth-data-tools.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/bluetooth-data-tools.svg?style=flat-square" alt="License">\n</p>\n\nTools for converting bluetooth data and packets\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install bluetooth-data-tools`\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- markdownlint-disable -->\n<!-- markdownlint-enable -->\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Cookiecutter](https://github.com/audreyr/cookiecutter) and the\n[browniebroke/cookiecutter-pypackage](https://github.com/browniebroke/cookiecutter-pypackage)\nproject template.\n',
     'author': 'J. Nick Koston',
     'author_email': 'nick@koston.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bdraco/bluetooth-data-tools',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'extras_require': extras_require,
-    'python_requires': '>=3.9,<4.0',
+    'python_requires': '>=3.10,<4.0',
 }
-
+from build_ext import *
+build(setup_kwargs)
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['bluetooth_data_tools'] package_data = \ {'': ['*']}
 extras_require = \ {'docs': ['Sphinx>=5.0,<6.0', 'sphinx-rtd-theme>=1.0,<2.0',
 'myst-parser>=0.18,<0.19']} setup_kwargs = { 'name': 'bluetooth-data-tools',
-'version': '0.3.1', 'description': 'Tools for converting bluetooth data and
+'version': '0.4.0', 'description': 'Tools for converting bluetooth data and
 packets', 'long_description': '# Bluetooth Data Tools\n\n
      \n \n_[CI_Status]\n\n \n_[Documentation_Status]\n\n \n_[Test_coverage
                                 percentage]\n\n
 \n
              \n \n_[Poetry]\n\n \n_[black]\n\n \n_[pre-commit]\n\n
 \n
       \n \n_[PyPI_Version]\n\n [Supported Python versions]\n [License]\n
@@ -19,8 +19,9 @@
 any kind welcome!\n\n## Credits\n\nThis package was created with\n
 [Cookiecutter](https://github.com/audreyr/cookiecutter) and the\n[browniebroke/
 cookiecutter-pypackage](https://github.com/browniebroke/cookiecutter-
 pypackage)\nproject template.\n', 'author': 'J. Nick Koston', 'author_email':
 'nick@koston.org', 'maintainer': 'None', 'maintainer_email': 'None', 'url':
 'https://github.com/bdraco/bluetooth-data-tools', 'package_dir': package_dir,
 'packages': packages, 'package_data': package_data, 'extras_require':
-extras_require, 'python_requires': '>=3.9,<4.0', } setup(**setup_kwargs)
+extras_require, 'python_requires': '>=3.10,<4.0', } from build_ext import *
+build(setup_kwargs) setup(**setup_kwargs)
```

### Comparing `bluetooth_data_tools-0.3.1/PKG-INFO` & `bluetooth_data_tools-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: bluetooth-data-tools
-Version: 0.3.1
+Version: 0.4.0
 Summary: Tools for converting bluetooth data and packets
 Home-page: https://github.com/bdraco/bluetooth-data-tools
 License: Apache Software License 2.0
 Author: J. Nick Koston
 Author-email: nick@koston.org
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: docs
 Requires-Dist: Sphinx (>=5.0,<6.0) ; extra == "docs"
 Requires-Dist: myst-parser (>=0.18,<0.19) ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme (>=1.0,<2.0) ; extra == "docs"
```

#### html2text {}

```diff
@@ -1,18 +1,17 @@
-Metadata-Version: 2.1 Name: bluetooth-data-tools Version: 0.3.1 Summary: Tools
+Metadata-Version: 2.1 Name: bluetooth-data-tools Version: 0.4.0 Summary: Tools
 for converting bluetooth data and packets Home-page: https://github.com/bdraco/
 bluetooth-data-tools License: Apache Software License 2.0 Author: J. Nick
-Koston Author-email: nick@koston.org Requires-Python: >=3.9,<4.0 Classifier:
+Koston Author-email: nick@koston.org Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Topic :: Software
-Development :: Libraries Provides-Extra: docs Requires-Dist: Sphinx
+:: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
+Software Development :: Libraries Provides-Extra: docs Requires-Dist: Sphinx
 (>=5.0,<6.0) ; extra == "docs" Requires-Dist: myst-parser (>=0.18,<0.19) ;
 extra == "docs" Requires-Dist: sphinx-rtd-theme (>=1.0,<2.0) ; extra == "docs"
 Project-URL: Bug Tracker, https://github.com/bdraco/bluetooth-data-tools/issues
 Project-URL: Changelog, https://github.com/bdraco/bluetooth-data-tools/blob/
 main/CHANGELOG.md Project-URL: Documentation, https://bluetooth-data-
 tools.readthedocs.io Project-URL: Repository, https://github.com/bdraco/
 bluetooth-data-tools Description-Content-Type: text/markdown # Bluetooth Data
```

