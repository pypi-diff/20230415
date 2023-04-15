# Comparing `tmp/ddpw-3.0.0.tar.gz` & `tmp/ddpw-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddpw-3.0.0.tar", last modified: Tue Nov 29 14:18:24 2022, max compression
+gzip compressed data, was "ddpw-4.0.0.tar", last modified: Sat Apr 15 18:52:06 2023, max compression
```

## Comparing `ddpw-3.0.0.tar` & `ddpw-4.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 14:18:24.950298 ddpw-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2022-11-29 14:18:14.000000 ddpw-3.0.0/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2022-11-29 14:18:24.950298 ddpw-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2022-11-29 14:18:14.000000 ddpw-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 14:18:24.946298 ddpw-3.0.0/ddpw/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-11-29 14:18:14.000000 ddpw-3.0.0/ddpw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2022-11-29 14:18:14.000000 ddpw-3.0.0/ddpw/artefacts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 14:18:24.950298 ddpw-3.0.0/ddpw/gpu_setup/
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2022-11-29 14:18:14.000000 ddpw-3.0.0/ddpw/gpu_setup/__dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2022-11-29 14:18:14.000000 ddpw-3.0.0/ddpw/gpu_setup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2022-11-29 14:18:14.000000 ddpw-3.0.0/ddpw/gpu_setup/__model.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2022-11-29 14:18:14.000000 ddpw-3.0.0/ddpw/gpu_setup/__seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     8341 2022-11-29 14:18:14.000000 ddpw-3.0.0/ddpw/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2022-11-29 14:18:14.000000 ddpw-3.0.0/ddpw/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2022-11-29 14:18:14.000000 ddpw-3.0.0/ddpw/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2022-11-29 14:18:14.000000 ddpw-3.0.0/ddpw/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 14:18:24.946298 ddpw-3.0.0/ddpw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2022-11-29 14:18:24.000000 ddpw-3.0.0/ddpw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      368 2022-11-29 14:18:24.000000 ddpw-3.0.0/ddpw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-29 14:18:24.000000 ddpw-3.0.0/ddpw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2022-11-29 14:18:24.000000 ddpw-3.0.0/ddpw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2022-11-29 14:18:24.000000 ddpw-3.0.0/ddpw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-11-29 14:18:24.950298 ddpw-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      811 2022-11-29 14:18:14.000000 ddpw-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:52:06.955824 ddpw-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-15 18:51:52.000000 ddpw-4.0.0/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-15 18:52:06.955824 ddpw-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-15 18:51:52.000000 ddpw-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:52:06.955824 ddpw-4.0.0/ddpw/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 18:51:52.000000 ddpw-4.0.0/ddpw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-15 18:51:52.000000 ddpw-4.0.0/ddpw/artefacts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:52:06.955824 ddpw-4.0.0/ddpw/gpu_setup/
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-15 18:51:52.000000 ddpw-4.0.0/ddpw/gpu_setup/__dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-15 18:51:52.000000 ddpw-4.0.0/ddpw/gpu_setup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-15 18:51:52.000000 ddpw-4.0.0/ddpw/gpu_setup/__model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-15 18:51:52.000000 ddpw-4.0.0/ddpw/gpu_setup/__seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-15 18:51:52.000000 ddpw-4.0.0/ddpw/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-04-15 18:51:52.000000 ddpw-4.0.0/ddpw/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-04-15 18:51:52.000000 ddpw-4.0.0/ddpw/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-04-15 18:51:52.000000 ddpw-4.0.0/ddpw/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:52:06.955824 ddpw-4.0.0/ddpw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-15 18:52:06.000000 ddpw-4.0.0/ddpw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-15 18:52:06.000000 ddpw-4.0.0/ddpw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 18:52:06.000000 ddpw-4.0.0/ddpw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-15 18:52:06.000000 ddpw-4.0.0/ddpw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-15 18:52:06.000000 ddpw-4.0.0/ddpw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 18:52:06.955824 ddpw-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-15 18:51:52.000000 ddpw-4.0.0/setup.py
```

### Comparing `ddpw-3.0.0/LICENCE.md` & `ddpw-4.0.0/LICENCE.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause Licence
 
-Copyright (c) 2022, Sujal Vijayaraghavan All rights reserved.
+Copyright (c) 2023, Sujal Vijayaraghavan All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
 Redistributions of source code must retain the above copyright notice, this list
 of conditions and the following disclaimer.
```

### Comparing `ddpw-3.0.0/PKG-INFO` & `ddpw-4.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddpw
-Version: 3.0.0
+Version: 4.0.0
 Summary: A utility package to scaffold PyTorch's DDP
 Home-page: https://ddpw.projects.sujal.tv
 Author: Sujal T.V.
 License: UNKNOWN
 Description: # DDPW
         
         [![AWS S3](https://img.shields.io/badge/documentation-sphinx-blue?link=https://ddpw.projects.sujal.tv)](https://ddpw.projects.sujal.tv)
@@ -13,15 +13,15 @@
         
         [![Publish documentation to AWS S3](https://github.com/sujaltv/ddpw/actions/workflows/s3_publish.yaml/badge.svg)](https://github.com/sujaltv/ddpw/actions/workflows/s3_publish.yaml)
         [![Publish to Anaconda](https://github.com/sujaltv/ddpw/actions/workflows/conda_publish.yaml/badge.svg)](https://github.com/sujaltv/ddpw/actions/workflows/conda_publish.yaml)
         [![Publish to PyPI](https://github.com/sujaltv/ddpw/actions/workflows/pypi_publish.yaml/badge.svg)](https://github.com/sujaltv/ddpw/actions/workflows/pypi_publish.yaml)
         
         ---
         
-        The Distributed Data Parallel wrapper (DDPW) is created as a utility package to
+        **Distributed Data Parallel Wrapper (DDPW)** is created as a utility package to
         encapsulate the scaffolding for PyTorch's Distributed Data Parallel.
         
         This code is written in Python. The [DDPW
         documentation](https://ddpw.projects.sujal.tv) contains details on how to use
         this package.
         
         ## Overview
@@ -32,32 +32,37 @@
         conda install -c tvsujal ddpw # with conda
         pip install ddpw # with pip from PyPI
         ```
         
         ### Usage
         
         ```python
-          from ddpw.platform import PlatformConfig
-          from ddpw.artefacts import ArtefactsConfig
-          from ddpw.job import JobConfig
-          from ddpw.wrapper import Wrapper
+        from ddpw.platform import Platform, PlatformConfig
+        from ddpw.artefacts import ArtefactsConfig
+        from ddpw.job import JobConfig, JobMode
+        from ddpw.wrapper import Wrapper
+        
+        from src import MyDataset, MyModel, MyOptimiser, MyTrainer
+        
+        # datasets
+        train_set = MyDataset(train=True)
+        test_set = MyDataset(train=False)
+        
+        # configure the platform
+        p_config = PlatformConfig(platform=Platform.GPU, n_gpus=4, cpus_per_task=2)
+        
+        # configure the artefacts (model, dataset, optimiser, etc.)
+        a_config = ArtefactsConfig(train_set=train_set, test_set=test_set,
+            batch_size=64, model=MyModel(), optimiser_loader=MyOptimiser(lr=0.1))
         
-          from src import MyTrainer
-        
-          p = PlatformConfig(...)
-          a = ArtefactsConfig(...)
-          t = JobConfig(...)
-        
-          d = Wrapper(p, a)
-          j = MyTrainer(t)
-        
-          d.start(j)
+        # call the job
+        Wrapper(p_config, a_config).start(MyTrainer())
         ```
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ddpw-3.0.0/ddpw/gpu_setup/__dataset.py` & `ddpw-4.0.0/ddpw/gpu_setup/__dataset.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,37 @@
-from typing import Optional, Callable
+from typing import Optional, Dict
 
 from torch.utils import data
-from torch.utils.data import DistributedSampler, DataLoader, random_split
+from torch.utils.data import DistributedSampler, DataLoader
 
 from ..utils import Utils
 from ..artefacts import ArtefactsConfig
 from ..platform import Platform, PlatformConfig
 
 
 def sampler(dataset: data.Dataset, world_size: int, global_rank: int,
-            batch_size: int, collate_fn: Optional[Callable] = None,
-            is_cpu: bool = False):
+            is_cpu: bool = False, data_loader_args: Optional[Dict] = {}):
   r"""
   This function selects a portion of the original dataset shared by other
   devices. If the device being trained on is a CPU, no sharing is necessary.
 
   :param data.Dataset dataset: The dataset from which to sample for the current
     device.
   :param int world_size: World size.
   :param int global_rank: Global rank of the current GPU.
-  :param int batch_size: Batch size.
-  :param Optional[Callable] collate_fn: The collate function to use in the
-    dataloader.
   :param bool is_cpu: Specifies if the device is a CPU or Apple M1. Default:
     `False`.
 
   :returns data.Dataset: A dataloader with portion of the dataset selected for
       the current process.
   """
 
   smplr = None if is_cpu else DistributedSampler(dataset, world_size,
                                                  rank=global_rank)
-  return DataLoader(dataset, batch_size, sampler=smplr, pin_memory=True,
-                    collate_fn=collate_fn)
+  return DataLoader(dataset, sampler=smplr, pin_memory=True, **data_loader_args)
 
 
 def dataset_setup(global_rank: int, p_config: PlatformConfig,
                   a_config: ArtefactsConfig):
   r"""
   This function selects a portion of the training dataset for validation if
   specified. In case of training/testing on multiple devices, it then allocates
@@ -48,38 +43,33 @@
   :param ArtefactsConfig a_config: Job configurations.
 
   :returns tuple: A triplet of dataloaders for the training, validation, and
       test datasets respectively.
   """
 
   train_loader = None
-  val_loader = None
+  validation_loader = None
   test_loader = None
 
-  val_set = a_config.validation_set
-
   is_cpu = p_config.platform in [Platform.CPU, Platform.MPS]
-  batch_size, collate_fn = a_config.batch_size, a_config.collate_fn
 
-  args = (p_config.world_size, global_rank, batch_size, collate_fn, is_cpu)
+  args = (p_config.world_size, global_rank, is_cpu, a_config.dataloader_args)
 
-  # if the training dataset is provided
+  # if a train split is available
   if (train_set := a_config.train_set) is not None:
-
-    # if requested to set aside a portion of the training set for validation
-    if a_config.needs_validation:
-      dataset_size = len(train_set)
-      v_size = (dataset_size * a_config.validation_percentage) // 100
-      t_size = dataset_size - v_size
-      Utils.print(f'\tTrain size = {t_size}; validation size = {v_size}.')
-      [train_set, val_set] = random_split(train_set, [t_size, v_size])
-    if val_set is not None:
-      val_loader = sampler(val_set, *args)
-
     train_loader = sampler(train_set, *args)
+    Utils.print(f'[Device {global_rank}] ' +
+                f'Received test set portion: {len(train_loader)}')
+
+  # if a validation split is available
+  if (validation_set := a_config.validation_set) is not None:
+    validation_loader = sampler(validation_set, *args)
+    Utils.print(f'[Device {global_rank}] ' +
+                f'Received test set portion: {len(validation_loader)}')
 
-  # if the test dataset is provided
+  # if a test split is available
   if (test_set := a_config.test_set) is not None:
-    Utils.print(f'\tTest size  {len(test_set)}.')
     test_loader = sampler(test_set, *args)
+    Utils.print(f'[Device {global_rank}] ' +
+                f'Received test set portion: {len(test_loader)}')
 
-  return train_loader, val_loader, test_loader
+  return train_loader, validation_loader, test_loader
```

### Comparing `ddpw-3.0.0/ddpw/gpu_setup/__init__.py` & `ddpw-4.0.0/ddpw/gpu_setup/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,17 +62,17 @@
   elif p_config.platform == Platform.MPS:
     a_config.model.to(torch.device('mps'))
 
   # 3. Wait for all processes to synchronise and then start the task
   Utils.print(f'[Device {global_rank}] Training model on device {local_rank}.')
   if p_config.requires_ipc:
     dist.barrier()
-  run.p_config = p_config
   run.a_config = a_config
+  run.p_config = p_config
 
   Utils.print(f'[Device {global_rank}] All setup finished.')
   run(global_rank, local_rank)
 
   if p_config.requires_ipc:
     dist.destroy_process_group()
 
-  Utils.print('Tasks on device complete.')
+  Utils.print(f'[Device {global_rank}] Tasks on device complete.')
```

### Comparing `ddpw-3.0.0/ddpw/gpu_setup/__model.py` & `ddpw-4.0.0/ddpw/gpu_setup/__model.py`

 * *Files identical despite different names*

### Comparing `ddpw-3.0.0/ddpw/platform.py` & `ddpw-4.0.0/ddpw/platform.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import final
+from typing import final, Optional, Callable
 from dataclasses import dataclass
 
 import torch.distributed as dist
 from .utils import Utils
 
 
 @final
@@ -18,14 +18,32 @@
 
   SLURM = 2
   r"""The platform to run on is a SLURM-based cluster of GPU nodes."""
 
   MPS = 3
   r"""The platform to run on is Mac's Apple M1 SoCs."""
 
+  @staticmethod
+  def from_num(num: int) -> 'Platform':
+    r"""
+    Given a device number, this method returns the corresponding platform.
+
+    :param int num: The platform number.
+    :returns Platform: The platform corresponding to the provided argument.
+    :raises ArgumentError: Raises argument error if the number if invalid.
+    """
+
+    match num:
+      case 0: return Platform.CPU
+      case 1: return Platform.GPU
+      case 2: return Platform.SLURM
+      case 3: return Platform.MPS
+      case _: raise ArgumentError("Undefined platform number given")
+
+
 @final
 @dataclass
 class PlatformConfig(object):
   r"""
   Platform-related configurations such as the environment, communication IP
   address and port, world size, `etc.`
   """
@@ -72,14 +90,17 @@
   timeout_min: int = 2880
   r"""Minimum timeout (in minutes) for SLURM-based jobs. Used only on SLURM
   platforms. Default: ``2880`` (two days)."""
 
   cpus_per_task: int = 1
   r"""Number of CPUs per task. Default: ``1``."""
 
+  upon_finish: Optional[Callable] = None
+  r"""Any cleanup tasks to be done upon completion. Default: ``None``."""
+
   @property
   def world_size(self):
     r"""World size. This is the total number of GPUs across nodes. For SLURM,
     this is implicitly the number of GPUs allotted on each node multiplied by
     the total number of nodes. Default: ``1``."""
 
     return self.n_nodes * self.n_gpus
```

### Comparing `ddpw-3.0.0/ddpw/utils.py` & `ddpw-4.0.0/ddpw/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,48 +20,40 @@
     if 'flush' not in kwargs:
       kwargs['flush'] = True
 
     if kwargs.get('verbose', Utils.verbose):
       if 'verbose' in kwargs: del(kwargs['verbose'])
       print(*args, **kwargs)
 
-
   @staticmethod
-  def all_average_gradients(model: torch.nn.Module):
+  def average_params_grads(model: torch.nn.Module, params: bool = False,
+                           grads: bool = True):
     r"""
-    Given a model, this method averages the gradients of the model across all
-    the GPUs in the world. Copied and modified from `PyTorch Blog
-    <https://pytorch.org/tutorials/intermediate/dist_tuto.html>`_.
-
-    :param nn.Module model: The model whose gradients are to be averaged.
+    Given a model, this method averages the parameters and/or their gradients of
+    the model across all the GPUs in the world. Copied and modified from
+    `PyTorch Blog <https://pytorch.org/tutorials/intermediate/dist_tuto.html>`_.
+
+    :param nn.Module model: The model whose parameters/gradients are to be
+        averaged.
+    :param bool params: Whether to average the parameters or not. Default:
+        `False`
+    :param bool grads: Whether to average the gradients or not. Default: `True`
     """
 
-    world_size = float(dist.get_world_size())
-
-    for params in model.parameters():
-      if params.grad is None: continue
-      dist.all_reduce(params.grad, op=dist.ReduceOp.SUM)
-      params.grad /= world_size
-
-
-  @staticmethod
-  def all_params_gradients(model: torch.nn.Module):
-    r"""
-    Given a model, this method averages the parameters of the model across all
-    the GPUs in the world.
-
-    :param nn.Module model: The model whose parameters are to be averaged.
-    """
+    if not (params and grads): return
 
     world_size = float(dist.get_world_size())
 
-    for params in model.parameters():
-      if params is None: continue
-      dist.all_reduce(params, op=dist.ReduceOp.SUM)
-      params /= world_size
+    for p in model.parameters():
+      if p.grad is not None and grads:
+        dist.all_reduce(p.grad, op=dist.ReduceOp.SUM)
+        p.grad /= world_size
+      if p is not None and params:
+        dist.all_reduce(p, op=dist.ReduceOp.SUM)
+        p /= world_size
 
   @staticmethod
   def optimiser_to(optimiser: torch.optim.Optimizer, device: torch.device):
     r"""
     This function offers a simple way to move all parameters of an optimiser or,
     effectively the optimiser itself, to the specified device. This method has
     been taken as is from a `solution
```

### Comparing `ddpw-3.0.0/ddpw/wrapper.py` & `ddpw-4.0.0/ddpw/wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 
 import torch.multiprocessing as mp
-from submitit import AutoExecutor, JobEnvironment
 
 from .utils import Utils
 from .job import Job
 from .gpu_setup import init_process
 from .artefacts import ArtefactsConfig
 from .platform import Platform, PlatformConfig
 
@@ -58,27 +57,26 @@
       p.start()
 
     for p in processes:
       p.join()
 
     Utils.print('All processes complete.')
 
-  def __slurm(self, individual_gpu, console_logs_path: str = './logs'):
+  def __slurm(self, individual_gpu, console_logs: str):
     r"""
     Similar to :py:meth:`.__gpu` but for SLURM. An additional step includes
     spinning up a process for each node, done with ``submitit``.
 
     :param Job run: Custom training/evaluation task.
-    :param str console_logs_path: Location to save console logs. Default:
-        ``./logs``.
+    :param str console_logs: Location to save console logs.
     """
-
     Utils.print('Setting up the SLURM platform.')
+    from submitit import AutoExecutor
 
-    executor = AutoExecutor(folder=console_logs_path)
+    executor = AutoExecutor(folder=console_logs)
     executor.update_parameters(
       name=self.p_config.name,
       mem_gb=12*self.p_config.n_nodes,
       gpus_per_node=self.p_config.n_gpus,
       tasks_per_node=self.p_config.n_gpus,
       cpus_per_task=self.p_config.cpus_per_task,
       nodes=self.p_config.n_nodes,
@@ -92,44 +90,46 @@
     r"""
     This method begins the setup process for CPU/GPU/SLURM-based jobs and
     commences the task (for training or evaluation).
 
     :param Job run: Custom training/evaluation definitions.
     """
 
-    run.p_config = self.p_config
-    run.a_config = self.a_config
-
     Utils.print('Setup details.')
-    run.p_config.print()
-    run.a_config.print()
-    run.j_config.print()
+    self.p_config.print()
+    self.a_config.print()
 
     Utils.print('Starting process(es).')
 
+    def finished():
+      if self.p_config.upon_finish is not None: self.p_config.upon_finish()
+
     if self.p_config.platform in [Platform.CPU, Platform.MPS]:
       init_process(0, 0, run, self.p_config, self.a_config)
-      Utils.print('CPU/MPS process finished.')
+      finished()
 
     elif self.p_config.platform == Platform.GPU:
       self.__gpu(run)
-      Utils.print('GPU processes finished.')
+      finished()
 
     elif self.p_config.platform == Platform.SLURM:
       def individual_gpu():
         r"""
         This nested function is the starting point for each SLURM-based GPU.
         """
+        from submitit import JobEnvironment
 
         self.p_config.master_addr = os.environ['HOSTNAME']
         job_env = JobEnvironment()
 
         Utils.print(f'Node {job_env.node}: Local rank: {job_env.local_rank}; ' +
                     f'Global rank: {job_env.global_rank}.')
 
         init_process(job_env.global_rank, job_env.local_rank, run,
                      self.p_config, self.a_config)
 
-      job = self.__slurm(individual_gpu, run.j_config.console_logs_path)
+        if (job_env.global_rank == 0): finished()
+
+      job = self.__slurm(individual_gpu, self.p_config.console_logs)
       Utils.print(f'SLURM job "{self.p_config.name}" scheduled; ' +
                   f'job ID: {job.job_id}.')
       Utils.print(f'See respective device logs for output on those devices.')
```

### Comparing `ddpw-3.0.0/ddpw.egg-info/PKG-INFO` & `ddpw-4.0.0/ddpw.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddpw
-Version: 3.0.0
+Version: 4.0.0
 Summary: A utility package to scaffold PyTorch's DDP
 Home-page: https://ddpw.projects.sujal.tv
 Author: Sujal T.V.
 License: UNKNOWN
 Description: # DDPW
         
         [![AWS S3](https://img.shields.io/badge/documentation-sphinx-blue?link=https://ddpw.projects.sujal.tv)](https://ddpw.projects.sujal.tv)
@@ -13,15 +13,15 @@
         
         [![Publish documentation to AWS S3](https://github.com/sujaltv/ddpw/actions/workflows/s3_publish.yaml/badge.svg)](https://github.com/sujaltv/ddpw/actions/workflows/s3_publish.yaml)
         [![Publish to Anaconda](https://github.com/sujaltv/ddpw/actions/workflows/conda_publish.yaml/badge.svg)](https://github.com/sujaltv/ddpw/actions/workflows/conda_publish.yaml)
         [![Publish to PyPI](https://github.com/sujaltv/ddpw/actions/workflows/pypi_publish.yaml/badge.svg)](https://github.com/sujaltv/ddpw/actions/workflows/pypi_publish.yaml)
         
         ---
         
-        The Distributed Data Parallel wrapper (DDPW) is created as a utility package to
+        **Distributed Data Parallel Wrapper (DDPW)** is created as a utility package to
         encapsulate the scaffolding for PyTorch's Distributed Data Parallel.
         
         This code is written in Python. The [DDPW
         documentation](https://ddpw.projects.sujal.tv) contains details on how to use
         this package.
         
         ## Overview
@@ -32,32 +32,37 @@
         conda install -c tvsujal ddpw # with conda
         pip install ddpw # with pip from PyPI
         ```
         
         ### Usage
         
         ```python
-          from ddpw.platform import PlatformConfig
-          from ddpw.artefacts import ArtefactsConfig
-          from ddpw.job import JobConfig
-          from ddpw.wrapper import Wrapper
+        from ddpw.platform import Platform, PlatformConfig
+        from ddpw.artefacts import ArtefactsConfig
+        from ddpw.job import JobConfig, JobMode
+        from ddpw.wrapper import Wrapper
+        
+        from src import MyDataset, MyModel, MyOptimiser, MyTrainer
+        
+        # datasets
+        train_set = MyDataset(train=True)
+        test_set = MyDataset(train=False)
+        
+        # configure the platform
+        p_config = PlatformConfig(platform=Platform.GPU, n_gpus=4, cpus_per_task=2)
+        
+        # configure the artefacts (model, dataset, optimiser, etc.)
+        a_config = ArtefactsConfig(train_set=train_set, test_set=test_set,
+            batch_size=64, model=MyModel(), optimiser_loader=MyOptimiser(lr=0.1))
         
-          from src import MyTrainer
-        
-          p = PlatformConfig(...)
-          a = ArtefactsConfig(...)
-          t = JobConfig(...)
-        
-          d = Wrapper(p, a)
-          j = MyTrainer(t)
-        
-          d.start(j)
+        # call the job
+        Wrapper(p_config, a_config).start(MyTrainer())
         ```
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ddpw-3.0.0/setup.py` & `ddpw-4.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,10 +19,10 @@
   classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux"
   ],
-  python_requires='>=3.8',
-  install_requires=['numpy>=1.22.2', 'submitit>=1.2.1', 'torch>=1.10.1']
+  python_requires='>=3.10',
+  install_requires=['numpy>=1.22.2', 'submitit>=1.2.1', 'torch>=2.0.0']
 )
```

