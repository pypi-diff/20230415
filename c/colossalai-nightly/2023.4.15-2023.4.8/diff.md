# Comparing `tmp/colossalai-nightly-2023.4.15.tar.gz` & `tmp/colossalai-nightly-2023.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colossalai-nightly-2023.4.15.tar", last modified: Sat Apr 15 00:14:52 2023, max compression
+gzip compressed data, was "colossalai-nightly-2023.4.8.tar", last modified: Sat Apr  8 00:13:40 2023, max compression
```

## Comparing `colossalai-nightly-2023.4.15.tar` & `colossalai-nightly-2023.4.8.tar`

### file list

```diff
@@ -1,871 +1,871 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.245868 colossalai-nightly-2023.4.15/
--rw-r--r--   0 runner    (1001) docker     (123)    22244 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    24365 2023-04-15 00:14:52.245868 colossalai-nightly-2023.4.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19962 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.157863 colossalai-nightly-2023.4.15/colossalai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.157863 colossalai-nightly-2023.4.15/colossalai/_C/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/_C/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.157863 colossalai-nightly-2023.4.15/colossalai/amp/
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/amp/amp_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.157863 colossalai-nightly-2023.4.15/colossalai/amp/apex_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/amp/apex_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/amp/apex_amp/apex_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.157863 colossalai-nightly-2023.4.15/colossalai/amp/naive_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/amp/naive_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/amp/naive_amp/_fp16_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/amp/naive_amp/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.157863 colossalai-nightly-2023.4.15/colossalai/amp/naive_amp/grad_scaler/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/amp/naive_amp/grad_scaler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/amp/naive_amp/naive_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.157863 colossalai-nightly-2023.4.15/colossalai/amp/torch_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/amp/torch_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/amp/torch_amp/_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/amp/torch_amp/torch_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.157863 colossalai-nightly-2023.4.15/colossalai/auto_parallel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.161863 colossalai-nightly-2023.4.15/colossalai/auto_parallel/checkpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/checkpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/checkpoint/build_c_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py
--rw-r--r--   0 runner    (1001) docker     (123)    18543 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/checkpoint/operation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.161863 colossalai-nightly-2023.4.15/colossalai/auto_parallel/meta_profiler/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/meta_profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/meta_profiler/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.161863 colossalai-nightly-2023.4.15/colossalai/auto_parallel/meta_profiler/meta_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/meta_profiler/meta_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    25633 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/meta_profiler/meta_registry/where.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/meta_profiler/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/meta_profiler/shard_metainfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.161863 colossalai-nightly-2023.4.15/colossalai/auto_parallel/offload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/offload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/offload/amp_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/offload/base_offload_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/offload/mem_optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/offload/region.py
--rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/offload/region_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/offload/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/offload/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    18548 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/offload/training_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/offload/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.165863 colossalai-nightly-2023.4.15/colossalai/auto_parallel/passes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/passes/comm_metainfo_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/passes/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/passes/meta_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    12068 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/passes/runtime_apply_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)    22687 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/passes/runtime_preparation_pass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.165863 colossalai-nightly-2023.4.15/colossalai/auto_parallel/pipeline_shard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/pipeline_shard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.165863 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.165863 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14745 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    20533 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.169864 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14856 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    43503 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19134 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13270 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/sharding_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.169864 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/solver/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9987 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    20519 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/solver/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.169864 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/utils/broadcast.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/utils/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/utils/reshape.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/utils/sharding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.169864 colossalai-nightly-2023.4.15/colossalai/booster/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/booster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/booster/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/booster/booster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.173864 colossalai-nightly-2023.4.15/colossalai/booster/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/booster/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/booster/mixed_precision/bf16.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/booster/mixed_precision/fp16_apex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/booster/mixed_precision/fp16_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/booster/mixed_precision/fp8.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/booster/mixed_precision/mixed_precision_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.173864 colossalai-nightly-2023.4.15/colossalai/booster/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/booster/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/booster/plugin/gemini_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/booster/plugin/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/booster/plugin/torch_ddp_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.173864 colossalai-nightly-2023.4.15/colossalai/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/builder/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.173864 colossalai-nightly-2023.4.15/colossalai/checkpoint_io/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/checkpoint_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/checkpoint_io/checkpoint_io_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/checkpoint_io/general_checkpoint_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/checkpoint_io/index_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    14373 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/checkpoint_io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.173864 colossalai-nightly-2023.4.15/colossalai/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.173864 colossalai-nightly-2023.4.15/colossalai/cli/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/cli/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/cli/benchmark/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/cli/benchmark/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/cli/benchmark/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.173864 colossalai-nightly-2023.4.15/colossalai/cli/check/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/cli/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/cli/check/check_installation.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.173864 colossalai-nightly-2023.4.15/colossalai/cli/launcher/
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/cli/launcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/cli/launcher/hostinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/cli/launcher/multinode_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/cli/launcher/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.173864 colossalai-nightly-2023.4.15/colossalai/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/cluster/device_mesh_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/cluster/dist_coordinator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/cluster/process_group_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.173864 colossalai-nightly-2023.4.15/colossalai/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/communication/collective.py
--rw-r--r--   0 runner    (1001) docker     (123)    19463 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/communication/p2p.py
--rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/communication/p2p_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/communication/ring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/communication/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.177864 colossalai-nightly-2023.4.15/colossalai/context/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/context/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/context/moe_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    23922 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/context/parallel_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/context/parallel_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.177864 colossalai-nightly-2023.4.15/colossalai/context/process_group_initializer/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/context/process_group_initializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/context/process_group_initializer/initializer_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/context/process_group_initializer/initializer_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/context/process_group_initializer/initializer_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/context/process_group_initializer/initializer_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/context/process_group_initializer/initializer_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/context/process_group_initializer/initializer_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/context/process_group_initializer/initializer_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/context/process_group_initializer/initializer_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/context/process_group_initializer/initializer_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/context/process_group_initializer/process_group_initializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.177864 colossalai-nightly-2023.4.15/colossalai/context/random/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/context/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/context/random/_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/context/random/seed_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/context/singleton_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.177864 colossalai-nightly-2023.4.15/colossalai/device/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17420 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/device/alpha_beta_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/device/calc_pipeline_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/device/device_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.177864 colossalai-nightly-2023.4.15/colossalai/engine/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/engine/_base_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.177864 colossalai-nightly-2023.4.15/colossalai/engine/gradient_accumulation/
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/engine/gradient_accumulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/engine/gradient_accumulation/_gradient_accumulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.177864 colossalai-nightly-2023.4.15/colossalai/engine/gradient_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/engine/gradient_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/engine/gradient_handler/_base_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/engine/gradient_handler/_moe_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/engine/gradient_handler/_zero_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/engine/gradient_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.185865 colossalai-nightly-2023.4.15/colossalai/engine/schedule/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/engine/schedule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/engine/schedule/_base_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/engine/schedule/_non_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    41258 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/engine/schedule/_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/engine/schedule/_pipeline_schedule_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.185865 colossalai-nightly-2023.4.15/colossalai/fx/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    19408 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/_meta_regist_12.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/_meta_regist_13.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.185865 colossalai-nightly-2023.4.15/colossalai/fx/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/codegen/activation_checkpoint_codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/graph_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.185865 colossalai-nightly-2023.4.15/colossalai/fx/passes/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13584 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/passes/adding_split_node_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/passes/concrete_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/passes/meta_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    16288 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/passes/passes_for_gpt2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/passes/shard_1d_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/passes/split_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/passes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.185865 colossalai-nightly-2023.4.15/colossalai/fx/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/dataflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.189865 colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.189865 colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_function/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_function/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_function/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_function/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_function/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_function/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_function/python_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.189865 colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_module/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_module/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_module/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_module/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_module/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_module/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_module/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_module/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_module/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_module/torch_op.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/shard_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/memory_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/opcount.py
--rw-r--r--   0 runner    (1001) docker     (123)    15387 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/shard_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/profiler/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.189865 colossalai-nightly-2023.4.15/colossalai/fx/tracer/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/_meta_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/_symbolic_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/_tracer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.189865 colossalai-nightly-2023.4.15/colossalai/fx/tracer/bias_addition_patch/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/bias_addition_patch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.193865 colossalai-nightly-2023.4.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.193865 colossalai-nightly-2023.4.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    26968 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/experimental.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.193865 colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.193865 colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/patched_function/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/patched_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/patched_function/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/patched_function/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/patched_function/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/patched_function/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.193865 colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/patched_module/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/patched_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/patched_module/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/patched_module/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/patched_module/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/patched_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/patched_module/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/patched_module/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/patched_module/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    24623 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/fx/tracer/tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/global_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.193865 colossalai-nightly-2023.4.15/colossalai/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/interface/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/interface/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.193865 colossalai-nightly-2023.4.15/colossalai/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.193865 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.197865 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/compat.h
--rw-r--r--   0 runner    (1001) docker     (123)    16815 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/cpu_adam.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.197865 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu
--rw-r--r--   0 runner    (1001) docker     (123)    37586 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.201866 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/include/
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/include/context.h
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h
--rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/include/ls_cub.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h
--rw-r--r--   0 runner    (1001) docker     (123)    48403 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    25828 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26286 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    22850 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    13636 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/type_shim.h
--rw-r--r--   0 runner    (1001) docker     (123)    24865 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/multihead_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/scaled_softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.201866 colossalai-nightly-2023.4.15/colossalai/kernel/jit/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/jit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/jit/bias_dropout_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/jit/bias_gelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/jit/option.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.201866 colossalai-nightly-2023.4.15/colossalai/kernel/op_builder/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/op_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/op_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/op_builder/cpu_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/op_builder/fused_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/op_builder/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/op_builder/moe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/op_builder/multi_head_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/op_builder/scaled_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/kernel/op_builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.201866 colossalai-nightly-2023.4.15/colossalai/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.201866 colossalai-nightly-2023.4.15/colossalai/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.205866 colossalai-nightly-2023.4.15/colossalai/nn/_ops/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/_ops/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/_ops/addmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/_ops/batch_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/_ops/element_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/_ops/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/_ops/embedding_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/_ops/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/_ops/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/_ops/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/_ops/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.205866 colossalai-nightly-2023.4.15/colossalai/nn/layer/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/base_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.205866 colossalai-nightly-2023.4.15/colossalai/nn/layer/colossalai_layer/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/colossalai_layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/colossalai_layer/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/colossalai_layer/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/colossalai_layer/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/colossalai_layer/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/colossalai_layer/normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.205866 colossalai-nightly-2023.4.15/colossalai/nn/layer/moe/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/moe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/moe/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/moe/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/moe/experts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/moe/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/moe/routers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/moe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.205866 colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_1d/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_1d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_1d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_1d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    49748 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_1d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.205866 colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_2d/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34900 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_2d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_2d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    50524 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_2d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.205866 colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_2p5d/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_2p5d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37643 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_2p5d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_2p5d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    50769 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_2p5d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.205866 colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_3d/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_3d/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22769 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_3d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_3d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    51441 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_3d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.209866 colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_sequence/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_sequence/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_sequence/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_sequence/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.209866 colossalai-nightly-2023.4.15/colossalai/nn/layer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/utils/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.209866 colossalai-nightly-2023.4.15/colossalai/nn/layer/vanilla/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/vanilla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14535 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/vanilla/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.209866 colossalai-nightly-2023.4.15/colossalai/nn/layer/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/layer/wrapper/pipeline_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.209866 colossalai-nightly-2023.4.15/colossalai/nn/loss/
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/loss/loss_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/loss/loss_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/loss/loss_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/loss/loss_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/loss/loss_moe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.209866 colossalai-nightly-2023.4.15/colossalai/nn/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/lr_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/lr_scheduler/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/lr_scheduler/delayed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/lr_scheduler/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/lr_scheduler/multistep.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/lr_scheduler/onecycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/lr_scheduler/poly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/lr_scheduler/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.209866 colossalai-nightly-2023.4.15/colossalai/nn/metric/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/metric/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/metric/accuracy_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/metric/accuracy_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/metric/accuracy_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.213866 colossalai-nightly-2023.4.15/colossalai/nn/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/optimizer/colossalai_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/optimizer/cpu_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/optimizer/fused_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/optimizer/fused_lamb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/optimizer/fused_sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/optimizer/hybrid_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/optimizer/lamb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/optimizer/lars.py
--rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/optimizer/nvme_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.213866 colossalai-nightly-2023.4.15/colossalai/nn/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/parallel/data_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.213866 colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.213866 colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/cache_embedding/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/cache_embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    28600 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/cache_embedding/copyer.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/colo_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/nn/parallel/reducer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.213866 colossalai-nightly-2023.4.15/colossalai/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/pipeline/layer_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.213866 colossalai-nightly-2023.4.15/colossalai/pipeline/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/pipeline/middleware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.213866 colossalai-nightly-2023.4.15/colossalai/pipeline/middleware/adaptor/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/pipeline/middleware/adaptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/pipeline/middleware/adaptor/fx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/pipeline/middleware/topo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/pipeline/pipelinable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/pipeline/pipeline_process_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.217867 colossalai-nightly-2023.4.15/colossalai/pipeline/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/pipeline/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59163 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/pipeline/rpc/_pipeline_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/pipeline/rpc/_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/pipeline/rpc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/pipeline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.217867 colossalai-nightly-2023.4.15/colossalai/registry/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/registry/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.217867 colossalai-nightly-2023.4.15/colossalai/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/tensor/colo_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/tensor/colo_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    22268 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/tensor/comm_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/tensor/compute_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/tensor/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.217867 colossalai-nightly-2023.4.15/colossalai/tensor/d_tensor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/tensor/d_tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/tensor/d_tensor/comm_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/tensor/d_tensor/d_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/tensor/d_tensor/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    25229 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/tensor/d_tensor/layout_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/tensor/d_tensor/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/tensor/d_tensor/sharding_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/tensor/d_tensor/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/tensor/dist_spec_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/tensor/distspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/tensor/op_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/tensor/param_op_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/tensor/process_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    36491 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/tensor/shape_consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/tensor/sharding_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/tensor/tensor_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/tensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.217867 colossalai-nightly-2023.4.15/colossalai/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/testing/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/testing/pytest_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/testing/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     8614 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.217867 colossalai-nightly-2023.4.15/colossalai/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/trainer/_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.221867 colossalai-nightly-2023.4.15/colossalai/trainer/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/trainer/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/trainer/hooks/_base_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/trainer/hooks/_checkpoint_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/trainer/hooks/_commons_.py
--rw-r--r--   0 runner    (1001) docker     (123)    13106 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/trainer/hooks/_log_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/trainer/hooks/_lr_scheduler_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/trainer/hooks/_metric_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.221867 colossalai-nightly-2023.4.15/colossalai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/activation_checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.221867 colossalai-nightly-2023.4.15/colossalai/utils/checkpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/checkpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/checkpoint/module_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/checkpoint/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.221867 colossalai-nightly-2023.4.15/colossalai/utils/checkpoint_io/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/checkpoint_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/checkpoint_io/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/checkpoint_io/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/checkpoint_io/convertor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/checkpoint_io/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/checkpoint_io/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/checkpoint_io/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/checkpoint_io/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/checkpoint_io/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/checkpoint_io/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/checkpointing.py
--rw-r--r--   0 runner    (1001) docker     (123)    17451 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/cuda.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.221867 colossalai-nightly-2023.4.15/colossalai/utils/data_sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/data_sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/data_sampler/base_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/data_sampler/data_parallel_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.221867 colossalai-nightly-2023.4.15/colossalai/utils/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22138 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/model/experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/model/lazy_init_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/moe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.225867 colossalai-nightly-2023.4.15/colossalai/utils/multi_tensor_apply/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/multi_tensor_apply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.225867 colossalai-nightly-2023.4.15/colossalai/utils/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/profiler/extention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.225867 colossalai-nightly-2023.4.15/colossalai/utils/profiler/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/profiler/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/profiler/legacy/comm_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/profiler/legacy/pcie_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/profiler/legacy/prof_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/profiler/stateful_tensor_mem_extention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.225867 colossalai-nightly-2023.4.15/colossalai/utils/rank_recorder/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/rank_recorder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/rank_recorder/rank_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.225867 colossalai-nightly-2023.4.15/colossalai/utils/tensor_detector/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/tensor_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/tensor_detector/tensor_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.225867 colossalai-nightly-2023.4.15/colossalai/zero/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.225867 colossalai-nightly-2023.4.15/colossalai/zero/gemini/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/gemini/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.225867 colossalai-nightly-2023.4.15/colossalai/zero/gemini/chunk/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/gemini/chunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22078 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/gemini/chunk/chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/gemini/chunk/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/gemini/chunk/search_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/gemini/chunk/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/gemini/colo_init_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    29001 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/gemini/gemini_ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/gemini/gemini_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/gemini/gemini_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)    14275 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/gemini/gemini_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.229867 colossalai-nightly-2023.4.15/colossalai/zero/gemini/memory_tracer/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/gemini/memory_tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/gemini/memory_tracer/memory_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/gemini/memory_tracer/memory_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/gemini/memory_tracer/memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/gemini/memory_tracer/param_runtime_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/gemini/memory_tracer/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/gemini/placement_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/gemini/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.229867 colossalai-nightly-2023.4.15/colossalai/zero/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.229867 colossalai-nightly-2023.4.15/colossalai/zero/legacy/gemini/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/gemini/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/gemini/gemini_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.229867 colossalai-nightly-2023.4.15/colossalai/zero/legacy/gemini/ophooks/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/gemini/ophooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/gemini/ophooks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.229867 colossalai-nightly-2023.4.15/colossalai/zero/legacy/gemini/paramhooks/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/gemini/paramhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/gemini/stateful_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/gemini/tensor_placement_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/gemini/tensor_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.229867 colossalai-nightly-2023.4.15/colossalai/zero/legacy/init_ctx/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/init_ctx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/init_ctx/init_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.229867 colossalai-nightly-2023.4.15/colossalai/zero/legacy/shard_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/shard_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/shard_utils/base_shard_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/shard_utils/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.229867 colossalai-nightly-2023.4.15/colossalai/zero/legacy/sharded_model/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/sharded_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/sharded_model/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/sharded_model/reduce_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29011 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/sharded_model/sharded_model_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/sharded_model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/sharded_model/zero_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.229867 colossalai-nightly-2023.4.15/colossalai/zero/legacy/sharded_optim/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/sharded_optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18665 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.233868 colossalai-nightly-2023.4.15/colossalai/zero/legacy/sharded_param/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/sharded_param/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/sharded_param/sharded_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/legacy/sharded_param/sharded_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.233868 colossalai-nightly-2023.4.15/colossalai/zero/low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/low_level/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.233868 colossalai-nightly-2023.4.15/colossalai/zero/low_level/bookkeeping/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/low_level/bookkeeping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/low_level/bookkeeping/base_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/low_level/bookkeeping/bucket_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/low_level/bookkeeping/gradient_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/low_level/bookkeeping/parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/low_level/bookkeeping/tensor_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    25467 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/low_level/low_level_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/colossalai/zero/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.233868 colossalai-nightly-2023.4.15/colossalai_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24365 2023-04-15 00:14:51.000000 colossalai-nightly-2023.4.15/colossalai_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    36286 2023-04-15 00:14:52.000000 colossalai-nightly-2023.4.15/colossalai_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 00:14:51.000000 colossalai-nightly-2023.4.15/colossalai_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-15 00:14:51.000000 colossalai-nightly-2023.4.15/colossalai_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-15 00:14:51.000000 colossalai-nightly-2023.4.15/colossalai_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-15 00:14:51.000000 colossalai-nightly-2023.4.15/colossalai_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.233868 colossalai-nightly-2023.4.15/op_builder/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/op_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/op_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/op_builder/cpu_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/op_builder/fused_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/op_builder/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/op_builder/moe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/op_builder/multi_head_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/op_builder/scaled_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/op_builder/scaled_upper_triangle_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/op_builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.233868 colossalai-nightly-2023.4.15/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 00:14:52.245868 colossalai-nightly-2023.4.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.157863 colossalai-nightly-2023.4.15/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.237868 colossalai-nightly-2023.4.15/tests/components_to_test/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/components_to_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/components_to_test/albert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/components_to_test/beit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/components_to_test/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/components_to_test/gpt2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/components_to_test/hanging_param_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/components_to_test/inline_op_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/components_to_test/nested_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/components_to_test/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/components_to_test/repeated_computed_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/components_to_test/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/components_to_test/simple_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.237868 colossalai-nightly-2023.4.15/tests/components_to_test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/components_to_test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/components_to_test/utils/dummy_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/components_to_test/utils/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.237868 colossalai-nightly-2023.4.15/tests/kit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/kit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.237868 colossalai-nightly-2023.4.15/tests/kit/model_zoo/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/kit/model_zoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.237868 colossalai-nightly-2023.4.15/tests/kit/model_zoo/diffusers/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/kit/model_zoo/diffusers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/kit/model_zoo/diffusers/diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/kit/model_zoo/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.237868 colossalai-nightly-2023.4.15/tests/kit/model_zoo/timm/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/kit/model_zoo/timm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/kit/model_zoo/timm/timm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.237868 colossalai-nightly-2023.4.15/tests/kit/model_zoo/torchaudio/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/kit/model_zoo/torchaudio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/kit/model_zoo/torchaudio/torchaudio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.237868 colossalai-nightly-2023.4.15/tests/kit/model_zoo/torchrec/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/kit/model_zoo/torchrec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/kit/model_zoo/torchrec/torchrec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.237868 colossalai-nightly-2023.4.15/tests/kit/model_zoo/torchvision/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/kit/model_zoo/torchvision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/kit/model_zoo/torchvision/torchvision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.237868 colossalai-nightly-2023.4.15/tests/kit/model_zoo/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/kit/model_zoo/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/kit/model_zoo/transformers/albert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/kit/model_zoo/transformers/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/kit/model_zoo/transformers/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/kit/model_zoo/transformers/opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/kit/model_zoo/transformers/t5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.237868 colossalai-nightly-2023.4.15/tests/test_analyzer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_analyzer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.241868 colossalai-nightly-2023.4.15/tests/test_analyzer/test_fx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_analyzer/test_fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_analyzer/test_fx/test_bias_addition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_analyzer/test_fx/test_mod_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_analyzer/test_fx/test_nested_ckpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_analyzer/test_fx/test_shape_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_analyzer/test_fx/test_symbolic_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_analyzer/test_fx/zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.241868 colossalai-nightly-2023.4.15/tests/test_analyzer/test_subclasses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_analyzer/test_subclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_analyzer/test_subclasses/test_aten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_analyzer/test_subclasses/test_flop_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_analyzer/test_subclasses/test_meta_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.241868 colossalai-nightly-2023.4.15/tests/test_auto_parallel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.241868 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_pass/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_pass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_pass/test_node_converting_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.241868 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.241868 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_gpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:52.245868 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12527 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-15 00:14:40.000000 colossalai-nightly-2023.4.15/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.453257 colossalai-nightly-2023.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    22244 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    24234 2023-04-08 00:13:40.453257 colossalai-nightly-2023.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19848 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.377252 colossalai-nightly-2023.4.8/colossalai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.377252 colossalai-nightly-2023.4.8/colossalai/_C/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/_C/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.377252 colossalai-nightly-2023.4.8/colossalai/amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/amp_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.377252 colossalai-nightly-2023.4.8/colossalai/amp/apex_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/apex_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/apex_amp/apex_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.377252 colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/_fp16_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.377252 colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/grad_scaler/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/grad_scaler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/naive_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.377252 colossalai-nightly-2023.4.8/colossalai/amp/torch_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/torch_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/torch_amp/_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/amp/torch_amp/torch_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.377252 colossalai-nightly-2023.4.8/colossalai/auto_parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.377252 colossalai-nightly-2023.4.8/colossalai/auto_parallel/checkpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/checkpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/checkpoint/build_c_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18543 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/checkpoint/operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.377252 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.381252 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25633 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/where.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/shard_metainfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.381252 colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/amp_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/base_offload_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/mem_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/region_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18548 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/training_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.381252 colossalai-nightly-2023.4.8/colossalai/auto_parallel/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/passes/comm_metainfo_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/passes/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/passes/meta_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12068 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/passes/runtime_apply_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22687 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/passes/runtime_preparation_pass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.381252 colossalai-nightly-2023.4.8/colossalai/auto_parallel/pipeline_shard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/pipeline_shard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.381252 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.385252 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14745 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20533 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16519 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.389253 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14856 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43503 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19134 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13270 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/sharding_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.389253 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9987 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20519 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/solver/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.389253 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/utils/broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/utils/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/utils/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/utils/sharding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.389253 colossalai-nightly-2023.4.8/colossalai/booster/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/booster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/booster/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7836 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/booster/booster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.389253 colossalai-nightly-2023.4.8/colossalai/booster/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/booster/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/booster/mixed_precision/bf16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/booster/mixed_precision/fp16_apex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/booster/mixed_precision/fp16_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/booster/mixed_precision/fp8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/booster/mixed_precision/mixed_precision_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.389253 colossalai-nightly-2023.4.8/colossalai/booster/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/booster/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15407 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/booster/plugin/gemini_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/booster/plugin/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/booster/plugin/torch_ddp_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.389253 colossalai-nightly-2023.4.8/colossalai/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/builder/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.389253 colossalai-nightly-2023.4.8/colossalai/checkpoint_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/checkpoint_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/checkpoint_io/checkpoint_io_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/checkpoint_io/general_checkpoint_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/checkpoint_io/index_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/checkpoint_io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.389253 colossalai-nightly-2023.4.8/colossalai/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.389253 colossalai-nightly-2023.4.8/colossalai/cli/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cli/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cli/benchmark/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cli/benchmark/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cli/benchmark/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.393253 colossalai-nightly-2023.4.8/colossalai/cli/check/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cli/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cli/check/check_installation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.393253 colossalai-nightly-2023.4.8/colossalai/cli/launcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cli/launcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cli/launcher/hostinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cli/launcher/multinode_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cli/launcher/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.393253 colossalai-nightly-2023.4.8/colossalai/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cluster/device_mesh_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cluster/dist_coordinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/cluster/process_group_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.393253 colossalai-nightly-2023.4.8/colossalai/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/communication/collective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19463 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/communication/p2p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/communication/p2p_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/communication/ring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/communication/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.393253 colossalai-nightly-2023.4.8/colossalai/context/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/moe_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23922 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/parallel_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/parallel_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.393253 colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/process_group_initializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.393253 colossalai-nightly-2023.4.8/colossalai/context/random/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/random/_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/random/seed_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/context/singleton_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.393253 colossalai-nightly-2023.4.8/colossalai/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17420 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/device/alpha_beta_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/device/calc_pipeline_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/device/device_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.397253 colossalai-nightly-2023.4.8/colossalai/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/_base_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.397253 colossalai-nightly-2023.4.8/colossalai/engine/gradient_accumulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/gradient_accumulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/gradient_accumulation/_gradient_accumulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.397253 colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/_base_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/_moe_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/_zero_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.397253 colossalai-nightly-2023.4.8/colossalai/engine/schedule/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/schedule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/schedule/_base_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/schedule/_non_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41258 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/schedule/_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/engine/schedule/_pipeline_schedule_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.397253 colossalai-nightly-2023.4.8/colossalai/fx/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19408 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/_meta_regist_12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/_meta_regist_13.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.397253 colossalai-nightly-2023.4.8/colossalai/fx/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44750 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/codegen/activation_checkpoint_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/graph_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.397253 colossalai-nightly-2023.4.8/colossalai/fx/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13584 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/passes/adding_split_node_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/passes/concrete_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/passes/meta_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16288 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/passes/passes_for_gpt2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/passes/shard_1d_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/passes/split_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/passes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.401254 colossalai-nightly-2023.4.8/colossalai/fx/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/dataflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.401254 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.401254 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/python_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.401254 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/torch_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/shard_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/memory_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/opcount.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15387 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/shard_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/profiler/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.401254 colossalai-nightly-2023.4.8/colossalai/fx/tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/_meta_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/_symbolic_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/_tracer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.401254 colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.405254 colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.405254 colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26968 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/experimental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.405254 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.405254 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.405254 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_module/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_module/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_module/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_module/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_module/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_module/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24623 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/fx/tracer/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/global_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.405254 colossalai-nightly-2023.4.8/colossalai/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/interface/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/interface/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.405254 colossalai-nightly-2023.4.8/colossalai/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.405254 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.409254 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16815 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/cpu_adam.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.409254 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    37586 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.413254 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/context.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/ls_cub.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    48403 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25828 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26286 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22850 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    13636 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/type_shim.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24865 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/multihead_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/scaled_softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.413254 colossalai-nightly-2023.4.8/colossalai/kernel/jit/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/jit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/jit/bias_dropout_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/jit/bias_gelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/jit/option.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.413254 colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/cpu_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/fused_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/moe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/multi_head_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/scaled_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.413254 colossalai-nightly-2023.4.8/colossalai/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.413254 colossalai-nightly-2023.4.8/colossalai/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.413254 colossalai-nightly-2023.4.8/colossalai/nn/_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/_ops/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/_ops/addmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/_ops/batch_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/_ops/element_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/_ops/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/_ops/embedding_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/_ops/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/_ops/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/_ops/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/_ops/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.413254 colossalai-nightly-2023.4.8/colossalai/nn/layer/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/base_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.413254 colossalai-nightly-2023.4.8/colossalai/nn/layer/colossalai_layer/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/colossalai_layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/colossalai_layer/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/colossalai_layer/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/colossalai_layer/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/colossalai_layer/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/colossalai_layer/normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.417255 colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/experts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/routers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.417255 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_1d/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_1d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_1d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_1d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49748 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_1d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.417255 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2d/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34900 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50524 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.417255 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2p5d/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2p5d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37643 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2p5d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2p5d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50769 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2p5d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.417255 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_3d/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_3d/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22769 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_3d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_3d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51441 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_3d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.417255 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_sequence/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_sequence/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_sequence/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.417255 colossalai-nightly-2023.4.8/colossalai/nn/layer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/utils/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.417255 colossalai-nightly-2023.4.8/colossalai/nn/layer/vanilla/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/vanilla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14535 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/vanilla/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.417255 colossalai-nightly-2023.4.8/colossalai/nn/layer/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/layer/wrapper/pipeline_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.421255 colossalai-nightly-2023.4.8/colossalai/nn/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/loss/loss_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/loss/loss_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/loss/loss_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/loss/loss_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/loss/loss_moe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.421255 colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/delayed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/multistep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/onecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/poly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.421255 colossalai-nightly-2023.4.8/colossalai/nn/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/metric/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/metric/accuracy_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/metric/accuracy_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/metric/accuracy_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.421255 colossalai-nightly-2023.4.8/colossalai/nn/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/optimizer/colossalai_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/optimizer/cpu_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/optimizer/fused_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/optimizer/fused_lamb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/optimizer/fused_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/optimizer/hybrid_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/optimizer/lamb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/optimizer/lars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/optimizer/nvme_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.421255 colossalai-nightly-2023.4.8/colossalai/nn/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/data_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.421255 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.425255 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28600 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/copyer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/colo_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/nn/parallel/reducer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.425255 colossalai-nightly-2023.4.8/colossalai/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/pipeline/layer_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.425255 colossalai-nightly-2023.4.8/colossalai/pipeline/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/pipeline/middleware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.425255 colossalai-nightly-2023.4.8/colossalai/pipeline/middleware/adaptor/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/pipeline/middleware/adaptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/pipeline/middleware/adaptor/fx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/pipeline/middleware/topo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/pipeline/pipelinable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/pipeline/pipeline_process_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.425255 colossalai-nightly-2023.4.8/colossalai/pipeline/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/pipeline/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59163 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/pipeline/rpc/_pipeline_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/pipeline/rpc/_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/pipeline/rpc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/pipeline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.425255 colossalai-nightly-2023.4.8/colossalai/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/registry/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.425255 colossalai-nightly-2023.4.8/colossalai/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/colo_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/colo_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22268 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/comm_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/compute_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.429255 colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11875 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/comm_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/d_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25229 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/layout_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/sharding_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/dist_spec_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/distspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/op_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/param_op_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/process_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36491 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/shape_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/sharding_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/tensor_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/tensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.429255 colossalai-nightly-2023.4.8/colossalai/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/testing/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/testing/pytest_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/testing/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8614 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.429255 colossalai-nightly-2023.4.8/colossalai/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/trainer/_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.429255 colossalai-nightly-2023.4.8/colossalai/trainer/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/trainer/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/trainer/hooks/_base_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/trainer/hooks/_checkpoint_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/trainer/hooks/_commons_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13106 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/trainer/hooks/_log_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/trainer/hooks/_lr_scheduler_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/trainer/hooks/_metric_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.429255 colossalai-nightly-2023.4.8/colossalai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/activation_checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.429255 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint/module_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.433256 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/convertor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/checkpointing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17451 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/cuda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.433256 colossalai-nightly-2023.4.8/colossalai/utils/data_sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/data_sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/data_sampler/base_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/data_sampler/data_parallel_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.433256 colossalai-nightly-2023.4.8/colossalai/utils/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21939 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/model/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/model/lazy_init_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/moe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.433256 colossalai-nightly-2023.4.8/colossalai/utils/multi_tensor_apply/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/multi_tensor_apply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.433256 colossalai-nightly-2023.4.8/colossalai/utils/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/profiler/extention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.433256 colossalai-nightly-2023.4.8/colossalai/utils/profiler/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/profiler/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/profiler/legacy/comm_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/profiler/legacy/pcie_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/profiler/legacy/prof_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/profiler/stateful_tensor_mem_extention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.433256 colossalai-nightly-2023.4.8/colossalai/utils/rank_recorder/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/rank_recorder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/rank_recorder/rank_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.433256 colossalai-nightly-2023.4.8/colossalai/utils/tensor_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/tensor_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/tensor_detector/tensor_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.433256 colossalai-nightly-2023.4.8/colossalai/zero/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.433256 colossalai-nightly-2023.4.8/colossalai/zero/gemini/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.437256 colossalai-nightly-2023.4.8/colossalai/zero/gemini/chunk/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/chunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22078 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/chunk/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/chunk/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/chunk/search_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/chunk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/colo_init_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28189 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/gemini_ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/gemini_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/gemini_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14001 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/gemini_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.437256 colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/memory_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/memory_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/param_runtime_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/placement_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/gemini/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.437256 colossalai-nightly-2023.4.8/colossalai/zero/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.437256 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/gemini_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.437256 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/ophooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/ophooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/ophooks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.437256 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/paramhooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/paramhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/stateful_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/tensor_placement_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/tensor_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.437256 colossalai-nightly-2023.4.8/colossalai/zero/legacy/init_ctx/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/init_ctx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/init_ctx/init_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.437256 colossalai-nightly-2023.4.8/colossalai/zero/legacy/shard_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/shard_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/shard_utils/base_shard_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/shard_utils/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.441256 colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_model/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_model/reduce_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29011 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_model/sharded_model_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_model/zero_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.441256 colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_optim/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18665 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.441256 colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_param/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_param/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_param/sharded_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_param/sharded_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.441256 colossalai-nightly-2023.4.8/colossalai/zero/low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/low_level/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.441256 colossalai-nightly-2023.4.8/colossalai/zero/low_level/bookkeeping/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/low_level/bookkeeping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/low_level/bookkeeping/base_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/low_level/bookkeeping/bucket_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/low_level/bookkeeping/gradient_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/low_level/bookkeeping/parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/low_level/bookkeeping/tensor_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25467 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/low_level/low_level_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/colossalai/zero/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.441256 colossalai-nightly-2023.4.8/colossalai_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24234 2023-04-08 00:13:40.000000 colossalai-nightly-2023.4.8/colossalai_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    36286 2023-04-08 00:13:40.000000 colossalai-nightly-2023.4.8/colossalai_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 00:13:40.000000 colossalai-nightly-2023.4.8/colossalai_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-08 00:13:40.000000 colossalai-nightly-2023.4.8/colossalai_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-08 00:13:40.000000 colossalai-nightly-2023.4.8/colossalai_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-08 00:13:40.000000 colossalai-nightly-2023.4.8/colossalai_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.441256 colossalai-nightly-2023.4.8/op_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/op_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/op_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/op_builder/cpu_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/op_builder/fused_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/op_builder/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/op_builder/moe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/op_builder/multi_head_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/op_builder/scaled_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/op_builder/scaled_upper_triangle_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/op_builder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.441256 colossalai-nightly-2023.4.8/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 00:13:40.453257 colossalai-nightly-2023.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.373252 colossalai-nightly-2023.4.8/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.445256 colossalai-nightly-2023.4.8/tests/components_to_test/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/albert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/beit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/hanging_param_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/inline_op_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/nested_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/repeated_computed_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/simple_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.445256 colossalai-nightly-2023.4.8/tests/components_to_test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/utils/dummy_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/components_to_test/utils/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.445256 colossalai-nightly-2023.4.8/tests/kit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.445256 colossalai-nightly-2023.4.8/tests/kit/model_zoo/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.445256 colossalai-nightly-2023.4.8/tests/kit/model_zoo/diffusers/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/diffusers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/diffusers/diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.445256 colossalai-nightly-2023.4.8/tests/kit/model_zoo/timm/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/timm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/timm/timm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.445256 colossalai-nightly-2023.4.8/tests/kit/model_zoo/torchaudio/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/torchaudio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/torchaudio/torchaudio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.445256 colossalai-nightly-2023.4.8/tests/kit/model_zoo/torchrec/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/torchrec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/torchrec/torchrec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.445256 colossalai-nightly-2023.4.8/tests/kit/model_zoo/torchvision/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/torchvision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/torchvision/torchvision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.445256 colossalai-nightly-2023.4.8/tests/kit/model_zoo/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/transformers/albert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/transformers/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/transformers/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/transformers/opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/kit/model_zoo/transformers/t5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.445256 colossalai-nightly-2023.4.8/tests/test_analyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_analyzer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.445256 colossalai-nightly-2023.4.8/tests/test_analyzer/test_fx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_analyzer/test_fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_analyzer/test_fx/test_bias_addition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_analyzer/test_fx/test_mod_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_analyzer/test_fx/test_nested_ckpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_analyzer/test_fx/test_shape_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_analyzer/test_fx/test_symbolic_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_analyzer/test_fx/zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.449257 colossalai-nightly-2023.4.8/tests/test_analyzer/test_subclasses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_analyzer/test_subclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_analyzer/test_subclasses/test_aten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_analyzer/test_subclasses/test_flop_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_analyzer/test_subclasses/test_meta_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.449257 colossalai-nightly-2023.4.8/tests/test_auto_parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.449257 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_pass/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_pass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_pass/test_node_converting_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.449257 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.449257 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:40.453257 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12527 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-08 00:13:28.000000 colossalai-nightly-2023.4.8/version.txt
```

### Comparing `colossalai-nightly-2023.4.15/LICENSE` & `colossalai-nightly-2023.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/PKG-INFO` & `colossalai-nightly-2023.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colossalai-nightly
-Version: 2023.4.15
+Version: 2023.4.8
 Summary: An integrated large-scale model training system with efficient parallelization techniques
 Home-page: https://www.colossalai.org
 License: Apache Software License 2.0
 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/discussions
 Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/issues
 Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io
@@ -46,22 +46,14 @@
         * [2022/09] [HPC-AI Tech Completes $6 Million Seed and Angel Round Fundraising](https://www.hpc-ai.tech/blog/hpc-ai-tech-completes-6-million-seed-and-angel-round-fundraising-led-by-bluerun-ventures-in-the)
         
         ## Table of Contents
         <ul>
          <li><a href="#Why-Colossal-AI">Why Colossal-AI</a> </li>
          <li><a href="#Features">Features</a> </li>
          <li>
-           <a href="#Colossal-AI-in-the-Real-World">Colossal-AI for Real World Applications</a>
-           <ul>
-             <li><a href="#ColossalChat">ColossalChat: An Open-Source Solution for Cloning ChatGPT With a Complete RLHF Pipeline</a></li>
-             <li><a href="#AIGC">AIGC: Acceleration of Stable Diffusion</a></li>
-             <li><a href="#Biomedicine">Biomedicine: Acceleration of AlphaFold Protein Structure</a></li>
-           </ul>
-         </li>
-         <li>
            <a href="#Parallel-Training-Demo">Parallel Training Demo</a>
            <ul>
              <li><a href="#GPT-3">GPT-3</a></li>
              <li><a href="#GPT-2">GPT-2</a></li>
              <li><a href="#BERT">BERT</a></li>
              <li><a href="#PaLM">PaLM</a></li>
              <li><a href="#OPT">OPT</a></li>
@@ -80,14 +72,22 @@
            <a href="#Inference-Energon-AI-Demo">Inference (Energon-AI) Demo</a>
            <ul>
              <li><a href="#GPT-3-Inference">GPT-3</a></li>
              <li><a href="#OPT-Serving">OPT-175B Online Serving for Text Generation</a></li>
              <li><a href="#BLOOM-Inference">176B BLOOM</a></li>
            </ul>
          </li>
+           <li>
+           <a href="#Colossal-AI-in-the-Real-World">Colossal-AI for Real World Applications</a>
+           <ul>
+             <li><a href="#ColossalChat">ColossalChat: An Open-Source Solution for Cloning ChatGPT With a Complete RLHF Pipeline</a></li>
+             <li><a href="#AIGC">AIGC: Acceleration of Stable Diffusion</a></li>
+             <li><a href="#Biomedicine">Biomedicine: Acceleration of AlphaFold Protein Structure</a></li>
+           </ul>
+         </li>
          <li>
            <a href="#Installation">Installation</a>
            <ul>
              <li><a href="#PyPI">PyPI</a></li>
              <li><a href="#Install-From-Source">Install From Source</a></li>
            </ul>
          </li>
@@ -129,96 +129,14 @@
           - Parallelism based on the configuration file
         
         - Inference
           - [Energon-AI](https://github.com/hpcaitech/EnergonAI)
         
         <p align="right">(<a href="#top">back to top</a>)</p>
         
-        ## Colossal-AI in the Real World
-        
-        ### ColossalChat
-        
-        <div align="center">
-           <a href="https://chat.colossalai.org/">
-           <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Chat-demo.png" width="700" />
-           </a>
-        </div>
-        
-        [ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://chat.colossalai.org)
-        
-        <p id="ColossalChat_scaling" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT%20scaling.png" width=800/>
-        </p>
-        
-        - Up to 7.73 times faster for single server training and 1.42 times faster for single-GPU inference
-        
-        <p id="ColossalChat-1GPU" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT-1GPU.jpg" width=450/>
-        </p>
-        
-        - Up to 10.3x growth in model capacity on one GPU
-        - A mini demo training process requires only 1.62GB of GPU memory (any consumer-grade GPU)
-        
-        <p id="ColossalChat-LoRA" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/LoRA%20data.jpg" width=600/>
-        </p>
-        
-        - Increase the capacity of the fine-tuning model by up to 3.7 times on a single GPU
-        - Keep at a sufficiently high running speed
-        
-        <p align="right">(<a href="#top">back to top</a>)</p>
-        
-        
-        ### AIGC
-        Acceleration of AIGC (AI-Generated Content) models such as [Stable Diffusion v1](https://github.com/CompVis/stable-diffusion) and [Stable Diffusion v2](https://github.com/Stability-AI/stablediffusion).
-        <p id="diffusion_train" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Stable%20Diffusion%20v2.png" width=800/>
-        </p>
-        
-        - [Training](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/diffusion): Reduce Stable Diffusion memory consumption by up to 5.6x and hardware cost by up to 46x (from A100 to RTX3060).
-        
-        <p id="diffusion_demo" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/DreamBooth.png" width=800/>
-        </p>
-        
-        - [DreamBooth Fine-tuning](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/dreambooth): Personalize your model using just 3-5 images of the desired subject.
-        
-        <p id="inference" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Stable%20Diffusion%20Inference.jpg" width=800/>
-        </p>
-        
-        - [Inference](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/diffusion): Reduce inference GPU memory consumption by 2.5x.
-        
-        
-        <p align="right">(<a href="#top">back to top</a>)</p>
-        
-        ### Biomedicine
-        Acceleration of [AlphaFold Protein Structure](https://alphafold.ebi.ac.uk/)
-        
-        <p id="FastFold" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/FastFold.jpg" width=800/>
-        </p>
-        
-        - [FastFold](https://github.com/hpcaitech/FastFold): Accelerating training and inference on GPU Clusters, faster data processing, inference sequence containing more than 10000 residues.
-        
-        <p id="FastFold-Intel" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/data%20preprocessing%20with%20Intel.jpg" width=600/>
-        </p>
-        
-        - [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference acceleration and 39% cost reduce.
-        
-        <p id="xTrimoMultimer" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/xTrimoMultimer_Table.jpg" width=800/>
-        </p>
-        
-        - [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer): accelerating structure prediction of protein monomers and multimer by 11x.
-        
-        
-        <p align="right">(<a href="#top">back to top</a>)</p>
-        
         ## Parallel Training Demo
         
         ### GPT-3
         <p align="center">
         <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/GPT3-v5.png" width=700/>
         </p>
         
@@ -304,22 +222,102 @@
         <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/BLOOM%20Inference.PNG" width=800/>
         </p>
         
         - [BLOOM](https://github.com/hpcaitech/EnergonAI/tree/main/examples/bloom): Reduce hardware deployment costs of 176-billion-parameter BLOOM by more than 10 times.
         
         <p align="right">(<a href="#top">back to top</a>)</p>
         
+        ## Colossal-AI in the Real World
+        
+        ### ColossalChat
+        
+        <div align="center">
+           <a href="https://chat.colossalai.org/">
+           <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Chat-demo.png" width="700" />
+           </a>
+        </div>
+        
+        [ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://chat.colossalai.org)
+        
+        <p id="ColossalChat_scaling" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT%20scaling.png" width=800/>
+        </p>
+        
+        - Up to 7.73 times faster for single server training and 1.42 times faster for single-GPU inference
+        
+        <p id="ColossalChat-1GPU" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT-1GPU.jpg" width=450/>
+        </p>
+        
+        - Up to 10.3x growth in model capacity on one GPU
+        - A mini demo training process requires only 1.62GB of GPU memory (any consumer-grade GPU)
+        
+        <p id="ColossalChat-LoRA" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/LoRA%20data.jpg" width=600/>
+        </p>
+        
+        - Increase the capacity of the fine-tuning model by up to 3.7 times on a single GPU
+        - Keep at a sufficiently high running speed
+        
+        <p align="right">(<a href="#top">back to top</a>)</p>
+        
+        
+        ### AIGC
+        Acceleration of AIGC (AI-Generated Content) models such as [Stable Diffusion v1](https://github.com/CompVis/stable-diffusion) and [Stable Diffusion v2](https://github.com/Stability-AI/stablediffusion).
+        <p id="diffusion_train" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Stable%20Diffusion%20v2.png" width=800/>
+        </p>
+        
+        - [Training](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/diffusion): Reduce Stable Diffusion memory consumption by up to 5.6x and hardware cost by up to 46x (from A100 to RTX3060).
+        
+        <p id="diffusion_demo" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/DreamBooth.png" width=800/>
+        </p>
+        
+        - [DreamBooth Fine-tuning](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/dreambooth): Personalize your model using just 3-5 images of the desired subject.
+        
+        <p id="inference" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Stable%20Diffusion%20Inference.jpg" width=800/>
+        </p>
+        
+        - [Inference](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/diffusion): Reduce inference GPU memory consumption by 2.5x.
+        
+        
+        <p align="right">(<a href="#top">back to top</a>)</p>
+        
+        ### Biomedicine
+        Acceleration of [AlphaFold Protein Structure](https://alphafold.ebi.ac.uk/)
+        
+        <p id="FastFold" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/FastFold.jpg" width=800/>
+        </p>
+        
+        - [FastFold](https://github.com/hpcaitech/FastFold): Accelerating training and inference on GPU Clusters, faster data processing, inference sequence containing more than 10000 residues.
+        
+        <p id="FastFold-Intel" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/data%20preprocessing%20with%20Intel.jpg" width=600/>
+        </p>
+        
+        - [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference acceleration and 39% cost reduce.
+        
+        <p id="xTrimoMultimer" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/xTrimoMultimer_Table.jpg" width=800/>
+        </p>
+        
+        - [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer): accelerating structure prediction of protein monomers and multimer by 11x.
+        
+        
+        <p align="right">(<a href="#top">back to top</a>)</p>
+        
         ## Installation
         
         Requirements:
         - PyTorch >= 1.11 (PyTorch 2.x in progress)
         - Python >= 3.7
         - CUDA >= 11.0
-        - [NVIDIA GPU Compute Capability](https://developer.nvidia.com/cuda-gpus) >= 7.0 (V100/RTX20 and higher)
-        - Linux OS
         
         If you encounter any problem with installation, you may want to raise an [issue](https://github.com/hpcaitech/ColossalAI/issues/new/choose) in this repository.
         
         ### Install from PyPI
         
         You can easily install Colossal-AI with the following command. **By default, we do not build PyTorch extensions during installation.**
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.4.15 Summary: An
+Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.4.8 Summary: An
 integrated large-scale model training system with efficient parallelization
 techniques Home-page: https://www.colossalai.org License: Apache Software
 License 2.0 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/
 discussions Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/
 issues Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io Project-URL:
 Github, https://github.com/hpcaitech/ColossalAI Description: # Colossal-AI
@@ -45,19 +45,14 @@
 Sequence Exceeding 10,000](https://www.hpc-ai.tech/blog/use-a-laptop-to-
 analyze-90-of-proteins-with-a-single-gpu-inference-sequence-exceeding) * [2022/
 09] [HPC-AI Tech Completes $6 Million Seed and Angel Round Fundraising](https:/
 /www.hpc-ai.tech/blog/hpc-ai-tech-completes-6-million-seed-and-angel-round-
 fundraising-led-by-bluerun-ventures-in-the) ## Table of Contents
     * Why_Colossal-AI
     * Features
-    * Colossal-AI_for_Real_World_Applications
-          o ColossalChat:_An_Open-Source_Solution_for_Cloning_ChatGPT_With_a
-            Complete_RLHF_Pipeline
-          o AIGC:_Acceleration_of_Stable_Diffusion
-          o Biomedicine:_Acceleration_of_AlphaFold_Protein_Structure
     * Parallel_Training_Demo
           o GPT-3
           o GPT-2
           o BERT
           o PaLM
           o OPT
           o ViT
@@ -65,14 +60,19 @@
     * Single_GPU_Training_Demo
           o GPT-2
           o PaLM
     * Inference_(Energon-AI)_Demo
           o GPT-3
           o OPT-175B_Online_Serving_for_Text_Generation
           o 176B_BLOOM
+    * Colossal-AI_for_Real_World_Applications
+          o ColossalChat:_An_Open-Source_Solution_for_Cloning_ChatGPT_With_a
+            Complete_RLHF_Pipeline
+          o AIGC:_Acceleration_of_Stable_Diffusion
+          o Biomedicine:_Acceleration_of_AlphaFold_Protein_Structure
     * Installation
           o PyPI
           o Install_From_Source
     * Use_Docker
     * Community
     * Contributing
     * Cite_Us
@@ -91,71 +91,14 @@
 (https://arxiv.org/abs/2105.13120) - [Zero Redundancy Optimizer (ZeRO)](https:/
 /arxiv.org/abs/1910.02054) - [Auto-Parallelism](https://arxiv.org/abs/
 2302.02599) - Heterogeneous Memory Management - [PatrickStar](https://
 arxiv.org/abs/2108.05818) - Friendly Usage - Parallelism based on the
 configuration file - Inference - [Energon-AI](https://github.com/hpcaitech/
 EnergonAI)
                                                                   (back_to_top)
-## Colossal-AI in the Real World ### ColossalChat
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                                Chat-demo.png]
-[ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/
-Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/
-chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/
-ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/
-@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-
-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://
-chat.colossalai.org)
- [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
-                        chatgpt/ChatGPT%20scaling.png]
-- Up to 7.73 times faster for single server training and 1.42 times faster for
-single-GPU inference
- [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
-                           chatgpt/ChatGPT-1GPU.jpg]
-- Up to 10.3x growth in model capacity on one GPU - A mini demo training
-process requires only 1.62GB of GPU memory (any consumer-grade GPU)
- [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
-                           chatgpt/LoRA%20data.jpg]
-- Increase the capacity of the fine-tuning model by up to 3.7 times on a single
-GPU - Keep at a sufficiently high running speed
-                                                                  (back_to_top)
-### AIGC Acceleration of AIGC (AI-Generated Content) models such as [Stable
-Diffusion v1](https://github.com/CompVis/stable-diffusion) and [Stable
-Diffusion v2](https://github.com/Stability-AI/stablediffusion).
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                         Stable%20Diffusion%20v2.png]
-- [Training](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/
-diffusion): Reduce Stable Diffusion memory consumption by up to 5.6x and
-hardware cost by up to 46x (from A100 to RTX3060).
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                                DreamBooth.png]
-- [DreamBooth Fine-tuning](https://github.com/hpcaitech/ColossalAI/tree/main/
-examples/images/dreambooth): Personalize your model using just 3-5 images of
-the desired subject.
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                      Stable%20Diffusion%20Inference.jpg]
-- [Inference](https://github.com/hpcaitech/ColossalAI/tree/main/examples/
-images/diffusion): Reduce inference GPU memory consumption by 2.5x.
-                                                                  (back_to_top)
-### Biomedicine Acceleration of [AlphaFold Protein Structure](https://
-alphafold.ebi.ac.uk/)
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                                 FastFold.jpg]
-- [FastFold](https://github.com/hpcaitech/FastFold): Accelerating training and
-inference on GPU Clusters, faster data processing, inference sequence
-containing more than 10000 residues.
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                   data%20preprocessing%20with%20Intel.jpg]
-- [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference
-acceleration and 39% cost reduce.
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                           xTrimoMultimer_Table.jpg]
-- [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer):
-accelerating structure prediction of protein monomers and multimer by 11x.
-                                                                  (back_to_top)
 ## Parallel Training Demo ### GPT-3
 [https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
                                  GPT3-v5.png]
 - Save 50% GPU resources and 10.7% acceleration ### GPT-2 [https://
 raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/GPT2.png]
 - 11x lower GPU memory consumption, and superlinear scaling efficiency with
 Tensor Parallelism [https://raw.githubusercontent.com/hpcaitech/public_assets/
@@ -205,35 +148,91 @@
 Try 175-billion-parameter OPT online services
 [https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
                             BLOOM%20Inference.PNG]
 - [BLOOM](https://github.com/hpcaitech/EnergonAI/tree/main/examples/bloom):
 Reduce hardware deployment costs of 176-billion-parameter BLOOM by more than 10
 times.
                                                                   (back_to_top)
+## Colossal-AI in the Real World ### ColossalChat
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                                Chat-demo.png]
+[ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/
+Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/
+chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/
+ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/
+@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-
+with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://
+chat.colossalai.org)
+ [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
+                        chatgpt/ChatGPT%20scaling.png]
+- Up to 7.73 times faster for single server training and 1.42 times faster for
+single-GPU inference
+ [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
+                           chatgpt/ChatGPT-1GPU.jpg]
+- Up to 10.3x growth in model capacity on one GPU - A mini demo training
+process requires only 1.62GB of GPU memory (any consumer-grade GPU)
+ [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
+                           chatgpt/LoRA%20data.jpg]
+- Increase the capacity of the fine-tuning model by up to 3.7 times on a single
+GPU - Keep at a sufficiently high running speed
+                                                                  (back_to_top)
+### AIGC Acceleration of AIGC (AI-Generated Content) models such as [Stable
+Diffusion v1](https://github.com/CompVis/stable-diffusion) and [Stable
+Diffusion v2](https://github.com/Stability-AI/stablediffusion).
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                         Stable%20Diffusion%20v2.png]
+- [Training](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/
+diffusion): Reduce Stable Diffusion memory consumption by up to 5.6x and
+hardware cost by up to 46x (from A100 to RTX3060).
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                                DreamBooth.png]
+- [DreamBooth Fine-tuning](https://github.com/hpcaitech/ColossalAI/tree/main/
+examples/images/dreambooth): Personalize your model using just 3-5 images of
+the desired subject.
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                      Stable%20Diffusion%20Inference.jpg]
+- [Inference](https://github.com/hpcaitech/ColossalAI/tree/main/examples/
+images/diffusion): Reduce inference GPU memory consumption by 2.5x.
+                                                                  (back_to_top)
+### Biomedicine Acceleration of [AlphaFold Protein Structure](https://
+alphafold.ebi.ac.uk/)
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                                 FastFold.jpg]
+- [FastFold](https://github.com/hpcaitech/FastFold): Accelerating training and
+inference on GPU Clusters, faster data processing, inference sequence
+containing more than 10000 residues.
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                   data%20preprocessing%20with%20Intel.jpg]
+- [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference
+acceleration and 39% cost reduce.
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                           xTrimoMultimer_Table.jpg]
+- [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer):
+accelerating structure prediction of protein monomers and multimer by 11x.
+                                                                  (back_to_top)
 ## Installation Requirements: - PyTorch >= 1.11 (PyTorch 2.x in progress) -
-Python >= 3.7 - CUDA >= 11.0 - [NVIDIA GPU Compute Capability](https://
-developer.nvidia.com/cuda-gpus) >= 7.0 (V100/RTX20 and higher) - Linux OS If
-you encounter any problem with installation, you may want to raise an [issue]
-(https://github.com/hpcaitech/ColossalAI/issues/new/choose) in this repository.
-### Install from PyPI You can easily install Colossal-AI with the following
-command. **By default, we do not build PyTorch extensions during
-installation.** ```bash pip install colossalai ``` **Note: only Linux is
-supported for now.** However, if you want to build the PyTorch extensions
-during installation, you can set `CUDA_EXT=1`. ```bash CUDA_EXT=1 pip install
-colossalai ``` **Otherwise, CUDA kernels will be built during runtime when you
-actually need them.** We also keep releasing the nightly version to PyPI every
-week. This allows you to access the unreleased features and bug fixes in the
-main branch. Installation can be made via ```bash pip install colossalai-
-nightly ``` ### Download From Source > The version of Colossal-AI will be in
-line with the main branch of the repository. Feel free to raise an issue if you
-encounter any problems. :) ```shell git clone https://github.com/hpcaitech/
-ColossalAI.git cd ColossalAI # install colossalai pip install . ``` By default,
-we do not compile CUDA/C++ kernels. ColossalAI will build them during runtime.
-If you want to install and enable CUDA kernel fusion (compulsory installation
-when using fused optimizer): ```shell CUDA_EXT=1 pip install . ```
+Python >= 3.7 - CUDA >= 11.0 If you encounter any problem with installation,
+you may want to raise an [issue](https://github.com/hpcaitech/ColossalAI/
+issues/new/choose) in this repository. ### Install from PyPI You can easily
+install Colossal-AI with the following command. **By default, we do not build
+PyTorch extensions during installation.** ```bash pip install colossalai ```
+**Note: only Linux is supported for now.** However, if you want to build the
+PyTorch extensions during installation, you can set `CUDA_EXT=1`. ```bash
+CUDA_EXT=1 pip install colossalai ``` **Otherwise, CUDA kernels will be built
+during runtime when you actually need them.** We also keep releasing the
+nightly version to PyPI every week. This allows you to access the unreleased
+features and bug fixes in the main branch. Installation can be made via ```bash
+pip install colossalai-nightly ``` ### Download From Source > The version of
+Colossal-AI will be in line with the main branch of the repository. Feel free
+to raise an issue if you encounter any problems. :) ```shell git clone https://
+github.com/hpcaitech/ColossalAI.git cd ColossalAI # install colossalai pip
+install . ``` By default, we do not compile CUDA/C++ kernels. ColossalAI will
+build them during runtime. If you want to install and enable CUDA kernel fusion
+(compulsory installation when using fused optimizer): ```shell CUDA_EXT=1 pip
+install . ```
                                                                   (back_to_top)
 ## Use Docker ### Pull from DockerHub You can directly pull the docker image
 from our [DockerHub page](https://hub.docker.com/r/hpcaitech/colossalai). The
 image is automatically uploaded upon release. ### Build On Your Own Run the
 following command to build a docker image from Dockerfile provided. > Building
 Colossal-AI from scratch requires GPU support, you need to use Nvidia Docker
 Runtime as the default when doing `docker build`. More details can be found
```

### Comparing `colossalai-nightly-2023.4.15/README.md` & `colossalai-nightly-2023.4.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,22 +35,14 @@
 * [2022/09] [HPC-AI Tech Completes $6 Million Seed and Angel Round Fundraising](https://www.hpc-ai.tech/blog/hpc-ai-tech-completes-6-million-seed-and-angel-round-fundraising-led-by-bluerun-ventures-in-the)
 
 ## Table of Contents
 <ul>
  <li><a href="#Why-Colossal-AI">Why Colossal-AI</a> </li>
  <li><a href="#Features">Features</a> </li>
  <li>
-   <a href="#Colossal-AI-in-the-Real-World">Colossal-AI for Real World Applications</a>
-   <ul>
-     <li><a href="#ColossalChat">ColossalChat: An Open-Source Solution for Cloning ChatGPT With a Complete RLHF Pipeline</a></li>
-     <li><a href="#AIGC">AIGC: Acceleration of Stable Diffusion</a></li>
-     <li><a href="#Biomedicine">Biomedicine: Acceleration of AlphaFold Protein Structure</a></li>
-   </ul>
- </li>
- <li>
    <a href="#Parallel-Training-Demo">Parallel Training Demo</a>
    <ul>
      <li><a href="#GPT-3">GPT-3</a></li>
      <li><a href="#GPT-2">GPT-2</a></li>
      <li><a href="#BERT">BERT</a></li>
      <li><a href="#PaLM">PaLM</a></li>
      <li><a href="#OPT">OPT</a></li>
@@ -69,14 +61,22 @@
    <a href="#Inference-Energon-AI-Demo">Inference (Energon-AI) Demo</a>
    <ul>
      <li><a href="#GPT-3-Inference">GPT-3</a></li>
      <li><a href="#OPT-Serving">OPT-175B Online Serving for Text Generation</a></li>
      <li><a href="#BLOOM-Inference">176B BLOOM</a></li>
    </ul>
  </li>
+   <li>
+   <a href="#Colossal-AI-in-the-Real-World">Colossal-AI for Real World Applications</a>
+   <ul>
+     <li><a href="#ColossalChat">ColossalChat: An Open-Source Solution for Cloning ChatGPT With a Complete RLHF Pipeline</a></li>
+     <li><a href="#AIGC">AIGC: Acceleration of Stable Diffusion</a></li>
+     <li><a href="#Biomedicine">Biomedicine: Acceleration of AlphaFold Protein Structure</a></li>
+   </ul>
+ </li>
  <li>
    <a href="#Installation">Installation</a>
    <ul>
      <li><a href="#PyPI">PyPI</a></li>
      <li><a href="#Install-From-Source">Install From Source</a></li>
    </ul>
  </li>
@@ -118,96 +118,14 @@
   - Parallelism based on the configuration file
 
 - Inference
   - [Energon-AI](https://github.com/hpcaitech/EnergonAI)
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
-## Colossal-AI in the Real World
-
-### ColossalChat
-
-<div align="center">
-   <a href="https://chat.colossalai.org/">
-   <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Chat-demo.png" width="700" />
-   </a>
-</div>
-
-[ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://chat.colossalai.org)
-
-<p id="ColossalChat_scaling" align="center">
-<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT%20scaling.png" width=800/>
-</p>
-
-- Up to 7.73 times faster for single server training and 1.42 times faster for single-GPU inference
-
-<p id="ColossalChat-1GPU" align="center">
-<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT-1GPU.jpg" width=450/>
-</p>
-
-- Up to 10.3x growth in model capacity on one GPU
-- A mini demo training process requires only 1.62GB of GPU memory (any consumer-grade GPU)
-
-<p id="ColossalChat-LoRA" align="center">
-<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/LoRA%20data.jpg" width=600/>
-</p>
-
-- Increase the capacity of the fine-tuning model by up to 3.7 times on a single GPU
-- Keep at a sufficiently high running speed
-
-<p align="right">(<a href="#top">back to top</a>)</p>
-
-
-### AIGC
-Acceleration of AIGC (AI-Generated Content) models such as [Stable Diffusion v1](https://github.com/CompVis/stable-diffusion) and [Stable Diffusion v2](https://github.com/Stability-AI/stablediffusion).
-<p id="diffusion_train" align="center">
-<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Stable%20Diffusion%20v2.png" width=800/>
-</p>
-
-- [Training](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/diffusion): Reduce Stable Diffusion memory consumption by up to 5.6x and hardware cost by up to 46x (from A100 to RTX3060).
-
-<p id="diffusion_demo" align="center">
-<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/DreamBooth.png" width=800/>
-</p>
-
-- [DreamBooth Fine-tuning](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/dreambooth): Personalize your model using just 3-5 images of the desired subject.
-
-<p id="inference" align="center">
-<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Stable%20Diffusion%20Inference.jpg" width=800/>
-</p>
-
-- [Inference](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/diffusion): Reduce inference GPU memory consumption by 2.5x.
-
-
-<p align="right">(<a href="#top">back to top</a>)</p>
-
-### Biomedicine
-Acceleration of [AlphaFold Protein Structure](https://alphafold.ebi.ac.uk/)
-
-<p id="FastFold" align="center">
-<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/FastFold.jpg" width=800/>
-</p>
-
-- [FastFold](https://github.com/hpcaitech/FastFold): Accelerating training and inference on GPU Clusters, faster data processing, inference sequence containing more than 10000 residues.
-
-<p id="FastFold-Intel" align="center">
-<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/data%20preprocessing%20with%20Intel.jpg" width=600/>
-</p>
-
-- [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference acceleration and 39% cost reduce.
-
-<p id="xTrimoMultimer" align="center">
-<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/xTrimoMultimer_Table.jpg" width=800/>
-</p>
-
-- [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer): accelerating structure prediction of protein monomers and multimer by 11x.
-
-
-<p align="right">(<a href="#top">back to top</a>)</p>
-
 ## Parallel Training Demo
 
 ### GPT-3
 <p align="center">
 <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/GPT3-v5.png" width=700/>
 </p>
 
@@ -293,22 +211,102 @@
 <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/BLOOM%20Inference.PNG" width=800/>
 </p>
 
 - [BLOOM](https://github.com/hpcaitech/EnergonAI/tree/main/examples/bloom): Reduce hardware deployment costs of 176-billion-parameter BLOOM by more than 10 times.
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
+## Colossal-AI in the Real World
+
+### ColossalChat
+
+<div align="center">
+   <a href="https://chat.colossalai.org/">
+   <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Chat-demo.png" width="700" />
+   </a>
+</div>
+
+[ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://chat.colossalai.org)
+
+<p id="ColossalChat_scaling" align="center">
+<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT%20scaling.png" width=800/>
+</p>
+
+- Up to 7.73 times faster for single server training and 1.42 times faster for single-GPU inference
+
+<p id="ColossalChat-1GPU" align="center">
+<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT-1GPU.jpg" width=450/>
+</p>
+
+- Up to 10.3x growth in model capacity on one GPU
+- A mini demo training process requires only 1.62GB of GPU memory (any consumer-grade GPU)
+
+<p id="ColossalChat-LoRA" align="center">
+<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/LoRA%20data.jpg" width=600/>
+</p>
+
+- Increase the capacity of the fine-tuning model by up to 3.7 times on a single GPU
+- Keep at a sufficiently high running speed
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+
+### AIGC
+Acceleration of AIGC (AI-Generated Content) models such as [Stable Diffusion v1](https://github.com/CompVis/stable-diffusion) and [Stable Diffusion v2](https://github.com/Stability-AI/stablediffusion).
+<p id="diffusion_train" align="center">
+<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Stable%20Diffusion%20v2.png" width=800/>
+</p>
+
+- [Training](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/diffusion): Reduce Stable Diffusion memory consumption by up to 5.6x and hardware cost by up to 46x (from A100 to RTX3060).
+
+<p id="diffusion_demo" align="center">
+<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/DreamBooth.png" width=800/>
+</p>
+
+- [DreamBooth Fine-tuning](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/dreambooth): Personalize your model using just 3-5 images of the desired subject.
+
+<p id="inference" align="center">
+<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Stable%20Diffusion%20Inference.jpg" width=800/>
+</p>
+
+- [Inference](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/diffusion): Reduce inference GPU memory consumption by 2.5x.
+
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
+### Biomedicine
+Acceleration of [AlphaFold Protein Structure](https://alphafold.ebi.ac.uk/)
+
+<p id="FastFold" align="center">
+<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/FastFold.jpg" width=800/>
+</p>
+
+- [FastFold](https://github.com/hpcaitech/FastFold): Accelerating training and inference on GPU Clusters, faster data processing, inference sequence containing more than 10000 residues.
+
+<p id="FastFold-Intel" align="center">
+<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/data%20preprocessing%20with%20Intel.jpg" width=600/>
+</p>
+
+- [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference acceleration and 39% cost reduce.
+
+<p id="xTrimoMultimer" align="center">
+<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/xTrimoMultimer_Table.jpg" width=800/>
+</p>
+
+- [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer): accelerating structure prediction of protein monomers and multimer by 11x.
+
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
 ## Installation
 
 Requirements:
 - PyTorch >= 1.11 (PyTorch 2.x in progress)
 - Python >= 3.7
 - CUDA >= 11.0
-- [NVIDIA GPU Compute Capability](https://developer.nvidia.com/cuda-gpus) >= 7.0 (V100/RTX20 and higher)
-- Linux OS
 
 If you encounter any problem with installation, you may want to raise an [issue](https://github.com/hpcaitech/ColossalAI/issues/new/choose) in this repository.
 
 ### Install from PyPI
 
 You can easily install Colossal-AI with the following command. **By default, we do not build PyTorch extensions during installation.**
```

#### html2text {}

```diff
@@ -38,19 +38,14 @@
 Sequence Exceeding 10,000](https://www.hpc-ai.tech/blog/use-a-laptop-to-
 analyze-90-of-proteins-with-a-single-gpu-inference-sequence-exceeding) * [2022/
 09] [HPC-AI Tech Completes $6 Million Seed and Angel Round Fundraising](https:/
 /www.hpc-ai.tech/blog/hpc-ai-tech-completes-6-million-seed-and-angel-round-
 fundraising-led-by-bluerun-ventures-in-the) ## Table of Contents
     * Why_Colossal-AI
     * Features
-    * Colossal-AI_for_Real_World_Applications
-          o ColossalChat:_An_Open-Source_Solution_for_Cloning_ChatGPT_With_a
-            Complete_RLHF_Pipeline
-          o AIGC:_Acceleration_of_Stable_Diffusion
-          o Biomedicine:_Acceleration_of_AlphaFold_Protein_Structure
     * Parallel_Training_Demo
           o GPT-3
           o GPT-2
           o BERT
           o PaLM
           o OPT
           o ViT
@@ -58,14 +53,19 @@
     * Single_GPU_Training_Demo
           o GPT-2
           o PaLM
     * Inference_(Energon-AI)_Demo
           o GPT-3
           o OPT-175B_Online_Serving_for_Text_Generation
           o 176B_BLOOM
+    * Colossal-AI_for_Real_World_Applications
+          o ColossalChat:_An_Open-Source_Solution_for_Cloning_ChatGPT_With_a
+            Complete_RLHF_Pipeline
+          o AIGC:_Acceleration_of_Stable_Diffusion
+          o Biomedicine:_Acceleration_of_AlphaFold_Protein_Structure
     * Installation
           o PyPI
           o Install_From_Source
     * Use_Docker
     * Community
     * Contributing
     * Cite_Us
@@ -84,71 +84,14 @@
 (https://arxiv.org/abs/2105.13120) - [Zero Redundancy Optimizer (ZeRO)](https:/
 /arxiv.org/abs/1910.02054) - [Auto-Parallelism](https://arxiv.org/abs/
 2302.02599) - Heterogeneous Memory Management - [PatrickStar](https://
 arxiv.org/abs/2108.05818) - Friendly Usage - Parallelism based on the
 configuration file - Inference - [Energon-AI](https://github.com/hpcaitech/
 EnergonAI)
                                                                   (back_to_top)
-## Colossal-AI in the Real World ### ColossalChat
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                                Chat-demo.png]
-[ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/
-Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/
-chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/
-ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/
-@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-
-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://
-chat.colossalai.org)
- [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
-                        chatgpt/ChatGPT%20scaling.png]
-- Up to 7.73 times faster for single server training and 1.42 times faster for
-single-GPU inference
- [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
-                           chatgpt/ChatGPT-1GPU.jpg]
-- Up to 10.3x growth in model capacity on one GPU - A mini demo training
-process requires only 1.62GB of GPU memory (any consumer-grade GPU)
- [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
-                           chatgpt/LoRA%20data.jpg]
-- Increase the capacity of the fine-tuning model by up to 3.7 times on a single
-GPU - Keep at a sufficiently high running speed
-                                                                  (back_to_top)
-### AIGC Acceleration of AIGC (AI-Generated Content) models such as [Stable
-Diffusion v1](https://github.com/CompVis/stable-diffusion) and [Stable
-Diffusion v2](https://github.com/Stability-AI/stablediffusion).
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                         Stable%20Diffusion%20v2.png]
-- [Training](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/
-diffusion): Reduce Stable Diffusion memory consumption by up to 5.6x and
-hardware cost by up to 46x (from A100 to RTX3060).
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                                DreamBooth.png]
-- [DreamBooth Fine-tuning](https://github.com/hpcaitech/ColossalAI/tree/main/
-examples/images/dreambooth): Personalize your model using just 3-5 images of
-the desired subject.
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                      Stable%20Diffusion%20Inference.jpg]
-- [Inference](https://github.com/hpcaitech/ColossalAI/tree/main/examples/
-images/diffusion): Reduce inference GPU memory consumption by 2.5x.
-                                                                  (back_to_top)
-### Biomedicine Acceleration of [AlphaFold Protein Structure](https://
-alphafold.ebi.ac.uk/)
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                                 FastFold.jpg]
-- [FastFold](https://github.com/hpcaitech/FastFold): Accelerating training and
-inference on GPU Clusters, faster data processing, inference sequence
-containing more than 10000 residues.
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                   data%20preprocessing%20with%20Intel.jpg]
-- [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference
-acceleration and 39% cost reduce.
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                           xTrimoMultimer_Table.jpg]
-- [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer):
-accelerating structure prediction of protein monomers and multimer by 11x.
-                                                                  (back_to_top)
 ## Parallel Training Demo ### GPT-3
 [https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
                                  GPT3-v5.png]
 - Save 50% GPU resources and 10.7% acceleration ### GPT-2 [https://
 raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/GPT2.png]
 - 11x lower GPU memory consumption, and superlinear scaling efficiency with
 Tensor Parallelism [https://raw.githubusercontent.com/hpcaitech/public_assets/
@@ -198,35 +141,91 @@
 Try 175-billion-parameter OPT online services
 [https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
                             BLOOM%20Inference.PNG]
 - [BLOOM](https://github.com/hpcaitech/EnergonAI/tree/main/examples/bloom):
 Reduce hardware deployment costs of 176-billion-parameter BLOOM by more than 10
 times.
                                                                   (back_to_top)
+## Colossal-AI in the Real World ### ColossalChat
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                                Chat-demo.png]
+[ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/
+Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/
+chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/
+ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/
+@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-
+with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://
+chat.colossalai.org)
+ [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
+                        chatgpt/ChatGPT%20scaling.png]
+- Up to 7.73 times faster for single server training and 1.42 times faster for
+single-GPU inference
+ [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
+                           chatgpt/ChatGPT-1GPU.jpg]
+- Up to 10.3x growth in model capacity on one GPU - A mini demo training
+process requires only 1.62GB of GPU memory (any consumer-grade GPU)
+ [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
+                           chatgpt/LoRA%20data.jpg]
+- Increase the capacity of the fine-tuning model by up to 3.7 times on a single
+GPU - Keep at a sufficiently high running speed
+                                                                  (back_to_top)
+### AIGC Acceleration of AIGC (AI-Generated Content) models such as [Stable
+Diffusion v1](https://github.com/CompVis/stable-diffusion) and [Stable
+Diffusion v2](https://github.com/Stability-AI/stablediffusion).
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                         Stable%20Diffusion%20v2.png]
+- [Training](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/
+diffusion): Reduce Stable Diffusion memory consumption by up to 5.6x and
+hardware cost by up to 46x (from A100 to RTX3060).
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                                DreamBooth.png]
+- [DreamBooth Fine-tuning](https://github.com/hpcaitech/ColossalAI/tree/main/
+examples/images/dreambooth): Personalize your model using just 3-5 images of
+the desired subject.
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                      Stable%20Diffusion%20Inference.jpg]
+- [Inference](https://github.com/hpcaitech/ColossalAI/tree/main/examples/
+images/diffusion): Reduce inference GPU memory consumption by 2.5x.
+                                                                  (back_to_top)
+### Biomedicine Acceleration of [AlphaFold Protein Structure](https://
+alphafold.ebi.ac.uk/)
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                                 FastFold.jpg]
+- [FastFold](https://github.com/hpcaitech/FastFold): Accelerating training and
+inference on GPU Clusters, faster data processing, inference sequence
+containing more than 10000 residues.
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                   data%20preprocessing%20with%20Intel.jpg]
+- [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference
+acceleration and 39% cost reduce.
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                           xTrimoMultimer_Table.jpg]
+- [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer):
+accelerating structure prediction of protein monomers and multimer by 11x.
+                                                                  (back_to_top)
 ## Installation Requirements: - PyTorch >= 1.11 (PyTorch 2.x in progress) -
-Python >= 3.7 - CUDA >= 11.0 - [NVIDIA GPU Compute Capability](https://
-developer.nvidia.com/cuda-gpus) >= 7.0 (V100/RTX20 and higher) - Linux OS If
-you encounter any problem with installation, you may want to raise an [issue]
-(https://github.com/hpcaitech/ColossalAI/issues/new/choose) in this repository.
-### Install from PyPI You can easily install Colossal-AI with the following
-command. **By default, we do not build PyTorch extensions during
-installation.** ```bash pip install colossalai ``` **Note: only Linux is
-supported for now.** However, if you want to build the PyTorch extensions
-during installation, you can set `CUDA_EXT=1`. ```bash CUDA_EXT=1 pip install
-colossalai ``` **Otherwise, CUDA kernels will be built during runtime when you
-actually need them.** We also keep releasing the nightly version to PyPI every
-week. This allows you to access the unreleased features and bug fixes in the
-main branch. Installation can be made via ```bash pip install colossalai-
-nightly ``` ### Download From Source > The version of Colossal-AI will be in
-line with the main branch of the repository. Feel free to raise an issue if you
-encounter any problems. :) ```shell git clone https://github.com/hpcaitech/
-ColossalAI.git cd ColossalAI # install colossalai pip install . ``` By default,
-we do not compile CUDA/C++ kernels. ColossalAI will build them during runtime.
-If you want to install and enable CUDA kernel fusion (compulsory installation
-when using fused optimizer): ```shell CUDA_EXT=1 pip install . ```
+Python >= 3.7 - CUDA >= 11.0 If you encounter any problem with installation,
+you may want to raise an [issue](https://github.com/hpcaitech/ColossalAI/
+issues/new/choose) in this repository. ### Install from PyPI You can easily
+install Colossal-AI with the following command. **By default, we do not build
+PyTorch extensions during installation.** ```bash pip install colossalai ```
+**Note: only Linux is supported for now.** However, if you want to build the
+PyTorch extensions during installation, you can set `CUDA_EXT=1`. ```bash
+CUDA_EXT=1 pip install colossalai ``` **Otherwise, CUDA kernels will be built
+during runtime when you actually need them.** We also keep releasing the
+nightly version to PyPI every week. This allows you to access the unreleased
+features and bug fixes in the main branch. Installation can be made via ```bash
+pip install colossalai-nightly ``` ### Download From Source > The version of
+Colossal-AI will be in line with the main branch of the repository. Feel free
+to raise an issue if you encounter any problems. :) ```shell git clone https://
+github.com/hpcaitech/ColossalAI.git cd ColossalAI # install colossalai pip
+install . ``` By default, we do not compile CUDA/C++ kernels. ColossalAI will
+build them during runtime. If you want to install and enable CUDA kernel fusion
+(compulsory installation when using fused optimizer): ```shell CUDA_EXT=1 pip
+install . ```
                                                                   (back_to_top)
 ## Use Docker ### Pull from DockerHub You can directly pull the docker image
 from our [DockerHub page](https://hub.docker.com/r/hpcaitech/colossalai). The
 image is automatically uploaded upon release. ### Build On Your Own Run the
 following command to build a docker image from Dockerfile provided. > Building
 Colossal-AI from scratch requires GPU support, you need to use Nvidia Docker
 Runtime as the default when doing `docker build`. More details can be found
```

### Comparing `colossalai-nightly-2023.4.15/colossalai/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/amp/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/amp/apex_amp/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/amp/apex_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/amp/apex_amp/apex_amp.py` & `colossalai-nightly-2023.4.8/colossalai/amp/apex_amp/apex_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/amp/naive_amp/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/amp/naive_amp/_fp16_optimizer.py` & `colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/_fp16_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/amp/naive_amp/_utils.py` & `colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py` & `colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py` & `colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py` & `colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/amp/naive_amp/naive_amp.py` & `colossalai-nightly-2023.4.8/colossalai/amp/naive_amp/naive_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/amp/torch_amp/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/amp/torch_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/amp/torch_amp/_grad_scaler.py` & `colossalai-nightly-2023.4.8/colossalai/amp/torch_amp/_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/amp/torch_amp/torch_amp.py` & `colossalai-nightly-2023.4.8/colossalai/amp/torch_amp/torch_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/checkpoint/operation.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/checkpoint/operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/meta_profiler/meta_registry/where.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/meta_registry/where.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/meta_profiler/registry.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/meta_profiler/shard_metainfo.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/meta_profiler/shard_metainfo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/offload/amp_optimizer.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/amp_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/offload/base_offload_module.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/base_offload_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/offload/mem_optimize.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/mem_optimize.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/offload/region.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/region.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/offload/region_manager.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/region_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/offload/runtime.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/runtime.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/offload/solver.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/solver.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/offload/training_simulator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/training_simulator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/offload/util.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/offload/util.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/passes/comm_metainfo_pass.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/passes/comm_metainfo_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/passes/meta_info_prop.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/passes/meta_info_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/passes/runtime_apply_pass.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/passes/runtime_apply_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/passes/runtime_preparation_pass.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/passes/runtime_preparation_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/constants.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/initialize.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/initialize.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/registry.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/options.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/options.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/sharding_strategy.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/sharding_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/solver/solver.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/solver/solver.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/utils/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/utils/broadcast.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/utils/broadcast.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/utils/factory.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/utils/factory.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/utils/misc.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/utils/misc.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/utils/reshape.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/utils/reshape.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/auto_parallel/tensor_shard/utils/sharding.py` & `colossalai-nightly-2023.4.8/colossalai/auto_parallel/tensor_shard/utils/sharding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/booster/accelerator.py` & `colossalai-nightly-2023.4.8/colossalai/booster/accelerator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/booster/booster.py` & `colossalai-nightly-2023.4.8/colossalai/booster/booster.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/booster/mixed_precision/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/booster/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/booster/mixed_precision/fp16_torch.py` & `colossalai-nightly-2023.4.8/colossalai/booster/mixed_precision/fp16_torch.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/booster/mixed_precision/mixed_precision_base.py` & `colossalai-nightly-2023.4.8/colossalai/booster/mixed_precision/mixed_precision_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/booster/plugin/gemini_plugin.py` & `colossalai-nightly-2023.4.8/colossalai/booster/plugin/gemini_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,23 +12,69 @@
 from torch.utils.data import DataLoader
 from torch.utils.data.distributed import DistributedSampler
 
 from colossalai.checkpoint_io import CheckpointIO, GeneralCheckpointIO
 from colossalai.checkpoint_io.utils import save_state_dict
 from colossalai.cluster import DistCoordinator
 from colossalai.interface import ModelWrapper, OptimizerWrapper
+from colossalai.tensor.colo_parameter import ColoParameter
 from colossalai.utils import get_current_device
 from colossalai.zero import GeminiDDP, zero_model_wrapper, zero_optim_wrapper
+from colossalai.zero.gemini.colo_init_context import _convert_to_coloparam
 from colossalai.zero.gemini.memory_tracer import MemStats
 
 from .plugin_base import Plugin
 
 __all__ = ['GeminiPlugin']
 
 
+def convert_to_colo_param(module: nn.Module) -> None:
+    """Convert module's paramters to ColoParameter. This is a workaround and will be deprecated when lazy init is compatible with Gemini.
+
+    Args:
+        module (nn.Module): Module to be converted.
+    """
+    converted_modules = set()    # handle shared modules
+    converted_params = dict()    # record mapping between (torch.Tensor, ColoTensor) to distinguish the same reference
+
+    def convert_recursively(m: nn.Module):
+        for child in m.children():
+            if child not in converted_modules:
+                converted_modules.add(child)
+                convert_recursively(child)
+
+        for name, p in m.named_parameters(recurse=False):
+            assert not isinstance(p, ColoParameter)
+            if p in converted_params:
+                target = converted_params[p]
+            else:
+                target = _convert_to_coloparam(p, p.device, p.dtype)
+                converted_params[p] = target
+            setattr(m, name, target)
+            target.shared_param_modules.append(m)
+
+    convert_recursively(module)
+
+    # optimizer should replace params in group as well. This attr should be deleted after replacing to avoid memory leak
+    module._converted_params = converted_params
+
+
+def replace_param_in_group(optimizer: Optimizer, converted_params: dict) -> None:
+    """Replace param in optimizer's group with converted ColoParameter.
+
+    Args:
+        optimizer (Optimizer): Optimizer to be replaced.
+        converted_params (dict): Mapping between (torch.Tensor, ColoTensor).
+    """
+    for group in optimizer.param_groups:
+        for i, p in enumerate(group['params']):
+            if p in converted_params:
+                group['params'][i] = converted_params[p]
+
+
 class GeminiCheckpointIO(GeneralCheckpointIO):
 
     def __init__(self) -> None:
         super().__init__()
         self.coordinator = DistCoordinator()
 
     def load_unsharded_model(self, model: GeminiDDP, checkpoint: str, strict: bool = True):
@@ -63,24 +109,28 @@
             super().save_lr_scheduler(lr_scheduler, checkpoint)
 
 
 class GeminiModel(ModelWrapper):
 
     def __init__(self, module: nn.Module, gemini_config: dict) -> None:
         super().__init__(module)
+        # TODO(ver217): only support Gemini now
+        convert_to_colo_param(module)
         self.module = zero_model_wrapper(module, zero_stage=3, gemini_config=gemini_config)
 
     def unwrap(self):
         # as save/load state dict is coupled with the GeminiDDP, we only return GeminiDDP model
         return self.module
 
 
 class GeminiOptimizer(OptimizerWrapper):
 
     def __init__(self, module: GeminiDDP, optimizer: Optimizer, zero_optim_config: dict, optim_kwargs: dict) -> None:
+        replace_param_in_group(optimizer, module.module._converted_params)
+        del module.module._converted_params
         optimizer = zero_optim_wrapper(module, optimizer, optim_config=zero_optim_config, **optim_kwargs)
         super().__init__(optimizer)
 
     def backward(self, loss: Tensor, *args, **kwargs):
         self.optim.backward(loss)
 
     def clip_grad_by_norm(self,
```

### Comparing `colossalai-nightly-2023.4.15/colossalai/booster/plugin/plugin_base.py` & `colossalai-nightly-2023.4.8/colossalai/booster/plugin/plugin_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/booster/plugin/torch_ddp_plugin.py` & `colossalai-nightly-2023.4.8/colossalai/booster/plugin/torch_ddp_plugin.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/builder/builder.py` & `colossalai-nightly-2023.4.8/colossalai/builder/builder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/checkpoint_io/checkpoint_io_base.py` & `colossalai-nightly-2023.4.8/colossalai/checkpoint_io/checkpoint_io_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Union
-from typing import Optional
 
 import torch
 import torch.nn as nn
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler as LRScheduler
 
 from colossalai.interface import ModelWrapper
@@ -101,15 +100,15 @@
         return origin_model
 
     def save_model(self,
                    model: Union[nn.Module, ModelWrapper],
                    checkpoint: str,
                    shard: bool = False,
                    gather_dtensor: bool = True,
-                   variant: str = None,
+                   prefix: str = None,
                    size_per_shard: int = 1024,
                    use_safetensors: bool = False):
         """
         Save model to checkpoint.
 
         Examples:
             >>> from colossalai.checkpoint_io import GeneralCheckpointIO
@@ -126,24 +125,24 @@
             checkpoint (str): checkpoint path. The checkpoint path can be :
                 1. a file path, e.g. 'model.pt'
                 2. a directory path to save the sharded checkpoint, e.g. './checkpoints/' when shard = True.
             shard (bool): whether to shard the checkpoint. Default: False. If set to True, the checkpoint will be sharded into
                 multiple files. The model shards will be specificed by a `model.index.json` file. When shard = True, please ensure
                 that the checkpoint path is a directory path instead of a file path.
             gather_dtensor (bool): whether to gather the distributed tensor to the first device. Default: True.
-            variant (str): If specified, weights are saved in the format pytorch_model.<variant>.bin. Default: None.
+            prefix (str): prefix for the model checkpoint file name when shard=True. Default: None.
             size_per_shard (int): size per shard in MB. Default: 1024. This value is only used when shard = True.
             use_safetensors (bool): whether to use safe tensors. Default: False. If set to True, the checkpoint will be saved
         """
 
         if isinstance(model, ModelWrapper):
             model = model.unwrap()
 
         if shard:
-            self.save_sharded_model(model, checkpoint, gather_dtensor, variant, size_per_shard, use_safetensors)
+            self.save_sharded_model(model, checkpoint, gather_dtensor, prefix, size_per_shard, use_safetensors)
         else:
             self.save_unsharded_model(model, checkpoint, gather_dtensor, use_safetensors)
 
     def load_optimizer(self, optimizer: Optimizer, checkpoint: str):
         """
         Load optimizer from checkpoint.
 
@@ -216,15 +215,15 @@
             checkpoint (str): checkpoint path. It should be a single file path pointing to a model weight binary.
             strict (bool): whether to strictly enforce that the param name in
                 the checkpoint match the keys returned by this module's.
         """
         pass
 
     @abstractmethod
-    def save_sharded_model(self, model: nn.Module, checkpoint: str, gather_dtensor: bool, variant: Optional[str],
+    def save_sharded_model(self, model: nn.Module, checkpoint: str, gather_dtensor: bool, prefix: str,
                            size_per_shard: int, use_safetensors: bool):
         """
         Save model to sharded checkpoint.
 
         Args:
             model (nn.Module): model to be saved.
             checkpoint (str): checkpoint path. It should be a directory path.
```

### Comparing `colossalai-nightly-2023.4.15/colossalai/checkpoint_io/general_checkpoint_io.py` & `colossalai-nightly-2023.4.8/colossalai/checkpoint_io/general_checkpoint_io.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,31 +2,28 @@
 
 import torch.nn as nn
 from torch.optim import Optimizer
 import logging
 import os
 import json
 import gc
-from typing import Optional
 
 from .checkpoint_io_base import CheckpointIO
 from .index_file import CheckpointIndexFile
 from .utils import (
     has_index_file, 
     load_state_dict, 
     save_state_dict, 
     is_safetensors_available,
     shard_checkpoint,
     load_shard_state_dict,
-    load_state_dict_into_model,
-    add_variant
+    load_state_dict_into_model
     )
 from .utils import SAFE_WEIGHTS_NAME, WEIGHTS_NAME, SAFE_WEIGHTS_INDEX_NAME, WEIGHTS_INDEX_NAME
 
-
 __all__ = ['GeneralCheckpointIO']
 
 
 class GeneralCheckpointIO(CheckpointIO):
     """
     Checkpoint IO
     """
@@ -68,40 +65,38 @@
         gather_dtensor: bool,
     ):
         # TODO(FrankLeeeee): handle distributed tensors
         save_state_dict(optimizer.state_dict(), checkpoint, use_safetensors=False)
 
 
     def save_sharded_model(self, model: nn.Module, checkpoint_path: str, gather_dtensor:bool = False, 
-                           variant: Optional[str] = None, max_shard_size: int = 1024, use_safetensors: bool = False):
+                           prefix: str = "", max_shard_size: int = 1024, use_safetensors: bool = False):
         """ 
         implement this method as it can be supported by Huggingface model,
         save shard model, save model to multiple files
         """
         if os.path.isfile(checkpoint_path):
             logging.error(f"Provided path ({checkpoint_path}) should be a directory, not a file")
             return
         
         Path(checkpoint_path).mkdir(parents=True, exist_ok=True)
         
         # shard checkpoint
         state_dict = model.state_dict()
         weights_name = SAFE_WEIGHTS_NAME if use_safetensors else WEIGHTS_NAME
-        weights_name = add_variant(weights_name, variant)
         shards, index = shard_checkpoint(state_dict, max_shard_size=max_shard_size, weights_name=weights_name)
 
         # Save the model
         for shard_file, shard in shards.items():
             checkpoint_file_path = os.path.join(checkpoint_path, shard_file)
             save_state_dict(shard, checkpoint_file_path, use_safetensors)
 
         # save index file
         save_index_file = SAFE_WEIGHTS_INDEX_NAME if use_safetensors else WEIGHTS_INDEX_NAME
-
-        save_index_file = os.path.join(checkpoint_path, add_variant(save_index_file, variant))
+        save_index_file = os.path.join(checkpoint_path, save_index_file)
         with open(save_index_file, "w", encoding="utf-8") as f:
             content = json.dumps(index, indent=2, sort_keys=True) + "\n"
             f.write(content)
         logging.info(
             f"The model is bigger than the maximum size per checkpoint ({max_shard_size}) and is going to be "
             f"split in {len(shards)} checkpoint shards. You can find where each parameters has been saved in the "
             f"index located at {save_index_file}."
```

### Comparing `colossalai-nightly-2023.4.15/colossalai/checkpoint_io/index_file.py` & `colossalai-nightly-2023.4.8/colossalai/checkpoint_io/index_file.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/checkpoint_io/utils.py` & `colossalai-nightly-2023.4.8/colossalai/checkpoint_io/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # coding=utf-8
 from pathlib import Path
 import torch
 import torch.nn as nn
 from typing import List, Dict, Mapping, OrderedDict, Optional, Tuple
 from colossalai.tensor.d_tensor.d_tensor import DTensor
-import re
 
 SAFE_WEIGHTS_NAME = "model.safetensors"
-WEIGHTS_NAME = "pytorch_model.bin"
+WEIGHTS_NAME = "model.bin"
 SAFE_WEIGHTS_INDEX_NAME = "model.safetensors.index.json"
-WEIGHTS_INDEX_NAME = "pytorch_model.bin.index.json"
+WEIGHTS_INDEX_NAME = "model.bin.index.json"
 
 # ======================================
 # General helper functions
 # ======================================
 
 def calculate_tensor_size(tensor: torch.Tensor) -> float:
     """
@@ -24,14 +23,15 @@
         tenosr (torch.Tensor): the tensor to calculate size for.
 
     Returns:
         float: size of the tensor in MB.
     """
     return tensor.numel() * tensor.element_size() / 1024 / 1024
 
+
 def is_safetensors_available() -> bool:
     """
     Check whether safetensors is available.
 
     Returns:
         bool: whether safetensors is available.
     """
@@ -354,22 +354,21 @@
 
     Returns:
         Tuple[bool, Optional[Path]]: a tuple of (has_index_file, index_file_path)
     """
     checkpoint_path = Path(checkpoint_path)
     if checkpoint_path.is_file():
         # check if it is .index.json
-        reg = re.compile("(.*?).index((\..*)?).json")
-        if reg.fullmatch(checkpoint_path.name) is not None:
+        if checkpoint_path.name.endswith('.index.json'):
             return True, checkpoint_path
         else:
             return False, None
     elif checkpoint_path.is_dir():
         # check if there is only one a file ending with .index.json in this directory
-        index_files = list(checkpoint_path.glob('*.index.*json'))
+        index_files = list(checkpoint_path.glob('*.index.json'))
 
         # if we found a .index.json file, make sure there is only one
         if len(index_files) > 0:
             assert len(
                 index_files
             ) == 1, f'Expected to find one .index.json file in {checkpoint_path}, but found {len(index_files)}'
 
@@ -403,17 +402,7 @@
             for k in f.keys():
                 state_dict[k] = f.get_tensor(k)
         return state_dict
 
     else:
         # load with torch
         return torch.load(checkpoint_file_path)
-    
-
-
-def add_variant(weights_name: str, variant: Optional[str] = None) -> str:
-    if variant is not None and len(variant) > 0:
-        splits = weights_name.split(".")
-        splits = splits[:-1] + [variant] + splits[-1:]
-        weights_name = ".".join(splits)
-
-    return weights_name
```

### Comparing `colossalai-nightly-2023.4.15/colossalai/cli/benchmark/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/cli/benchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/cli/benchmark/benchmark.py` & `colossalai-nightly-2023.4.8/colossalai/cli/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/cli/benchmark/utils.py` & `colossalai-nightly-2023.4.8/colossalai/cli/benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/cli/check/check_installation.py` & `colossalai-nightly-2023.4.8/colossalai/cli/check/check_installation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/cli/launcher/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/cli/launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/cli/launcher/hostinfo.py` & `colossalai-nightly-2023.4.8/colossalai/cli/launcher/hostinfo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/cli/launcher/multinode_runner.py` & `colossalai-nightly-2023.4.8/colossalai/cli/launcher/multinode_runner.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/cli/launcher/run.py` & `colossalai-nightly-2023.4.8/colossalai/cli/launcher/run.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/cluster/device_mesh_manager.py` & `colossalai-nightly-2023.4.8/colossalai/cluster/device_mesh_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/cluster/dist_coordinator.py` & `colossalai-nightly-2023.4.8/colossalai/cluster/dist_coordinator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/cluster/process_group_manager.py` & `colossalai-nightly-2023.4.8/colossalai/cluster/process_group_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/communication/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/communication/collective.py` & `colossalai-nightly-2023.4.8/colossalai/communication/collective.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/communication/p2p.py` & `colossalai-nightly-2023.4.8/colossalai/communication/p2p.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/communication/p2p_v2.py` & `colossalai-nightly-2023.4.8/colossalai/communication/p2p_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/communication/ring.py` & `colossalai-nightly-2023.4.8/colossalai/communication/ring.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/communication/utils.py` & `colossalai-nightly-2023.4.8/colossalai/communication/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/constants.py` & `colossalai-nightly-2023.4.8/colossalai/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/context/config.py` & `colossalai-nightly-2023.4.8/colossalai/context/config.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/context/moe_context.py` & `colossalai-nightly-2023.4.8/colossalai/context/moe_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/context/parallel_context.py` & `colossalai-nightly-2023.4.8/colossalai/context/parallel_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/context/parallel_mode.py` & `colossalai-nightly-2023.4.8/colossalai/context/parallel_mode.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/context/process_group_initializer/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/context/process_group_initializer/initializer_1d.py` & `colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_1d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/context/process_group_initializer/initializer_2d.py` & `colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_2d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/context/process_group_initializer/initializer_2p5d.py` & `colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_2p5d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/context/process_group_initializer/initializer_3d.py` & `colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_3d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/context/process_group_initializer/initializer_data.py` & `colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_data.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/context/process_group_initializer/initializer_model.py` & `colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/context/process_group_initializer/initializer_pipeline.py` & `colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_pipeline.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/context/process_group_initializer/initializer_sequence.py` & `colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_sequence.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/context/process_group_initializer/initializer_tensor.py` & `colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/initializer_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/context/process_group_initializer/process_group_initializer.py` & `colossalai-nightly-2023.4.8/colossalai/context/process_group_initializer/process_group_initializer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/context/random/_helper.py` & `colossalai-nightly-2023.4.8/colossalai/context/random/_helper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/context/random/seed_manager.py` & `colossalai-nightly-2023.4.8/colossalai/context/random/seed_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/context/singleton_meta.py` & `colossalai-nightly-2023.4.8/colossalai/context/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/device/alpha_beta_profiler.py` & `colossalai-nightly-2023.4.8/colossalai/device/alpha_beta_profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/device/calc_pipeline_strategy.py` & `colossalai-nightly-2023.4.8/colossalai/device/calc_pipeline_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/device/device_mesh.py` & `colossalai-nightly-2023.4.8/colossalai/device/device_mesh.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/engine/_base_engine.py` & `colossalai-nightly-2023.4.8/colossalai/engine/_base_engine.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/engine/gradient_accumulation/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/engine/gradient_accumulation/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/engine/gradient_accumulation/_gradient_accumulation.py` & `colossalai-nightly-2023.4.8/colossalai/engine/gradient_accumulation/_gradient_accumulation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/engine/gradient_handler/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/engine/gradient_handler/_base_gradient_handler.py` & `colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/_base_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py` & `colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/engine/gradient_handler/_moe_gradient_handler.py` & `colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/_moe_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py` & `colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py` & `colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/engine/gradient_handler/_zero_gradient_handler.py` & `colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/_zero_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/engine/gradient_handler/utils.py` & `colossalai-nightly-2023.4.8/colossalai/engine/gradient_handler/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/engine/schedule/_base_schedule.py` & `colossalai-nightly-2023.4.8/colossalai/engine/schedule/_base_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/engine/schedule/_non_pipeline_schedule.py` & `colossalai-nightly-2023.4.8/colossalai/engine/schedule/_non_pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/engine/schedule/_pipeline_schedule.py` & `colossalai-nightly-2023.4.8/colossalai/engine/schedule/_pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/engine/schedule/_pipeline_schedule_v2.py` & `colossalai-nightly-2023.4.8/colossalai/engine/schedule/_pipeline_schedule_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/_compatibility.py` & `colossalai-nightly-2023.4.8/colossalai/fx/_compatibility.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/_meta_regist_12.py` & `colossalai-nightly-2023.4.8/colossalai/fx/_meta_regist_12.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/_meta_regist_13.py` & `colossalai-nightly-2023.4.8/colossalai/fx/_meta_regist_13.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/codegen/activation_checkpoint_codegen.py` & `colossalai-nightly-2023.4.8/colossalai/fx/codegen/activation_checkpoint_codegen.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/graph_module.py` & `colossalai-nightly-2023.4.8/colossalai/fx/graph_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/passes/adding_split_node_pass.py` & `colossalai-nightly-2023.4.8/colossalai/fx/passes/adding_split_node_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/passes/concrete_info_prop.py` & `colossalai-nightly-2023.4.8/colossalai/fx/passes/concrete_info_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/passes/meta_info_prop.py` & `colossalai-nightly-2023.4.8/colossalai/fx/passes/meta_info_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/passes/passes_for_gpt2_test.py` & `colossalai-nightly-2023.4.8/colossalai/fx/passes/passes_for_gpt2_test.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/passes/shard_1d_pass.py` & `colossalai-nightly-2023.4.8/colossalai/fx/passes/shard_1d_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/passes/split_module.py` & `colossalai-nightly-2023.4.8/colossalai/fx/passes/split_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/passes/utils.py` & `colossalai-nightly-2023.4.8/colossalai/fx/passes/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/profiler/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/profiler/constants.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/profiler/dataflow.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/dataflow.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/constants.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_function/activation_function.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/activation_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_function/embedding.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_function/normalization.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_function/pooling.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_module/activation_function.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/activation_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_module/attention.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/attention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_module/convolution.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_module/normalization.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_module/pooling.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/profiler_module/rnn.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/profiler_module/rnn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/registry.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/profiler/experimental/shard_utils.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/experimental/shard_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/profiler/memory_utils.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/memory_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/profiler/opcount.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/opcount.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/profiler/profiler.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/profiler/shard_utils.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/shard_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/profiler/tensor.py` & `colossalai-nightly-2023.4.8/colossalai/fx/profiler/tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/proxy.py` & `colossalai-nightly-2023.4.8/colossalai/fx/proxy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/tracer/_meta_trace.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/_meta_trace.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/tracer/_symbolic_trace.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/_symbolic_trace.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/tracer/_tracer_utils.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/_tracer_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/tracer/experimental.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/experimental.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/patched_function/convolution.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/patched_function/embedding.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/patched_function/normalization.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/patched_module/convolution.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_module/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/patched_module/normalization.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_module/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/patched_module/pooling.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_module/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/tracer/meta_patch/patched_module/rnn.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/meta_patch/patched_module/rnn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/tracer/registry.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/fx/tracer/tracer.py` & `colossalai-nightly-2023.4.8/colossalai/fx/tracer/tracer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/global_variables.py` & `colossalai-nightly-2023.4.8/colossalai/global_variables.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/initialize.py` & `colossalai-nightly-2023.4.8/colossalai/initialize.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/interface/model.py` & `colossalai-nightly-2023.4.8/colossalai/interface/model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/interface/optimizer.py` & `colossalai-nightly-2023.4.8/colossalai/interface/optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/cpu_adam.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/cpu_adam.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/include/context.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/context.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/csrc/type_shim.h` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/csrc/type_shim.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/flash_attention.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/flash_attention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/layer_norm.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/layer_norm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/multihead_attention.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/cuda_native/scaled_softmax.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/cuda_native/scaled_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/jit/bias_dropout_add.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/jit/bias_dropout_add.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/jit/bias_gelu.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/jit/bias_gelu.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/jit/option.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/jit/option.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/op_builder/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/op_builder/builder.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/builder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/op_builder/cpu_adam.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/op_builder/fused_optim.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/fused_optim.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/op_builder/layernorm.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/layernorm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/op_builder/moe.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/op_builder/multi_head_attn.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/multi_head_attn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/op_builder/scaled_masked_softmax.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/scaled_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/kernel/op_builder/utils.py` & `colossalai-nightly-2023.4.8/colossalai/kernel/op_builder/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/logging/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/logging/logger.py` & `colossalai-nightly-2023.4.8/colossalai/logging/logger.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/_ops/_utils.py` & `colossalai-nightly-2023.4.8/colossalai/nn/_ops/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/_ops/addmm.py` & `colossalai-nightly-2023.4.8/colossalai/nn/_ops/addmm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/_ops/batch_norm.py` & `colossalai-nightly-2023.4.8/colossalai/nn/_ops/batch_norm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/_ops/element_wise.py` & `colossalai-nightly-2023.4.8/colossalai/nn/_ops/element_wise.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/_ops/embedding.py` & `colossalai-nightly-2023.4.8/colossalai/nn/_ops/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/_ops/embedding_bag.py` & `colossalai-nightly-2023.4.8/colossalai/nn/_ops/embedding_bag.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/_ops/layernorm.py` & `colossalai-nightly-2023.4.8/colossalai/nn/_ops/layernorm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/_ops/linear.py` & `colossalai-nightly-2023.4.8/colossalai/nn/_ops/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/_ops/loss.py` & `colossalai-nightly-2023.4.8/colossalai/nn/_ops/loss.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/_ops/view.py` & `colossalai-nightly-2023.4.8/colossalai/nn/_ops/view.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/init.py` & `colossalai-nightly-2023.4.8/colossalai/nn/init.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/base_layer.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/base_layer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/colossalai_layer/_utils.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/colossalai_layer/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/colossalai_layer/dropout.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/colossalai_layer/dropout.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/colossalai_layer/embedding.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/colossalai_layer/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/colossalai_layer/linear.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/colossalai_layer/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/colossalai_layer/normalization.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/colossalai_layer/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/moe/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/moe/_operation.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/moe/checkpoint.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/moe/experts.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/experts.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/moe/layers.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/moe/routers.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/routers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/moe/utils.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/moe/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_1d/_operation.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_1d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_1d/_utils.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_1d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_1d/layers.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_1d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_2d/_operation.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_2d/_utils.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_2d/layers.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_2p5d/_operation.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2p5d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_2p5d/_utils.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2p5d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_2p5d/layers.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_2p5d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_3d/_operation.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_3d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_3d/_utils.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_3d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_3d/layers.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_3d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_sequence/_operation.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_sequence/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/parallel_sequence/layers.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/parallel_sequence/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/utils/common.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/utils/common.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/vanilla/layers.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/vanilla/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/layer/wrapper/pipeline_wrapper.py` & `colossalai-nightly-2023.4.8/colossalai/nn/layer/wrapper/pipeline_wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/loss/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/nn/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/loss/loss_1d.py` & `colossalai-nightly-2023.4.8/colossalai/nn/loss/loss_1d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/loss/loss_2d.py` & `colossalai-nightly-2023.4.8/colossalai/nn/loss/loss_2d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/loss/loss_2p5d.py` & `colossalai-nightly-2023.4.8/colossalai/nn/loss/loss_2p5d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/loss/loss_3d.py` & `colossalai-nightly-2023.4.8/colossalai/nn/loss/loss_3d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/loss/loss_moe.py` & `colossalai-nightly-2023.4.8/colossalai/nn/loss/loss_moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/lr_scheduler/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/lr_scheduler/cosine.py` & `colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/cosine.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/lr_scheduler/delayed.py` & `colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/delayed.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/lr_scheduler/linear.py` & `colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/lr_scheduler/multistep.py` & `colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/multistep.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/lr_scheduler/onecycle.py` & `colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/onecycle.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/lr_scheduler/poly.py` & `colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/poly.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/lr_scheduler/torch.py` & `colossalai-nightly-2023.4.8/colossalai/nn/lr_scheduler/torch.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/metric/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/nn/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/metric/accuracy_2d.py` & `colossalai-nightly-2023.4.8/colossalai/nn/metric/accuracy_2d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/metric/accuracy_2p5d.py` & `colossalai-nightly-2023.4.8/colossalai/nn/metric/accuracy_2p5d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/metric/accuracy_3d.py` & `colossalai-nightly-2023.4.8/colossalai/nn/metric/accuracy_3d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/optimizer/colossalai_optimizer.py` & `colossalai-nightly-2023.4.8/colossalai/nn/optimizer/colossalai_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/optimizer/cpu_adam.py` & `colossalai-nightly-2023.4.8/colossalai/nn/optimizer/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/optimizer/fused_adam.py` & `colossalai-nightly-2023.4.8/colossalai/nn/optimizer/fused_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/optimizer/fused_lamb.py` & `colossalai-nightly-2023.4.8/colossalai/nn/optimizer/fused_lamb.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/optimizer/fused_sgd.py` & `colossalai-nightly-2023.4.8/colossalai/nn/optimizer/fused_sgd.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/optimizer/hybrid_adam.py` & `colossalai-nightly-2023.4.8/colossalai/nn/optimizer/hybrid_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/optimizer/lamb.py` & `colossalai-nightly-2023.4.8/colossalai/nn/optimizer/lamb.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/optimizer/lars.py` & `colossalai-nightly-2023.4.8/colossalai/nn/optimizer/lars.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/optimizer/nvme_optimizer.py` & `colossalai-nightly-2023.4.8/colossalai/nn/optimizer/nvme_optimizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-import math
+import torch
 import os
 import tempfile
-from typing import Callable, Dict, List, Optional
-
-import torch
+import math
 from torch.nn.parameter import Parameter
+from typing import Optional, List, Dict, Callable
 
 
 class NVMeOptimizer(torch.optim.Optimizer):
     """A base class for offloading optimizer states.
 
     Args:
         params: parameters
@@ -39,17 +38,16 @@
             backend = 'uring' if 'uring' in get_backends() else 'aio'
             self.offloader = DiskOffloader(self.offload_dir, 8, backend=backend)
         else:
             self.offload_dir = None
             self.offloader = None
         self.is_on_nvme: Dict[Parameter, bool] = {}
         self.offloaded_numel: int = 0
-        # As param may be not materialized here, these attributes are initalized when the first step
-        self.total_numel: Optional[int] = None
-        self.can_offload_numel: Optional[int] = None
+        self.total_numel: int = self._get_numel()
+        self.can_offload_numel = math.floor(self.total_numel * self.nvme_offload_fraction)
 
         self.prefetch_params: List[Parameter] = []
         self.param_to_prefetch_idx: Dict[Parameter, int] = {}
 
     def _get_numel(self) -> int:
         numel = 0
         for group in self.param_groups:
@@ -75,17 +73,14 @@
                     continue
                 if len(self.state[p]) > 0 and self.is_on_nvme[p]:
                     assert p.device.type == 'cpu'
                     self.param_to_prefetch_idx[p] = len(self.prefetch_params)
                     self.prefetch_params.append(p)
 
     def _pre_step(self, *state_keys: str) -> None:
-        if self.total_numel is None:
-            self.total_numel = self._get_numel()
-            self.can_offload_numel = math.floor(self.total_numel * self.nvme_offload_fraction)
         self._setup_prefetch_params()
         if self.offloader is None or len(self.prefetch_params) == 0:
             return
         state = self.state[self.prefetch_params[0]]
         for key in state_keys:
             self.offloader.async_read(state[key])
```

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/parallel/data_parallel.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/data_parallel.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/cache_embedding/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/cache_embedding/copyer.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/copyer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/colo_module.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/colo_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/embedding.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/linear.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/parallel/layers/module_utils.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/layers/module_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/nn/parallel/reducer.py` & `colossalai-nightly-2023.4.8/colossalai/nn/parallel/reducer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/pipeline/layer_spec.py` & `colossalai-nightly-2023.4.8/colossalai/pipeline/layer_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/pipeline/middleware/adaptor/fx.py` & `colossalai-nightly-2023.4.8/colossalai/pipeline/middleware/adaptor/fx.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/pipeline/middleware/topo.py` & `colossalai-nightly-2023.4.8/colossalai/pipeline/middleware/topo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/pipeline/pipelinable.py` & `colossalai-nightly-2023.4.8/colossalai/pipeline/pipelinable.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/pipeline/pipeline_process_group.py` & `colossalai-nightly-2023.4.8/colossalai/pipeline/pipeline_process_group.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/pipeline/rpc/_pipeline_base.py` & `colossalai-nightly-2023.4.8/colossalai/pipeline/rpc/_pipeline_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/pipeline/rpc/_pipeline_schedule.py` & `colossalai-nightly-2023.4.8/colossalai/pipeline/rpc/_pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/pipeline/rpc/utils.py` & `colossalai-nightly-2023.4.8/colossalai/pipeline/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/pipeline/utils.py` & `colossalai-nightly-2023.4.8/colossalai/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/registry/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/registry/registry.py` & `colossalai-nightly-2023.4.8/colossalai/registry/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/tensor/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/tensor/colo_parameter.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/colo_parameter.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/tensor/colo_tensor.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/colo_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/tensor/comm_spec.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/comm_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/tensor/compute_spec.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/compute_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/tensor/d_tensor/comm_spec.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/comm_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/tensor/d_tensor/d_tensor.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/d_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/tensor/d_tensor/layout.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/layout.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/tensor/d_tensor/layout_converter.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/layout_converter.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/tensor/d_tensor/sharding_spec.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/sharding_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/tensor/d_tensor/utils.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/d_tensor/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/tensor/dist_spec_mgr.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/dist_spec_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/tensor/distspec.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/distspec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/tensor/op_wrapper.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/op_wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/tensor/param_op_hook.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/param_op_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/tensor/process_group.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/process_group.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/tensor/shape_consistency.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/shape_consistency.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/tensor/sharding_spec.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/sharding_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/tensor/tensor_spec.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/tensor_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/tensor/utils.py` & `colossalai-nightly-2023.4.8/colossalai/tensor/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/testing/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/testing/comparison.py` & `colossalai-nightly-2023.4.8/colossalai/testing/comparison.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/testing/pytest_wrapper.py` & `colossalai-nightly-2023.4.8/colossalai/testing/pytest_wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/testing/random.py` & `colossalai-nightly-2023.4.8/colossalai/testing/random.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/testing/utils.py` & `colossalai-nightly-2023.4.8/colossalai/testing/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/trainer/_trainer.py` & `colossalai-nightly-2023.4.8/colossalai/trainer/_trainer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/trainer/hooks/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/trainer/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/trainer/hooks/_base_hook.py` & `colossalai-nightly-2023.4.8/colossalai/trainer/hooks/_base_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/trainer/hooks/_checkpoint_hook.py` & `colossalai-nightly-2023.4.8/colossalai/trainer/hooks/_checkpoint_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/trainer/hooks/_log_hook.py` & `colossalai-nightly-2023.4.8/colossalai/trainer/hooks/_log_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/trainer/hooks/_lr_scheduler_hook.py` & `colossalai-nightly-2023.4.8/colossalai/trainer/hooks/_lr_scheduler_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/trainer/hooks/_metric_hook.py` & `colossalai-nightly-2023.4.8/colossalai/trainer/hooks/_metric_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/activation_checkpoint.py` & `colossalai-nightly-2023.4.8/colossalai/utils/activation_checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/checkpoint/module_checkpoint.py` & `colossalai-nightly-2023.4.8/colossalai/utils/checkpoint/module_checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/checkpoint/utils.py` & `colossalai-nightly-2023.4.8/colossalai/utils/checkpoint/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/checkpoint_io/backend.py` & `colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/backend.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/checkpoint_io/convertor.py` & `colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/convertor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/checkpoint_io/distributed.py` & `colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/distributed.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/checkpoint_io/io.py` & `colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/io.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/checkpoint_io/meta.py` & `colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/meta.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/checkpoint_io/reader.py` & `colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/reader.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/checkpoint_io/utils.py` & `colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/checkpoint_io/writer.py` & `colossalai-nightly-2023.4.8/colossalai/utils/checkpoint_io/writer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/checkpointing.py` & `colossalai-nightly-2023.4.8/colossalai/utils/checkpointing.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/common.py` & `colossalai-nightly-2023.4.8/colossalai/utils/common.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/cuda.py` & `colossalai-nightly-2023.4.8/colossalai/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/data_sampler/data_parallel_sampler.py` & `colossalai-nightly-2023.4.8/colossalai/utils/data_sampler/data_parallel_sampler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/memory.py` & `colossalai-nightly-2023.4.8/colossalai/utils/memory.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/model/experimental.py` & `colossalai-nightly-2023.4.8/colossalai/utils/model/experimental.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import torch
 import torch.distributed as dist
 import torch.nn as nn
 from torch import Tensor
 from torch.utils._pytree import tree_map
 
-from colossalai._analyzer._subclasses import MetaTensor
+from colossalai.fx.profiler.tensor import MetaTensor
 from colossalai.tensor.d_tensor.d_tensor import DTensor
 from colossalai.tensor.d_tensor.layout import Layout
 
 # reference: https://pytorch.org/cppdocs/notes/tensor_creation.html
 _NORMAL_FACTORY = [
     "arange",
     "empty",
@@ -33,15 +33,15 @@
 ]
 
 _EARLY_MATERIALIZED_OPS = ['__getitem__', 'split']
 
 # If your intent is to change the metadata of a Tensor (such as sizes / strides / storage / storage_offset)
 # without autograd tracking the change, remove the .data / .detach() call and wrap the change in a `with torch.no_grad():` block.
 # These ops cannot be unwrapped using .data
-_CHANGE_META_OPS = ['_cudnn_rnn_flatten_weight', 'requires_grad_', '__get__', '__set__']
+_CHANGE_META_OPS = ['_cudnn_rnn_flatten_weight', 'requires_grad_', '__get__']
 
 _LEGACY_TENSOR_CONSTRUCTOR = {
     'FloatTensor': torch.float,
     'DoubleTensor': torch.double,
     'HalfTensor': torch.half,
     'BFloat16Tensor': torch.bfloat16,
     'ByteTensor': torch.uint8,
@@ -71,20 +71,14 @@
 
     @classmethod
     def __torch_function__(cls, func, types, args=(), kwargs=None):
         cls._pre_op_fn()
         return super().__torch_function__(func, types, args, kwargs)
 
 
-def _data_tolist(tensor: torch.Tensor) -> list:
-    """tolist() method is not allowed for a subclass of tensor. Tensor.data returns a Tensor.
-    """
-    return tensor.data.tolist()
-
-
 def _convert_cls(tensor: 'LazyTensor', target: torch.Tensor) -> torch.Tensor:
     """Convert a lazy tensor's class to target's class, with target's data.
 
     The reason why we change the class of a lazy tensor in-place is that this can easily handle shared modules/parameters, which is common in huggingface models.
     If we create a new tensor and update the module by ``setattr(module, name, param)``, the shared parameters will not be updated. And we have to track all shared parameters and update them manually.
 
     Args:
@@ -96,15 +90,15 @@
     """
     cls_to_become = nn.Parameter if isinstance(tensor, nn.Parameter) else torch.Tensor
     tensor.__class__ = cls_to_become
     tensor.data = target
     tensor.requires_grad = target.requires_grad
     # subclass of torch.Tensor does not have tolist() method
     # overwrite this method after materialization or distribution
-    tensor.tolist = MethodType(_data_tolist, tensor)
+    tensor.tolist = MethodType(torch.Tensor.tolist, target)
     return tensor
 
 
 class LazyTensor(torch.Tensor):
     """A naive implementation of LazyTensor (https://arxiv.org/pdf/2102.13267.pdf).
 
     Usage:
@@ -146,15 +140,15 @@
         if concrete_data is not None:
             # some ops don't support meta backend and should have concrete data
             elem = concrete_data
         else:
             if meta_data is None:
                 device = kwargs.get('device', 'cpu')
                 elem = func(*args, **{**kwargs, 'device': 'meta'})
-                meta_data = MetaTensor(elem, device=device)
+                meta_data = MetaTensor(elem, fake_device=device)
             elem = meta_data._tensor
         # As a meta tensor cannot be modified __class__ to torch.Tensor, we should use an empty real tensor here
         r = torch.Tensor._make_subclass(cls, _EMPTY_DATA, require_grad=elem.requires_grad)
         r._meta_data = meta_data
         return r
 
     def __init__(self, func, *args, meta_data=None, concrete_data=None, **kwargs):
@@ -257,15 +251,15 @@
         if kwargs is None:
             kwargs = {}
         if func.__name__ in _EARLY_MATERIALIZED_OPS:
             # These OPs cannot be lazy and related tensors should be early materialized
             tree_map(cls._replace_with_materialized, args)
             tree_map(cls._replace_with_materialized, kwargs)
         is_inplace: bool = (func.__name__.endswith('_') and not (func.__name__.endswith('__'))
-                            or func.__name__ in ('__setitem__', '__set__'))
+                            or func.__name__ == "__setitem__")
 
         is_change_meta_op: bool = func.__name__ in _CHANGE_META_OPS
 
         if isinstance(func, torch._C.ScriptMethod):
             # FIXME(ver217): torch script functions are not verified
 
             target = None
```

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/model/lazy_init_context.py` & `colossalai-nightly-2023.4.8/colossalai/utils/model/lazy_init_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/model/utils.py` & `colossalai-nightly-2023.4.8/colossalai/utils/model/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/moe.py` & `colossalai-nightly-2023.4.8/colossalai/utils/moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py` & `colossalai-nightly-2023.4.8/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/profiler/legacy/comm_profiler.py` & `colossalai-nightly-2023.4.8/colossalai/utils/profiler/legacy/comm_profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/profiler/legacy/pcie_profiler.py` & `colossalai-nightly-2023.4.8/colossalai/utils/profiler/legacy/pcie_profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/profiler/legacy/prof_utils.py` & `colossalai-nightly-2023.4.8/colossalai/utils/profiler/legacy/prof_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/profiler/profiler.py` & `colossalai-nightly-2023.4.8/colossalai/utils/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/profiler/stateful_tensor_mem_extention.py` & `colossalai-nightly-2023.4.8/colossalai/utils/profiler/stateful_tensor_mem_extention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/rank_recorder/rank_recorder.py` & `colossalai-nightly-2023.4.8/colossalai/utils/rank_recorder/rank_recorder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/tensor_detector/tensor_detector.py` & `colossalai-nightly-2023.4.8/colossalai/utils/tensor_detector/tensor_detector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/utils/timer.py` & `colossalai-nightly-2023.4.8/colossalai/utils/timer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/zero/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/gemini/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/gemini/chunk/chunk.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/chunk/chunk.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/gemini/chunk/manager.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/chunk/manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/gemini/chunk/search_utils.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/chunk/search_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,18 +42,17 @@
             acc += left
             left = chunk_size
         left -= s
     return left + acc
 
 
 def _tensor_numel(local_param: ColoParameter, strict_ddp_flag: bool):
-    if strict_ddp_flag and type(local_param) is ColoParameter:
+    if strict_ddp_flag:
         return local_param.numel_global()
     else:
-        # if local_param is not ColoParameter, we assume it's replicated
         return local_param.numel()
 
 
 def classify_params_by_dp_degree(param_order: OrderedParamGenerator,
                                  strict_ddp_flag: bool = False) -> Dict[int, List[ColoParameter]]:
     """classify_params_by_dp_degree
 
@@ -64,21 +63,19 @@
 
     Returns:
         Dict[int, List[ColoParameter]]: a dict contains the classification results.
         The keys are dp_degrees and the values are parameters.
     """
     params_dict: Dict[int, List[ColoParameter]] = dict()
     for param in param_order.generate():
-        # assert isinstance(param, ColoParameter), "please init model in the ColoInitContext"
+        assert isinstance(param, ColoParameter), "please init model in the ColoInitContext"
         if is_ddp_ignored(param):
             continue
 
-        if strict_ddp_flag or type(param) is not ColoParameter:
-            # if model is not initialized with ColoInitContext, we assume it's replicated
-            # TODO(ver217): integrate DTensor
+        if strict_ddp_flag:
             param_key = dist.get_world_size()
         else:
             param_key = param.process_group.dp_world_size()
 
         if param_key not in params_dict:
             params_dict[param_key] = []
         params_dict[param_key].append(param)
```

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/gemini/chunk/utils.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/chunk/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/gemini/colo_init_context.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/colo_init_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/gemini/gemini_ddp.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/gemini_ddp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import itertools
 from collections import OrderedDict
 from functools import partial
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Optional
 
 import torch
 import torch.distributed as dist
 import torch.nn as nn
 
 from colossalai.logging import get_dist_logger
 from colossalai.nn.parallel.data_parallel import ColoDDP, _cast_float, free_storage
 from colossalai.tensor import ProcessGroup as ColoProcessGroup
 from colossalai.tensor import ReplicaSpec
 from colossalai.tensor.colo_parameter import ColoParameter, ColoTensor, ColoTensorSpec
 from colossalai.tensor.param_op_hook import ColoParamOpHookManager
 from colossalai.utils import get_current_device, is_ddp_ignored
-from colossalai.utils.model.experimental import LazyTensor
 
 from .chunk import Chunk, ChunkManager, TensorState, init_chunk_manager
 from .gemini_hook import GeminiZeROHook
 from .gemini_mgr import GeminiManager
 from .memory_tracer import MemStats, OrderedParamGenerator
 from .utils import get_temp_total_chunk_on_cuda
 
@@ -52,25 +51,27 @@
 
     def __init__(self,
                  module: torch.nn.Module,
                  gemini_manager: GeminiManager,
                  pin_memory: bool = False,
                  force_outputs_fp32: bool = False,
                  strict_ddp_mode: bool = False) -> None:
+        super().__init__(module, process_group=ColoProcessGroup())
         self.gemini_manager = gemini_manager
         self.chunk_manager: ChunkManager = gemini_manager.chunk_manager
         self.force_outputs_fp32 = force_outputs_fp32
         self.param_op_hook = GeminiZeROHook(gemini_manager)
         self.fp32_params: List[ColoTensor] = list()
         self.fp16_params: List[ColoParameter] = list()
         self.overflow_counter = 0
         self.grads_device: Dict[torch.Tensor, torch.device] = dict()
         self.param2name: Dict[nn.Parameter, str] = dict()
         self.name2param: Dict[str, nn.Parameter] = dict()
 
+        self._cast_buffers()
         self._logger = get_dist_logger()
 
         if self.gemini_manager._premade_memstats_:
             # build chunk in param runtime visited order.
             param_order = self.gemini_manager.memstats()._param_runtime_order
         else:
             # build chunk in param initialized order.
@@ -86,16 +87,14 @@
 
         for name, param in module.named_parameters():
             self.param2name[param] = name
         for m_name, m_var in module.named_modules():
             for p_name, p_var in m_var.named_parameters(recurse=False):
                 param_name = m_name + '.' + p_name if m_name else p_name
                 self.name2param[param_name] = p_var
-        super().__init__(module, process_group=ColoProcessGroup())
-        self._cast_buffers()
 
     def _post_forward(self):
         """This function is only triggered for inference.
         """
         access_list = list(self.chunk_manager.accessed_chunks)
         # we need to scatter all accessed chunks and move them to their original places
         for chunk in access_list:
@@ -475,16 +474,15 @@
                     input_name = key[len(prefix):]
                     if input_name not in local_state:
                         unexpected_keys.append(key)
 
     def _init_chunks(self, param_order, strict_ddp_mode: bool, cpu_offload: bool, pin_memory: bool):
         ddp_pg = ColoProcessGroup()
         for p in param_order.generate():
-            self._preprocess_param(p)
-            assert type(p) is ColoParameter
+            assert isinstance(p, ColoParameter)
 
             # gather sharded parameters in the strict ddp mode
             if strict_ddp_mode:
                 if not p.is_replicate():
                     p.set_dist_spec(ReplicaSpec())
                 p.set_process_group(pg=ddp_pg)
 
@@ -529,35 +527,18 @@
 
             # keep gathered chunks are in CUDA
             if chunk_16.keep_gathered:
                 self.grads_device[p] = get_current_device()
 
     def _cast_buffers(self):
         for buffer in self.module.buffers():
-            if isinstance(buffer, LazyTensor):
-                buffer.materialize()
             buffer.data = buffer.cuda()
             if torch.is_floating_point(buffer):
                 buffer.data = buffer.half()
 
-    def _preprocess_param(self, p: Union[nn.Parameter, ColoParameter, 'LazyTensor']) -> None:
-        """Convert parameter to ColoParameter in-place.
-        Args:
-            p (Union[nn.Parameter, ColoParameter, LazyTensor]): parameter to be converted
-        """
-        if type(p) is ColoParameter:
-            # model is initialized with ColoInitContext
-            return
-        requires_grad = p.requires_grad
-        if isinstance(p, LazyTensor):
-            # model is initialized with LazyInitContext
-            p.materialize()
-        p.__class__ = ColoParameter
-        p.__init__(p, requires_grad=requires_grad)
-
 
 class GeminiDDP(ZeroDDP):
 
     def __init__(self,
                  module: torch.nn.Module,
                  device: torch.device,
                  placement_policy: str = "cpu",
```

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/gemini/gemini_hook.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/gemini_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/gemini/gemini_mgr.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/gemini_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/gemini/gemini_optimizer.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/gemini_optimizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,23 +42,20 @@
         module (ZeroDDP): A ``ZeroDDP`` instance.
         gpu_margin_mem_ratio (float, optional): The ratio of GPU remaining memory (after the first forward-backward)
             which will be used when using hybrid CPU optimizer.
             This argument is meaningless when `placement_policy` of `GeminiManager` is not "auto".
             Defaults to 0.0.
         initial_scale (float, optional): Initial scale used by DynamicGradScaler. Defaults to 2**32.
         min_scale (float, optional): Min scale used by DynamicGradScaler. Defaults to 1.
-        growth_factor (float, optional): Growth_factor used by DynamicGradScaler. Defaults to 2.
-        backoff_factor (float, optional): Backoff_factor used by DynamicGradScaler. Defaults to 0.5.
-        growth_interval (float, optional): Growth_interval used by DynamicGradScaler. Defaults to 1000.
-        hysteresis (float, optional): Hysteresis used by DynamicGradScaler. Defaults to 2.
-        max_scale (int, optional): Max_scale used by DynamicGradScaler. Defaults to 2**32.
-        clipping_norm (float, optional): The norm value used to clip gradient. Defaults to 0.0.
-        norm_type (float, optional): The type of norm used for gradient clipping. Currently, only L2-norm (norm_type=2.0)
-            is supported in ZeroOptimizer. Defaults to 2.0.
-    """
+        growth_factor (float, optional): growth_factor used by DynamicGradScaler. Defaults to 2.
+        backoff_factor (float, optional): backoff_factor used by DynamicGradScaler. Defaults to 0.5.
+        growth_interval (float, optional): growth_interval used by DynamicGradScaler. Defaults to 1000.
+        hysteresis (float, optional): hysteresis used by DynamicGradScaler. Defaults to 2.
+        max_scale (int, optional): max_scale used by DynamicGradScaler. Defaults to 2**32.
+        """
 
     def __init__(self,
                  optim: Optimizer,
                  module: ZeroDDP,
                  gpu_margin_mem_ratio: float = 0.0,
                  initial_scale: float = 2**32,
                  min_scale: float = 1,
```

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/gemini/memory_tracer/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/gemini/memory_tracer/memory_monitor.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/memory_monitor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/gemini/memory_tracer/memory_stats.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/memory_stats.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/gemini/memory_tracer/memstats_collector.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/memstats_collector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/gemini/memory_tracer/param_runtime_order.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/param_runtime_order.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/gemini/memory_tracer/utils.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/memory_tracer/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/gemini/placement_policy.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/placement_policy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/gemini/utils.py` & `colossalai-nightly-2023.4.8/colossalai/zero/gemini/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/legacy/__init__.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/legacy/gemini/gemini_context.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/gemini_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/legacy/gemini/ophooks/utils.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/ophooks/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/legacy/gemini/stateful_tensor.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/stateful_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/legacy/gemini/tensor_placement_policy.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/tensor_placement_policy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/legacy/gemini/tensor_utils.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/gemini/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/legacy/init_ctx/init_context.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/init_ctx/init_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/legacy/shard_utils/base_shard_strategy.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/shard_utils/base_shard_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/legacy/shard_utils/commons.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/shard_utils/commons.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/legacy/sharded_model/_utils.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_model/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/legacy/sharded_model/reduce_scatter.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_model/reduce_scatter.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/legacy/sharded_model/sharded_model_v2.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_model/sharded_model_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/legacy/sharded_model/utils.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_model/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/legacy/sharded_model/zero_hook.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_model/zero_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/legacy/sharded_param/sharded_param.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_param/sharded_param.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/legacy/sharded_param/sharded_tensor.py` & `colossalai-nightly-2023.4.8/colossalai/zero/legacy/sharded_param/sharded_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/low_level/_utils.py` & `colossalai-nightly-2023.4.8/colossalai/zero/low_level/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/low_level/bookkeeping/bucket_store.py` & `colossalai-nightly-2023.4.8/colossalai/zero/low_level/bookkeeping/bucket_store.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/low_level/bookkeeping/gradient_store.py` & `colossalai-nightly-2023.4.8/colossalai/zero/low_level/bookkeeping/gradient_store.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/low_level/bookkeeping/parameter_store.py` & `colossalai-nightly-2023.4.8/colossalai/zero/low_level/bookkeeping/parameter_store.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/low_level/bookkeeping/tensor_bucket.py` & `colossalai-nightly-2023.4.8/colossalai/zero/low_level/bookkeeping/tensor_bucket.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/low_level/low_level_optim.py` & `colossalai-nightly-2023.4.8/colossalai/zero/low_level/low_level_optim.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai/zero/wrapper.py` & `colossalai-nightly-2023.4.8/colossalai/zero/wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/colossalai_nightly.egg-info/PKG-INFO` & `colossalai-nightly-2023.4.8/colossalai_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colossalai-nightly
-Version: 2023.4.15
+Version: 2023.4.8
 Summary: An integrated large-scale model training system with efficient parallelization techniques
 Home-page: https://www.colossalai.org
 License: Apache Software License 2.0
 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/discussions
 Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/issues
 Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io
@@ -46,22 +46,14 @@
         * [2022/09] [HPC-AI Tech Completes $6 Million Seed and Angel Round Fundraising](https://www.hpc-ai.tech/blog/hpc-ai-tech-completes-6-million-seed-and-angel-round-fundraising-led-by-bluerun-ventures-in-the)
         
         ## Table of Contents
         <ul>
          <li><a href="#Why-Colossal-AI">Why Colossal-AI</a> </li>
          <li><a href="#Features">Features</a> </li>
          <li>
-           <a href="#Colossal-AI-in-the-Real-World">Colossal-AI for Real World Applications</a>
-           <ul>
-             <li><a href="#ColossalChat">ColossalChat: An Open-Source Solution for Cloning ChatGPT With a Complete RLHF Pipeline</a></li>
-             <li><a href="#AIGC">AIGC: Acceleration of Stable Diffusion</a></li>
-             <li><a href="#Biomedicine">Biomedicine: Acceleration of AlphaFold Protein Structure</a></li>
-           </ul>
-         </li>
-         <li>
            <a href="#Parallel-Training-Demo">Parallel Training Demo</a>
            <ul>
              <li><a href="#GPT-3">GPT-3</a></li>
              <li><a href="#GPT-2">GPT-2</a></li>
              <li><a href="#BERT">BERT</a></li>
              <li><a href="#PaLM">PaLM</a></li>
              <li><a href="#OPT">OPT</a></li>
@@ -80,14 +72,22 @@
            <a href="#Inference-Energon-AI-Demo">Inference (Energon-AI) Demo</a>
            <ul>
              <li><a href="#GPT-3-Inference">GPT-3</a></li>
              <li><a href="#OPT-Serving">OPT-175B Online Serving for Text Generation</a></li>
              <li><a href="#BLOOM-Inference">176B BLOOM</a></li>
            </ul>
          </li>
+           <li>
+           <a href="#Colossal-AI-in-the-Real-World">Colossal-AI for Real World Applications</a>
+           <ul>
+             <li><a href="#ColossalChat">ColossalChat: An Open-Source Solution for Cloning ChatGPT With a Complete RLHF Pipeline</a></li>
+             <li><a href="#AIGC">AIGC: Acceleration of Stable Diffusion</a></li>
+             <li><a href="#Biomedicine">Biomedicine: Acceleration of AlphaFold Protein Structure</a></li>
+           </ul>
+         </li>
          <li>
            <a href="#Installation">Installation</a>
            <ul>
              <li><a href="#PyPI">PyPI</a></li>
              <li><a href="#Install-From-Source">Install From Source</a></li>
            </ul>
          </li>
@@ -129,96 +129,14 @@
           - Parallelism based on the configuration file
         
         - Inference
           - [Energon-AI](https://github.com/hpcaitech/EnergonAI)
         
         <p align="right">(<a href="#top">back to top</a>)</p>
         
-        ## Colossal-AI in the Real World
-        
-        ### ColossalChat
-        
-        <div align="center">
-           <a href="https://chat.colossalai.org/">
-           <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Chat-demo.png" width="700" />
-           </a>
-        </div>
-        
-        [ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://chat.colossalai.org)
-        
-        <p id="ColossalChat_scaling" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT%20scaling.png" width=800/>
-        </p>
-        
-        - Up to 7.73 times faster for single server training and 1.42 times faster for single-GPU inference
-        
-        <p id="ColossalChat-1GPU" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT-1GPU.jpg" width=450/>
-        </p>
-        
-        - Up to 10.3x growth in model capacity on one GPU
-        - A mini demo training process requires only 1.62GB of GPU memory (any consumer-grade GPU)
-        
-        <p id="ColossalChat-LoRA" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/LoRA%20data.jpg" width=600/>
-        </p>
-        
-        - Increase the capacity of the fine-tuning model by up to 3.7 times on a single GPU
-        - Keep at a sufficiently high running speed
-        
-        <p align="right">(<a href="#top">back to top</a>)</p>
-        
-        
-        ### AIGC
-        Acceleration of AIGC (AI-Generated Content) models such as [Stable Diffusion v1](https://github.com/CompVis/stable-diffusion) and [Stable Diffusion v2](https://github.com/Stability-AI/stablediffusion).
-        <p id="diffusion_train" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Stable%20Diffusion%20v2.png" width=800/>
-        </p>
-        
-        - [Training](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/diffusion): Reduce Stable Diffusion memory consumption by up to 5.6x and hardware cost by up to 46x (from A100 to RTX3060).
-        
-        <p id="diffusion_demo" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/DreamBooth.png" width=800/>
-        </p>
-        
-        - [DreamBooth Fine-tuning](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/dreambooth): Personalize your model using just 3-5 images of the desired subject.
-        
-        <p id="inference" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Stable%20Diffusion%20Inference.jpg" width=800/>
-        </p>
-        
-        - [Inference](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/diffusion): Reduce inference GPU memory consumption by 2.5x.
-        
-        
-        <p align="right">(<a href="#top">back to top</a>)</p>
-        
-        ### Biomedicine
-        Acceleration of [AlphaFold Protein Structure](https://alphafold.ebi.ac.uk/)
-        
-        <p id="FastFold" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/FastFold.jpg" width=800/>
-        </p>
-        
-        - [FastFold](https://github.com/hpcaitech/FastFold): Accelerating training and inference on GPU Clusters, faster data processing, inference sequence containing more than 10000 residues.
-        
-        <p id="FastFold-Intel" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/data%20preprocessing%20with%20Intel.jpg" width=600/>
-        </p>
-        
-        - [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference acceleration and 39% cost reduce.
-        
-        <p id="xTrimoMultimer" align="center">
-        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/xTrimoMultimer_Table.jpg" width=800/>
-        </p>
-        
-        - [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer): accelerating structure prediction of protein monomers and multimer by 11x.
-        
-        
-        <p align="right">(<a href="#top">back to top</a>)</p>
-        
         ## Parallel Training Demo
         
         ### GPT-3
         <p align="center">
         <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/GPT3-v5.png" width=700/>
         </p>
         
@@ -304,22 +222,102 @@
         <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/BLOOM%20Inference.PNG" width=800/>
         </p>
         
         - [BLOOM](https://github.com/hpcaitech/EnergonAI/tree/main/examples/bloom): Reduce hardware deployment costs of 176-billion-parameter BLOOM by more than 10 times.
         
         <p align="right">(<a href="#top">back to top</a>)</p>
         
+        ## Colossal-AI in the Real World
+        
+        ### ColossalChat
+        
+        <div align="center">
+           <a href="https://chat.colossalai.org/">
+           <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Chat-demo.png" width="700" />
+           </a>
+        </div>
+        
+        [ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://chat.colossalai.org)
+        
+        <p id="ColossalChat_scaling" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT%20scaling.png" width=800/>
+        </p>
+        
+        - Up to 7.73 times faster for single server training and 1.42 times faster for single-GPU inference
+        
+        <p id="ColossalChat-1GPU" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/ChatGPT-1GPU.jpg" width=450/>
+        </p>
+        
+        - Up to 10.3x growth in model capacity on one GPU
+        - A mini demo training process requires only 1.62GB of GPU memory (any consumer-grade GPU)
+        
+        <p id="ColossalChat-LoRA" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/chatgpt/LoRA%20data.jpg" width=600/>
+        </p>
+        
+        - Increase the capacity of the fine-tuning model by up to 3.7 times on a single GPU
+        - Keep at a sufficiently high running speed
+        
+        <p align="right">(<a href="#top">back to top</a>)</p>
+        
+        
+        ### AIGC
+        Acceleration of AIGC (AI-Generated Content) models such as [Stable Diffusion v1](https://github.com/CompVis/stable-diffusion) and [Stable Diffusion v2](https://github.com/Stability-AI/stablediffusion).
+        <p id="diffusion_train" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Stable%20Diffusion%20v2.png" width=800/>
+        </p>
+        
+        - [Training](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/diffusion): Reduce Stable Diffusion memory consumption by up to 5.6x and hardware cost by up to 46x (from A100 to RTX3060).
+        
+        <p id="diffusion_demo" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/DreamBooth.png" width=800/>
+        </p>
+        
+        - [DreamBooth Fine-tuning](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/dreambooth): Personalize your model using just 3-5 images of the desired subject.
+        
+        <p id="inference" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/Stable%20Diffusion%20Inference.jpg" width=800/>
+        </p>
+        
+        - [Inference](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/diffusion): Reduce inference GPU memory consumption by 2.5x.
+        
+        
+        <p align="right">(<a href="#top">back to top</a>)</p>
+        
+        ### Biomedicine
+        Acceleration of [AlphaFold Protein Structure](https://alphafold.ebi.ac.uk/)
+        
+        <p id="FastFold" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/FastFold.jpg" width=800/>
+        </p>
+        
+        - [FastFold](https://github.com/hpcaitech/FastFold): Accelerating training and inference on GPU Clusters, faster data processing, inference sequence containing more than 10000 residues.
+        
+        <p id="FastFold-Intel" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/data%20preprocessing%20with%20Intel.jpg" width=600/>
+        </p>
+        
+        - [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference acceleration and 39% cost reduce.
+        
+        <p id="xTrimoMultimer" align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/xTrimoMultimer_Table.jpg" width=800/>
+        </p>
+        
+        - [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer): accelerating structure prediction of protein monomers and multimer by 11x.
+        
+        
+        <p align="right">(<a href="#top">back to top</a>)</p>
+        
         ## Installation
         
         Requirements:
         - PyTorch >= 1.11 (PyTorch 2.x in progress)
         - Python >= 3.7
         - CUDA >= 11.0
-        - [NVIDIA GPU Compute Capability](https://developer.nvidia.com/cuda-gpus) >= 7.0 (V100/RTX20 and higher)
-        - Linux OS
         
         If you encounter any problem with installation, you may want to raise an [issue](https://github.com/hpcaitech/ColossalAI/issues/new/choose) in this repository.
         
         ### Install from PyPI
         
         You can easily install Colossal-AI with the following command. **By default, we do not build PyTorch extensions during installation.**
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.4.15 Summary: An
+Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.4.8 Summary: An
 integrated large-scale model training system with efficient parallelization
 techniques Home-page: https://www.colossalai.org License: Apache Software
 License 2.0 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/
 discussions Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/
 issues Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io Project-URL:
 Github, https://github.com/hpcaitech/ColossalAI Description: # Colossal-AI
@@ -45,19 +45,14 @@
 Sequence Exceeding 10,000](https://www.hpc-ai.tech/blog/use-a-laptop-to-
 analyze-90-of-proteins-with-a-single-gpu-inference-sequence-exceeding) * [2022/
 09] [HPC-AI Tech Completes $6 Million Seed and Angel Round Fundraising](https:/
 /www.hpc-ai.tech/blog/hpc-ai-tech-completes-6-million-seed-and-angel-round-
 fundraising-led-by-bluerun-ventures-in-the) ## Table of Contents
     * Why_Colossal-AI
     * Features
-    * Colossal-AI_for_Real_World_Applications
-          o ColossalChat:_An_Open-Source_Solution_for_Cloning_ChatGPT_With_a
-            Complete_RLHF_Pipeline
-          o AIGC:_Acceleration_of_Stable_Diffusion
-          o Biomedicine:_Acceleration_of_AlphaFold_Protein_Structure
     * Parallel_Training_Demo
           o GPT-3
           o GPT-2
           o BERT
           o PaLM
           o OPT
           o ViT
@@ -65,14 +60,19 @@
     * Single_GPU_Training_Demo
           o GPT-2
           o PaLM
     * Inference_(Energon-AI)_Demo
           o GPT-3
           o OPT-175B_Online_Serving_for_Text_Generation
           o 176B_BLOOM
+    * Colossal-AI_for_Real_World_Applications
+          o ColossalChat:_An_Open-Source_Solution_for_Cloning_ChatGPT_With_a
+            Complete_RLHF_Pipeline
+          o AIGC:_Acceleration_of_Stable_Diffusion
+          o Biomedicine:_Acceleration_of_AlphaFold_Protein_Structure
     * Installation
           o PyPI
           o Install_From_Source
     * Use_Docker
     * Community
     * Contributing
     * Cite_Us
@@ -91,71 +91,14 @@
 (https://arxiv.org/abs/2105.13120) - [Zero Redundancy Optimizer (ZeRO)](https:/
 /arxiv.org/abs/1910.02054) - [Auto-Parallelism](https://arxiv.org/abs/
 2302.02599) - Heterogeneous Memory Management - [PatrickStar](https://
 arxiv.org/abs/2108.05818) - Friendly Usage - Parallelism based on the
 configuration file - Inference - [Energon-AI](https://github.com/hpcaitech/
 EnergonAI)
                                                                   (back_to_top)
-## Colossal-AI in the Real World ### ColossalChat
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                                Chat-demo.png]
-[ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/
-Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/
-chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/
-ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/
-@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-
-with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://
-chat.colossalai.org)
- [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
-                        chatgpt/ChatGPT%20scaling.png]
-- Up to 7.73 times faster for single server training and 1.42 times faster for
-single-GPU inference
- [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
-                           chatgpt/ChatGPT-1GPU.jpg]
-- Up to 10.3x growth in model capacity on one GPU - A mini demo training
-process requires only 1.62GB of GPU memory (any consumer-grade GPU)
- [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
-                           chatgpt/LoRA%20data.jpg]
-- Increase the capacity of the fine-tuning model by up to 3.7 times on a single
-GPU - Keep at a sufficiently high running speed
-                                                                  (back_to_top)
-### AIGC Acceleration of AIGC (AI-Generated Content) models such as [Stable
-Diffusion v1](https://github.com/CompVis/stable-diffusion) and [Stable
-Diffusion v2](https://github.com/Stability-AI/stablediffusion).
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                         Stable%20Diffusion%20v2.png]
-- [Training](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/
-diffusion): Reduce Stable Diffusion memory consumption by up to 5.6x and
-hardware cost by up to 46x (from A100 to RTX3060).
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                                DreamBooth.png]
-- [DreamBooth Fine-tuning](https://github.com/hpcaitech/ColossalAI/tree/main/
-examples/images/dreambooth): Personalize your model using just 3-5 images of
-the desired subject.
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                      Stable%20Diffusion%20Inference.jpg]
-- [Inference](https://github.com/hpcaitech/ColossalAI/tree/main/examples/
-images/diffusion): Reduce inference GPU memory consumption by 2.5x.
-                                                                  (back_to_top)
-### Biomedicine Acceleration of [AlphaFold Protein Structure](https://
-alphafold.ebi.ac.uk/)
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                                 FastFold.jpg]
-- [FastFold](https://github.com/hpcaitech/FastFold): Accelerating training and
-inference on GPU Clusters, faster data processing, inference sequence
-containing more than 10000 residues.
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                   data%20preprocessing%20with%20Intel.jpg]
-- [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference
-acceleration and 39% cost reduce.
-[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
-                           xTrimoMultimer_Table.jpg]
-- [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer):
-accelerating structure prediction of protein monomers and multimer by 11x.
-                                                                  (back_to_top)
 ## Parallel Training Demo ### GPT-3
 [https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
                                  GPT3-v5.png]
 - Save 50% GPU resources and 10.7% acceleration ### GPT-2 [https://
 raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/GPT2.png]
 - 11x lower GPU memory consumption, and superlinear scaling efficiency with
 Tensor Parallelism [https://raw.githubusercontent.com/hpcaitech/public_assets/
@@ -205,35 +148,91 @@
 Try 175-billion-parameter OPT online services
 [https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
                             BLOOM%20Inference.PNG]
 - [BLOOM](https://github.com/hpcaitech/EnergonAI/tree/main/examples/bloom):
 Reduce hardware deployment costs of 176-billion-parameter BLOOM by more than 10
 times.
                                                                   (back_to_top)
+## Colossal-AI in the Real World ### ColossalChat
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                                Chat-demo.png]
+[ColossalChat](https://github.com/hpcaitech/ColossalAI/tree/main/applications/
+Chat): An open-source solution for cloning [ChatGPT](https://openai.com/blog/
+chatgpt/) with a complete RLHF pipeline. [[code]](https://github.com/hpcaitech/
+ColossalAI/tree/main/applications/Chat) [[blog]](https://medium.com/
+@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-
+with-a-complete-rlhf-pipeline-5edf08fb538b) [[demo]](https://
+chat.colossalai.org)
+ [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
+                        chatgpt/ChatGPT%20scaling.png]
+- Up to 7.73 times faster for single server training and 1.42 times faster for
+single-GPU inference
+ [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
+                           chatgpt/ChatGPT-1GPU.jpg]
+- Up to 10.3x growth in model capacity on one GPU - A mini demo training
+process requires only 1.62GB of GPU memory (any consumer-grade GPU)
+ [https://raw.githubusercontent.com/hpcaitech/public_assets/main/applications/
+                           chatgpt/LoRA%20data.jpg]
+- Increase the capacity of the fine-tuning model by up to 3.7 times on a single
+GPU - Keep at a sufficiently high running speed
+                                                                  (back_to_top)
+### AIGC Acceleration of AIGC (AI-Generated Content) models such as [Stable
+Diffusion v1](https://github.com/CompVis/stable-diffusion) and [Stable
+Diffusion v2](https://github.com/Stability-AI/stablediffusion).
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                         Stable%20Diffusion%20v2.png]
+- [Training](https://github.com/hpcaitech/ColossalAI/tree/main/examples/images/
+diffusion): Reduce Stable Diffusion memory consumption by up to 5.6x and
+hardware cost by up to 46x (from A100 to RTX3060).
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                                DreamBooth.png]
+- [DreamBooth Fine-tuning](https://github.com/hpcaitech/ColossalAI/tree/main/
+examples/images/dreambooth): Personalize your model using just 3-5 images of
+the desired subject.
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                      Stable%20Diffusion%20Inference.jpg]
+- [Inference](https://github.com/hpcaitech/ColossalAI/tree/main/examples/
+images/diffusion): Reduce inference GPU memory consumption by 2.5x.
+                                                                  (back_to_top)
+### Biomedicine Acceleration of [AlphaFold Protein Structure](https://
+alphafold.ebi.ac.uk/)
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                                 FastFold.jpg]
+- [FastFold](https://github.com/hpcaitech/FastFold): Accelerating training and
+inference on GPU Clusters, faster data processing, inference sequence
+containing more than 10000 residues.
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                   data%20preprocessing%20with%20Intel.jpg]
+- [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference
+acceleration and 39% cost reduce.
+[https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
+                           xTrimoMultimer_Table.jpg]
+- [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer):
+accelerating structure prediction of protein monomers and multimer by 11x.
+                                                                  (back_to_top)
 ## Installation Requirements: - PyTorch >= 1.11 (PyTorch 2.x in progress) -
-Python >= 3.7 - CUDA >= 11.0 - [NVIDIA GPU Compute Capability](https://
-developer.nvidia.com/cuda-gpus) >= 7.0 (V100/RTX20 and higher) - Linux OS If
-you encounter any problem with installation, you may want to raise an [issue]
-(https://github.com/hpcaitech/ColossalAI/issues/new/choose) in this repository.
-### Install from PyPI You can easily install Colossal-AI with the following
-command. **By default, we do not build PyTorch extensions during
-installation.** ```bash pip install colossalai ``` **Note: only Linux is
-supported for now.** However, if you want to build the PyTorch extensions
-during installation, you can set `CUDA_EXT=1`. ```bash CUDA_EXT=1 pip install
-colossalai ``` **Otherwise, CUDA kernels will be built during runtime when you
-actually need them.** We also keep releasing the nightly version to PyPI every
-week. This allows you to access the unreleased features and bug fixes in the
-main branch. Installation can be made via ```bash pip install colossalai-
-nightly ``` ### Download From Source > The version of Colossal-AI will be in
-line with the main branch of the repository. Feel free to raise an issue if you
-encounter any problems. :) ```shell git clone https://github.com/hpcaitech/
-ColossalAI.git cd ColossalAI # install colossalai pip install . ``` By default,
-we do not compile CUDA/C++ kernels. ColossalAI will build them during runtime.
-If you want to install and enable CUDA kernel fusion (compulsory installation
-when using fused optimizer): ```shell CUDA_EXT=1 pip install . ```
+Python >= 3.7 - CUDA >= 11.0 If you encounter any problem with installation,
+you may want to raise an [issue](https://github.com/hpcaitech/ColossalAI/
+issues/new/choose) in this repository. ### Install from PyPI You can easily
+install Colossal-AI with the following command. **By default, we do not build
+PyTorch extensions during installation.** ```bash pip install colossalai ```
+**Note: only Linux is supported for now.** However, if you want to build the
+PyTorch extensions during installation, you can set `CUDA_EXT=1`. ```bash
+CUDA_EXT=1 pip install colossalai ``` **Otherwise, CUDA kernels will be built
+during runtime when you actually need them.** We also keep releasing the
+nightly version to PyPI every week. This allows you to access the unreleased
+features and bug fixes in the main branch. Installation can be made via ```bash
+pip install colossalai-nightly ``` ### Download From Source > The version of
+Colossal-AI will be in line with the main branch of the repository. Feel free
+to raise an issue if you encounter any problems. :) ```shell git clone https://
+github.com/hpcaitech/ColossalAI.git cd ColossalAI # install colossalai pip
+install . ``` By default, we do not compile CUDA/C++ kernels. ColossalAI will
+build them during runtime. If you want to install and enable CUDA kernel fusion
+(compulsory installation when using fused optimizer): ```shell CUDA_EXT=1 pip
+install . ```
                                                                   (back_to_top)
 ## Use Docker ### Pull from DockerHub You can directly pull the docker image
 from our [DockerHub page](https://hub.docker.com/r/hpcaitech/colossalai). The
 image is automatically uploaded upon release. ### Build On Your Own Run the
 following command to build a docker image from Dockerfile provided. > Building
 Colossal-AI from scratch requires GPU support, you need to use Nvidia Docker
 Runtime as the default when doing `docker build`. More details can be found
```

### Comparing `colossalai-nightly-2023.4.15/colossalai_nightly.egg-info/SOURCES.txt` & `colossalai-nightly-2023.4.8/colossalai_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/op_builder/__init__.py` & `colossalai-nightly-2023.4.8/op_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/op_builder/builder.py` & `colossalai-nightly-2023.4.8/op_builder/builder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/op_builder/cpu_adam.py` & `colossalai-nightly-2023.4.8/op_builder/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/op_builder/fused_optim.py` & `colossalai-nightly-2023.4.8/op_builder/fused_optim.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/op_builder/layernorm.py` & `colossalai-nightly-2023.4.8/op_builder/layernorm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/op_builder/moe.py` & `colossalai-nightly-2023.4.8/op_builder/moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/op_builder/multi_head_attn.py` & `colossalai-nightly-2023.4.8/op_builder/multi_head_attn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/op_builder/scaled_masked_softmax.py` & `colossalai-nightly-2023.4.8/op_builder/scaled_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/op_builder/scaled_upper_triangle_masked_softmax.py` & `colossalai-nightly-2023.4.8/op_builder/scaled_upper_triangle_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/op_builder/utils.py` & `colossalai-nightly-2023.4.8/op_builder/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/setup.py` & `colossalai-nightly-2023.4.8/setup.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/components_to_test/albert.py` & `colossalai-nightly-2023.4.8/tests/components_to_test/albert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/components_to_test/beit.py` & `colossalai-nightly-2023.4.8/tests/components_to_test/beit.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/components_to_test/bert.py` & `colossalai-nightly-2023.4.8/tests/components_to_test/bert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/components_to_test/gpt2.py` & `colossalai-nightly-2023.4.8/tests/components_to_test/gpt2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/components_to_test/hanging_param_model.py` & `colossalai-nightly-2023.4.8/tests/components_to_test/hanging_param_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/components_to_test/inline_op_model.py` & `colossalai-nightly-2023.4.8/tests/components_to_test/inline_op_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/components_to_test/nested_model.py` & `colossalai-nightly-2023.4.8/tests/components_to_test/nested_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/components_to_test/registry.py` & `colossalai-nightly-2023.4.8/tests/components_to_test/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/components_to_test/repeated_computed_layers.py` & `colossalai-nightly-2023.4.8/tests/components_to_test/repeated_computed_layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/components_to_test/resnet.py` & `colossalai-nightly-2023.4.8/tests/components_to_test/resnet.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/components_to_test/simple_net.py` & `colossalai-nightly-2023.4.8/tests/components_to_test/simple_net.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/components_to_test/utils/executor.py` & `colossalai-nightly-2023.4.8/tests/components_to_test/utils/executor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/kit/model_zoo/diffusers/diffusers.py` & `colossalai-nightly-2023.4.8/tests/kit/model_zoo/diffusers/diffusers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/kit/model_zoo/registry.py` & `colossalai-nightly-2023.4.8/tests/kit/model_zoo/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/kit/model_zoo/timm/timm.py` & `colossalai-nightly-2023.4.8/tests/kit/model_zoo/timm/timm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/kit/model_zoo/torchaudio/torchaudio.py` & `colossalai-nightly-2023.4.8/tests/kit/model_zoo/torchaudio/torchaudio.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/kit/model_zoo/torchrec/torchrec.py` & `colossalai-nightly-2023.4.8/tests/kit/model_zoo/torchrec/torchrec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/kit/model_zoo/torchvision/torchvision.py` & `colossalai-nightly-2023.4.8/tests/kit/model_zoo/torchvision/torchvision.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/kit/model_zoo/transformers/albert.py` & `colossalai-nightly-2023.4.8/tests/kit/model_zoo/transformers/albert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/kit/model_zoo/transformers/bert.py` & `colossalai-nightly-2023.4.8/tests/kit/model_zoo/transformers/bert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/kit/model_zoo/transformers/gpt.py` & `colossalai-nightly-2023.4.8/tests/kit/model_zoo/transformers/gpt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/kit/model_zoo/transformers/opt.py` & `colossalai-nightly-2023.4.8/tests/kit/model_zoo/transformers/opt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/kit/model_zoo/transformers/t5.py` & `colossalai-nightly-2023.4.8/tests/kit/model_zoo/transformers/t5.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_analyzer/test_fx/test_bias_addition.py` & `colossalai-nightly-2023.4.8/tests/test_analyzer/test_fx/test_bias_addition.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_analyzer/test_fx/test_mod_dir.py` & `colossalai-nightly-2023.4.8/tests/test_analyzer/test_fx/test_mod_dir.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_analyzer/test_fx/test_nested_ckpt.py` & `colossalai-nightly-2023.4.8/tests/test_analyzer/test_fx/test_nested_ckpt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_analyzer/test_fx/test_shape_prop.py` & `colossalai-nightly-2023.4.8/tests/test_analyzer/test_fx/test_shape_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_analyzer/test_fx/test_symbolic_profile.py` & `colossalai-nightly-2023.4.8/tests/test_analyzer/test_fx/test_symbolic_profile.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_analyzer/test_fx/zoo.py` & `colossalai-nightly-2023.4.8/tests/test_analyzer/test_fx/zoo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_analyzer/test_subclasses/test_aten.py` & `colossalai-nightly-2023.4.8/tests/test_analyzer/test_subclasses/test_aten.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_analyzer/test_subclasses/test_flop_tensor.py` & `colossalai-nightly-2023.4.8/tests/test_analyzer/test_subclasses/test_flop_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_analyzer/test_subclasses/test_meta_mode.py` & `colossalai-nightly-2023.4.8/tests/test_analyzer/test_subclasses/test_meta_mode.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_pass/test_node_converting_pass.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_pass/test_node_converting_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.4.15/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py` & `colossalai-nightly-2023.4.8/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py`

 * *Files identical despite different names*

