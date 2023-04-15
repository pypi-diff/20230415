# Comparing `tmp/snapatac2-2.2.0.tar.gz` & `tmp/snapatac2-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapatac2-2.2.0.tar", last modified: Fri Dec  2 17:39:29 2022, max compression
+gzip compressed data, was "snapatac2-2.3.0.tar", last modified: Sat Apr 15 05:58:14 2023, max compression
```

## Comparing `snapatac2-2.2.0.tar` & `snapatac2-2.3.0.tar`

### file list

```diff
@@ -1,59 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 17:39:29.400432 snapatac2-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2022-12-02 17:39:26.000000 snapatac2-2.2.0/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2022-12-02 17:39:26.000000 snapatac2-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2022-12-02 17:39:26.000000 snapatac2-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      388 2022-12-02 17:39:29.400432 snapatac2-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       85 2022-12-02 17:39:26.000000 snapatac2-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       68 2022-12-02 17:39:26.000000 snapatac2-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-02 17:39:29.400432 snapatac2-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2022-12-02 17:39:26.000000 snapatac2-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 17:39:29.392432 snapatac2-2.2.0/snapatac2/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2022-12-02 17:39:26.000000 snapatac2-2.2.0/snapatac2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2022-12-02 17:39:26.000000 snapatac2-2.2.0/snapatac2/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2022-12-02 17:39:26.000000 snapatac2-2.2.0/snapatac2/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2022-12-02 17:39:26.000000 snapatac2-2.2.0/snapatac2/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2022-12-02 17:39:26.000000 snapatac2-2.2.0/snapatac2/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 17:39:29.396432 snapatac2-2.2.0/snapatac2/export/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2022-12-02 17:39:26.000000 snapatac2-2.2.0/snapatac2/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2022-12-02 17:39:26.000000 snapatac2-2.2.0/snapatac2/genome.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 17:39:29.396432 snapatac2-2.2.0/snapatac2/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)    13250 2022-12-02 17:39:26.000000 snapatac2-2.2.0/snapatac2/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2022-12-02 17:39:26.000000 snapatac2-2.2.0/snapatac2/plotting/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2022-12-02 17:39:26.000000 snapatac2-2.2.0/snapatac2/plotting/_network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 17:39:29.396432 snapatac2-2.2.0/snapatac2/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2022-12-02 17:39:26.000000 snapatac2-2.2.0/snapatac2/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15151 2022-12-02 17:39:26.000000 snapatac2-2.2.0/snapatac2/preprocessing/_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2022-12-02 17:39:26.000000 snapatac2-2.2.0/snapatac2/preprocessing/_harmony.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2022-12-02 17:39:26.000000 snapatac2-2.2.0/snapatac2/preprocessing/_knn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2022-12-02 17:39:26.000000 snapatac2-2.2.0/snapatac2/preprocessing/_mnn_correct.py
--rw-r--r--   0 runner    (1001) docker     (123)    11684 2022-12-02 17:39:26.000000 snapatac2-2.2.0/snapatac2/preprocessing/_scrublet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 17:39:29.396432 snapatac2-2.2.0/snapatac2/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2022-12-02 17:39:26.000000 snapatac2-2.2.0/snapatac2/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2022-12-02 17:39:26.000000 snapatac2-2.2.0/snapatac2/tools/_call_peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11027 2022-12-02 17:39:26.000000 snapatac2-2.2.0/snapatac2/tools/_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     8869 2022-12-02 17:39:26.000000 snapatac2-2.2.0/snapatac2/tools/_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2022-12-02 17:39:26.000000 snapatac2-2.2.0/snapatac2/tools/_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10992 2022-12-02 17:39:26.000000 snapatac2-2.2.0/snapatac2/tools/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2022-12-02 17:39:26.000000 snapatac2-2.2.0/snapatac2/tools/_motif.py
--rw-r--r--   0 runner    (1001) docker     (123)    18424 2022-12-02 17:39:26.000000 snapatac2-2.2.0/snapatac2/tools/_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2022-12-02 17:39:26.000000 snapatac2-2.2.0/snapatac2/tools/_smooth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 17:39:29.396432 snapatac2-2.2.0/snapatac2/tools/embedding/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2022-12-02 17:39:26.000000 snapatac2-2.2.0/snapatac2/tools/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2022-12-02 17:39:26.000000 snapatac2-2.2.0/snapatac2/tools/embedding/_laplacian.py
--rw-r--r--   0 runner    (1001) docker     (123)    10773 2022-12-02 17:39:26.000000 snapatac2-2.2.0/snapatac2/tools/embedding/_spectral.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2022-12-02 17:39:26.000000 snapatac2-2.2.0/snapatac2/tools/embedding/_umap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 17:39:29.396432 snapatac2-2.2.0/snapatac2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2022-12-02 17:39:29.000000 snapatac2-2.2.0/snapatac2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2022-12-02 17:39:29.000000 snapatac2-2.2.0/snapatac2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-02 17:39:29.000000 snapatac2-2.2.0/snapatac2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-02 17:39:29.000000 snapatac2-2.2.0/snapatac2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      213 2022-12-02 17:39:29.000000 snapatac2-2.2.0/snapatac2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-02 17:39:29.000000 snapatac2-2.2.0/snapatac2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 17:39:29.400432 snapatac2-2.2.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2022-12-02 17:39:26.000000 snapatac2-2.2.0/src/call_peaks.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2022-12-02 17:39:26.000000 snapatac2-2.2.0/src/export.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2022-12-02 17:39:26.000000 snapatac2-2.2.0/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2022-12-02 17:39:26.000000 snapatac2-2.2.0/src/motif.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2022-12-02 17:39:26.000000 snapatac2-2.2.0/src/network.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2022-12-02 17:39:26.000000 snapatac2-2.2.0/src/preprocessing.rs
--rw-r--r--   0 runner    (1001) docker     (123)    12152 2022-12-02 17:39:26.000000 snapatac2-2.2.0/src/utils.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:58:14.214284 snapatac2-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-15 05:58:10.000000 snapatac2-2.3.0/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-15 05:58:10.000000 snapatac2-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-15 05:58:10.000000 snapatac2-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-15 05:58:14.214284 snapatac2-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-15 05:58:10.000000 snapatac2-2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-15 05:58:10.000000 snapatac2-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 05:58:14.214284 snapatac2-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-15 05:58:10.000000 snapatac2-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:58:14.210284 snapatac2-2.3.0/snapatac2/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:58:14.210284 snapatac2-2.3.0/snapatac2/export/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/genome.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:58:14.210284 snapatac2-2.3.0/snapatac2/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15448 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/plotting/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/plotting/_network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:58:14.210284 snapatac2-2.3.0/snapatac2/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21050 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/preprocessing/_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/preprocessing/_harmony.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/preprocessing/_knn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/preprocessing/_mnn_correct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12873 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/preprocessing/_scrublet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:58:14.214284 snapatac2-2.3.0/snapatac2/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/tools/_call_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11027 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/tools/_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/tools/_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15443 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/tools/_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/tools/_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10992 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/tools/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/tools/_motif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19635 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/tools/_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/tools/_smooth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:58:14.210284 snapatac2-2.3.0/snapatac2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-15 05:58:14.000000 snapatac2-2.3.0/snapatac2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-15 05:58:14.000000 snapatac2-2.3.0/snapatac2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 05:58:14.000000 snapatac2-2.3.0/snapatac2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 05:58:14.000000 snapatac2-2.3.0/snapatac2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-15 05:58:14.000000 snapatac2-2.3.0/snapatac2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-15 05:58:14.000000 snapatac2-2.3.0/snapatac2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:58:14.214284 snapatac2-2.3.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-15 05:58:10.000000 snapatac2-2.3.0/src/call_peaks.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    13155 2023-04-15 05:58:10.000000 snapatac2-2.3.0/src/embedding.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-15 05:58:10.000000 snapatac2-2.3.0/src/export.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-04-15 05:58:10.000000 snapatac2-2.3.0/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-15 05:58:10.000000 snapatac2-2.3.0/src/motif.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-15 05:58:10.000000 snapatac2-2.3.0/src/network.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-04-15 05:58:10.000000 snapatac2-2.3.0/src/preprocessing.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:58:14.214284 snapatac2-2.3.0/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-04-15 05:58:10.000000 snapatac2-2.3.0/src/utils/anndata.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-04-15 05:58:10.000000 snapatac2-2.3.0/src/utils.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:58:14.214284 snapatac2-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-15 05:58:10.000000 snapatac2-2.3.0/tests/test_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-15 05:58:10.000000 snapatac2-2.3.0/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-04-15 05:58:10.000000 snapatac2-2.3.0/tests/test_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-15 05:58:10.000000 snapatac2-2.3.0/tests/test_tools.py
```

### Comparing `snapatac2-2.2.0/Cargo.toml` & `snapatac2-2.3.0/Cargo.toml`

 * *Files 24% similar despite different names*

```diff
@@ -7,45 +7,48 @@
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/"
 homepage = "https://github.com/"
 keywords = ["single-cell", "biology"]
 
 [dependencies]
-#anndata-rs = { path = "../../anndata-rs/anndata-rs" }
-#pyanndata = { path = "../../anndata-rs/pyanndata" }
 #snapatac2-core = { path = "../snapatac2-core" }
-anndata-rs = { git = "https://github.com/kaizhang/anndata-rs.git", rev = "5159de91d5c20bac89d88c592efb6d7e8bffd6ab" }
-pyanndata = { git = "https://github.com/kaizhang/anndata-rs.git", rev = "5159de91d5c20bac89d88c592efb6d7e8bffd6ab" }
-snapatac2-core = { git = "https://github.com/kaizhang/SnapATAC2.git", rev = "417d163f94d259fcf6086206e64a6eb6ae9c9e1e" }
+snapatac2-core = { git = "https://github.com/kaizhang/SnapATAC2.git", rev = "9285fa5be15287870a6af7b0d2bfdec225c3127e" }
+#anndata = { path = "../../anndata-rs/anndata" }
+#anndata-hdf5 = { path = "../../anndata-rs/anndata-hdf5" }
+#pyanndata = { path = "../../anndata-rs/pyanndata" }
+anndata = { git = "https://github.com/kaizhang/anndata-rs.git", rev = "1aba156d6c2f63c16433c7385fd26a8960162283" }
+anndata-hdf5 = { git = "https://github.com/kaizhang/anndata-rs.git", rev = "1aba156d6c2f63c16433c7385fd26a8960162283" }
+pyanndata = { git = "https://github.com/kaizhang/anndata-rs.git", rev = "1aba156d6c2f63c16433c7385fd26a8960162283" }
 anyhow = "1.0"
 bed-utils = { git = "https://github.com/kaizhang/bed-utils.git", rev = "19832eda2909dbe87289e09ba966af0797adb9f8" }
 flate2 = "1.0"
-hdf5 = "0.8"
 hora = "0.1"
 itertools = "0.8"
 linreg = "0.2"
 log = "0.4"
 linfa = "0.6"
 linfa-clustering = "0.6"
-noodles = { version = "0.27.0", features = ["bam", "sam"] }
-numpy = "0.17.2"
-nalgebra-sparse = "0.8"
+noodles = { version = "0.34.0", features = ["bam", "sam"] }
+numpy = "0.18.0"
+nalgebra-sparse = "0.9"
+nalgebra = "0.32"
 ndarray = "0.15"
-polars = { version = "0.25", features = ["ndarray", "dtype-categorical"] }
-pyo3-log = "0.7"
+polars = { version = "0.26", features = ["ndarray", "dtype-categorical"] }
+pyo3-log = "0.8"
 rand_isaac = "0.3"
 rand_core = "0.6"
+rand = "0.8"
 rayon = "1.5"
 statrs = "0.16"
 tempfile = "3.3"
 
 [target.'cfg(not(target_env = "msvc"))'.dependencies]
 tikv-jemallocator = {version = "0.5", features = ["disable_initial_exec_tls"]}
 
 [dependencies.pyo3]
-version = "0.17.3"
+version = "0.18.0"
 features = ["extension-module", "anyhow"]
 
 [lib]
 name = "_snapatac2"
 crate-type = ["cdylib"]
```

### Comparing `snapatac2-2.2.0/LICENSE` & `snapatac2-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snapatac2-2.2.0/setup.py` & `snapatac2-2.3.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,30 +23,31 @@
     rust_extensions=[
         RustExtension("snapatac2._snapatac2", debug=False, binding=Binding.PyO3),
     ],
     packages=[
         "snapatac2",
         "snapatac2.preprocessing",
         "snapatac2.tools",
-        "snapatac2.tools.embedding",
         "snapatac2.plotting",
         "snapatac2.export",
     ],
     zip_safe=False,
     python_requires=">=3.7",
     install_requires=[
         "anndata>=0.8.0",
         "kaleido",
+        "multiprocess",
         "natsort",
         "numpy>=1.16.0",
         "pandas",
         "plotly>=5.6.0",
-        "polars>=0.14.0",
+        "polars>=0.14.0, <=0.18.0",
         "pooch>=1.6.0",
         "igraph>=0.10.0",
+        "pynndescent",
         "pyarrow",
         "pyfaidx",
         "rustworkx",
         "scipy>=1.4",
         "scikit-learn>=0.22",
         "tqdm>=4.62",
         "typing_extensions",
```

### Comparing `snapatac2-2.2.0/snapatac2/__init__.py` & `snapatac2-2.3.0/snapatac2/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from ._version import __version__
-from ._io import read_10x_mtx
+#from ._io import read_10x_mtx
 from . import preprocessing as pp
 from . import tools as tl
 from . import plotting as pl
 from . import export as ex
 
 from snapatac2._snapatac2 import (
     AnnData, AnnDataSet, PyDNAMotif,
-    read, read_mtx, read_csv, read_dataset, read_motifs,
+    read, read_mtx, read_dataset, read_motifs,
 )
 
 import sys
 sys.modules.update({f'{__name__}.{m}': globals()[m] for m in ['pp', 'tl', 'pl', 'ex']})
 
 import logging
 logging.basicConfig(
```

### Comparing `snapatac2-2.2.0/snapatac2/_io.py` & `snapatac2-2.3.0/snapatac2/_io.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.2.0/snapatac2/export/__init__.py` & `snapatac2-2.3.0/snapatac2/export/__init__.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.2.0/snapatac2/genome.py` & `snapatac2-2.3.0/snapatac2/genome.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         "chr18": 78077248,
         "chr19": 59128983,
         "chr20": 63025520,
         "chr21": 48129895,
         "chr22": 51304566,
         "chrX": 155270560,
         "chrY": 59373566,
+        "chrM": 16571,
     },
     "gencode_v41_GRCh37.gff3.gz",
     "gencode_v41_GRCh37.fa.gz",
 )
 
 hg19 = GRCh37
```

### Comparing `snapatac2-2.2.0/snapatac2/plotting/__init__.py` & `snapatac2-2.3.0/snapatac2/plotting/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,45 @@
 from __future__ import annotations
 
 import numpy as np
 
 from snapatac2._snapatac2 import AnnData, AnnDataSet
 from snapatac2.tools._misc import aggregate_X
-from ._base import render_plot, heatmap
+from snapatac2._utils import find_elbow
+from ._base import render_plot, heatmap, kde2d, scatter, scatter3d
 from ._network import network_scores, network_edge_stat
 
 __all__ = [
     'tsse', 'scrublet', 'umap', 'network_scores', 'spectral_eigenvalues',
     'regions', 'motif_enrichment',
 ]
 
 def tsse(
     adata: AnnData,
-    show_cells: bool = False,
     min_fragment: int = 500,
-    width: int = 600,
+    width: int = 500,
     height: int = 400,
-    show: bool = True,
-    interactive: bool = True,
-    out_file: str | None = None,
+    **kwargs,
 ) -> 'plotly.graph_objects.Figure' | None:
     """Plot the TSS enrichment vs. number of fragments density figure.
 
     Parameters
     ----------
     adata
         Annotated data matrix.
-    show_cells
-        Whether to show individual cells as dots on the plot
     min_fragment
         The cells' unique fragments lower than it should be removed
     width
         The width of the plot
     height
         The height of the plot
-    show
-        Show the figure
-    interactive
-        Whether to make interactive plot
-    out_file
-        Path of the output file for saving the output image, end with
-        '.svg' or '.pdf' or '.png' or '.html'.
+    kwargs        
+        Additional arguments passed to :func:`~snapatac2.pl.render_plot` to
+        control the final plot output. Please see :func:`~snapatac2.pl.render_plot`
+        for details.
 
     Returns
     -------
     'plotly.graph_objects.Figure' | None
         If `show=False` and `out_file=None`, an `plotly.graph_objects.Figure` will be 
         returned, which can then be further customized using the plotly API.
 
@@ -55,58 +48,27 @@
     .. plotly::
 
         >>> import snapatac2 as snap
         >>> data = snap.read(str(snap.datasets.pbmc5k(type='gene')))
         >>> fig = snap.pl.tsse(data, show=False, out_file=None)
         >>> fig.show()
     """
-    import plotly.graph_objects as go
-
-    selected_cells = adata.obs["n_fragment"] >= min_fragment
+    selected_cells = np.where(adata.obs["n_fragment"] >= min_fragment)[0]
     x = adata.obs["n_fragment"][selected_cells]
     y = adata.obs["tsse"][selected_cells]
 
-    log_x = np.log10(x)
-    log_x_min, log_x_max = log_x.min(), log_x.max()
-    x_range = log_x_max - log_x_min
-    bin_x = np.linspace(log_x_min - 0.1 * x_range, log_x_max + 0.2 * x_range, 20)
-
-    y_min, y_max = y.min(), y.max()
-    y_range = y_max - y_min
-    bin_y = np.linspace(y_min - 0.1 * y_range, y_max + 0.2 * y_range, 15)
-
-    (z, rx, ry) = np.histogram2d(log_x,y, bins=(bin_x, bin_y))
-    fig = go.Figure(data =
-        go.Contour(
-            z = z.T,
-            x = 10**rx,
-            y = ry,
-            colorscale = 'Blues',
-        )
-    )
-
-    if show_cells:
-        fig.add_trace(go.Scatter(
-                x = x,
-                y = y,
-                xaxis = 'x',
-                yaxis = 'y',
-                mode = 'markers',
-                marker = dict(color = 'rgba(0,0,0,0.3)', size = 3)
-        ))
-
-    fig.update_xaxes(type="log")
+    fig = kde2d(x, y, log_x=True, log_y=False)
     fig.update_layout(
-        template="simple_white",
         xaxis_title="Number of unique fragments",
         yaxis_title="TSS enrichment score",
     )
 
-    return render_plot(fig, width, height, interactive, show, out_file)
+    return render_plot(fig, width, height, **kwargs)
 
+'''
 def scrublet(
     adata: AnnData,
     width: int = 800,
     height: int = 400,
     show: bool = True,
     interactive: bool = True,
     out_file: str | None = None,
@@ -162,14 +124,15 @@
     fig.add_trace(go.Histogram(x=sim_scores), row=1, col=2)
     if thres is not None:
         fig.add_vline(x=thres, line_width=3, line_dash="dash", line_color="green")
         fig.add_vrect(x0=thres, x1 = sim_scores.max(), line_width=0, fillcolor="red", opacity=0.2)
 
     fig.update(layout_showlegend=False)
     return render_plot(fig, width, height, interactive, show, out_file)
+'''
 
 def spectral_eigenvalues(
     adata: AnnData,
     width: int = 600,
     height: int = 400,
     show: bool = True,
     interactive: bool = True,
@@ -203,15 +166,17 @@
     import plotly.express as px
     import pandas as pd
 
     data = adata.uns["spectral_eigenvalue"]
 
     df = pd.DataFrame({"Component": map(str, range(1, data.shape[0] + 1)), "Eigenvalue": data})
     fig = px.scatter(df, x="Component", y="Eigenvalue", template="plotly_white")
-    fig.add_vline(x=_detect(data))
+    n = find_elbow(data)
+    adata.uns["num_eigen"] = n
+    fig.add_vline(x=n)
 
     return render_plot(fig, width, height, interactive, show, out_file)
 
 def regions(
     data: AnnData | AnnDataSet,
     groupby: str | list[str],
     peaks: dict[str, list[str]],
@@ -248,15 +213,16 @@
     'plotly.graph_objects.Figure' | None
         If `show=False` and `out_file=None`, an `plotly.graph_objects.Figure` will be 
         returned, which can then be further customized using the plotly API.
     """
     import polars as pl
     import plotly.graph_objects as go
 
-    count = pl.DataFrame(aggregate_X(data, groupby=groupby, normalize="RPKM"))
+    count = aggregate_X(data, groupby=groupby, normalize="RPKM")
+    count = pl.DataFrame(count.X.T, schema=list(count.obs_names))
     idx = data.var_ix(np.concatenate(list(peaks.values())).tolist())
     mat = np.log2(1 + count.to_numpy()[idx, :])
 
     trace = go.Heatmap(
         x=count.columns,
         y=np.concatenate(list(peaks.values()))[::-1],
         z=mat,
@@ -270,23 +236,20 @@
         "xaxis": { "title": groupby },
     }
     fig = go.Figure(data=data, layout=layout)
     return render_plot(fig, width, height, interactive, show, out_file)
 
 def umap(
     adata: AnnData,
-    color: str | np.ndarray,
+    color: str | np.ndarray | None = None,
     use_rep: str = "X_umap",
-    marker_size: float = 2,
-    marker_opacity: float = 0.5,
-    width: float = 550,
-    height: float = 500,
-    show: bool = True,
-    interactive: bool = True,
-    out_file: str | None = None,
+    marker_size: float = None,
+    marker_opacity: float = 1,
+    sample_size: int | None = None,
+    **kwargs,
 ) -> 'plotly.graph_objects.Figure' | None:
     """Plot the UMAP embedding.
 
     Parameters
     ----------
     adata
         Annotated data matrix.
@@ -295,108 +258,81 @@
         `obs`.
     use_rep
         Use the indicated representation in `.obsm`.
     marker_size
         Size of the dots.
     marker_opacity
         Opacity of the dots.
-    width
-        The width of the plot.
-    height
-        The height of the plot.
-    interactive
-        Whether to make interactive plot.
-    out_file
-        Path of the output file for saving the output image, end with
-        '.svg' or '.pdf' or '.png' or '.html'.
+    sample_size
+        If the number of cells is larger than `sample_size`, a random sample of
+        `sample_size` cells will be used for plotting.
+    kwargs        
+        Additional arguments passed to :func:`~snapatac2.pl.render_plot` to
+        control the final plot output. Please see :func:`~snapatac2.pl.render_plot`
+        for details.
 
     Returns
     -------
     'plotly.graph_objects.Figure' | None
         If `show=False` and `out_file=None`, an `plotly.graph_objects.Figure` will be 
         returned, which can then be further customized using the plotly API.
     """
-    import plotly.express as px
     from natsort import index_natsorted
-    import pandas as pd
 
     embedding = adata.obsm[use_rep] 
 
     if isinstance(color, str):
         groups = adata.obs[color].to_numpy()
     else:
         groups = color
         color = "color"
-
-    idx = index_natsorted(groups)
-    embedding = embedding[idx, :]
-    groups = [groups[i] for i in idx]
+    
+    if sample_size is not None and adata.shape[0] > sample_size:
+        idx = np.random.choice(adata.shape[0], sample_size, replace=False)
+        embedding = embedding[idx, :]
+        if groups is not None: groups = groups[idx]
+
+    if groups is not None:
+        idx = index_natsorted(groups)
+        embedding = embedding[idx, :]
+        groups = [groups[i] for i in idx]
+
+    if marker_size is None:
+        num_points = embedding.shape[0]
+        marker_size = (1000 / num_points)**(1/3) * 3
 
     if embedding.shape[1] >= 3:
-        df = pd.DataFrame({
-            "UMAP-1": embedding[:, 0],
-            "UMAP-2": embedding[:, 1],
-            "UMAP-3": embedding[:, 2],
-            color: groups,
-        })
-        fig = px.scatter_3d(df,
-            x='UMAP-1', y='UMAP-2', z='UMAP-3',
-            color=color,
-            color_discrete_sequence=px.colors.qualitative.Dark24,
-        )
+        return scatter3d(embedding[:, 0], embedding[:, 1], embedding[:, 2], color=groups,
+            x_label="UMAP-1", y_label="UMAP-2", z_label="UMAP-3", color_label=color,
+            marker_size=marker_size, marker_opacity=marker_opacity, **kwargs)
     else:
-        df = pd.DataFrame({
-            "UMAP-1": embedding[:, 0],
-            "UMAP-2": embedding[:, 1],
-            color: groups,
-        })
-        fig = px.scatter(
-            df, x="UMAP-1", y="UMAP-2", color=color,
-            color_discrete_sequence=px.colors.qualitative.Dark24,
-        )
-    fig.update_traces(
-        marker_size=marker_size,
-        marker={"opacity": marker_opacity},
-    )
-
-    fig.update_layout(
-        template="simple_white",
-        legend= {'itemsizing': 'constant'},
-    )
-    return render_plot(fig, width, height, interactive, show, out_file)
+        return scatter(embedding[:, 0], embedding[:, 1], color=groups,
+            x_label="UMAP-1", y_label="UMAP-2", color_label=color,
+            marker_size=marker_size, marker_opacity=marker_opacity, **kwargs)
 
 def motif_enrichment(
     enrichment: list(str, 'pl.DataFrame'),
     min_log_fc: float = 1,
     max_fdr: float = 0.01,
-    width: float = 600,
-    height: float = 400,
-    show: bool = True,
-    interactive: bool = True,
-    out_file: str | None = None,
+    **kwargs,
 ) -> 'plotly.graph_objects.Figure' | None:
     """Plot the motif enrichment result.
 
     Parameters
     ----------
     enrichment
         Motif enrichment result.
     min_log_fc
         Retain motifs that satisfy: log2-fold-change >= `min_log_fc`.
     max_fdr
         Retain motifs that satisfy: FDR <= `max_fdr`.
-    width
-        The width of the plot.
-    height
-        The height of the plot.
-    interactive
-        Whether to make interactive plot.
-    out_file
-        Path of the output file for saving the output image, end with
-        '.svg' or '.pdf' or '.png' or '.html'.
+    kwargs        
+        Additional arguments passed to :func:`~snapatac2.pl.render_plot` to
+        control the final plot output. Please see :func:`~snapatac2.pl.render_plot`
+        for details.
 
     Returns
     -------
     'plotly.graph_objects.Figure' | None
         If `show=False` and `out_file=None`, an `plotly.graph_objects.Figure` will be 
         returned, which can then be further customized using the plotly API.
     """
@@ -416,26 +352,17 @@
     minval = np.min(pvals[np.nonzero(pvals)])
     pvals = np.clip(pvals, minval, None)
     pvals = sign * np.log(-np.log10(pvals))
 
     df = pd.DataFrame(
         pvals.T,
         columns=list(enrichment.keys()),
-        index=next(iter(enrichment.values()))['motif name'].to_numpy()[passed],
+        index=next(iter(enrichment.values()))['id'].to_numpy()[passed],
     )
       
-    fig = heatmap(
+    return heatmap(
         df.to_numpy(),
         row_names=df.index,
         column_names=df.columns,
         colorscale='RdBu_r',
-    )
-    return render_plot(fig, width, height, interactive, show, out_file)
-
-def _detect(x, saturation=0.01):
-    accum_gap = 0
-    for i in range(1, len(x)):
-        gap = x[i-1] - x[i]
-        accum_gap = accum_gap + gap
-        if gap < saturation * accum_gap:
-            return i
-    return None
+        **kwargs,
+    )
```

### Comparing `snapatac2-2.2.0/snapatac2/plotting/_network.py` & `snapatac2-2.3.0/snapatac2/plotting/_network.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.2.0/snapatac2/preprocessing/_basic.py` & `snapatac2-2.3.0/snapatac2/preprocessing/_basic.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 from typing_extensions import Literal
 
 from pathlib import Path
 import numpy as np
-import math
+import anndata as ad
+import logging
 
+import snapatac2
 from snapatac2._snapatac2 import AnnData, AnnDataSet, PyFlagStat
 import snapatac2._snapatac2 as internal
 from snapatac2.genome import Genome
-from snapatac2._utils import is_anndata 
 
 def make_fragment_file(
     bam_file: Path,
     output_file: Path,
     is_paired: bool = True,
     barcode_tag: str | None = None,
     barcode_regex: str | None = None,
@@ -56,47 +57,55 @@
         `A01535:24:HW2MMDSX2:2:1359:8513:3458:bd:69:Y6:10:TGATAGGTTG`.
     umi_tag
         Extract UMI from TAG fields of BAM records.
     umi_regex
         Extract UMI from read names of BAM records using regular expressions.
         See `barcode_regex` for more details.
     shift_left
-        Insertion site correction for the left end.
+        Insertion site correction for the left end. Note this has no effect on single-end reads.
     shift_right
-        Insertion site correction for the right end.
+        Insertion site correction for the right end. Note this has no effect on single-end reads.
     min_mapq
         Filter the reads based on MAPQ.
     chunk_size
         The size of data retained in memory when performing sorting. Larger chunk sizes
         result in faster sorting and greater memory usage.
 
     Returns
     -------
     PyFlagStat
         Various statistics.
     """
+    if barcode_tag is None and barcode_regex is None:
+        raise ValueError("Either barcode_tag or barcode_regex must be set.")
+    if barcode_tag is not None and barcode_regex is not None:
+        raise ValueError("Only one of barcode_tag or barcode_regex can be set.")
+
     return internal.make_fragment_file(
-        bam_file, output_file, is_paired, barcode_tag, barcode_regex,
-        umi_tag, umi_regex, shift_left, shift_right, min_mapq, chunk_size
+        bam_file, output_file, is_paired, shift_left, shift_right, chunk_size,
+        barcode_tag, barcode_regex, umi_tag, umi_regex, min_mapq,
     )
 
 def import_data(
     fragment_file: Path,
     *,
     file: Path | None = None,
     genome: Genome | None = None,
-    gff_file: Path | None = None,
+    gene_anno: Path | None = None,
     chrom_size: dict[str, int] | None = None,
     min_num_fragments: int = 200,
     min_tsse: float = 1,
     sorted_by_barcode: bool = True,
     low_memory: bool = True,
     whitelist: Path | list[str] | None = None,
+    shift_left: int = 0,
+    shift_right: int = 0,
     chunk_size: int = 2000,
     tempdir: Path | None = None,
+    backend: str | None = None,
 ) -> AnnData:
     """Import dataset and compute QC metrics.
 
     This function will store fragments as base-resolution TN5 insertions in the
     resulting h5ad file (in `.obsm['insertion']`), along with the chromosome
     sizes (in `.uns['reference_sequences']`). Various QC metrics, including TSSe,
     number of unique fragments, duplication rate, fraction of mitochondrial DNA
@@ -107,22 +116,26 @@
     fragment_file
         File name of the fragment file.
     file
         File name of the output h5ad file used to store the result. If provided,
         result will be saved to a backed AnnData, otherwise an in-memory AnnData
         is used.
     genome
-        A Genome object. If not set, `gff_file` and `chrom_size` must be provided.
-    gff_file
-        File name of the gene annotation file in GFF format.
+        A Genome object, providing gene annotation and chromosome sizes.
+        If not set, `gff_file` and `chrom_size` must be provided.
+        `genome` has lower priority than `gff_file` and `chrom_size`.
+    gene_anno
+        File name of the gene annotation file in GFF or GTF format.
         This is required if `genome` is not set.
+        Setting `gene_anno` will override the `genome` parameter.
     chrom_size
         A dictionary containing chromosome sizes, for example,
         `{"chr1": 2393, "chr2": 2344, ...}`.
         This is required if `genome` is not set.
+        Setting `chrom_size` will override the `genome` parameter.
     min_num_fragments
         Number of unique fragments threshold used to filter cells
     min_tsse
         TSS enrichment threshold used to filter cells
     sorted_by_barcode
         Whether the fragment file has been sorted by cell barcodes.
         If `sorted_by_barcode == True`, this function makes use of small fixed amout of 
@@ -132,139 +145,213 @@
         Whether to use the low memory mode when `sorted_by_barcode == False`.
         It does this by first sort the records by barcodes and then process them
         in batch. The parameter has no effect when `sorted_by_barcode == True`.
     whitelist
         File name or a list of barcodes. If it is a file name, each line
         must contain a valid barcode. When provided, only barcodes in the whitelist
         will be retained.
+    shift_left
+        Insertion site correction for the left end.
+    shift_right
+        Insertion site correction for the right end. Note this has no effect on single-end reads.
+        For single-end reads, `shift_right` will be set using the value of `shift_left`.
     chunk_size
         Increasing the chunk_size speeds up I/O but uses more memory.
     tempdir
         Location to store temporary files. If `None`, system temporary directory
         will be used.
+    backend
+        The backend.
 
     Returns
     -------
     AnnData | ad.AnnData
         An annotated data matrix of shape `n_obs` x `n_vars`. Rows correspond to
         cells and columns to regions. If `file=None`, an in-memory AnnData will be
         returned, otherwise a backed AnnData is returned.
     """
     if genome is not None:
-        chrom_size = genome.chrom_sizes
-        gff_file = genome.fetch_annotations()
+        if chrom_size is None:
+            chrom_size = genome.chrom_sizes
+        if gene_anno is None:
+            gene_anno = genome.fetch_annotations()
 
     if whitelist is not None:
         if isinstance(whitelist, str) or isinstance(whitelist, Path):
             with open(whitelist, "r") as fl:
                 whitelist = set([line.strip() for line in fl])
         else:
             whitelist = set(whitelist)
-    return internal.import_fragments(
-        file, fragment_file, gff_file, chrom_size, min_num_fragments,
-        min_tsse, sorted_by_barcode, low_memory, whitelist, chunk_size, tempdir
+        
+    adata = ad.AnnData() if file is None else AnnData(filename=file, backend=backend)
+    internal.import_fragments(
+        adata, fragment_file, gene_anno, chrom_size, min_num_fragments,
+        min_tsse, sorted_by_barcode, low_memory, shift_left, shift_right,
+        chunk_size, whitelist, tempdir,
     )
+    return adata
 
 def add_tile_matrix(
-    adata: AnnData,
+    adata: AnnData | list[AnnData],
+    *,
     bin_size: int = 500,
+    inplace: bool = True,
     chunk_size: int = 500,
-    n_jobs: int = 4
-) -> None:
+    exclude_chroms: list[str] | str | None = ["chrM", "chrY", "M", "Y"],
+    file: Path | None = None,
+    backend: str | None = None,
+    n_jobs: int = 8,
+) -> AnnData | None:
     """Generate cell by bin count matrix.
 
     This function is used to generate and add a cell by bin count matrix to the AnnData
     object.
 
     :func:`~snapatac2.pp.import_data` must be ran first in order to use this function.
 
     Parameters
     ----------
     adata
         The (annotated) data matrix of shape `n_obs` x `n_vars`.
         Rows correspond to cells and columns to regions.
+        `adata` could also be a list of AnnData objects when `inplace=True`.
+        In this case, the function will be applied to each AnnData object in parallel.
     bin_size
         The size of consecutive genomic regions used to record the counts.
+    inplace
+        Whether to add the tile matrix to the AnnData object or return a new AnnData object.
     chunk_size
         Increasing the chunk_size speeds up I/O but uses more memory.
+    exclude_chroms
+        A list of chromosomes to exclude.
+    file
+        File name of the output file used to store the result. If provided, result will
+        be saved to a backed AnnData, otherwise an in-memory AnnData is used.
+    backend
+        The backend to use for storing the result. If `None`, the default backend will be used.
     n_jobs
-        Number of CPUs to use.
+        Number of jobs to run in parallel when `adata` is a list.
+        If `n_jobs=-1`, all CPUs will be used.
     """
-    internal.mk_tile_matrix(adata, bin_size, chunk_size, n_jobs)
+    if isinstance(exclude_chroms, str):
+        exclude_chroms = [exclude_chroms]
+
+    if inplace:
+        if isinstance(adata, list):
+            snapatac2._utils.anndata_par(
+                adata,
+                lambda x: internal.mk_tile_matrix(x, bin_size, chunk_size, exclude_chroms, None),
+                n_jobs=n_jobs,
+            )
+        else:
+            internal.mk_tile_matrix(adata, bin_size, chunk_size, exclude_chroms, None)
+    else:
+        if file is None:
+            if adata.isbacked:
+                out = ad.AnnData(obs=adata.obs[:].to_pandas())
+            else:
+                out = ad.AnnData(obs=adata.obs[:])
+        else:
+            out = AnnData(filename=file, backend=backend, obs=adata.obs[:])
+        internal.mk_tile_matrix(adata, bin_size, chunk_size, exclude_chroms, out)
+        return out
 
 def make_peak_matrix(
     adata: AnnData | AnnDataSet,
+    *,
+    use_rep: str | list[str] | None = None,
+    inplace: bool = False,
     file: Path | None = None,
-    use_rep: str | list[str] = "peaks",
+    backend: str | None = None,
     peak_file: Path | None = None,
     chunk_size: int = 500,
+    use_x: bool = False,
 ) -> AnnData:
     """Generate cell by peak count matrix.
 
     This function will generate a cell by peak count matrix and store it in a 
     new .h5ad file.
 
     :func:`~snapatac2.pp.import_data` must be ran first in order to use this function.
 
     Parameters
     ----------
     adata
         The (annotated) data matrix of shape `n_obs` x `n_vars`.
         Rows correspond to cells and columns to regions.
-    file
-        File name of the output h5ad file used to store the result. If provided,
-        result will be saved to a backed AnnData, otherwise an in-memory AnnData
-        is used.
     use_rep
         This is used to read peak information from `.uns[use_rep]`.
         The peaks can also be provided by a list of strings:
         ["chr1:1-100", "chr2:2-200"].
+    inplace
+        Whether to add the tile matrix to the AnnData object or return a new AnnData object.
+    file
+        File name of the output h5ad file used to store the result. If provided,
+        result will be saved to a backed AnnData, otherwise an in-memory AnnData
+        is used.
+    backend
+        The backend to use for storing the result. If `None`, the default backend will be used.
     peak_file
         Bed file containing the peaks. If provided, peak information will be read
         from this file.
     chunk_size
         Chunk size
+    use_x
+        If True, use the matrix stored in `.X` as raw counts.
+        Otherwise the `.obsm['insertion']` is used.
 
     Returns
     -------
-    AnnData | ad.AnnData
+    AnnData | ad.AnnData | None
         An annotated data matrix of shape `n_obs` x `n_vars`. Rows correspond to
         cells and columns to peaks. If `file=None`, an in-memory AnnData will be
         returned, otherwise a backed AnnData is returned.
     """
     import gzip
 
     if peak_file is not None and use_rep is not None:
         raise RuntimeError("'peak_file' and 'use_rep' cannot be both set") 
 
+    if use_rep is None and peak_file is None:
+        use_rep = "peaks"
+
     if isinstance(use_rep, str):
         df = adata.uns[use_rep]
         peaks = df[df.columns[0]]
     else:
         peaks = use_rep
 
     if peak_file is not None:
         if Path(peak_file).suffix == ".gz":
             with gzip.open(peak_file, 'rt') as f:
                 peaks = [line.strip() for line in f]
         else:
             with open(peak_file, 'r') as f:
                 peaks = [line.strip() for line in f]
 
-    anndata = internal.mk_peak_matrix(adata, peaks, file, chunk_size)
-    if file is None and adata.isbacked: # anndata accepts only pandas DataFrame
-        anndata.obs = adata.obs[:].to_pandas()
+    if inplace:
+        internal.mk_peak_matrix(adata, peaks, chunk_size, use_x, None)
     else:
-        anndata.obs = adata.obs[:]
-    return anndata
+        if file is None:
+            if adata.isbacked:
+                out = ad.AnnData(obs=adata.obs[:].to_pandas())
+            else:
+                out = ad.AnnData(obs=adata.obs[:])
+        else:
+            out = AnnData(filename=file, backend=backend, obs=adata.obs[:])
+        internal.mk_peak_matrix(adata, peaks, chunk_size, use_x, out)
+        return out
 
 def make_gene_matrix(
     adata: AnnData | AnnDataSet,
-    gff_file: Genome | Path,
+    gene_anno: Genome | Path,
+    *,
+    inplace: bool = False,
     file: Path | None = None,
+    backend: str | None = None,
     chunk_size: int = 500,
     use_x: bool = False,
     id_type: Literal['gene', 'transcript'] = "gene",
 ) -> AnnData:
     """Generate cell by gene activity matrix.
 
     Generate cell by gene activity matrix by counting the TN5 insertions in gene
@@ -272,16 +359,16 @@
     will be created.
 
     Parameters
     ----------
     adata
         The (annotated) data matrix of shape `n_obs` x `n_vars`.
         Rows correspond to cells and columns to regions.
-    gff_file
-        Either a Genome object or the path of a gene annotation file in GFF format.
+    gene_anno
+        Either a Genome object or the path of a gene annotation file in GFF or GTF format.
     file
         File name of the h5ad file used to store the result.
     chunk_size
         Chunk size
     use_x
         If True, use the matrix stored in `.X` to compute the gene activity.
         Otherwise the `.obsm['insertion']` is used.
@@ -289,23 +376,29 @@
         "gene" or "transcript".
 
     Returns
     -------
     AnnData
         A new AnnData object, where rows correspond to cells and columns to genes.
     """
-    if isinstance(gff_file, Genome):
-        gff_file = gff_file.fetch_annotations()
+    if isinstance(gene_anno, Genome):
+        gene_anno = gene_anno.fetch_annotations()
 
-    anndata = internal.mk_gene_matrix(adata, gff_file, file, chunk_size, use_x, id_type)
-    if file is None and adata.isbacked: # anndata accepts only pandas DataFrame
-        anndata.obs = adata.obs[:].to_pandas()
+    if inplace:
+        internal.mk_gene_matrix(adata, gene_anno, chunk_size, use_x, id_type, None)
     else:
-        anndata.obs = adata.obs[:]
-    return anndata
+        if file is None:
+            if adata.isbacked:
+                out = ad.AnnData(obs=adata.obs[:].to_pandas())
+            else:
+                out = ad.AnnData(obs=adata.obs[:])
+        else:
+            out = AnnData(filename=file, backend=backend, obs=adata.obs[:])
+        internal.mk_gene_matrix(adata, gene_anno, chunk_size, use_x, id_type, out)
+        return out
 
 def filter_cells(
     data: AnnData,
     min_counts: int | None = 1000,
     min_tsse: float | None = 5.0,
     max_counts: int | None = None,
     max_tsse: float | None = None,
@@ -349,72 +442,129 @@
     if inplace:
         if data.isbacked:
             data.subset(selected_cells)
         else:
             data._inplace_subset_obs(selected_cells)
     else:
         return selected_cells
+
+def _find_most_accessible_features(
+    feature_count,
+    filter_lower_quantile,
+    filter_upper_quantile,
+    total_features,
+) -> np.ndarray:
+    idx = np.argsort(feature_count)
+    for i in range(idx.size):
+        if feature_count[idx[i]] > 0:
+            break
+    idx = idx[i:]
+    n = idx.size
+    n_lower = int(filter_lower_quantile * n)
+    n_upper = int(filter_upper_quantile * n)
+    idx = idx[n_lower:n-n_upper]
+    return idx[::-1][:total_features]
+ 
  
 def select_features(
-    adata: AnnData | AnnDataSet,
-    min_cells: int = 1,
-    most_variable: int | float | None = 1000000,
+    adata: AnnData | AnnDataSet | list[AnnData],
+    n_features: int = 500000,
+    filter_lower_quantile: float = 0.005,
+    filter_upper_quantile: float = 0.005,
     whitelist: Path | None = None,
     blacklist: Path | None = None,
+    max_iter: int = 1,
     inplace: bool = True,
-) -> np.ndarray | None:
+    n_jobs: int = 8,
+) -> np.ndarray | list[np.ndarray] | None:
     """
     Perform feature selection.
 
     Note
     ----
     This function does not perform the actual subsetting. The feature mask is used by
     various functions to generate submatrices on the fly.
 
     Parameters
     ----------
     adata
         The (annotated) data matrix of shape `n_obs` x `n_vars`.
         Rows correspond to cells and columns to regions.
-    min_cells
-        Minimum number of cells.
-    most_variable
-        If None, do not perform feature selection using most variable features
+        `adata` can also be a list of AnnData objects.
+        In this case, the function will be applied to each AnnData object in parallel.
+    n_features
+        Number of features to keep. Note that the final number of features
+        may be smaller than this number if there is not enough features that pass
+        the filtering criteria.
+    filter_lower_quantile
+        Lower quantile of the feature count distribution to filter out.
+    filter_upper_quantile
+        Upper quantile of the feature count distribution to filter out.
     whitelist
         A user provided bed file containing genome-wide whitelist regions.
-        Features that are overlapped with these regions will be retained.
+        None-zero features listed here will be kept regardless of the other
+        filtering criteria.
     blacklist 
         A user provided bed file containing genome-wide blacklist regions.
         Features that are overlapped with these regions will be removed.
     inplace
         Perform computation inplace or return result.
+    n_jobs
+        Number of parallel jobs to use when `adata` is a list.
     
     Returns
     -------
     np.ndarray | None:
         If `inplace = False`, return a boolean index mask that does filtering,
         where `True` means that the feature is kept, `False` means the feature is removed.
         Otherwise, store this index mask directly to `.var['selected']`.
     """
+    if isinstance(adata, list):
+        result = snapatac2._utils.anndata_par(
+            adata,
+            lambda x: select_features(x, n_features, filter_lower_quantile, filter_upper_quantile, whitelist, blacklist, max_iter, inplace),
+            n_jobs=n_jobs,
+        )
+        if inplace:
+            return None
+        else:
+            return result
+
     count = np.zeros(adata.shape[1])
     for batch, _, _ in adata.chunked_X(2000):
-        batch.data = np.ones(batch.indices.shape, dtype=np.float64)
         count += np.ravel(batch.sum(axis = 0))
+    adata.var['count'] = count
 
-    selected_features = count >= min_cells
+    selected_features = _find_most_accessible_features(
+        count, filter_lower_quantile, filter_upper_quantile, n_features)
 
-    if whitelist is not None:
-        selected_features &= internal.intersect_bed(adata.var_names, str(whitelist))
     if blacklist is not None:
-        selected_features &= np.logical_not(internal.intersect_bed(adata.var_names, str(blacklist)))
+        blacklist = np.logical_not(internal.intersect_bed(adata.var_names, str(blacklist)))
+        selected_features = selected_features[np.logical_not(blacklist[selected_features])]
+
+    # Iteratively select features
+    iter = 1
+    while iter < max_iter:
+        embedding = snapatac2.tl.spectral(adata, features=selected_features, inplace=False)[1]
+        clusters = snapatac2.tl.leiden(snapatac2.pp.knn(embedding, inplace=False))
+        rpm = snapatac2.tl.aggregate_X(adata, groupby=clusters).X
+        var = np.var(np.log(rpm + 1), axis=0)
+        selected_features = np.argsort(var)[::-1][:n_features]
+
+        if blacklist is not None:
+            selected_features = selected_features[np.logical_not(blacklist[selected_features])]
+        iter += 1
+
+    result = np.zeros(adata.shape[1], dtype=bool)
+    result[selected_features] = True
 
-    if most_variable is not None and len(count[selected_features]) > most_variable:
-        mean = count[selected_features].mean()
-        std = math.sqrt(count[selected_features].var())
-        zscores = np.absolute((count - mean) / std)
-        cutoff = np.sort(zscores)[most_variable - 1]
-        selected_features &= zscores <= cutoff
+    if whitelist is not None:
+        whitelist = np.array(internal.intersect_bed(adata.var_names, str(whitelist)))
+        whitelist &= count != 0
+        result |= whitelist
+    
+    logging.info(f"Selected {result.sum()} features.")
 
     if inplace:
-        adata.var["selected"] = selected_features
+        adata.var["selected"] = result
     else:
-        return selected_features
+        return result
```

### Comparing `snapatac2-2.2.0/snapatac2/preprocessing/_harmony.py` & `snapatac2-2.3.0/snapatac2/preprocessing/_harmony.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,17 +6,20 @@
 import numpy as np
 
 from snapatac2._snapatac2 import AnnData, AnnDataSet
 from snapatac2._utils import is_anndata 
 
 def harmony(
     adata: AnnData | AnnDataSet | np.ndarray,
-    batch: str,
-    use_dims: int | list[int] | None = None,
+    *,
+    batch: str | list[str],
     use_rep: str = "X_spectral",
+    use_dims: int | list[int] | None = None,
+    groupby: str | list[str] | None = None,
+    key_added: str | None = None,
     inplace: bool = True,
     **kwargs,
 ) -> np.ndarray | None:
     """
     Use harmonypy to integrate different experiments.
 
     Harmony is an algorithm for integrating single-cell
@@ -29,45 +32,74 @@
     ----------
     adata
         The (annotated) data matrix of shape `n_obs` x `n_vars`.
         Rows correspond to cells and columns to regions.
     batch
         The name of the column in ``adata.obs`` that differentiates
         among experiments/batches.
-    use_dims
-        Use these dimensions in `use_rep`.
     use_rep
         The name of the field in ``adata.obsm`` where the lower dimensional
         representation is stored.
+    use_dims
+        Use these dimensions in `use_rep`.
+    groupby
+        If specified, split the data into groups and perform batch correction
+        on each group separately.
+    key_added
+        If specified, add the result to ``adata.obsm`` with this key. Otherwise,
+        it will be stored in ``adata.obsm[use_rep + "_harmony"]``.
     inplace
         Whether to store the result in the anndata object.
     kwargs
         Any additional arguments will be passed to
         ``harmonypy.run_harmony()``.
 
     Returns
     -------
     np.ndarray | None
         if `inplace=True` it updates adata with the field
         ``adata.obsm[`use_rep`_harmony]``, containing principal components
         adjusted by Harmony such that different experiments are integrated.
         Otherwise, it returns the result as a numpy array.
     """
-    try:
-        import harmonypy
-    except ImportError:
-        raise ImportError("\nplease install harmonypy:\n\n\tpip install harmonypy")
-
+    # Check if the data is in an AnnData object
     if is_anndata(adata):
         mat = adata.obsm[use_rep]
     else:
         mat = adata
         inplace = False
 
+    # Use only the specified dimensions
     if isinstance(use_dims, int): use_dims = range(use_dims) 
     mat = mat if use_dims is None else mat[:, use_dims]
 
-    harmony_out = harmonypy.run_harmony(mat, adata.obs[...].to_pandas(), batch, **kwargs)
+    # Create a pandas dataframe with the batch information
+    if isinstance(batch, str):
+        batch = adata.obs[batch]
+
+    if groupby is None:
+        mat = _harmony(mat, batch, **kwargs)
+    else:
+        if isinstance(groupby, str): groupby = adata.obs[groupby]
+        groups = list(set(groupby))
+        for group in groups:
+            group_idx = [i for i, x in enumerate(groupby) if x == group]
+            mat[group_idx, :] = _harmony(mat[group_idx, :], batch[group_idx], **kwargs)
+
     if inplace:
-        adata.obsm[use_rep + "_harmony"] = harmony_out.Z_corr.T
+        if key_added is None:
+            adata.obsm[use_rep + "_harmony"] = mat
+        else:
+            adata.obsm[key_added] = mat
     else:
-        return harmony_out.Z_corr.T
+        return mat
+
+def _harmony(data_matrix, batch_labels, **kwargs):
+    try:
+        import harmonypy
+    except ImportError:
+        raise ImportError("\nplease install harmonypy:\n\n\tpip install harmonypy")
+    import pandas as pd
+
+    meta = pd.DataFrame({'batch': np.array(batch_labels)})
+    harmony_out = harmonypy.run_harmony(data_matrix, meta, 'batch', **kwargs)
+    return harmony_out.Z_corr.T
```

### Comparing `snapatac2-2.2.0/snapatac2/preprocessing/_knn.py` & `snapatac2-2.3.0/snapatac2/preprocessing/_knn.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 from __future__ import annotations
+from typing_extensions import Literal
 
 import numpy as np
 from scipy.sparse import csr_matrix
 
-from snapatac2._utils import is_anndata 
+from snapatac2._utils import is_anndata
 from snapatac2._snapatac2 import AnnData, AnnDataSet, approximate_nearest_neighbors
 
 # TODO: add random state
 def knn(
     adata: AnnData | AnnDataSet | np.ndarray,
     n_neighbors: int = 50,
     use_dims: int | list[int] | None = None,
     use_rep: str | None = None,
-    use_approximate_search: bool = True,
+    method: Literal['hora', 'pynndescent', 'exact'] = "hora",
     n_jobs: int = -1,
     inplace: bool = True,
+    random_state: int = 0,
 ) -> csr_matrix | None:
     """
     Compute a neighborhood graph of observations.
 
     Parameters
     ----------
     adata
         Annotated data matrix or numpy array.
     n_neighbors
         The number of nearest neighbors to be searched.
     use_dims
         The dimensions used for computation.
     use_rep
         The key for the matrix
-    use_approximate_search
-        Whether to use approximate nearest neighbor search
+    method
+        'hora', 'pynndescent', or 'exact'
     n_jobs
         number of CPUs to use
     inplace
         Whether to store the result in the anndata object.
+    random_state
+        Random seed for approximate nearest neighbor search.
 
     Returns
     -------
     csr_matrix | None
         if `inplace=True`, store KNN in `.obsp['distances']`.
         Otherwise, return a sparse matrix.
     """
@@ -54,18 +58,27 @@
     if use_dims is not None:
         if isinstance(use_dims, int):
             data = data[:, :use_dims]
         else:
             data = data[:, use_dims]
 
     n = data.shape[0]
-    if use_approximate_search:
+    if method == 'hora':
         (d, indices, indptr) = approximate_nearest_neighbors(data.astype(np.float32), n_neighbors)
         adj = csr_matrix((d, indices, indptr), shape=(n, n))
+    elif method == 'pynndescent':
+        import pynndescent
+        index = pynndescent.NNDescent(data, n_neighbors=max(50, n_neighbors), random_state=random_state)
+        adj, distances = index.neighbor_graph
+        indices = np.ravel(adj[:, :n_neighbors])
+        distances = np.ravel(distances[:, :n_neighbors]) 
+        indptr = np.arange(0, distances.size + 1, n_neighbors)
+        adj = csr_matrix((distances, indices, indptr), shape=(n, n))
     else:
         from sklearn.neighbors import kneighbors_graph
         adj = kneighbors_graph(data, n_neighbors, mode='distance', n_jobs=n_jobs)
+        adj.sort_indices()
     
     if inplace:
         adata.obsp['distances'] = adj
     else:
         return adj
```

### Comparing `snapatac2-2.2.0/snapatac2/preprocessing/_mnn_correct.py` & `snapatac2-2.3.0/snapatac2/preprocessing/_mnn_correct.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,43 +5,55 @@
 from scipy.special import logsumexp
 
 from snapatac2._snapatac2 import AnnData, AnnDataSet
 from snapatac2._utils import is_anndata 
 
 def mnc_correct(
     adata: AnnData | AnnDataSet | np.adarray,
+    *,
     batch: str | list[str],
     n_neighbors: int = 5,
     n_clusters: int = 40,
-    use_dims: int | list[int] | None = None,
-    use_rep: str = "X_spectral",
     n_iter: int = 1,
+    use_rep: str = "X_spectral",
+    use_dims: int | list[int] | None = None,
+    groupby: str | list[str] | None = None,
+    key_added: str | None = None,
     inplace: bool = True,
+    n_jobs: int = 8,
 ) -> np.ndarray | None:
     """
     A modified MNN-Correct algorithm based on cluster centroid.
 
     Parameters
     ----------
     data
         Matrice or AnnData object. Matrices should be shaped like n_obs x n_vars.
     batch
         Batch labels for cells. If a string, labels will be obtained from `obs`.
     n_neighbors
         Number of mutual nearest neighbors.
     n_clusters
         Number of clusters
-    use_dims
-        Use these dimensions in `use_rep`.
-    use_rep
-        Use the indicated representation in `.obsm`.
     n_iter
         Number of iterations.
+    use_rep
+        Use the indicated representation in `.obsm`.
+    use_dims
+        Use these dimensions in `use_rep`.
+    groupby
+        If specified, split the data into groups and perform batch correction
+        on each group separately.
+    key_added
+        If specified, add the result to ``adata.obsm`` with this key. Otherwise,
+        it will be stored in ``adata.obsm[use_rep + "_mnn"]``.
     inplace
         Whether to store the result in the anndata object.
+    n_jobs
+        Number of jobs to use for parallelization.
 
     Returns
     -------
     np.ndarray | None
         if `inplace=True` it updates adata with the field
         ``adata.obsm[`use_rep`_mnn]``, containing adjusted principal components.
         Otherwise, it returns the result as a numpy array.
@@ -52,57 +64,93 @@
         mat = adata
         inplace = False
 
     if isinstance(use_dims, int): use_dims = range(use_dims) 
     mat = mat if use_dims is None else mat[:, use_dims]
     mat = np.asarray(mat)
 
-    if isinstance(batch, str):
-        labels = adata.obs[batch]
+    if isinstance(batch, str): labels = adata.obs[batch]
 
-    label_uniq = list(set(labels))
+    if groupby is None:
+        mat = _mnc_correct_main(mat, labels, n_iter, n_neighbors, n_clusters)
+    else:
+        from multiprocess import Pool
+
+        if isinstance(groupby, str): groupby = adata.obs[groupby]
 
-    for _ in range(n_iter):
-        batch_idx = []
-        data_by_batch = []
-        for label in label_uniq:
-            idx = [i for i, x in enumerate(labels) if x == label]
-            batch_idx.append(idx)
-            data_by_batch.append(mat[idx,:])
-        mat_ = mnc_correct_multi(data_by_batch, n_neighbors, n_clusters)
-        new = np.array(mat, copy=True)
-        idx = list(itertools.chain.from_iterable(batch_idx))
-        for i in range(len(labels)):
-            new[idx[i]] = mat_[i,:]
-        mat = new
+        group_indices = {}
+        for i, group in enumerate(groupby):
+            if group in group_indices:
+                group_indices[group].append(i)
+            else:
+                group_indices[group] = [i]
+        group_indices = [x for x in group_indices.values()]
+
+        inputs = [(mat[group_idx, :], labels[group_idx]) for group_idx in group_indices]
+        with Pool(n_jobs) as p:
+            results = p.map(lambda x: _mnc_correct_main(x[0], x[1], n_iter, n_neighbors, n_clusters), inputs)
+        for idx, result in zip(group_indices, results):
+            mat[idx, :] = result
 
     if inplace:
-        adata.obsm[use_rep + "_mnn"] = mat
+        if key_added is None:
+            adata.obsm[use_rep + "_mnn"] = mat
+        else:
+            adata.obsm[key_added] = mat
     else:
         return mat
 
-def mnc_correct_multi(datas, n_neighbors, n_clusters):
+def _mnc_correct_main(
+    data_matrix,
+    batch_labels,
+    n_iter,
+    n_neighbors,
+    n_clusters,
+    random_state=0
+):
+    label_uniq = list(set(batch_labels))
+
+    if len(label_uniq) > 1:
+        for _ in range(n_iter):
+            batch_idx = []
+            data_by_batch = []
+            for label in label_uniq:
+                idx = [i for i, x in enumerate(batch_labels) if x == label]
+                batch_idx.append(idx)
+                data_by_batch.append(data_matrix[idx,:])
+            new_matrix = _mnc_correct_multi(data_by_batch, n_neighbors, n_clusters, random_state)
+
+            idx = list(itertools.chain.from_iterable(batch_idx))
+            idx = np.argsort(idx)
+            data_matrix = new_matrix[idx, :]
+    return data_matrix
+
+def _mnc_correct_multi(datas, n_neighbors, n_clusters, random_state):
     data0 = datas[0]
     for i in range(1, len(datas)):
         data1 = datas[i]
-        pdata0, pdata1 = mnc_correct_pair(data0, data1, n_clusters, n_neighbors)
+        pdata0, pdata1 = _mnc_correct_pair(data0, data1, n_clusters, n_neighbors, random_state)
         ratio = data0.shape[0] / (data0.shape[0] + data1.shape[0])
         data0_ = pdata0.project(data0, weight = 1 - ratio)
         data1_ = pdata1.project(data1, weight = ratio)
         data0 = np.concatenate((data0_, data1_), axis=0)
     return data0
 
-def mnc_correct_pair(X, Y, n_clusters, n_neighbors, random_state=0):
+def _mnc_correct_pair(X, Y, n_clusters, n_neighbors, random_state):
     from sklearn.neighbors import KDTree
     from sklearn.cluster import KMeans
 
     n_X = X.shape[0]
     n_Y = Y.shape[0]
-    c_X = KMeans(n_clusters=min(n_clusters, n_X), random_state=random_state).fit(X).cluster_centers_
-    c_Y = KMeans(n_clusters=min(n_clusters, n_Y), random_state=random_state).fit(Y).cluster_centers_
+    c_X = KMeans(
+        n_clusters=min(n_clusters, n_X), n_init=10, random_state=random_state
+    ).fit(X).cluster_centers_
+    c_Y = KMeans(
+        n_clusters=min(n_clusters, n_Y), n_init=10, random_state=random_state
+    ).fit(Y).cluster_centers_
 
     tree_X = KDTree(c_X)
     tree_Y = KDTree(c_Y)
 
     # X by Y matrix
     m_X = tree_Y.query(c_X, k=min(n_neighbors, n_Y), return_distance=False)
```

### Comparing `snapatac2-2.2.0/snapatac2/preprocessing/_scrublet.py` & `snapatac2-2.3.0/snapatac2/preprocessing/_scrublet.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 """ Implementation of the scrublet algorithm for single-cell ATAC-seq data
 """
 from __future__ import annotations
 
 import numpy as np
 import scipy.sparse as ss
 import logging
+import anndata as ad
 
-from .._utils import chunks
+from .._utils import chunks, anndata_par
 from snapatac2._snapatac2 import AnnData, approximate_nearest_neighbors
-from snapatac2.tools.embedding._spectral import Spectral
+from snapatac2.tools._embedding import spectral
 
 def scrublet(
-    adata: AnnData,
+    adata: AnnData | list[AnnData],
     features: str | np.ndarray | None = "selected",
     n_comps: int = 15,
     sim_doublet_ratio: float = 2.0,
     expected_doublet_rate: float = 0.1,
     n_neighbors: int | None = None,
     use_approx_neighbors=True,
     random_state: int = 0,
+    inplace: bool = True,
+    n_jobs: int = 8,
+    verbose: bool = True,
 ) -> None:
     """
     Compute probability of being a doublet using the scrublet algorithm.
 
     Parameters
     ----------
     adata
-        AnnData object
+        The (annotated) data matrix of shape `n_obs` x `n_vars`.
+        Rows correspond to cells and columns to regions.
+        `adata` can also be a list of AnnData objects.
+        In this case, the function will be applied to each AnnData object in parallel.
     features
         Boolean index mask, where `True` means that the feature is kept, and
         `False` means the feature is removed.
     n_comps
         Number of PCs
     sim_doublet_ratio
         Number of doublets to simulate relative to the number of observed cells.
@@ -40,117 +47,148 @@
         Number of neighbors used to construct the KNN graph of observed
         cells and simulated doublets. If `None`, this is 
         set to round(0.5 * sqrt(n_cells))
     use_approx_neighbors
         Whether to use approximate search.
     random_state
         Random state.
+    inplace
+        Whether update the AnnData object inplace
+    n_jobs
+        Number of jobs to run in parallel.
+    verbose
+        Whether to print progress messages.
     
     Returns
     -------
-    None
-        It updates adata with the following fields:
-            - ``adata.obs["doublet_score"]``: scrublet doublet score
-            - ``adata.uns["scrublet"]["sim_doublet_score"]``: doublet scores of simulated doublets 
+    tuple[np.ndarray, np.ndarray] | None:
+        if ``inplace = True``, it updates adata with the following fields:
+            - ``adata.obs["doublet_probability"]``: probability of being a doublet
+            - ``adata.obs["doublet_score"]``: doublet score
     """
-    #- adata.uns["scrublet_cell_embedding"]: embedding of cells
-    #- adata.uns["scrublet_sim_doublet_embedding"]: embedding of simulated doublets
+    if isinstance(adata, list):
+        result = anndata_par(
+            adata,
+            lambda x: scrublet(x, features, n_comps, sim_doublet_ratio, expected_doublet_rate, n_neighbors, use_approx_neighbors, random_state, inplace, n_jobs, verbose),
+            n_jobs=n_jobs,
+        )
+        if inplace:
+            return None
+        else:
+            return result
 
     if isinstance(features, str):
         if features in adata.var:
             features = adata.var[features]
         else:
             raise NameError("Please call `select_features` first or explicitly set `features = None`")
 
     if features is None:
-        count_matrix = adata.X[...]
+        count_matrix = adata.X[:]
     else:
         count_matrix = adata.X[:, features]
 
     if min(count_matrix.shape) == 0: raise NameError("Matrix is empty")
 
     if n_neighbors is None:
         n_neighbors = int(round(0.5 * np.sqrt(count_matrix.shape[0])))
 
-    (doublet_scores_obs, doublet_scores_sim, manifold_obs, manifold_sim) = scrub_doublets_core(
+    doublet_scores_obs, doublet_scores_sim, _, _ = scrub_doublets_core(
         count_matrix, n_neighbors, sim_doublet_ratio, expected_doublet_rate,
         n_comps=n_comps,
         use_approx_neighbors = use_approx_neighbors,
-        random_state=random_state
-        )
-    adata.obs["doublet_score"] = doublet_scores_obs
-    adata.uns["scrublet_sim_doublet_score"] = doublet_scores_sim
+        random_state=random_state,
+        verbose=False,
+    )
+    probs = get_doublet_probability(
+        doublet_scores_sim, doublet_scores_obs, random_state,
+    )
+ 
+    if inplace:
+        adata.obs["doublet_probability"] = probs
+        adata.obs["doublet_score"] = doublet_scores_obs
+        adata.uns["scrublet_sim_doublet_score"] = doublet_scores_sim
+    else:
+        return probs, doublet_scores_obs
 
-def call_doublets(
-    adata: AnnData,
-    threshold: str | float = "gmm",
-    random_state: int = 0,
+def filter_doublets(
+    adata: AnnData | list[AnnData],
+    probability_threshold: float | None = 0.5,
+    score_threshold: float | None = None,
     inplace: bool = True,
-) -> tuple[np.ndarray, float] | None:
+    n_jobs: int = 8,
+    verbose: bool = True,
+) -> np.ndarray | None:
     """
-    Find doublet score threshold for calling doublets.
-    `pp.scrublet` must be run first.
+    Remove doublets.
+    :func:`~snapatac2.pp.scrublet` must be ran first in order to use this function.
 
     Parameters
     ----------
     adata
-        AnnData object
-    threshold
-        Mannually specify a threshold or use one of the default methods to
-        automatically identify a threshold:
-
-        - 'gmm': fit a 2-component gaussian mixture model.
-        - 'scrublet': the method used in the scrublet paper (not implemented).
-    random_state
-        Random state
+        The (annotated) data matrix of shape `n_obs` x `n_vars`.
+        Rows correspond to cells and columns to regions.
+    probability_threshold
+        Threshold for doublet probability.
+    score_threshold
+        Threshold for doublet score.
     inplace
-        Whether update the AnnData object inplace
-    
+        Perform computation inplace or return result.
+    n_jobs
+        Number of jobs to run in parallel.
+    verbose
+        Whether to print progress messages.
+
     Returns
     -------
-    tuple[np.ndarray, float] | None:
-        if ``inplace = True``, it updates adata with the following fields:
-            - ``adata.obs["is_doublet"]``: boolean mask
-            - ``adata.uns["scrublet"]["threshold"]``: saved threshold
+    np.ndarray | None:
+        If `inplace = True`, directly subsets the data matrix. Otherwise return 
+        a boolean index mask that does filtering, where `True` means that the
+        cell is kept, `False` means the cell is removed.
     """
+    if isinstance(adata, list):
+        result = anndata_par(
+            adata,
+            lambda x: filter_doublets(x, probability_threshold, score_threshold, inplace, n_jobs, verbose),
+            n_jobs=n_jobs,
+        )
+        if inplace:
+            return None
+        else:
+            return result
 
-    if 'scrublet_sim_doublet_score' not in adata.uns:
-        raise NameError("Please call `scrublet` first")
-
-    doublet_scores_sim = adata.uns["scrublet_sim_doublet_score"]
-    doublet_scores_obs = adata.obs["doublet_score"].to_numpy()
+    if probability_threshold is not None and score_threshold is not None:
+        raise ValueError("Only one of `probability_threshold` and `score_threshold` can be set.")
+    if probability_threshold is not None:
+        probs = adata.obs["doublet_probability"].to_numpy()
+        is_doublet = probs > probability_threshold
+    if score_threshold is not None:
+        scores = adata.obs["doublet_score"].to_numpy()
+        is_doublet = scores > score_threshold
 
-    if isinstance(threshold, float):
-        thres = threshold
-    elif threshold == "gmm":
-        thres, _ = get_doublet_probability(
-            doublet_scores_sim, doublet_scores_obs, random_state
-        )
-    elif threshold == "scrublet":
-        from skimage.filters import threshold_minimum
-        thres = threshold_minimum(doublet_scores_sim)
-    else:
-        raise NameError("Invalid value for the `threshold` argument")
+    if verbose: logging.info(f"Detected doublet rate = {np.mean(is_doublet)*100:.3f}%")
 
-    doublets = doublet_scores_obs >= thres
     if inplace:
-        adata.uns["scrublet_threshold"] = thres
-        adata.obs["is_doublet"] = doublets
+        if adata.isbacked:
+            adata.subset(~is_doublet)
+        else:
+            adata._inplace_subset_obs(~is_doublet)
     else:
-        return (doublets, thres)
+        return ~is_doublet
 
 def scrub_doublets_core(
     count_matrix: ss.spmatrix,
     n_neighbors: int,
     sim_doublet_ratio: float,
     expected_doublet_rate: float,
     synthetic_doublet_umi_subsampling: float =1.0,
     n_comps: int = 30,
     use_approx_neighbors: bool = True,
     random_state: int = 0,
+    verbose: bool = False,
 ) -> None:
     """
     Modified scrublet pipeline for single-cell ATAC-seq data.
 
     Automatically sets a threshold for calling doublets, but it's best to check 
     this by running plot_histogram() afterwards and adjusting threshold 
     with call_doublets(threshold=new_threshold) if necessary.
@@ -172,46 +210,49 @@
     doublet_scores_obs_, doublet_errors_obs_,
     doublet_scores_sim_, doublet_errors_sim_,
     predicted_doublets_, z_scores_ 
     threshold_, detected_doublet_rate_,
     detectable_doublet_fraction_, overall_doublet_rate_,
     doublet_parents_, doublet_neighbor_parents_ 
     """
+    import gc
+
     total_counts_obs = count_matrix.sum(1).A.squeeze()
 
-    logging.info('Simulating doublets...')
+    if verbose: logging.info('Simulating doublets...')
     (count_matrix_sim, total_counts_sim, _) = simulate_doublets(
         count_matrix, total_counts_obs, sim_doublet_ratio,
         synthetic_doublet_umi_subsampling, random_state
     )
 
-    logging.info('Spectral embedding ...')
-    (manifold_obs, manifold_sim) = get_manifold(count_matrix, count_matrix_sim, n_comps=n_comps)
+    if verbose: logging.info('Spectral embedding ...')
+    n = count_matrix.shape[0]
+    merged_matrix = ss.vstack([count_matrix, count_matrix_sim])
+    del count_matrix_sim
+    gc.collect()
+    _, evecs = spectral(
+        ad.AnnData(X=merged_matrix, dtype=merged_matrix.dtype),
+        features=None,
+        n_comps=n_comps,
+        inplace=False,
+    )
+    manifold = np.asanyarray(evecs)
+    manifold_obs = manifold[0:n, ]
+    manifold_sim = manifold[n:, ]
 
-    logging.info('Calculating doublet scores...')
-    (doublet_scores_obs, doublet_scores_sim) = calculate_doublet_scores(
+    if verbose: logging.info('Calculating doublet scores...')
+    doublet_scores_obs, doublet_scores_sim = calculate_doublet_scores(
         manifold_obs, manifold_sim, k = n_neighbors,
         exp_doub_rate = expected_doublet_rate,
         use_approx_neighbors = use_approx_neighbors,
         random_state = random_state,
     )
 
     return (doublet_scores_obs, doublet_scores_sim, manifold_obs, manifold_sim)
 
-def get_manifold(obs_norm, sim_norm, n_comps=30, random_state=0):
-    model = Spectral(n_dim=n_comps, distance="jaccard").fit(obs_norm, verbose=0)
-    for c in chunks(obs_norm, 2000):
-        model.extend(c)
-    for c in chunks(sim_norm, 2000):
-        model.extend(c)
-    manifold = np.asanyarray(model.transform()[1])
-    n = obs_norm.shape[0]
-    manifold_obs = manifold[0:n, ]
-    manifold_sim = manifold[n:, ]
-    return (manifold_obs, manifold_sim)
 
 def simulate_doublets(
     count_matrix: ss.spmatrix,
     total_counts: np.ndarray,
     sim_doublet_ratio: int = 2,
     synthetic_doublet_umi_subsampling: float = 1.0,
     random_state: int = 0,
@@ -327,21 +368,21 @@
 
     return (doublet_scores_obs, doublet_scores_sim)
 
 def get_doublet_probability(
     doublet_scores_sim: np.ndarray,
     doublet_scores: np.ndarray,
     random_state: int = 0,
+    verbose: bool = False,
 ):
     from sklearn.mixture import BayesianGaussianMixture
 
     X = doublet_scores_sim.reshape((-1, 1))
     gmm = BayesianGaussianMixture(
         n_components=2, n_init=10, max_iter=1000, random_state=random_state
     ).fit(X)
-    i = np.argmax(gmm.means_)
 
-    probs_sim = gmm.predict_proba(X)[:,i]
-    vals = X[probs_sim > 0.5]
-    threshold = X.max() if vals.size == 0 else vals.min()
+    if verbose:
+        logging.info("GMM means: {}".format(gmm.means_))
 
-    return (threshold, gmm.predict_proba(doublet_scores.reshape((-1, 1)))[:,i])
+    i = np.argmax(gmm.means_)
+    return gmm.predict_proba(doublet_scores.reshape((-1, 1)))[:,i]
```

### Comparing `snapatac2-2.2.0/snapatac2/tools/_call_peaks.py` & `snapatac2-2.3.0/snapatac2/tools/_call_peaks.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.2.0/snapatac2/tools/_clustering.py` & `snapatac2-2.3.0/snapatac2/tools/_clustering.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.2.0/snapatac2/tools/_diff.py` & `snapatac2-2.3.0/snapatac2/tools/_diff.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,35 +13,30 @@
     groupby: str | list[str],
     pvalue: float = 0.01,
 ) -> dict[str, list[str]]:
     """
     A quick-and-dirty way to get marker regions.
     """
     import scipy.stats
-    import polars as pl
 
-    count = pl.DataFrame(aggregate_X(data, groupby, normalize="RPKM"))
-    names = np.array(data.var_names)
-    z = scipy.stats.zscore(
-        np.log2(1 + count.to_numpy()),
-        axis = 1,
-    )
+    count = aggregate_X(data, groupby, normalize="RPKM")
+    z = scipy.stats.zscore(np.log2(1 + count.X), axis = 0)
     peaks = {}
-    for i in range(z.shape[1]):
-        pvals = scipy.stats.norm.sf(z[:, i])
+    for i in range(z.shape[0]):
+        pvals = scipy.stats.norm.sf(z[i, :])
         select = pvals < pvalue
         if np.where(select)[0].size >= 1:
-            peaks[count.columns[i]] = names[select]
+            peaks[count.obs_names[i]] = count.var_names[select]
     return peaks
 
 def diff_test(
     data: AnnData | AnnDataSet,
-    cell_group1: list[int] | list[str] | 'np.ndarray[bool]',
-    cell_group2: list[int] | list[str] | 'np.ndarray[bool]',
-    features : list[str] | list[int] | 'np.ndarray[bool]' | None = None,
+    cell_group1: list[int] | list[str],
+    cell_group2: list[int] | list[str],
+    features : list[str] | list[int] | None = None,
     covariates: list[str] | None = None,
     direction: Literal["positive", "negative", "both"] = "both",
     min_log_fc: float = 0.25,
     min_pct: float = 0.05,
 ) -> 'polars.DataFrame':
     """
     Identify differentially accessible regions.
@@ -75,53 +70,43 @@
     -------
     pl.DataFrame
         A DataFrame with 4 columns: "feature name", "log2(fold_change)",
         "p-value", and "adjusted p-value".
     """
     import polars as pl
 
-    def to_indices(xs, n, type):
-        if isinstance(xs, np.ndarray):
-            if xs.dtype == 'bool':
-                if xs.shape != (n, ):
-                    raise NameError("the length of boolean mask must be the same as the number of cells")
+    def to_indices(xs, type):
+        xs = [_convert_to_bool_if_np_bool(x) for x in xs]
+        if all(isinstance(x, bool) for x in xs):
+            return [i for i, value in enumerate(xs) if value]
+        elif all([isinstance(item, str) for item in xs]):
+            if type == "obs":
+                if data.isbacked:
+                    return data.obs_ix(xs)
                 else:
-                    return np.where(xs)[0].tolist()
+                    return [data.obs_names.get_loc(x) for x in xs]
             else:
-                xs = xs.tolist()
-
-        if isinstance(xs, list):
-            if all([isinstance(item, int) for item in xs]):
-                return xs
-            elif all([isinstance(item, str) for item in xs]):
-                if type == "obs":
-                    if data.isbacked:
-                        return data.obs_ix(xs)
-                    else:
-                        return [data.obs_names.get_loc(x) for x in xs]
+                if data.isbacked:
+                    return data.var_ix(xs)
                 else:
-                    if data.isbacked:
-                        return data.var_ix(xs)
-                    else:
-                        return [data.var_names.get_loc(x) for x in xs]
-            else:
-                raise NameError("invalid type")
+                    return [data.var_names.get_loc(x) for x in xs]
         else:
-            raise NameError("invalid type")
-    cell_group1 = to_indices(cell_group1, data.n_obs, "obs")
+            return xs
+
+    cell_group1 = to_indices(cell_group1, "obs")
     n_group1 = len(cell_group1)
-    cell_group2 = to_indices(cell_group2, data.n_obs, "obs")
+    cell_group2 = to_indices(cell_group2, "obs")
     n_group2 = len(cell_group2)
 
     cell_by_peak = data.X[cell_group1 + cell_group2, :].tocsc()
     test_var = np.array([0] * n_group1 + [1] * n_group2)
     if covariates is not None:
         raise NameError("covariates is not implemented")
 
-    features = range(data.n_vars) if features is None else to_indices(features, data.n_vars, "var")
+    features = range(data.n_vars) if features is None else to_indices(features, "var")
     logging.info("Input contains {} features, now perform filtering with 'min_log_fc = {}' and 'min_pct = {}' ...".format(len(features), min_log_fc, min_pct))
     filtered = _filter_features(
         cell_by_peak[:n_group1, :],
         cell_by_peak[n_group1:, :],
         features,
         direction,
         min_pct,
@@ -259,20 +244,25 @@
     Returns
     -------
     The P-value.
     """
     from sklearn.linear_model import LogisticRegression
     from sklearn.metrics import log_loss
 
-    model = LogisticRegression(penalty="none", random_state=0, n_jobs=1,
+    model = LogisticRegression(penalty=None, random_state=0, n_jobs=1,
         solver="lbfgs", multi_class='ovr', warm_start=False,
         max_iter = 1000,
         ).fit(X0, y)
     reduced = -log_loss(y, model.predict_proba(X0), normalize=False)
 
-    model = LogisticRegression(penalty="none", random_state=0, n_jobs=1,
+    model = LogisticRegression(penalty=None, random_state=0, n_jobs=1,
         solver="lbfgs", multi_class='ovr', warm_start=False,
         max_iter = 1000,
         ).fit(X1, y)
     full = -log_loss(y, model.predict_proba(X1), normalize=False)
     chi = -2 * (reduced - full)
-    return chi2.sf(chi, X1.shape[1] - X0.shape[1])
+    return chi2.sf(chi, X1.shape[1] - X0.shape[1])
+
+def _convert_to_bool_if_np_bool(value):
+    if isinstance(value, np.bool_):
+        return bool(value)
+    return value
```

### Comparing `snapatac2-2.2.0/snapatac2/tools/_integration.py` & `snapatac2-2.3.0/snapatac2/tools/_integration.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.2.0/snapatac2/tools/_misc.py` & `snapatac2-2.3.0/snapatac2/tools/_misc.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.2.0/snapatac2/tools/_motif.py` & `snapatac2-2.3.0/snapatac2/tools/_motif.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 from typing_extensions import Literal
 
+import numpy as np
 from pathlib import Path
 import logging
 
 from snapatac2._snapatac2 import PyDNAMotif
 from snapatac2._utils import fetch_seq
 from snapatac2.genome import Genome
 from snapatac2.tools._diff import _p_adjust_bh
@@ -60,15 +61,17 @@
     region_to_idx = dict(map(lambda x: (x[1], x[0]), enumerate(all_regions)))
 
     logging.info("Fetching {} sequences ...".format(len(all_regions)))
     genome = genome_fasta.fetch_fasta() if isinstance(genome_fasta, Genome) else str(genome_fasta)
     genome = Fasta(genome, one_based_attributes=False)
     sequences = [fetch_seq(genome, region) for region in all_regions]
 
+    motif_id = []
     motif_name = []
+    motif_family = []
     group_name = []
     fold_change = []
     n_fg = []
     N_fg = []
     n_bg = []
     N_bg = []
     logging.info("Computing enrichment ...")
@@ -84,38 +87,42 @@
         for key, val in regions.items():
             total_fg = len(val)
             bound_fg = count_occurrence(val, region_to_idx, bound)
 
             if bound_fg == 0:
                 log_fc = 0 if bound_bg == 0 else float('-inf')
             else:
-                log_fc = log2((bound_fg / total_fg) / (bound_bg / total_bg))
+                log_fc = log2((bound_fg / total_fg) / (bound_bg / total_bg)) if bound_bg > 0 else float('inf')
 
-            motif_name.append(motif.id)
+            motif_id.append(motif.id)
+            motif_name.append(motif.name)
+            motif_family.append(motif.family)
             group_name.append(key)
             fold_change.append(log_fc)
             n_fg.append(bound_fg)
             N_fg.append(total_fg)
             n_bg.append(bound_bg)
             N_bg.append(total_bg)
           
-    if method == "bionomial":
+    if method == "binomial":
         pval = binom.cdf(n_fg, N_fg, np.array(n_bg) / np.array(N_bg))
     elif method == "hypergeometric":
         pval = hypergeom.cdf(n_fg, N_bg, n_bg, N_fg)
     else:
         raise NameError("'method' needs to be 'binomial' or 'hypergeometric'")
 
     result = dict(
-        (key, {'motif name': [], 'log2(fold change)': [], 'p-value': []}) for key in regions.keys()
+        (key, {'id': [], 'name': [], 'family': [], 'log2(fold change)': [], 'p-value': []}) for key in regions.keys()
     )
     for i, key in enumerate(group_name):
         log_fc = fold_change[i]
         p = (1 - pval[i]) if log_fc >= 0 else pval[i]
-        result[key]['motif name'].append(motif_name[i])
+        result[key]['id'].append(motif_id[i])
+        result[key]['name'].append(motif_name[i])
+        result[key]['family'].append(motif_family[i])
         result[key]['log2(fold change)'].append(log_fc)
         result[key]['p-value'].append(float(p))
 
     for key in result.keys():
         result[key]['adjusted p-value'] = _p_adjust_bh(result[key]['p-value'])
         result[key] = pl.DataFrame(result[key])
     return result
```

### Comparing `snapatac2-2.2.0/snapatac2/tools/_network.py` & `snapatac2-2.3.0/snapatac2/tools/_network.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from snapatac2._utils import fetch_seq
 from snapatac2._snapatac2 import (
     AnnData, AnnDataSet, link_region_to_gene, PyDNAMotif, spearman
 )
 
 __all__ = ['NodeData', 'LinkData',
            'init_network_from_annotation', 'add_cor_scores', 'add_regr_scores',
-           'add_tf_binding', 'link_tf_to_gene', 'prune_network']
+           'add_tf_binding', 'link_tf_to_gene', 'prune_network', 'pagerank']
 
 class NodeData:
     def __init__(self, id: str = "", type: str = "") -> None:
         self.id = id
         self.type = type
         self.regr_fitness = None
 
@@ -85,28 +85,28 @@
         str(anno_file),
         upstream,
         downstream,
         id_type,
         coding_gene_only,
     )
     for (id, type), regions in links.items():
-        to = graph.add_node(NodeData(id, type))
+        to = graph.add_node(NodeData(id.upper(), type))
         for i, t, distance in regions:
             key = (i, t)
             if key in region_added:
                 graph.add_edge(region_added[key], to, LinkData(distance))
             else:
                 region_added[key] = graph.add_parent(to, NodeData(i, t), LinkData(distance))
     return graph
 
 def add_cor_scores(
     network: rx.PyDiGraph,
     *,
-    gene_mat: AnnData | AnnDataSet,
-    peak_mat: AnnData | AnnDataSet,
+    gene_mat: AnnData | AnnDataSet | None = None,
+    peak_mat: AnnData | AnnDataSet | None = None,
     select: list[str] | None = None,
     overwrite: bool = False,
 ):
     """
     Compute correlation scores for any two connected nodes in the network.
 
     This function can be used to compute correlation scores for any type of
@@ -150,16 +150,16 @@
             scores = np.ravel(spearman(X.T, y.reshape((1, -1))))
             for nd, sc in zip(nd_X, scores):
                 setattr(network.get_edge_data(nd, nd_y), key, sc)
 
 def add_regr_scores(
     network: rx.PyDiGraph,
     *,
-    peak_mat: AnnData | AnnDataSet,
-    gene_mat: AnnData | AnnDataSet,
+    peak_mat: AnnData | AnnDataSet | None = None,
+    gene_mat: AnnData | AnnDataSet | None = None,
     select: list[str] | None = None,
     method: Literal["gb_tree", "elastic_net"] = "elastic_net",
     scale_X: bool = False,
     scale_Y: bool = False,
     alpha: float = 1.0,
     l1_ratio: float = 0.5,
     use_gpu: bool = False,
@@ -197,16 +197,17 @@
         Whether to use gpu
     overwrite
         Whether to overwrite existing records.
     """
     from tqdm import tqdm
 
     key = "regr_score"
-    if list(peak_mat.obs_names) != list(gene_mat.obs_names):
-        raise NameError("gene matrix and peak matrix should have the same obs_names")
+    if peak_mat is not None and gene_mat is not None:
+        if list(peak_mat.obs_names) != list(gene_mat.obs_names):
+            raise NameError("gene matrix and peak matrix should have the same obs_names")
     if select is not None:
         select = set(select)
     without_overwrite = None if overwrite else key 
     tree_method = "gpu_hist" if use_gpu else "hist"
     
     if network.num_edges() == 0:
         return network
@@ -223,44 +224,48 @@
             raise NameError("Unknown method")
         network[nd_y].regr_fitness = fitness
         for nd, sc in zip(nd_X, scores):
             setattr(network.get_edge_data(nd, nd_y), key, sc)
 
 def add_tf_binding(
     network: rx.PyDiGraph,
+    *,
     motifs: list[PyDNAMotif],
     genome_fasta: Path | Genome,
+    pvalue: float = 1e-5,
 ):
     """Add TF motif binding information.
 
     Parameters
     ----------
     network
         Network
     motifs
         TF motifs
     genome_fasta
         A fasta file containing the genome sequences or a Genome object.
+    pvalue
+        P-value threshold for motif binding.
     """
     from pyfaidx import Fasta
     from tqdm import tqdm
     import itertools
 
     regions = [(i, network[i].id) for i in network.node_indices() if network[i].type == "region"]
     logging.info("Fetching {} sequences ...".format(len(regions)))
     genome = genome_fasta.fetch_fasta() if isinstance(genome_fasta, Genome) else str(genome_fasta)
     genome = Fasta(genome, one_based_attributes=False)
     sequences = [fetch_seq(genome, region) for _, region in regions]
 
     logging.info("Searching for the binding sites of {} motifs ...".format(len(motifs)))
     for motif in tqdm(motifs):
-        bound = motif.with_nucl_prob().exists(sequences)
+        bound = motif.with_nucl_prob().exists(sequences, pvalue=pvalue)
         if any(bound):
             name = motif.id if motif.name is None else motif.name
-            nid = network.add_node(NodeData(name, "motif"))
+            nid = network.add_node(NodeData(name.upper(), "motif"))
             network.add_edges_from(
                 [(nid, i, LinkData()) for i, _ in itertools.compress(regions, bound)]
             )
 
 def link_tf_to_gene(network: rx.PyDiGraph) -> rx.PyDiGraph:
     """Contruct a genetic network by linking TFs to target genes.
     
@@ -370,33 +375,63 @@
                 remove.append(nid)
         if len(remove) > 0:
             graph.remove_nodes_from(remove)
             logging.info("Removed {} isolated nodes.".format(len(remove)))
 
     return graph
 
-def pagerank(network):
+def pagerank(
+    network,
+    node_weights: str | list[float] | None = None,
+    edge_weights: str | list[float] | None = None,
+) -> list[tuple[str, float]]:
     tfs = {network[nid].id for nid in network.node_indices() if network.out_degree(nid) > 0}
-    g = _to_igraph(network, reverse_edge=True)
-    return [(i['name'], s) for i, s in zip(g.vs, g.pagerank(weights='regr_score')) if i['name'] in tfs]
+    g = _to_igraph(network, node_weights, edge_weights, True)
+    pagerank_scores = g.personalized_pagerank(
+        reset=None if node_weights is None else 'weight',
+        weights=None if edge_weights is None else 'weight',
+    )
+    return [(i['name'], s) for i, s in zip(g.vs, pagerank_scores) if i['name'] in tfs]
 
-def _to_igraph(graph, edge_weight="regr_score", reverse_edge=False):
+def _to_igraph(
+    graph,
+    node_weights: str | list[float] | None = None,
+    edge_weights: str | list[float] | None = None,
+    reverse_edge: bool = False,
+):
     import igraph as ig
     g = ig.Graph()
-    g.add_vertices([x.id for x in graph.nodes()])
+
+    nodes = [x.id for x in graph.nodes()]
+    node_attributes = None
+    if node_weights is not None:
+        if isinstance(node_weights, str):
+            node_attributes = {"weight": [getattr(x, node_weights) for x in graph.nodes()]}
+        else:
+            node_attributes = {"weight": node_weights}
+    g.add_vertices(nodes, attributes=node_attributes)
     
     edges = []
-    regr_score = []
+    if edge_weights is not None and isinstance(edge_weights, list):
+        weights = edge_weights
+    else:
+        weights = []
     for fr, to, edge in graph.edge_index_map().values():
         if reverse_edge:
             edges.append((graph[to].id, graph[fr].id))
         else:
             edges.append((graph[fr].id, graph[to].id))
-        regr_score.append(edge.regr_score)
-    g.add_edges(edges, attributes={"regr_score": regr_score})
+        if edge_weights is not None and isinstance(edge_weights, str):
+            weights.append(getattr(edge, edge_weights))
+    if len(weights) > 0:
+        edge_attributes = {"weight": weights}
+    else:
+        edge_attributes = None
+    g.add_edges(edges, attributes=edge_attributes)
+
     return g
 
 def _network_stats(network: rx.PyDiGraph):
     from collections import defaultdict
 
     nNodes = network.num_nodes()
     nEdges = network.num_edges()
@@ -457,70 +492,64 @@
         X = self.mat_X[:, [self.idx_map_X[nd] for nd in nd_X]]
 
         self.index += 1
         return (nd_X, X), (nd_y, y)
 
 def _get_data_iter(
     network: rx.PyDiGraph,
-    peak_mat: AnnData | AnnDataSet,
-    gene_mat: AnnData | AnnDataSet,
+    peak_mat: AnnData | AnnDataSet | None,
+    gene_mat: AnnData | AnnDataSet | None,
     select: set[str] | None = None,
     without_overwrite: str | None = None,
     scale_X: bool = False,
     scale_Y: bool = False,
 ) -> _DataPairIter:
     """
     """
     from scipy.stats import zscore
 
     def get_mat(nids, node_getter, gene_mat, peak_mat):
         genes = []
         peaks = []
+        mats = []
 
         for x in nids:
             nd = node_getter(x) 
             if nd.type == "gene" or nd.type == "motif":
                 genes.append(x)
             elif nd.type == "region":
                 peaks.append(x)
             else:
                 raise NameError("unknown type: {}".format(nd.type))
 
-        if len(genes) == gene_mat.n_vars:
-            g_mat = gene_mat.X[:]
-        else:
-            if gene_mat.isbacked:
-                ix = gene_mat.var_ix([node_getter(x).id for x in genes])
+        if len(genes) != 0:
+            if len(genes) == gene_mat.n_vars:
+                mats.append(gene_mat.X[:])
             else:
-                ix = [gene_mat.var_names.get_loc(node_getter(x).id) for x in genes]
-            g_mat = gene_mat.X[:, ix]
-
-        if len(peaks) == peak_mat.n_vars:
-            p_mat = peak_mat.X[:]
-        else:
-            if peak_mat.isbacked:
-                ix = peak_mat.var_ix([node_getter(x).id for x in peaks])
+                idx_map = {x.upper(): i for i, x in enumerate(gene_mat.var_names)}
+                ix = [idx_map[node_getter(x).id] for x in genes]
+                mats.append(gene_mat.X[:, ix])
+
+        if len(peaks) != 0:
+            if len(peaks) == peak_mat.n_vars:
+                mats.append(peak_mat.X[:])
             else:
-                ix = [peak_mat.var_names.get_loc(node_getter(x).id) for x in peaks]
-            p_mat = peak_mat.X[:, ix]
-
-        if len(genes) == 0:
-            mats = [p_mat]
-        elif len(peaks) == 0:
-            mats = [g_mat]
-        else:
-            mats = [g_mat, p_mat]
+                if peak_mat.isbacked:
+                    ix = peak_mat.var_ix([node_getter(x).id for x in peaks])
+                else:
+                    ix = [peak_mat.var_names.get_loc(node_getter(x).id) for x in peaks]
+                mats.append(peak_mat.X[:, ix])
         
         if all([sp.issparse(x) for x in mats]):
             mat = sp.hstack(mats, format="csc")
         else:
             mat = np.hstack(mats)
         return (genes + peaks, mat)
 
-    all_genes = set(gene_mat.var_names)
+    all_genes = set([x.upper() for x in gene_mat.var_names])
     select = all_genes if select is None else select
     id_XY = []
 
     for nid in network.node_indices():
         if network[nid].type == "region" or network[nid].id in select:
             parents = [pid for pid, _, edge_data in network.in_edges(nid)
                        if (without_overwrite is None or
```

### Comparing `snapatac2-2.2.0/snapatac2/tools/_smooth.py` & `snapatac2-2.3.0/snapatac2/tools/_smooth.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.2.0/snapatac2.egg-info/SOURCES.txt` & `snapatac2-2.3.0/snapatac2.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -26,23 +26,26 @@
 snapatac2/preprocessing/_knn.py
 snapatac2/preprocessing/_mnn_correct.py
 snapatac2/preprocessing/_scrublet.py
 snapatac2/tools/__init__.py
 snapatac2/tools/_call_peaks.py
 snapatac2/tools/_clustering.py
 snapatac2/tools/_diff.py
+snapatac2/tools/_embedding.py
 snapatac2/tools/_integration.py
 snapatac2/tools/_misc.py
 snapatac2/tools/_motif.py
 snapatac2/tools/_network.py
 snapatac2/tools/_smooth.py
-snapatac2/tools/embedding/__init__.py
-snapatac2/tools/embedding/_laplacian.py
-snapatac2/tools/embedding/_spectral.py
-snapatac2/tools/embedding/_umap.py
 src/call_peaks.rs
+src/embedding.rs
 src/export.rs
 src/lib.rs
 src/motif.rs
 src/network.rs
 src/preprocessing.rs
-src/utils.rs
+src/utils.rs
+src/utils/anndata.rs
+tests/test_func.py
+tests/test_pipeline.py
+tests/test_similarity.py
+tests/test_tools.py
```

### Comparing `snapatac2-2.2.0/src/call_peaks.rs` & `snapatac2-2.3.0/src/call_peaks.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,43 @@
-use crate::utils::{AnnDataObj, extract_anndata};
+use crate::utils::AnnDataLike;
 use snapatac2_core::{export::Exporter, utils::merge_peaks};
 
-use pyanndata::utils::conversion::RustToPy;
-use pyo3::{prelude::*, Python};
+use std::ops::Deref;
+use anndata::Backend;
+use anndata_hdf5::H5;
+use pyanndata::data::PyDataFrame;
+use pyo3::prelude::*;
 use bed_utils::bed::{BEDLike, GenomicRange, io::Reader, tree::BedTree};
 use flate2::read::MultiGzDecoder;
 use tempfile::Builder;
 use log::info;
 use std::fs::File;
 use polars::{prelude::{DataFrame, NamedFrom}, series::Series};
 use std::collections::HashSet;
 use anyhow::Result;
 
 #[pyfunction]
-pub fn call_peaks<'py>(
-    py: Python<'py>,
-    anndata: &PyAny,
+pub fn call_peaks(
+    anndata: AnnDataLike,
     group_by: Vec<&str>,
     selections: Option<HashSet<&str>>,
     q_value: f64,
     out_dir: Option<&str>,
-) -> Result<PyObject> {
+) -> Result<PyDataFrame> {
     let dir = Builder::new().tempdir_in("./").unwrap();
     let temp_dir = out_dir.unwrap_or(dir.path().to_str().unwrap());
 
-    let peak_files = match extract_anndata(py, anndata)? {
-        AnnDataObj::AnnData(data) => data.inner().call_peaks(
-            q_value, &group_by, selections, temp_dir, "", ".NarrowPeak.gz",
-        )?,
-        AnnDataObj::AnnDataSet(data) => data.inner().call_peaks(
-            q_value, &group_by, selections, temp_dir, "", ".NarrowPeak.gz",
-        )?,
-        AnnDataObj::PyAnnData(data) => data.call_peaks(
-            q_value, &group_by, selections, temp_dir, "", ".NarrowPeak.gz",
-        )?,
-    };
-
+    macro_rules! run {
+        ($data:expr) => {
+            $data.call_peaks(
+                q_value, &group_by, selections, temp_dir, "", ".NarrowPeak.gz",
+            )?
+        }
+    }
+    let peak_files = crate::with_anndata!(&anndata, run);
     let peak_iter = peak_files.values().flat_map(|fl|
         Reader::new(MultiGzDecoder::new(File::open(fl).unwrap()), None)
         .into_records().map(Result::unwrap)
     );
 
     info!("Merging peaks...");
     let peaks: Vec<_> = merge_peaks(peak_iter, 250).flatten().collect();
@@ -56,9 +54,9 @@
             peaks_index.find(&bed).for_each(|(_, i)| values[*i] = true);
         });
         Series::new(key.as_str(), values)
     });
 
     let df = DataFrame::new(std::iter::once(peaks_str).chain(iter).collect())?;
     dir.close()?;
-    Ok(df.rust_into_py(py)?)
+    Ok(df.into())
 }
```

### Comparing `snapatac2-2.2.0/src/export.rs` & `snapatac2-2.3.0/src/export.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,47 @@
-use crate::utils::{AnnDataObj, extract_anndata};
+use crate::utils::AnnDataLike;
 use snapatac2_core::export::Exporter;
 
-use pyo3::{prelude::*, Python};
+use std::ops::Deref;
+use anndata::Backend;
+use anndata_hdf5::H5;
+use pyo3::prelude::*;
 use std::{collections::{HashSet, HashMap}, path::PathBuf};
 use anyhow::Result;
 
 #[pyfunction]
-pub fn export_bed<'py>(
-    py: Python<'py>,
-    anndata: &PyAny,
+pub fn export_bed(
+    anndata: AnnDataLike,
     barcodes: Vec<&str>,
     group_by: Vec<&str>,
     selections: Option<HashSet<&str>>,
     dir: PathBuf,
     prefix: &str,
     suffix: &str,
 ) -> Result<HashMap<String, PathBuf>> {
-    match extract_anndata(py, anndata)? {
-        AnnDataObj::AnnData(data) => data.inner().export_bed(
-            Some(&barcodes), &group_by, selections, dir, prefix, suffix,
-        ),
-        AnnDataObj::AnnDataSet(data) => data.inner().export_bed(
-            Some(&barcodes), &group_by, selections, dir, prefix, suffix,
-        ),
-        AnnDataObj::PyAnnData(data) => data.export_bed(
-            Some(&barcodes), &group_by, selections, dir, prefix, suffix,
-        ),
+    macro_rules! run {
+        ($data:expr) => {
+            $data.export_bed(
+                Some(&barcodes), &group_by, selections, dir, prefix, suffix,
+            )
+        }
     }
+    crate::with_anndata!(&anndata, run)
 }
 
 #[pyfunction]
-pub fn export_bigwig<'py>(
-    py: Python<'py>,
-    anndata: &PyAny,
+pub fn export_bigwig(
+    anndata: AnnDataLike,
     group_by: Vec<&str>,
     selections: Option<HashSet<&str>>,
     resolution: usize,
     dir: PathBuf,
     prefix: &str,
     suffix: &str,
 ) -> Result<HashMap<String, PathBuf>> {
-    match extract_anndata(py, anndata)? {
-        AnnDataObj::AnnData(data) => data.inner()
-            .export_bigwig(&group_by, selections, resolution, dir, prefix, suffix),
-        AnnDataObj::AnnDataSet(data) => data.inner()
-            .export_bigwig(&group_by, selections, resolution, dir, prefix, suffix),
-        AnnDataObj::PyAnnData(data) => data
-            .export_bigwig(&group_by, selections, resolution, dir, prefix, suffix),
+    macro_rules! run {
+        ($data:expr) => {
+            $data.export_bigwig(&group_by, selections, resolution, dir, prefix, suffix)
+        }
     }
+    crate::with_anndata!(&anndata, run)
 }
```

### Comparing `snapatac2-2.2.0/src/lib.rs` & `snapatac2-2.3.0/src/lib.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 mod export;
 mod utils;
 mod call_peaks;
 mod preprocessing;
+mod embedding;
 mod network;
 mod motif;
 
 use pyo3::{prelude::*, PyResult, Python};
 use pyanndata;
 
 #[cfg(not(target_env = "msvc"))]
@@ -15,31 +16,35 @@
 #[global_allocator]
 static GLOBAL: Jemalloc = Jemalloc;
 
 #[pymodule]
 fn _snapatac2(_py: Python, m: &PyModule) -> PyResult<()> {
     pyo3_log::init();
 
+    // AnnData related functions
     m.add_class::<pyanndata::AnnData>().unwrap();
     m.add_class::<pyanndata::AnnDataSet>().unwrap();
-    m.add_class::<pyanndata::PyMatrixElem>().unwrap();
+    m.add_class::<pyanndata::PyArrayElem>().unwrap();
     m.add_function(wrap_pyfunction!(pyanndata::read, m)?)?;
     m.add_function(wrap_pyfunction!(pyanndata::read_mtx, m)?)?;
-    m.add_function(wrap_pyfunction!(pyanndata::read_csv, m)?)?;
+    //m.add_function(wrap_pyfunction!(pyanndata::read_csv, m)?)?;
     m.add_function(wrap_pyfunction!(pyanndata::read_dataset, m)?)?;
 
+    // Motif analysis related functions
     m.add_class::<motif::PyDNAMotif>().unwrap();
     m.add_class::<motif::PyDNAMotifScanner>().unwrap();
     m.add_class::<motif::PyDNAMotifTest>().unwrap();
     m.add_function(wrap_pyfunction!(motif::read_motifs, m)?)?;
  
+    // Preprocessing related functions
     m.add_class::<preprocessing::PyFlagStat>().unwrap();
     m.add_function(wrap_pyfunction!(preprocessing::make_fragment_file, m)?)?;
     m.add_function(wrap_pyfunction!(preprocessing::import_fragments, m)?)?;
     m.add_function(wrap_pyfunction!(preprocessing::mk_tile_matrix, m)?)?;
+    m.add_function(wrap_pyfunction!(preprocessing::mk_tile_matrix_par, m)?)?;
     m.add_function(wrap_pyfunction!(preprocessing::mk_gene_matrix, m)?)?;
     m.add_function(wrap_pyfunction!(preprocessing::mk_peak_matrix, m)?)?;
 
     m.add_function(wrap_pyfunction!(export::export_bed, m)?)?;
     m.add_function(wrap_pyfunction!(export::export_bigwig, m)?)?;
     m.add_function(wrap_pyfunction!(call_peaks::call_peaks, m)?)?;
 
@@ -50,10 +55,13 @@
     m.add_function(wrap_pyfunction!(utils::pearson, m)?)?;
     m.add_function(wrap_pyfunction!(utils::spearman, m)?)?;
     m.add_function(wrap_pyfunction!(utils::simple_lin_reg, m)?)?;
     m.add_function(wrap_pyfunction!(utils::jm_regress, m)?)?;
     m.add_function(wrap_pyfunction!(utils::intersect_bed, m)?)?;
     m.add_function(wrap_pyfunction!(utils::kmeans, m)?)?;
     m.add_function(wrap_pyfunction!(utils::approximate_nearest_neighbors, m)?)?;
+    m.add_function(wrap_pyfunction!(embedding::spectral_embedding, m)?)?;
+    m.add_function(wrap_pyfunction!(embedding::multi_spectral_embedding, m)?)?;
+    m.add_function(wrap_pyfunction!(embedding::spectral_embedding_nystrom, m)?)?;
 
     Ok(())
-}
+}
```

### Comparing `snapatac2-2.2.0/src/motif.rs` & `snapatac2-2.3.0/src/motif.rs`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         id: &str,
         matrix: &'py PyAny,
     ) -> Self {
         let pwm: PyReadonlyArray<f64, Ix2> = matrix.extract().unwrap();
         let motif = motif::DNAMotif {
             id: id.to_string(),
             name: None,
+            family: None,
             probability: pwm.as_array().rows().into_iter()
                 .map(|row| row.into_iter().map(|x| *x).collect::<Vec<_>>().try_into().unwrap()).collect(),
         };
         PyDNAMotif(motif)
     }
 
     #[getter]
@@ -44,22 +45,26 @@
 
     #[setter]
     fn set_name(&mut self, value: String) -> PyResult<()> {
         self.0.name = Some(value);
         Ok(())
     }
 
+    #[getter]
+    fn family(&self) -> Option<String> { self.0.family.clone() }
+
+    #[setter]
+    fn set_family(&mut self, value: String) -> PyResult<()> {
+        self.0.family = Some(value);
+        Ok(())
+    }
+
     fn info_content(&self) -> f64 { self.0.info_content() }
 
-    #[args(
-        a = "0.25",
-        c = "0.25",
-        g = "0.25",
-        t = "0.25",
-    )]
+    #[pyo3(signature = (a=0.25, c=0.25, g=0.25, t=0.25))]
     fn with_nucl_prob(&self, a: f64, c: f64, g: f64, t: f64) -> PyDNAMotifScanner {
         PyDNAMotifScanner(self.0.clone().to_scanner(motif::BackgroundProb([a, c, g, t])))
     }
 }
 
 #[pyclass]
 #[repr(transparent)]
@@ -70,45 +75,31 @@
 impl PyDNAMotifScanner {
     #[getter]
     fn id(&self) -> String { self.0.motif.id.clone() }
 
     #[getter]
     fn name(&self) -> Option<String> { self.0.motif.name.clone() }
 
-    #[args(
-        seq,
-        pvalue = "1e-5",
-    )]
+    #[pyo3(signature = (seq, pvalue=1e-5))]
     fn find(&self, seq: &str, pvalue: f64) -> Vec<(usize, f64)> {
         self.0.find(seq.as_bytes(), pvalue).collect()
     }
 
-    #[args(
-        seq,
-        pvalue = "1e-5",
-        rc = "true",
-    )]
+    #[pyo3(signature = (seq, pvalue=1e-5, rc=true))]
     fn exist(&self, seq: &str, pvalue: f64, rc: bool) -> bool {
         self.0.find(seq.as_bytes(), pvalue).next().is_some() ||
             (rc && self.0.find(rev_compl(seq).as_bytes(), pvalue).next().is_some())
     }
 
-    #[args(
-        seqs,
-        pvalue = "1e-5",
-        rc = "true",
-    )]
+    #[pyo3(signature = (seqs, pvalue=1e-5, rc=true))]
     fn exists(&self, seqs: Vec<&str>, pvalue: f64, rc: bool) -> Vec<bool> {
         seqs.into_par_iter().map(|x| self.exist(x, pvalue, rc)).collect()
     }
 
-    #[args(
-        seqs,
-        pvalue = "1e-5",
-    )]
+    #[pyo3(signature = (seqs, pvalue=1e-5))]
     fn with_background(&self, seqs: Vec<&str>, pvalue: f64) -> PyDNAMotifTest {
         let n = seqs.len();
         PyDNAMotifTest {
             scanner: self.clone(),
             pvalue,
             occurrence_background: seqs.into_par_iter().filter(|x| self.exist(x, pvalue, true)).count(),
             total_background: n,
```

### Comparing `snapatac2-2.2.0/src/network.rs` & `snapatac2-2.3.0/src/network.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-use crate::utils::open_file;
+use crate::utils::read_transcripts;
 
 use pyo3::prelude::*;
 
 use snapatac2_core::{
     network::link_region_to_promoter,
-    preprocessing::{Promoters, read_transcripts},
+    preprocessing::Promoters,
 };
 use bed_utils::bed::GenomicRange;
 use std::{
     str::FromStr,
     collections::HashMap,
-    io::BufReader,
 };
 
 #[pyfunction]
 pub(crate) fn link_region_to_gene(
     regions: Vec<String>,
     annot_fl: &str,
     upstream: u64,
     downstream: u64,
     id_type: &str,
     coding_gene_only: bool,
 ) -> HashMap<(String, String), Vec<(String, String, u64)>>
 {
     let promoters = Promoters::new(
-        read_transcripts(BufReader::new(open_file(annot_fl))).into_iter()
+        read_transcripts(annot_fl).into_iter()
             .filter(|x| if coding_gene_only { x.is_coding.unwrap_or(true) } else { true })
             .collect(),
         upstream,
         downstream,
         false,
     );
     let regions_: Vec<GenomicRange> = regions.into_iter().map(|x| GenomicRange::from_str(&x).unwrap()).collect();
```

### Comparing `snapatac2-2.2.0/src/preprocessing.rs` & `snapatac2-2.3.0/src/preprocessing.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 use crate::utils::*;
 
+use anndata::Backend;
+use anndata_hdf5::H5;
+use rayon::prelude::{IntoParallelIterator, ParallelIterator};
 use std::path::PathBuf;
-use std::{io::BufReader, str::FromStr, collections::BTreeMap, ops::Deref, collections::HashSet};
-use pyo3::{prelude::*, Python};
+use std::{str::FromStr, collections::BTreeMap, ops::Deref, collections::HashSet};
+use pyo3::prelude::*;
 use bed_utils::{bed, bed::GenomicRange};
-use bed_utils::bed::tree::GenomeRegions;
-use anndata_rs::{anndata, AnnDataOp, AnnDataIterator};
-use pyanndata::{AnnData, PyAnnData};
+use pyanndata::PyAnnData;
 use anyhow::Result;
 
 use snapatac2_core::{
-    preprocessing::{
-        Transcript, Fragment, FlagStat, ReadGenomeCoverage, create_gene_matrix,
-        create_peak_matrix, create_tile_matrix, read_transcripts,
-    },
+    preprocessing::{Fragment, FlagStat},
     preprocessing,
 };
 
 #[pyclass]
 pub(crate) struct PyFlagStat(FlagStat);
 
 #[pymethods]
@@ -33,22 +31,22 @@
 }
 
 #[pyfunction]
 pub(crate) fn make_fragment_file(
     bam_file: PathBuf,
     output_file: PathBuf,
     is_paired: bool,
+    shift_left: i64,
+    shift_right: i64,
+    chunk_size: usize,
     barcode_tag: Option<&str>,
     barcode_regex: Option<&str>,
     umi_tag: Option<&str>,
     umi_regex: Option<&str>,
-    shift_left: i64,
-    shift_right: i64,
     mapq: Option<u8>,
-    chunk_size: usize,
 ) -> PyFlagStat
 {
     fn parse_tag(tag: &str) -> [u8; 2] {
         let tag_b = tag.as_bytes();
         if tag_b.len() == 2 {
             [tag_b[0], tag_b[1]]
         } else {
@@ -61,28 +59,29 @@
         umi_tag.map(|x| parse_tag(x)), umi_regex,
         shift_left, shift_right, mapq, chunk_size,
     );
     PyFlagStat(stat)
 }
 
 #[pyfunction]
-pub(crate) fn import_fragments<'py>(
-    py: Python<'py>,
-    output_file: Option<PathBuf>,
+pub(crate) fn import_fragments(
+    anndata: AnnDataLike,
     fragment_file: PathBuf,
     gtf_file: PathBuf,
     chrom_size: BTreeMap<&str, u64>,
     min_num_fragment: u64,
     min_tsse: f64,
     fragment_is_sorted_by_name: bool,
     low_memory: bool,
-    white_list: Option<HashSet<String>>,
+    shift_left: i64,
+    shift_right: i64,
     chunk_size: usize,
+    white_list: Option<HashSet<String>>,
     tempdir: Option<PathBuf>,
-) -> Result<PyObject>
+) -> Result<()>
 {
     let promoters = preprocessing::make_promoter_map(preprocessing::read_tss(open_file(gtf_file)));
     let final_white_list = if fragment_is_sorted_by_name || low_memory || min_num_fragment <= 0 {
         white_list
     } else {
         let mut barcode_count = preprocessing::get_barcode_count(
             bed::io::Reader::new(
@@ -93,135 +92,170 @@
         let list: HashSet<String> = barcode_count.drain().filter_map(|(k, v)|
             if v >= min_num_fragment { Some(k) } else { None }).collect();
         match white_list {
             None => Some(list),
             Some(x) => Some(list.intersection(&x).map(Clone::clone).collect()),
         }
     };
-    let is_sorted = if !fragment_is_sorted_by_name && low_memory { true } else { false };
     let chrom_sizes = chrom_size.into_iter().map(|(chr, s)| GenomicRange::new(chr, 0, s)).collect();
     let fragments = bed::io::Reader::new(open_file(&fragment_file), Some("#".to_string()))
-        .into_records::<Fragment>().map(Result::unwrap);
+        .into_records::<Fragment>().map(|x| {
+            let mut f = x.unwrap();
+            shift_fragment(&mut f, shift_left, shift_right);
+            f
+    });
     let sorted_fragments: Box<dyn Iterator<Item = Fragment>> = if !fragment_is_sorted_by_name && low_memory {
         Box::new(bed::sort_bed_by_key(fragments, |x| x.barcode.clone(), tempdir))
     } else {
         Box::new(fragments)
     };
+    let is_sorted = if fragment_is_sorted_by_name || low_memory { true } else { false };
 
-    match output_file {
-        None => {
-            let mut anndata = PyAnnData::new(py)?;
-            preprocessing::import_fragments(
-                &mut anndata, sorted_fragments, &promoters, &chrom_sizes,
-                final_white_list.as_ref(), min_num_fragment, min_tsse, is_sorted, chunk_size,
-            )?;
-            Ok(anndata.to_object(py))
-        },
-        Some(fl) => {
-            let mut anndata = anndata::AnnData::new(fl, 0, 0)?;
+    macro_rules! run {
+        ($data:expr) => {
             preprocessing::import_fragments(
-                &mut anndata, sorted_fragments, &promoters, &chrom_sizes,
+                $data, sorted_fragments, &promoters, &chrom_sizes,
                 final_white_list.as_ref(), min_num_fragment, min_tsse, is_sorted, chunk_size,
-            )?;
-            Ok(AnnData::wrap(anndata).into_py(py))
-        },
+            )?
+        };
     }
+
+    crate::with_anndata!(&anndata, run);
+    Ok(())
 } 
 
+fn shift_fragment(fragment: &mut Fragment, shift_left: i64, shift_right: i64) {
+    if shift_left != 0 {
+        fragment.start = fragment.start.saturating_add_signed(shift_left);
+        if fragment.strand.is_some() {
+            fragment.end = fragment.end.saturating_add_signed(shift_left);
+        }
+    }
+    if shift_right != 0 && fragment.strand.is_none() {
+        fragment.end = fragment.end.saturating_add_signed(shift_right);
+    }
+}
+
 #[pyfunction]
-pub(crate) fn mk_tile_matrix<'py>(
-    py: Python<'py>, anndata: &'py PyAny, bin_size: u64, chunk_size: usize, num_cpu: usize
-) -> PyResult<()>
-{
-    match extract_anndata(py, anndata)? {
-        AnnDataObj::AnnData(x) => with_cpu(num_cpu, ||
-            create_tile_matrix(x.inner().deref(), bin_size, chunk_size).unwrap()),
-        AnnDataObj::PyAnnData(x) => create_tile_matrix(&x, bin_size, chunk_size).unwrap(),
-        _ => todo!(),
-    };
+pub(crate) fn mk_tile_matrix(
+    anndata: AnnDataLike, bin_size: usize, chunk_size: usize, 
+    exclude_chroms: Option<Vec<&str>>,
+    out: Option<AnnDataLike>
+) -> Result<()>
+{
+    macro_rules! run {
+        ($data:expr) => {
+            if let Some(out) = out {
+                macro_rules! run2 {
+                    ($out_data:expr) => {
+                        preprocessing::create_tile_matrix(
+                            $data,
+                            bin_size,
+                            chunk_size,
+                            exclude_chroms.as_ref().map(|x| x.as_slice()),
+                            Some($out_data)
+                        )?
+                    };
+                }
+                crate::with_anndata!(&out, run2);
+            } else {
+                preprocessing::create_tile_matrix(
+                    $data,
+                    bin_size,
+                    chunk_size,
+                    exclude_chroms.as_ref().map(|x| x.as_slice()),
+                    None::<&PyAnnData>
+                )?;
+            }
+        };
+    }
+
+    crate::with_anndata!(&anndata, run);
     Ok(())
 }
 
+/// Create tile matrix in parallel. Due to the limitation of Python GIL,
+/// this function is only applicable to pure Rust AnnData objects.
 #[pyfunction]
-pub(crate) fn mk_peak_matrix<'py>(
-    py: Python<'py>,
-    input: &'py PyAny,
-    peaks_str: &'py PyAny,
-    output_file: Option<PathBuf>,
-    chunk_size: usize,
-) -> PyResult<PyObject>
+pub(crate) fn mk_tile_matrix_par(
+    adatas: Vec<RustAnnDataLike>, bin_size: usize, chunk_size: usize, 
+    n_jobs: usize, exclude_chroms: Option<Vec<&str>>,
+) -> Result<()>
 {
-    fn action<A>(in_data: AnnDataObj, peaks: &GenomeRegions<GenomicRange>, out_data: &A, chunk_size: usize) -> Result<()>
-    where
-        A: AnnDataOp + AnnDataIterator,
-    {
-        match in_data {
-            AnnDataObj::AnnData(data) => create_peak_matrix(
-                out_data, data.inner().raw_count_iter(chunk_size)?.map(|x| x.0), &peaks),
-            AnnDataObj::AnnDataSet(data) => create_peak_matrix(
-                out_data, data.inner().raw_count_iter(chunk_size)?.map(|x| x.0), &peaks),
-            AnnDataObj::PyAnnData(data) => create_peak_matrix(
-                out_data, data.raw_count_iter(chunk_size)?.map(|x| x.0), &peaks),
-        }
+    macro_rules! run {
+        ($data:expr) => {
+            preprocessing::create_tile_matrix(
+                $data,
+                bin_size,
+                chunk_size,
+                exclude_chroms.as_ref().map(|x| x.as_slice()),
+                None::<&PyAnnData>
+            ).unwrap()
+        };
     }
 
-    let peaks: Result<GenomeRegions<GenomicRange>> = peaks_str.iter()?
-        .map(|x| Ok(GenomicRange::from_str(x?.extract()?).unwrap())).collect();
-    let in_anndata = extract_anndata(py, input)?;
-    if let Some(fl) = output_file {
-        let anndata = anndata::AnnData::new(fl, 0, 0)?;
-        action(in_anndata, &peaks?, &anndata, chunk_size)?;
-        Ok(AnnData::wrap(anndata).into_py(py))
-    } else {
-        let anndata = PyAnnData::new(py)?;
-        action(in_anndata, &peaks?, &anndata, chunk_size)?;
-        Ok(anndata.to_object(py))
+    rayon::ThreadPoolBuilder::new().num_threads(n_jobs).build().unwrap().install(|| {
+        adatas.into_par_iter().for_each(|adata| {
+            crate::with_rs_anndata!(&adata, run);
+        });
+    });
+    Ok(())
+}
+
+#[pyfunction]
+pub(crate) fn mk_peak_matrix(
+    anndata: AnnDataLike,
+    peaks: &PyAny,
+    chunk_size: usize,
+    use_x: bool,
+    out: Option<AnnDataLike>,
+) -> Result<()>
+{
+    let peaks = peaks.iter()?
+        .map(|x| GenomicRange::from_str(x.unwrap().extract().unwrap()).unwrap());
+
+    macro_rules! run {
+        ($data:expr) => {
+            if let Some(out) = out {
+                macro_rules! run2 {
+                    ($out_data:expr) => {
+                        preprocessing::create_peak_matrix($data, peaks, chunk_size, Some($out_data), use_x)?
+                    };
+                }
+                crate::with_anndata!(&out, run2);
+            } else {
+                preprocessing::create_peak_matrix($data, peaks, chunk_size, None::<&PyAnnData>, use_x)?;
+            }
+        }
     }
+    crate::with_anndata!(&anndata, run);
+    Ok(())
 }
 
 #[pyfunction]
-pub(crate) fn mk_gene_matrix<'py>(
-    py: Python<'py>,
-    input: &PyAny,
+pub(crate) fn mk_gene_matrix(
+    anndata: AnnDataLike,
     gff_file: PathBuf,
-    output_file: Option<PathBuf>,
     chunk_size: usize,
     use_x: bool,
     id_type: &str,
-) -> PyResult<PyObject>
+    out: Option<AnnDataLike>,
+) -> Result<()>
 {
-    fn action<A>(in_data: AnnDataObj, transcripts: Vec<Transcript>, out_data: &A,
-        chunk_size: usize, use_x: bool, id_type: &str) -> Result<()>
-    where
-        A: AnnDataOp + AnnDataIterator,
-    {
-        match in_data {
-            AnnDataObj::AnnData(data) => if use_x {
-                create_gene_matrix(out_data, data.inner().read_chrom_values::<u32>(chunk_size)?.map(|x| x.0), transcripts, id_type)
+    let transcripts = read_transcripts(gff_file);
+    macro_rules! run {
+        ($data:expr) => {
+            if let Some(out) = out {
+                macro_rules! run2 {
+                    ($out_data:expr) => {
+                        preprocessing::create_gene_matrix($data, transcripts, id_type, chunk_size, Some($out_data), use_x)?
+                    };
+                }
+                crate::with_anndata!(&out, run2);
             } else {
-                create_gene_matrix(out_data, data.inner().raw_count_iter(chunk_size)?.map(|x| x.0), transcripts, id_type)
-            },
-            AnnDataObj::AnnDataSet(data) => if use_x {
-                create_gene_matrix(out_data, data.inner().read_chrom_values::<u32>(chunk_size)?.map(|x| x.0), transcripts, id_type)
-            } else {
-                create_gene_matrix(out_data, data.inner().raw_count_iter(chunk_size)?.map(|x| x.0), transcripts, id_type)
-            },
-            AnnDataObj::PyAnnData(data) => if use_x {
-                create_gene_matrix(out_data, data.read_chrom_values::<u32>(chunk_size)?.map(|x| x.0), transcripts, id_type)
-            } else {
-                create_gene_matrix(out_data, data.raw_count_iter(chunk_size)?.map(|x| x.0), transcripts, id_type)
-            },
+                preprocessing::create_gene_matrix($data, transcripts, id_type, chunk_size, None::<&PyAnnData>, use_x)?;
+            }
         }
     }
- 
-    let transcripts = read_transcripts(BufReader::new(open_file(gff_file)));
-    let in_anndata = extract_anndata(py, input)?;
-    if let Some(fl) = output_file {
-        let anndata = anndata::AnnData::new(fl, 0, 0)?;
-        action(in_anndata, transcripts, &anndata, chunk_size, use_x, id_type)?;
-        Ok(AnnData::wrap(anndata).into_py(py))
-    } else {
-        let anndata = PyAnnData::new(py)?;
-        action(in_anndata, transcripts, &anndata, chunk_size, use_x, id_type)?;
-        Ok(anndata.to_object(py))
-    }
+    crate::with_anndata!(&anndata, run);
+    Ok(())
 }
```

### Comparing `snapatac2-2.2.0/src/utils.rs` & `snapatac2-2.3.0/src/utils.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,32 @@
-use pyanndata::{AnnData, AnnDataSet, PyAnnData};
+mod anndata;
+
+pub use self::anndata::{PyAnnData, AnnDataLike, RustAnnDataLike};
+
 use pyo3::{
     prelude::*,
     types::PyIterator,
     PyResult, Python,
-    PyTypeInfo,
 };
 use numpy::{Element, PyReadonlyArrayDyn, PyReadonlyArray, Ix1, Ix2, PyArray, IntoPyArray};
+use snapatac2_core::preprocessing::{Transcript, read_transcripts_from_gff, read_transcripts_from_gtf};
 use snapatac2_core::utils::similarity;
 
-use hdf5::H5Type;
 use bed_utils::{bed, bed::GenomicRange, bed::BED};
+use std::io::BufReader;
 use std::{str::FromStr, fs::File};
 use std::path::Path;
 use flate2::read::MultiGzDecoder;
-use hdf5;
 use linreg::lin_reg_imprecise;
 use linfa::{DatasetBase, traits::{Fit, Predict}};
 use linfa_clustering::KMeans;
 use rand_core::SeedableRng;
 use rand_isaac::Isaac64Rng;
 use hora::core::ann_index::ANNIndex;
 use nalgebra_sparse::CsrMatrix;
-use rayon::ThreadPoolBuilder;
 
 macro_rules! with_sparsity_pattern {
     ($dtype:expr, $indices:expr, $indptr:expr, $n:expr, $fun:ident) => {
         match $dtype {
             "int32" => {
                 let indices_ = $indices.extract::<PyReadonlyArray<i32, Ix1>>()?;
                 let indptr_ = $indptr.extract::<PyReadonlyArray<i32, Ix1>>()?;
@@ -254,18 +255,18 @@
 #[pyfunction]
 pub(crate) fn approximate_nearest_neighbors(
     data_: PyReadonlyArray<'_, f32, Ix2>,
     k: usize,
 ) -> PyResult<(Vec<f32>, Vec<i32>, Vec<i32>)>
 {
     let data = data_.as_array();
-    let dimension = data.shape()[1];
+    let shape = data.shape();
     let mut index = hora::index::hnsw_idx::HNSWIndex::<f32, usize>::new(
-        dimension,
-        &hora::index::hnsw_params::HNSWParams::<f32>::default(),
+        shape[1],
+        &hora::index::hnsw_params::HNSWParams::<f32>::default().max_item(shape[0].max(1000000)),
     );
     for (i, sample) in data.axis_iter(ndarray::Axis(0)).enumerate() {
         index.add(sample.to_vec().as_slice(), i).unwrap();
     }
     index.build(hora::core::metrics::Metric::Euclidean).unwrap();
     let row_iter = data.axis_iter(ndarray::Axis(0)).map(move |row| {
         index.search_nodes(row.to_vec().as_slice(), k).into_iter()
@@ -273,15 +274,14 @@
     });
     Ok(to_csr_matrix(row_iter))
 }
 
 pub(crate) fn to_csr_matrix<I, D>(iter: I) -> (Vec<D>, Vec<i32>, Vec<i32>)
 where
     I: Iterator<Item = Vec<(usize, D)>>,
-    D: H5Type,
 {
     let mut data: Vec<D> = Vec::new();
     let mut indices: Vec<i32> = Vec::new();
     let mut indptr: Vec<i32> = Vec::new();
 
     let n = iter.fold(0, |r_idx, mut row| {
         row.sort_by(|a, b| a.0.cmp(&b.0));
@@ -307,28 +307,22 @@
 }
 
 /// Determine if a file is gzipped.
 pub(crate) fn is_gzipped<P: AsRef<Path>>(file: P) -> bool {
     MultiGzDecoder::new(File::open(file).unwrap()).header().is_some()
 }
 
-pub fn with_cpu<OP, R>(num_cpu: usize, op: OP) -> R
-where OP: FnOnce() -> R + Send, R: Send
-{
-    ThreadPoolBuilder::new().num_threads(num_cpu).build().unwrap().install(op)
-}
-
-pub enum AnnDataObj<'a> {
-    AnnData(AnnData),
-    PyAnnData(PyAnnData<'a>),
-    AnnDataSet(AnnDataSet),
-}
-
-pub fn extract_anndata<'py>(py: Python<'py>, anndata: &'py PyAny) -> PyResult<AnnDataObj<'py>> {
-    if anndata.is_instance(AnnData::type_object(py))? {
-        Ok(AnnDataObj::AnnData(anndata.extract::<AnnData>()?))
-    } else if anndata.is_instance(AnnDataSet::type_object(py))? {
-        Ok(AnnDataObj::AnnDataSet(anndata.extract::<AnnDataSet>()?))
+pub fn read_transcripts<P: AsRef<std::path::Path>>(file_path: P) -> Vec<Transcript> {
+    let path = if file_path.as_ref().extension().unwrap() == "gz" {
+        file_path.as_ref().file_stem().unwrap().as_ref()
+    } else {
+        file_path.as_ref()
+    };
+    if path.extension().unwrap() == "gff" {
+        read_transcripts_from_gff(BufReader::new(open_file(file_path))).unwrap()
+    } else if path.extension().unwrap() == "gtf" {
+        read_transcripts_from_gtf(BufReader::new(open_file(file_path))).unwrap()
     } else {
-        anndata.extract::<PyAnnData>().map(|x| AnnDataObj::PyAnnData(x))
+        read_transcripts_from_gff(BufReader::new(open_file(file_path.as_ref())))
+            .unwrap_or_else(|_| read_transcripts_from_gtf(BufReader::new(open_file(file_path))).unwrap())
     }
 }
```

