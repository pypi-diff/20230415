# Comparing `tmp/dxsp-1.0.8.tar.gz` & `tmp/dxsp-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.0.8.tar", max compression
+gzip compressed data, was "dxsp-1.0.9.tar", max compression
```

## Comparing `dxsp-1.0.8.tar` & `dxsp-1.0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-13 13:59:15.003624 dxsp-1.0.8/LICENSE
--rw-r--r--   0        0        0     2877 2023-04-13 13:59:15.003624 dxsp-1.0.8/README.md
--rw-r--r--   0        0        0      137 2023-04-13 13:59:15.003624 dxsp-1.0.8/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-04-13 13:59:15.003624 dxsp-1.0.8/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8589 2023-04-13 13:59:15.003624 dxsp-1.0.8/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0    16070 2023-04-13 13:59:15.003624 dxsp-1.0.8/dxsp/main.py
--rw-r--r--   0        0        0      678 2023-04-13 13:59:15.651630 dxsp-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     3456 1970-01-01 00:00:00.000000 dxsp-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-13 14:38:11.405686 dxsp-1.0.9/LICENSE
+-rw-r--r--   0        0        0     2877 2023-04-13 14:38:11.405686 dxsp-1.0.9/README.md
+-rw-r--r--   0        0        0      137 2023-04-13 14:38:11.405686 dxsp-1.0.9/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-04-13 14:38:11.405686 dxsp-1.0.9/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8589 2023-04-13 14:38:11.405686 dxsp-1.0.9/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0    16065 2023-04-13 14:38:11.405686 dxsp-1.0.9/dxsp/main.py
+-rw-r--r--   0        0        0      678 2023-04-13 14:38:12.053685 dxsp-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3456 1970-01-01 00:00:00.000000 dxsp-1.0.9/PKG-INFO
```

### Comparing `dxsp-1.0.8/LICENSE` & `dxsp-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.0.8/README.md` & `dxsp-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-1.0.8/dxsp/assets/blockchains.py` & `dxsp-1.0.9/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.0.8/dxsp/main.py` & `dxsp-1.0.9/dxsp/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from dotenv import load_dotenv
 import json
 import requests
 import asyncio
 from web3 import Web3
 from pycoingecko import CoinGeckoAPI
 
-from dxsp.assets.blockchains import blockchains
+from assets.blockchains import blockchains
 
 
 
 
 class DexSwap:
 
 
@@ -25,18 +25,18 @@
                  w3: Web3 = None,
                  protocol_type: str = None,
                  dex_exchange: str = None,
                  base_trading_symbol: str = None,
                  amount_trading_option: int = 1,
                  ):
         logging.getLogger(__name__).addHandler(logging.NullHandler())
-        logging.debug(msg=f"DexSwap initiated for chain_id" {chain_id})
+        logging.debug(msg=f"DexSwap initiated for chain_id {chain_id}")
         self.chain_id = int(chain_id)
         blockchain = blockchains[self.chain_id ]
-        logging.debug(msg=f"blockchain details" {blockchain})
+        logging.debug(msg=f"blockchain details {blockchain}")
 
         self.wallet_address = wallet_address
         self.private_key = private_key
         self.block_explorer_api = block_explorer_api
 
         self.block_explorer_url = block_explorer_url
         if self.block_explorer_url is None:
```

### Comparing `dxsp-1.0.8/pyproject.toml` & `dxsp-1.0.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.0.8"
+version = "1.0.9"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `dxsp-1.0.8/PKG-INFO` & `dxsp-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.0.8
+Version: 1.0.9
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

