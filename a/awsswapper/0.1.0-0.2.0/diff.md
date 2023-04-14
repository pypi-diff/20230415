# Comparing `tmp/awsswapper-0.1.0.tar.gz` & `tmp/awsswapper-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsswapper-0.1.0.tar", max compression
+gzip compressed data, was "awsswapper-0.2.0.tar", max compression
```

## Comparing `awsswapper-0.1.0.tar` & `awsswapper-0.2.0.tar`

### file list

```diff
@@ -1,91 +1,4 @@
--rw-r--r--   0        0        0       34 2023-03-07 01:14:39.848354 awsswapper-0.1.0/awsswapper/.mypy_cache/.gitignore
--rw-r--r--   0        0        0        2 2023-03-07 01:14:39.847427 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/@plugins_snapshot.json
--rw-r--r--   0        0        0   108590 2023-03-07 01:14:39.750161 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/_ast.data.json
--rw-r--r--   0        0        0     1801 2023-03-07 01:14:39.751421 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/_ast.meta.json
--rw-r--r--   0        0        0    53423 2023-03-07 01:14:39.740132 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/_codecs.data.json
--rw-r--r--   0        0        0     1783 2023-03-07 01:14:39.740906 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/_codecs.meta.json
--rw-r--r--   0        0        0    10107 2023-03-07 01:14:39.734402 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/_collections_abc.data.json
--rw-r--r--   0        0        0     1775 2023-03-07 01:14:39.734849 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/_collections_abc.meta.json
--rw-r--r--   0        0        0    91041 2023-03-07 01:14:39.733116 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1856 2023-03-07 01:14:39.733683 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0    20746 2023-03-07 01:14:39.728872 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/abc.data.json
--rw-r--r--   0        0        0     1743 2023-03-07 01:14:39.729469 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/abc.meta.json
--rw-r--r--   0        0        0    62687 2023-03-07 01:14:39.725828 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/array.data.json
--rw-r--r--   0        0        0     1761 2023-03-07 01:14:39.726707 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/array.meta.json
--rw-r--r--   0        0        0  1053089 2023-03-07 01:14:39.806745 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/builtins.data.json
--rw-r--r--   0        0        0     1886 2023-03-07 01:14:39.809085 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/builtins.meta.json
--rw-r--r--   0        0        0   125884 2023-03-07 01:14:39.721562 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/codecs.data.json
--rw-r--r--   0        0        0     1782 2023-03-07 01:14:39.722421 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/codecs.meta.json
--rw-r--r--   0        0        0   375860 2023-03-07 01:14:39.713139 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/collections/__init__.data.json
--rw-r--r--   0        0        0     1799 2023-03-07 01:14:39.714219 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/collections/__init__.meta.json
--rw-r--r--   0        0        0     4080 2023-03-07 01:14:39.691464 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/collections/abc.data.json
--rw-r--r--   0        0        0     1690 2023-03-07 01:14:39.691945 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/collections/abc.meta.json
--rw-r--r--   0        0        0   127398 2023-03-07 01:14:39.841095 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/configparser.data.json
--rw-r--r--   0        0        0     1788 2023-03-07 01:14:39.841709 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/configparser.meta.json
--rw-r--r--   0        0        0    98660 2023-03-07 01:14:39.690052 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/contextlib.data.json
--rw-r--r--   0        0        0     1785 2023-03-07 01:14:39.690775 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/contextlib.meta.json
--rw-r--r--   0        0        0   138900 2023-03-07 01:14:39.684681 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1835 2023-03-07 01:14:39.685482 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     8115 2023-03-07 01:14:39.675184 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/email/__init__.data.json
--rw-r--r--   0        0        0     1768 2023-03-07 01:14:39.675746 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/email/__init__.meta.json
--rw-r--r--   0        0        0    12870 2023-03-07 01:14:39.673853 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/email/charset.data.json
--rw-r--r--   0        0        0     1718 2023-03-07 01:14:39.674379 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/email/charset.meta.json
--rw-r--r--   0        0        0     8403 2023-03-07 01:14:39.672250 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/email/contentmanager.data.json
--rw-r--r--   0        0        0     1739 2023-03-07 01:14:39.672852 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/email/contentmanager.meta.json
--rw-r--r--   0        0        0    24212 2023-03-07 01:14:39.670535 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/email/errors.data.json
--rw-r--r--   0        0        0     1725 2023-03-07 01:14:39.671132 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/email/errors.meta.json
--rw-r--r--   0        0        0     9462 2023-03-07 01:14:39.668032 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/email/header.data.json
--rw-r--r--   0        0        0     1713 2023-03-07 01:14:39.668997 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/email/header.meta.json
--rw-r--r--   0        0        0    59357 2023-03-07 01:14:39.663312 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/email/message.data.json
--rw-r--r--   0        0        0     1940 2023-03-07 01:14:39.664260 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/email/message.meta.json
--rw-r--r--   0        0        0    32681 2023-03-07 01:14:39.657954 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/email/policy.data.json
--rw-r--r--   0        0        0     1811 2023-03-07 01:14:39.658629 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/email/policy.meta.json
--rw-r--r--   0        0        0    64169 2023-03-07 01:14:39.654893 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/enum.data.json
--rw-r--r--   0        0        0     1839 2023-03-07 01:14:39.655775 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/enum.meta.json
--rw-r--r--   0        0        0    24332 2023-03-07 01:14:39.651669 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/genericpath.data.json
--rw-r--r--   0        0        0     1772 2023-03-07 01:14:39.652215 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/genericpath.meta.json
--rw-r--r--   0        0        0     6556 2023-03-07 01:14:39.649491 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/importlib/__init__.data.json
--rw-r--r--   0        0        0     1756 2023-03-07 01:14:39.650083 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/importlib/__init__.meta.json
--rw-r--r--   0        0        0    76341 2023-03-07 01:14:39.647382 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/importlib/abc.data.json
--rw-r--r--   0        0        0     1904 2023-03-07 01:14:39.648252 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/importlib/abc.meta.json
--rw-r--r--   0        0        0    70469 2023-03-07 01:14:39.642504 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/importlib/machinery.data.json
--rw-r--r--   0        0        0     1851 2023-03-07 01:14:39.643522 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/importlib/machinery.meta.json
--rw-r--r--   0        0        0    71224 2023-03-07 01:14:39.632533 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1858 2023-03-07 01:14:39.634069 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    90827 2023-03-07 01:14:39.626372 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/io.data.json
--rw-r--r--   0        0        0     1801 2023-03-07 01:14:39.627108 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/io.meta.json
--rw-r--r--   0        0        0    27100 2023-03-07 01:14:39.620778 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/mmap.data.json
--rw-r--r--   0        0        0     1732 2023-03-07 01:14:39.621455 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/mmap.meta.json
--rw-r--r--   0        0        0   327565 2023-03-07 01:14:39.617003 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/os/__init__.data.json
--rw-r--r--   0        0        0     1924 2023-03-07 01:14:39.618566 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/os/__init__.meta.json
--rw-r--r--   0        0        0     5359 2023-03-07 01:14:39.598177 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/os/path.data.json
--rw-r--r--   0        0        0     1713 2023-03-07 01:14:39.598720 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/os/path.meta.json
--rw-r--r--   0        0        0    91396 2023-03-07 01:14:39.596614 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/pathlib.data.json
--rw-r--r--   0        0        0     1810 2023-03-07 01:14:39.597526 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/pathlib.meta.json
--rw-r--r--   0        0        0    48691 2023-03-07 01:14:39.591275 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/pickle.data.json
--rw-r--r--   0        0        0     1811 2023-03-07 01:14:39.592257 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/pickle.meta.json
--rw-r--r--   0        0        0    80785 2023-03-07 01:14:39.586305 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/posixpath.data.json
--rw-r--r--   0        0        0     1805 2023-03-07 01:14:39.586959 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/posixpath.meta.json
--rw-r--r--   0        0        0   151215 2023-03-07 01:14:39.581962 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/re.data.json
--rw-r--r--   0        0        0     1896 2023-03-07 01:14:39.582822 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/re.meta.json
--rw-r--r--   0        0        0    15141 2023-03-07 01:14:39.572496 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/sre_compile.data.json
--rw-r--r--   0        0        0     1727 2023-03-07 01:14:39.573049 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/sre_compile.meta.json
--rw-r--r--   0        0        0    29768 2023-03-07 01:14:39.570756 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/sre_constants.data.json
--rw-r--r--   0        0        0     1725 2023-03-07 01:14:39.571422 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/sre_constants.meta.json
--rw-r--r--   0        0        0    53137 2023-03-07 01:14:39.568491 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/sre_parse.data.json
--rw-r--r--   0        0        0     1805 2023-03-07 01:14:39.569111 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/sre_parse.meta.json
--rw-r--r--   0        0        0   166751 2023-03-07 01:14:39.565436 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/subprocess.data.json
--rw-r--r--   0        0        0     1865 2023-03-07 01:14:39.566167 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/subprocess.meta.json
--rw-r--r--   0        0        0   139750 2023-03-07 01:14:39.555539 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/sys.data.json
--rw-r--r--   0        0        0     1844 2023-03-07 01:14:39.556759 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/sys.meta.json
--rw-r--r--   0        0        0   256964 2023-03-07 01:14:39.545610 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/types.data.json
--rw-r--r--   0        0        0     1814 2023-03-07 01:14:39.546613 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/types.meta.json
--rw-r--r--   0        0        0   411069 2023-03-07 01:14:39.532316 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/typing.data.json
--rw-r--r--   0        0        0     1857 2023-03-07 01:14:39.533224 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/typing.meta.json
--rw-r--r--   0        0        0    64438 2023-03-07 01:14:39.506978 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/typing_extensions.data.json
--rw-r--r--   0        0        0     1780 2023-03-07 01:14:39.508046 awsswapper-0.1.0/awsswapper/.mypy_cache/3.9/typing_extensions.meta.json
--rw-r--r--   0        0        0      190 2023-03-07 01:14:39.848564 awsswapper-0.1.0/awsswapper/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      783 2021-05-18 23:51:05.223633 awsswapper-0.1.0/awsswapper/__init__.py
--rw-r--r--   0        0        0      372 2021-05-18 23:42:57.039449 awsswapper-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1130 1970-01-01 00:00:00.000000 awsswapper-0.1.0/setup.py
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 awsswapper-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1129 2023-04-14 21:54:45.122371 awsswapper-0.2.0/awsswapper/__init__.py
+-rw-r--r--   0        0        0      372 2023-04-14 22:29:48.513972 awsswapper-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 awsswapper-0.2.0/setup.py
+-rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 awsswapper-0.2.0/PKG-INFO
```

### Comparing `awsswapper-0.1.0/PKG-INFO` & `awsswapper-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsswapper
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Willem Thiart
 Author-email: himself@willemthiart.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

