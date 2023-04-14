# Comparing `tmp/hcai-datasets-nightly-0.1.7.dev202304131555.tar.gz` & `tmp/hcai-datasets-nightly-0.1.7.dev202304142234.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-datasets-nightly-0.1.7.dev202304131555.tar", last modified: Thu Apr 13 15:55:58 2023, max compression
+gzip compressed data, was "hcai-datasets-nightly-0.1.7.dev202304142234.tar", last modified: Fri Apr 14 22:34:35 2023, max compression
```

## Comparing `hcai-datasets-nightly-0.1.7.dev202304131555.tar` & `hcai-datasets-nightly-0.1.7.dev202304142234.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.139700 hcai-datasets-nightly-0.1.7.dev202304131555/
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-04-13 15:55:58.139700 hcai-datasets-nightly-0.1.7.dev202304131555/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8154 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.131699 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_dataset_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_dataset_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_dataset_utils/bridge_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (122)      928 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_dataset_utils/bridge_tf.py
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_dataset_utils/dataset_indexed.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_dataset_utils/import_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_dataset_utils/pytorch_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     2770 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_dataset_utils/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.131699 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.131699 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      607 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_affectnet_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_affectnet_tensorflow_native.py
--rw-r--r--   0 runner    (1001) docker     (122)      957 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_affectnet_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_ckplus_tensorflow_native.py
--rw-r--r--   0 runner    (1001) docker     (122)      946 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_ckplus_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_faces_tensorflow_native.py
--rw-r--r--   0 runner    (1001) docker     (122)      947 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_faces_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_nova_tensorflow_native.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.131699 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_affectnet/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.135699 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_affectnet/Ignore_Lists/
--rw-r--r--   0 runner    (1001) docker     (122)  2377285 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json
--rw-r--r--   0 runner    (1001) docker     (122)     6234 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_affectnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_affectnet/hcai_affectnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     5916 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.135699 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_audioset/
--rw-r--r--   0 runner    (1001) docker     (122)       66 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_audioset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2412 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_audioset/hcai_audioset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.135699 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_ckplus/
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_ckplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_ckplus/hcai_ckplus.py
--rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.135699 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_faces/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_faces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_faces/hcai_faces.py
--rw-r--r--   0 runner    (1001) docker     (122)     2051 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_faces/hcai_faces_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.135699 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_is2021_ess/
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_is2021_ess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.135699 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_librispeech/
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_librispeech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_librispeech/hcai_librispeech.py
--rw-r--r--   0 runner    (1001) docker     (122)      711 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_librispeech/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.139700 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19035 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py
--rw-r--r--   0 runner    (1001) docker     (122)     7686 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py
--rw-r--r--   0 runner    (1001) docker     (122)    22257 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.139700 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12651 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10754 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/utils/nova_string_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.139700 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1198 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/tests/dummy_set.py
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/tests/test_bridge_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 15:55:58.139700 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-04-13 15:55:58.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2439 2023-04-13 15:55:58.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 15:55:58.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-13 15:55:58.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-13 15:55:58.000000 hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-13 15:55:58.139700 hcai-datasets-nightly-0.1.7.dev202304131555/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-04-13 15:55:43.000000 hcai-datasets-nightly-0.1.7.dev202304131555/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.025945 hcai-datasets-nightly-0.1.7.dev202304142234/
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-04-14 22:34:35.025945 hcai-datasets-nightly-0.1.7.dev202304142234/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8154 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.017945 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_dataset_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_dataset_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_dataset_utils/bridge_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      928 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_dataset_utils/bridge_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_dataset_utils/dataset_indexed.py
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_dataset_utils/import_validator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_dataset_utils/pytorch_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2770 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_dataset_utils/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.017945 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.021945 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      607 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_affectnet_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_affectnet_tensorflow_native.py
+-rw-r--r--   0 runner    (1001) docker     (122)      957 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_affectnet_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_ckplus_tensorflow_native.py
+-rw-r--r--   0 runner    (1001) docker     (122)      946 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_ckplus_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_faces_tensorflow_native.py
+-rw-r--r--   0 runner    (1001) docker     (122)      947 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_faces_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1977 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_nova_tensorflow_native.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.021945 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_affectnet/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.021945 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_affectnet/Ignore_Lists/
+-rw-r--r--   0 runner    (1001) docker     (122)  2377285 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json
+-rw-r--r--   0 runner    (1001) docker     (122)     6234 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_affectnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_affectnet/hcai_affectnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5916 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.021945 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_audioset/
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_audioset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2412 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_audioset/hcai_audioset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.021945 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_ckplus/
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_ckplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_ckplus/hcai_ckplus.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1940 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.025945 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_faces/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_faces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_faces/hcai_faces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2051 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_faces/hcai_faces_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.025945 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_is2021_ess/
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_is2021_ess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.025945 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_librispeech/
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_librispeech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_librispeech/hcai_librispeech.py
+-rw-r--r--   0 runner    (1001) docker     (122)      711 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_librispeech/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.025945 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20249 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7686 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22257 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.025945 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12651 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10754 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/utils/nova_string_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.025945 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1198 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/tests/dummy_set.py
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/tests/test_bridge_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 22:34:35.025945 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9089 2023-04-14 22:34:34.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2439 2023-04-14 22:34:34.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-14 22:34:34.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-14 22:34:34.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-14 22:34:34.000000 hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-14 22:34:35.025945 hcai-datasets-nightly-0.1.7.dev202304142234/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2181 2023-04-14 22:34:26.000000 hcai-datasets-nightly-0.1.7.dev202304142234/setup.py
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/PKG-INFO` & `hcai-datasets-nightly-0.1.7.dev202304142234/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-datasets-nightly
-Version: 0.1.7.dev202304131555
+Version: 0.1.7.dev202304142234
 Summary: !Alpha Version! - This repository contains the backend server for the nova annotation ui (https://github.com/hcmlab/nova)
 Home-page: https://github.com/hcmlab/nova-server
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/README.md` & `hcai-datasets-nightly-0.1.7.dev202304142234/README.md`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_dataset_utils/bridge_pytorch.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_dataset_utils/bridge_pytorch.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_dataset_utils/bridge_tf.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_dataset_utils/bridge_tf.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_dataset_utils/import_validator.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_dataset_utils/import_validator.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_dataset_utils/pytorch_dataset_wrapper.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_dataset_utils/pytorch_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_dataset_utils/statistics.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_dataset_utils/statistics.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/__init__.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_affectnet_pytorch.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_affectnet_pytorch.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_affectnet_tensorflow_native.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_affectnet_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_affectnet_tfds.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_affectnet_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_ckplus_tensorflow_native.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_ckplus_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_ckplus_tfds.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_ckplus_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_faces_tensorflow_native.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_faces_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_faces_tfds.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_faces_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/examples/example_nova_tensorflow_native.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/examples/example_nova_tensorflow_native.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_affectnet/hcai_affectnet.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_affectnet/hcai_affectnet.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_audioset/hcai_audioset.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_audioset/hcai_audioset.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_ckplus/hcai_ckplus.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_ckplus/hcai_ckplus.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_faces/hcai_faces.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_faces/hcai_faces.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_faces/hcai_faces_iterable.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_faces/hcai_faces_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_librispeech/hcai_librispeech.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_librispeech/hcai_librispeech.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_librispeech/preprocessing.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_librispeech/preprocessing.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 
 import numpy as np
 import os
+import copy
 
 import nova_utils.db_utils.nova_types as nt
 import hcai_datasets.hcai_nova_dynamic.utils.nova_data_utils as ndu
 import hcai_datasets.hcai_nova_dynamic.utils.nova_anno_utils as nau
 from nova_utils.interfaces.dataset_iterable import DatasetIterable
 
 from hcai_datasets.hcai_nova_dynamic.utils.nova_data_utils import (
@@ -108,14 +109,16 @@
         self.annos, self.anno_schemes = self._populate_label_info_from_mongo_doc(
             mongo_schemes
         )
         self.data_info, self.data_schemes = self._populate_data_info_from_mongo_doc(
             mongo_data
         )
 
+        self.session_info = {s: {} for s in self.sessions}
+
         # setting supervised keys
         if supervised_keys and self.flatten_samples:
             if supervised_keys[0] not in self.data_streams:
                 # remove <role> of supervised keys
                 _, data_stream = split_role_key(supervised_keys[0])
                 if not data_stream in self.data_streams:
                     print(
@@ -139,14 +142,51 @@
                 else:
                     supervised_keys[1] = scheme
 
         self.supervised_keys = tuple(supervised_keys) if supervised_keys else None
 
         self._iterable = self._yield_sample()
 
+    def to_single_session_iterator(self, session_id=""):
+        """Returns a copy of the iterator for a single session. All data objects and annotation objects will be initialized."""
+        ds_iter_copy = copy.copy(self)
+        if session_id not in self.sessions:
+            print(
+                f"WARNING: Session {session_id} not found in iterator session list. Using first session instead: {ds_iter_copy.sessions[0]}"
+            )
+            session_id = ds_iter_copy.sessions[0]
+        elif not session_id:
+            session_id = ds_iter_copy.sessions[0]
+
+        ds_iter_copy._init_session(session_id)
+        return ds_iter_copy
+
+    def _init_session(self, session):
+        """Opens all annotations and data readers"""
+
+        if (
+            not self.session_info[session]
+            or not self.session_info[session]["is_active"]
+        ):
+
+            # Gather all data we need for this session
+            self._load_annotation_for_session(session, time_to_ms=True)
+            self._open_data_reader_for_session(session)
+
+            session_info = self.nova_db_handler.get_session_info(self.dataset, session)[
+                0
+            ]
+
+            # Depricate other sessions
+            for id, s in self.session_info.items():
+                s["is_active"] = False
+
+            session_info["is_active"] = True
+            self.session_info[session] = session_info
+
     def _populate_label_info_from_mongo_doc(self, mongo_schemes):
         """
         Setting self.annos
         Args:
           mongo_schemes:
 
         Returns:
@@ -260,15 +300,17 @@
                             sr=data_stream["sr"],
                             data_type=dtype,
                             is_valid=data_stream["isValid"],
                             sample_data_path=sample_data_path,
                             lazy_loading=self.lazy_loading,
                         )
                     else:
-                        raise ValueError("Invalid data type".format(data_stream["type"]))
+                        raise ValueError(
+                            "Invalid data type".format(data_stream["type"])
+                        )
 
                 except FileNotFoundError as fnf:
                     if self.fake_missing_data:
                         raise FileNotFoundError
                     else:
                         print(f"WARNING: Ignoring exception - {fnf}")
                         continue
@@ -294,47 +336,40 @@
             finally:
                 anno.set_annotation_from_mongo_doc(mongo_anno, time_to_ms=time_to_ms)
 
     def _open_data_reader_for_session(self, session):
         for data_id, data in self.data_info.items():
             try:
                 data_path = os.path.join(
-                    self.nova_data_dir, self.dataset, session, data_id + "." + data.file_ext
+                    self.nova_data_dir,
+                    self.dataset,
+                    session,
+                    data_id + "." + data.file_ext,
                 )
                 data.open_file_reader(data_path)
             except FileNotFoundError as fnf:
                 if self.fake_missing_data:
                     print(f"WARNING: {fnf} - Providing dummy data")
                 else:
                     raise fnf
 
-
     def _yield_sample(self):
         """Yields examples."""
 
         # Needed to sort the samples later and assure that the order is the same as in nova. Necessary for CML till the tfds can be returned in order.
         sample_counter = 1
 
         for session in self.sessions:
 
-            _frame_size_ms = self.frame_size_ms
-            _stride_ms = self.stride_ms
-
-            # Gather all data we need for this session
-            try:
-                self._load_annotation_for_session(session, time_to_ms=True)
-                self._open_data_reader_for_session(session)
-            except FileNotFoundError as fnf:
-                print(f"WARNING: {fnf} - Skipping session {session}")
-                continue
+            self._init_session(session)
 
-            session_info = self.nova_db_handler.get_session_info(self.dataset, session)[
-                0
-            ]
+            session_info = self.session_info[session]
             dur = session_info["duration"]
+            _frame_size_ms = self.frame_size_ms
+            _stride_ms = self.stride_ms
 
             # If we are loading any datastreams we check if any datastream is shorter than the duration stored in the database suggests
             if self.data_info:
                 dur = min(*[v.dur for k, v in self.data_info.items()], dur)
 
             if not dur:
                 raise ValueError("Session {} has no duration.".format(session))
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_tfds.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/tests/dummy_set.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/tests/dummy_set.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets/tests/test_bridge_pytorch.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets/tests/test_bridge_pytorch.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets_nightly.egg-info/PKG-INFO` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets_nightly.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-datasets-nightly
-Version: 0.1.7.dev202304131555
+Version: 0.1.7.dev202304142234
 Summary: !Alpha Version! - This repository contains the backend server for the nova annotation ui (https://github.com/hcmlab/nova)
 Home-page: https://github.com/hcmlab/nova-server
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/hcai_datasets_nightly.egg-info/SOURCES.txt` & `hcai-datasets-nightly-0.1.7.dev202304142234/hcai_datasets_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-datasets-nightly-0.1.7.dev202304131555/setup.py` & `hcai-datasets-nightly-0.1.7.dev202304142234/setup.py`

 * *Files identical despite different names*

