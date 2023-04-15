# Comparing `tmp/flgo-0.0.8.tar.gz` & `tmp/flgo-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flgo-0.0.8.tar", last modified: Thu Apr  6 17:47:50 2023, max compression
+gzip compressed data, was "flgo-0.0.9.tar", last modified: Sat Apr 15 17:18:20 2023, max compression
```

## Comparing `flgo-0.0.8.tar` & `flgo-0.0.9.tar`

### file list

```diff
@@ -1,190 +1,279 @@
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.993871 flgo-0.0.8/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1091 2023-03-21 13:46:37.000000 flgo-0.0.8/LICENSE
--rw-rw-r--   0 wz        (1001) wz        (1001)      485 2023-04-06 17:47:49.993871 flgo-0.0.8/PKG-INFO
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-21 13:46:37.000000 flgo-0.0.8/README.md
--rw-rw-r--   0 wz        (1001) wz        (1001)      590 2023-04-06 17:47:34.000000 flgo-0.0.8/pyproject.toml
--rw-rw-r--   0 wz        (1001) wz        (1001)       38 2023-04-06 17:47:49.993871 flgo-0.0.8/setup.cfg
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.981871 flgo-0.0.8/src/
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.985871 flgo-0.0.8/src/flgo/
--rw-rw-r--   0 wz        (1001) wz        (1001)      635 2023-04-06 17:45:35.000000 flgo-0.0.8/src/flgo/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/algorithm/
--rw-rw-r--   0 wz        (1001) wz        (1001)     3749 2023-04-06 17:45:35.000000 flgo-0.0.8/src/flgo/algorithm/TiFL.py
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-06 17:45:35.000000 flgo-0.0.8/src/flgo/algorithm/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3337 2023-04-06 17:45:35.000000 flgo-0.0.8/src/flgo/algorithm/afl.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2383 2023-04-06 17:45:35.000000 flgo-0.0.8/src/flgo/algorithm/fedasync.py
--rw-rw-r--   0 wz        (1001) wz        (1001)       86 2023-04-06 17:45:35.000000 flgo-0.0.8/src/flgo/algorithm/fedavg.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    31560 2023-04-06 17:45:35.000000 flgo-0.0.8/src/flgo/algorithm/fedbase.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2554 2023-04-06 17:45:35.000000 flgo-0.0.8/src/flgo/algorithm/fedbuff.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2258 2023-04-06 17:45:35.000000 flgo-0.0.8/src/flgo/algorithm/fedfa.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3381 2023-04-06 17:45:35.000000 flgo-0.0.8/src/flgo/algorithm/fedfv.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2690 2023-04-06 17:45:35.000000 flgo-0.0.8/src/flgo/algorithm/fedmgda+.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1364 2023-04-06 17:45:35.000000 flgo-0.0.8/src/flgo/algorithm/fedprox.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1800 2023-04-06 17:45:35.000000 flgo-0.0.8/src/flgo/algorithm/mifa.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1478 2023-04-06 17:45:35.000000 flgo-0.0.8/src/flgo/algorithm/powerofchoice.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1282 2023-04-06 17:45:35.000000 flgo-0.0.8/src/flgo/algorithm/qfedavg.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3396 2023-04-06 17:45:35.000000 flgo-0.0.8/src/flgo/algorithm/scaffold.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    11512 2023-04-06 17:45:35.000000 flgo-0.0.8/src/flgo/algorithm/vflbase.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1920 2023-04-06 17:45:35.000000 flgo-0.0.8/src/flgo/benchmark/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    15858 2023-04-06 17:45:35.000000 flgo-0.0.8/src/flgo/benchmark/base.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/cifar100_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1526 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/cifar100_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      845 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/cifar100_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/cifar100_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      957 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/cifar100_classification/model/cnn.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     5298 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/cifar100_classification/model/resnet18.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/cifar10_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1690 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/cifar10_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      829 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/cifar10_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/cifar10_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      895 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/cifar10_classification/model/cnn.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      897 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/cifar10_classification/model/mlp.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/citeseer_link_prediction/
--rw-rw-r--   0 wz        (1001) wz        (1001)       82 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/citeseer_link_prediction/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      748 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/citeseer_link_prediction/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/citeseer_link_prediction/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      825 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/citeseer_link_prediction/model/GCN.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/citeseer_node_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)       86 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/citeseer_node_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      807 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/citeseer_node_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/citeseer_node_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      727 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/citeseer_node_classification/model/GCN.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/cora_link_prediction/
--rw-rw-r--   0 wz        (1001) wz        (1001)       78 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/cora_link_prediction/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      736 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/cora_link_prediction/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/cora_link_prediction/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      825 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/cora_link_prediction/model/GCN.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/cora_node_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)       82 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/cora_node_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      794 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/cora_node_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/cora_node_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      727 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/cora_node_classification/model/GCN.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      730 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/cora_node_classification/model/GraphSAGE_1.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     4070 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/cora_node_classification/model/GraphSage.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/emnist_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      195 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/emnist_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1205 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/emnist_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/emnist_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1037 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/emnist_classification/model/cnn.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      709 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/emnist_classification/model/mlp.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/enzymes_graph_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)       86 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/enzymes_graph_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      748 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/enzymes_graph_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/enzymes_graph_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1258 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/enzymes_graph_classification/model/GCN.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1581 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/enzymes_graph_classification/model/GIN.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/fashion_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      194 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/fashion_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      818 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/fashion_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/fashion_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      578 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/fashion_classification/model/lr.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/femnist_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/femnist_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     5751 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/femnist_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/leaf_reddit/
--rw-rw-r--   0 wz        (1001) wz        (1001)       87 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/leaf_reddit/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    10075 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/leaf_reddit/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/leaf_reddit/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      980 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/leaf_reddit/model/stackedlstm.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/leaf_sent140/
--rw-rw-r--   0 wz        (1001) wz        (1001)       86 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/leaf_sent140/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    11324 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/leaf_sent140/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/leaf_sent140/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1278 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/leaf_sent140/model/stackedlstm.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/mnist_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1668 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/mnist_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      809 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/mnist_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/mnist_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1031 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/mnist_classification/model/cnn.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      801 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/mnist_classification/model/mlp.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/mutag_graph_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)       84 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/mutag_graph_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      742 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/mutag_graph_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/mutag_graph_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1260 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/mutag_graph_classification/model/GCN.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/pubmed_link_prediction/
--rw-rw-r--   0 wz        (1001) wz        (1001)       80 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/pubmed_link_prediction/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      742 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/pubmed_link_prediction/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/pubmed_link_prediction/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      824 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/pubmed_link_prediction/model/GCN.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/pubmed_node_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)       84 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/pubmed_node_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      801 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/pubmed_node_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/pubmed_node_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      726 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/pubmed_node_classification/model/GCN.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/shakespeare_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      100 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/shakespeare_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    15270 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/shakespeare_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.989871 flgo-0.0.8/src/flgo/benchmark/shakespeare_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     2169 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/shakespeare_classification/model/stackedlstm.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.993871 flgo-0.0.8/src/flgo/benchmark/svhn_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)      195 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/svhn_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1222 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/svhn_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.993871 flgo-0.0.8/src/flgo/benchmark/svhn_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      895 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/svhn_classification/model/cnn.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      897 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/svhn_classification/model/mlp.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.993871 flgo-0.0.8/src/flgo/benchmark/synthetic_regression/
--rw-rw-r--   0 wz        (1001) wz        (1001)       76 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/synthetic_regression/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     3918 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/synthetic_regression/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.993871 flgo-0.0.8/src/flgo/benchmark/synthetic_regression/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)      555 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/synthetic_regression/model/lr.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.993871 flgo-0.0.8/src/flgo/benchmark/toolkits/
--rw-rw-r--   0 wz        (1001) wz        (1001)      150 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/toolkits/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.993871 flgo-0.0.8/src/flgo/benchmark/toolkits/cv/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/toolkits/cv/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.993871 flgo-0.0.8/src/flgo/benchmark/toolkits/cv/centralize/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/toolkits/cv/centralize/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.993871 flgo-0.0.8/src/flgo/benchmark/toolkits/cv/horizontal/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/toolkits/cv/horizontal/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     9110 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/toolkits/cv/horizontal/image_classification.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.993871 flgo-0.0.8/src/flgo/benchmark/toolkits/cv/vertical/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/toolkits/cv/vertical/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.993871 flgo-0.0.8/src/flgo/benchmark/toolkits/graph/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/toolkits/graph/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.993871 flgo-0.0.8/src/flgo/benchmark/toolkits/graph/horizontal/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/toolkits/graph/horizontal/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     5245 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/toolkits/graph/horizontal/graph_classification.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     7700 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/toolkits/graph/horizontal/link_prediction.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     7337 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/toolkits/graph/horizontal/node_classification.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.993871 flgo-0.0.8/src/flgo/benchmark/toolkits/nlp/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/toolkits/nlp/__init__.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.993871 flgo-0.0.8/src/flgo/benchmark/toolkits/nlp/horizontal/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/toolkits/nlp/horizontal/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/toolkits/nlp/horizontal/text_prediction.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    20144 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/toolkits/partition.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.993871 flgo-0.0.8/src/flgo/benchmark/toolkits/tabular/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/toolkits/tabular/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     2465 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/toolkits/visualization.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.993871 flgo-0.0.8/src/flgo/benchmark/vertical_mnist_classification/
--rw-rw-r--   0 wz        (1001) wz        (1001)       87 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/vertical_mnist_classification/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     7193 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/benchmark/vertical_mnist_classification/core.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.993871 flgo-0.0.8/src/flgo/benchmark/vertical_mnist_classification/model/
--rw-rw-r--   0 wz        (1001) wz        (1001)     1162 2023-04-06 17:45:37.000000 flgo-0.0.8/src/flgo/benchmark/vertical_mnist_classification/model/mlp.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.993871 flgo-0.0.8/src/flgo/experiment/
--rw-rw-r--   0 wz        (1001) wz        (1001)       62 2023-04-06 17:45:35.000000 flgo-0.0.8/src/flgo/experiment/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    26973 2023-04-06 17:45:35.000000 flgo-0.0.8/src/flgo/experiment/analyzer.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     6628 2023-04-06 17:45:35.000000 flgo-0.0.8/src/flgo/experiment/device_scheduler.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.993871 flgo-0.0.8/src/flgo/experiment/logger/
--rw-rw-r--   0 wz        (1001) wz        (1001)    87170 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/experiment/logger/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    36840 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/experiment/logger/config.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    59394 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/experiment/logger/handlers.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1587 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/experiment/logger/simple_logger.py
--rw-rw-r--   0 wz        (1001) wz        (1001)      967 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/experiment/logger/tune_logger.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1023 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/experiment/logger/vertical_logger.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.993871 flgo-0.0.8/src/flgo/simulator/
--rw-rw-r--   0 wz        (1001) wz        (1001)     2981 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/simulator/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    23835 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/simulator/base.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    16615 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/simulator/default_simulator.py
--rw-rw-r--   0 wz        (1001) wz        (1001)     1030 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/simulator/my_simulator.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    17522 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/simulator/phone_simulator.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.993871 flgo-0.0.8/src/flgo/utils/
--rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/utils/__init__.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    40666 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/utils/fflow.py
--rw-rw-r--   0 wz        (1001) wz        (1001)    28136 2023-04-06 17:45:36.000000 flgo-0.0.8/src/flgo/utils/fmodule.py
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.985871 flgo-0.0.8/src/flgo.egg-info/
--rw-rw-r--   0 wz        (1001) wz        (1001)      485 2023-04-06 17:47:49.000000 flgo-0.0.8/src/flgo.egg-info/PKG-INFO
--rw-rw-r--   0 wz        (1001) wz        (1001)     5861 2023-04-06 17:47:49.000000 flgo-0.0.8/src/flgo.egg-info/SOURCES.txt
--rw-rw-r--   0 wz        (1001) wz        (1001)        1 2023-04-06 17:47:49.000000 flgo-0.0.8/src/flgo.egg-info/dependency_links.txt
--rw-rw-r--   0 wz        (1001) wz        (1001)        5 2023-04-06 17:47:49.000000 flgo-0.0.8/src/flgo.egg-info/top_level.txt
-drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-06 17:47:49.993871 flgo-0.0.8/tests/
--rw-rw-r--   0 wz        (1001) wz        (1001)      947 2023-03-21 13:46:37.000000 flgo-0.0.8/tests/test.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.677821 flgo-0.0.9/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1091 2023-03-21 13:46:37.000000 flgo-0.0.9/LICENSE
+-rw-rw-r--   0 wz        (1001) wz        (1001)      485 2023-04-15 17:18:20.677821 flgo-0.0.9/PKG-INFO
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-03-21 13:46:37.000000 flgo-0.0.9/README.md
+-rw-rw-r--   0 wz        (1001) wz        (1001)      590 2023-04-15 17:17:37.000000 flgo-0.0.9/pyproject.toml
+-rw-rw-r--   0 wz        (1001) wz        (1001)       38 2023-04-15 17:18:20.677821 flgo-0.0.9/setup.cfg
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.653821 flgo-0.0.9/src/
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.661821 flgo-0.0.9/src/flgo/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      635 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.665821 flgo-0.0.9/src/flgo/algorithm/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3749 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/algorithm/TiFL.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/algorithm/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3362 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/algorithm/afl.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     6959 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/algorithm/clustered_sampling.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2383 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/algorithm/fedasync.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)       86 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/algorithm/fedavg.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      711 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/algorithm/fedavgm.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    32159 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/algorithm/fedbase.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2554 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/algorithm/fedbuff.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2258 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/algorithm/fedfa.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3381 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/algorithm/fedfv.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     7213 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/algorithm/fedmf.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2690 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/algorithm/fedmgda+.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1364 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/algorithm/fedprox.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1800 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/algorithm/mifa.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1528 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/algorithm/powerofchoice.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1282 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/algorithm/qfedavg.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3421 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/algorithm/scaffold.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     9202 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/algorithm/sesorec.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    15663 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/algorithm/vflbase.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.665821 flgo-0.0.9/src/flgo/benchmark/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2327 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/benchmark/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    15990 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/benchmark/base.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.665821 flgo-0.0.9/src/flgo/benchmark/ciao_recommendation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      202 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/benchmark/ciao_recommendation/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      827 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/benchmark/ciao_recommendation/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.665821 flgo-0.0.9/src/flgo/benchmark/ciao_recommendation/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      848 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/ciao_recommendation/model/mf.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.665821 flgo-0.0.9/src/flgo/benchmark/cifar100_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1734 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/benchmark/cifar100_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      862 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/benchmark/cifar100_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.665821 flgo-0.0.9/src/flgo/benchmark/cifar100_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      957 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/cifar100_classification/model/cnn.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     5298 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/cifar100_classification/model/resnet18.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.665821 flgo-0.0.9/src/flgo/benchmark/cifar10_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1870 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/benchmark/cifar10_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      882 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/benchmark/cifar10_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.665821 flgo-0.0.9/src/flgo/benchmark/cifar10_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      895 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/cifar10_classification/model/cnn.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      897 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/cifar10_classification/model/mlp.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.665821 flgo-0.0.9/src/flgo/benchmark/citeseer_link_prediction/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      368 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/benchmark/citeseer_link_prediction/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      994 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/benchmark/citeseer_link_prediction/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.665821 flgo-0.0.9/src/flgo/benchmark/citeseer_link_prediction/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      825 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/citeseer_link_prediction/model/GCN.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.665821 flgo-0.0.9/src/flgo/benchmark/citeseer_node_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      372 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/benchmark/citeseer_node_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      828 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/benchmark/citeseer_node_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.665821 flgo-0.0.9/src/flgo/benchmark/citeseer_node_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      727 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/citeseer_node_classification/model/GCN.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.665821 flgo-0.0.9/src/flgo/benchmark/coco_detection/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      265 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/benchmark/coco_detection/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     6869 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/benchmark/coco_detection/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.665821 flgo-0.0.9/src/flgo/benchmark/coco_detection/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     9129 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/coco_detection/model/FasterRCNN.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/coco_detection/model/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.665821 flgo-0.0.9/src/flgo/benchmark/coco_segmentation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      271 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/coco_segmentation/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     8043 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/coco_segmentation/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.665821 flgo-0.0.9/src/flgo/benchmark/coco_segmentation/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/coco_segmentation/model/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      521 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/coco_segmentation/model/fcn_resnet50.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1459 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/coco_segmentation/model/unet.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.665821 flgo-0.0.9/src/flgo/benchmark/cora_link_prediction/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      364 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/cora_link_prediction/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      986 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/cora_link_prediction/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.665821 flgo-0.0.9/src/flgo/benchmark/cora_link_prediction/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      853 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/cora_link_prediction/model/GCN.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.665821 flgo-0.0.9/src/flgo/benchmark/cora_node_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      368 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/cora_node_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      820 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/cora_node_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.665821 flgo-0.0.9/src/flgo/benchmark/cora_node_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      727 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/cora_node_classification/model/GCN.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      730 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/cora_node_classification/model/GraphSAGE_1.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     4070 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/cora_node_classification/model/GraphSage.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.665821 flgo-0.0.9/src/flgo/benchmark/emnist_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      357 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/emnist_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1205 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/emnist_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.665821 flgo-0.0.9/src/flgo/benchmark/emnist_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      875 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/emnist_classification/model/cnn.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      709 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/emnist_classification/model/mlp.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.665821 flgo-0.0.9/src/flgo/benchmark/enzymes_graph_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      366 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/enzymes_graph_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      848 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/enzymes_graph_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/enzymes_graph_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1258 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/enzymes_graph_classification/model/GCN.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1581 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/enzymes_graph_classification/model/GIN.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/epinions_recommendation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      202 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/epinions_recommendation/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      839 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/epinions_recommendation/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/epinions_recommendation/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      848 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/epinions_recommendation/model/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      938 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/epinions_recommendation/model/mf.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/fashion_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      356 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/fashion_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      833 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/fashion_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/fashion_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      578 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/fashion_classification/model/lr.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/femnist_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      358 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/femnist_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     5719 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/femnist_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/femnist_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/femnist_classification/model/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      875 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/femnist_classification/model/cnn.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/leaf_reddit/
+-rw-rw-r--   0 wz        (1001) wz        (1001)       87 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/leaf_reddit/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    10067 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/leaf_reddit/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/leaf_reddit/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      980 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/leaf_reddit/model/stackedlstm.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/leaf_sent140/
+-rw-rw-r--   0 wz        (1001) wz        (1001)       86 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/leaf_sent140/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    11316 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/leaf_sent140/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/leaf_sent140/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1278 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/leaf_sent140/model/stackedlstm.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/local_movielens_recommendation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      193 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/local_movielens_recommendation/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      845 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/local_movielens_recommendation/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/local_movielens_recommendation/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1748 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/local_movielens_recommendation/model/mf.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/mnist_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1850 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/mnist_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      826 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/mnist_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/mnist_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1031 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/mnist_classification/model/cnn.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      801 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/mnist_classification/model/mlp.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/movielens_recommendation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      202 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/movielens_recommendation/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      841 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/movielens_recommendation/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/movielens_recommendation/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/movielens_recommendation/model/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      787 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/movielens_recommendation/model/mf.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/mutag_graph_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      362 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/mutag_graph_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      844 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/mutag_graph_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/mutag_graph_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1260 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/mutag_graph_classification/model/GCN.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/pubmed_link_prediction/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      366 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/pubmed_link_prediction/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      990 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/pubmed_link_prediction/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/pubmed_link_prediction/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      824 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/pubmed_link_prediction/model/GCN.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/pubmed_node_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      370 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/pubmed_node_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      826 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/pubmed_node_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/pubmed_node_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      726 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/pubmed_node_classification/model/GCN.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/sbdataset_segmentation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      269 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/sbdataset_segmentation/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     6616 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/sbdataset_segmentation/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/sbdataset_segmentation/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/sbdataset_segmentation/model/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      521 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/sbdataset_segmentation/model/fcn_resnet50.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1459 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/sbdataset_segmentation/model/unet.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/shakespeare_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      262 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/shakespeare_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    15262 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/shakespeare_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/shakespeare_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2169 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/shakespeare_classification/model/stackedlstm.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/social_splitted_ciao/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/social_splitted_ciao/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     9422 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/social_splitted_ciao/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/social_splitted_ciao/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/social_splitted_ciao/model/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/social_splitted_ciaodvd/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/social_splitted_ciaodvd/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     9159 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/social_splitted_ciaodvd/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/social_splitted_douban/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/social_splitted_douban/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     8287 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/social_splitted_douban/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/social_splitted_epinions/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/social_splitted_epinions/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     9343 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/social_splitted_epinions/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/social_splitted_epinions/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/social_splitted_epinions/model/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.669821 flgo-0.0.9/src/flgo/benchmark/social_splitted_filmtrust/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/social_splitted_filmtrust/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     9196 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/social_splitted_filmtrust/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.673821 flgo-0.0.9/src/flgo/benchmark/svhn_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      355 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/svhn_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      966 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/svhn_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.673821 flgo-0.0.9/src/flgo/benchmark/svhn_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      895 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/svhn_classification/model/cnn.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      897 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/svhn_classification/model/mlp.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.673821 flgo-0.0.9/src/flgo/benchmark/synthetic_regression/
+-rw-rw-r--   0 wz        (1001) wz        (1001)       78 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/synthetic_regression/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3881 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/synthetic_regression/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.673821 flgo-0.0.9/src/flgo/benchmark/synthetic_regression/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      555 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/synthetic_regression/model/lr.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.673821 flgo-0.0.9/src/flgo/benchmark/toolkits/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      656 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/toolkits/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.673821 flgo-0.0.9/src/flgo/benchmark/toolkits/cv/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/toolkits/cv/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.673821 flgo-0.0.9/src/flgo/benchmark/toolkits/cv/classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)    10387 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/toolkits/cv/classification/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.673821 flgo-0.0.9/src/flgo/benchmark/toolkits/cv/detection/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3782 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/toolkits/cv/detection/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     6637 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/toolkits/cv/detection/coco_eval.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     9180 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/toolkits/cv/detection/coco_utils.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2636 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/toolkits/cv/detection/presets.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    23926 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/toolkits/cv/detection/transforms.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     8962 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/toolkits/cv/detection/utils.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.673821 flgo-0.0.9/src/flgo/benchmark/toolkits/cv/segmentation/
+-rw-rw-r--   0 wz        (1001) wz        (1001)    10990 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/toolkits/cv/segmentation/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3943 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/toolkits/cv/segmentation/coco_utils.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1314 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/toolkits/cv/segmentation/presets.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     2797 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/toolkits/cv/segmentation/transforms.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    10779 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/toolkits/cv/segmentation/utils.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.673821 flgo-0.0.9/src/flgo/benchmark/toolkits/graph/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/toolkits/graph/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.673821 flgo-0.0.9/src/flgo/benchmark/toolkits/graph/graph_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     6774 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/toolkits/graph/graph_classification/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.673821 flgo-0.0.9/src/flgo/benchmark/toolkits/graph/link_prediction/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     8345 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/toolkits/graph/link_prediction/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.673821 flgo-0.0.9/src/flgo/benchmark/toolkits/graph/node_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)    10959 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/toolkits/graph/node_classification/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.673821 flgo-0.0.9/src/flgo/benchmark/toolkits/nlp/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/toolkits/nlp/__init__.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.673821 flgo-0.0.9/src/flgo/benchmark/toolkits/nlp/text_prediction/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/toolkits/nlp/text_prediction/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    22318 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/toolkits/partition.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.673821 flgo-0.0.9/src/flgo/benchmark/toolkits/rec/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/toolkits/rec/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     8776 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/toolkits/rec/datasets.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.673821 flgo-0.0.9/src/flgo/benchmark/toolkits/rec/rating_prediction/
+-rw-rw-r--   0 wz        (1001) wz        (1001)    11628 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/toolkits/rec/rating_prediction/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      425 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/toolkits/rec/utils.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.673821 flgo-0.0.9/src/flgo/benchmark/toolkits/tabular/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/toolkits/tabular/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     7425 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/toolkits/visualization.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.673821 flgo-0.0.9/src/flgo/benchmark/vertical_mnist_classification/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      260 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/vertical_mnist_classification/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     7165 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/vertical_mnist_classification/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.673821 flgo-0.0.9/src/flgo/benchmark/vertical_mnist_classification/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1162 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/vertical_mnist_classification/model/mlp.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.673821 flgo-0.0.9/src/flgo/benchmark/voc_detection/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      219 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/voc_detection/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      992 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/benchmark/voc_detection/core.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.673821 flgo-0.0.9/src/flgo/benchmark/voc_detection/model/
+-rw-rw-r--   0 wz        (1001) wz        (1001)    10832 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/voc_detection/model/FasterRCNN.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/voc_detection/model/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    32695 2023-04-15 17:15:53.000000 flgo-0.0.9/src/flgo/benchmark/voc_detection/model/yolov3.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.673821 flgo-0.0.9/src/flgo/experiment/
+-rw-rw-r--   0 wz        (1001) wz        (1001)       62 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/experiment/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    27104 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/experiment/analyzer.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     6651 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/experiment/device_scheduler.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.673821 flgo-0.0.9/src/flgo/experiment/logger/
+-rw-rw-r--   0 wz        (1001) wz        (1001)    87348 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/experiment/logger/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    36840 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/experiment/logger/config.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    59619 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/experiment/logger/handlers.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1612 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/experiment/logger/simple_logger.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)      967 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/experiment/logger/tune_logger.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1048 2023-04-15 17:15:52.000000 flgo-0.0.9/src/flgo/experiment/logger/vertical_logger.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.673821 flgo-0.0.9/src/flgo/simulator/
+-rw-rw-r--   0 wz        (1001) wz        (1001)     3083 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/simulator/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    23923 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/simulator/base.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    16663 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/simulator/default_simulator.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)     1030 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/simulator/my_simulator.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    17547 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/simulator/phone_simulator.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.677821 flgo-0.0.9/src/flgo/utils/
+-rw-rw-r--   0 wz        (1001) wz        (1001)        0 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/utils/__init__.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    42268 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/utils/fflow.py
+-rw-rw-r--   0 wz        (1001) wz        (1001)    28159 2023-04-15 17:15:51.000000 flgo-0.0.9/src/flgo/utils/fmodule.py
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.661821 flgo-0.0.9/src/flgo.egg-info/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      485 2023-04-15 17:18:20.000000 flgo-0.0.9/src/flgo.egg-info/PKG-INFO
+-rw-rw-r--   0 wz        (1001) wz        (1001)     9010 2023-04-15 17:18:20.000000 flgo-0.0.9/src/flgo.egg-info/SOURCES.txt
+-rw-rw-r--   0 wz        (1001) wz        (1001)        1 2023-04-15 17:18:20.000000 flgo-0.0.9/src/flgo.egg-info/dependency_links.txt
+-rw-rw-r--   0 wz        (1001) wz        (1001)        5 2023-04-15 17:18:20.000000 flgo-0.0.9/src/flgo.egg-info/top_level.txt
+drwxrwxr-x   0 wz        (1001) wz        (1001)        0 2023-04-15 17:18:20.677821 flgo-0.0.9/tests/
+-rw-rw-r--   0 wz        (1001) wz        (1001)      947 2023-03-21 13:46:37.000000 flgo-0.0.9/tests/test.py
```

### Comparing `flgo-0.0.8/LICENSE` & `flgo-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/pyproject.toml` & `flgo-0.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "setuptools>=61.0", 
 ]
 build-backend = "setuptools.build_meta"
 [project]
 name = "flgo"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Zheng Wang", email="zwang@stu.xmu.edu.cn" },
 ]
 description = "A Research-oriented FL Platform. "
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `flgo-0.0.8/src/flgo/__init__.py` & `flgo-0.0.9/src/flgo/__init__.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/algorithm/TiFL.py` & `flgo-0.0.9/src/flgo/algorithm/TiFL.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/algorithm/afl.py` & `flgo-0.0.9/src/flgo/algorithm/afl.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         lmbd = (1.0 / rho) * (1 - np.sum(np.asarray(u)[:rho]))
         for i in range(len(p)):
             res.append(max(p[i] + lmbd, 0))
         return res
 
     def global_test(self, flag='valid'):
         """
-        Validate accuracies and losses on clients' local datasets
+        Validate accuracies and losses on clients' local_movielens_recommendation datasets
         Args:
             flag: choose train data or valid data to evaluate
         Returns:
             metrics: a dict contains the lists of each metric_value of the clients
         """
         all_metrics = collections.defaultdict(list)
         for c in self.clients:
```

### Comparing `flgo-0.0.8/src/flgo/algorithm/fedasync.py` & `flgo-0.0.9/src/flgo/algorithm/fedasync.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/algorithm/fedbase.py` & `flgo-0.0.9/src/flgo/algorithm/fedbase.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 # The BasicParty
 class BasicParty:
     def __init__(self, *args, **kwargs):
         self.actions = {}  # the message-action map that is used to customize the communication process
         self.id = None  # the id for communicating
-        self._object_map = collections.defaultdict(lambda:None) # mapping objects according to their ids
+        self._object_map = {} # mapping objects according to their ids
 
     def register_action_to_mtype(self, action_name: str, mtype):
         r"""
         Register an existing method as the action corresponding to the message type.
 
         Args:
             action_name: the name of the instance method
@@ -97,23 +97,25 @@
         self has no attribute named party_names. Otherwise, parties will be extend to
         the attribute party_names of self.
         
         Args:
             parties (list): a list of objects
             parties_name (str): the name of attribute to store parties
 
-        Example::
+        Example:
+        ```python
             >>> a = BasicParty()
             >>> b = BasicParty()
             >>> c = BasicParty()
             >>> a.register_objects([b, c], 'parties')
             >>> a.parties # will be [b,c]
             >>> d = BasicParty()
             >>> a.register_objects([d], 'parties')
             >>> a.parties # will be [b,c,d]
+        ```
         """
         if type(parties) is not list:
             raise TypeError("parties should be a list")
         if not hasattr(self, parties_name):
             setattr(self, parties_name, parties)
         else:
             tmp = getattr(self, parties_name)
@@ -174,18 +176,19 @@
         self.id = -1
 
     def run(self):
         """
         Running the FL symtem where the global model is trained and evaluated iteratively.
         """
         self.gv.logger.time_start('Total Time Cost')
-        self.gv.logger.info("--------------Initial Evaluation--------------")
-        self.gv.logger.time_start('Eval Time Cost')
-        self.gv.logger.log_once()
-        self.gv.logger.time_end('Eval Time Cost')
+        if self.eval_interval>0:
+            self.gv.logger.info("--------------Initial Evaluation--------------")
+            self.gv.logger.time_start('Eval Time Cost')
+            self.gv.logger.log_once()
+            self.gv.logger.time_end('Eval Time Cost')
         while self.current_round <= self.num_rounds:
             self.gv.clock.step()
             # iterate
             updated = self.iterate()
             # using logger to evaluate the model if the model is updated
             if updated is True or updated is None:
                 self.gv.logger.info("--------------Round {}--------------".format(self.current_round))
@@ -282,15 +285,15 @@
             client_package (dict): the reply from the target object and
             will be 'None' if losing connection
         """
         return super(BasicServer, self).communicate_with(target_id, package)
 
     def pack(self, client_id, mtype=0, *args, **kwargs):
         r"""
-        Pack the necessary information for the client's local training.
+        Pack the necessary information for the client's local_movielens_recommendation training.
         Any operations of compression or encryption should be done here.
 
         Args:
             client_id (int): the id of the client to communicate with
             mtype: the message type
 
         Returns:
@@ -303,27 +306,27 @@
     def unpack(self, packages_received_from_clients):
         r"""
         Unpack the information from the received packages. Return models and losses as default.
 
         Args:
             packages_received_from_clients (list): a list of packages
 
-        Returns::
+        Returns:
             res (dict): collections.defaultdict that contains several lists of the clients' reply
         """
         if len(packages_received_from_clients) == 0: return collections.defaultdict(list)
         res = {pname: [] for pname in packages_received_from_clients[0]}
         for cpkg in packages_received_from_clients:
             for pname, pval in cpkg.items():
                 res[pname].append(pval)
         return res
 
     def global_lr_scheduler(self, current_round):
         r"""
-        Control the step size (i.e. learning rate) of local training
+        Control the step size (i.e. learning rate) of local_movielens_recommendation training
         Args:
             current_round (int): the current communication round
         """
         if self.lr_scheduler_type == -1:
             return
         elif self.lr_scheduler_type == 0:
             """eta_{round+1} = DecayRate * eta_{round}"""
@@ -343,32 +346,34 @@
         full sample, uniform sample without replacement, and MDSample
         with replacement. Particularly, if 'available' is in self.sample_option,
         the server will only sample from currently available clients.
 
         Returns:
             a list of the ids of the selected clients
 
-        Example::
+        Example:
+        ```python
             >>> selected_clients=self.sample()
             >>> selected_clients
             >>> # The selected_clients is a list of clients' ids
+        ```
         """
         all_clients = self.available_clients if 'available' in self.sample_option else [cid for cid in
                                                                                         range(self.num_clients)]
         # full sampling with unlimited communication resources of the server
         if 'full' in self.sample_option:
             return all_clients
         # sample clients
         elif 'uniform' in self.sample_option:
             # original sample proposed by fedavg
             selected_clients = list(
                 np.random.choice(all_clients, min(self.clients_per_round, len(all_clients)), replace=False)) if len(
                 all_clients) > 0 else []
         elif 'md' in self.sample_option:
-            # the default setting that is introduced by FedProx, where the clients are sampled with the probability in proportion to their local data sizes
+            # the default setting that is introduced by FedProx, where the clients are sampled with the probability in proportion to their local_movielens_recommendation data sizes
             local_data_vols = [self.clients[cid].datavol for cid in all_clients]
             total_data_vol = sum(local_data_vols)
             p = np.array(local_data_vols) / total_data_vol
             selected_clients = list(np.random.choice(all_clients, self.clients_per_round, replace=True, p=p)) if len(
                 all_clients) > 0 else []
         return selected_clients
 
@@ -383,22 +388,24 @@
         -------------------------------------------------------------------------------------------------------------------------
          weighted_scale                 |uniform (default)          |weighted_com (original fedavg)   |other
         ==========================================================================================================================
         N/K * Σpk * model_k             |1/K * Σmodel_k             |(1-Σpk) * w_old + Σpk * model_k  |Σ(pk/Σpk) * model_k
 
 
         Args:
-            models (list): a list of local models
+            models (list): a list of local_movielens_recommendation models
 
         Returns:
             the aggregated model
 
-        Example::
+        Example:
+        ```python
             >>> models = [m1, m2] # m1, m2 are models with the same architecture
             >>> m_new = self.aggregate(models)
+        ```
         """
         if len(models) == 0: return self.model
         local_data_vols = [c.datavol for c in self.clients]
         total_data_vol = sum(local_data_vols)
         if self.aggregation_option == 'weighted_scale':
             p = [1.0 * local_data_vols[cid] / total_data_vol for cid in self.received_clients]
             K = len(models)
@@ -414,15 +421,15 @@
             p = [1.0 * local_data_vols[cid] / total_data_vol for cid in self.received_clients]
             sump = sum(p)
             p = [pk / sump for pk in p]
             return fmodule._model_sum([model_k * pk for model_k, pk in zip(models, p)])
 
     def global_test(self, model=None, flag:str='valid'):
         r"""
-        Collect local testing result of all the clients.
+        Collect local_movielens_recommendation testing result of all the clients.
 
         Args:
             model (flgo.utils.fmodule.FModule|torch.nn.Module): the model to be sevaluated
             flag (str): choose the data to evaluate the model
 
         Returns:
             metrics (dict): a dict contains key-value pairs like (metric_name,
@@ -440,40 +447,41 @@
         r"""
         Evaluate the model on the test dataset owned by the server.
 
         Args:
             model (flgo.utils.fmodule.FModule): the model need to be evaluated
             flag (str): choose the data to evaluate the model
 
-        Returns::
+        Returns:
             metrics (dict): the dict contains the evaluating results
         """
         if model is None: model = self.model
         dataset = getattr(self, flag+'_data') if hasattr(self, flag+'_data') else None
         if dataset is None:
             return {}
         else:
-            return self.calculator.test(model, dataset, batch_size=self.option['test_batch_size'],
+            return self.calculator.test(model, dataset, batch_size=min(self.option['test_batch_size'], len(dataset)),
                                         num_workers=self.option['num_workers'], pin_memory=self.option['pin_memory'])
 
     def init_algo_para(self, algo_para: dict):
         """
         Initialize the algorithm-dependent hyper-parameters for the server and all the clients.
 
         Args:
             algo_paras (dict): the dict that defines the hyper-parameters (i.e. name, value and type) for the algorithm.
 
-        Example::
+        Example:
+        ```python
             >>> # s is an instance of Server and s.clients are instances of Client
             >>> s.u # will raise error
             >>> [c.u for c in s.clients] # will raise errors too
             >>> s.init_algo_para({'u': 0.1})
             >>> s.u # will be 0.1
             >>> [c.u for c in s.clients] # will be [0.1, 0.1,..., 0.1]
-
+        ```
         Note:
             Once `option['algo_para']` is not `None`, the value of the pre-defined hyperparameters will be replaced by the list of values in `option['algo_para']`,
             which requires the length of `option['algo_para']` is equal to the length of `algo_paras`
         """
         self.algo_para = algo_para
         if len(self.algo_para) == 0: return
         # initialize algorithm-dependent hyperparameters from the input options
@@ -537,21 +545,21 @@
         self.dropped_clients = []
 
 
 class BasicClient(BasicParty):
     def __init__(self, option={}):
         super().__init__()
         self.id = None
-        # create local dataset
+        # create local_movielens_recommendation dataset
         self.data_loader = None
         self.test_data = None
         self.valid_data = None
         self.train_data = None
         self.model = None
-        # local calculator
+        # local_movielens_recommendation calculator
         self.device = self.gv.apply_for_device()
         self.calculator = self.gv.TaskCalculator(self.device, option['optimizer'])
         # hyper-parameters for training
         self.optimizer_name = option['optimizer']
         self.learning_rate = option['learning_rate']
         self.momentum = option['momentum']
         self.weight_decay = option['weight_decay']
@@ -571,16 +579,16 @@
         self.option = option
         self.actions = {0: self.reply}
 
     @ss.with_completeness
     @fmodule.with_multi_gpus
     def train(self, model):
         r"""
-        Standard local training procedure. Train the transmitted model with
-        local training dataset.
+        Standard local_movielens_recommendation training procedure. Train the transmitted model with
+        local_movielens_recommendation training dataset.
 
         Args:
             model (FModule): the global model
         """
         model.train()
         optimizer = self.calculator.get_optimizer(model, lr=self.learning_rate, weight_decay=self.weight_decay,
                                                   momentum=self.momentum)
@@ -604,15 +612,15 @@
             flag (str): choose the data to evaluate the model
 
         Returns:
             metric (dict): the evaluating results (e.g. metric = {'loss':1.02})
         """
         dataset = getattr(self, flag + '_data') if hasattr(self, flag + '_data') else None
         if dataset is None: return {}
-        return self.calculator.test(model, dataset, self.test_batch_size, self.option['num_workers'])
+        return self.calculator.test(model, dataset, min(self.test_batch_size, len(dataset)), self.option['num_workers'])
 
 
     def unpack(self, received_pkg):
         r"""
         Unpack the package received from the server
 
         Args:
@@ -622,15 +630,15 @@
             the unpacked information
         """
         # unpack the received package
         return received_pkg['model']
 
     def reply(self, svr_pkg):
         r"""
-        Reply a package to the server. The whole local procedure should be defined here.
+        Reply a package to the server. The whole local_movielens_recommendation procedure should be defined here.
         The standard form consists of three procedure: unpacking the
         server_package to obtain the global model, training the global model,
         and finally packing the updated model into client_package.
 
         Args:
             svr_pkg (dict): the package received from the server
 
@@ -683,27 +691,27 @@
             True if the client is working
         """
 
         return self.gv.simulator.client_states[self.id] == 'working'
 
     def train_loss(self, model):
         r"""
-        Get the loss value of the model on local training data
+        Get the loss value of the model on local_movielens_recommendation training data
 
         Args:
             model (flgo.utils.fmodule.FModule|torch.nn.Module): model
 
         Returns:
             the training loss of model on self's training data
         """
         return self.test(model, 'train')['loss']
 
     def valid_loss(self, model):
         r"""
-        Get the loss value of the model on local validating data
+        Get the loss value of the model on local_movielens_recommendation validating data
 
         Args:
             model (flgo.utils.fmodule.FModule|torch.nn.Module): model
 
         Returns:
             the validation loss of model on self's validation data
         """
@@ -715,34 +723,34 @@
         """
         self.register_objects([server], 'server_list')
         if server is not None:
             self.server = server
 
     def set_local_epochs(self, epochs=None):
         r"""
-        Set local training epochs
+        Set local_movielens_recommendation training epochs
         """
         if epochs is None: return
         self.epochs = epochs
         self.num_steps = self.epochs * math.ceil(len(self.train_data) / self.batch_size)
         return
 
     def set_batch_size(self, batch_size=None):
         r"""
-        Set local training batch size
+        Set local_movielens_recommendation training batch size
 
         Args:
             batch_size (int): the training batch size
         """
         if batch_size is None: return
         self.batch_size = batch_size
 
     def set_learning_rate(self, lr=None):
         """
-        Set the learning rate of local training
+        Set the learning rate of local_movielens_recommendation training
         Args:
             lr (float): a real number
         """
         self.learning_rate = lr if lr else self.learning_rate
 
     def get_time_response(self):
         """
@@ -762,15 +770,15 @@
         try:
             batch_data = next(self.data_loader)
         except Exception as e:
             self.data_loader = iter(self.calculator.get_dataloader(self.train_data, batch_size=self.batch_size,
                                                                    num_workers=self.loader_num_workers,
                                                                    pin_memory=self.option['pin_memory']))
             batch_data = next(self.data_loader)
-        # clear local DataLoader when finishing local training
+        # clear local_movielens_recommendation DataLoader when finishing local_movielens_recommendation training
         self.current_steps = (self.current_steps + 1) % self.num_steps
         if self.current_steps == 0: self.data_loader = None
         return batch_data
 
     def update_device(self, dev):
         """
         Update running-time GPU device to dev
```

### Comparing `flgo-0.0.8/src/flgo/algorithm/fedbuff.py` & `flgo-0.0.9/src/flgo/algorithm/fedbuff.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/algorithm/fedfa.py` & `flgo-0.0.9/src/flgo/algorithm/fedfa.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/algorithm/fedfv.py` & `flgo-0.0.9/src/flgo/algorithm/fedfv.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/algorithm/fedmgda+.py` & `flgo-0.0.9/src/flgo/algorithm/fedmgda+.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/algorithm/fedprox.py` & `flgo-0.0.9/src/flgo/algorithm/fedprox.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/algorithm/mifa.py` & `flgo-0.0.9/src/flgo/algorithm/mifa.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/algorithm/qfedavg.py` & `flgo-0.0.9/src/flgo/algorithm/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/algorithm/scaffold.py` & `flgo-0.0.9/src/flgo/algorithm/scaffold.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             "model": copy.deepcopy(self.model),
             "cg": self.cg,
         }
 
     def iterate(self):
         # sample clients
         self.selected_clients = self.sample()
-        # local training
+        # local_movielens_recommendation training
         res = self.communicate(self.selected_clients)
         dys, dcs = res['dy'], res['dc']
         # aggregate
         self.model, self.cg = self.aggregate(dys, dcs)
         return
 
     def aggregate(self, dys, dcs):
```

### Comparing `flgo-0.0.8/src/flgo/algorithm/vflbase.py` & `flgo-0.0.9/src/flgo/algorithm/vflbase.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,30 @@
+from __future__ import annotations
+
+import flgo.utils.fmodule
 from .fedbase import BasicParty
 import collections
 import torch
 import torch.multiprocessing as mp
 
 class PassiveParty(BasicParty):
-    def __init__(self, option):
+    r"""This is the implementation of the passive party in vertival FL.
+    The passive party owns only a part of data features without label information.
+
+    Args:
+        option (dict): running-time option
+    """
+    def __init__(self, option:dict):
         super().__init__()
         self.option = option
         self.actions = {0: self.forward, 1:self.backward, 2:self.forward_test}
         self.id = None
-        # create local dataset
+        # create local_movielens_recommendation dataset
         self.data_loader = None
-        # local calculator
+        # local_movielens_recommendation calculator
         self.device = self.gv.apply_for_device()
         self.calculator = self.gv.TaskCalculator(self.device, option['optimizer'])
         # hyper-parameters for training
         self.optimizer_name = option['optimizer']
         self.lr = option['learning_rate']
         self.momentum = option['momentum']
         self.weight_decay = option['weight_decay']
@@ -26,43 +35,82 @@
         self.test_batch_size = option['test_batch_size']
         self.loader_num_workers = option['num_workers']
         self.current_steps = 0
         # system setting
         self._effective_num_steps = self.num_steps
         self._latency = 0
 
-    def forward(self, package):
+    def forward(self, package:dict={}):
+        r"""
+        Local forward to computing the activations on local_movielens_recommendation features
+
+        Args:
+            package (dict): the package from the active party that contains batch information and the type of data
+
+        Returns:
+            passive_package (dict): the package that contains the activation to be sent to the active party
+        """
         batch_ids = package['batch']
         tmp = {'train': self.train_data, 'valid': self.valid_data, 'test':self.test_data}
         dataset = tmp[package['data_type']]
         # select samples in batch
         self.activation = self.local_module(dataset.get_batch_by_id(batch_ids)[0].to(self.device))
         return {'activation': self.activation.clone().detach()}
 
     def backward(self, package):
+        r"""
+        Local backward to computing the gradients on local_movielens_recommendation modules
+
+        Args:
+            package (dict): the package from the active party that contains the derivations
+        """
         derivation = package['derivation']
         self.update_local_module(derivation, self.activation)
         return
 
     def update_local_module(self, derivation, activation):
+        r"""
+        Update local_movielens_recommendation modules according to the derivation and the activation
+
+        Args:
+            derivation (Any): the derivation from the active party
+            activation (Any): the local_movielens_recommendation computed activation
+        """
         optimizer = self.calculator.get_optimizer(self.local_module, self.lr)
         loss_surrogat = (derivation*activation).sum()
         loss_surrogat.backward()
         optimizer.step()
         return
 
     def forward_test(self, package):
+        r"""
+        Local forward to computing the activations on local_movielens_recommendation features for testing
+
+        Args:
+            package (dict): the package from the active party that contains batch information and the type of data
+
+        Returns:
+            passive_package (dict): the package that contains the activation to be sent to the active party
+        """
         batch_ids = package['batch']
         tmp = {'train': self.train_data, 'valid': self.valid_data, 'test':self.test_data}
         dataset = tmp[package['data_type']]
         # select samples in batch
         self.activation = self.local_module(dataset.get_batch_by_id(batch_ids)[0].to(self.device))
         return {'activation': self.activation}
 
 class ActiveParty(PassiveParty):
+    r"""
+    This is the implementation of the active party in vertival FL. The active party owns
+    the data label information and may also own parts of data features. If a active party owns
+    data features, it is also a passive party simultaneously.
+
+    Args:
+        option (dict): running-time option
+    """
     def __init__(self, option):
         super().__init__(option)
         self.actions = {0: self.forward, 1: self.backward,2:self.forward_test}
         self.device = torch.device('cpu') if option['server_with_cpu'] else self.gv.apply_for_device()
         self.calculator = self.gv.TaskCalculator(self.device, optimizer_name = option['optimizer'])
         # basic configuration
         self.task = option['task']
@@ -128,15 +176,15 @@
         return self.unpack(packages_received_from_clients)
 
     def unpack(self, packages_received_from_clients):
         """
         Unpack the information from the received packages. Return models and losses as default.
         Args:
             packages_received_from_clients (list of dict):
-        Returns::
+        Returns:
             res (dict): collections.defaultdict that contains several lists of the clients' reply
         """
         if len(packages_received_from_clients)==0: return collections.defaultdict(list)
         res = {pname:[] for pname in packages_received_from_clients[0]}
         for cpkg in packages_received_from_clients:
             for pname, pval in cpkg.items():
                 res[pname].append(pval)
@@ -166,58 +214,117 @@
         self.gv.logger.info("=================End==================")
         self.gv.logger.time_end('Total Time Cost')
         # save results as .json file
         self.gv.logger.save_output_as_json()
         return
 
     def iterate(self):
+        r"""
+        The standard VFL process.
+
+         1. The active party first generates the batch information.
+
+         2. Then, it collects activations from all the passive parties.
+
+         3. Thirdly, it continues the forward passing and backward passing to update the decoder part of the model, and distributes the derivations to parties.
+
+         4. Finally, each passive party will update its local_movielens_recommendation modules accoring to the derivations and activations.
+
+        Returns:
+            updated (bool): whether the model is updated in this iteration
+        """
         self._data_type='train'
         self.crt_batch = self.get_batch_data()
         activations = self.communicate([pid for pid in range(len(self.parties))], mtype=0)['activation']
         self.defusions = self.update_global_module(activations, self.global_module)
         _ = self.communicate([pid for pid in range(len(self.parties))], mtype=1)
         return True
 
-    def pack(self, client_id, mtype=0):
+    def pack(self, party_id, mtype=0):
+        r"""
+        Pack the necessary information to parties into packages.
+
+        Args:
+            party_id (int): the id of the party
+            mtype (Any): the message type
+
+        Returns:
+            package (dict): the package
+        """
         if mtype==0:
             return {'batch': self.crt_batch[2], 'data_type': self._data_type}
         elif mtype==1:
-            return {'derivation': self.defusion[client_id]}
+            return {'derivation': self.defusion[party_id]}
         elif mtype==2:
             return {'batch': self.crt_test_batch[2], 'data_type': self._data_type}
 
     def get_batch_data(self):
         """
         Get the batch of data
-        Returns::
-            a batch of data
+        Returns:
+            batch_data (Any): a batch of data
         """
         try:
             batch_data = next(self.data_loader)
         except:
             self.data_loader = iter(self.calculator.get_dataloader(self.train_data, batch_size=self.batch_size))
             batch_data = next(self.data_loader)
         return batch_data
 
-    def update_global_module(self, activations, model):
+    def update_global_module(self, activations:list, model:torch.nn.Module|flgo.utils.fmodule.FModule):
+        r"""
+        Update the global module by computing the forward passing and the backward passing. The attribute
+        self.defusion and self.fusion.grad will be changed after calling this method.
+
+        Args:
+            activations (list): a list of activations from all the passive parties
+            model (torch.nn.Module|flgo.utils.fmodule.FModule): the model
+        """
         self.fusion = self.fuse(activations)
         self.fusion.requires_grad=True
         optimizer = self.calculator.get_optimizer(self.global_module, lr=self.lr)
         loss = self.calculator.compute_loss(model, (self.fusion, self.crt_batch[1]))['loss']
         loss.backward()
         optimizer.step()
         self.defusion = self.defuse(self.fusion)
 
-    def fuse(self, activations):
+    def fuse(self, activations:list):
+        r"""
+        Fuse the activations into one.
+
+        Args:
+            activations (list): a list of activations from all the passive parties
+
+        Returns:
+            fusion (Any): the fused result
+        """
         return torch.stack(activations).mean(dim=0)
 
     def defuse(self, fusion):
+        r"""
+        Defuse the fusion into derivations.
+
+        Args:
+            fusion (Any): the fused result
+
+        Returns:
+            derivations (list): a list of derivations
+        """
         return [fusion.grad for _ in self.parties]
 
-    def test(self, flag='test'):
+    def test(self, flag:str='test') -> dict:
+        r"""
+        Test the performance of the model
+
+        Args:
+            flag (str): the type of dataset
+
+        Returns:
+            result (dict): a dict that contains the testing result
+        """
         self.set_model_mode('eval')
         flag_dict = {'test':self.test_data, 'train':self.train_data, 'valid':self.valid_data}
         dataset = flag_dict[flag]
         self._data_type = flag
         dataloader = self.calculator.get_dataloader(dataset, batch_size=128)
         total_loss = 0.0
         num_correct = 0
@@ -231,14 +338,20 @@
             correct = y_pred.eq(batch_data[1].data.view_as(y_pred)).long().cpu().sum()
             num_correct += correct.item()
             total_loss += batch_mean_loss * len(batch_data[1])
         self.set_model_mode('train')
         return {'accuracy': 1.0 * num_correct / len(dataset), 'loss': total_loss / len(dataset)}
 
     def set_model_mode(self,mode = 'train'):
+        r"""
+        Set all the modes of the modules owned by all the parties.
+
+        Args:
+            mode (str): the mode of models
+        """
         for party in self.parties:
             if hasattr(party, 'local_module') and party.local_module is not None:
                 if mode == 'train':
                     party.local_module.train()
                 else:
                     party.local_module.eval()
             if hasattr(party, 'global_module') and party.global_module is not None:
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/__init__.py` & `flgo-0.0.9/src/flgo/benchmark/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 r"""
 This module is designed for fast creating federated tasks. For example,
 in FL, a commonly used benchmark is federated MNIST that splits MNIST
 into 100 shards and each shard contains data of two types of labels.
 
 In FLGo, three basic components are created to describe a general
-procedure that can easily convert various ML tasks into federated ones:
+procedure that can easily convert various ML tasks into federated ones.
 
-    1. TaskGenerator
-        1.1 load the original dataset
-        1.2 partition the original dataset into local data
+Components:
+    * `TaskGenerator`
+        - load the original dataset
+        - partition the original dataset into local_movielens_recommendation data
 
-    2. TaskPipe
-        2.1 store the partition information of TaskGenerator into the disk
+    * `TaskPipe`
+        - store the partition information of TaskGenerator into the disk
             when generating federated tasks
-        2.2 load the original dataset and the partition information to
+        - load the original dataset and the partition information to
             create the federated scenario when optimizing models
 
-    3. TaskCalculator
-        3.1 support task-specific computation when optimizing models, such
+    * `TaskCalculator`
+        - support task-specific computation when optimizing models, such
             as putting data into device, computing loss, evaluating models,
             and creating the data loader
 
 The architecture of a complete federate benchmark is shown as follows:
+
 ```
 benchmark_name                  # benchmark folder
 ├─ core.py                      # core file
 │   ├─ TaskGenerator            # class TaskGenerator(...)
 │   ├─ TaskPipe                 # class TaskPipe(...)
 │   └─ TaskCalculator           # class TaskCalculator(...)
 │
@@ -34,10 +36,27 @@
 │   ├─ ...
 │   └─ modelN_name.py           # model N (e.g. ResNet)
 │       ├─ init_local_module    # the function initializes personal models for parties
 │       └─ init_global_module   # the function initializes the global models for parties
 │
 └─ __init__.py                  # containing the variable default_model
 ```
+
+**Example**:
+The architecture of MNIST is
+```
+├─ core.py
+│   ├─ TaskGenerator
+│   ├─ TaskPipe
+│   └─ TaskCalculator
+├─  model
+│   ├─ cnn.py
+│   └─ mlp.py
+│       ├─ init_local_module
+│       └─ init_global_module
+└─ __init__.py
+```
+
+The details of implementing a customized benchmark are in Tutorial.3
 """
 
 path = '/'.join(__file__.split('/')[:-1])
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/base.py` & `flgo-0.0.9/src/flgo/benchmark/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,29 +78,30 @@
     def get_optimizer(self, model, *args, **kwargs):
         """Return the optimizer on the parameters of the model"""
         pass
 
 class BasicTaskGenerator(AbstractTaskGenerator):
     r"""
         Load the original dataset and partition the
-        original dataset into local data
+        original dataset into local_movielens_recommendation data
     """
     def __init__(self, benchmark:str, rawdata_path:str):
         """
         Args:
             benchmark (str): the name of the federated task
             rawdata_path (str): the dictionary of the original dataset
         """
         # basic attribution
         self.benchmark = benchmark
         self.rawdata_path = rawdata_path
         # optional attribution
         self.partitioner = None
         self.train_data = None
         self.test_data = None
+        self.valid_data = None
         self.task_name = None
         self.para = {}
         self.additional_option = {}
         self.train_additional_option = {}
         self.test_additional_option = {}
 
     def generate(self, *args, **kwarg):
@@ -114,15 +115,15 @@
         return
 
     def load_data(self, *args, **kwargs):
         """Download and load dataset into memory."""
         raise NotImplementedError
 
     def partition(self, *args, **kwargs):
-        """Partition the data into different local datasets"""
+        """Partition the data into different local_movielens_recommendation datasets"""
         return
 
     def register_partitioner(self, partitioner=None):
         """Register the partitioner as self's data partitioner"""
         self.partitioner = partitioner
 
     def init_para(self, para_list=None):
@@ -236,15 +237,15 @@
         task_data = self.load_data(running_time_option)
         objects = self.generate_objects(running_time_option)
         self.distribute(task_data, objects)
         return objects
 
     def distribute(self, task_data: dict, objects: list):
         r"""
-        Distribute the loaded local datasets to different objects in
+        Distribute the loaded local_movielens_recommendation datasets to different objects in
         the federated scenario
         """
         for ob in objects:
             ob_data = task_data[ob.name]
             for data_name, data in ob_data.items():
                 ob.set_data(data, data_name)
 
@@ -374,15 +375,15 @@
 
 class XYHorizontalTaskPipe(BasicTaskPipe):
     """
     This pipe is for supervised learning where each sample contains a feature $x_i$ and a label $y_i$
      that can be indexed by $i$.
     To use this pipe, it's necessary to set the attribute `test_data` of the generator to be a dict like:
         {'x': [...], 'y':[...]}
-    and the attribute `local_datas` to be a list of the above dict that means the local data owned by clients:
+    and the attribute `local_datas` to be a list of the above dict that means the local_movielens_recommendation data owned by clients:
         [{'x':[...], 'y':[...]}, ..., ]
     """
     TaskDataset = torch.utils.data.TensorDataset
 
     def save_task(self, generator):
         client_names = self.gen_client_names(len(generator.local_datas))
         feddata = {'client_names': client_names, 'server': {'data': generator.test_data}}
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/cifar100_classification/core.py` & `flgo-0.0.9/src/flgo/benchmark/voc_detection/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,23 @@
-import torchvision
-from flgo.benchmark.toolkits.cv.horizontal.image_classification import BuiltinClassGenerator, BuiltinClassPipe, GeneralCalculator
-import flgo.benchmark
-import os.path
-builtin_class = torchvision.datasets.CIFAR100
-transforms = torchvision.transforms.Compose([torchvision.transforms.ToTensor(), torchvision.transforms.Normalize((0.4914, 0.4822, 0.4465), (0.2023, 0.1994, 0.2010))])
-TaskCalculator = GeneralCalculator
+import torchvision.datasets
+import torchvision.transforms as transforms
+from flgo.benchmark.toolkits.cv.detection import *
+import torchvision.datasets
+import os
+import flgo
+
+transform = transforms.ToTensor()
+builtin_class = torchvision.datasets.VOCDetection
+path = os.path.join(flgo.benchmark.path,'RAW_DATA', 'VOC')
 
 class TaskGenerator(BuiltinClassGenerator):
-    def __init__(self, rawdata_path=os.path.join(flgo.benchmark.path,'RAW_DATA', 'CIFAR10')):
-        super(TaskGenerator, self).__init__('cifar100_classification', rawdata_path, builtin_class, transforms)
+    def __init__(self, rawdata_path=path, year='2007'):
+        super(TaskGenerator, self).__init__(benchmark=os.path.split(os.path.dirname(__file__))[-1], rawdata_path=rawdata_path, builtin_class=builtin_class, transform=transform)
+        self.additional_option = {'year':year}
+        self.train_additional_option = {'image_set':'trainval'}
+        self.test_additional_option = {'image_set':'test'} if year=='2007' else {}
 
 class TaskPipe(BuiltinClassPipe):
     def __init__(self, task_path):
-        super(TaskPipe, self).__init__(task_path, builtin_class, transforms)
+        super(TaskPipe, self).__init__(task_path, builtin_class, transform)
+
+TaskCalculator = GeneralCalculator
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/cifar100_classification/model/cnn.py` & `flgo-0.0.9/src/flgo/benchmark/cifar100_classification/model/cnn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/benchmark/cifar100_classification/model/resnet18.py` & `flgo-0.0.9/src/flgo/benchmark/cifar100_classification/model/resnet18.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/benchmark/cifar10_classification/__init__.py` & `flgo-0.0.9/src/flgo/benchmark/cifar10_classification/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 r"""CIFAR10 is a popular image classification benchmark in federated learning that
 is firstly used in `Communication-Efficient Learning of Deep Networks from Decentralized
 Data` (https://arxiv.org/abs/1602.05629). To create federated tasks based on this benchmark,
 you can try the following example:
 
 Example 1: create a IID partitioned CIFAR10 for 100 clients
+```
 >>> config = {'benchmark':{'name':'flgo.benchmark.cifar10_classification'},'partitioner':{'name': 'IIDPartitioner','para':{'num_clients':100}}}
 >>> flgo.gen_task(config, task_path='./test_cifar10')
+```
 After running the above codes, there will be a task dictionary './test_cifar10' that represents a federated task.
 This task is corresponding to a static scenario where the samples in CIFAR10 is I.I.D. allocated to 100 clients,
 and is also reusable for different algorithms so that a fair comparison can be easily achieved by optimizing
 the same model on the same task.
 
 Example 2: create a non-IID partitioned CIFAR10 for 100 clients
+```
 >>> niid_config = {'benchmark':{'name':'flgo.benchmark.cifar10_classification'},'partitioner':{'name': 'DirichletPartitioner','para':{'num_clients':100, 'alpha':0.5}}}
 >>> flgo.gen_task(niid_config, task_path='./test_cifar_dir0.5')
+```
 To create a non-IID CIFAR10, the only difference is to specify different partitioners in configurations, where
 the term `IIDPartitioner` is replaced by `DirichletPartitioner`. In addition, parameters of the partitioner can
 be input by `para`.
 """
 import flgo.benchmark.toolkits.visualization
 from flgo.benchmark.cifar10_classification.model import cnn
+import flgo.benchmark.toolkits.partition
 
+default_partitioner = flgo.benchmark.toolkits.partition.IIDPartitioner
+default_partition_para = {'num_clients':100}
 default_model = cnn
 visualize = flgo.benchmark.toolkits.visualization.visualize_by_class
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/cifar10_classification/core.py` & `flgo-0.0.9/src/flgo/benchmark/cifar100_classification/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import torchvision
-from flgo.benchmark.toolkits.cv.horizontal.image_classification import BuiltinClassGenerator, BuiltinClassPipe, GeneralCalculator
+from flgo.benchmark.toolkits.cv.classification import BuiltinClassGenerator, BuiltinClassPipe, GeneralCalculator
 import flgo.benchmark
 import os.path
-transforms = torchvision.transforms.Compose([torchvision.transforms.ToTensor(), torchvision.transforms.Normalize((0.4914, 0.4822, 0.4465), (0.2023, 0.1994, 0.2010))])
 
-TaskCalculator = GeneralCalculator
+builtin_class = torchvision.datasets.CIFAR100
+transform = torchvision.transforms.Compose([torchvision.transforms.ToTensor(), torchvision.transforms.Normalize((0.4914, 0.4822, 0.4465), (0.2023, 0.1994, 0.2010))])
+path = os.path.join(flgo.benchmark.path,'RAW_DATA', 'CIFAR100')
 
 class TaskGenerator(BuiltinClassGenerator):
-    def __init__(self, rawdata_path=os.path.join(flgo.benchmark.path,'RAW_DATA', 'CIFAR10')):
-        super(TaskGenerator, self).__init__('cifar10_classification', rawdata_path, torchvision.datasets.CIFAR10, transforms)
+    def __init__(self, rawdata_path=path):
+        super(TaskGenerator, self).__init__(os.path.split(os.path.dirname(__file__))[-1], rawdata_path, builtin_class, transform)
 
 class TaskPipe(BuiltinClassPipe):
     def __init__(self, task_path):
-        super(TaskPipe, self).__init__(task_path, torchvision.datasets.CIFAR10, transforms)
+        super(TaskPipe, self).__init__(task_path, builtin_class, transform)
+
+TaskCalculator = GeneralCalculator
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/cifar10_classification/model/cnn.py` & `flgo-0.0.9/src/flgo/benchmark/cifar10_classification/model/cnn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/benchmark/cifar10_classification/model/mlp.py` & `flgo-0.0.9/src/flgo/benchmark/cifar10_classification/model/mlp.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/benchmark/citeseer_link_prediction/core.py` & `flgo-0.0.9/src/flgo/benchmark/ciao_recommendation/core.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from torch_geometric.datasets import Planetoid
+from ..toolkits.rec.datasets import Ciao
+from ..toolkits.rec.rating_prediction import BuiltinClassGenerator, BuiltinClassPipe, GeneralCalculator
+import os
 import flgo.benchmark
-import os.path
-from flgo.benchmark.toolkits.graph.horizontal.link_prediction import *
 
-TaskCalculator = LinkPredicitonTaskCalculator
-class TaskGenerator(LinkPredicitonTaskGenenerator):
-    def __init__(self, rawdata_path=os.path.join(flgo.benchmark.path,'RAW_DATA', 'CITESEER'),*args, **kwargs):
-        super(TaskGenerator, self).__init__(benchmark='citeseer_link_prediction',rawdata_path=rawdata_path,
-                                            builtin_class=Planetoid, dataset_name='Citeseer', num_clients=10)
+path = os.path.join(flgo.benchmark.path,'RAW_DATA', 'CIAO')
+builtin_class  = Ciao
 
-class TaskPipe(LinkPredicitonTaskPipe):
-    def __init__(self, task_name):
-        super(TaskPipe, self).__init__(task_name, Planetoid, transform=None)
+class TaskGenerator(BuiltinClassGenerator):
+    def __init__(self, rawdata_path=path, split='train', min_val=10, max_val=10e8):
+        super(TaskGenerator, self).__init__(os.path.split(os.path.dirname(__file__))[-1], rawdata_path=rawdata_path, builtin_class=builtin_class)
+        self.additional_option = {'split': split, 'download':True, 'min_val':min_val, 'max_val':max_val}
+
+class TaskPipe(BuiltinClassPipe):
+    def __init__(self, task_path):
+        super(TaskPipe, self).__init__(task_path, builtin_class)
+
+TaskCalculator = GeneralCalculator
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/citeseer_link_prediction/model/GCN.py` & `flgo-0.0.9/src/flgo/benchmark/citeseer_link_prediction/model/GCN.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/benchmark/citeseer_node_classification/core.py` & `flgo-0.0.9/src/flgo/benchmark/local_movielens_recommendation/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-from torch_geometric.datasets import Planetoid
+from ..toolkits.rec.datasets import MovieLens
+from ..toolkits.rec.rating_prediction import BuiltinClassGenerator, BuiltinClassPipe, UserLevelCalculator
+import os
 import flgo.benchmark
-import os.path
-from flgo.benchmark.toolkits.graph.horizontal.node_classification import *
 
-TaskCalculator = NodeClassificationTaskCalculator
-class TaskGenerator(NodeClassificationTaskGen):
-    def __init__(self, rawdata_path=os.path.join(flgo.benchmark.path,'RAW_DATA', 'CITESEER'), *args, **kwargs):
-        super(TaskGenerator, self).__init__(benchmark='citeseer_node_classification',
-                                            rawdata_path=rawdata_path, builtin_class=Planetoid,
-                                            dataset_name='CITESEER', num_clients=10)
+path = os.path.join(flgo.benchmark.path,'RAW_DATA', 'MOVIELENS')
+builtin_class  = MovieLens
 
-class TaskPipe(NodeClassificationTaskPipe):
-    def __init__(self, task_name):
-        super(TaskPipe, self).__init__(task_name, Planetoid, transform=None)
+class TaskGenerator(BuiltinClassGenerator):
+    def __init__(self, rawdata_path=path, split='100k', min_val=10, max_val=10e8):
+        super(TaskGenerator, self).__init__(os.path.split(os.path.dirname(__file__))[-1], rawdata_path=rawdata_path, builtin_class=builtin_class)
+        self.additional_option = {'split': split, 'download':True, 'min_val':min_val, 'max_val':max_val}
+
+class TaskPipe(BuiltinClassPipe):
+    def __init__(self, task_path):
+        super(TaskPipe, self).__init__(task_path, builtin_class)
+
+TaskCalculator = UserLevelCalculator
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/citeseer_node_classification/model/GCN.py` & `flgo-0.0.9/src/flgo/benchmark/citeseer_node_classification/model/GCN.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/benchmark/cora_link_prediction/core.py` & `flgo-0.0.9/src/flgo/benchmark/pubmed_node_classification/core.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from torch_geometric.datasets import Planetoid
+import  torch_geometric.datasets
 import flgo.benchmark
-import os.path
-from flgo.benchmark.toolkits.graph.horizontal.link_prediction import *
+from flgo.benchmark.toolkits.graph.node_classification import *
 
-TaskCalculator = LinkPredicitonTaskCalculator
-class TaskGenerator(LinkPredicitonTaskGenenerator):
-    def __init__(self, rawdata_path=os.path.join(flgo.benchmark.path,'RAW_DATA', 'CORA'),*args, **kwargs):
-        super(TaskGenerator, self).__init__(benchmark='cora_link_prediction',rawdata_path=rawdata_path,
-                                            builtin_class=Planetoid, dataset_name='Cora', num_clients=10)
+path = os.path.join(flgo.benchmark.path,'RAW_DATA', 'PubMed')
+builtin_class = torch_geometric.datasets.Planetoid
 
-class TaskPipe(LinkPredicitonTaskPipe):
-    def __init__(self, task_name):
-        super(TaskPipe, self).__init__(task_name, Planetoid, transform=None)
+TaskCalculator = GeneralCalculator
+
+class TaskGenerator(BuiltinClassGenerator):
+    def __init__(self, rawdata_path=path):
+        super(TaskGenerator, self).__init__(benchmark=os.path.split(os.path.dirname(__file__))[-1],
+                                            rawdata_path=rawdata_path, builtin_class=builtin_class, transform=None, pre_transform=None)
+        self.additional_option = {'name': 'PubMed'}
+
+class TaskPipe(BuiltinClassPipe):
+    def __init__(self, task_path):
+        super(TaskPipe, self).__init__(task_path, buildin_class=builtin_class, transform=None)
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/cora_link_prediction/model/GCN.py` & `flgo-0.0.9/src/flgo/benchmark/pubmed_link_prediction/model/GCN.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import torch
 from torch_geometric.nn import GCNConv
 from flgo.utils.fmodule import FModule
 
 class Model(FModule):
     def __init__(self):
         super(Model, self).__init__()
-        self.conv1 = GCNConv(1433, 128)
+        self.conv1 = GCNConv(500, 128)
         self.conv2 = GCNConv(128, 64)
 
     def encode(self, x, edge_index):
         x = self.conv1(x, edge_index)
         x = x.relu()
         return self.conv2(x, edge_index)
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/cora_node_classification/model/GCN.py` & `flgo-0.0.9/src/flgo/benchmark/cora_node_classification/model/GCN.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/benchmark/cora_node_classification/model/GraphSAGE_1.py` & `flgo-0.0.9/src/flgo/benchmark/cora_node_classification/model/GraphSAGE_1.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/benchmark/cora_node_classification/model/GraphSage.py` & `flgo-0.0.9/src/flgo/benchmark/cora_node_classification/model/GraphSage.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/benchmark/emnist_classification/core.py` & `flgo-0.0.9/src/flgo/benchmark/emnist_classification/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import torchvision
-from flgo.benchmark.toolkits.cv.horizontal.image_classification import BuiltinClassGenerator, BuiltinClassPipe, GeneralCalculator
+from flgo.benchmark.toolkits.cv.classification import BuiltinClassGenerator, BuiltinClassPipe, GeneralCalculator
 import flgo.benchmark
 import os.path
-TaskCalculator = GeneralCalculator
+
+builtin_class = torchvision.datasets.EMNIST
+transform = torchvision.transforms.Compose([torchvision.transforms.ToTensor()])
+path = os.path.join(flgo.benchmark.path,'RAW_DATA', 'EMNIST')
 
 class TaskGenerator(BuiltinClassGenerator):
-    def __init__(self, rawdata_path=os.path.join(flgo.benchmark.path,'RAW_DATA', 'EMNIST'), split='byclass'):
-        super(TaskGenerator, self).__init__('emnist_classification', rawdata_path, torchvision.datasets.EMNIST, torchvision.transforms.Compose([torchvision.transforms.ToTensor(),]))
+    def __init__(self, rawdata_path=path, split='byclass'):
+        super(TaskGenerator, self).__init__(os.path.split(os.path.dirname(__file__))[-1], rawdata_path, builtin_class, transform)
         self.split = split
         self.additional_option = {'split': self.split}
 
     def load_data(self):
         self.train_data = torchvision.datasets.EMNIST(root=self.rawdata_path, split = self.split, download=True, train=True, transform=self.transform)
         self.test_data = torchvision.datasets.EMNIST(root=self.rawdata_path, split = self.split, download=True, train=False, transform=self.transform)
 
 class TaskPipe(BuiltinClassPipe):
     def __init__(self, task_path):
-        super(TaskPipe, self).__init__(task_path, torchvision.datasets.EMNIST, torchvision.transforms.Compose([torchvision.transforms.ToTensor(), ]))
+        super(TaskPipe, self).__init__(task_path, builtin_class, transform)
+
+TaskCalculator = GeneralCalculator
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/emnist_classification/model/cnn.py` & `flgo-0.0.9/src/flgo/benchmark/mnist_classification/model/cnn.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 class Model(FModule):
     def __init__(self):
         super().__init__()
         self.conv1 = nn.Conv2d(in_channels=1, out_channels=32, kernel_size=5, padding=2)
         self.conv2 = nn.Conv2d(in_channels=32, out_channels=64, kernel_size=5, padding=2)
         self.fc1 = nn.Linear(3136, 512)
-        self.fc2 = nn.Linear(512, 62)
+        self.fc2 = nn.Linear(512, 10)
 
     def forward(self, x):
         x = self.get_embedding(x)
         x = self.fc2(x)
         return x
 
     def get_embedding(self, x):
-        x = x.view((x.shape[0], 28, 28))
+        x = x.view((x.shape[0],28,28))
         x = x.unsqueeze(1)
         x = F.max_pool2d(F.relu(self.conv1(x)), 2)
         x = F.max_pool2d(F.relu(self.conv2(x)), 2)
-        x = x.view(-1, x.shape[1] * x.shape[2] * x.shape[3])
+        x = x.view(-1, x.shape[1]*x.shape[2]*x.shape[3])
         x = F.relu(self.fc1(x))
         return x
 
 def init_local_module(object):
     pass
 
 def init_global_module(object):
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/emnist_classification/model/mlp.py` & `flgo-0.0.9/src/flgo/benchmark/emnist_classification/model/mlp.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/benchmark/enzymes_graph_classification/core.py` & `flgo-0.0.9/src/flgo/benchmark/pubmed_link_prediction/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from torch_geometric.datasets import TUDataset
+import torch_geometric.datasets
 import flgo.benchmark
-import os.path
-from flgo.benchmark.toolkits.graph.horizontal.graph_classification import *
+from flgo.benchmark.toolkits.graph.link_prediction import *
 
-TaskCalculator = GraphClassificationTaskCalculator
+path = os.path.join(flgo.benchmark.path,'RAW_DATA', 'PUBMED')
+builtin_class = torch_geometric.datasets.Planetoid
+TaskCalculator = GeneralCalculator
 
-class TaskGenerator(GraphClassificationTaskGen):
-    def __init__(self, rawdata_path=os.path.join(flgo.benchmark.path,'RAW_DATA', 'ENZYMES'),*args, **kwargs):
-        super(TaskGenerator, self).__init__(benchmark='enzymes_graph_classification',rawdata_path=rawdata_path,
-                                            builtin_class=TUDataset, dataset_name='Enzymes')
+class TaskGenerator(BuiltinClassGenerator):
+    def __init__(self, rawdata_path=path,  test_rate=0.2, test_node_split=True, disjoint_train_ratio=0.3, neg_sampling_ratio=1.0):
+        super(TaskGenerator, self).__init__(benchmark=os.path.split(os.path.dirname(__file__))[-1],rawdata_path=rawdata_path,
+                                            builtin_class=builtin_class, test_rate=test_rate, test_node_split=test_node_split, disjoint_train_ratio=disjoint_train_ratio, neg_sampling_ratio=neg_sampling_ratio)
+        self.additional_option = {'name': 'Pubmed'}
 
-class TaskPipe(GraphClassificationTaskPipe):
+class TaskPipe(BuiltinClassPipe):
     def __init__(self, task_name):
-        super(TaskPipe, self).__init__(task_name, TUDataset, transform=None)
+        super(TaskPipe, self).__init__(task_name, builtin_class=builtin_class)
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/enzymes_graph_classification/model/GCN.py` & `flgo-0.0.9/src/flgo/benchmark/enzymes_graph_classification/model/GCN.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/benchmark/enzymes_graph_classification/model/GIN.py` & `flgo-0.0.9/src/flgo/benchmark/enzymes_graph_classification/model/GIN.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/benchmark/fashion_classification/core.py` & `flgo-0.0.9/src/flgo/benchmark/fashion_classification/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import torchvision
-from flgo.benchmark.toolkits.cv.horizontal.image_classification import BuiltinClassGenerator, BuiltinClassPipe, GeneralCalculator
+from flgo.benchmark.toolkits.cv.classification import BuiltinClassGenerator, BuiltinClassPipe, GeneralCalculator
 import flgo.benchmark
 import os.path
 builtin_class = torchvision.datasets.FashionMNIST
-transforms = torchvision.transforms.Compose([torchvision.transforms.ToTensor(), torchvision.transforms.Normalize((0.1307,), (0.3081,))])
+transform = torchvision.transforms.Compose([torchvision.transforms.ToTensor(), torchvision.transforms.Normalize((0.1307,), (0.3081,))])
+path = os.path.join(flgo.benchmark.path,'RAW_DATA', 'FASHION')
+
 TaskCalculator = GeneralCalculator
 
 class TaskGenerator(BuiltinClassGenerator):
-    def __init__(self, rawdata_path=os.path.join(flgo.benchmark.path,'RAW_DATA', 'FASHION')):
-        super(TaskGenerator, self).__init__('fashion_classification',rawdata_path , builtin_class, transforms)
+    def __init__(self, rawdata_path=path):
+        super(TaskGenerator, self).__init__(os.path.split(os.path.dirname(__file__))[-1], rawdata_path, builtin_class, transform)
 
 class TaskPipe(BuiltinClassPipe):
     def __init__(self, task_path):
-        super(TaskPipe, self).__init__(task_path, builtin_class, transforms)
+        super(TaskPipe, self).__init__(task_path, builtin_class, transform)
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/fashion_classification/model/lr.py` & `flgo-0.0.9/src/flgo/benchmark/fashion_classification/model/lr.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/benchmark/femnist_classification/core.py` & `flgo-0.0.9/src/flgo/benchmark/femnist_classification/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import math
 import shutil
 import urllib.request
-import random
 import zipfile
+from typing import Any
+
 import flgo.benchmark
 import os.path
 import json
 import numpy as np
-from sklearn.model_selection import train_test_split
-from torchvision.datasets import MNIST, utils
+from torchvision.datasets import MNIST
 from PIL import Image
 import os.path
 import torch
 import torchvision
-from tqdm import tqdm
 
-from flgo.benchmark.toolkits.cv.horizontal.image_classification import BuiltinClassGenerator, BuiltinClassPipe, GeneralCalculator
+from flgo.benchmark.toolkits.cv.classification import BuiltinClassGenerator, BuiltinClassPipe, GeneralCalculator
 
 def download_from_url(url= None, filepath = '.'):
     """Download dataset from url to filepath."""
     if url:urllib.request.urlretrieve(url, filepath)
     return filepath
 
 def extract_from_zip(src_path, target_path):
@@ -34,16 +33,16 @@
     """
     This dataset is derived from the Leaf repository
     (https://github.com/TalwalkarLab/leaf) pre-processing of the Extended MNIST
     dataset, grouping examples by writer. Details about Leaf were published in
     "LEAF: A Benchmark for Federated Settings" https://arxiv.org/abs/1812.01097.
     """
 
-    def __init__(self, root, train=True, transform=None, target_transform=None,
-                 download=False):
+    def __init__(self, root:str, train:bool=True, transform:Any=None, target_transform:Any=None,
+                 download:bool=False):
         super(MNIST, self).__init__(root, transform=transform,
                                     target_transform=target_transform)
         self.train = train
         if self.train:
             data_file = self.training_file
         else:
             data_file = self.test_file
@@ -117,14 +116,18 @@
         train_data, train_targets, train_sample_id = Xs[train_indices], Ys[train_indices], sample_ids[train_indices]
         test_data, test_targets, test_sample_id = Xs[test_indices], Ys[test_indices], sample_ids[test_indices]
         torch.save((train_data, train_targets, train_sample_id), os.path.join(self.processed_folder, "training.pt"))
         torch.save((test_data, test_targets, test_sample_id), os.path.join(self.processed_folder, "test.pt"))
 
 TaskCalculator = GeneralCalculator
 
+builtin_class = FEMNIST
+path = os.path.join(flgo.benchmark.path,'RAW_DATA', 'MNIST')
+transform = torchvision.transforms.Compose([torchvision.transforms.ToTensor(), ])
+
 class TaskGenerator(BuiltinClassGenerator):
-    def __init__(self, rawdata_path=os.path.join(flgo.benchmark.path,'RAW_DATA', 'MNIST')):
-        super(TaskGenerator, self).__init__('femnist_classification', rawdata_path, FEMNIST, torchvision.transforms.Compose([torchvision.transforms.ToTensor(),]))
+    def __init__(self, rawdata_path=path):
+        super(TaskGenerator, self).__init__(os.path.split(os.path.dirname(__file__))[-1], rawdata_path, builtin_class, transform)
 
 class TaskPipe(BuiltinClassPipe):
     def __init__(self, task_path):
-        super(TaskPipe, self).__init__(task_path, FEMNIST, torchvision.transforms.Compose([torchvision.transforms.ToTensor(), ]))
+        super(TaskPipe, self).__init__(task_path, builtin_class, transform)
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/leaf_reddit/core.py` & `flgo-0.0.9/src/flgo/benchmark/leaf_reddit/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
             if isinstance(idx, list):
                 return self.dataset[[self.indices[i] for i in idx]]
             return self.dataset[self.indices[idx]]
 
     def save_task(self, generator):
         client_names = self.gen_client_names(len(generator.local_datas))
         feddata = {'client_names': client_names, 'server_data': list(range(len(generator.test_data))),
-                   'rawdata_path': generator.rawdata_path}
+                   'rawdata_path': generator.root}
         for cid in range(len(client_names)): feddata[client_names[cid]] = {'data': generator.local_datas[cid], }
         with open(os.path.join(self.task_path, 'data.json'), 'w') as outf:
             json.dump(feddata, outf)
         return
 
     def load_data(self, running_time_option) -> dict:
         # load the datasets
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/leaf_reddit/model/stackedlstm.py` & `flgo-0.0.9/src/flgo/benchmark/leaf_reddit/model/stackedlstm.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/benchmark/leaf_sent140/core.py` & `flgo-0.0.9/src/flgo/benchmark/leaf_sent140/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,15 +196,15 @@
             if isinstance(idx, list):
                 return self.dataset[[self.indices[i] for i in idx]]
             return self.dataset[self.indices[idx]]
 
     def save_task(self, generator):
         client_names = self.gen_client_names(len(generator.local_datas))
         feddata = {'client_names': client_names, 'server_data': list(range(len(generator.test_data))),
-                   'rawdata_path': generator.rawdata_path}
+                   'rawdata_path': generator.root}
         for cid in range(len(client_names)): feddata[client_names[cid]] = {'data': generator.local_datas[cid], }
         with open(os.path.join(self.task_path, 'data.json'), 'w') as outf:
             json.dump(feddata, outf)
         return
 
     def load_data(self, running_time_option) -> dict:
         # load the datasets
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/leaf_sent140/model/stackedlstm.py` & `flgo-0.0.9/src/flgo/benchmark/leaf_sent140/model/stackedlstm.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/benchmark/mnist_classification/__init__.py` & `flgo-0.0.9/src/flgo/benchmark/mnist_classification/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 r"""MNIST is a popular image classification benchmark in federated learning that
 is firstly used in `Communication-Efficient Learning of Deep Networks from Decentralized
 Data` (https://arxiv.org/abs/1602.05629). To create federated tasks based on this benchmark,
 you can try the following example:
 
 Example 1: create a IID partitioned MNIST for 100 clients
+```
 >>> config = {'benchmark':{'name':'flgo.benchmark.mnist_classification'},'partitioner':{'name': 'IIDPartitioner','para':{'num_clients':100}}}
 >>> flgo.gen_task(config, task_path='./test_mnist')
+```
 After running the above codes, there will be a task dictionary './test_mnist' that represents a federated task.
 This task is corresponding to a static scenario where the samples in MNIST is I.I.D. allocated to 100 clients,
 and is also reusable for different algorithms so that a fair comparison can be easily achieved by optimizing
 the same model on the same task.
 
 Example 2: create a non-IID partitioned MNIST for 100 clients
+```
 >>> niid_config = {'benchmark':{'name':'flgo.benchmark.mnist_classification'},'partitioner':{'name': 'DirichletPartitioner','para':{'num_clients':100, 'alpha':0.5}}}
 >>> flgo.gen_task(niid_config, task_path='./test_mnist_dir0.5')
+```
 To create a non-IID MNIST, the only difference is to specify different partitioners in configurations, where
 the term `IIDPartitioner` is replaced by `DirichletPartitioner`. In addition, parameters of the partitioner can
 be input by `para`.
 """
 import flgo.benchmark.toolkits.visualization
 from flgo.benchmark.mnist_classification.model import cnn
+import flgo.benchmark.toolkits.partition
+
+default_partitioner = flgo.benchmark.toolkits.partition.IIDPartitioner
+default_partition_para = {'num_clients':100}
 default_model = cnn
 visualize = flgo.benchmark.toolkits.visualization.visualize_by_class
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/mnist_classification/core.py` & `flgo-0.0.9/src/flgo/benchmark/mnist_classification/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import torchvision
-from flgo.benchmark.toolkits.cv.horizontal.image_classification import BuiltinClassGenerator, BuiltinClassPipe, GeneralCalculator
+from flgo.benchmark.toolkits.cv.classification import BuiltinClassGenerator, BuiltinClassPipe, GeneralCalculator
 import flgo.benchmark
 import os.path
 
 builtin_class = torchvision.datasets.MNIST
-transforms = torchvision.transforms.Compose([torchvision.transforms.ToTensor(), torchvision.transforms.Normalize((0.1307,), (0.3081,))])
+transform = torchvision.transforms.Compose([torchvision.transforms.ToTensor(), torchvision.transforms.Normalize((0.1307,), (0.3081,))])
+path = os.path.join(flgo.benchmark.path,'RAW_DATA', 'MNIST')
+
 TaskCalculator = GeneralCalculator
 
 class TaskGenerator(BuiltinClassGenerator):
-    def __init__(self, rawdata_path=os.path.join(flgo.benchmark.path,'RAW_DATA', 'MNIST')):
-        super(TaskGenerator, self).__init__('mnist_classification', rawdata_path, builtin_class, transforms)
+    def __init__(self, rawdata_path=path):
+        super(TaskGenerator, self).__init__(os.path.split(os.path.dirname(__file__))[-1], rawdata_path, builtin_class, transform)
 
 class TaskPipe(BuiltinClassPipe):
     def __init__(self, task_path):
-        super(TaskPipe, self).__init__(task_path, builtin_class, transforms)
+        super(TaskPipe, self).__init__(task_path, builtin_class, transform)
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/mnist_classification/model/cnn.py` & `flgo-0.0.9/src/flgo/benchmark/mnist_classification/model/mlp.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,31 @@
+
 from torch import nn
 import torch.nn.functional as F
 from flgo.utils.fmodule import FModule
 
+
 class Model(FModule):
     def __init__(self):
-        super().__init__()
-        self.conv1 = nn.Conv2d(in_channels=1, out_channels=32, kernel_size=5, padding=2)
-        self.conv2 = nn.Conv2d(in_channels=32, out_channels=64, kernel_size=5, padding=2)
-        self.fc1 = nn.Linear(3136, 512)
-        self.fc2 = nn.Linear(512, 10)
+        super(Model, self).__init__()
+        self.fc1 = nn.Linear(784, 200)
+        self.fc2 = nn.Linear(200, 200)
+        self.fc3 = nn.Linear(200, 10)
 
     def forward(self, x):
         x = self.get_embedding(x)
-        x = self.fc2(x)
+        x = self.fc3(x)
         return x
 
     def get_embedding(self, x):
-        x = x.view((x.shape[0],28,28))
-        x = x.unsqueeze(1)
-        x = F.max_pool2d(F.relu(self.conv1(x)), 2)
-        x = F.max_pool2d(F.relu(self.conv2(x)), 2)
-        x = x.view(-1, x.shape[1]*x.shape[2]*x.shape[3])
-        x = F.relu(self.fc1(x))
+        x = x.view(-1, x.shape[1] * x.shape[-2] * x.shape[-1])
+        x = self.fc1(x)
+        x = F.relu(x)
+        x = self.fc2(x)
+        x = F.relu(x)
         return x
 
 def init_local_module(object):
     pass
 
 def init_global_module(object):
-    if 'Server' in object.__class__.__name__:
-        object.model = Model().to(object.device)
+    object.model = Model().to(object.device) if 'Server' in object.__class__.__name__ else None
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/mnist_classification/model/mlp.py` & `flgo-0.0.9/src/flgo/benchmark/svhn_classification/model/mlp.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-
 from torch import nn
-import torch.nn.functional as F
 from flgo.utils.fmodule import FModule
 
-
 class Model(FModule):
-    def __init__(self):
+    def __init__(self, dim_in=3*32*32, dim_hidden=200, dim_out=10):
         super(Model, self).__init__()
-        self.fc1 = nn.Linear(784, 200)
-        self.fc2 = nn.Linear(200, 200)
-        self.fc3 = nn.Linear(200, 10)
+        self.layer_input = nn.Linear(dim_in, dim_hidden)
+        self.relu = nn.ReLU()
+        self.fc1 = nn.Linear(dim_hidden, dim_hidden)
+        self.fc2 = nn.Linear(dim_hidden, dim_out)
 
     def forward(self, x):
         x = self.get_embedding(x)
-        x = self.fc3(x)
+        x = self.fc2(x)
         return x
 
     def get_embedding(self, x):
         x = x.view(-1, x.shape[1] * x.shape[-2] * x.shape[-1])
+        x = self.layer_input(x)
+        x = self.relu(x)
         x = self.fc1(x)
-        x = F.relu(x)
-        x = self.fc2(x)
-        x = F.relu(x)
+        x = self.relu(x)
         return x
 
 def init_local_module(object):
     pass
 
 def init_global_module(object):
-    object.model = Model().to(object.device) if 'Server' in object.__class__.__name__ else None
+    if 'Server' in object.__class__.__name__:
+        object.model = Model().to(object.device)
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/mutag_graph_classification/core.py` & `flgo-0.0.9/src/flgo/benchmark/citeseer_link_prediction/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from torch_geometric.datasets import TUDataset
+import torch_geometric.datasets
 import flgo.benchmark
-import os.path
-from flgo.benchmark.toolkits.graph.horizontal.graph_classification import *
+from flgo.benchmark.toolkits.graph.link_prediction import *
 
-TaskCalculator = GraphClassificationTaskCalculator
+path = os.path.join(flgo.benchmark.path,'RAW_DATA', 'CITESEER')
+builtin_class = torch_geometric.datasets.Planetoid
+TaskCalculator = GeneralCalculator
 
-class TaskGenerator(GraphClassificationTaskGen):
-    def __init__(self, rawdata_path=os.path.join(flgo.benchmark.path,'RAW_DATA', 'MUTAG'),*args, **kwargs):
-        super(TaskGenerator, self).__init__(benchmark='mutag_graph_classification',rawdata_path=rawdata_path,
-                                            builtin_class=TUDataset, dataset_name='Mutag')
+class TaskGenerator(BuiltinClassGenerator):
+    def __init__(self, rawdata_path=path,  test_rate=0.2, test_node_split=True, disjoint_train_ratio=0.3, neg_sampling_ratio=1.0):
+        super(TaskGenerator, self).__init__(benchmark=os.path.split(os.path.dirname(__file__))[-1],rawdata_path=rawdata_path,
+                                            builtin_class=builtin_class, test_rate=test_rate, test_node_split=test_node_split, disjoint_train_ratio=disjoint_train_ratio, neg_sampling_ratio=neg_sampling_ratio)
+        self.additional_option = {'name': 'Citeseer'}
 
-class TaskPipe(GraphClassificationTaskPipe):
+class TaskPipe(BuiltinClassPipe):
     def __init__(self, task_name):
-        super(TaskPipe, self).__init__(task_name, TUDataset, transform=None)
+        super(TaskPipe, self).__init__(task_name, builtin_class=builtin_class)
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/mutag_graph_classification/model/GCN.py` & `flgo-0.0.9/src/flgo/benchmark/mutag_graph_classification/model/GCN.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/benchmark/pubmed_link_prediction/core.py` & `flgo-0.0.9/src/flgo/benchmark/cifar10_classification/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,19 @@
-from torch_geometric.datasets import Planetoid
+import torchvision
+from flgo.benchmark.toolkits.cv.classification import BuiltinClassGenerator, BuiltinClassPipe, GeneralCalculator
 import flgo.benchmark
 import os.path
-from flgo.benchmark.toolkits.graph.horizontal.link_prediction import *
 
-TaskCalculator = LinkPredicitonTaskCalculator
-class TaskGenerator(LinkPredicitonTaskGenenerator):
-    def __init__(self, rawdata_path=os.path.join(flgo.benchmark.path,'RAW_DATA', 'PUBMED'),*args, **kwargs):
-        super(TaskGenerator, self).__init__(benchmark='pubmed_link_prediction',rawdata_path=rawdata_path,
-                                            builtin_class=Planetoid, dataset_name='Pubmed', num_clients=10)
+# task configuration
+transform = torchvision.transforms.Compose([torchvision.transforms.ToTensor(), torchvision.transforms.Normalize((0.4914, 0.4822, 0.4465), (0.2023, 0.1994, 0.2010))])
+path = os.path.join(flgo.benchmark.path,'RAW_DATA', 'CIFAR10')
+builtin_class = torchvision.datasets.CIFAR10
 
-class TaskPipe(LinkPredicitonTaskPipe):
-    def __init__(self, task_name):
-        super(TaskPipe, self).__init__(task_name, Planetoid, transform=None)
+class TaskGenerator(BuiltinClassGenerator):
+    def __init__(self, rawdata_path=path):
+        super(TaskGenerator, self).__init__(os.path.split(os.path.dirname(__file__))[-1], rawdata_path, builtin_class, transform)
+
+class TaskPipe(BuiltinClassPipe):
+    def __init__(self, task_path):
+        super(TaskPipe, self).__init__(task_path, builtin_class, transform)
+
+TaskCalculator = GeneralCalculator
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/pubmed_link_prediction/model/GCN.py` & `flgo-0.0.9/src/flgo/benchmark/cora_link_prediction/model/GCN.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import torch
 from torch_geometric.nn import GCNConv
 from flgo.utils.fmodule import FModule
 
 class Model(FModule):
     def __init__(self):
         super(Model, self).__init__()
-        self.conv1 = GCNConv(500, 128)
+        self.conv1 = GCNConv(1433, 128)
         self.conv2 = GCNConv(128, 64)
 
     def encode(self, x, edge_index):
-        x = self.conv1(x, edge_index)
+        x = self.conv1(x, edge_index.long())
         x = x.relu()
-        return self.conv2(x, edge_index)
+        return self.conv2(x, edge_index.long())
 
     def decode(self, z, edge_label_index):
-        return (z[edge_label_index[0]] * z[edge_label_index[1]]).sum(dim=-1)
+        return (z[edge_label_index.long()[0]] * z[edge_label_index.long()[1]]).sum(dim=-1)
 
     def decode_all(self, z):
         prob_adj = z @ z.t()
         return (prob_adj > 0).nonzero(as_tuple=False).t()
 
 def init_local_module(object):
     pass
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/pubmed_node_classification/model/GCN.py` & `flgo-0.0.9/src/flgo/benchmark/pubmed_node_classification/model/GCN.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/benchmark/shakespeare_classification/core.py` & `flgo-0.0.9/src/flgo/benchmark/shakespeare_classification/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,15 +275,15 @@
             if isinstance(idx, list):
                 return self.dataset[[self.indices[i] for i in idx]]
             return self.dataset[self.indices[idx]]
 
     def save_task(self, generator):
         client_names = self.gen_client_names(len(generator.local_datas))
         feddata = {'client_names': client_names, 'server_data': list(range(len(generator.test_data))),
-                   'rawdata_path': generator.rawdata_path}
+                   'rawdata_path': generator.root}
         for cid in range(len(client_names)): feddata[client_names[cid]] = {'data': generator.local_datas[cid], }
         with open(os.path.join(self.task_path, 'data.json'), 'w') as outf:
             json.dump(feddata, outf)
         return
 
     def load_data(self, running_time_option) -> dict:
         # load the datasets
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/shakespeare_classification/model/stackedlstm.py` & `flgo-0.0.9/src/flgo/benchmark/shakespeare_classification/model/stackedlstm.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/benchmark/svhn_classification/core.py` & `flgo-0.0.9/src/flgo/benchmark/svhn_classification/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 import torchvision
-from flgo.benchmark.toolkits.cv.horizontal.image_classification import BuiltinClassGenerator, BuiltinClassPipe, GeneralCalculator
+from flgo.benchmark.toolkits.cv.classification import BuiltinClassGenerator, BuiltinClassPipe, GeneralCalculator
 import flgo.benchmark
 import os.path
-import torch
-transforms = torchvision.transforms.Compose([torchvision.transforms.ToTensor(), torchvision.transforms.Normalize((0.4914, 0.4822, 0.4465), (0.2023, 0.1994, 0.2010))])
 
+transform = torchvision.transforms.Compose([torchvision.transforms.ToTensor(), torchvision.transforms.Normalize((0.4914, 0.4822, 0.4465), (0.2023, 0.1994, 0.2010))])
+builtin_class = torchvision.datasets.SVHN
+path = os.path.join(flgo.benchmark.path,'RAW_DATA', 'SVHN')
 TaskCalculator = GeneralCalculator
 
 class TaskGenerator(BuiltinClassGenerator):
-    def __init__(self, rawdata_path=os.path.join(flgo.benchmark.path,'RAW_DATA', 'SVHN')):
-        super(TaskGenerator, self).__init__('svhn_classification', rawdata_path, torchvision.datasets.SVHN, transforms)
+    def __init__(self, rawdata_path=path):
+        super(TaskGenerator, self).__init__(os.path.split(os.path.dirname(__file__))[-1], rawdata_path, builtin_class, transform)
         self.train_additional_option = {'split':'train'}
         self.test_additional_option = {'split':'test'}
 
-    def load_data(self):
-        self.train_data = self.builtin_class(root=self.rawdata_path, download=True, split='train', transform=self.transform)
-        self.test_data = self.builtin_class(root=self.rawdata_path, download=True, split='test',transform=self.transform)
-
 class TaskPipe(BuiltinClassPipe):
     def __init__(self, task_path):
-        super(TaskPipe, self).__init__(task_path, torchvision.datasets.SVHN, transforms)
+        super(TaskPipe, self).__init__(task_path, builtin_class, transform)
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/svhn_classification/model/cnn.py` & `flgo-0.0.9/src/flgo/benchmark/svhn_classification/model/cnn.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/benchmark/synthetic_regression/core.py` & `flgo-0.0.9/src/flgo/benchmark/synthetic_regression/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-import numpy as np
 from flgo.benchmark.base import *
-from flgo.benchmark.toolkits.cv.horizontal.image_classification import GeneralCalculator
+from flgo.benchmark.toolkits.cv.classification import GeneralCalculator
 from flgo.benchmark.toolkits.partition import BasicPartitioner
 TaskPipe = XYHorizontalTaskPipe
 TaskCalculator = GeneralCalculator
 
 class TaskGenerator(BasicTaskGenerator):
     def __init__(self, alpha=0.0, beta=0.0, num_clients=30, imbalance=0.0, mean_datavol=400, dimension=60, num_classes=10, *args, **kwargs):
         super().__init__('synthetic_regression', '')
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/synthetic_regression/model/lr.py` & `flgo-0.0.9/src/flgo/benchmark/synthetic_regression/model/lr.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/benchmark/toolkits/cv/horizontal/image_classification.py` & `flgo-0.0.9/src/flgo/benchmark/toolkits/cv/classification/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,18 +16,32 @@
     def __init__(self, benchmark, rawdata_path, builtin_class, transform=None):
         super(BuiltinClassGenerator, self).__init__(benchmark, rawdata_path)
         self.builtin_class = builtin_class
         self.transform = transform
         self.additional_option = {}
         self.train_additional_option = {}
         self.test_additional_option = {}
+        self.download = True
 
     def load_data(self):
-        self.train_data = self.builtin_class(root=self.rawdata_path, download=True, train=True, transform=self.transform)
-        self.test_data = self.builtin_class(root=self.rawdata_path, download=True, train=False, transform=self.transform)
+        # load the datasets
+        train_default_init_para = {'root': self.rawdata_path, 'download':self.download, 'train':True, 'transform':self.transform}
+        test_default_init_para = {'root': self.rawdata_path, 'download':self.download, 'train':False, 'transform':self.transform}
+        train_default_init_para.update(self.additional_option)
+        train_default_init_para.update(self.train_additional_option)
+        test_default_init_para.update(self.additional_option)
+        test_default_init_para.update(self.test_additional_option)
+        if 'kwargs' not in self.builtin_class.__init__.__annotations__:
+            train_pop_key = [k for k in train_default_init_para.keys() if k not in self.builtin_class.__init__.__annotations__]
+            test_pop_key = [k for k in test_default_init_para.keys() if k not in self.builtin_class.__init__.__annotations__]
+            for k in train_pop_key: train_default_init_para.pop(k)
+            for k in test_pop_key: test_default_init_para.pop(k)
+        # init datasets
+        self.train_data = self.builtin_class(**train_default_init_para)
+        self.test_data = self.builtin_class(**test_default_init_para)
 
     def partition(self):
         self.local_datas = self.partitioner(self.train_data)
         self.num_clients = len(self.local_datas)
 
 class BuiltinClassPipe(BasicTaskPipe):
     r"""
@@ -63,21 +77,27 @@
                     if isinstance(idx, list):
                         return self.dataset[[self.indices[i] for i in idx]]
                     return self.dataset[self.indices[idx]]
                 else:
                     return self.dataset[self.indices[idx]][0] + self.perturbation[self.indices[idx]],  self.dataset[self.indices[idx]][1]
 
     def __init__(self, task_path, buildin_class, transform=None):
+        """
+        Args:
+            task_path (str): the path of the task
+            builtin_class (class): class in torchvision.datasets
+            transform (torchvision.transforms.*): the transform
+        """
         super(BuiltinClassPipe, self).__init__(task_path)
         self.builtin_class = buildin_class
         self.transform = transform
 
     def save_task(self, generator):
         client_names = self.gen_client_names(len(generator.local_datas))
-        feddata = {'client_names': client_names, 'server_data': list(range(len(generator.test_data))),  'rawdata_path': generator.rawdata_path, 'additional_option': generator.additional_option, 'train_additional_option':generator.train_additional_option, 'test_additional_option':generator.test_additional_option,}
+        feddata = {'client_names': client_names, 'server_data': list(range(len(generator.test_data))),  'rawdata_path': generator.root, 'additional_option': generator.additional_option, 'train_additional_option':generator.train_additional_option, 'test_additional_option':generator.test_additional_option, }
         for cid in range(len(client_names)): feddata[client_names[cid]] = {'data': generator.local_datas[cid],}
         if hasattr(generator.partitioner, 'local_perturbation'): feddata['local_perturbation'] = generator.partitioner.local_perturbation
         with open(os.path.join(self.task_path, 'data.json'), 'w') as outf:
             json.dump(feddata, outf)
         return
 
     def load_data(self, running_time_option) -> dict:
@@ -85,18 +105,19 @@
         train_default_init_para = {'root': self.feddata['rawdata_path'], 'download':True, 'train':True, 'transform':self.transform}
         test_default_init_para = {'root': self.feddata['rawdata_path'], 'download':True, 'train':False, 'transform':self.transform}
         if 'additional_option' in self.feddata.keys():
             train_default_init_para.update(self.feddata['additional_option'])
             test_default_init_para.update(self.feddata['additional_option'])
         if 'train_additional_option' in self.feddata.keys(): train_default_init_para.update(self.feddata['train_additional_option'])
         if 'test_additional_option' in self.feddata.keys(): test_default_init_para.update(self.feddata['test_additional_option'])
-        train_pop_key = [k for k in train_default_init_para.keys() if k not in self.builtin_class.__init__.__annotations__]
-        test_pop_key = [k for k in test_default_init_para.keys() if k not in self.builtin_class.__init__.__annotations__]
-        for k in train_pop_key: train_default_init_para.pop(k)
-        for k in test_pop_key: test_default_init_para.pop(k)
+        if 'kwargs' not in self.builtin_class.__init__.__annotations__:
+            train_pop_key = [k for k in train_default_init_para.keys() if k not in self.builtin_class.__init__.__annotations__]
+            test_pop_key = [k for k in test_default_init_para.keys() if k not in self.builtin_class.__init__.__annotations__]
+            for k in train_pop_key: train_default_init_para.pop(k)
+            for k in test_pop_key: test_default_init_para.pop(k)
         train_data = self.builtin_class(**train_default_init_para)
         test_data = self.builtin_class(**test_default_init_para)
         test_data = self.TaskDataset(test_data, list(range(len(test_data))), None, running_time_option['pin_memory'])
         # rearrange data for server
         server_data_test, server_data_valid = self.split_dataset(test_data, running_time_option['test_holdout'])
         task_data = {'server': {'test': server_data_test, 'valid': server_data_valid}}
         # rearrange data for clients
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/toolkits/graph/horizontal/graph_classification.py` & `flgo-0.0.9/src/flgo/benchmark/toolkits/graph/graph_classification/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,115 +1,133 @@
-from torch import Tensor
+import torch
 from torch_geometric.data import Data, DataLoader
+from flgo.benchmark.toolkits.graph.node_classification import BuiltinClassGenerator as NodeClassGenerator
+import os
+try:
+    import ujson as json
+except:
+    import json
+from flgo.benchmark.base import BasicTaskPipe, BasicTaskCalculator
+import random
 
-import collections
-import numpy as np
-
-from flgo.benchmark.base import *
-
-from flgo.benchmark.toolkits import BasicTaskPipe, BasicTaskCalculator
-
-
-class GraphClassificationTaskGen(BasicTaskGenerator):
-    def __init__(self, benchmark, rawdata_path, builtin_class, dataset_name, transforms=None):
-        super(GraphClassificationTaskGen, self).__init__(benchmark, rawdata_path)
-        self.builtin_class = builtin_class
-        self.dataset_name = dataset_name
-        self.transforms = transforms
-        self.additional_option = {}
-
+class BuiltinClassGenerator(NodeClassGenerator):
     def load_data(self):
-        self.all_data, self.perm = self.builtin_class(root=self.rawdata_path, name=self.dataset_name, transform=self.transforms).shuffle(return_perm=True)
-        self.num_samples = len(self.all_data)
-        k = int(0.9 * self.num_samples)
-        self.train_data = self.all_data[:k]
-        self.test_data = list(range(self.num_samples))[k:]
+        default_init_para = {'root': self.rawdata_path, 'download':self.download, 'train':True, 'transform':self.transform}
+        default_init_para.update(self.additional_option)
+        if 'kwargs' not in self.builtin_class.__init__.__annotations__:
+            pop_key = [k for k in default_init_para.keys() if k not in self.builtin_class.__init__.__annotations__]
+            for k in pop_key: default_init_para.pop(k)
+        self.dataset = self.builtin_class(**default_init_para)
+        self.num_samples = len(self.dataset)
+        k = int(self.test_rate*self.num_samples)
+        all_idxs = list(range(self.num_samples))
+        random.shuffle(all_idxs)
+        self.test_idxs = all_idxs[:k]
+        self.train_idxs = all_idxs[k:]
+        self.train_data = self.dataset[self.train_idxs]
+        self.train_data = [(d, self.dataset[d].y) for d in self.train_idxs]
+        self.test_data = self.dataset[self.test_idxs]
 
     def partition(self):
         self.local_datas = self.partitioner(self.train_data)
         self.num_clients = len(self.local_datas)
+        self.local_datas = [[self.train_data[idx][0] for idx in local_data] for local_data in self.local_datas]
 
-
-class GraphClassificationTaskPipe(BasicTaskPipe):
-    def __init__(self, task_name, buildin_class, transform=None):
-        super(GraphClassificationTaskPipe, self).__init__(task_name)
+class BuiltinClassPipe(BasicTaskPipe):
+    def __init__(self, task_path, buildin_class, transform=None, pre_transform=None):
+        super(BuiltinClassPipe, self).__init__(task_path)
         self.builtin_class = buildin_class
+        self.pre_transform = pre_transform
         self.transform = transform
 
     def save_task(self, generator):
-        client_names = self.gen_client_names(len(generator.local_nodes))
+        client_names = self.gen_client_names(len(generator.local_datas))
         feddata = {'client_names': client_names,
                    'server_data': list(range(len(generator.test_data))),
-                   'rawdata_path': generator.rawdata_path,
-                   'para': generator.para,
-                   'dataset_name': generator.dataset_name,
-                   'perm': generator.perm}
+                   'rawdata_path': generator.root,
+                   'additional_option':generator.additional_option,
+                   'test_idxs':generator.test_idxs,
+                   'download': generator.download_data,
+                   }
         for cid in range(len(client_names)):
             feddata[client_names[cid]] = {'data': generator.local_datas[cid], }
         with open(os.path.join(self.task_path, 'data.json'), 'w') as outf:
             json.dump(feddata, outf)
         return
 
     def load_data(self, running_time_option) -> dict:
+        default_init_para = {'root': self.feddata['rawdata_path'], 'download':self.feddata['download'], 'train':True, 'transform':self.transform, 'pre_transform':self.pre_transform}
+        default_init_para.update(self.feddata['additional_option'])
+        if 'kwargs' not in self.builtin_class.__init__.__annotations__:
+            pop_key = [k for k in default_init_para.keys() if k not in self.builtin_class.__init__.__annotations__]
+            for k in pop_key: default_init_para.pop(k)
         # load the datasets
-        dataset = self.builtin_class(root=self.feddata['rawdata_path'], name=self.feddata['dataset_name'],
-                                     transform=self.transform)
-        dataset = dataset[self.feddata['perm']]
-        test_data = dataset[self.feddata['server_data']]
-        server_data_test, server_data_valid = self.split_dataset(test_data, running_time_option['test_holdout'])
-        task_data = {'server': {'test': server_data_test, 'valid': server_data_valid}}
+        dataset = self.builtin_class(**default_init_para)
+        k = int(len(self.feddata['test_idxs'])*running_time_option['test_holdout'])
+        valid_idxs = self.feddata['test_idxs'][:k]
+        test_idxs = self.feddata['test_idxs'][k:]
+        server_data_test = dataset[test_idxs]
+        server_data_valid = dataset[valid_idxs]
+        task_data = {'server': {'test': server_data_test if len(test_idxs)>0 else None, 'valid': server_data_valid if len(valid_idxs)>0 else None}}
         # rearrange data for clients
         for cid, cname in enumerate(self.feddata['client_names']):
-            cdata = self.feddata[cname]['data']
-            cdata_train, cdata_valid = self.split_dataset(cdata, running_time_option['train_holdout'])
-            task_data[cname] = {'train': cdata_train, 'valid': cdata_valid}
+            cdata_all = self.feddata[cname]['data']
+            ck = int(running_time_option['train_holdout']*len(cdata_all))
+            cdata_valid = cdata_all[:ck]
+            cdata_train = cdata_all[ck:]
+            if running_time_option['train_holdout'] > 0 and running_time_option['local_test']:
+                ck2 = int(0.5*ck)
+                cdata_test = cdata_valid[ck2:]
+                cdata_valid = cdata_valid[:ck2]
+            else:
+                cdata_test = []
+            task_data[cname] = {'train': dataset[cdata_train] if len(cdata_train)>0 else None, 'valid': dataset[cdata_valid] if len(cdata_valid)>0 else None, 'test': dataset[cdata_test] if len(cdata_test)>0 else None}
         return task_data
 
-
-class GraphClassificationTaskCalculator(BasicTaskCalculator):
+class GeneralCalculator(BasicTaskCalculator):
     def __init__(self, device, optimizer_name='sgd'):
-        super(GraphClassificationTaskCalculator, self).__init__(device, optimizer_name)
+        super(GeneralCalculator, self).__init__(device, optimizer_name)
         self.criterion = torch.nn.CrossEntropyLoss()
         self.DataLoader = DataLoader
 
     def compute_loss(self, model, data):
         """
         Args: model: the model to train
                  data: the training dataset
         Returns: dict of train-one-step's result, which should at least contains the key 'loss'
         """
         tdata = self.to_device(data)
-        outputs = model(tdata[0])
-        loss = self.criterion(outputs, tdata[-1])
+        outputs = model(tdata)
+        loss = self.criterion(outputs, tdata.y)
         return {'loss': loss}
 
     @torch.no_grad()
-    def test(self, model, dataset, batch_size=64, num_workers=0):
+    def test(self, model, dataset, batch_size=64, num_workers=0, pin_memory=False):
         """
         Metric = [mean_accuracy, mean_loss]
         Args:
             dataset:
                  batch_size:
         Returns: [mean_accuracy, mean_loss]
         """
         model.eval()
         if batch_size == -1: batch_size = len(dataset)
-        data_loader = self.get_dataloader(dataset, batch_size=batch_size, num_workers=num_workers)
+        data_loader = self.get_dataloader(dataset, batch_size=batch_size, num_workers=num_workers, pin_memory=pin_memory)
         total_loss = 0.0
         num_correct = 0
         for batch_id, batch_data in enumerate(data_loader):
             batch_data = self.to_device(batch_data)
-            outputs = model(batch_data[0])
-            batch_mean_loss = self.criterion(outputs, batch_data[-1]).item()
+            outputs = model(batch_data)
+            batch_mean_loss = self.criterion(outputs, batch_data.y).item()
             y_pred = outputs.data.max(1, keepdim=True)[1]
-            correct = y_pred.eq(batch_data[-1].data.view_as(y_pred)).long().cpu().sum()
+            correct = y_pred.eq(batch_data.y.data.view_as(y_pred)).long().cpu().sum()
             num_correct += correct.item()
-            total_loss += batch_mean_loss * len(batch_data[-1])
+            total_loss += batch_mean_loss * len(batch_data.y)
         return {'accuracy': 1.0 * num_correct / len(dataset), 'loss': total_loss / len(dataset)}
 
     def to_device(self, data):
-        return data[0].to(self.device), data[1].to(self.device)
+        return data.to(self.device)
 
-    def get_dataloader(self, dataset, batch_size=64, shuffle=True, num_workers=0):
+    def get_dataloader(self, dataset, batch_size=64, shuffle=True, num_workers=0, pin_memory=False):
         if self.DataLoader == None:
             raise NotImplementedError("DataLoader Not Found.")
-        return self.DataLoader(dataset, batch_size=batch_size, shuffle=shuffle, num_workers=num_workers)
+        return self.DataLoader(dataset, batch_size=batch_size, shuffle=shuffle, num_workers=num_workers, pin_memory=pin_memory)
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/toolkits/graph/horizontal/link_prediction.py` & `flgo-0.0.9/src/flgo/benchmark/toolkits/graph/link_prediction/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,125 +1,112 @@
 import copy
-
 import community.community_louvain
 import networkx as nx
 import torch_geometric
 from torch_geometric.transforms import RandomLinkSplit
+import torch_geometric.transforms as T
 from torch_geometric.utils import negative_sampling, from_networkx
 import torch_geometric.utils
 import collections
 
 from flgo.benchmark.base import *
 
-
-class LinkPredicitonTaskGenenerator(BasicTaskGenerator):
-    def __init__(self, benchmark, rawdata_path, builtin_class, dataset_name, transforms=None, num_clients=10):
-        super(LinkPredicitonTaskGenenerator, self).__init__(benchmark, rawdata_path)
+class BuiltinClassGenerator(BasicTaskGenerator):
+    def __init__(self, benchmark, rawdata_path, builtin_class, transform=None, pre_transform=None, test_rate=0.2, test_node_split=True, disjoint_train_ratio=0.3, neg_sampling_ratio=1.0):
+        super(BuiltinClassGenerator, self).__init__(benchmark, rawdata_path)
         self.builtin_class = builtin_class
-        self.dataset_name = dataset_name
-        self.transforms = transforms
-        self.num_clients = num_clients
+        self.transform = transform
+        self.pre_transform = pre_transform
+        self.test_rate = test_rate
+        self.test_node_split = test_node_split
+        self.disjoint_train_ratio = disjoint_train_ratio
+        self.neg_sampling_ratio = neg_sampling_ratio
+        self.download = False
 
     def load_data(self):
-        all_data = self.builtin_class(root=self.rawdata_path, name=self.dataset_name, transform=self.transforms).data
-        transform = RandomLinkSplit(is_undirected=all_data.is_undirected(), num_test=0.2, num_val=0,
-                                    add_negative_train_samples=False)
-        local_data, _, test_data = transform(all_data)
-        self.local_data_edge_label_index = local_data.edge_label_index
-        self.test_data_edge_label_index = test_data.edge_label_index
-        self.test_data_edge_label = test_data.edge_label
-        self.train_G = torch_geometric.utils.to_networkx(all_data, to_undirected=all_data.is_undirected(),
-                                                         node_attrs=['x'])
+        default_init_para = {'root': self.rawdata_path, 'download':self.download, 'train':True, 'transform':self.transform, 'pre_transform':self.pre_transform}
+        default_init_para.update(self.additional_option)
+        if 'kwargs' not in self.builtin_class.__init__.__annotations__:
+            pop_key = [k for k in default_init_para.keys() if k not in self.builtin_class.__init__.__annotations__]
+            for k in pop_key: default_init_para.pop(k)
+        self.dataset = self.builtin_class(**default_init_para).data
+        transform_for_create_test = T.RandomLinkSplit(neg_sampling_ratio=0.0, is_undirected=self.dataset.is_undirected(), num_test=self.test_rate, num_val=0, add_negative_train_samples=False)
+        _,_,test_data = transform_for_create_test(self.dataset)
+        self.test_nodes = list(set(test_data.edge_label_index.view(-1).tolist()))
+        all_nodes = list(set(self.dataset.edge_index.view(-1).tolist()))
+        self.train_nodes = list(set(all_nodes).difference(self.test_nodes)) if self.test_node_split else all_nodes
+        self.G = torch_geometric.utils.to_networkx(self.dataset, to_undirected=self.dataset.is_undirected(), node_attrs=['x', 'y', 'train_mask', 'val_mask', 'test_mask'])
+        self.train_data = nx.subgraph(self.G, self.train_nodes)
 
     def partition(self):
-        self.local_nodes = [[] for _ in range(self.num_clients)]
-        node_groups = community.community_louvain.best_partition(self.train_G)
-        groups = collections.defaultdict(list)
-        for ni, gi in node_groups.items():
-            groups[gi].append(ni)
-        groups = {k: groups[k] for k in list(range(len(groups)))}
-        # ensure the number of groups is larger than the number of clients
-        while len(groups) < self.num_clients:
-            # find the group with the largest size
-            groups_lens = [groups[k] for k in range(len(groups))]
-            max_gi = np.argmax(groups_lens)
-            # set the size of the new group
-            min_glen = min(groups_lens)
-            max_glen = max(groups_lens)
-            if max_glen < 2 * min_glen: min_glen = max_glen // 2
-            # split the group with the largest size into two groups
-            nodes_in_gi = groups[max_gi]
-            new_group_id = len(groups)
-            groups[new_group_id] = nodes_in_gi[:min_glen]
-            groups[max_gi] = nodes_in_gi[min_glen:]
-        # allocate different groups to clients
-        groups_lens = [groups[k] for k in range(len(groups))]
-        group_ids = np.argsort(groups_lens)
-        for gi in group_ids:
-            cid = np.argmin([len(li) for li in self.local_nodes])
-            self.local_nodes[cid].extend(groups[gi])
+        self.local_datas = self.partitioner(self.train_data)
+        self.num_clients = len(self.local_datas)
 
     def get_task_name(self):
         return '_'.join(['B-' + self.benchmark, 'P-None', 'N-' + str(self.num_clients)])
 
-
-class LinkPredicitonTaskPipe(BasicTaskPipe):
-    def __init__(self, task_name, buildin_class, transform=None):
-        super(LinkPredicitonTaskPipe, self).__init__(task_name)
-        self.builtin_class = buildin_class
+class BuiltinClassPipe(BasicTaskPipe):
+    def __init__(self, task_name, builtin_class, transform=None, pre_transform=None):
+        super(BuiltinClassPipe, self).__init__(task_name)
+        self.builtin_class = builtin_class
+        self.pre_transform = pre_transform
         self.transform = transform
 
     def save_task(self, generator):
-        client_names = self.gen_client_names(len(generator.local_nodes))
-        feddata = {'client_names': client_names,
-                   'server_data':
-                       {'edge_label_index': generator.test_data_edge_label_index.tolist(),
-                        'edge_label': generator.test_data_edge_label.tolist()},
-                   'rawdata_path': generator.rawdata_path,
-                   'dataset_name': generator.dataset_name,
-                   'local_edge_label_index': generator.local_data_edge_label_index.tolist()}
-        for cid in range(len(client_names)): feddata[client_names[cid]] = {'data': generator.local_nodes[cid]}
+        client_names = self.gen_client_names(len(generator.local_datas))
+        feddata = {'client_names': client_names, 'server_data': generator.test_nodes,
+                   'rawdata_path': generator.root, 'additional_option': generator.additional_option,
+                   'train_additional_option': generator.train_additional_option,
+                   'test_additional_option': generator.test_additional_option,
+                   'test_rate': generator.test_rate,
+                   'disjoint_train_ratio': generator.disjoint_train_ratio,
+                   'neg_sampling_ratio': generator.neg_sampling_ratio
+                   }
+        for cid in range(len(client_names)): feddata[client_names[cid]] = {'data': generator.local_datas[cid], }
         with open(os.path.join(self.task_path, 'data.json'), 'w') as outf:
             json.dump(feddata, outf)
         return
 
     def load_data(self, running_time_option) -> dict:
-        # load the datasets
-        all_data = self.builtin_class(root=self.feddata['rawdata_path'], name=self.feddata['dataset_name'],
-                                           transform=self.transform).data
-        server_data = copy.deepcopy(all_data)
-        server_data.edge_label_index = torch.Tensor(self.feddata['server_data']['edge_label_index'])
-        server_data.edge_label = torch.Tensor(self.feddata['server_data']['edge_label'])
-
-        local_data = copy.deepcopy(all_data)
-        local_data_edge_label_index = torch.Tensor(self.feddata['local_edge_label_index'])
-        edge_index = torch.cat([local_data_edge_label_index,
-                                           torch.flip(local_data_edge_label_index, dims=[0])], dim=1)
-        local_data.edge_index = edge_index
-        server_data.edge_index = edge_index
-        task_data = {'server': {'test': server_data}}
-        G = torch_geometric.utils.to_networkx(local_data, to_undirected=local_data.is_undirected(),
-                                              node_attrs=['x'])
+        default_init_para = {'root': self.feddata['rawdata_path'], 'download': True, 'train': True, 'transform': self.transform, 'pre_transform':self.pre_transform}
+        default_init_para.update(self.feddata['additional_option'])
+        if 'kwargs' not in self.builtin_class.__init__.__annotations__:
+            pop_key = [k for k in default_init_para.keys() if k not in self.builtin_class.__init__.__annotations__]
+            for k in pop_key: default_init_para.pop(k)
+        self.dataset = self.builtin_class(**default_init_para).data
+        self.G = torch_geometric.utils.to_networkx(self.dataset, to_undirected=self.dataset.is_undirected(), node_attrs=['x', 'y', 'train_mask', 'val_mask', 'test_mask'])
+        if self.feddata['test_rate']>0:
+            test_dataset = from_networkx(nx.subgraph(self.G, self.feddata['server_data']))
+            server_valid_data,_,server_test_data = T.RandomLinkSplit(neg_sampling_ratio=self.feddata['neg_sampling_ratio'],is_undirected=self.dataset.is_undirected(),num_test=1-running_time_option['test_holdout'], num_val=0.0, add_negative_train_samples=True)(test_dataset)
+            if len(server_valid_data.edge_label)==0:server_valid_data = None
+            if len(server_test_data.edge_label)==0:server_test_data = None
+        else:
+            server_test_data,server_valid_data = None,None
+        task_data = {'server': {'test': server_test_data, 'valid': server_valid_data}}
         # rearrange data for clients
+        if running_time_option['local_test']:
+            num_val = running_time_option['train_holdout']*0.5
+            num_test = running_time_option['train_holdout']*0.5
+        else:
+            num_val = running_time_option['train_holdout']
+            num_test = 0
         for cid, cname in enumerate(self.feddata['client_names']):
-            cdata = from_networkx(nx.subgraph(G, self.feddata[cname]['data']))
-            transform = RandomLinkSplit(is_undirected=cdata.is_undirected(), num_test=running_time_option['train_holdout'], num_val=0,
-                                        add_negative_train_samples=False)
-            train_data, _, val_data = transform(cdata)
-            task_data[cname] = {'train': train_data, 'valid': val_data}
+            c_dataset = from_networkx(nx.subgraph(self.G, self.feddata[cname]['data']))
+            ctrans = RandomLinkSplit(neg_sampling_ratio=self.feddata['neg_sampling_ratio'],is_undirected=self.dataset.is_undirected(), num_test=num_test, num_val=num_val,
+                                        add_negative_train_samples=False, disjoint_train_ratio=self.feddata['disjoint_train_ratio'])
+            cdata_train, cdata_valid, cdata_test = ctrans(c_dataset)
+            task_data[cname] = {'train': cdata_train, 'valid': cdata_valid if len(cdata_valid.edge_label)>0 else None, 'test':cdata_test if len(cdata_test.edge_label)>0 else None}
         return task_data
 
-
-class LinkPredicitonTaskCalculator(BasicTaskCalculator):
+class GeneralCalculator(BasicTaskCalculator):
     def __init__(self, device, optimizer_name='sgd'):
-        super(LinkPredicitonTaskCalculator, self).__init__(device, optimizer_name)
+        super(GeneralCalculator, self).__init__(device, optimizer_name)
         self.criterion = torch.nn.BCEWithLogitsLoss()
         self.DataLoader = torch_geometric.loader.DataLoader
 
-
     def compute_loss(self, model, data):
         tdata = self.data_to_device(data)
         z = model.encode(tdata.x, tdata.edge_label_index)
         neg_edge_index = negative_sampling(
             edge_index=tdata.edge_index, num_nodes=tdata.num_nodes,
             num_neg_samples=tdata.edge_label_index.size(1)
         )
@@ -132,15 +119,15 @@
             tdata.edge_label.new_zeros(neg_edge_index.size(1))
         ], dim=0)
         outputs = model.decode(z, edge_label_index).view(-1)
         loss = self.criterion(outputs, edge_label)
         return {'loss': loss}
 
     @torch.no_grad()
-    def test(self, model, dataset, batch_size=64, num_workers=0):
+    def test(self, model, dataset, batch_size=64, num_workers=0, pin_memory=False):
         total_loss = 0
         total_num_samples = 0
         tdata = self.data_to_device(dataset)
         z = model.encode(tdata.x, tdata.edge_index)
         outputs = model.decode(z, tdata.edge_label_index).view(-1)
         loss = self.criterion(outputs, tdata.edge_label)
         num_samples = len(tdata.x)
@@ -148,9 +135,9 @@
         total_num_samples += num_samples
         total_loss = total_loss.item()
         return {'loss': total_loss / total_num_samples}
 
     def data_to_device(self, data):
         return data.to(self.device)
 
-    def get_dataloader(self, dataset, batch_size=64, shuffle=True, num_workers=0):
-        return self.DataLoader([dataset], batch_size=batch_size, shuffle=shuffle)
+    def get_dataloader(self, dataset, batch_size=64, shuffle=True, num_workers=0, pin_memory=False):
+        return self.DataLoader([dataset], batch_size=batch_size, shuffle=shuffle, pin_memory=pin_memory)
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/toolkits/graph/horizontal/node_classification.py` & `flgo-0.0.9/src/flgo/benchmark/vertical_mnist_classification/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,154 +1,150 @@
-import community.community_louvain
-import torch_geometric.transforms as T
-from torch_geometric.utils import mask_to_index, index_to_mask, from_networkx
-import torch_geometric.utils
-import collections
-from flgo.benchmark.base import *
-import networkx as nx
-
-
-class NodeClassificationTaskGen(BasicTaskGenerator):
-    def __init__(self, benchmark, rawdata_path, builtin_class, dataset_name, transforms=None, num_clients=10):
-        super(NodeClassificationTaskGen, self).__init__(benchmark, rawdata_path)
-        self.builtin_class = builtin_class
-        self.dataset_name = dataset_name
-        self.transforms = transforms
-        self.num_clients = num_clients
-
-
-    def load_data(self):
-        self.all_data = T.RandomNodeSplit(split='train_rest', num_val=0.1, num_test=0.2)(
-            self.builtin_class(root=self.rawdata_path, name=self.dataset_name, transform=self.transforms).data)
-        self.test_nodes = mask_to_index(self.all_data.test_mask)
-        self.all_train_nodes = mask_to_index(self.all_data.train_mask)
-        self.all_val_nodes = mask_to_index(self.all_data.val_mask)
-        self.G = torch_geometric.utils.to_networkx(self.all_data, to_undirected=self.all_data.is_undirected(),
-                                                   node_attrs=['x', 'y', 'train_mask', 'val_mask', 'test_mask'])
-
+from flgo.benchmark.mnist_classification.core import builtin_class, transform
+from flgo.benchmark.base import BasicTaskPipe, BasicTaskCalculator
+from flgo.benchmark.toolkits.cv.classification import BuiltinClassGenerator
+import torch
+import os.path
+from torch.utils.data import Dataset
+import flgo
+import random
+import json
+
+class TaskGenerator(BuiltinClassGenerator):
+    def __init__(self, rawdata_path=os.path.join(flgo.benchmark.path,'RAW_DATA', 'MNIST')):
+        super(TaskGenerator, self).__init__('vertical_mnist_classification', rawdata_path, builtin_class, transform)
 
     def partition(self):
-        self.local_nodes = [[] for _ in range(self.num_clients)]
-        node_groups = community.community_louvain.best_partition(self.G)
-        groups = collections.defaultdict(list)
-        for ni, gi in node_groups.items():
-            groups[gi].append(ni)
-        groups = {k: groups[k] for k in list(range(len(groups)))}
-        # ensure the number of groups is larger than the number of clients
-        while len(groups) < self.num_clients:
-            # find the group with the largest size
-            groups_lens = [groups[k] for k in range(len(groups))]
-            max_gi = np.argmax(groups_lens)
-            # set the size of the new group
-            min_glen = min(groups_lens)
-            max_glen = max(groups_lens)
-            if max_glen < 2 * min_glen: min_glen = max_glen // 2
-            # split the group with the largest size into two groups
-            nodes_in_gi = groups[max_gi]
-            new_group_id = len(groups)
-            groups[new_group_id] = nodes_in_gi[:min_glen]
-            groups[max_gi] = nodes_in_gi[min_glen:]
-        # allocate different groups to clients
-        groups_lens = [groups[k] for k in range(len(groups))]
-        group_ids = np.argsort(groups_lens)
-        for gi in group_ids:
-            cid = np.argmin([len(li) for li in self.local_nodes])
-            self.local_nodes[cid].extend(groups[gi])
+        self.local_datas = self.partitioner(self.train_data)
+        self.num_objects = len(self.local_datas)
+        if self.test_data is not None:
+            self.test_local_datas = [{'sample_idxs':list(range(len(self.test_data))), 'pt_feature':pdata['pt_feature'], 'with_label':pdata['with_label']} for pdata in self.local_datas]
 
     def get_task_name(self):
-        return '_'.join(['B-'+self.benchmark,  'P-None', 'N-'+str(self.num_clients)])
+        return '_'.join(['B-' + self.benchmark, 'P-' + str(self.partitioner), 'N-' + str(self.partitioner.num_parties)])
 
-
-class NodeClassificationTaskPipe(BasicTaskPipe):
-    def __init__(self, task_name, buildin_class, transform=None):
-        super(NodeClassificationTaskPipe, self).__init__(task_name)
-        self.builtin_class = buildin_class
+class PartialDataset(Dataset):
+    def __init__(self, dataset, pt_feature=None, with_label=False, sample_idxs = []):
+        self.dataset = dataset
+        self.sample_idxs = sample_idxs
+        self.pt_feature = pt_feature
+        self.with_label = with_label
+
+    def gen_id(self, *args, **kwargs) -> list:
+        return list(range(len(self.dataset)))
+
+    def partition(self, x):
+        return (torch.split(x, self.pt_feature[1], dim=self.pt_feature[0]))[self.pt_feature[2]]
+
+    def is_with_label(self):
+        return self.with_label
+
+    def __len__(self):
+        return len(self.sample_idxs)
+
+    def __getitem__(self, item):
+        sidx = self.sample_idxs[item]
+        x,y = self.dataset[sidx][0], self.dataset[sidx][1]
+        sid = self.dataset.ids[sidx]
+        if self.with_label:
+            return self.partition(x), y, sid
+        else:
+            return self.partition(x), None, sid
+
+    def get_batch_by_id(self, ids):
+        try:
+            xs = [self.partition(self.dataset[sid][0]) for sid in ids]
+            ys = [self.dataset[sid][1] for sid in ids]
+        except:
+            raise ValueError("sample with id={} doesn't exists in the current dataset")
+        return torch.stack(xs), torch.LongTensor(ys), ids
+
+class TaskPipe(BasicTaskPipe):
+    TaskDataset = PartialDataset
+    def __init__(self, task_name):
+        super().__init__(task_name)
+        self.builtin_class = builtin_class
         self.transform = transform
 
     def save_task(self, generator):
-        client_names = self.gen_client_names(len(generator.local_nodes))
-        feddata = {'client_names': client_names,
-                   'server_data': generator.test_nodes.tolist(),
-                   'rawdata_path': generator.rawdata_path,
-                   'dataset_name': generator.dataset_name,
-                   'all_train_nodes': generator.all_train_nodes.tolist(),
-                   'all_val_nodes': generator.all_val_nodes.tolist()}
-        for cid in range(len(client_names)): feddata[client_names[cid]] = {'data': generator.local_nodes[cid]}
+        party_names = self.gen_client_names(len(generator.local_datas))
+        feddata = {'party_names': party_names,'rawdata_path': generator.root, 'additional_option': generator.additional_option}
+        for pid in range(len(party_names)):
+            feddata[party_names[pid]] = {
+                'data':{
+                    'with_label': generator.local_datas[pid]['with_label'],
+                    'pt_feature': generator.local_datas[pid]['pt_feature'],
+                    'train':generator.local_datas[pid]['sample_idxs'],
+                    'test': generator.test_local_datas[pid]['sample_idxs'],
+                },
+            }
         with open(os.path.join(self.task_path, 'data.json'), 'w') as outf:
             json.dump(feddata, outf)
-        return
 
     def load_data(self, running_time_option) -> dict:
         # load the datasets
-        self.all_data = self.builtin_class(root=self.feddata['rawdata_path'], name=self.feddata['dataset_name'],
-                                           transform=self.transform).data
-        self.all_data.test_mask = index_to_mask(torch.LongTensor(self.feddata['server_data']),
-                                                size=self.all_data.num_nodes)
-        self.all_data.train_mask = index_to_mask(torch.LongTensor(self.feddata['all_train_nodes']),
-                                                 size=self.all_data.num_nodes)
-        self.all_data.val_mask = index_to_mask(torch.LongTensor(self.feddata['all_val_nodes']),
-                                               size=self.all_data.num_nodes)
-        task_data = {'server': {'test': self.all_data}}
-        G = torch_geometric.utils.to_networkx(self.all_data, to_undirected=self.all_data.is_undirected(),
-                                              node_attrs=['x', 'y', 'train_mask', 'val_mask', 'test_mask'])
-        # rearrange data for clients
-        for cid, cname in enumerate(self.feddata['client_names']):
-            cdata = from_networkx(nx.subgraph(G, self.feddata[cname]['data']))
-            cdata.test_mask = cdata.val_mask
-            task_data[cname] = {'train': cdata, 'valid': cdata}
+        train_data = self.builtin_class(root=self.feddata['rawdata_path'], download=True, train=True, transform=self.transform, **self.feddata['additional_option'])
+        test_data = self.builtin_class(root=self.feddata['rawdata_path'], download=True, train=False, transform=self.transform, **self.feddata['additional_option'])
+        train_data.ids = list(range(len(train_data)))
+        test_data.ids = list(range(len(test_data)))
+        train_sidxs = list(range(len(train_data)))
+        random.shuffle(train_sidxs)
+        valid_sample_idxs = train_sidxs[:int(len(train_data)* running_time_option['train_holdout'])]
+        train_sample_idxs = train_sidxs[int(len(train_data)* running_time_option['train_holdout']):]
+        task_data = {}
+        for pid, party_name in enumerate(self.feddata['party_names']):
+            pdata = self.feddata[party_name]['data']
+            with_label, pt_feature, train_idxs, test_idxs = pdata['with_label'], pdata['pt_feature'], pdata['train'], pdata['test']
+            local_train_data = self.TaskDataset(train_data, pt_feature, with_label, train_sample_idxs)
+            local_valid_data = self.TaskDataset(train_data, pt_feature, with_label, valid_sample_idxs)
+            local_test_data = self.TaskDataset(test_data, pt_feature, with_label, test_idxs)
+            task_data[party_name] = {'train':local_train_data, 'valid':local_valid_data, 'test':local_test_data}
         return task_data
 
-"""
-load_data -> return task_data = {
-    'server': {'test': anything, 'xxx': anything},
-    'Client01': {'train': anything, ...}
-    ...
-}
-
-generate_objects -> [object1, object2, ...]
-object1.name = task_data[0] = 'server'
-object2.name = task_data[1] = 'Client01'
-....
-
-distribute:
-    specify the object according to the name of the object
-        object_x
-        x_data = task_data[x_name] (i.e. {'xxx':anything, ...})
-        for key in x_data:
-            object_x.set_data(key, x_data[key])
-            
-set_data(data_name, data):
-    setattr(self, data_name+'_data', data)
-    
-"""
-class NodeClassificationTaskCalculator(BasicTaskCalculator):
+class TaskCalculator(BasicTaskCalculator):
     def __init__(self, device, optimizer_name='sgd'):
-        super(NodeClassificationTaskCalculator, self).__init__(device, optimizer_name)
-        self.criterion = torch.nn.NLLLoss()
-        self.DataLoader = torch_geometric.loader.DataLoader
+        super(TaskCalculator, self).__init__(device, optimizer_name)
+        self.criterion = torch.nn.CrossEntropyLoss()
+        self.DataLoader = torch.utils.data.DataLoader
 
     def compute_loss(self, model, data):
-        tdata = self.data_to_device(data)
-        outputs = model(tdata)
-        loss = self.criterion(outputs[tdata.train_mask], tdata.y[tdata.train_mask])
+        """
+        Args: model: the model to train
+                 data: the training dataset
+        Returns: dict of train-one-step's result, which should at least contains the key 'loss'
+        """
+        model.to(self.device)
+        tdata = self.to_device(data)
+        outputs = model(tdata[0])
+        loss = self.criterion(outputs, tdata[-1])
         return {'loss': loss}
 
     @torch.no_grad()
     def test(self, model, dataset, batch_size=64, num_workers=0):
-        loader = self.DataLoader([dataset], batch_size=batch_size)
-        total_loss = 0
-        total_num_samples = 0
-        for batch in loader:
-            tdata = self.data_to_device(batch)
-            outputs = model(tdata)
-            loss = self.criterion(outputs[tdata.test_mask], tdata.y[tdata.test_mask])
-            num_samples = len(tdata.x)
-            total_loss += num_samples * loss
-            total_num_samples += num_samples
-        total_loss = total_loss.item()
-        return {'loss': total_loss / total_num_samples}
+        """
+        Metric = [mean_accuracy, mean_loss]
+        Args: model:
+                 dataset:
+                 batch_size:
+        Returns: [mean_accuracy, mean_loss]
+        """
+        model.eval()
+        if batch_size==-1:batch_size=len(dataset)
+        data_loader = self.get_dataloader(dataset, batch_size=batch_size, num_workers=num_workers)
+        total_loss = 0.0
+        num_correct = 0
+        for batch_id, batch_data in enumerate(data_loader):
+            batch_data = self.to_device(batch_data)
+            outputs = model(batch_data[0])
+            batch_mean_loss = self.criterion(outputs, batch_data[-1]).item()
+            y_pred = outputs.data.max(1, keepdim=True)[1]
+            correct = y_pred.eq(batch_data[-1].data.view_as(y_pred)).long().cpu().sum()
+            num_correct += correct.item()
+            total_loss += batch_mean_loss * len(batch_data[-1])
+        return {'accuracy': 1.0*num_correct/len(dataset), 'loss':total_loss/len(dataset)}
 
-    def data_to_device(self, data):
-        return data.to(self.device)
+    def to_device(self, data):
+        return data[0].to(self.device), data[1].to(self.device)
 
     def get_dataloader(self, dataset, batch_size=64, shuffle=True, num_workers=0):
-        return self.DataLoader([dataset], batch_size=batch_size, shuffle=shuffle)
+        if self.DataLoader == None:
+            raise NotImplementedError("DataLoader Not Found.")
+        return self.DataLoader(dataset, batch_size=batch_size, shuffle=shuffle, num_workers=num_workers)
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/toolkits/partition.py` & `flgo-0.0.9/src/flgo/benchmark/toolkits/partition.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 r"""
 This file contains preset partitioners for the benchmarks.
 All the Partitioner should implement the method `__call__(self, data)`
 where `data` is the dataset to be partitioned and the return is a list of the partitioned result.
 
 For example, The IIDPartitioner.__call__ receives a indexable object (i.e. instance of torchvision.datasets.mnsit.MNSIT)
-and I.I.D. selects samples' indices in the original dataset as each client's local data.
+and I.I.D. selects samples' indices in the original dataset as each client's local_movielens_recommendation data.
 The list of list of sample indices are finally returnerd (e.g. [[0,1,2,...,1008], ...,[25,23,98,...,997]]).
 
 To use the partitioner, you can specify Partitioner in the configuration dict for `flgo.gen_task`.
  Example 1: passing the parameter of __init__ of the Partitioner through the dict `para`
 >>>import flgo
 >>>config = {'benchmark':{'name':'flgo.benchmark.mnist_classification'},
 ...            'partitioner':{'name':'IIDPartitioner', 'para':{'num_clients':20, 'alpha':1.0}}}
 >>>flgo.gen_task(config, './test_partition')
 """
 
 from abc import abstractmethod, ABCMeta
 import random
 import numpy as np
 import collections
-
 import torch
+try:
+    import community.community_louvain
+except:
+    pass
 
 class AbstractPartitioner(metaclass=ABCMeta):
     @abstractmethod
     def __call__(self, *args, **kwargs):
         pass
 
 class BasicPartitioner(AbstractPartitioner):
@@ -45,15 +48,15 @@
 
         Args:
             num_clients (int): the number of clients
             datasize (int): the total data size
             imbalance (float): the degree of data imbalance across clients
 
         Returns:
-            a list of integer numbers that represents local data sizes
+            a list of integer numbers that represents local_movielens_recommendation data sizes
         """
         if imbalance == 0:
             samples_per_client = [int(datasize / num_clients) for _ in range(num_clients)]
             for _ in range(datasize % num_clients): samples_per_client[_] += 1
         else:
             imbalance = max(0.1, imbalance)
             sigma = imbalance
@@ -99,15 +102,15 @@
         return samples_per_client
 
 class IIDPartitioner(BasicPartitioner):
     """`Partition the indices of samples in the original dataset indentically and independently.
 
     Args:
         num_clients (int, optional): the number of clients
-        imbalance (float, optional): the degree of imbalance of the amounts of different local data (0<=imbalance<=1)
+        imbalance (float, optional): the degree of imbalance of the amounts of different local_movielens_recommendation data (0<=imbalance<=1)
     """
     def __init__(self, num_clients=100, imbalance=0):
         self.num_clients = num_clients
         self.imbalance = imbalance
 
     def __str__(self):
         name = "iid"
@@ -124,15 +127,15 @@
 class DirichletPartitioner(BasicPartitioner):
     """`Partition the indices of samples in the original dataset according to Dirichlet distribution of the
     particular attribute. This way of partition is widely used by existing works in federated learning.
 
     Args:
         num_clients (int, optional): the number of clients
         alpha (float, optional): `alpha`(i.e. alpha>=0) in Dir(alpha*p) where p is the global distribution. The smaller alpha is, the higher heterogeneity the data is.
-        imbalance (float, optional): the degree of imbalance of the amounts of different local data (0<=imbalance<=1)
+        imbalance (float, optional): the degree of imbalance of the amounts of different local_movielens_recommendation data (0<=imbalance<=1)
         error_bar (float, optional): the allowed error when the generated distribution mismatches the distirbution that is actually wanted, since there may be no solution for particular imbalance and alpha.
         flag_index (int, optional): the index of the distribution-dependent (i.e. label) attribute in each sample.
     """
     def __init__(self, num_clients=100, alpha=1.0, error_bar=1e-6, imbalance=0, flag_index=-1):
         self.num_clients = num_clients
         self.alpha = alpha
         self.imbalance = imbalance
@@ -146,18 +149,19 @@
 
     def __call__(self, data):
         attrs = [d[self.flag_index] for d in data]
         num_attrs = len(set(attrs))
         samples_per_client = self.data_imbalance_generator(self.num_clients, len(data), self.imbalance)
         # count the label distribution
         lb_counter = collections.Counter(attrs)
+        lb_names = list(lb_counter.keys())
         p = np.array([1.0 * v / len(data) for v in lb_counter.values()])
         lb_dict = {}
         attrs = np.array(attrs)
-        for lb in range(len(lb_counter.keys())):
+        for lb in lb_names:
             lb_dict[lb] = np.where(attrs == lb)[0]
         proportions = [np.random.dirichlet(self.alpha * p) for _ in range(self.num_clients)]
         while np.any(np.isnan(proportions)):
             proportions = [np.random.dirichlet(self.alpha * p) for _ in range(self.num_clients)]
         sorted_cid_map = {k: i for k, i in zip(np.argsort(samples_per_client), [_ for _ in range(self.num_clients)])}
         error_increase_interval = 500
         max_error = self.error_bar
@@ -195,17 +199,17 @@
                     break
             if len(alter_norms) > 0 and min(alter_norms) < error_norm:
                 alcid = np.argmin(alter_norms)
                 proportions[excid] = sup_prop[alcid]
             loop_count += 1
         local_datas = [[] for _ in range(self.num_clients)]
         self.dirichlet_dist = []  # for efficiently visualizing
-        for lb in lb_counter.keys():
+        for lb in lb_names:
             lb_idxs = lb_dict[lb]
-            lb_proportion = np.array([pi[lb] * si for pi, si in zip(proportions, samples_per_client)])
+            lb_proportion = np.array([pi[lb_names.index(lb)] * si for pi, si in zip(proportions, samples_per_client)])
             lb_proportion = lb_proportion / lb_proportion.sum()
             lb_proportion = (np.cumsum(lb_proportion) * len(lb_idxs)).astype(int)[:-1]
             lb_datas = np.split(lb_idxs, lb_proportion)
             self.dirichlet_dist.append([len(lb_data) for lb_data in lb_datas])
             local_datas = [local_data + lb_data.tolist() for local_data, lb_data in zip(local_datas, lb_datas)]
         self.dirichlet_dist = np.array(self.dirichlet_dist).T
         for i in range(self.num_clients): np.random.shuffle(local_datas[i])
@@ -215,15 +219,15 @@
 class DiversityPartitioner(BasicPartitioner):
     """`Partition the indices of samples in the original dataset according to numbers of types of a particular
     attribute (e.g. label) . This way of partition is widely used by existing works in federated learning.
 
     Args:
         num_clients (int, optional): the number of clients
         diversity (float, optional): the ratio of locally owned types of the attributes (i.e. the actual number=diversity * total_num_of_types)
-        imbalance (float, optional): the degree of imbalance of the amounts of different local data (0<=imbalance<=1)
+        imbalance (float, optional): the degree of imbalance of the amounts of different local_movielens_recommendation data (0<=imbalance<=1)
         flag_index (int, optional): the index of the distribution-dependent (i.e. label) attribute in each sample.
     """
     def __init__(self, num_clients=100, diversity=1.0, flag_index=-1):
         self.num_clients = num_clients
         self.diversity = diversity
         self.flag_index = flag_index
 
@@ -272,15 +276,15 @@
 
 class GaussianPerturbationPartitioner(BasicPartitioner):
     """`Partition the indices of samples I.I.D. and bind additional and static gaussian noise to each sample, which is
     a setting of feature skew in federated learning.
 
     Args:
         num_clients (int, optional): the number of clients
-        imbalance (float, optional): the degree of imbalance of the amounts of different local data (0<=imbalance<=1)
+        imbalance (float, optional): the degree of imbalance of the amounts of different local_movielens_recommendation data (0<=imbalance<=1)
         sigma (float, optional): the degree of feature skew
         scale (float, optional): the standard deviation of noise
         feature_index (int, optional): the index of the feature to be processed for each sample.
     """
     def __init__(self, num_clients=100, imbalance=0.0, sigma=0.1, scale=0.1, feature_index=0):
         self.num_clients = num_clients
         self.imbalance = imbalance
@@ -311,40 +315,44 @@
 
 class IDPartitioner(BasicPartitioner):
     """`Partition the indices of samples I.I.D. according to the ID of each sample, which requires the passed parameter
     `data` has attribution `id`.
 
     Args:
         num_clients (int, optional): the number of clients
-        priority (str, optional): The value should be in set ('random', 'max', 'min'). If the number of clients is smaller than the total number of all the clients, this term will decide the selected clients according to their local data sizes.
+        priority (str, optional): The value should be in set ('random', 'max', 'min'). If the number of clients is smaller than the total number of all the clients, this term will decide the selected clients according to their local_movielens_recommendation data sizes.
     """
-    def __init__(self, num_clients=-1, priority='random'):
+    def __init__(self, num_clients=-1, priority='random', flag=None):
         self.num_clients = int(num_clients)
         self.priorty = priority
-        return
+        self.flag = flag
 
     def __str__(self):
         return 'id'
 
     def __call__(self, data):
         all_data = list(range(len(data)))
-        data_owners = data.id
+        if self.flag is not None:
+            data_owners = [d[self.flag] for d in data]
+        else:
+            data_owners = data.id
         local_datas = collections.defaultdict(list)
         for idx in range(len(all_data)):
-            local_datas[data_owners[idx]].append(all_data[idx])
+            local_datas[data_owners[idx]].append(idx)
         local_datas = list(local_datas.values())
         if self.num_clients < 0:
             self.num_clients = len(local_datas)
         elif self.priorty == 'max':
             local_datas = sorted(local_datas, key=lambda x: len('x'), reverse=True)[:self.num_clients]
         elif self.priorty == 'min':
             local_datas = sorted(local_datas, key=lambda x: len('x'))[:self.num_clients]
         elif self.priorty == 'random':
             random.shuffle(local_datas)
             local_datas = local_datas[:self.num_clients]
+        local_datas = sorted(local_datas, key=lambda x:data[x[0]][self.flag] if self.flag is not None else data.id[x[0]])
         return local_datas
 
 class VerticalSplittedPartitioner(BasicPartitioner):
     """`Partition the indices and shapes of samples in the original dataset for vertical federated learning. Different
     to the above partitioners, the partitioner.__call__ returns more flexible partition information instead of the indices that
     can be used to rebuild the partitioned data.
 
@@ -395,8 +403,47 @@
             return None
         if k == 1:
             if n >= l:
                 yield (n,)
             return None
         for i in range(l, n + 1):
             for result in self.integer_k_partition(n - i, k - 1, i):
-                yield (i,) + result
+                yield (i,) + result
+
+class NodeLouvainPartitioner(BasicPartitioner):
+    """
+    """
+    def __init__(self, num_clients=100):
+        self.num_clients = num_clients
+
+    def __str__(self):
+        name = "Louvain"
+        return name
+
+    def __call__(self, data):
+        local_nodes = [[] for _ in range(self.num_clients)]
+        self.node_groups = community.community_louvain.best_partition(data)
+        groups = collections.defaultdict(list)
+        for ni, gi in self.node_groups.items():
+            groups[gi].append(ni)
+        groups = {k: groups[k] for k in list(range(len(groups)))}
+        # ensure the number of groups is larger than the number of clients
+        while len(groups) < self.num_clients:
+            # find the group with the largest size
+            groups_lens = [groups[k] for k in range(len(groups))]
+            max_gi = np.argmax(groups_lens)
+            # set the size of the new group
+            min_glen = min(groups_lens)
+            max_glen = max(groups_lens)
+            if max_glen < 2 * min_glen: min_glen = max_glen // 2
+            # split the group with the largest size into two groups
+            nodes_in_gi = groups[max_gi]
+            new_group_id = len(groups)
+            groups[new_group_id] = nodes_in_gi[:min_glen]
+            groups[max_gi] = nodes_in_gi[min_glen:]
+        # allocate different groups to clients
+        groups_lens = [groups[k] for k in range(len(groups))]
+        group_ids = np.argsort(groups_lens)
+        for gi in group_ids:
+            cid = np.argmin([len(li) for li in local_nodes])
+            local_nodes[cid].extend(groups[gi])
+        return local_nodes
```

### Comparing `flgo-0.0.8/src/flgo/benchmark/vertical_mnist_classification/model/mlp.py` & `flgo-0.0.9/src/flgo/benchmark/vertical_mnist_classification/model/mlp.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/experiment/analyzer.py` & `flgo-0.0.9/src/flgo/experiment/analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,20 +164,22 @@
 class Selector:
     r"""
     Filter the records and read them into memory accoring to customized settings
     
     Args:
         selector_config (dict): the dictionary that is used to filter records
 
-    Example::
+    Example:
+    ```python
         >>> task='./my_task'
         >>> selector = Selector({'task':task, 'header':['fedavg'], 'filter':{'lr':0.1}})
         >>> selector.records[task]
         >>> # selector.records is a dict where selector.records[task] is a list
         >>> # of the records that pass the filter
+    ```
     """
     def __init__(self, selector_config):
         self.config = selector_config
         self.tasks = [selector_config['task']] if type(selector_config['task']) is not list else selector_config['task']
         self.headers = selector_config['header'] if type(selector_config['header']) is list else [selector_config['header']]
         self.filter = selector_config['filter'] if 'filter' in selector_config.keys() else {}
         self.legend_with = selector_config['legend_with'] if 'legend_with' in selector_config.keys() else []
@@ -259,28 +261,30 @@
 
     Args:
         rec (Record): the record
         args (dict): the painting arguments
         obj_option (dict): the personal option for each object
         draw_func (str): optional, the function name. All the subclass of this class won't claim this parameter.
 
-    Example::
+    Example:
+    ```python
         >>> class GroupCurve(PaintObject):
         ...     def __init__(self, rec, args,  obj_option):
         ...         super(GroupCurve, self).__init__(rec, args, obj_option, '')
         ...
         ...     def draw(self, ax):
         ...         x = self.rec.data[self.args['x']]
         ...         ykey = self.args['y']
         ...         mean_y = self.rec.data[ykey]
         ...         min_y = np.min(np.array([d[ykey] for d in self.rec.datas]), axis=0)
         ...         max_y = np.max(np.array([d[ykey] for d in self.rec.datas]), axis=0)
         ...         ax.plot(x, mean_y, label=self.rec.data['label'])
         ...         ax.fill_between(x, max_y, min_y, alpha=0.3)
         ...         ax.legend()
+    ```
     """
     def __init__(self, rec: Record, args: dict,  obj_option: dict, draw_func: str):
         self.rec = rec
         self.args = args
         self.obj_option = obj_option
         self.draw_func = draw_func
         self.para = (rec.data[v] for v in args.values())
@@ -364,17 +368,19 @@
                 'fig_option':{...}, # the options of the figure such as title, xlabel, xlim, no_legend
             }
         
         Args:
             object_class (class|str): the types of the obejct to be drawed
             fig_config (dict): the drawing configuration
 
-        Example::
+        Example:
+        ```python
             >>> p=Painter(records)
             >>> p.create_figure(Curve, {'args':{'x':'communication_round', 'y':'valid_loss'}})
+        ```
         """
         object_class = eval(object_class) if type(object_class) is str else object_class
         if 'split' in  fig_config.keys():
             cols = fig_config['split']['cols'] if 'cols' in fig_config['split'] else 4
             rows = int(math.ceil(len(self.records)/cols))
             cols = min(len(self.records), cols)
             if 'figsize' in fig_config['split']:
@@ -612,18 +618,20 @@
         in this column is v_k=func(Record_k, col_option), where func can be 
         arbitrarily customized.
 
         Args:
             func (func|str): the name of the function or the function
             col_option (dict|str): the option of the column to index data in each record
 
-        Example::
+        Example:
+        ```python
             >>> tb = Table(records)
             >>> tb.add_column(min_value, col_option={'x':'valid_loss'})
             >>> tb.print()
+        ```
         """
         func = eval(func) if type(func) is str else func
         col_option = {'x': col_option} if type(col_option) is not dict else col_option
         column = []
         for rec in self.records:
             column.append(func(rec, col_option))
         if 'name' in col_option.keys():
@@ -654,26 +662,28 @@
     Args:
         config (dict|str): the analysis plan
         save_figure (bool): whether to save figures
         save_text (bool): whether to save table as .txt file
         path (str): the path to store the results
         seed (int): random seed
 
-    Example::
+    Example:
+    ```python
         >>> import flgo.experiment.analyzer as al
         >>> # only records of fedavg running on the task 'my_task' with learning rate lr<=0.01 will be selected
         >>> selector_config = {'task':'./my_task', 'header':['fedavg'], 'filter':['LR':'<=0.1']}
         >>> # draw the learning curve on the validation dataset
         >>> painter_config = {'Curve':[{'args':{'x':'communication_round', 'y':'valid_loss'}}]}
         >>> # show the minimal value of validation loss
         >>> table_config = {'min_value':[{'x':'valid_loss'}]}
         >>> # create analysis plan
         >>> analysis_plan = {'Selector':selector_config, 'Painter':painter_config, 'Table':table_config}
         >>> # call this function
         >>> al.show(analysis_plan)
+    ```
     """
     random.seed(seed)
     np.random.seed(seed)
     option = load_configuration(config)
     record_selector = Selector(option['Selector'])
     if 'Painter' in option.keys():
         painter = Painter(record_selector.all_records, save_figure=save_figure, path=path)
```

### Comparing `flgo-0.0.8/src/flgo/experiment/device_scheduler.py` & `flgo-0.0.9/src/flgo/experiment/device_scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,19 +86,21 @@
         devices (list): a list of the index numbers of GPUs
         put_interval (int, optional): the minimal time interval (i.e. seconds) to allocate the same device
         mean_memory_occupated (int, optional): the initial mean memory occupation (i.e. MB) for all the runners
         available_interval (int, optional): a gpu will be returned only if it is kept available for a period longer than this term
         dynamic_memory_occupated (bool, optional): whether to dynamically estimate the memory occupation
         dynamic_condition (str): 'mean' or 'max'
 
-    Example::
+    Example:
+    ```python
         >>> import flgo.experiment.device_scheduler
         >>> sc = flgo.experiment.device_scheduler.AutoScheduler([0,1])
         >>> import flgo
         >>> flgo.multi_init_and_run(runner_args, scheduler=sc)
+    ```
     """
     def __init__(self, devices:list, put_interval = 5, mean_memory_occupated = 1000, available_interval=5, dynamic_memory_occupated=True, dynamic_condition='mean'):
         super(AutoScheduler, self).__init__(devices)
         pynvml.nvmlInit()
         crt_time = time.time()
         self.dev_state = {
             dev:{
```

### Comparing `flgo-0.0.8/src/flgo/experiment/logger/__init__.py` & `flgo-0.0.9/src/flgo/experiment/logger/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 r"""
 This module is to help conduct experiments in federated learning by providing high-level APIs to
 records information during running-time. To customized the logger, anyone should overwrite the three
 methods:
+
+Example:
+```python
 >>> import flgo.experiment.logger
 >>> class MyLogger(flgo.experiment.logger.BasicLogger):
 ...     def initialize(self):
 ...         # make necessary initialization here
 ...         pass
 ...
 ...     def log_once(self):
@@ -14,14 +17,16 @@
 ...         # that will be saved into .json after the training finishes).
 ...         pass
 ...
 ...     def organize_output(self):
 ...         # organize the variables in self.output here before saving it into .json file
 ...         pass
 >>> runner = flgo.init(task, algorithm=fedavg, Logger=MyLogger)
+```
+
 Then the customized Logger will be used to record running-time variables.
 
 The Logger is also used to enable early stopping, where 'valid_loss' must be a key in self.output if
 early stopping is enabled. We also provide several preset loggers like BasicLogger, SimpleLogger, TuneLogger.
 """
 import torch.multiprocessing
 import sys, os, time, io, traceback, warnings, weakref, collections.abc
@@ -2239,15 +2244,19 @@
         return
 
     def show_current_output(self, yes_key=['train', 'test', 'valid'], no_key=['dist']):
         for key, val in self.output.items():
             a = [(yk in key) for yk in yes_key]
             nf = [(nk not in key) for nk in no_key]
             if np.all(nf) and np.any(a):
-                self.info(self.temp.format(key, val[-1]))
+                try:
+                    content = self.temp.format(key, val[-1])
+                except:
+                    content = "{}:".format(key)+str(val[-1])
+                self.info(content)
 
     def get_output_name(self, suffix='.json'):
         if not hasattr(self, 'option'): raise NotImplementedError('logger has no attr named "option"')
         header = "{}_".format(self.option["algorithm"])
         if hasattr(self, 'coordinator'):
             for para, pv in self.coordinator.algo_para.items():
                 header = header + para + "{}_".format(pv)
```

### Comparing `flgo-0.0.8/src/flgo/experiment/logger/config.py` & `flgo-0.0.9/src/flgo/experiment/logger/config.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/experiment/logger/handlers.py` & `flgo-0.0.9/src/flgo/experiment/logger/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -728,22 +728,22 @@
     LOG_NEWS      = 7       #  network news subsystem
     LOG_UUCP      = 8       #  UUCP subsystem
     LOG_CRON      = 9       #  clock daemon
     LOG_AUTHPRIV  = 10      #  security/authorization messages (private)
     LOG_FTP       = 11      #  FTP daemon
 
     #  other codes through 15 reserved for system use
-    LOG_LOCAL0    = 16      #  reserved for local use
-    LOG_LOCAL1    = 17      #  reserved for local use
-    LOG_LOCAL2    = 18      #  reserved for local use
-    LOG_LOCAL3    = 19      #  reserved for local use
-    LOG_LOCAL4    = 20      #  reserved for local use
-    LOG_LOCAL5    = 21      #  reserved for local use
-    LOG_LOCAL6    = 22      #  reserved for local use
-    LOG_LOCAL7    = 23      #  reserved for local use
+    LOG_LOCAL0    = 16      #  reserved for local_movielens_recommendation use
+    LOG_LOCAL1    = 17      #  reserved for local_movielens_recommendation use
+    LOG_LOCAL2    = 18      #  reserved for local_movielens_recommendation use
+    LOG_LOCAL3    = 19      #  reserved for local_movielens_recommendation use
+    LOG_LOCAL4    = 20      #  reserved for local_movielens_recommendation use
+    LOG_LOCAL5    = 21      #  reserved for local_movielens_recommendation use
+    LOG_LOCAL6    = 22      #  reserved for local_movielens_recommendation use
+    LOG_LOCAL7    = 23      #  reserved for local_movielens_recommendation use
 
     priority_names = {
         "alert":    LOG_ALERT,
         "crit":     LOG_CRIT,
         "critical": LOG_CRIT,
         "debug":    LOG_DEBUG,
         "emerg":    LOG_EMERG,
@@ -794,15 +794,15 @@
 
     def __init__(self, address=('localhost', SYSLOG_UDP_PORT),
                  facility=LOG_USER, socktype=None):
         """
         Initialize a handler.
 
         If address is specified as a string, a UNIX socket is used. To log to a
-        local syslogd, "SysLogHandler(address="/dev/log")" can be used.
+        local_movielens_recommendation syslogd, "SysLogHandler(address="/dev/log")" can be used.
         If facility is not specified, LOG_USER is used. If socktype is
         specified as socket.SOCK_DGRAM or socket.SOCK_STREAM, that specific
         socket type will be used. For Unix sockets, you can also specify a
         socktype of None, in which case socket.SOCK_DGRAM will be used, falling
         back to socket.SOCK_STREAM.
         """
         logging.Handler.__init__(self)
```

### Comparing `flgo-0.0.8/src/flgo/experiment/logger/simple_logger.py` & `flgo-0.0.9/src/flgo/experiment/logger/simple_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from flgo.experiment.logger import BasicLogger
 import numpy as np
 import flgo.simulator.base as ss
 
 class SimpleLogger(BasicLogger):
     r"""Simple Logger. Only evaluating model performance on testing dataset and validation dataset."""
     def initialize(self):
-        """This method is used to record the stastic variables that won't change across rounds (e.g. local data size)"""
+        """This method is used to record the stastic variables that won't change across rounds (e.g. local_movielens_recommendation data size)"""
         for c in self.participants:
             self.output['client_datavol'].append(len(c.train_data))
 
     """This logger only records metrics on validation dataset"""
     def log_once(self, *args, **kwargs):
         self.info('Current_time:{}'.format(self.clock.current_time))
         self.output['time'].append(self.clock.current_time)
```

### Comparing `flgo-0.0.8/src/flgo/experiment/logger/tune_logger.py` & `flgo-0.0.9/src/flgo/experiment/logger/tune_logger.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/experiment/logger/vertical_logger.py` & `flgo-0.0.9/src/flgo/experiment/logger/vertical_logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from flgo.experiment.logger import BasicLogger
 
 class VerticalLogger(BasicLogger):
     r"""Vertical Logger. Vertical FL should use this Logger"""
     def initialize(self):
-        """This method is used to record the stastic variables that won't change across rounds (e.g. local data size)"""
+        """This method is used to record the stastic variables that won't change across rounds (e.g. local_movielens_recommendation data size)"""
         for c in self.participants:
             self.output['client_datavol'].append(len(c.train_data))
 
     """This logger only records metrics on validation dataset"""
     def log_once(self, *args, **kwargs):
         self.info('Current_time:{}'.format(self.clock.current_time))
         self.output['time'].append(self.clock.current_time)
```

### Comparing `flgo-0.0.8/src/flgo/simulator/__init__.py` & `flgo-0.0.9/src/flgo/simulator/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 r"""
 This module is to simulate arbitrary system heterogeneity that may occur in practice.
-We conclude four types of system heterogeneity from existing works:
-    1) availability: the devices will be either available or unavailable at each moment, where only the
+We conclude four types of system heterogeneity from existing works.
+System Heterogeneity Description:
+    1. **Availability**: the devices will be either available or unavailable at each moment, where only the
                     available devices can be selected to participate in training.
-    2) responsiveness: the responsiveness describes the length of the period from the server broadcasting the
+
+    2. **Responsiveness**: the responsiveness describes the length of the period from the server broadcasting the
                     gloabl model to the server receiving the locally trained model from a particular client.
-    3) completeness: since the server cannot fully control the behavior of devices,it's possible for devices to
+
+    3. **Completeness**: since the server cannot fully control the behavior of devices,it's possible for devices to
                     upload imcomplete model updates (i.e. only training for a few steps).
-    4) connectivity: the clients who promise to complete training may suffer accidients so that the server may lose
-                    connections with these client who will never return the currently trained local model.
+
+    4. **Connectivity**: the clients who promise to complete training may suffer accidients so that the server may lose
+                    connections with these client who will never return the currently trained local_movielens_recommendation model.
+
 We build up a client state machine to simulate the four types of system heterogeneity, and provide high-level
 APIs to allow customized system heterogeneity simulation.
 
-Example 1: How to customize the system heterogeneity?
+**Example**: How to customize the system heterogeneity:
+```python
 >>> class MySimulator(flgo.simulator.base.BasicSimulator):
 ...     def update_client_availability(self):
 ...         # update the variable 'prob_available' and 'prob_unavailable' for all the clients
 ...         self.set_variable(self.all_clients, 'prob_available', [0.9 for _ in self.all_clients])
 ...         self.set_variable(self.all_clients, 'prob_unavailable', [0.1 for _ in self.all_clients])
 ...
 ...     def update_client_connectivity(self, client_ids):
@@ -29,12 +35,13 @@
 ...
 ...     def update_client_completeness(self, client_ids, *args, **kwargs):
 ...         # update the variable 'working_amount' for clients in client_ids
 ...         self.set_variable(client_ids, 'working_amount',  [max(int(self.clients[cid].num_steps*np.random.rand()), 1) for cid in client_ids])
 >>> r = flgo.init(task, algorithm=fedavg, Simulator=MySimulator)
 >>> # The runner r will be runned under the customized system heterogeneity, where the clients' states will be flushed by
 >>> # MySimulator.update_client_xxx at each moment of the virtual clock or particular events happen (i.e. a client was selected)
+```
 
 We also provide some preset Simulator like flgo.simulator.DefaultSimulator and flgo.simulator.
 """
 from flgo.simulator.default_simulator import Simulator as DefaultSimulator
 from flgo.simulator.phone_simulator import Simulator as PhoneSimulator
```

### Comparing `flgo-0.0.8/src/flgo/simulator/base.py` & `flgo-0.0.9/src/flgo/simulator/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,15 +215,15 @@
         if len(objects)>0:
             self.server = objects[0]
             self.clients = objects[1:]
         else:
             self.server = None
             self.clients = []
         self.all_clients = list(range(len(self.clients)))
-        self.random_module = np.random.RandomState(0) if random_seed_gen is None else np.random.RandomState(next(random_seed_gen))
+        self.random_module = np.random.RandomState(0)
         # client states and the variables
         self.client_states = ['idle' for _ in self.clients]
         self.roundwise_fixed_availability = False
         self.availability_latest_round = -1
         self.variables = [{
             'prob_available': 1.,
             'prob_unavailable': 0.,
@@ -407,21 +407,23 @@
 #     return f_timestep
 
 # sampling phase
 def with_availability(sample):
     r"""
     The decorator for sampling with client availability
 
-    Example::
+    Example:
+    ```python
         >>> import flgo.algorithm.fedbase
         >>> import flgo.simulator.base as ss
         >>> class Server(flgo.algorithm.fedbase.BasicServer):
         ...     @ss.with_availability
         ...     def sample(self):
         ...         ...
+    ```
     """
     @functools.wraps(sample)
     def sample_with_availability(self):
         available_clients = self.gv.simulator.idle_clients
         # ensure that there is at least one client to be available at the current moment
         # while len(available_clients) == 0:
         #     self.gv.clock.step()
@@ -440,21 +442,23 @@
     return sample_with_availability
 
 # communicating phase
 def with_dropout(communicate):
     r"""
     The decorator for communicating to simulate the scene where clients may drop out
 
-    Example::
+    Example:
+    ```python
         >>> import flgo.algorithm.fedbase
         >>> import flgo.simulator.base as ss
         >>> class Server(flgo.algorithm.fedbase.BasicServer):
         ...     @ss.with_dropout
         ...     def communicate(self,...):
         ...         ...
+    ```
     """
     @functools.wraps(communicate)
     def communicate_with_dropout(self, selected_clients, mtype=0, asynchronous=False):
         if len(selected_clients) > 0:
             self.gv.simulator.update_client_connectivity(selected_clients)
             probs_drop = self.gv.simulator.get_variable(selected_clients, 'prob_drop')
             self._dropped_selected_clients = [cid for cid,prob in zip(selected_clients, probs_drop) if self.gv.simulator.random_module.rand() <= prob]
@@ -465,26 +469,28 @@
     return communicate_with_dropout
 
 # communicating phase
 def with_latency(communicate_with):
     r"""
     The decorator to simulate the scene where there are network latencies during communication
 
-    Example::
+    Example:
+    ```python
         >>> import flgo.algorithm.fedbase
         >>> import flgo.simulator.base as ss
         >>> class Server(flgo.algorithm.fedbase.BasicServer):
         ...     @ss.with_latency
         ...     def communicate_with(self,...):
         ...         ...
+    ```
     """
     @functools.wraps(communicate_with)
     def delayed_communicate_with(self, target_id, package):
         # Calculate latency for the target client
-        # Set local model size of clients for computation cost estimation
+        # Set local_movielens_recommendation model size of clients for computation cost estimation
         model_size = package['model'].count_parameters(output=False) if 'model' in package.keys() else 0
         self.gv.simulator.set_variable(target_id, '__model_size', model_size)
         # Set downloading package sizes for clients for downloading cost estimation
         self.gv.simulator.set_variable(target_id, '__download_package_size',size_of_package(package))
         res = communicate_with(self, target_id, package)
         # Set uploading package sizes for clients for uploading cost estimation
         self.gv.simulator.set_variable(target_id, '__upload_package_size', size_of_package(res))
@@ -497,47 +503,51 @@
         self.clients[target_id]._latency = latency
         res['__cid'] = target_id
         # Compute the arrival time
         res['__t'] = self.gv.clock.current_time + latency
         return res
     return delayed_communicate_with
 
-# local training phase
+# local_movielens_recommendation training phase
 def with_completeness(train):
     r"""
     The decorator to simulate the scene where the clients may upload incomplete model updates
 
-    Example::
+    Example:
+    ```python
         >>> import flgo.algorithm.fedbase
         >>> import flgo.simulator.base as ss
         >>> class Client(flgo.algorithm.fedbase.BasicClient):
         ...     @ss.with_completeness
         ...     def train(self,...):
         ...         ...
+    ```
     """
     @functools.wraps(train)
     def train_with_incomplete_update(self, model, *args, **kwargs):
         old_num_steps = self.num_steps
         self.num_steps = self._working_amount
         res = train(self, model, *args, **kwargs)
         self.num_steps = old_num_steps
         return res
     return train_with_incomplete_update
 
 def with_clock(communicate):
     r"""
     The decorator to simulate the scene where there is a virtual global clock
 
-    Example::
+    Example:
+    ```python
         >>> import flgo.algorithm.fedbase
         >>> import flgo.simulator.base as ss
         >>> class Server(flgo.algorithm.fedbase.BasicServer):
         ...     @ss.with_clock
         ...     def communicate(self,...):
         ...         ...
+    ```
     """
     def communicate_with_clock(self, selected_clients, mtype=0, asynchronous=False):
         self.gv.simulator.update_client_completeness(selected_clients)
         res = communicate(self, selected_clients, mtype, asynchronous)
         # If all the selected clients are unavailable, directly return the result without waiting.
         # Else if all the available clients have dropped out and not using asynchronous communication,  waiting for `tolerance_for_latency` time units.
         tolerance_for_latency = self.get_tolerance_for_latency()
```

### Comparing `flgo-0.0.8/src/flgo/simulator/default_simulator.py` & `flgo-0.0.9/src/flgo/simulator/default_simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     return
 
 def y_max_first_client_availability(simulator, beta=0.1):
     """
     This setting follows the activity mode in 'Fast Federated Learning in the
     Presence of Arbitrary Device Unavailability' , where each client ci will be ready
     for joining in a round with a static probability:
-        pi = alpha * min({label kept by ci}) / max({all labels}) + ( 1 - alpha )
+        pi = beta * min({label kept by ci}) / max({all labels}) + ( 1 - beta )
     and the participation of client is independent across rounds. The string mode
     should be like 'YMaxFirst-x' where x should be replaced by a float number.
     """
     # alpha = float(mode[mode.find('-') + 1:]) if mode.find('-') != -1 else 0.1
     def label_counter(dataset):
         return collections.Counter([int(dataset[di][-1]) for di in range(len(dataset))])
     label_num = len(label_counter(simulator.server.test_data))
@@ -219,15 +219,15 @@
     simulator.set_variable(simulator.all_clients, 'working_amount', working_amounts)
     return
 
 def arbitrary_dynamic_unifrom_client_completeness(simulator, a=1, b=1):
     """
     This setting follows the setting in the paper 'Tackling the Objective Inconsistency Problem in
     Heterogeneous Federated Optimization' (http://arxiv.org/abs/2007.07481). The string `mode` should be like
-    'FEDNOVA-Uniform(a,b)' where `a` is the minimal value of the number of local epochs and `b` is the maximal
+    'FEDNOVA-Uniform(a,b)' where `a` is the minimal value of the number of local_movielens_recommendation epochs and `b` is the maximal
     value. If this mode is active, the `num_epochs` and `num_steps` of clients will be disable.
     """
     simulator._incomplete_a = min(a, 1)
     simulator._incomplete_b = max(b, simulator._incomplete_a)
     def f(self, client_ids = []):
         for cid in client_ids:
             self.clients[cid].set_local_epochs(self.random_module.randint(low=self._incomplete_a, high=self._incomplete_b))
@@ -236,15 +236,15 @@
         return
     return f
 
 def arbitrary_static_unifrom_client_completeness(simulator, a=1, b=1):
     """
     This setting follows the setting in the paper 'Tackling the Objective Inconsistency Problem in
     Heterogeneous Federated Optimization' (http://arxiv.org/abs/2007.07481). The string `mode` should be like
-    'FEDNOVA-Uniform(a,b)' where `a` is the minimal value of the number of local epochs and `b` is the maximal
+    'FEDNOVA-Uniform(a,b)' where `a` is the minimal value of the number of local_movielens_recommendation epochs and `b` is the maximal
     value. If this mode is active, the `num_epochs` and `num_steps` of clients will be disable.
     """
     a = min(a, 1)
     b = max(b, a)
     for cid in simulator.clients:
         simulator.clients[cid].set_local_epochs(np.random.randint(low=a, high=b))
     working_amounts = [simulator.clients[cid].num_steps for cid in simulator.all_clients]
```

### Comparing `flgo-0.0.8/src/flgo/simulator/my_simulator.py` & `flgo-0.0.9/src/flgo/simulator/my_simulator.py`

 * *Files identical despite different names*

### Comparing `flgo-0.0.8/src/flgo/simulator/phone_simulator.py` & `flgo-0.0.9/src/flgo/simulator/phone_simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,15 +255,15 @@
     def update_client_responsiveness(self, client_ids, *args, **kwargs):
         # calculate time of uploading and downloading model
         latency = []
         up_pkg_sizes = self.get_variable(client_ids, '__upload_package_size')
         down_pkg_sizes = self.get_variable(client_ids, '__download_package_size')
         for cid, upsize,down_size in zip(client_ids, up_pkg_sizes, down_pkg_sizes):
             latency.append(int(1.0*upsize/self.net_speeds[cid][0] + 1.0*down_size/self.net_speeds[cid][1]))
-        # calculate time of local computing
+        # calculate time of local_movielens_recommendation computing
         tlcs = []
         model_sizes =  self.get_variable(client_ids, '__model_size')
         working_amounts = self.get_variable(client_ids, 'working_amount')
         for cid, model_size, wa in zip(client_ids, model_sizes, working_amounts):
             uk = self.client_us[cid]
             tlc_k = uk*model_size/1000.0*self.clients[cid].batch_size*wa/1000.0
             tlcs.append(tlc_k)
```

### Comparing `flgo-0.0.8/src/flgo/utils/fflow.py` & `flgo-0.0.9/src/flgo/utils/fflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,28 +101,28 @@
     parser.add_argument('--aggregate', help='methods for aggregating models', type=str, choices=agg_list, default='uniform')
     # hyper-parameters of training in server side
     parser.add_argument('--num_rounds', help='number of communication rounds', type=int, default=20)
     parser.add_argument('--proportion', help='proportion of clients sampled per round', type=float, default=0.2)
     parser.add_argument('--learning_rate_decay', help='learning rate decay for the training process;', type=float, default=0.998)
     parser.add_argument('--lr_scheduler', help='type of the global learning rate scheduler', type=int, default=-1)
     parser.add_argument('--early_stop', help='stop training if there is no improvement for no smaller than the maximum rounds', type=int, default=-1)
-    # hyper-parameters of local training
+    # hyper-parameters of local_movielens_recommendation training
     parser.add_argument('--num_epochs', help='number of epochs when clients trainset on data;', type=int, default=5)
-    parser.add_argument('--num_steps', help='the number of local steps, which dominate num_epochs when setting num_steps>0', type=int, default=-1)
+    parser.add_argument('--num_steps', help='the number of local_movielens_recommendation steps, which dominate num_epochs when setting num_steps>0', type=int, default=-1)
     parser.add_argument('--learning_rate', help='learning rate for inner solver;', type=float, default=0.1)
     parser.add_argument('--batch_size', help='batch size when clients trainset on data;', type=float, default='64')
     parser.add_argument('--optimizer', help='select the optimizer for gd', type=str, choices=optimizer_list, default='SGD')
-    parser.add_argument('--momentum', help='momentum of local update', type=float, default=0)
+    parser.add_argument('--momentum', help='momentum of local_movielens_recommendation update', type=float, default=0)
     parser.add_argument('--weight_decay', help='weight decay for the training process', type=float, default=0)
     # algorithm-dependent hyper-parameters
     parser.add_argument('--algo_para', help='algorithm-dependent hyper-parameters', nargs='*', type=float)
 
     """Environment Options"""
     # the ratio of the amount of the data used to train
-    parser.add_argument('--train_holdout', help='the rate of holding out the validation dataset from all the local training datasets', type=float, default=0.1)
+    parser.add_argument('--train_holdout', help='the rate of holding out the validation dataset from all the local_movielens_recommendation training datasets', type=float, default=0.1)
     parser.add_argument('--test_holdout', help='the rate of holding out the validation dataset from the training datasets', type=float, default=0.0)
     parser.add_argument('--local_test', help='if this term is set True and train_holdout>0, (0.5*train_holdout) of data will be set as client.test_data.', action="store_true", default=False)
     # realistic machine config
     parser.add_argument('--seed', help='seed for random initialization;', type=int, default=0)
     parser.add_argument('--gpu', nargs='*', help='GPU IDs and empty input is equal to using CPU', type=int)
     parser.add_argument('--server_with_cpu', help='seed for random initialization;', action="store_true", default=False)
     parser.add_argument('--num_parallels', help="the number of parallels in the clients computing session", type=int, default=1)
@@ -179,35 +179,46 @@
         bmk_para (dict): the customized parameter dict of the method TaskGenerator.__init__() of the benchmark
         Partitioner (flgo.benchmark.toolkits.partition.BasicPartitioner|str): the class of the Partitioner or the name of the Partitioner that was realized in flgo.benchmark.toolkits.partition
         par_para (dict): the customized parameter dict of the method Partitioner.__init__()
         task_path (str): the path to store the generated task
         rawdata_path (str): where the raw data will be downloaded\stored
         seed (int): the random seed used to generate the task
 
-    Example::
+    Example:
+    ```python
         >>> import flgo
         >>> import flgo.benchmark.mnist_classification as mnist
         >>> from flgo.benchmark.toolkits.partition import IIDPartitioner
         >>> # GENERATE TASK BY PASSING THE MODULE OF BENCHMARK AND THE CLASS OF THE PARTITIOENR
         >>> flgo.gen_task_by_para(benchmark=mnist, Partitioner = IIDPartitioner, par_para={'num_clients':100}, task_path='./mnist_gen_by_para1')
         >>> # GENERATE THE SAME TASK BY PASSING THE STRING
         >>> flgo.gen_task_by_para(benchmark='flgo.benchmark.mnist_classification', Partitioner='IIDPartitioner', par_para={'num_clients':100}, task_path='./mnist_gen_by_para2')
+    ```
     """
     random.seed(3 + seed)
     np.random.seed(97 + seed)
     torch.manual_seed(12+seed)
     os.environ['PYTHONHASHSEED'] = str(seed)
     if type(benchmark) is str: benchmark = importlib.import_module(benchmark)
     if not hasattr(benchmark, '__path__'): raise RuntimeError("benchmark should be a package or the path of a package")
     if Partitioner is not None:
         if type(Partitioner) is str:
             if Partitioner in globals().keys(): Partitioner = eval(Partitioner)
             else: Partitioner = getattr(flgo.benchmark.toolkits.partition, Partitioner)
         partitioner = Partitioner(**par_para)
-    else: partitioner = None
+    else:
+        try:
+            if hasattr(benchmark, 'default_partitioner'):
+                Partitioner = getattr(benchmark, 'default_partitioner')
+                default_partition_para = getattr(benchmark, 'default_partition_para') if hasattr(benchmark, 'default_partition_para') else {}
+                partitioner = Partitioner(**default_partition_para)
+            else:
+                partitioner = None
+        except:
+            partitioner = None
     if rawdata_path!='': bmk_para['rawdata_path']=rawdata_path
     bmk_core = benchmark.core
     task_generator = getattr(bmk_core, 'TaskGenerator')(**bmk_para)
     if partitioner is not None:
         task_generator.register_partitioner(partitioner)
         partitioner.register_generator(task_generator)
     task_generator.generate()
@@ -242,55 +253,70 @@
     Generate a federated task that is specified by the benchmark information and the partition information, where the generated task will be stored in the task_path and the raw data will be downloaded into the rawdata_path.
 
         config (dict || str): configuration is either a dict contains parameters or a filename of a .yml file
         task_path (str): where the generated task will be stored
         rawdata_path (str): where the raw data will be downloaded\stored
         seed (int): the random seed used to generate the task
 
-    Example::
+    Example:
+    ```python
         >>> import flgo
         >>> config = {'benchmark':{'name':'flgo.benchmark.mnist_classification'}, 'partitioner':{'name':'IIDParitioner', 'para':{'num_clients':100}}}
         >>> flgo.gen_task(config, './my_mnist_iid')
         >>> # The task will be stored as `my_mnist_iid` in the current working dictionary
+    ```
     """
     # setup random seed
     random.seed(3 + seed)
     np.random.seed(97 + seed)
     torch.manual_seed(12+seed)
     os.environ['PYTHONHASHSEED'] = str(seed)
     # load configuration
     gen_option = load_configuration(config)
+    if type(gen_option['benchmark']) is not dict: gen_option['benchmark']={'name':gen_option['benchmark']}
     if 'para' not in gen_option['benchmark'].keys(): gen_option['benchmark']['para'] = {}
     if 'partitioner' in gen_option.keys():
         # update parameters of partitioner
         if 'para' not in gen_option['partitioner'].keys():
             gen_option['partitioner']['para'] = {}
         else:
             if 'name' not in gen_option['partitioner'].keys():
                 gen_option['benchmark']['para'].update(gen_option['partitioner']['para'])
     # init generator
     if rawdata_path!='': gen_option['benchmark']['para']['rawdata_path']=rawdata_path
     if type(gen_option['benchmark']['name']) is str:
         bmk_core = importlib.import_module('.'.join([gen_option['benchmark']['name'], 'core']))
     elif hasattr(gen_option['benchmark']['name'], '__path__'):
-        bmk_core = getattr(gen_option['benchmark']['name'],'core')
+        bmk_core = importlib.import_module('.core', gen_option['benchmark']['name'].__name__)
     else:
         raise RuntimeError("The value of parameter config['benchmark']['name'] should be either a string or a python package.")
     task_generator = getattr(bmk_core, 'TaskGenerator')(**gen_option['benchmark']['para'])
+    bmk_module = importlib.import_module(gen_option['benchmark']['name']) if type(
+        gen_option['benchmark']['name']) is str else gen_option['benchmark']['name']
     # create partitioner for generator if specified
     if 'partitioner' in gen_option.keys() and 'name' in gen_option['partitioner'].keys():
         Partitioner = gen_option['partitioner']['name']
         if type(Partitioner) is str:
             if Partitioner in globals().keys(): Partitioner = eval(Partitioner)
             else: Partitioner = getattr(flgo.benchmark.toolkits.partition, Partitioner)
         partitioner = Partitioner(**gen_option['partitioner']['para'])
         task_generator.register_partitioner(partitioner)
         partitioner.register_generator(task_generator)
     else:
-        partitioner = None
+        try:
+            if hasattr(bmk_module, 'default_partitioner'):
+                Partitioner = getattr(bmk_module, 'default_partitioner')
+                default_partition_para = getattr(bmk_module, 'default_partition_para') if hasattr(bmk_module, 'default_partition_para') else {}
+                partitioner = Partitioner(**default_partition_para)
+                task_generator.register_partitioner(partitioner)
+                partitioner.register_generator(task_generator)
+            else:
+                partitioner = None
+        except:
+            partitioner = None
     # generate federated task
     task_generator.generate()
     # save the generated federated benchmark
     # initialize task pipe
     if task_path=='': task_path = os.path.join('.', task_generator.task_name)
     task_pipe = getattr(bmk_core, 'TaskPipe')(task_path)
     # check if task already exists
@@ -306,15 +332,15 @@
         print('Task {} has been successfully generated.'.format(task_generator.task_name))
     except Exception as e:
         print(e)
         task_pipe.remove_task()
         print("Failed to saving splited dataset.")
     # save visualization
     try:
-        visualize_func = getattr(importlib.import_module(gen_option['benchmark']['name']),'visualize')
+        visualize_func = getattr(bmk_module,'visualize')
         visualize_func(task_generator, partitioner, task_path)
     except:
         pass
 
 def init(task: str, algorithm, option = {}, model=None, Logger: flgo.experiment.logger.BasicLogger = None, Simulator: BasicSimulator=flgo.simulator.DefaultSimulator, scene='horizontal'):
     r"""
     Initialize a runner in FLGo, which is to optimize a model on a specific task (i.e. IID-mnist-of-100-clients) by the selected federated algorithm.
@@ -327,24 +353,26 @@
         Logger (flgo.experiment.logger.BasicLogger): the class of the logger inherited from flgo.experiment.logger.BasicLogger
         Simulator (flgo.simulator.base.BasicSimulator): the class of the simulator inherited from flgo.simulator.BasicSimulator
         scene (str): 'horizontal' or 'vertical' in current version of FLGo
 
     Returns:
         runner: the object instance that has the method runner.run()
 
-    Example::
+    Example:
+    ```python
         >>> import flgo
         >>> from flgo.algorithm import fedavg
         >>> from flgo.experiment.logger.simple_logger import SimpleLogger
         >>> # create task 'mnist_iid' by flgo.gen_task('gen_config.yml', 'mnist_iid') if there exists no such task
         >>> if os.path.exists('mnist_iid'): flgo.gen_task({'benchmark':{'name':'flgo.benchmark.mnist_classification'}, 'partitioner':{'name':'IIDPartitioner','para':{'num_clients':100}}}, 'mnist_iid')
         >>> # create runner
         >>> fedavg_runner = flgo.init('mnist_iid', algorithm=fedavg, option = {'num_rounds':20, 'gpu':[0], 'learning_rate':0.1})
         >>> fedavg_runner.run()
         ... # the training will start after runner.run() was called, and the running-time results will be recorded by Logger into the task dictionary
+    ```
     """
 
     # init option
     option = load_configuration(option)
     default_option = read_option_from_command()
     for op_key in option:
         if op_key in default_option.keys():
@@ -367,17 +395,21 @@
     option['server_with_cpu'] = True if option['num_parallels']>1 else option['server_with_cpu']
     # init task info
     if not os.path.exists(task):
         raise FileExistsError("Fedtask '{}' doesn't exist. Please generate the specified task by flgo.gen_task().")
     with open(os.path.join(task, 'info'), 'r') as inf:
         task_info = json.load(inf)
     benchmark = task_info['benchmark']
-    if model== None: model = getattr(importlib.import_module(benchmark), 'default_model')
+    if model== None:
+        bmk_module = importlib.import_module(benchmark)
+        if hasattr(bmk_module, 'default_model'):
+            model = getattr(bmk_module, 'default_model')
+        else:
+            model = algorithm
     option['model'] = (model.__name__).split('.')[-1]
-
     # create global variable
     gv = GlobalVariable()
     # init logger
     if Logger is None:
         if scene=='horizontal':
             Logger = flgo.experiment.logger.simple_logger.SimpleLogger
         elif scene=='vertical':
@@ -418,15 +450,15 @@
     # init communicator
     gv.communicator = flgo.VirtualCommunicator(objects)
 
     for ob in objects: ob.initialize()
 
     # init virtual system environment
     gv.logger.info('Use `{}` as the system simulator'.format(str(Simulator)))
-    flgo.simulator.base.random_seed_gen = flgo.simulator.base.seed_generator(option['seed'])
+    # flgo.simulator.base.random_seed_gen = flgo.simulator.base.seed_generator(option['seed'])
     gv.clock = flgo.simulator.base.ElemClock()
     gv.simulator = Simulator(objects, option)
     gv.clock.register_simulator(simulator=gv.simulator)
 
     gv.logger.register_variable(coordinator=objects[0], participants=objects[1:], option=option, clock=gv.clock, scene=scene, objects = objects)
     gv.logger.initialize()
     gv.logger.info('Ready to start.')
@@ -478,15 +510,14 @@
         res = (os.path.join(runner.gv.logger.get_output_path(), runner.gv.logger.get_output_name()), pid)
         send_end.send(res)
     except Exception as e:
         s = 'Process {} exits with error:" {}". '.format(pid, str(e))
         res = (opt, s, pid)
         send_end.send(res)
 
-
 def tune(task: str, algorithm, option: dict = {}, model=None, Logger: flgo.experiment.logger.BasicLogger = flgo.experiment.logger.tune_logger.TuneLogger, Simulator: BasicSimulator=flgo.simulator.DefaultSimulator, scene='horizontal', scheduler=None):
     """
         Tune hyper-parameters for the specific (task, algorithm, model) in parallel.
         Args:
             task (str): the dictionary of the federated task
             algorithm (module|class): the algorithm will be used to optimize the model in federated manner, which must contain pre-defined attributions (e.g. algorithm.Server and algorithm.Client for horizontal federated learning)
             option (dict): the dict whose values should be of type list to construct the combinations
@@ -605,21 +636,23 @@
         runner_args (list): each element in runner_args should be either a dict or a tuple or parameters
         devices (list): a list of gpu id
         scheduler (flgo.experiment.device_scheduler.BasicScheduler(...)): GPU scheduler
 
     Returns:
         a list of output results of runners
 
-    Example::
+    Example:
+    ```python
         >>> from flgo.algorithm import fedavg, fedprox, scaffold
         >>> # create task 'mnist_iid' by flgo.gen_task if there exists no such task
         >>> task='./mnist_iid'
         >>> if os.path.exists(task): flgo.gen_task({'benchmark':{'name':'flgo.benchmark.mnist_classification'}, 'partitioner':{'name':'IIDPartitioner','para':{'num_clients':100}}}, task)
         >>> algos = [fedavg, fedprox, scaffold]
         >>> flgo.multi_init_and_run([{'task':task, 'algorithm':algo} for algo in algos], devices=[0])
+    ```
     """
     if len(runner_args)==0:return
     args = []
     if type(runner_args[0]) is dict:
         for a in runner_args:
             tmp = collections.defaultdict(lambda:None, a)
             if tmp['task'] is None or tmp['algorithm'] is None:
```

### Comparing `flgo-0.0.8/src/flgo/utils/fmodule.py` & `flgo-0.0.9/src/flgo/utils/fmodule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import torch
 from torch import nn
 
 class FModule(nn.Module):
     r"""
     This module implements commonly used model-level operators like add, sub, and so on.
 
-    Example::
+    Example:
+    ```python
         >>> class TestModel(FModule):
         ...     def __init__(self):
         ...         self.mlp = torch.nn.Linear(2,2, bias=False)
         >>> m1 = TestModel()
         >>> m2 = TestModel()
         >>> m3 = m1+m2
         >>> (m1.mlp.weight+m2.mlp.weight)==m3.mlp.weight
+    ```
     """
     def __init__(self):
         super().__init__()
         self.ingraph = False
 
     def __add__(self, other):
         if isinstance(other, int) and other == 0 : return self
```

### Comparing `flgo-0.0.8/src/flgo.egg-info/SOURCES.txt` & `flgo-0.0.9/src/flgo.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -5,43 +5,59 @@
 src/flgo.egg-info/PKG-INFO
 src/flgo.egg-info/SOURCES.txt
 src/flgo.egg-info/dependency_links.txt
 src/flgo.egg-info/top_level.txt
 src/flgo/algorithm/TiFL.py
 src/flgo/algorithm/__init__.py
 src/flgo/algorithm/afl.py
+src/flgo/algorithm/clustered_sampling.py
 src/flgo/algorithm/fedasync.py
 src/flgo/algorithm/fedavg.py
+src/flgo/algorithm/fedavgm.py
 src/flgo/algorithm/fedbase.py
 src/flgo/algorithm/fedbuff.py
 src/flgo/algorithm/fedfa.py
 src/flgo/algorithm/fedfv.py
+src/flgo/algorithm/fedmf.py
 src/flgo/algorithm/fedmgda+.py
 src/flgo/algorithm/fedprox.py
 src/flgo/algorithm/mifa.py
 src/flgo/algorithm/powerofchoice.py
 src/flgo/algorithm/qfedavg.py
 src/flgo/algorithm/scaffold.py
+src/flgo/algorithm/sesorec.py
 src/flgo/algorithm/vflbase.py
 src/flgo/benchmark/__init__.py
 src/flgo/benchmark/base.py
+src/flgo/benchmark/ciao_recommendation/__init__.py
+src/flgo/benchmark/ciao_recommendation/core.py
+src/flgo/benchmark/ciao_recommendation/model/mf.py
 src/flgo/benchmark/cifar100_classification/__init__.py
 src/flgo/benchmark/cifar100_classification/core.py
 src/flgo/benchmark/cifar100_classification/model/cnn.py
 src/flgo/benchmark/cifar100_classification/model/resnet18.py
 src/flgo/benchmark/cifar10_classification/__init__.py
 src/flgo/benchmark/cifar10_classification/core.py
 src/flgo/benchmark/cifar10_classification/model/cnn.py
 src/flgo/benchmark/cifar10_classification/model/mlp.py
 src/flgo/benchmark/citeseer_link_prediction/__init__.py
 src/flgo/benchmark/citeseer_link_prediction/core.py
 src/flgo/benchmark/citeseer_link_prediction/model/GCN.py
 src/flgo/benchmark/citeseer_node_classification/__init__.py
 src/flgo/benchmark/citeseer_node_classification/core.py
 src/flgo/benchmark/citeseer_node_classification/model/GCN.py
+src/flgo/benchmark/coco_detection/__init__.py
+src/flgo/benchmark/coco_detection/core.py
+src/flgo/benchmark/coco_detection/model/FasterRCNN.py
+src/flgo/benchmark/coco_detection/model/__init__.py
+src/flgo/benchmark/coco_segmentation/__init__.py
+src/flgo/benchmark/coco_segmentation/core.py
+src/flgo/benchmark/coco_segmentation/model/__init__.py
+src/flgo/benchmark/coco_segmentation/model/fcn_resnet50.py
+src/flgo/benchmark/coco_segmentation/model/unet.py
 src/flgo/benchmark/cora_link_prediction/__init__.py
 src/flgo/benchmark/cora_link_prediction/core.py
 src/flgo/benchmark/cora_link_prediction/model/GCN.py
 src/flgo/benchmark/cora_node_classification/__init__.py
 src/flgo/benchmark/cora_node_classification/core.py
 src/flgo/benchmark/cora_node_classification/model/GCN.py
 src/flgo/benchmark/cora_node_classification/model/GraphSAGE_1.py
@@ -50,68 +66,113 @@
 src/flgo/benchmark/emnist_classification/core.py
 src/flgo/benchmark/emnist_classification/model/cnn.py
 src/flgo/benchmark/emnist_classification/model/mlp.py
 src/flgo/benchmark/enzymes_graph_classification/__init__.py
 src/flgo/benchmark/enzymes_graph_classification/core.py
 src/flgo/benchmark/enzymes_graph_classification/model/GCN.py
 src/flgo/benchmark/enzymes_graph_classification/model/GIN.py
+src/flgo/benchmark/epinions_recommendation/__init__.py
+src/flgo/benchmark/epinions_recommendation/core.py
+src/flgo/benchmark/epinions_recommendation/model/__init__.py
+src/flgo/benchmark/epinions_recommendation/model/mf.py
 src/flgo/benchmark/fashion_classification/__init__.py
 src/flgo/benchmark/fashion_classification/core.py
 src/flgo/benchmark/fashion_classification/model/lr.py
 src/flgo/benchmark/femnist_classification/__init__.py
 src/flgo/benchmark/femnist_classification/core.py
+src/flgo/benchmark/femnist_classification/model/__init__.py
+src/flgo/benchmark/femnist_classification/model/cnn.py
 src/flgo/benchmark/leaf_reddit/__init__.py
 src/flgo/benchmark/leaf_reddit/core.py
 src/flgo/benchmark/leaf_reddit/model/stackedlstm.py
 src/flgo/benchmark/leaf_sent140/__init__.py
 src/flgo/benchmark/leaf_sent140/core.py
 src/flgo/benchmark/leaf_sent140/model/stackedlstm.py
+src/flgo/benchmark/local_movielens_recommendation/__init__.py
+src/flgo/benchmark/local_movielens_recommendation/core.py
+src/flgo/benchmark/local_movielens_recommendation/model/mf.py
 src/flgo/benchmark/mnist_classification/__init__.py
 src/flgo/benchmark/mnist_classification/core.py
 src/flgo/benchmark/mnist_classification/model/cnn.py
 src/flgo/benchmark/mnist_classification/model/mlp.py
+src/flgo/benchmark/movielens_recommendation/__init__.py
+src/flgo/benchmark/movielens_recommendation/core.py
+src/flgo/benchmark/movielens_recommendation/model/__init__.py
+src/flgo/benchmark/movielens_recommendation/model/mf.py
 src/flgo/benchmark/mutag_graph_classification/__init__.py
 src/flgo/benchmark/mutag_graph_classification/core.py
 src/flgo/benchmark/mutag_graph_classification/model/GCN.py
 src/flgo/benchmark/pubmed_link_prediction/__init__.py
 src/flgo/benchmark/pubmed_link_prediction/core.py
 src/flgo/benchmark/pubmed_link_prediction/model/GCN.py
 src/flgo/benchmark/pubmed_node_classification/__init__.py
 src/flgo/benchmark/pubmed_node_classification/core.py
 src/flgo/benchmark/pubmed_node_classification/model/GCN.py
+src/flgo/benchmark/sbdataset_segmentation/__init__.py
+src/flgo/benchmark/sbdataset_segmentation/core.py
+src/flgo/benchmark/sbdataset_segmentation/model/__init__.py
+src/flgo/benchmark/sbdataset_segmentation/model/fcn_resnet50.py
+src/flgo/benchmark/sbdataset_segmentation/model/unet.py
 src/flgo/benchmark/shakespeare_classification/__init__.py
 src/flgo/benchmark/shakespeare_classification/core.py
 src/flgo/benchmark/shakespeare_classification/model/stackedlstm.py
+src/flgo/benchmark/social_splitted_ciao/__init__.py
+src/flgo/benchmark/social_splitted_ciao/core.py
+src/flgo/benchmark/social_splitted_ciao/model/__init__.py
+src/flgo/benchmark/social_splitted_ciaodvd/__init__.py
+src/flgo/benchmark/social_splitted_ciaodvd/core.py
+src/flgo/benchmark/social_splitted_douban/__init__.py
+src/flgo/benchmark/social_splitted_douban/core.py
+src/flgo/benchmark/social_splitted_epinions/__init__.py
+src/flgo/benchmark/social_splitted_epinions/core.py
+src/flgo/benchmark/social_splitted_epinions/model/__init__.py
+src/flgo/benchmark/social_splitted_filmtrust/__init__.py
+src/flgo/benchmark/social_splitted_filmtrust/core.py
 src/flgo/benchmark/svhn_classification/__init__.py
 src/flgo/benchmark/svhn_classification/core.py
 src/flgo/benchmark/svhn_classification/model/cnn.py
 src/flgo/benchmark/svhn_classification/model/mlp.py
 src/flgo/benchmark/synthetic_regression/__init__.py
 src/flgo/benchmark/synthetic_regression/core.py
 src/flgo/benchmark/synthetic_regression/model/lr.py
 src/flgo/benchmark/toolkits/__init__.py
 src/flgo/benchmark/toolkits/partition.py
 src/flgo/benchmark/toolkits/visualization.py
 src/flgo/benchmark/toolkits/cv/__init__.py
-src/flgo/benchmark/toolkits/cv/centralize/__init__.py
-src/flgo/benchmark/toolkits/cv/horizontal/__init__.py
-src/flgo/benchmark/toolkits/cv/horizontal/image_classification.py
-src/flgo/benchmark/toolkits/cv/vertical/__init__.py
+src/flgo/benchmark/toolkits/cv/classification/__init__.py
+src/flgo/benchmark/toolkits/cv/detection/__init__.py
+src/flgo/benchmark/toolkits/cv/detection/coco_eval.py
+src/flgo/benchmark/toolkits/cv/detection/coco_utils.py
+src/flgo/benchmark/toolkits/cv/detection/presets.py
+src/flgo/benchmark/toolkits/cv/detection/transforms.py
+src/flgo/benchmark/toolkits/cv/detection/utils.py
+src/flgo/benchmark/toolkits/cv/segmentation/__init__.py
+src/flgo/benchmark/toolkits/cv/segmentation/coco_utils.py
+src/flgo/benchmark/toolkits/cv/segmentation/presets.py
+src/flgo/benchmark/toolkits/cv/segmentation/transforms.py
+src/flgo/benchmark/toolkits/cv/segmentation/utils.py
 src/flgo/benchmark/toolkits/graph/__init__.py
-src/flgo/benchmark/toolkits/graph/horizontal/__init__.py
-src/flgo/benchmark/toolkits/graph/horizontal/graph_classification.py
-src/flgo/benchmark/toolkits/graph/horizontal/link_prediction.py
-src/flgo/benchmark/toolkits/graph/horizontal/node_classification.py
+src/flgo/benchmark/toolkits/graph/graph_classification/__init__.py
+src/flgo/benchmark/toolkits/graph/link_prediction/__init__.py
+src/flgo/benchmark/toolkits/graph/node_classification/__init__.py
 src/flgo/benchmark/toolkits/nlp/__init__.py
-src/flgo/benchmark/toolkits/nlp/horizontal/__init__.py
-src/flgo/benchmark/toolkits/nlp/horizontal/text_prediction.py
+src/flgo/benchmark/toolkits/nlp/text_prediction/__init__.py
+src/flgo/benchmark/toolkits/rec/__init__.py
+src/flgo/benchmark/toolkits/rec/datasets.py
+src/flgo/benchmark/toolkits/rec/utils.py
+src/flgo/benchmark/toolkits/rec/rating_prediction/__init__.py
 src/flgo/benchmark/toolkits/tabular/__init__.py
 src/flgo/benchmark/vertical_mnist_classification/__init__.py
 src/flgo/benchmark/vertical_mnist_classification/core.py
 src/flgo/benchmark/vertical_mnist_classification/model/mlp.py
+src/flgo/benchmark/voc_detection/__init__.py
+src/flgo/benchmark/voc_detection/core.py
+src/flgo/benchmark/voc_detection/model/FasterRCNN.py
+src/flgo/benchmark/voc_detection/model/__init__.py
+src/flgo/benchmark/voc_detection/model/yolov3.py
 src/flgo/experiment/__init__.py
 src/flgo/experiment/analyzer.py
 src/flgo/experiment/device_scheduler.py
 src/flgo/experiment/logger/__init__.py
 src/flgo/experiment/logger/config.py
 src/flgo/experiment/logger/handlers.py
 src/flgo/experiment/logger/simple_logger.py
```

### Comparing `flgo-0.0.8/tests/test.py` & `flgo-0.0.9/tests/test.py`

 * *Files identical despite different names*

