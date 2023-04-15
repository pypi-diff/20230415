# Comparing `tmp/hlatypingtools-1.0.0.tar.gz` & `tmp/hlatypingtools-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hlatypingtools-1.0.0.tar", max compression
+gzip compressed data, was "hlatypingtools-1.0.1.tar", max compression
```

## Comparing `hlatypingtools-1.0.0.tar` & `hlatypingtools-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0        0 2023-04-14 14:02:29.564981 hlatypingtools-1.0.0/hlatypingtools/__init__.py
--rw-r--r--   0        0        0      632 2023-04-14 16:08:15.663091 hlatypingtools-1.0.0/hlatypingtools/decrypt_file.py
--rw-r--r--   0        0        0     2950 2023-04-14 16:51:00.238909 hlatypingtools-1.0.0/hlatypingtools/get_info.py
--rw-r--r--   0        0        0      529 2023-04-14 16:58:58.541951 hlatypingtools-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2721 2023-04-14 17:10:41.358676 hlatypingtools-1.0.0/README.md
--rw-r--r--   0        0        0     3427 1970-01-01 00:00:00.000000 hlatypingtools-1.0.0/setup.py
--rw-r--r--   0        0        0     3180 1970-01-01 00:00:00.000000 hlatypingtools-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       59 2023-04-15 19:16:13.832019 hlatypingtools-1.0.1/hlatypingtools/__init__.py
+-rw-r--r--   0        0        0   180055 2023-04-14 16:57:03.007528 hlatypingtools-1.0.1/hlatypingtools/data/data.pickle.aes
+-rw-r--r--   0        0        0      632 2023-04-14 16:08:15.663091 hlatypingtools-1.0.1/hlatypingtools/decrypt_file.py
+-rw-r--r--   0        0        0     2950 2023-04-14 16:51:00.238909 hlatypingtools-1.0.1/hlatypingtools/get_info.py
+-rw-r--r--   0        0        0      529 2023-04-15 19:34:58.520498 hlatypingtools-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2807 2023-04-15 19:16:52.738119 hlatypingtools-1.0.1/README.md
+-rw-r--r--   0        0        0     3557 1970-01-01 00:00:00.000000 hlatypingtools-1.0.1/setup.py
+-rw-r--r--   0        0        0     3265 1970-01-01 00:00:00.000000 hlatypingtools-1.0.1/PKG-INFO
```

### Comparing `hlatypingtools-1.0.0/hlatypingtools/decrypt_file.py` & `hlatypingtools-1.0.1/hlatypingtools/decrypt_file.py`

 * *Files identical despite different names*

### Comparing `hlatypingtools-1.0.0/hlatypingtools/get_info.py` & `hlatypingtools-1.0.1/hlatypingtools/get_info.py`

 * *Files identical despite different names*

### Comparing `hlatypingtools-1.0.0/pyproject.toml` & `hlatypingtools-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hlatypingtools"
-version = "1.0.0"
+version = "1.0.1"
 description = ""
 authors = ["JasonMendoza2008 <lhotteromain@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pandas = "^2.0.0"
```

### Comparing `hlatypingtools-1.0.0/README.md` & `hlatypingtools-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # HLATypingTools
 
 ## Getting Started
 #### Install from PyPI (recommended)
 To use `HLATypingTools`, run `pip install HLATypingTools` in your terminal.
+All python packages necessary for `HLATypingTools` will automatically be downloaded.
 
 #### Usage
 If you haven't decrypted the data yet (first time you are using the package and you did request access to the product),
 run:
 ```py
 from hlatypingtools.decrypt_file import decrypt_file
```

### Comparing `hlatypingtools-1.0.0/setup.py` & `hlatypingtools-1.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['hlatypingtools']
 
 package_data = \
-{'': ['*']}
+{'': ['*'], 'hlatypingtools': ['data/data.pickle.aes']}
 
 install_requires = \
 ['openpyxl>=3.1.2,<4.0.0',
  'pandas-stubs>=2.0.0.230412,<3.0.0.0',
  'pandas>=2.0.0,<3.0.0',
  'pyaescrypt>=6.0.0,<7.0.0']
 
 setup_kwargs = {
     'name': 'hlatypingtools',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': '',
-    'long_description': '# HLATypingTools\n\n## Getting Started\n#### Install from PyPI (recommended)\nTo use `HLATypingTools`, run `pip install HLATypingTools` in your terminal.\n\n#### Usage\nIf you haven\'t decrypted the data yet (first time you are using the package and you did request access to the product),\nrun:\n```py\nfrom hlatypingtools.decrypt_file import decrypt_file\n\npassword: str = "___"   # Replace with password provided by the author \ndecrypt_file(password)\n```\nIt should print `File decrypted successfully`.\n\nThen you can use the package as follows:\n```py\nfrom hlatypingtools.get_info import get_allele_info\n\nallele: str = "A*01:01"\nprint(get_allele_info(allele, "Broad"))  # will output A1\nprint(get_allele_info(allele, "G Group"))  # will output A*01:01:01G\nprint(get_allele_info(allele, "P Group"))  # will output A*01:01P\nprint(get_allele_info(allele, "% locus"))  # will output 11.906\n```\n\nOr as follows:\n```py\nfrom hlatypingtools.get_info import get_locus\nprint(get_locus("A*01:01"))  # will output HLA_A\n```\n\nOr as follows to output all possible high-resolution alleles for a given low-resolution typing:\n```py\nfrom hlatypingtools.get_info import get_same_low_res_broad, get_same_low_res_assigned_type\nbroad = "DQ3"\nprint("DQB1*03:01" in get_same_low_res_broad(broad))  # will output True\nprint("DQB1*03:02" in get_same_low_res_broad(broad))  # will output True\n\nassigned_type = "DQ7"\nprint("DQB1*03:01" in get_same_low_res_assigned_type(assigned_type))  # will output True\nprint("DQB1*03:02" in get_same_low_res_assigned_type(assigned_type))  # will output False\n```\nNote:\n- Broad = something like A1, B7, Cw1, DR1, **DQ3** (!!!), DQA1&ast;01, DR52, DPB1&ast;01, or DPA1&ast;01\n- Assigned Type = something like A1, B7, Cw1, DR1, **DQ7** (!!!), DQA1&ast;01, DR52, DPB1&ast;01, or DPA1&ast;01\n\n#### Exit codes\n```\n0: Wrong password.\n1: Tried to acess the functions of the package without decrypting the data first.\n2: type_info requested is not available.\n3: wrong format for a low-resolution input. Has to be of the form A1, B7, Cw1, DR1, DQ3, DQA1*01, DR52, DPB1*01, or \nDPA1*01.\n```\n\n## About the source code\n- Follows [PEP8](https://peps.python.org/pep-0008/) Style Guidelines.\n- All functions are unit-tested with [pytest](https://docs.pytest.org/en/stable/).\n- All variables are correctly type-hinted, reviewed with [static type checker](https://mypy.readthedocs.io/en/stable/)\n`mypy`.\n- All functions are documented with [docstrings](https://www.python.org/dev/peps/pep-0257/).\n\n\n## Useful links:\n- [Corresponding GitHub repository](https://github.com/JasonMendoza2008/HLATypingTools)\n- [Corresponding PyPI page](https://pypi.org/project/HLATypingTools)\n',
+    'long_description': '# HLATypingTools\n\n## Getting Started\n#### Install from PyPI (recommended)\nTo use `HLATypingTools`, run `pip install HLATypingTools` in your terminal.\nAll python packages necessary for `HLATypingTools` will automatically be downloaded.\n\n#### Usage\nIf you haven\'t decrypted the data yet (first time you are using the package and you did request access to the product),\nrun:\n```py\nfrom hlatypingtools.decrypt_file import decrypt_file\n\npassword: str = "___"   # Replace with password provided by the author \ndecrypt_file(password)\n```\nIt should print `File decrypted successfully`.\n\nThen you can use the package as follows:\n```py\nfrom hlatypingtools.get_info import get_allele_info\n\nallele: str = "A*01:01"\nprint(get_allele_info(allele, "Broad"))  # will output A1\nprint(get_allele_info(allele, "G Group"))  # will output A*01:01:01G\nprint(get_allele_info(allele, "P Group"))  # will output A*01:01P\nprint(get_allele_info(allele, "% locus"))  # will output 11.906\n```\n\nOr as follows:\n```py\nfrom hlatypingtools.get_info import get_locus\nprint(get_locus("A*01:01"))  # will output HLA_A\n```\n\nOr as follows to output all possible high-resolution alleles for a given low-resolution typing:\n```py\nfrom hlatypingtools.get_info import get_same_low_res_broad, get_same_low_res_assigned_type\nbroad = "DQ3"\nprint("DQB1*03:01" in get_same_low_res_broad(broad))  # will output True\nprint("DQB1*03:02" in get_same_low_res_broad(broad))  # will output True\n\nassigned_type = "DQ7"\nprint("DQB1*03:01" in get_same_low_res_assigned_type(assigned_type))  # will output True\nprint("DQB1*03:02" in get_same_low_res_assigned_type(assigned_type))  # will output False\n```\nNote:\n- Broad = something like A1, B7, Cw1, DR1, **DQ3** (!!!), DQA1&ast;01, DR52, DPB1&ast;01, or DPA1&ast;01\n- Assigned Type = something like A1, B7, Cw1, DR1, **DQ7** (!!!), DQA1&ast;01, DR52, DPB1&ast;01, or DPA1&ast;01\n\n#### Exit codes\n```\n0: Wrong password.\n1: Tried to acess the functions of the package without decrypting the data first.\n2: type_info requested is not available.\n3: wrong format for a low-resolution input. Has to be of the form A1, B7, Cw1, DR1, DQ3, DQA1*01, DR52, DPB1*01, or \nDPA1*01.\n```\n\n## About the source code\n- Follows [PEP8](https://peps.python.org/pep-0008/) Style Guidelines.\n- All functions are unit-tested with [pytest](https://docs.pytest.org/en/stable/).\n- All variables are correctly type-hinted, reviewed with [static type checker](https://mypy.readthedocs.io/en/stable/)\n`mypy`.\n- All functions are documented with [docstrings](https://www.python.org/dev/peps/pep-0257/).\n\n\n## Useful links:\n- [Corresponding GitHub repository](https://github.com/JasonMendoza2008/HLATypingTools)\n- [Corresponding PyPI page](https://pypi.org/project/HLATypingTools)\n',
     'author': 'JasonMendoza2008',
     'author_email': 'lhotteromain@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `hlatypingtools-1.0.0/PKG-INFO` & `hlatypingtools-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hlatypingtools
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 Author: JasonMendoza2008
 Author-email: lhotteromain@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -15,14 +15,15 @@
 Description-Content-Type: text/markdown
 
 # HLATypingTools
 
 ## Getting Started
 #### Install from PyPI (recommended)
 To use `HLATypingTools`, run `pip install HLATypingTools` in your terminal.
+All python packages necessary for `HLATypingTools` will automatically be downloaded.
 
 #### Usage
 If you haven't decrypted the data yet (first time you are using the package and you did request access to the product),
 run:
 ```py
 from hlatypingtools.decrypt_file import decrypt_file
```

