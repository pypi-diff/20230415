# Comparing `tmp/returnn-1.20230414.234522.tar.gz` & `tmp/returnn-1.20230415.10040.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/returnn-1.20230414.234522.tar", last modified: Fri Apr 14 21:59:32 2023, max compression
+gzip compressed data, was "dist/returnn-1.20230415.10040.tar", last modified: Fri Apr 14 23:16:01 2023, max compression
```

## Comparing `returnn-1.20230414.234522.tar` & `returnn-1.20230415.10040.tar`

### file list

```diff
@@ -1,421 +1,423 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/.kateconfig
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/_setup_info_generated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/demos/
--rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/12AX.cluster_map
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-fwd.config
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-horovod-mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-horovod-mpi.py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-horovod-mpi.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-hyper-param-tuning.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-iter-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-list-devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-lua-torch-layer.config
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-pretrain.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-record-and-push-to-webserver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-rf.config
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-rhn-enwik8.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-sprint-interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-tf-att-copy.config
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-tf-attention.config
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-tf-chunking-blstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-tf-contribrnn-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-tf-enc-dec.config
--rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-tf-hard-att-copy.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-tf-lstm-benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-tf-maxgradnorm-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-tf-native-lstm-lowmem.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-tf-native-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-tf-native-lstm2.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-tf-native-lstm2.12ax.tuned.config
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-tf-neural-transducer.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-tf-rec-explicit-lstm.config
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-tf-rec-explicit-rnn.config
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-tf-rec-self-att.config
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-tf-search-compiled-graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-tf-vanilla-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-timit-lstm-ctc.config
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-torch.config
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo-upd-mult-model.lstm.12ax.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/demo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/demos/mdlstm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/demos/mdlstm/IAM/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/demos/mdlstm/IAM/IAM_lines/
--rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/mdlstm/IAM/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/mdlstm/IAM/chars.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/mdlstm/IAM/config_demo
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/mdlstm/IAM/config_fwd
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/mdlstm/IAM/config_real
--rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/mdlstm/IAM/create_IAM_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/mdlstm/IAM/decode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/demos/mdlstm/IAM/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/demos/mdlstm/IAM/features/raw/
--rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/mdlstm/IAM/features/raw/demo.h5
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/mdlstm/IAM/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/mdlstm/IAM/lines.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/demos/mdlstm/IAM/split/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/mdlstm/IAM/split/eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/mdlstm/IAM/split/train.txt
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/mdlstm/IAM/split/valid.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/mdlstm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/demos/mdlstm/artificial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/mdlstm/artificial/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/mdlstm/artificial/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/mdlstm/artificial/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/mdlstm/artificial/trainconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/demos/mdlstm/artificial_rgb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/mdlstm/artificial_rgb/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/mdlstm/artificial_rgb/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/mdlstm/artificial_rgb/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/demos/mdlstm/artificial_rgb/trainconfig
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/__old_mod_loader__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/datasets/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/datasets/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/datasets/bundle_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/datasets/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/datasets/cached2.py
--rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/datasets/generating.py
--rw-r--r--   0 runner    (1001) docker     (123)    65108 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/datasets/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/datasets/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/datasets/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/datasets/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/datasets/multi_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/datasets/normalization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/datasets/numpy_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/datasets/raw_wav.py
--rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/datasets/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/datasets/stereo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn/datasets/util/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/datasets/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/datasets/util/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/datasets/util/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/engine/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-14 21:59:13.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/.git
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 21:59:17.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-14 21:59:17.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-14 21:59:17.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-04-14 21:59:17.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/aligner.gif
--rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-04-14 21:59:17.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/check.png
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-14 21:59:17.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-14 21:59:17.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/core.h
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-14 21:59:17.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/pytorch_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-14 21:59:17.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-14 21:59:17.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-14 21:59:17.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-14 21:59:17.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-14 21:59:17.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-14 21:59:17.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-14 21:59:17.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-14 21:59:17.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-14 21:59:17.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-14 21:59:17.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-14 21:59:17.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/ref_rna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-04-14 21:59:17.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-14 21:59:17.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-14 21:59:17.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-14 21:59:17.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-14 21:59:17.000000 returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn/extern/graph_editor/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/extern/graph_editor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/extern/graph_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/extern/graph_editor/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/extern/graph_editor/reroute.py
--rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/extern/graph_editor/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/extern/graph_editor/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/extern/graph_editor/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/extern/graph_editor/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30348 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/frontend/_numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/frontend/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/frontend/array_.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/frontend/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/frontend/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/frontend/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/frontend/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/frontend/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/frontend/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/frontend/dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/frontend/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/frontend/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/frontend/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/frontend/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/frontend/math_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/frontend/matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/frontend/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/frontend/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/frontend/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8633 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/frontend/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/frontend/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/frontend/run_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/frontend/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/frontend/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn/import_/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/import_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/import_/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/import_/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/import_/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/learning_rate_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/native_op.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   244328 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn/sprint/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/sprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/sprint/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/sprint/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/sprint/error_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/sprint/extern_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/sprint/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tensor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    97348 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tensor/_dim_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)   155428 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tensor/_tensor_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tensor/_tensor_mixin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tensor/_tensor_op_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tensor/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tensor/dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tensor/marked_dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tensor/tensor_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn/tf/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)   151442 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn/tf/frontend_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/frontend_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22492 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/frontend_layers/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/frontend_layers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/frontend_layers/config_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/frontend_layers/debug_eager_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/frontend_layers/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)    69697 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/frontend_layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14466 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/frontend_layers/make_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/frontend_layers/prev_tensor_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn/tf/frontend_low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/frontend_low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19964 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/frontend_low_level/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/hyper_param_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   149447 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   588393 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/layers/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)   538391 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/layers/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/layers/segmental_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52075 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/layers/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    78675 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)   222320 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn/tf/util/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   292981 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/util/ken_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/tf/util/open_fst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/torch/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn/torch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/torch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/torch/data/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/torch/data/returnn_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/torch/data/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20825 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/torch/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn/torch/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/torch/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33286 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/torch/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/torch/frontend/_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/torch/frontend/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn/torch/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/torch/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/torch/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/torch/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn/util/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   144922 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/util/better_exchook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/util/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/util/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/util/debug_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/util/fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/util/literal_py_to_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/util/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/util/py-to-pickle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/util/py_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/util/sig_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/returnn/util/task_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/returnn.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/DummySprintExec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/PyCharm-inspection-profile.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/tests/PyCharm.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/PyCharm.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/PyCharm.idea/.name
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/PyCharm.idea/codeStyleSettings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/tests/PyCharm.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/PyCharm.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/tests/PyCharm.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/PyCharm.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/PyCharm.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/PyCharm.idea/returnn.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/tests/PyCharm.idea/scopes/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/PyCharm.idea/scopes/scope_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/_set_num_threads1.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/_setup_test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/bpe-unicode-demo.codes
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/bpe-unicode-demo.vocab
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/lexicon_opt.fst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/lexicon_opt.isyms
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/lexicon_opt.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/lexicon_opt.osyms
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/lint_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/pycharm-inspect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/rf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/spelling.dic
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_Fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_GeneratingDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_HDFDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_LearningRateControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_MultiProcDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_PTDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_Pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_SprintDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_SprintInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_TFEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)   134969 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_TFNativeOp.py
--rw-r--r--   0 runner    (1001) docker     (123)   551303 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_TFNetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_TFNetworkRecLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_TFNetworkSigProcLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_TFUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)   187471 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_TFUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_TF_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_TaskSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_TaskSystem_SharedMem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_TranslationDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_fork_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_hdf_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_rf_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_rf_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_rf_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_rf_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_rf_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_torch_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tests/test_torch_internal_frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/_setup_returnn_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/analyze-dataset-batches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/bliss-collect-seq-lens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/bliss-dump-text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/bliss-get-segment-names.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/bliss-to-ogg-zip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/bpe-create-lexicon.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/calculate-word-error-rate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/cleanup-old-models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/collect-orth-symbols.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/collect-words.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/compile_native_op.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/compile_tf_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/debug-dump-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/debug-plot-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/dump-dataset-raw-strings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/dump-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/dump-forward-stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/dump-forward.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/dump-network-json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/dump-pickle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/extract_state_tying_from_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/get-attention-weights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/get-best-model-epoch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/hdf_dump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/hdf_dump_translation_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/import-blocks-mt-model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/import-t2t-mt-model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/tools/lattice_rescorer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/lattice_rescorer/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/lattice_rescorer/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/lattice_rescorer/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/tools/lattice_rescorer/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/lattice_rescorer/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/lattice_rescorer/example/libs_list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:59:32.000000 returnn-1.20230414.234522/tools/lattice_rescorer/example/network.040/
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/lattice_rescorer/example/rescore_lattice.sh
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/lattice_rescorer/example/state_vars_list
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/lattice_rescorer/example/tensor_names_list
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/lattice_rescorer/file.h
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/lattice_rescorer/htklatticerescorer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/lattice_rescorer/htklatticerescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/lattice_rescorer/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/lattice_rescorer/rescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/lattice_rescorer/vocabulary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/lattice_rescorer/vocabulary.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/tf_avg_checkpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/tf_inspect_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-04-14 21:59:11.000000 returnn-1.20230414.234522/tools/tf_inspect_summary_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/.kateconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/_setup_info_generated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/12AX.cluster_map
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-fwd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-horovod-mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-horovod-mpi.py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-horovod-mpi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-hyper-param-tuning.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-iter-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-list-devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-lua-torch-layer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-pretrain.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-record-and-push-to-webserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-rf.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-rhn-enwik8.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-sprint-interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-tf-att-copy.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-tf-attention.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-tf-chunking-blstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-tf-contribrnn-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-tf-enc-dec.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-tf-hard-att-copy.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-tf-lstm-benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-tf-maxgradnorm-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-tf-native-lstm-lowmem.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-tf-native-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-tf-native-lstm2.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-tf-native-lstm2.12ax.tuned.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-tf-neural-transducer.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-tf-rec-explicit-lstm.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-tf-rec-explicit-rnn.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-tf-rec-self-att.config
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-tf-search-compiled-graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-tf-vanilla-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-timit-lstm-ctc.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-torch.config
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo-upd-mult-model.lstm.12ax.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/demo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/demos/mdlstm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/demos/mdlstm/IAM/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/demos/mdlstm/IAM/IAM_lines/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/mdlstm/IAM/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/mdlstm/IAM/chars.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/mdlstm/IAM/config_demo
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/mdlstm/IAM/config_fwd
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/mdlstm/IAM/config_real
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/mdlstm/IAM/create_IAM_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/mdlstm/IAM/decode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/demos/mdlstm/IAM/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/demos/mdlstm/IAM/features/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/mdlstm/IAM/features/raw/demo.h5
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/mdlstm/IAM/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/mdlstm/IAM/lines.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/demos/mdlstm/IAM/split/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/mdlstm/IAM/split/eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/mdlstm/IAM/split/train.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/mdlstm/IAM/split/valid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/mdlstm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/demos/mdlstm/artificial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/mdlstm/artificial/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/mdlstm/artificial/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/mdlstm/artificial/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/mdlstm/artificial/trainconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/demos/mdlstm/artificial_rgb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/mdlstm/artificial_rgb/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/mdlstm/artificial_rgb/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/mdlstm/artificial_rgb/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/demos/mdlstm/artificial_rgb/trainconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24324 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/__old_mod_loader__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/datasets/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62931 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/datasets/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/datasets/bundle_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/datasets/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/datasets/cached2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/datasets/generating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65108 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/datasets/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/datasets/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/datasets/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75821 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/datasets/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/datasets/multi_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14607 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/datasets/normalization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/datasets/numpy_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/datasets/raw_wav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/datasets/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/datasets/stereo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn/datasets/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/datasets/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/datasets/util/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/datasets/util/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/engine/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-14 23:15:44.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/.git
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 23:15:46.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-14 23:15:46.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-14 23:15:46.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-04-14 23:15:46.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/aligner.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-04-14 23:15:46.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/check.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-14 23:15:46.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-14 23:15:46.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-14 23:15:46.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/pytorch_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-14 23:15:46.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-14 23:15:46.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-14 23:15:46.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-14 23:15:46.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-14 23:15:46.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-14 23:15:46.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-14 23:15:46.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-14 23:15:46.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-14 23:15:46.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-14 23:15:46.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-14 23:15:46.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/ref_rna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-04-14 23:15:46.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-14 23:15:46.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-14 23:15:46.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-14 23:15:46.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-14 23:15:46.000000 returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn/extern/graph_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/extern/graph_editor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/extern/graph_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/extern/graph_editor/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/extern/graph_editor/reroute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/extern/graph_editor/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/extern/graph_editor/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/extern/graph_editor/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/extern/graph_editor/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32120 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/frontend/_numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/frontend/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/frontend/array_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/frontend/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/frontend/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/frontend/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/frontend/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/frontend/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/frontend/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/frontend/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/frontend/dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/frontend/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/frontend/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/frontend/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/frontend/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/frontend/math_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/frontend/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/frontend/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/frontend/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/frontend/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8633 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/frontend/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/frontend/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/frontend/run_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/frontend/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/frontend/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn/import_/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/import_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/import_/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/import_/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/import_/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/learning_rate_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/native_op.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   244328 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/pretrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn/sprint/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/sprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/sprint/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/sprint/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/sprint/error_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/sprint/extern_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/sprint/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tensor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97348 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tensor/_dim_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)   155428 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tensor/_tensor_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tensor/_tensor_mixin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tensor/_tensor_op_overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tensor/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tensor/dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tensor/marked_dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tensor/tensor_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36852 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151442 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn/tf/frontend_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/frontend_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27303 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/frontend_layers/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/frontend_layers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/frontend_layers/config_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/frontend_layers/debug_eager_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/frontend_layers/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69697 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/frontend_layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14466 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/frontend_layers/make_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/frontend_layers/prev_tensor_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn/tf/frontend_low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/frontend_low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19964 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/frontend_low_level/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/hyper_param_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn/tf/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   149447 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   588393 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/layers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   538391 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/layers/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/layers/segmental_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52075 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/layers/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78675 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)   222320 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71410 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn/tf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   292981 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/util/ken_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/tf/util/open_fst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/torch/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn/torch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/torch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/torch/data/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/torch/data/returnn_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/torch/data/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20825 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/torch/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn/torch/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/torch/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39449 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/torch/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/torch/frontend/_rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/torch/frontend/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn/torch/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/torch/functional/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/torch/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/torch/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144922 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/util/better_exchook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/util/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/util/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/util/debug_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/util/fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/util/literal_py_to_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/util/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/util/py-to-pickle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/util/py_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/util/sig_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/returnn/util/task_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11784 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/returnn.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/DummySprintExec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/PyCharm-inspection-profile.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/tests/PyCharm.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/PyCharm.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/PyCharm.idea/.name
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/PyCharm.idea/codeStyleSettings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/tests/PyCharm.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/PyCharm.idea/codeStyles/Project.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/tests/PyCharm.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/PyCharm.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/PyCharm.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/PyCharm.idea/returnn.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/tests/PyCharm.idea/scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/PyCharm.idea/scopes/scope_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/_set_num_threads1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/_setup_test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/bpe-unicode-demo.codes
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/bpe-unicode-demo.vocab
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/lexicon_opt.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/lexicon_opt.isyms
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/lexicon_opt.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/lexicon_opt.osyms
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/lint_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/pycharm-inspect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/rf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/spelling.dic
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_Dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_Fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_GeneratingDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_HDFDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_LearningRateControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_MultiProcDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_PTDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_Pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_SprintDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_SprintInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   238053 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_TFEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134969 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_TFNativeOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   551303 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_TFNetworkLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   549696 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_TFNetworkRecLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_TFNetworkSigProcLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_TFUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187471 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_TFUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_TF_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_TaskSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_TaskSystem_SharedMem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_TranslationDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_fork_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_hdf_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_rf_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_rf_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_rf_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_rf_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_rf_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_rf_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_torch_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tests/test_torch_internal_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/_setup_returnn_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/analyze-dataset-batches.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/bliss-collect-seq-lens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/bliss-dump-text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/bliss-get-segment-names.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/bliss-to-ogg-zip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/bpe-create-lexicon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/calculate-word-error-rate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/cleanup-old-models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/collect-orth-symbols.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/collect-words.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/compile_native_op.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/compile_tf_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/debug-dump-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/debug-plot-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/dump-dataset-raw-strings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/dump-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/dump-forward-stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/dump-forward.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/dump-network-json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/dump-pickle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/extract_state_tying_from_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/get-attention-weights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/get-best-model-epoch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/hdf_dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/hdf_dump_translation_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/import-blocks-mt-model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/import-t2t-mt-model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/tools/lattice_rescorer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/lattice_rescorer/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/lattice_rescorer/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/lattice_rescorer/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/tools/lattice_rescorer/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/lattice_rescorer/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/lattice_rescorer/example/libs_list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 23:16:01.000000 returnn-1.20230415.10040/tools/lattice_rescorer/example/network.040/
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/lattice_rescorer/example/rescore_lattice.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/lattice_rescorer/example/state_vars_list
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/lattice_rescorer/example/tensor_names_list
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/lattice_rescorer/file.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/lattice_rescorer/htklatticerescorer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/lattice_rescorer/htklatticerescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/lattice_rescorer/main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/lattice_rescorer/rescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/lattice_rescorer/vocabulary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/lattice_rescorer/vocabulary.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/tf_avg_checkpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/tf_inspect_checkpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-04-14 23:15:43.000000 returnn-1.20230415.10040/tools/tf_inspect_summary_log.py
```

### Comparing `returnn-1.20230414.234522/.gitignore` & `returnn-1.20230415.10040/.gitignore`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/.gitmodules` & `returnn-1.20230415.10040/.gitmodules`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/CHANGELOG.md` & `returnn-1.20230415.10040/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/CODEOWNERS` & `returnn-1.20230415.10040/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/CONTRIBUTING.md` & `returnn-1.20230415.10040/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/LICENSE` & `returnn-1.20230415.10040/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/MANIFEST.in` & `returnn-1.20230415.10040/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/PKG-INFO` & `returnn-1.20230415.10040/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230414.234522
+Version: 1.20230415.10040
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230414.234522/README.rst` & `returnn-1.20230415.10040/README.rst`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/__init__.py` & `returnn-1.20230415.10040/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/12AX.cluster_map` & `returnn-1.20230415.10040/demos/12AX.cluster_map`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-fwd.config` & `returnn-1.20230415.10040/demos/demo-fwd.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-horovod-mpi.py` & `returnn-1.20230415.10040/demos/demo-horovod-mpi.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-horovod-mpi.py.sh` & `returnn-1.20230415.10040/demos/demo-horovod-mpi.py.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-hyper-param-tuning.config` & `returnn-1.20230415.10040/demos/demo-hyper-param-tuning.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-iter-dataset.py` & `returnn-1.20230415.10040/demos/demo-iter-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-list-devices.py` & `returnn-1.20230415.10040/demos/demo-list-devices.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-lua-torch-layer.config` & `returnn-1.20230415.10040/demos/demo-lua-torch-layer.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-record-and-push-to-webserver.py` & `returnn-1.20230415.10040/demos/demo-record-and-push-to-webserver.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-returnn-as-framework.py` & `returnn-1.20230415.10040/demos/demo-returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-rf.config` & `returnn-1.20230415.10040/demos/demo-rf.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-rhn-enwik8.config` & `returnn-1.20230415.10040/demos/demo-rhn-enwik8.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-sprint-interface.py` & `returnn-1.20230415.10040/demos/demo-sprint-interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-tf-att-copy.config` & `returnn-1.20230415.10040/demos/demo-tf-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-tf-attention.config` & `returnn-1.20230415.10040/demos/demo-tf-attention.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-tf-chunking-blstm.12ax.config` & `returnn-1.20230415.10040/demos/demo-tf-chunking-blstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-tf-contribrnn-lstm.12ax.config` & `returnn-1.20230415.10040/demos/demo-tf-contribrnn-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-tf-enc-dec.config` & `returnn-1.20230415.10040/demos/demo-tf-enc-dec.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-tf-hard-att-copy.config` & `returnn-1.20230415.10040/demos/demo-tf-hard-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-tf-lstm-benchmark.py` & `returnn-1.20230415.10040/demos/demo-tf-lstm-benchmark.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-tf-maxgradnorm-lstm.12ax.config` & `returnn-1.20230415.10040/demos/demo-tf-maxgradnorm-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-tf-native-lstm-lowmem.12ax.config` & `returnn-1.20230415.10040/demos/demo-tf-native-lstm-lowmem.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-tf-native-lstm.12ax.config` & `returnn-1.20230415.10040/demos/demo-tf-native-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-tf-native-lstm2.12ax.config` & `returnn-1.20230415.10040/demos/demo-tf-native-lstm2.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-tf-native-lstm2.12ax.tuned.config` & `returnn-1.20230415.10040/demos/demo-tf-native-lstm2.12ax.tuned.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-tf-neural-transducer.12ax.config` & `returnn-1.20230415.10040/demos/demo-tf-neural-transducer.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-tf-rec-explicit-lstm.config` & `returnn-1.20230415.10040/demos/demo-tf-rec-explicit-lstm.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-tf-rec-explicit-rnn.config` & `returnn-1.20230415.10040/demos/demo-tf-rec-explicit-rnn.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-tf-rec-self-att.config` & `returnn-1.20230415.10040/demos/demo-tf-rec-self-att.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-tf-search-compiled-graph.py` & `returnn-1.20230415.10040/demos/demo-tf-search-compiled-graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-tf-vanilla-lstm.12ax.config` & `returnn-1.20230415.10040/demos/demo-tf-vanilla-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-timit-lstm-ctc.config` & `returnn-1.20230415.10040/demos/demo-timit-lstm-ctc.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-torch.config` & `returnn-1.20230415.10040/demos/demo-torch.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo-upd-mult-model.lstm.12ax.config` & `returnn-1.20230415.10040/demos/demo-upd-mult-model.lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/demo.sh` & `returnn-1.20230415.10040/demos/demo.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png` & `returnn-1.20230415.10040/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/mdlstm/IAM/IAM_lines/a01-007-04.png` & `returnn-1.20230415.10040/demos/mdlstm/IAM/IAM_lines/a01-007-04.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/mdlstm/IAM/IAM_lines/a01-007-06.png` & `returnn-1.20230415.10040/demos/mdlstm/IAM/IAM_lines/a01-007-06.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/mdlstm/IAM/README.txt` & `returnn-1.20230415.10040/demos/mdlstm/IAM/README.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/mdlstm/IAM/config_demo` & `returnn-1.20230415.10040/demos/mdlstm/IAM/config_demo`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/mdlstm/IAM/config_fwd` & `returnn-1.20230415.10040/demos/mdlstm/IAM/config_fwd`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/mdlstm/IAM/config_real` & `returnn-1.20230415.10040/demos/mdlstm/IAM/config_real`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/mdlstm/IAM/create_IAM_dataset.py` & `returnn-1.20230415.10040/demos/mdlstm/IAM/create_IAM_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/mdlstm/IAM/decode.py` & `returnn-1.20230415.10040/demos/mdlstm/IAM/decode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/mdlstm/IAM/features/raw/demo.h5` & `returnn-1.20230415.10040/demos/mdlstm/IAM/features/raw/demo.h5`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/mdlstm/IAM/split/eval.txt` & `returnn-1.20230415.10040/demos/mdlstm/IAM/split/eval.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/mdlstm/IAM/split/train.txt` & `returnn-1.20230415.10040/demos/mdlstm/IAM/split/train.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/mdlstm/IAM/split/valid.txt` & `returnn-1.20230415.10040/demos/mdlstm/IAM/split/valid.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/mdlstm/artificial/create_test_h5.py` & `returnn-1.20230415.10040/demos/mdlstm/artificial/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/mdlstm/artificial/forwardconfig` & `returnn-1.20230415.10040/demos/mdlstm/artificial/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/mdlstm/artificial/trainconfig` & `returnn-1.20230415.10040/demos/mdlstm/artificial/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/mdlstm/artificial_rgb/create_test_h5.py` & `returnn-1.20230415.10040/demos/mdlstm/artificial_rgb/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/mdlstm/artificial_rgb/forwardconfig` & `returnn-1.20230415.10040/demos/mdlstm/artificial_rgb/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/demos/mdlstm/artificial_rgb/trainconfig` & `returnn-1.20230415.10040/demos/mdlstm/artificial_rgb/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/__init__.py` & `returnn-1.20230415.10040/returnn/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/__main__.py` & `returnn-1.20230415.10040/returnn/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/__old_mod_loader__.py` & `returnn-1.20230415.10040/returnn/__old_mod_loader__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/__setup__.py` & `returnn-1.20230415.10040/returnn/__setup__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/config.py` & `returnn-1.20230415.10040/returnn/config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/datasets/audio.py` & `returnn-1.20230415.10040/returnn/datasets/audio.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/datasets/basic.py` & `returnn-1.20230415.10040/returnn/datasets/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/datasets/bundle_file.py` & `returnn-1.20230415.10040/returnn/datasets/bundle_file.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/datasets/cached.py` & `returnn-1.20230415.10040/returnn/datasets/cached.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/datasets/cached2.py` & `returnn-1.20230415.10040/returnn/datasets/cached2.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/datasets/generating.py` & `returnn-1.20230415.10040/returnn/datasets/generating.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/datasets/hdf.py` & `returnn-1.20230415.10040/returnn/datasets/hdf.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/datasets/lm.py` & `returnn-1.20230415.10040/returnn/datasets/lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/datasets/map.py` & `returnn-1.20230415.10040/returnn/datasets/map.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/datasets/meta.py` & `returnn-1.20230415.10040/returnn/datasets/meta.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/datasets/multi_proc.py` & `returnn-1.20230415.10040/returnn/datasets/multi_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/datasets/normalization_data.py` & `returnn-1.20230415.10040/returnn/datasets/normalization_data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/datasets/numpy_dump.py` & `returnn-1.20230415.10040/returnn/datasets/numpy_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/datasets/raw_wav.py` & `returnn-1.20230415.10040/returnn/datasets/raw_wav.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/datasets/sprint.py` & `returnn-1.20230415.10040/returnn/datasets/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/datasets/stereo.py` & `returnn-1.20230415.10040/returnn/datasets/stereo.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/datasets/util/feature_extraction.py` & `returnn-1.20230415.10040/returnn/datasets/util/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/datasets/util/vocabulary.py` & `returnn-1.20230415.10040/returnn/datasets/util/vocabulary.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/engine/base.py` & `returnn-1.20230415.10040/returnn/engine/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/engine/batch.py` & `returnn-1.20230415.10040/returnn/engine/batch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/WarpRna/__init__.py` & `returnn-1.20230415.10040/returnn/extern/WarpRna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/WarpRna/__main__.py` & `returnn-1.20230415.10040/returnn/extern/WarpRna/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/LICENSE` & `returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/README.md` & `returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/aligner.gif` & `returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/aligner.gif`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/check.png` & `returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/check.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/core.cu` & `returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/core.h` & `returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/core_cpu.cpp` & `returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/core_cpu.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE` & `returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md` & `returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp` & `returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu` & `returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h` & `returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py` & `returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py` & `returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py` & `returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/ref_rna.py` & `returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/ref_rna.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py` & `returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc` & `returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h` & `returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py` & `returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/WarpRna/warp-rna/test.cpp` & `returnn-1.20230415.10040/returnn/extern/WarpRna/warp-rna/test.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/graph_editor/__init__.py` & `returnn-1.20230415.10040/returnn/extern/graph_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/graph_editor/edit.py` & `returnn-1.20230415.10040/returnn/extern/graph_editor/edit.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/graph_editor/reroute.py` & `returnn-1.20230415.10040/returnn/extern/graph_editor/reroute.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/graph_editor/select.py` & `returnn-1.20230415.10040/returnn/extern/graph_editor/select.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/graph_editor/subgraph.py` & `returnn-1.20230415.10040/returnn/extern/graph_editor/subgraph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/graph_editor/transform.py` & `returnn-1.20230415.10040/returnn/extern/graph_editor/transform.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/extern/graph_editor/util.py` & `returnn-1.20230415.10040/returnn/extern/graph_editor/util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/frontend/__init__.py` & `returnn-1.20230415.10040/returnn/frontend/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 # Now the rest, in alphabetical order.
 from .array_ import *
 from .attention import *
 from .cond import *
 from .const import *
 from .container import *
+from .conv import *
 from .dims import *
 from .dropout import *
 from .dtype import *
 from .gradient import *
 from .linear import *
 from .loss import *
 from .math_ import *
```

### Comparing `returnn-1.20230414.234522/returnn/frontend/_backend.py` & `returnn-1.20230415.10040/returnn/frontend/_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -782,14 +782,69 @@
         :param momentum:
         :param affine:
         :param use_mask:
         :return:
         """
         raise NotImplementedError
 
+    # noinspection PyShadowingBuiltins
+    @staticmethod
+    def conv(
+        source: Tensor,
+        *,
+        in_dim: Dim,
+        out_dim: Dim,
+        in_spatial_dims: Sequence[Dim],
+        out_spatial_dims: Optional[Sequence[Dim]] = None,
+        filter: Tensor,
+        filter_size: Sequence[Dim],  # to have the order well-defined
+        padding: str,
+        strides: Optional[Union[int, Sequence[int]]] = None,
+        dilation_rate: Optional[Union[int, Sequence[int]]] = None,
+        groups: Optional[int] = None,
+        bias: Optional[Tensor] = None,
+    ) -> Tuple[Tensor, Sequence[Dim]]:
+        """convolution"""
+        raise NotImplementedError
+
+    # noinspection PyShadowingBuiltins
+    @staticmethod
+    def transposed_conv(
+        source: Tensor,
+        *,
+        in_dim: Dim,
+        out_dim: Dim,
+        in_spatial_dims: Sequence[Dim],
+        out_spatial_dims: Optional[Sequence[Dim]] = None,
+        filter: Tensor,
+        filter_size: Sequence[Dim],
+        padding: str,
+        remove_padding: Union[Sequence[int], int] = 0,
+        output_padding: Optional[Union[Sequence[Optional[int]], int]] = None,
+        strides: Optional[Sequence[int]] = None,
+        bias: Optional[Tensor] = None,
+    ) -> Tuple[Tensor, Sequence[Dim]]:
+        """transposed convolution"""
+        raise NotImplementedError
+
+    @staticmethod
+    def pool(
+        source: Tensor,
+        *,
+        mode: str,
+        pool_size: Sequence[int],
+        padding: str = "valid",
+        dilation_rate: Union[Sequence[int], int] = 1,
+        strides: Sequence[int],
+        in_spatial_dims: Sequence[Dim],
+        out_spatial_dims: Optional[Sequence[Dim]] = None,
+    ) -> Tuple[Tensor, Sequence[Dim]]:
+        """pooling"""
+        raise NotImplementedError
+
 
 # We use a global instance, and we modify __class__ inplace,
 # such that any reference to this can be updated.
 # This is exposed to the user as `returnn.frontend`.
 # The __class__ assignment is done in `select_engine`.
 # Use object.__new__ because we disallow creating instances of Frontend.
 global_backend = object.__new__(Backend)
```

### Comparing `returnn-1.20230414.234522/returnn/frontend/_numpy_backend.py` & `returnn-1.20230415.10040/returnn/frontend/_numpy_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/frontend/_utils.py` & `returnn-1.20230415.10040/returnn/frontend/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/frontend/array_.py` & `returnn-1.20230415.10040/returnn/frontend/array_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/frontend/attention.py` & `returnn-1.20230415.10040/returnn/frontend/attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/frontend/cond.py` & `returnn-1.20230415.10040/returnn/frontend/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/frontend/const.py` & `returnn-1.20230415.10040/returnn/frontend/const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/frontend/container.py` & `returnn-1.20230415.10040/returnn/frontend/container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/frontend/dims.py` & `returnn-1.20230415.10040/returnn/frontend/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/frontend/dropout.py` & `returnn-1.20230415.10040/returnn/frontend/dropout.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/frontend/dtype.py` & `returnn-1.20230415.10040/returnn/frontend/dtype.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/frontend/init.py` & `returnn-1.20230415.10040/returnn/frontend/init.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/frontend/linear.py` & `returnn-1.20230415.10040/returnn/frontend/linear.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/frontend/loss.py` & `returnn-1.20230415.10040/returnn/frontend/loss.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/frontend/math_.py` & `returnn-1.20230415.10040/returnn/frontend/math_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/frontend/matmul.py` & `returnn-1.20230415.10040/returnn/frontend/matmul.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/frontend/module.py` & `returnn-1.20230415.10040/returnn/frontend/module.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/frontend/normalization.py` & `returnn-1.20230415.10040/returnn/frontend/normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/frontend/parameter.py` & `returnn-1.20230415.10040/returnn/frontend/parameter.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/frontend/rand.py` & `returnn-1.20230415.10040/returnn/frontend/rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/frontend/reduce.py` & `returnn-1.20230415.10040/returnn/frontend/reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/frontend/run_ctx.py` & `returnn-1.20230415.10040/returnn/frontend/run_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/frontend/state.py` & `returnn-1.20230415.10040/returnn/frontend/state.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/frontend/types.py` & `returnn-1.20230415.10040/returnn/frontend/types.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/import_/common.py` & `returnn-1.20230415.10040/returnn/import_/common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/import_/git.py` & `returnn-1.20230415.10040/returnn/import_/git.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/import_/import_.py` & `returnn-1.20230415.10040/returnn/import_/import_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/learning_rate_control.py` & `returnn-1.20230415.10040/returnn/learning_rate_control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/log.py` & `returnn-1.20230415.10040/returnn/log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/native_op.cpp` & `returnn-1.20230415.10040/returnn/native_op.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/native_op.py` & `returnn-1.20230415.10040/returnn/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/pretrain.py` & `returnn-1.20230415.10040/returnn/pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/sprint/cache.py` & `returnn-1.20230415.10040/returnn/sprint/cache.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/sprint/control.py` & `returnn-1.20230415.10040/returnn/sprint/control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/sprint/error_signals.py` & `returnn-1.20230415.10040/returnn/sprint/error_signals.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/sprint/extern_interface.py` & `returnn-1.20230415.10040/returnn/sprint/extern_interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/sprint/interface.py` & `returnn-1.20230415.10040/returnn/sprint/interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tensor/_dim_extra.py` & `returnn-1.20230415.10040/returnn/tensor/_dim_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tensor/_tensor_extra.py` & `returnn-1.20230415.10040/returnn/tensor/_tensor_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tensor/_tensor_mixin_base.py` & `returnn-1.20230415.10040/returnn/tensor/_tensor_mixin_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tensor/_tensor_op_overloads.py` & `returnn-1.20230415.10040/returnn/tensor/_tensor_op_overloads.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tensor/control_flow_ctx.py` & `returnn-1.20230415.10040/returnn/tensor/control_flow_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tensor/dim.py` & `returnn-1.20230415.10040/returnn/tensor/dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tensor/marked_dim.py` & `returnn-1.20230415.10040/returnn/tensor/marked_dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tensor/tensor.py` & `returnn-1.20230415.10040/returnn/tensor/tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tensor/tensor_dict.py` & `returnn-1.20230415.10040/returnn/tensor/tensor_dict.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tf/compat.py` & `returnn-1.20230415.10040/returnn/tf/compat.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tf/data_pipeline.py` & `returnn-1.20230415.10040/returnn/tf/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tf/distributed.py` & `returnn-1.20230415.10040/returnn/tf/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tf/engine.py` & `returnn-1.20230415.10040/returnn/tf/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tf/frontend_layers/_backend.py` & `returnn-1.20230415.10040/returnn/tf/frontend_layers/_backend.py`

 * *Files 13% similar despite different names*

```diff
@@ -587,14 +587,143 @@
                 "momentum": momentum,
                 "epsilon": epsilon,
                 "masked_time": use_mask,
             },
             name="batch_norm",
         )
 
+    # noinspection PyShadowingBuiltins
+    @staticmethod
+    def conv(
+        source: Tensor,
+        *,
+        in_dim: Dim,
+        out_dim: Dim,
+        in_spatial_dims: Sequence[Dim],
+        out_spatial_dims: Optional[Sequence[Dim]] = None,
+        filter: Tensor,
+        filter_size: Sequence[Dim],  # to have the order well-defined
+        padding: str,
+        strides: Optional[Union[int, Sequence[int]]] = None,
+        dilation_rate: Optional[Union[int, Sequence[int]]] = None,
+        groups: Optional[int] = None,
+        bias: Optional[Tensor] = None,
+    ) -> Tuple[Tensor, Sequence[Dim]]:
+        """conv"""
+        if not out_spatial_dims:
+            out_spatial_dims = rf.make_conv_out_spatial_dims(
+                description_prefix="conv",
+                in_spatial_dims=in_spatial_dims,
+                filter_size=[d.dimension for d in filter_size],
+                strides=strides or 1,
+                dilation_rate=dilation_rate or 1,
+                padding=padding,
+            )
+        layer_dict = {
+            "class": "conv",
+            "from": source,
+            "in_dim": in_dim,
+            "in_spatial_dims": in_spatial_dims,
+            "out_dim": out_dim,
+            "out_spatial_dims": out_spatial_dims,
+            "filter_size": filter_size,
+            "padding": padding,
+        }
+        if strides:
+            layer_dict["strides"] = strides
+        if dilation_rate:
+            layer_dict["dilation_rate"] = dilation_rate
+        if groups:
+            layer_dict["groups"] = groups
+        layer_dict.update({"filter": filter, "with_bias": bias is not None})
+        if bias is not None:
+            layer_dict["bias"] = bias
+        out = rfl.make_layer(layer_dict, name="conv")
+        return out, out_spatial_dims
+
+    # noinspection PyShadowingBuiltins
+    @staticmethod
+    def transposed_conv(
+        source: Tensor,
+        *,
+        in_dim: Dim,
+        out_dim: Dim,
+        in_spatial_dims: Sequence[Dim],
+        out_spatial_dims: Optional[Sequence[Dim]] = None,
+        filter: Tensor,
+        filter_size: Sequence[Dim],
+        padding: str,
+        remove_padding: Union[Sequence[int], int] = 0,
+        output_padding: Optional[Union[Sequence[Optional[int]], int]] = None,
+        strides: Optional[Sequence[int]] = None,
+        bias: Optional[Tensor] = None,
+    ) -> Tuple[Tensor, Sequence[Dim]]:
+        """transposed conv"""
+        if not out_spatial_dims:
+            out_spatial_dims = [Dim(None, name=f"out-spatial-dim{i}") for i, s in enumerate(filter_size)]
+            for i in range(len(filter_size)):
+                s = filter_size[i].dimension if not strides else strides[i]
+                if filter_size[i].dimension == s == 1 or (s == 1 and padding.lower() == "same"):
+                    out_spatial_dims[i] = in_spatial_dims[i]
+        layer_dict = {
+            "class": "transposed_conv",
+            "from": source,
+            "in_dim": in_dim,
+            "in_spatial_dims": in_spatial_dims,
+            "out_dim": out_dim,
+            "out_spatial_dims": out_spatial_dims,
+            "filter_size": filter_size,
+            "padding": padding,
+        }
+        if remove_padding:
+            layer_dict["remove_padding"] = remove_padding
+        if output_padding:
+            layer_dict["output_padding"] = output_padding
+        if strides:
+            layer_dict["strides"] = strides
+        layer_dict.update({"filter": filter, "with_bias": bias is not None})
+        if bias is not None:
+            layer_dict["bias"] = bias
+        out = rfl.make_layer(layer_dict, name="transposed_conv")
+        return out, out_spatial_dims
+
+    @staticmethod
+    def pool(
+        source: Tensor,
+        *,
+        mode: str,
+        pool_size: Sequence[int],
+        padding: str = "valid",
+        dilation_rate: Union[Sequence[int], int] = 1,
+        strides: Sequence[int],
+        in_spatial_dims: Sequence[Dim],
+        out_spatial_dims: Optional[Sequence[Dim]] = None,
+    ) -> Tuple[Tensor, Sequence[Dim]]:
+        """pool"""
+        if out_spatial_dims is None:
+            out_spatial_dims = rf.make_conv_out_spatial_dims(
+                description_prefix="pool",
+                in_spatial_dims=in_spatial_dims,
+                filter_size=pool_size,
+                strides=strides,
+                dilation_rate=dilation_rate,
+                padding=padding,
+            )
+        args = {
+            "mode": mode,
+            "pool_size": pool_size,
+            "padding": padding,
+            "dilation_rate": dilation_rate,
+            "strides": strides,
+            "in_spatial_dims": in_spatial_dims,
+            "out_spatial_dims": out_spatial_dims,
+        }
+        layer = rfl.make_layer({"class": "pool", "from": source, **args}, name="pool")
+        return layer, out_spatial_dims
+
 
 def _random_replay_eval(idx, **_kwargs):
     # noinspection PyProtectedMember
     elem = ReturnnLayersBackend._random_journal[idx]
     assert isinstance(elem, dict)
     out = elem["out"]
     assert isinstance(out, Tensor)
```

### Comparing `returnn-1.20230414.234522/returnn/tf/frontend_layers/_utils.py` & `returnn-1.20230415.10040/returnn/tf/frontend_layers/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tf/frontend_layers/config_entry_points.py` & `returnn-1.20230415.10040/returnn/tf/frontend_layers/config_entry_points.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tf/frontend_layers/debug_eager_mode.py` & `returnn-1.20230415.10040/returnn/tf/frontend_layers/debug_eager_mode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tf/frontend_layers/dims.py` & `returnn-1.20230415.10040/returnn/tf/frontend_layers/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tf/frontend_layers/layer.py` & `returnn-1.20230415.10040/returnn/tf/frontend_layers/layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tf/frontend_layers/make_layer.py` & `returnn-1.20230415.10040/returnn/tf/frontend_layers/make_layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tf/frontend_layers/prev_tensor_ref.py` & `returnn-1.20230415.10040/returnn/tf/frontend_layers/prev_tensor_ref.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tf/frontend_low_level/_backend.py` & `returnn-1.20230415.10040/returnn/tf/frontend_low_level/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tf/horovod.py` & `returnn-1.20230415.10040/returnn/tf/horovod.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tf/hyper_param_tuning.py` & `returnn-1.20230415.10040/returnn/tf/hyper_param_tuning.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tf/layers/base.py` & `returnn-1.20230415.10040/returnn/tf/layers/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tf/layers/basic.py` & `returnn-1.20230415.10040/returnn/tf/layers/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tf/layers/rec.py` & `returnn-1.20230415.10040/returnn/tf/layers/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tf/layers/segmental_model.py` & `returnn-1.20230415.10040/returnn/tf/layers/segmental_model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tf/layers/signal_processing.py` & `returnn-1.20230415.10040/returnn/tf/layers/signal_processing.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tf/native_op.py` & `returnn-1.20230415.10040/returnn/tf/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tf/network.py` & `returnn-1.20230415.10040/returnn/tf/network.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tf/sprint.py` & `returnn-1.20230415.10040/returnn/tf/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tf/updater.py` & `returnn-1.20230415.10040/returnn/tf/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tf/util/basic.py` & `returnn-1.20230415.10040/returnn/tf/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tf/util/data.py` & `returnn-1.20230415.10040/returnn/tf/util/data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tf/util/ken_lm.py` & `returnn-1.20230415.10040/returnn/tf/util/ken_lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/tf/util/open_fst.py` & `returnn-1.20230415.10040/returnn/tf/util/open_fst.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/torch/data/pipeline.py` & `returnn-1.20230415.10040/returnn/torch/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/torch/data/returnn_dataset_wrapper.py` & `returnn-1.20230415.10040/returnn/torch/data/returnn_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/torch/data/tensor_utils.py` & `returnn-1.20230415.10040/returnn/torch/data/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/torch/engine.py` & `returnn-1.20230415.10040/returnn/torch/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/torch/frontend/_rand.py` & `returnn-1.20230415.10040/returnn/torch/frontend/_rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/torch/frontend/bridge.py` & `returnn-1.20230415.10040/returnn/torch/frontend/bridge.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/torch/updater.py` & `returnn-1.20230415.10040/returnn/torch/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/util/basic.py` & `returnn-1.20230415.10040/returnn/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/util/better_exchook.py` & `returnn-1.20230415.10040/returnn/util/better_exchook.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/util/bpe.py` & `returnn-1.20230415.10040/returnn/util/bpe.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/util/debug.py` & `returnn-1.20230415.10040/returnn/util/debug.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/util/debug_helpers.py` & `returnn-1.20230415.10040/returnn/util/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/util/fsa.py` & `returnn-1.20230415.10040/returnn/util/fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/util/literal_py_to_pickle.py` & `returnn-1.20230415.10040/returnn/util/literal_py_to_pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/util/pprint.py` & `returnn-1.20230415.10040/returnn/util/pprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/util/py-to-pickle.cpp` & `returnn-1.20230415.10040/returnn/util/py-to-pickle.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/util/sig_proc.py` & `returnn-1.20230415.10040/returnn/util/sig_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn/util/task_system.py` & `returnn-1.20230415.10040/returnn/util/task_system.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/returnn.egg-info/PKG-INFO` & `returnn-1.20230415.10040/returnn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230414.234522
+Version: 1.20230415.10040
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230414.234522/returnn.egg-info/SOURCES.txt` & `returnn-1.20230415.10040/returnn.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -155,14 +155,15 @@
 returnn/frontend/_numpy_backend.py
 returnn/frontend/_utils.py
 returnn/frontend/array_.py
 returnn/frontend/attention.py
 returnn/frontend/cond.py
 returnn/frontend/const.py
 returnn/frontend/container.py
+returnn/frontend/conv.py
 returnn/frontend/dims.py
 returnn/frontend/dropout.py
 returnn/frontend/dtype.py
 returnn/frontend/gradient.py
 returnn/frontend/init.py
 returnn/frontend/linear.py
 returnn/frontend/loss.py
@@ -302,14 +303,15 @@
 tests/test_demos.py
 tests/test_fork_exec.py
 tests/test_hdf_dump.py
 tests/test_rf_array.py
 tests/test_rf_attention.py
 tests/test_rf_base.py
 tests/test_rf_container.py
+tests/test_rf_conv.py
 tests/test_rf_normalization.py
 tests/test_tensor.py
 tests/test_tools.py
 tests/test_torch_frontend.py
 tests/test_torch_internal_frontend.py
 tests/PyCharm.idea/.gitignore
 tests/PyCharm.idea/.name
```

### Comparing `returnn-1.20230414.234522/setup.py` & `returnn-1.20230415.10040/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/DummySprintExec.py` & `returnn-1.20230415.10040/tests/DummySprintExec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/PyCharm-inspection-profile.xml` & `returnn-1.20230415.10040/tests/PyCharm-inspection-profile.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/PyCharm.idea/codeStyleSettings.xml` & `returnn-1.20230415.10040/tests/PyCharm.idea/codeStyleSettings.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml` & `returnn-1.20230415.10040/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/_set_num_threads1.py` & `returnn-1.20230415.10040/tests/_set_num_threads1.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/_setup_test_env.py` & `returnn-1.20230415.10040/tests/_setup_test_env.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/bpe-unicode-demo.codes` & `returnn-1.20230415.10040/tests/bpe-unicode-demo.codes`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/bpe-unicode-demo.vocab` & `returnn-1.20230415.10040/tests/bpe-unicode-demo.vocab`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/lexicon_opt.isyms` & `returnn-1.20230415.10040/tests/lexicon_opt.isyms`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/lexicon_opt.jpg` & `returnn-1.20230415.10040/tests/lexicon_opt.jpg`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/lint_common.py` & `returnn-1.20230415.10040/tests/lint_common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/pycharm-inspect.py` & `returnn-1.20230415.10040/tests/pycharm-inspect.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/pylint.py` & `returnn-1.20230415.10040/tests/pylint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/returnn-as-framework.py` & `returnn-1.20230415.10040/tests/returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/rf_utils.py` & `returnn-1.20230415.10040/tests/rf_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/spelling.dic` & `returnn-1.20230415.10040/tests/spelling.dic`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_Config.py` & `returnn-1.20230415.10040/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_Dataset.py` & `returnn-1.20230415.10040/tests/test_Dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_Fsa.py` & `returnn-1.20230415.10040/tests/test_Fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_GeneratingDataset.py` & `returnn-1.20230415.10040/tests/test_GeneratingDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_HDFDataset.py` & `returnn-1.20230415.10040/tests/test_HDFDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_LearningRateControl.py` & `returnn-1.20230415.10040/tests/test_LearningRateControl.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_Log.py` & `returnn-1.20230415.10040/tests/test_Log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_MultiProcDataset.py` & `returnn-1.20230415.10040/tests/test_MultiProcDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_PTDataset.py` & `returnn-1.20230415.10040/tests/test_PTDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_Pretrain.py` & `returnn-1.20230415.10040/tests/test_Pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_ResNet.py` & `returnn-1.20230415.10040/tests/test_ResNet.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_SprintDataset.py` & `returnn-1.20230415.10040/tests/test_SprintDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_SprintInterface.py` & `returnn-1.20230415.10040/tests/test_SprintInterface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_TFEngine.py` & `returnn-1.20230415.10040/tests/test_TFEngine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_TFNativeOp.py` & `returnn-1.20230415.10040/tests/test_TFNativeOp.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_TFNetworkLayer.py` & `returnn-1.20230415.10040/tests/test_TFNetworkLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_TFNetworkRecLayer.py` & `returnn-1.20230415.10040/tests/test_TFNetworkRecLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_TFNetworkSigProcLayer.py` & `returnn-1.20230415.10040/tests/test_TFNetworkSigProcLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_TFUpdater.py` & `returnn-1.20230415.10040/tests/test_TFUpdater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_TFUtil.py` & `returnn-1.20230415.10040/tests/test_TFUtil.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_TF_determinism.py` & `returnn-1.20230415.10040/tests/test_TF_determinism.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_TaskSystem.py` & `returnn-1.20230415.10040/tests/test_TaskSystem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_TaskSystem_SharedMem.py` & `returnn-1.20230415.10040/tests/test_TaskSystem_SharedMem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_TranslationDataset.py` & `returnn-1.20230415.10040/tests/test_TranslationDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_Util.py` & `returnn-1.20230415.10040/tests/test_Util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_demos.py` & `returnn-1.20230415.10040/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_fork_exec.py` & `returnn-1.20230415.10040/tests/test_fork_exec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_hdf_dump.py` & `returnn-1.20230415.10040/tests/test_hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_rf_array.py` & `returnn-1.20230415.10040/tests/test_rf_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_rf_attention.py` & `returnn-1.20230415.10040/tests/test_rf_attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_rf_base.py` & `returnn-1.20230415.10040/tests/test_rf_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_rf_container.py` & `returnn-1.20230415.10040/tests/test_rf_container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_rf_normalization.py` & `returnn-1.20230415.10040/tests/test_rf_normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_tensor.py` & `returnn-1.20230415.10040/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_tools.py` & `returnn-1.20230415.10040/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_torch_frontend.py` & `returnn-1.20230415.10040/tests/test_torch_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tests/test_torch_internal_frontend.py` & `returnn-1.20230415.10040/tests/test_torch_internal_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/analyze-dataset-batches.py` & `returnn-1.20230415.10040/tools/analyze-dataset-batches.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/bliss-collect-seq-lens.py` & `returnn-1.20230415.10040/tools/bliss-collect-seq-lens.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/bliss-dump-text.py` & `returnn-1.20230415.10040/tools/bliss-dump-text.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/bliss-get-segment-names.py` & `returnn-1.20230415.10040/tools/bliss-get-segment-names.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/bliss-to-ogg-zip.py` & `returnn-1.20230415.10040/tools/bliss-to-ogg-zip.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/bpe-create-lexicon.py` & `returnn-1.20230415.10040/tools/bpe-create-lexicon.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/calculate-word-error-rate.py` & `returnn-1.20230415.10040/tools/calculate-word-error-rate.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/cleanup-old-models.py` & `returnn-1.20230415.10040/tools/cleanup-old-models.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/collect-orth-symbols.py` & `returnn-1.20230415.10040/tools/collect-orth-symbols.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/collect-words.py` & `returnn-1.20230415.10040/tools/collect-words.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/compile_native_op.py` & `returnn-1.20230415.10040/tools/compile_native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/compile_tf_graph.py` & `returnn-1.20230415.10040/tools/compile_tf_graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/debug-dump-search-scores.py` & `returnn-1.20230415.10040/tools/debug-dump-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/debug-plot-search-scores.py` & `returnn-1.20230415.10040/tools/debug-plot-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/dump-dataset-raw-strings.py` & `returnn-1.20230415.10040/tools/dump-dataset-raw-strings.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/dump-dataset.py` & `returnn-1.20230415.10040/tools/dump-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/dump-forward-stats.py` & `returnn-1.20230415.10040/tools/dump-forward-stats.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/dump-forward.py` & `returnn-1.20230415.10040/tools/dump-forward.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/dump-network-json.py` & `returnn-1.20230415.10040/tools/dump-network-json.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/dump-pickle.py` & `returnn-1.20230415.10040/tools/dump-pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/extract_state_tying_from_dataset.py` & `returnn-1.20230415.10040/tools/extract_state_tying_from_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/get-attention-weights.py` & `returnn-1.20230415.10040/tools/get-attention-weights.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/get-best-model-epoch.py` & `returnn-1.20230415.10040/tools/get-best-model-epoch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/hdf_dump.py` & `returnn-1.20230415.10040/tools/hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/hdf_dump_translation_dataset.py` & `returnn-1.20230415.10040/tools/hdf_dump_translation_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/import-blocks-mt-model.py` & `returnn-1.20230415.10040/tools/import-blocks-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/import-t2t-mt-model.py` & `returnn-1.20230415.10040/tools/import-t2t-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/lattice_rescorer/Makefile` & `returnn-1.20230415.10040/tools/lattice_rescorer/Makefile`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/lattice_rescorer/README.md` & `returnn-1.20230415.10040/tools/lattice_rescorer/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/lattice_rescorer/example/README.md` & `returnn-1.20230415.10040/tools/lattice_rescorer/example/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config` & `returnn-1.20230415.10040/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config` & `returnn-1.20230415.10040/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/lattice_rescorer/example/rescore_lattice.sh` & `returnn-1.20230415.10040/tools/lattice_rescorer/example/rescore_lattice.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/lattice_rescorer/file.h` & `returnn-1.20230415.10040/tools/lattice_rescorer/file.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/lattice_rescorer/htklatticerescorer.cc` & `returnn-1.20230415.10040/tools/lattice_rescorer/htklatticerescorer.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/lattice_rescorer/htklatticerescorer.h` & `returnn-1.20230415.10040/tools/lattice_rescorer/htklatticerescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/lattice_rescorer/main.cc` & `returnn-1.20230415.10040/tools/lattice_rescorer/main.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/lattice_rescorer/rescorer.h` & `returnn-1.20230415.10040/tools/lattice_rescorer/rescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/lattice_rescorer/vocabulary.cc` & `returnn-1.20230415.10040/tools/lattice_rescorer/vocabulary.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/lattice_rescorer/vocabulary.h` & `returnn-1.20230415.10040/tools/lattice_rescorer/vocabulary.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/tf_avg_checkpoints.py` & `returnn-1.20230415.10040/tools/tf_avg_checkpoints.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/tf_inspect_checkpoint.py` & `returnn-1.20230415.10040/tools/tf_inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230414.234522/tools/tf_inspect_summary_log.py` & `returnn-1.20230415.10040/tools/tf_inspect_summary_log.py`

 * *Files identical despite different names*

