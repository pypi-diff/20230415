# Comparing `tmp/cardano-nft-vending-machine-0.6.2.tar.gz` & `tmp/cardano-nft-vending-machine-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/thaddeusdiamond/workspaces/wildtangz/cardano-vending-machine/dist/.tmp-39ddsqdz/cardano-nft-vending-machine-0.6.2.tar", last modified: Fri Mar 31 02:09:16 2023, max compression
+gzip compressed data, was "/Users/thaddeusdiamond/workspaces/wildtangz/cardano-vending-machine/dist/.tmp-qnpfdt7c/cardano-nft-vending-machine-0.6.3.tar", last modified: Sat Apr 15 01:56:09 2023, max compression
```

## Comparing `cardano-nft-vending-machine-0.6.2.tar` & `cardano-nft-vending-machine-0.6.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-03-31 02:09:16.944103 cardano-nft-vending-machine-0.6.2/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    11348 2022-06-01 02:40:16.000000 cardano-nft-vending-machine-0.6.2/LICENSE
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    13097 2023-03-31 02:09:16.943734 cardano-nft-vending-machine-0.6.2/PKG-INFO
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    12437 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.6.2/README.md
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      960 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.6.2/pyproject.toml
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       38 2023-03-31 02:09:16.944213 cardano-nft-vending-machine-0.6.2/setup.cfg
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-03-31 02:09:16.931867 cardano-nft-vending-machine-0.6.2/src/
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-03-31 02:09:16.934319 cardano-nft-vending-machine-0.6.2/src/cardano/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-06-01 02:40:43.000000 cardano-nft-vending-machine-0.6.2/src/cardano/__init__.py
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-03-31 02:09:16.938297 cardano-nft-vending-machine-0.6.2/src/cardano/wt/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-06-01 02:40:43.000000 cardano-nft-vending-machine-0.6.2/src/cardano/wt/__init__.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     4987 2023-02-15 06:22:29.000000 cardano-nft-vending-machine-0.6.2/src/cardano/wt/blockfrost.py
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-03-31 02:09:16.939350 cardano-nft-vending-machine-0.6.2/src/cardano/wt/bonuses/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2023-02-16 05:42:18.000000 cardano-nft-vending-machine-0.6.2/src/cardano/wt/bonuses/__init__.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      487 2023-02-16 05:42:18.000000 cardano-nft-vending-machine-0.6.2/src/cardano/wt/bonuses/bogo.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     2803 2022-10-04 18:29:05.000000 cardano-nft-vending-machine-0.6.2/src/cardano/wt/cardano_cli.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     5560 2023-03-09 19:37:45.000000 cardano-nft-vending-machine-0.6.2/src/cardano/wt/mint.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     9760 2023-02-16 05:42:18.000000 cardano-nft-vending-machine-0.6.2/src/cardano/wt/nft_vending_machine.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      838 2022-09-24 03:04:23.000000 cardano-nft-vending-machine-0.6.2/src/cardano/wt/utxo.py
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-03-31 02:09:16.941378 cardano-nft-vending-machine-0.6.2/src/cardano/wt/whitelist/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-09-24 03:04:23.000000 cardano-nft-vending-machine-0.6.2/src/cardano/wt/whitelist/__init__.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     4250 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.6.2/src/cardano/wt/whitelist/asset_whitelist.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     2503 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.6.2/src/cardano/wt/whitelist/filesystem.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     1140 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.6.2/src/cardano/wt/whitelist/no_whitelist.py
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     4888 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.6.2/src/cardano/wt/whitelist/wallet_whitelist.py
-drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-03-31 02:09:16.943240 cardano-nft-vending-machine-0.6.2/src/cardano_nft_vending_machine.egg-info/
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    13097 2023-03-31 02:09:16.000000 cardano-nft-vending-machine-0.6.2/src/cardano_nft_vending_machine.egg-info/PKG-INFO
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      772 2023-03-31 02:09:16.000000 cardano-nft-vending-machine-0.6.2/src/cardano_nft_vending_machine.egg-info/SOURCES.txt
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        1 2023-03-31 02:09:16.000000 cardano-nft-vending-machine-0.6.2/src/cardano_nft_vending_machine.egg-info/dependency_links.txt
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       53 2023-03-31 02:09:16.000000 cardano-nft-vending-machine-0.6.2/src/cardano_nft_vending_machine.egg-info/requires.txt
--rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        8 2023-03-31 02:09:16.000000 cardano-nft-vending-machine-0.6.2/src/cardano_nft_vending_machine.egg-info/top_level.txt
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-04-15 01:56:09.669736 cardano-nft-vending-machine-0.6.3/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    11348 2022-06-01 02:40:16.000000 cardano-nft-vending-machine-0.6.3/LICENSE
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    13218 2023-04-15 01:56:09.669399 cardano-nft-vending-machine-0.6.3/PKG-INFO
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    12558 2023-04-01 01:43:17.000000 cardano-nft-vending-machine-0.6.3/README.md
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      960 2023-04-14 03:02:31.000000 cardano-nft-vending-machine-0.6.3/pyproject.toml
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       38 2023-04-15 01:56:09.669840 cardano-nft-vending-machine-0.6.3/setup.cfg
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-04-15 01:56:09.658271 cardano-nft-vending-machine-0.6.3/src/
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-04-15 01:56:09.660004 cardano-nft-vending-machine-0.6.3/src/cardano/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-06-01 02:40:43.000000 cardano-nft-vending-machine-0.6.3/src/cardano/__init__.py
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-04-15 01:56:09.662989 cardano-nft-vending-machine-0.6.3/src/cardano/wt/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-06-01 02:40:43.000000 cardano-nft-vending-machine-0.6.3/src/cardano/wt/__init__.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     4987 2023-02-15 06:22:29.000000 cardano-nft-vending-machine-0.6.3/src/cardano/wt/blockfrost.py
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-04-15 01:56:09.663956 cardano-nft-vending-machine-0.6.3/src/cardano/wt/bonuses/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2023-02-16 05:42:18.000000 cardano-nft-vending-machine-0.6.3/src/cardano/wt/bonuses/__init__.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      487 2023-02-16 05:42:18.000000 cardano-nft-vending-machine-0.6.3/src/cardano/wt/bonuses/bogo.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     2803 2022-10-04 18:29:05.000000 cardano-nft-vending-machine-0.6.3/src/cardano/wt/cardano_cli.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     5560 2023-03-09 19:37:45.000000 cardano-nft-vending-machine-0.6.3/src/cardano/wt/mint.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     9768 2023-04-13 20:07:17.000000 cardano-nft-vending-machine-0.6.3/src/cardano/wt/nft_vending_machine.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      838 2022-09-24 03:04:23.000000 cardano-nft-vending-machine-0.6.3/src/cardano/wt/utxo.py
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-04-15 01:56:09.666894 cardano-nft-vending-machine-0.6.3/src/cardano/wt/whitelist/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        0 2022-09-24 03:04:23.000000 cardano-nft-vending-machine-0.6.3/src/cardano/wt/whitelist/__init__.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     4250 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.6.3/src/cardano/wt/whitelist/asset_whitelist.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     2503 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.6.3/src/cardano/wt/whitelist/filesystem.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     1140 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.6.3/src/cardano/wt/whitelist/no_whitelist.py
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)     4888 2023-03-31 02:08:34.000000 cardano-nft-vending-machine-0.6.3/src/cardano/wt/whitelist/wallet_whitelist.py
+drwxrwxr-x   0 thaddeusdiamond   (501) staff       (20)        0 2023-04-15 01:56:09.668886 cardano-nft-vending-machine-0.6.3/src/cardano_nft_vending_machine.egg-info/
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)    13218 2023-04-15 01:56:09.000000 cardano-nft-vending-machine-0.6.3/src/cardano_nft_vending_machine.egg-info/PKG-INFO
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)      772 2023-04-15 01:56:09.000000 cardano-nft-vending-machine-0.6.3/src/cardano_nft_vending_machine.egg-info/SOURCES.txt
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        1 2023-04-15 01:56:09.000000 cardano-nft-vending-machine-0.6.3/src/cardano_nft_vending_machine.egg-info/dependency_links.txt
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)       53 2023-04-15 01:56:09.000000 cardano-nft-vending-machine-0.6.3/src/cardano_nft_vending_machine.egg-info/requires.txt
+-rw-rw-r--   0 thaddeusdiamond   (501) staff       (20)        8 2023-04-15 01:56:09.000000 cardano-nft-vending-machine-0.6.3/src/cardano_nft_vending_machine.egg-info/top_level.txt
```

### Comparing `cardano-nft-vending-machine-0.6.2/LICENSE` & `cardano-nft-vending-machine-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.6.2/PKG-INFO` & `cardano-nft-vending-machine-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardano-nft-vending-machine
-Version: 0.6.2
+Version: 0.6.3
 Summary: Library to perform NFT mints automatically on the Cardano blockchain
 Project-URL: Documentation, https://thaddeusdiamond.github.io/cardano-nft-vending-machine/cardano/
 Project-URL: Source, https://github.com/thaddeusdiamond/cardano-nft-vending-machine
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -128,14 +128,16 @@
 	-h, --help  show this help message and exit
 	--old-wl-file OLD_WL_FILE
 		Most recent run of this program that was uploaded to cloud storage
 	--out-file OUT_FILE
 		Where to store the new used whitelist information if any changes (can be same as --old-wl-file)
 	--whitelist-dir WHITELIST_DIR
 		Local folder where consumed whitelist files have gone after processing by vending machine
+	--whitelist-dir WHITELIST_DIR
+		Local folder where unused whitelist files are stored to be processed by vending machine
 	--credentials CREDENTIALS
 		JSON-formatted application-specific credentials
 	--upload-method UPLOAD_METHOD
 		Mechanism for uploading changes in whitelist files (e.g., CloudFlare)
 
 ## APIs
 All API documentation is auto-generated from ``pydoc3``-formatted multi-line strings in the source code.  A mirror of ``master`` is hosted on [Github Pages](https://thaddeusdiamond.github.io/cardano-nft-vending-machine/cardano/).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cardano-nft-vending-machine Version: 0.6.2 Summary:
+Metadata-Version: 2.1 Name: cardano-nft-vending-machine Version: 0.6.3 Summary:
 Library to perform NFT mints automatically on the Cardano blockchain Project-
 URL: Documentation, https://thaddeusdiamond.github.io/cardano-nft-vending-
 machine/cardano/ Project-URL: Source, https://github.com/thaddeusdiamond/
 cardano-nft-vending-machine Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.8
@@ -89,23 +89,25 @@
 OLD_WL_FILE --out-file OUT_FILE --whitelist-dir WHITELIST_DIR [--credentials
 CREDENTIALS] [--upload-method UPLOAD_METHOD] Determine if a set of whitelist
 assets have been recently used in the vending machine optional arguments: -h, -
 -help show this help message and exit --old-wl-file OLD_WL_FILE Most recent run
 of this program that was uploaded to cloud storage --out-file OUT_FILE Where to
 store the new used whitelist information if any changes (can be same as --old-
 wl-file) --whitelist-dir WHITELIST_DIR Local folder where consumed whitelist
-files have gone after processing by vending machine --credentials CREDENTIALS
-JSON-formatted application-specific credentials --upload-method UPLOAD_METHOD
-Mechanism for uploading changes in whitelist files (e.g., CloudFlare) ## APIs
-All API documentation is auto-generated from ``pydoc3``-formatted multi-line
-strings in the source code. A mirror of ``master`` is hosted on [Github Pages]
-(https://thaddeusdiamond.github.io/cardano-nft-vending-machine/cardano/). ##
-Build Building this project creates a ``.whl`` file for uploading to [PyPI]()
-or installing locally on a server. All output is, by default, stored to ``dist/
-``. To build, run: python3 -m build ## Test To enhance the output of tests, we
+files have gone after processing by vending machine --whitelist-dir
+WHITELIST_DIR Local folder where unused whitelist files are stored to be
+processed by vending machine --credentials CREDENTIALS JSON-formatted
+application-specific credentials --upload-method UPLOAD_METHOD Mechanism for
+uploading changes in whitelist files (e.g., CloudFlare) ## APIs All API
+documentation is auto-generated from ``pydoc3``-formatted multi-line strings in
+the source code. A mirror of ``master`` is hosted on [Github Pages](https://
+thaddeusdiamond.github.io/cardano-nft-vending-machine/cardano/). ## Build
+Building this project creates a ``.whl`` file for uploading to [PyPI]() or
+installing locally on a server. All output is, by default, stored to ``dist/``.
+To build, run: python3 -m build ## Test To enhance the output of tests, we
 recommend installing [pytest-clarity](https://pypi.org/project/pytest-clarity/
 ): pip3 install pytest-clarity Tests are stored in the ``tests`` subdirectory
 and are run using [pytest](https://docs.pytest.org/en/7.1.x/). But before
 invoking the tests you need to create secrets for [blockfrost.io](https://
 blockfrost.io) and fund a test address (the "funder") as below. ### Blockfrost
 Key Files There are two supported test Cardano networks on Blockfrost as of the
 time of this writing: preprod and preview. More information on these two
```

### Comparing `cardano-nft-vending-machine-0.6.2/README.md` & `cardano-nft-vending-machine-0.6.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,16 @@
 	-h, --help  show this help message and exit
 	--old-wl-file OLD_WL_FILE
 		Most recent run of this program that was uploaded to cloud storage
 	--out-file OUT_FILE
 		Where to store the new used whitelist information if any changes (can be same as --old-wl-file)
 	--whitelist-dir WHITELIST_DIR
 		Local folder where consumed whitelist files have gone after processing by vending machine
+	--whitelist-dir WHITELIST_DIR
+		Local folder where unused whitelist files are stored to be processed by vending machine
 	--credentials CREDENTIALS
 		JSON-formatted application-specific credentials
 	--upload-method UPLOAD_METHOD
 		Mechanism for uploading changes in whitelist files (e.g., CloudFlare)
 
 ## APIs
 All API documentation is auto-generated from ``pydoc3``-formatted multi-line strings in the source code.  A mirror of ``master`` is hosted on [Github Pages](https://thaddeusdiamond.github.io/cardano-nft-vending-machine/cardano/).
```

#### html2text {}

```diff
@@ -80,23 +80,25 @@
 OLD_WL_FILE --out-file OUT_FILE --whitelist-dir WHITELIST_DIR [--credentials
 CREDENTIALS] [--upload-method UPLOAD_METHOD] Determine if a set of whitelist
 assets have been recently used in the vending machine optional arguments: -h, -
 -help show this help message and exit --old-wl-file OLD_WL_FILE Most recent run
 of this program that was uploaded to cloud storage --out-file OUT_FILE Where to
 store the new used whitelist information if any changes (can be same as --old-
 wl-file) --whitelist-dir WHITELIST_DIR Local folder where consumed whitelist
-files have gone after processing by vending machine --credentials CREDENTIALS
-JSON-formatted application-specific credentials --upload-method UPLOAD_METHOD
-Mechanism for uploading changes in whitelist files (e.g., CloudFlare) ## APIs
-All API documentation is auto-generated from ``pydoc3``-formatted multi-line
-strings in the source code. A mirror of ``master`` is hosted on [Github Pages]
-(https://thaddeusdiamond.github.io/cardano-nft-vending-machine/cardano/). ##
-Build Building this project creates a ``.whl`` file for uploading to [PyPI]()
-or installing locally on a server. All output is, by default, stored to ``dist/
-``. To build, run: python3 -m build ## Test To enhance the output of tests, we
+files have gone after processing by vending machine --whitelist-dir
+WHITELIST_DIR Local folder where unused whitelist files are stored to be
+processed by vending machine --credentials CREDENTIALS JSON-formatted
+application-specific credentials --upload-method UPLOAD_METHOD Mechanism for
+uploading changes in whitelist files (e.g., CloudFlare) ## APIs All API
+documentation is auto-generated from ``pydoc3``-formatted multi-line strings in
+the source code. A mirror of ``master`` is hosted on [Github Pages](https://
+thaddeusdiamond.github.io/cardano-nft-vending-machine/cardano/). ## Build
+Building this project creates a ``.whl`` file for uploading to [PyPI]() or
+installing locally on a server. All output is, by default, stored to ``dist/``.
+To build, run: python3 -m build ## Test To enhance the output of tests, we
 recommend installing [pytest-clarity](https://pypi.org/project/pytest-clarity/
 ): pip3 install pytest-clarity Tests are stored in the ``tests`` subdirectory
 and are run using [pytest](https://docs.pytest.org/en/7.1.x/). But before
 invoking the tests you need to create secrets for [blockfrost.io](https://
 blockfrost.io) and fund a test address (the "funder") as below. ### Blockfrost
 Key Files There are two supported test Cardano networks on Blockfrost as of the
 time of this writing: preprod and preview. More information on these two
```

### Comparing `cardano-nft-vending-machine-0.6.2/pyproject.toml` & `cardano-nft-vending-machine-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62.3.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cardano-nft-vending-machine"
-version = "0.6.2"
+version = "0.6.3"
 
 description = "Library to perform NFT mints automatically on the Cardano blockchain"
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

### Comparing `cardano-nft-vending-machine-0.6.2/src/cardano/wt/blockfrost.py` & `cardano-nft-vending-machine-0.6.3/src/cardano/wt/blockfrost.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.6.2/src/cardano/wt/cardano_cli.py` & `cardano-nft-vending-machine-0.6.3/src/cardano/wt/cardano_cli.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.6.2/src/cardano/wt/mint.py` & `cardano-nft-vending-machine-0.6.3/src/cardano/wt/mint.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.6.2/src/cardano/wt/nft_vending_machine.py` & `cardano-nft-vending-machine-0.6.3/src/cardano/wt/nft_vending_machine.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             shutil.move(mint_metadata_orig, mint_metadata_locked)
         combined_output_path = os.path.join(output_dir, metadata_subdir, f"{txn_id}.json")
         with open(combined_output_path, 'w') as combined_metadata_handle:
             json.dump({'721': { self.mint.policy : combined_nft_metadata }}, combined_metadata_handle)
         return combined_output_path
 
     def __do_vend(self, mint_req, output_dir, locked_subdir, metadata_subdir):
-        available_mints = os.listdir(self.mint.nfts_dir)
+        available_mints = sorted(os.listdir(self.mint.nfts_dir))
         if not available_mints:
             print("WARNING: Metadata directory is empty, please restock the vending machine...")
         elif self.vend_randomly:
             random.shuffle(available_mints)
 
         non_lovelace_bals = [balance for balance in mint_req.balances if balance.policy != Utxo.Balance.LOVELACE_POLICY]
         if non_lovelace_bals:
```

### Comparing `cardano-nft-vending-machine-0.6.2/src/cardano/wt/utxo.py` & `cardano-nft-vending-machine-0.6.3/src/cardano/wt/utxo.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.6.2/src/cardano/wt/whitelist/asset_whitelist.py` & `cardano-nft-vending-machine-0.6.3/src/cardano/wt/whitelist/asset_whitelist.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.6.2/src/cardano/wt/whitelist/filesystem.py` & `cardano-nft-vending-machine-0.6.3/src/cardano/wt/whitelist/filesystem.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.6.2/src/cardano/wt/whitelist/no_whitelist.py` & `cardano-nft-vending-machine-0.6.3/src/cardano/wt/whitelist/no_whitelist.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.6.2/src/cardano/wt/whitelist/wallet_whitelist.py` & `cardano-nft-vending-machine-0.6.3/src/cardano/wt/whitelist/wallet_whitelist.py`

 * *Files identical despite different names*

### Comparing `cardano-nft-vending-machine-0.6.2/src/cardano_nft_vending_machine.egg-info/PKG-INFO` & `cardano-nft-vending-machine-0.6.3/src/cardano_nft_vending_machine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardano-nft-vending-machine
-Version: 0.6.2
+Version: 0.6.3
 Summary: Library to perform NFT mints automatically on the Cardano blockchain
 Project-URL: Documentation, https://thaddeusdiamond.github.io/cardano-nft-vending-machine/cardano/
 Project-URL: Source, https://github.com/thaddeusdiamond/cardano-nft-vending-machine
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -128,14 +128,16 @@
 	-h, --help  show this help message and exit
 	--old-wl-file OLD_WL_FILE
 		Most recent run of this program that was uploaded to cloud storage
 	--out-file OUT_FILE
 		Where to store the new used whitelist information if any changes (can be same as --old-wl-file)
 	--whitelist-dir WHITELIST_DIR
 		Local folder where consumed whitelist files have gone after processing by vending machine
+	--whitelist-dir WHITELIST_DIR
+		Local folder where unused whitelist files are stored to be processed by vending machine
 	--credentials CREDENTIALS
 		JSON-formatted application-specific credentials
 	--upload-method UPLOAD_METHOD
 		Mechanism for uploading changes in whitelist files (e.g., CloudFlare)
 
 ## APIs
 All API documentation is auto-generated from ``pydoc3``-formatted multi-line strings in the source code.  A mirror of ``master`` is hosted on [Github Pages](https://thaddeusdiamond.github.io/cardano-nft-vending-machine/cardano/).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cardano-nft-vending-machine Version: 0.6.2 Summary:
+Metadata-Version: 2.1 Name: cardano-nft-vending-machine Version: 0.6.3 Summary:
 Library to perform NFT mints automatically on the Cardano blockchain Project-
 URL: Documentation, https://thaddeusdiamond.github.io/cardano-nft-vending-
 machine/cardano/ Project-URL: Source, https://github.com/thaddeusdiamond/
 cardano-nft-vending-machine Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.8
@@ -89,23 +89,25 @@
 OLD_WL_FILE --out-file OUT_FILE --whitelist-dir WHITELIST_DIR [--credentials
 CREDENTIALS] [--upload-method UPLOAD_METHOD] Determine if a set of whitelist
 assets have been recently used in the vending machine optional arguments: -h, -
 -help show this help message and exit --old-wl-file OLD_WL_FILE Most recent run
 of this program that was uploaded to cloud storage --out-file OUT_FILE Where to
 store the new used whitelist information if any changes (can be same as --old-
 wl-file) --whitelist-dir WHITELIST_DIR Local folder where consumed whitelist
-files have gone after processing by vending machine --credentials CREDENTIALS
-JSON-formatted application-specific credentials --upload-method UPLOAD_METHOD
-Mechanism for uploading changes in whitelist files (e.g., CloudFlare) ## APIs
-All API documentation is auto-generated from ``pydoc3``-formatted multi-line
-strings in the source code. A mirror of ``master`` is hosted on [Github Pages]
-(https://thaddeusdiamond.github.io/cardano-nft-vending-machine/cardano/). ##
-Build Building this project creates a ``.whl`` file for uploading to [PyPI]()
-or installing locally on a server. All output is, by default, stored to ``dist/
-``. To build, run: python3 -m build ## Test To enhance the output of tests, we
+files have gone after processing by vending machine --whitelist-dir
+WHITELIST_DIR Local folder where unused whitelist files are stored to be
+processed by vending machine --credentials CREDENTIALS JSON-formatted
+application-specific credentials --upload-method UPLOAD_METHOD Mechanism for
+uploading changes in whitelist files (e.g., CloudFlare) ## APIs All API
+documentation is auto-generated from ``pydoc3``-formatted multi-line strings in
+the source code. A mirror of ``master`` is hosted on [Github Pages](https://
+thaddeusdiamond.github.io/cardano-nft-vending-machine/cardano/). ## Build
+Building this project creates a ``.whl`` file for uploading to [PyPI]() or
+installing locally on a server. All output is, by default, stored to ``dist/``.
+To build, run: python3 -m build ## Test To enhance the output of tests, we
 recommend installing [pytest-clarity](https://pypi.org/project/pytest-clarity/
 ): pip3 install pytest-clarity Tests are stored in the ``tests`` subdirectory
 and are run using [pytest](https://docs.pytest.org/en/7.1.x/). But before
 invoking the tests you need to create secrets for [blockfrost.io](https://
 blockfrost.io) and fund a test address (the "funder") as below. ### Blockfrost
 Key Files There are two supported test Cardano networks on Blockfrost as of the
 time of this writing: preprod and preview. More information on these two
```

### Comparing `cardano-nft-vending-machine-0.6.2/src/cardano_nft_vending_machine.egg-info/SOURCES.txt` & `cardano-nft-vending-machine-0.6.3/src/cardano_nft_vending_machine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

