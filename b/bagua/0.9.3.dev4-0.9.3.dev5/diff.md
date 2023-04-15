# Comparing `tmp/bagua-0.9.3.dev4.tar.gz` & `tmp/bagua-0.9.3.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/__w/bagua/bagua/dist/.tmp-dnpcflld/bagua-0.9.3.dev4.tar", last modified: Sat Apr 15 10:00:42 2023, max compression
+gzip compressed data, was "/__w/bagua/bagua/dist/.tmp-zpoy7d1u/bagua-0.9.3.dev5.tar", last modified: Sat Apr 15 12:29:13 2023, max compression
```

## Comparing `bagua-0.9.3.dev4.tar` & `bagua-0.9.3.dev5.tar`

### file list

```diff
@@ -1,661 +1,661 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/.buildkite/
--rw-r--r--   0 root         (0) root         (0)     1715 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/.buildkite/pipeline.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/.buildkite/scripts/
--rw-r--r--   0 root         (0) root         (0)      970 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/.buildkite/scripts/benchmark.sh
--rw-r--r--   0 root         (0) root         (0)     5373 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/.buildkite/scripts/benchmark_master.sh
--rw-r--r--   0 root         (0) root         (0)     2001 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/.buildkite/scripts/benchmark_worker.sh
--rwxr-xr-x   0 root         (0) root         (0)      112 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/.buildkite/scripts/example.sh
--rw-r--r--   0 root         (0) root         (0)      435 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/.buildkite/scripts/install_bagua.sh
--rwxr-xr-x   0 root         (0) root         (0)      358 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/.buildkite/scripts/run_pytest.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/.github/
--rw-r--r--   0 root         (0) root         (0)      748 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/.github/CODEOWNERS
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      723 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 root         (0) root         (0)      595 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 root         (0) root         (0)      708 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/.github/dependabot.yml
--rw-r--r--   0 root         (0) root         (0)      756 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/.github/issue-close-app.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      286 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/.github/workflows/bagua-net-ci.yml
--rw-r--r--   0 root         (0) root         (0)     4668 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/.github/workflows/bagua-pypi-publish.yml
--rw-r--r--   0 root         (0) root         (0)      907 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/.github/workflows/bagua-python-package-check.yml
--rw-r--r--   0 root         (0) root         (0)      482 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/.github/workflows/black.yml
--rw-r--r--   0 root         (0) root         (0)     2558 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/.github/workflows/dockerhub.yml
--rw-r--r--   0 root         (0) root         (0)     1141 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/.github/workflows/flake8.yml
--rw-r--r--   0 root         (0) root         (0)     1159 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/.github/workflows/pytype.yml
--rw-r--r--   0 root         (0) root         (0)      535 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/.github/workflows/rustfmt.yml
--rw-r--r--   0 root         (0) root         (0)      246 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/.gitignore
--rw-r--r--   0 root         (0) root         (0)      200 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/.gitmodules
--rw-r--r--   0 root         (0) root         (0)    11029 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1087 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     1087 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      805 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      637 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/Makefile
--rw-r--r--   0 root         (0) root         (0)    10292 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9791 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/bagua/
--rw-r--r--   0 root         (0) root         (0)      339 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1289 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/bagua_define.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/bagua/distributed/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/distributed/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12057 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/distributed/launch.py
--rw-r--r--   0 root         (0) root         (0)    24025 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/distributed/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/bagua/script/
--rw-r--r--   0 root         (0) root         (0)       37 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/script/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4533 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/script/bagua_sys_perf
--rw-r--r--   0 root         (0) root         (0)     7437 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/script/baguarun.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/bagua/service/
--rw-r--r--   0 root         (0) root         (0)       76 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/service/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15639 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/service/autotune_service.py
--rw-r--r--   0 root         (0) root         (0)     4775 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/service/autotune_system.py
--rw-r--r--   0 root         (0) root         (0)     5726 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/service/autotune_task_manager.py
--rw-r--r--   0 root         (0) root         (0)     2237 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/service/bayesian_optimizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/bagua/torch_api/
--rw-r--r--   0 root         (0) root         (0)     1497 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/bagua/torch_api/algorithms/
--rw-r--r--   0 root         (0) root         (0)     1101 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/algorithms/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13830 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/algorithms/async_model_average.py
--rw-r--r--   0 root         (0) root         (0)     9202 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/algorithms/base.py
--rw-r--r--   0 root         (0) root         (0)     2795 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/algorithms/bytegrad.py
--rw-r--r--   0 root         (0) root         (0)    10572 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/algorithms/decentralized.py
--rw-r--r--   0 root         (0) root         (0)     2237 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/algorithms/gradient_allreduce.py
--rw-r--r--   0 root         (0) root         (0)     9992 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/algorithms/q_adam.py
--rw-r--r--   0 root         (0) root         (0)    16103 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/bucket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/bagua/torch_api/checkpoint/
--rw-r--r--   0 root         (0) root         (0)      114 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/checkpoint/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12238 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/checkpoint/checkpointing.py
--rw-r--r--   0 root         (0) root         (0)    45904 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/communication.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/bagua/torch_api/contrib/
--rw-r--r--   0 root         (0) root         (0)      302 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/contrib/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4737 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/contrib/cache_loader.py
--rw-r--r--   0 root         (0) root         (0)     2582 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/contrib/cached_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/bagua/torch_api/contrib/fuse/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/contrib/fuse/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20240 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/contrib/fuse/optimizer.py
--rw-r--r--   0 root         (0) root         (0)    13250 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/contrib/load_balancing_data_loader.py
--rw-r--r--   0 root         (0) root         (0)    10981 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/contrib/sync_batchnorm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/bagua/torch_api/contrib/utils/
--rw-r--r--   0 root         (0) root         (0)       35 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/contrib/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7057 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/contrib/utils/redis_store.py
--rw-r--r--   0 root         (0) root         (0)     4140 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/contrib/utils/store.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/bagua/torch_api/data_parallel/
--rw-r--r--   0 root         (0) root         (0)       63 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/data_parallel/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20686 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/data_parallel/bagua_distributed.py
--rw-r--r--   0 root         (0) root         (0)    15123 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/data_parallel/distributed.py
--rw-r--r--   0 root         (0) root         (0)     2253 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/data_parallel/functional.py
--rw-r--r--   0 root         (0) root         (0)     5570 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/distributed.py
--rw-r--r--   0 root         (0) root         (0)     3292 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/env.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/bagua/torch_api/model_parallel/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/model_parallel/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/bagua/torch_api/model_parallel/moe/
--rw-r--r--   0 root         (0) root         (0)       83 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/model_parallel/moe/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1425 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/model_parallel/moe/experts.py
--rw-r--r--   0 root         (0) root         (0)     3546 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/model_parallel/moe/layer.py
--rw-r--r--   0 root         (0) root         (0)    13628 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/model_parallel/moe/sharded_moe.py
--rw-r--r--   0 root         (0) root         (0)      149 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/model_parallel/moe/utils.py
--rw-r--r--   0 root         (0) root         (0)    11765 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/tensor.py
--rw-r--r--   0 root         (0) root         (0)     7731 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua/torch_api/utils.py
--rw-r--r--   0 root         (0) root         (0)       27 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/bagua/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/bagua.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10292 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/bagua.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    36352 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/bagua.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/bagua.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/bagua.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/bagua.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      254 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/bagua.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/bagua.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/bagua_core/
--rw-r--r--   0 root         (0) root         (0)      181 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua_core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      262 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua_core/_environment.py
--rw-r--r--   0 root         (0) root         (0)     4471 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/bagua_core/bagua_install_deps.py
--rw-r--r--   0 root         (0) root         (0)     1630 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/cliff.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/docker/
--rw-r--r--   0 root         (0) root         (0)     1142 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/docker/Dockerfile.manylinux-cuda102
--rw-r--r--   0 root         (0) root         (0)     1217 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/docker/Dockerfile.manylinux-cuda111
--rw-r--r--   0 root         (0) root         (0)     1217 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/docker/Dockerfile.manylinux-cuda113
--rw-r--r--   0 root         (0) root         (0)     1218 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/docker/Dockerfile.manylinux-cuda115
--rw-r--r--   0 root         (0) root         (0)     1249 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/docker/Dockerfile.manylinux-cuda116
--rw-r--r--   0 root         (0) root         (0)     1249 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/docker/Dockerfile.manylinux-cuda117
--rw-r--r--   0 root         (0) root         (0)     2708 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/docker/Dockerfile.pytorch-1.10.0-cuda11.3-cudnn8
--rw-r--r--   0 root         (0) root         (0)     2962 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/docker/Dockerfile.pytorch-1.11.0-cuda11.3-cudnn8
--rw-r--r--   0 root         (0) root         (0)     2840 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/docker/Dockerfile.pytorch-1.12.0-cuda11.3-cudnn8
--rw-r--r--   0 root         (0) root         (0)     2840 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/docker/Dockerfile.pytorch-1.13.0-cuda11.6-cudnn8
--rw-r--r--   0 root         (0) root         (0)     2698 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/docker/Dockerfile.pytorch-1.9.0-cuda10.2-cudnn7
--rw-r--r--   0 root         (0) root         (0)     2698 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/docker/Dockerfile.pytorch-1.9.0-cuda11.1-cudnn8
--rw-r--r--   0 root         (0) root         (0)     2839 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/docker/Dockerfile.pytorch-2.0.0-cuda11.7-cudnn8
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/docs/_autoapi_templates/
--rw-r--r--   0 root         (0) root         (0)      673 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/docs/_autoapi_templates/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/docs/_autoapi_templates/python/
--rw-r--r--   0 root         (0) root         (0)       32 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/docs/_autoapi_templates/python/attribute.rst
--rw-r--r--   0 root         (0) root         (0)     2008 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/docs/_autoapi_templates/python/class.rst
--rw-r--r--   0 root         (0) root         (0)      765 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/docs/_autoapi_templates/python/data.rst
--rw-r--r--   0 root         (0) root         (0)       33 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/docs/_autoapi_templates/python/exception.rst
--rw-r--r--   0 root         (0) root         (0)      594 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/docs/_autoapi_templates/python/function.rst
--rw-r--r--   0 root         (0) root         (0)      847 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/docs/_autoapi_templates/python/method.rst
--rw-r--r--   0 root         (0) root         (0)     2454 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/docs/_autoapi_templates/python/module.rst
--rw-r--r--   0 root         (0) root         (0)       34 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/docs/_autoapi_templates/python/package.rst
--rw-r--r--   0 root         (0) root         (0)     7076 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)       70 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/docs/doc-requirements.txt
--rw-r--r--   0 root         (0) root         (0)      673 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/docs/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/examples/
--rw-r--r--   0 root         (0) root         (0)     1089 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/examples/LICENSE
--rw-r--r--   0 root         (0) root         (0)      189 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/examples/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/examples/benchmark/
--rw-r--r--   0 root         (0) root         (0)      338 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/examples/benchmark/README.md
--rw-r--r--   0 root         (0) root         (0)       35 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/examples/benchmark/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     6520 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/examples/benchmark/synthetic_benchmark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/examples/communication_primitives/
--rw-r--r--   0 root         (0) root         (0)      235 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/examples/communication_primitives/README.md
--rw-r--r--   0 root         (0) root         (0)     6662 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/examples/communication_primitives/main.py
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/examples/communication_primitives/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/examples/elastic_training/
--rw-r--r--   0 root         (0) root         (0)      412 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/examples/elastic_training/README.md
--rw-r--r--   0 root         (0) root         (0)     8178 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/examples/elastic_training/main.py
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/examples/elastic_training/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/examples/imagenet/
--rw-r--r--   0 root         (0) root         (0)     1382 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/examples/imagenet/README.md
--rw-r--r--   0 root         (0) root         (0)    17552 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/examples/imagenet/main.py
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/examples/imagenet/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/examples/mnist/
--rw-r--r--   0 root         (0) root         (0)      171 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/examples/mnist/README.md
--rw-r--r--   0 root         (0) root         (0)     8644 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/examples/mnist/main.py
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/examples/mnist/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/examples/moe/
--rw-r--r--   0 root         (0) root         (0)      199 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/examples/moe/README.md
--rw-r--r--   0 root         (0) root         (0)     8884 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/examples/moe/mnist_main.py
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/examples/moe/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/examples/squad/
--rw-r--r--   0 root         (0) root         (0)      958 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/examples/squad/README.md
--rw-r--r--   0 root         (0) root         (0)    41793 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/examples/squad/main.py
--rw-r--r--   0 root         (0) root         (0)       56 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/examples/squad/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/figures/
--rw-r--r--   0 root         (0) root         (0)    14450 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/figures/logo.png
--rw-r--r--   0 root         (0) root         (0)     3036 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/install.sh
--rw-r--r--   0 root         (0) root         (0)     4374 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/install_master.sh
--rw-r--r--   0 root         (0) root         (0)      334 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/
--rw-r--r--   0 root         (0) root         (0)      109 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/.gitignore
--rw-r--r--   0 root         (0) root         (0)    67240 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/Cargo.lock
--rw-r--r--   0 root         (0) root         (0)      139 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/Cargo.toml
--rw-r--r--   0 root         (0) root         (0)      188 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-c/
--rw-r--r--   0 root         (0) root         (0)      730 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-c/Cargo.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-c/src/
--rw-r--r--   0 root         (0) root         (0)     8640 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-c/src/lib.rs
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/
--rw-r--r--   0 root         (0) root         (0)     1082 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/Cargo.toml
--rw-r--r--   0 root         (0) root         (0)     4349 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/build.rs
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/cpp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/cpp/include/
--rw-r--r--   0 root         (0) root         (0)      895 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/cpp/include/bagua_utils.h
--rw-r--r--   0 root         (0) root         (0)    24308 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/cpp/include/dbg.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/kernels/
--rw-r--r--   0 root         (0) root         (0)    25551 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/kernels/bagua_kernels.cu
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/comm_ops/
--rw-r--r--   0 root         (0) root         (0)     2222 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/comm_ops/centralized_full_precision_synchronous.rs
--rw-r--r--   0 root         (0) root         (0)     2903 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/comm_ops/centralized_low_precision_synchronous.rs
--rw-r--r--   0 root         (0) root         (0)     7645 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/comm_ops/decentralized_full_precision_asynchronous.rs
--rw-r--r--   0 root         (0) root         (0)     4806 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/comm_ops/decentralized_full_precision_synchronous.rs
--rw-r--r--   0 root         (0) root         (0)     6375 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/comm_ops/decentralized_low_precision_synchronous.rs
--rw-r--r--   0 root         (0) root         (0)      571 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/comm_ops/mod.rs
--rw-r--r--   0 root         (0) root         (0)      665 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/comm_ops/python_ffi_op.rs
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/communicators/
--rw-r--r--   0 root         (0) root         (0)    53076 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/communicators/mod.rs
--rw-r--r--   0 root         (0) root         (0)      559 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/cuda_utils.rs
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/datatypes/
--rw-r--r--   0 root         (0) root         (0)    46518 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/datatypes/mod.rs
--rw-r--r--   0 root         (0) root         (0)      759 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/events.rs
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/kernels/
--rw-r--r--   0 root         (0) root         (0)     3917 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/kernels/mod.rs
--rw-r--r--   0 root         (0) root         (0)    12601 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/lib.rs
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/resource_pool/
--rw-r--r--   0 root         (0) root         (0)     2182 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/resource_pool/mod.rs
--rw-r--r--   0 root         (0) root         (0)    66619 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/torch_ffi.rs
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/
--rw-r--r--   0 root         (0) root         (0)      294 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/.gitignore
--rw-r--r--   0 root         (0) root         (0)      110 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/.gitmodules
--rw-r--r--   0 root         (0) root         (0)    15030 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      329 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/CONTRIBUTORS
--rw-r--r--   0 root         (0) root         (0)     1046 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6566 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/
--rw-r--r--   0 root         (0) root         (0)     3313 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     2282 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/benchmark_events.cpp
--rw-r--r--   0 root         (0) root         (0)     9764 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/benchmark_ops.cpp
--rw-r--r--   0 root         (0) root         (0)     8731 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/benchmark_utils.hpp
--rw-r--r--   0 root         (0) root         (0)     2297 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/benchmark_utils_ht.hpp
--rw-r--r--   0 root         (0) root         (0)     1587 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/benchmark_utils_mpi.hpp
--rw-r--r--   0 root         (0) root         (0)     2273 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/benchmark_utils_nccl.hpp
--rw-r--r--   0 root         (0) root         (0)     2358 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/benchmark_waits.cpp
--rw-r--r--   0 root         (0) root         (0)    12693 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/plot_benchmarks.py
--rw-r--r--   0 root         (0) root         (0)     9566 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/run_benchmarks.py
--rw-r--r--   0 root         (0) root         (0)     2244 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/wait.cu
--rw-r--r--   0 root         (0) root         (0)     1412 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/wait.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/
--rw-r--r--   0 root         (0) root         (0)      587 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/Al_config.hpp.in
--rw-r--r--   0 root         (0) root         (0)     2265 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/AluminumConfig.cmake.in
--rw-r--r--   0 root         (0) root         (0)     1335 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/FindCUB.cmake
--rw-r--r--   0 root         (0) root         (0)     1625 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/FindHWLOC.cmake
--rw-r--r--   0 root         (0) root         (0)     2190 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/FindNCCL.cmake
--rw-r--r--   0 root         (0) root         (0)      755 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/FindNVTX.cmake
--rw-r--r--   0 root         (0) root         (0)     2002 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/HipBuildSystem.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/
--rw-r--r--   0 root         (0) root         (0)    47921 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/Al.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/
--rw-r--r--   0 root         (0) root         (0)     1311 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     2505 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/base.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/
--rw-r--r--   0 root         (0) root         (0)      232 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     6578 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/cuda.hpp
--rw-r--r--   0 root         (0) root         (0)     2536 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/cuda_mempool.hpp
--rw-r--r--   0 root         (0) root         (0)     2025 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/events.hpp
--rw-r--r--   0 root         (0) root         (0)     2423 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/gpu_status_flag.hpp
--rw-r--r--   0 root         (0) root         (0)     2320 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/gpu_wait.hpp
--rw-r--r--   0 root         (0) root         (0)     1778 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/helper_kernels.hpp
--rw-r--r--   0 root         (0) root         (0)     3080 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/streams.hpp
--rw-r--r--   0 root         (0) root         (0)     2337 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/sync_memory.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/
--rw-r--r--   0 root         (0) root         (0)      395 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     3258 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/allgather.hpp
--rw-r--r--   0 root         (0) root         (0)     3581 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/allgatherv.hpp
--rw-r--r--   0 root         (0) root         (0)     3094 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/allreduce.hpp
--rw-r--r--   0 root         (0) root         (0)     2862 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/alltoall.hpp
--rw-r--r--   0 root         (0) root         (0)     4941 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/alltoallv.hpp
--rw-r--r--   0 root         (0) root         (0)     2094 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/barrier.hpp
--rw-r--r--   0 root         (0) root         (0)     6031 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/base_state.hpp
--rw-r--r--   0 root         (0) root         (0)     2864 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/bcast.hpp
--rw-r--r--   0 root         (0) root         (0)     2618 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/communicator.hpp
--rw-r--r--   0 root         (0) root         (0)     3485 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/gather.hpp
--rw-r--r--   0 root         (0) root         (0)     4058 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/gatherv.hpp
--rw-r--r--   0 root         (0) root         (0)     7427 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/pt2pt.hpp
--rw-r--r--   0 root         (0) root         (0)     3137 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/reduce.hpp
--rw-r--r--   0 root         (0) root         (0)     2979 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/reduce_scatter.hpp
--rw-r--r--   0 root         (0) root         (0)     3179 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/reduce_scatterv.hpp
--rw-r--r--   0 root         (0) root         (0)     3772 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/scatter.hpp
--rw-r--r--   0 root         (0) root         (0)     4362 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/scatterv.hpp
--rw-r--r--   0 root         (0) root         (0)    36227 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht_impl.hpp
--rw-r--r--   0 root         (0) root         (0)     1746 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/internal.hpp
--rw-r--r--   0 root         (0) root         (0)     4552 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mempool.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/
--rw-r--r--   0 root         (0) root         (0)      461 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     2861 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/allgather.hpp
--rw-r--r--   0 root         (0) root         (0)     3535 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/allgatherv.hpp
--rw-r--r--   0 root         (0) root         (0)    42883 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/allreduce.hpp
--rw-r--r--   0 root         (0) root         (0)     2847 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/alltoall.hpp
--rw-r--r--   0 root         (0) root         (0)     4479 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/alltoallv.hpp
--rw-r--r--   0 root         (0) root         (0)     2240 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/barrier.hpp
--rw-r--r--   0 root         (0) root         (0)     2151 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/base_state.hpp
--rw-r--r--   0 root         (0) root         (0)     2617 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/bcast.hpp
--rw-r--r--   0 root         (0) root         (0)     3067 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/communicator.hpp
--rw-r--r--   0 root         (0) root         (0)     3221 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/gather.hpp
--rw-r--r--   0 root         (0) root         (0)     3889 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/gatherv.hpp
--rw-r--r--   0 root         (0) root         (0)     6043 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/pt2pt.hpp
--rw-r--r--   0 root         (0) root         (0)     3363 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/reduce.hpp
--rw-r--r--   0 root         (0) root         (0)     3153 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/reduce_scatter.hpp
--rw-r--r--   0 root         (0) root         (0)     3480 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/reduce_scatterv.hpp
--rw-r--r--   0 root         (0) root         (0)     3313 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/scatter.hpp
--rw-r--r--   0 root         (0) root         (0)     3952 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/scatterv.hpp
--rw-r--r--   0 root         (0) root         (0)     8509 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/utils.hpp
--rw-r--r--   0 root         (0) root         (0)     4533 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_comm_and_stream_wrapper.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda/
--rw-r--r--   0 root         (0) root         (0)      358 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     2396 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda/communicator.hpp
--rw-r--r--   0 root         (0) root         (0)     5473 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda/rma.hpp
--rw-r--r--   0 root         (0) root         (0)    10021 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda/rma_ipc.hpp
--rw-r--r--   0 root         (0) root         (0)     2115 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda/rma_null.hpp
--rw-r--r--   0 root         (0) root         (0)     2467 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda/rma_self.hpp
--rw-r--r--   0 root         (0) root         (0)     4933 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda/util.hpp
--rw-r--r--   0 root         (0) root         (0)     4129 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda_impl.hpp
--rw-r--r--   0 root         (0) root         (0)    32186 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_impl.hpp
--rw-r--r--   0 root         (0) root         (0)    51540 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/nccl_impl.hpp
--rw-r--r--   0 root         (0) root         (0)     2232 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/profiling.hpp
--rw-r--r--   0 root         (0) root         (0)     5988 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/progress.hpp
--rw-r--r--   0 root         (0) root         (0)     5096 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/state.hpp
--rw-r--r--   0 root         (0) root         (0)     3203 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/trace.hpp
--rw-r--r--   0 root         (0) root         (0)     3055 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/tuning_params.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/utils/
--rw-r--r--   0 root         (0) root         (0)      291 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/utils/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     7761 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/utils/caching_allocator.hpp
--rw-r--r--   0 root         (0) root         (0)     3210 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/utils/locked_resource_pool.hpp
--rw-r--r--   0 root         (0) root         (0)     3587 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/utils/meta.hpp
--rw-r--r--   0 root         (0) root         (0)     5256 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/utils/mpsc_queue.hpp
--rw-r--r--   0 root         (0) root         (0)     4251 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/utils/spsc_queue.hpp
--rw-r--r--   0 root         (0) root         (0)     1883 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/utils/utils.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/
--rw-r--r--   0 root         (0) root         (0)     5002 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/Al.cpp
--rw-r--r--   0 root         (0) root         (0)     3123 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/cuda/
--rw-r--r--   0 root         (0) root         (0)      414 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/cuda/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     2683 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/cuda/cuda.cpp
--rw-r--r--   0 root         (0) root         (0)     3163 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/cuda/gpu_status_flag.cpp
--rw-r--r--   0 root         (0) root         (0)     2493 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/cuda/gpu_wait.cpp
--rw-r--r--   0 root         (0) root         (0)     2109 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/cuda/helper_kernels.cu
--rw-r--r--   0 root         (0) root         (0)     3928 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/cuda/streams.cpp
--rw-r--r--   0 root         (0) root         (0)     1744 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/ht_impl.cpp
--rw-r--r--   0 root         (0) root         (0)     1385 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/mempool.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/mpi_cuda/
--rw-r--r--   0 root         (0) root         (0)      403 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/mpi_cuda/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1706 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/mpi_cuda/communicator.cpp
--rw-r--r--   0 root         (0) root         (0)     3542 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/mpi_cuda/rma.cpp
--rw-r--r--   0 root         (0) root         (0)     1474 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/mpi_cuda_impl.cpp
--rw-r--r--   0 root         (0) root         (0)     2522 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/mpi_impl.cpp
--rw-r--r--   0 root         (0) root         (0)     2864 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/nccl_impl.cpp
--rw-r--r--   0 root         (0) root         (0)     2219 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/profiling.cpp
--rw-r--r--   0 root         (0) root         (0)    20918 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/progress.cpp
--rw-r--r--   0 root         (0) root         (0)     2830 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/trace.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/
--rw-r--r--   0 root         (0) root         (0)     3286 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     4685 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/cuda_vector.hpp
--rw-r--r--   0 root         (0) root         (0)     4017 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/hang_watchdog.hpp
--rw-r--r--   0 root         (0) root         (0)    34118 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/op_dispatcher.hpp
--rw-r--r--   0 root         (0) root         (0)    44646 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/op_runner_impl.hpp
--rw-r--r--   0 root         (0) root         (0)     8572 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/run_tests.py
--rw-r--r--   0 root         (0) root         (0)     5802 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_exchange.cpp
--rw-r--r--   0 root         (0) root         (0)    18155 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_ops.cpp
--rw-r--r--   0 root         (0) root         (0)     9380 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_rma_halo_exchange.cpp
--rw-r--r--   0 root         (0) root         (0)     4467 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_rma_ring.cpp
--rw-r--r--   0 root         (0) root         (0)     1581 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_stream_mem_ops.cpp
--rw-r--r--   0 root         (0) root         (0)    12514 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_utils.hpp
--rw-r--r--   0 root         (0) root         (0)    10487 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_utils_ht.hpp
--rw-r--r--   0 root         (0) root         (0)     8385 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_utils_mpi.hpp
--rw-r--r--   0 root         (0) root         (0)     2648 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_utils_mpi_cuda.hpp
--rw-r--r--   0 root         (0) root         (0)     9815 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_utils_nccl.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/
--rw-r--r--   0 root         (0) root         (0)      127 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/.git
--rw-r--r--   0 root         (0) root         (0)       98 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1839 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/.travis.yml
--rw-r--r--   0 root         (0) root         (0)     3168 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     4430 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      656 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/INSTALL
--rw-r--r--   0 root         (0) root         (0)     1055 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4955 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/README.md
--rw-r--r--   0 root         (0) root         (0)      114 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/cxxopts-config.cmake.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/include/
--rw-r--r--   0 root         (0) root         (0)    42643 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/include/cxxopts.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/src/
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/src/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1212 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/src/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     4831 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/src/example.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1359 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/add-subdirectory-test/
--rw-r--r--   0 root         (0) root         (0)      267 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/add-subdirectory-test/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)   377366 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/catch.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/find-package-test/
--rw-r--r--   0 root         (0) root         (0)      258 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/find-package-test/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/link_a.cpp
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/link_b.cpp
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/main.cpp
--rw-r--r--   0 root         (0) root         (0)    18892 2023-04-15 10:00:34.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/options.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/
--rw-r--r--   0 root         (0) root         (0)    65123 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/.cproject
--rw-r--r--   0 root         (0) root         (0)      835 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/.project
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/.settings/
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/.settings/.gitignore
--rw-r--r--   0 root         (0) root         (0)    10954 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/.settings/org.eclipse.cdt.codan.core.prefs
--rw-r--r--   0 root         (0) root         (0)    14273 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/.settings/org.eclipse.cdt.core.prefs
--rw-r--r--   0 root         (0) root         (0)       86 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/.settings/org.eclipse.cdt.ui.prefs
--rw-r--r--   0 root         (0) root         (0)      190 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/.settings/org.eclipse.core.runtime.prefs
--rw-r--r--   0 root         (0) root         (0)    22309 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/CHANGE_LOG.TXT
--rw-r--r--   0 root         (0) root         (0)     1600 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/LICENSE.TXT
--rw-r--r--   0 root         (0) root         (0)     6051 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/README.md
--rw-r--r--   0 root         (0) root         (0)     7688 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/common.mk
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/
--rw-r--r--   0 root         (0) root         (0)    33331 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_histogram.cuh
--rw-r--r--   0 root         (0) root         (0)    28525 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_radix_sort_downsweep.cuh
--rw-r--r--   0 root         (0) root         (0)    17917 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_radix_sort_upsweep.cuh
--rw-r--r--   0 root         (0) root         (0)    16916 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_reduce.cuh
--rw-r--r--   0 root         (0) root         (0)    24791 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_reduce_by_key.cuh
--rw-r--r--   0 root         (0) root         (0)    35663 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_rle.cuh
--rw-r--r--   0 root         (0) root         (0)    18729 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_scan.cuh
--rw-r--r--   0 root         (0) root         (0)    16655 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_segment_fixup.cuh
--rw-r--r--   0 root         (0) root         (0)    29594 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_select_if.cuh
--rw-r--r--   0 root         (0) root         (0)    27377 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_spmv_orig.cuh
--rw-r--r--   0 root         (0) root         (0)    27444 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/single_pass_scan_operators.cuh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/
--rw-r--r--   0 root         (0) root         (0)    25011 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_adjacent_difference.cuh
--rw-r--r--   0 root         (0) root         (0)    54550 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_discontinuity.cuh
--rw-r--r--   0 root         (0) root         (0)    52305 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_exchange.cuh
--rw-r--r--   0 root         (0) root         (0)    16291 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_histogram.cuh
--rw-r--r--   0 root         (0) root         (0)    53671 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_load.cuh
--rw-r--r--   0 root         (0) root         (0)    25230 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_radix_rank.cuh
--rw-r--r--   0 root         (0) root         (0)    38342 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_radix_sort.cuh
--rw-r--r--   0 root         (0) root         (0)     6181 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_raking_layout.cuh
--rw-r--r--   0 root         (0) root         (0)    25300 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_reduce.cuh
--rw-r--r--   0 root         (0) root         (0)   102978 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_scan.cuh
--rw-r--r--   0 root         (0) root         (0)    11964 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_shuffle.cuh
--rw-r--r--   0 root         (0) root         (0)    41449 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_store.cuh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/
--rw-r--r--   0 root         (0) root         (0)     3285 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_histogram_atomic.cuh
--rw-r--r--   0 root         (0) root         (0)     8198 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_histogram_sort.cuh
--rw-r--r--   0 root         (0) root         (0)     9731 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_reduce_raking.cuh
--rw-r--r--   0 root         (0) root         (0)     8369 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_reduce_raking_commutative_only.cuh
--rw-r--r--   0 root         (0) root         (0)     9769 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_reduce_warp_reductions.cuh
--rw-r--r--   0 root         (0) root         (0)    28460 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_scan_raking.cuh
--rw-r--r--   0 root         (0) root         (0)    19117 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_scan_warp_scans.cuh
--rw-r--r--   0 root         (0) root         (0)    20949 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_scan_warp_scans2.cuh
--rw-r--r--   0 root         (0) root         (0)    19463 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_scan_warp_scans3.cuh
--rw-r--r--   0 root         (0) root         (0)     3626 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/cub.cuh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/
--rw-r--r--   0 root         (0) root         (0)    54347 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_histogram.cuh
--rw-r--r--   0 root         (0) root         (0)    13891 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_partition.cuh
--rw-r--r--   0 root         (0) root         (0)    42384 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_radix_sort.cuh
--rw-r--r--   0 root         (0) root         (0)    38904 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_reduce.cuh
--rw-r--r--   0 root         (0) root         (0)    14817 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_run_length_encode.cuh
--rw-r--r--   0 root         (0) root         (0)    21786 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_scan.cuh
--rw-r--r--   0 root         (0) root         (0)    54689 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_segmented_radix_sort.cuh
--rw-r--r--   0 root         (0) root         (0)    36523 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_segmented_reduce.cuh
--rw-r--r--   0 root         (0) root         (0)    18838 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_select.cuh
--rw-r--r--   0 root         (0) root         (0)     8523 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_spmv.cuh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/
--rw-r--r--   0 root         (0) root         (0)    57226 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_histogram.cuh
--rw-r--r--   0 root         (0) root         (0)    80406 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_radix_sort.cuh
--rw-r--r--   0 root         (0) root         (0)    42707 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_reduce.cuh
--rw-r--r--   0 root         (0) root         (0)    25478 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_reduce_by_key.cuh
--rw-r--r--   0 root         (0) root         (0)    23601 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_rle.cuh
--rw-r--r--   0 root         (0) root         (0)    22778 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_scan.cuh
--rw-r--r--   0 root         (0) root         (0)    24454 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_select_if.cuh
--rw-r--r--   0 root         (0) root         (0)    33269 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_spmv_orig.cuh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/grid/
--rw-r--r--   0 root         (0) root         (0)     5861 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/grid/grid_barrier.cuh
--rw-r--r--   0 root         (0) root         (0)     8198 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/grid/grid_even_share.cuh
--rw-r--r--   0 root         (0) root         (0)     4827 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/grid/grid_mapping.cuh
--rw-r--r--   0 root         (0) root         (0)     7475 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/grid/grid_queue.cuh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/host/
--rw-r--r--   0 root         (0) root         (0)     4581 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/host/mutex.cuh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/
--rw-r--r--   0 root         (0) root         (0)     8781 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/arg_index_input_iterator.cuh
--rw-r--r--   0 root         (0) root         (0)     8104 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/cache_modified_input_iterator.cuh
--rw-r--r--   0 root         (0) root         (0)     8322 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/cache_modified_output_iterator.cuh
--rw-r--r--   0 root         (0) root         (0)     7650 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/constant_input_iterator.cuh
--rw-r--r--   0 root         (0) root         (0)     7369 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/counting_input_iterator.cuh
--rw-r--r--   0 root         (0) root         (0)     6817 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/discard_output_iterator.cuh
--rw-r--r--   0 root         (0) root         (0)    10546 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/tex_obj_input_iterator.cuh
--rw-r--r--   0 root         (0) root         (0)    12430 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/tex_ref_input_iterator.cuh
--rw-r--r--   0 root         (0) root         (0)     8611 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/transform_input_iterator.cuh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/thread/
--rw-r--r--   0 root         (0) root         (0)    18869 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/thread/thread_load.cuh
--rw-r--r--   0 root         (0) root         (0)     9228 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/thread/thread_operators.cuh
--rw-r--r--   0 root         (0) root         (0)     6037 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/thread/thread_reduce.cuh
--rw-r--r--   0 root         (0) root         (0)    10566 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/thread/thread_scan.cuh
--rw-r--r--   0 root         (0) root         (0)     4797 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/thread/thread_search.cuh
--rw-r--r--   0 root         (0) root         (0)    17932 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/thread/thread_store.cuh
--rw-r--r--   0 root         (0) root         (0)    28716 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_allocator.cuh
--rw-r--r--   0 root         (0) root         (0)     6955 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_arch.cuh
--rw-r--r--   0 root         (0) root         (0)     5061 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_debug.cuh
--rw-r--r--   0 root         (0) root         (0)    10658 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_device.cuh
--rw-r--r--   0 root         (0) root         (0)     3710 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_macro.cuh
--rw-r--r--   0 root         (0) root         (0)     2100 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_namespace.cuh
--rw-r--r--   0 root         (0) root         (0)    22318 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_ptx.cuh
--rw-r--r--   0 root         (0) root         (0)    40178 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_type.cuh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/warp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/warp/specializations/
--rw-r--r--   0 root         (0) root         (0)    21412 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/warp/specializations/warp_reduce_shfl.cuh
--rw-r--r--   0 root         (0) root         (0)    14280 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/warp/specializations/warp_reduce_smem.cuh
--rw-r--r--   0 root         (0) root         (0)    25284 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/warp/specializations/warp_scan_shfl.cuh
--rw-r--r--   0 root         (0) root         (0)    16153 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/warp/specializations/warp_scan_smem.cuh
--rw-r--r--   0 root         (0) root         (0)    25032 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/warp/warp_reduce.cuh
--rw-r--r--   0 root         (0) root         (0)    38915 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/warp/warp_scan.cuh
--rw-r--r--   0 root         (0) root         (0)    16543 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/eclipse code style profile.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/block/
--rw-r--r--   0 root         (0) root         (0)       69 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/block/.gitignore
--rw-r--r--   0 root         (0) root         (0)     5255 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/block/Makefile
--rw-r--r--   0 root         (0) root         (0)    10724 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/block/example_block_radix_sort.cu
--rw-r--r--   0 root         (0) root         (0)     9644 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/block/example_block_reduce.cu
--rw-r--r--   0 root         (0) root         (0)    11329 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/block/example_block_scan.cu
--rw-r--r--   0 root         (0) root         (0)     1554 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/block/reduce_by_key.cu
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/
--rw-r--r--   0 root         (0) root         (0)       75 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/.gitignore
--rw-r--r--   0 root         (0) root         (0)     8830 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/Makefile
--rw-r--r--   0 root         (0) root         (0)     8173 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_partition_flagged.cu
--rw-r--r--   0 root         (0) root         (0)     8236 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_partition_if.cu
--rw-r--r--   0 root         (0) root         (0)     8303 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_radix_sort.cu
--rw-r--r--   0 root         (0) root         (0)     5825 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_reduce.cu
--rw-r--r--   0 root         (0) root         (0)     6007 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_scan.cu
--rw-r--r--   0 root         (0) root         (0)     8156 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_select_flagged.cu
--rw-r--r--   0 root         (0) root         (0)     8210 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_select_if.cu
--rw-r--r--   0 root         (0) root         (0)     7493 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_select_unique.cu
--rw-r--r--   0 root         (0) root         (0)    13277 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_sort_find_non_trivial_runs.cu
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/.gitignore
--rw-r--r--   0 root         (0) root         (0)     4949 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/defunct/
--rw-r--r--   0 root         (0) root         (0)    37185 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/defunct/example_coo_spmv.cu
--rw-r--r--   0 root         (0) root         (0)    95317 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/defunct/test_device_seg_reduce.cu
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/histogram/
--rw-r--r--   0 root         (0) root         (0)     4374 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/histogram/histogram_cub.h
--rw-r--r--   0 root         (0) root         (0)     6368 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/histogram/histogram_gmem_atomics.h
--rw-r--r--   0 root         (0) root         (0)     6812 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/histogram/histogram_smem_atomics.h
--rw-r--r--   0 root         (0) root         (0)    21778 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/histogram_compare.cu
--rw-r--r--   0 root         (0) root         (0)    39231 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/sparse_matrix.h
--rw-r--r--   0 root         (0) root         (0)    30656 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/spmv_compare.cu
--rwxr-xr-x   0 root         (0) root         (0)      749 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/spmv_script.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/.gitignore
--rw-r--r--   0 root         (0) root         (0)    18927 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/Makefile
--rw-r--r--   0 root         (0) root         (0)     8397 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/half.h
--rw-r--r--   0 root         (0) root         (0)      315 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/link_a.cu
--rw-r--r--   0 root         (0) root         (0)      315 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/link_b.cu
--rw-r--r--   0 root         (0) root         (0)      113 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/link_main.cpp
--rw-r--r--   0 root         (0) root         (0)     5148 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/mersenne.h
--rw-r--r--   0 root         (0) root         (0)    16564 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_allocator.cu
--rw-r--r--   0 root         (0) root         (0)     9623 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_block_histogram.cu
--rw-r--r--   0 root         (0) root         (0)    19496 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_block_load_store.cu
--rw-r--r--   0 root         (0) root         (0)    25392 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_block_radix_sort.cu
--rw-r--r--   0 root         (0) root         (0)    26628 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_block_reduce.cu
--rw-r--r--   0 root         (0) root         (0)    34810 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_block_scan.cu
--rw-r--r--   0 root         (0) root         (0)    70313 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_histogram.cu
--rw-r--r--   0 root         (0) root         (0)    46469 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_radix_sort.cu
--rw-r--r--   0 root         (0) root         (0)    49902 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_reduce.cu
--rw-r--r--   0 root         (0) root         (0)    30363 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_reduce_by_key.cu
--rw-r--r--   0 root         (0) root         (0)    31192 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_run_length_encode.cu
--rw-r--r--   0 root         (0) root         (0)    33600 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_scan.cu
--rw-r--r--   0 root         (0) root         (0)    37640 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_select_if.cu
--rw-r--r--   0 root         (0) root         (0)    21518 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_select_unique.cu
--rw-r--r--   0 root         (0) root         (0)     5132 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_grid_barrier.cu
--rw-r--r--   0 root         (0) root         (0)    25549 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_iterator.cu
--rw-r--r--   0 root         (0) root         (0)    54847 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_util.h
--rw-r--r--   0 root         (0) root         (0)    27186 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_warp_reduce.cu
--rw-r--r--   0 root         (0) root         (0)    20350 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_warp_scan.cu
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/tune/
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/tune/.gitignore
--rw-r--r--   0 root         (0) root         (0)     6388 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/tune/Makefile
--rw-r--r--   0 root         (0) root         (0)    27663 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/tune/tune_device_reduce.cu
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-py/
--rw-r--r--   0 root         (0) root         (0)      783 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-py/Cargo.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-py/src/
--rw-r--r--   0 root         (0) root         (0)    18099 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-core-py/src/lib.rs
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-opentelemetry/
--rw-r--r--   0 root         (0) root         (0)      629 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-opentelemetry/Cargo.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-opentelemetry/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-opentelemetry/src/exporter/
--rw-r--r--   0 root         (0) root         (0)     1022 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-opentelemetry/src/exporter/agent.rs
--rw-r--r--   0 root         (0) root         (0)     1815 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-opentelemetry/src/exporter/mod.rs
--rw-r--r--   0 root         (0) root         (0)      720 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-core/bagua-opentelemetry/src/lib.rs
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-net/
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-net/.gitignore
--rw-r--r--   0 root         (0) root         (0)    47812 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-net/Cargo.lock
--rw-r--r--   0 root         (0) root         (0)      873 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-net/Cargo.toml
--rw-r--r--   0 root         (0) root         (0)     2792 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-net/README.md
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-net/cbindgen.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-net/cc/
--rw-r--r--   0 root         (0) root         (0)      617 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-net/cc/Makefile
--rw-r--r--   0 root         (0) root         (0)     4307 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-net/cc/bagua_net.cc
--rw-r--r--   0 root         (0) root         (0)     3652 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-net/cc/bagua_net.h
--rw-r--r--   0 root         (0) root         (0)     2013 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-net/cc/nccl_types.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-net/cc/v3/
--rw-r--r--   0 root         (0) root         (0)     6979 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-net/cc/v3/nccl_net_v3.cc
--rw-r--r--   0 root         (0) root         (0)     5237 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-net/cc/v3/nccl_net_v3.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-net/cc/v4/
--rw-r--r--   0 root         (0) root         (0)     6974 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-net/cc/v4/nccl_net_v4.cc
--rw-r--r--   0 root         (0) root         (0)     5293 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-net/cc/v4/nccl_net_v4.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-net/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/rust/bagua-net/src/implement/
--rw-r--r--   0 root         (0) root         (0)       59 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-net/src/implement/mod.rs
--rw-r--r--   0 root         (0) root         (0)    24303 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-net/src/implement/nthread_per_socket_backend.rs
--rw-r--r--   0 root         (0) root         (0)    26153 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-net/src/implement/tokio_backend.rs
--rw-r--r--   0 root         (0) root         (0)     1991 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-net/src/interface.rs
--rw-r--r--   0 root         (0) root         (0)     9189 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-net/src/lib.rs
--rw-r--r--   0 root         (0) root         (0)    10872 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/rust/bagua-net/src/utils.rs
--rw-r--r--   0 root         (0) root         (0)       63 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4329 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/tests/
--rw-r--r--   0 root         (0) root         (0)      353 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/tests/comm/
--rw-r--r--   0 root         (0) root         (0)     7695 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/comm/test_communicator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/tests/contrib/
--rw-r--r--   0 root         (0) root         (0)     1710 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/contrib/test_cached_dataset.py
--rw-r--r--   0 root         (0) root         (0)    16758 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/contrib/test_fused_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     2258 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/contrib/test_load_balancing_data_loader.py
--rw-r--r--   0 root         (0) root         (0)     2487 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/contrib/test_store.py
--rw-r--r--   0 root         (0) root         (0)     7260 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/contrib/test_sync_bn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/tests/internal/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/internal/__init__.py
--rw-r--r--   0 root         (0) root         (0)      328 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/internal/common_utils.py
--rw-r--r--   0 root         (0) root         (0)     1368 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/internal/compressor.py
--rw-r--r--   0 root         (0) root         (0)     1568 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/internal/multi_process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/tests/internal/torch/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/internal/torch/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19031 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/internal/torch/_core.py
--rw-r--r--   0 root         (0) root         (0)     9668 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/internal/torch/common_cuda.py
--rw-r--r--   0 root         (0) root         (0)    28169 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/internal/torch/common_distributed.py
--rw-r--r--   0 root         (0) root         (0)   103561 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/internal/torch/common_utils.py
--rw-r--r--   0 root         (0) root         (0)    13117 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/internal/torch/expecttest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/tests/pytorch_lightning/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/pytorch_lightning/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5803 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/pytorch_lightning/boring_model.py
--rw-r--r--   0 root         (0) root         (0)     3013 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/pytorch_lightning/test_bagua_strategy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/tests/service/
--rw-r--r--   0 root         (0) root         (0)    12336 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/service/test_autotune_service.py
--rw-r--r--   0 root         (0) root         (0)     1180 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/service/test_bayesian_optimizer.py
--rw-r--r--   0 root         (0) root         (0)      764 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/test_bagua_define.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/tests/torch_api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 10:00:42.000000 bagua-0.9.3.dev4/tests/torch_api/data_parallel/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/torch_api/data_parallel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4178 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/torch_api/data_parallel/test_async_model_average.py
--rw-r--r--   0 root         (0) root         (0)     4645 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/torch_api/data_parallel/test_bagua_ddp.py
--rw-r--r--   0 root         (0) root         (0)     6109 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/torch_api/data_parallel/test_bagua_module.py
--rw-r--r--   0 root         (0) root         (0)     7880 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/torch_api/data_parallel/test_broadcast_state.py
--rw-r--r--   0 root         (0) root         (0)    38585 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/torch_api/data_parallel/test_c10d_common.py
--rw-r--r--   0 root         (0) root         (0)    13349 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/torch_api/data_parallel/test_decentralized.py
--rw-r--r--   0 root         (0) root         (0)     3761 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/torch_api/data_parallel/test_gradient_allreduce.py
--rw-r--r--   0 root         (0) root         (0)    13542 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/torch_api/data_parallel/test_low_precision_decentralized.py
--rw-r--r--   0 root         (0) root         (0)     8782 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/torch_api/data_parallel/test_multi_models.py
--rw-r--r--   0 root         (0) root         (0)     4160 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/torch_api/test_async_model_average.py
--rw-r--r--   0 root         (0) root         (0)     5972 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/torch_api/test_bagua_module.py
--rw-r--r--   0 root         (0) root         (0)     7824 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/torch_api/test_broadcast_state.py
--rw-r--r--   0 root         (0) root         (0)    13237 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/torch_api/test_decentralized.py
--rw-r--r--   0 root         (0) root         (0)     3665 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/torch_api/test_gradient_allreduce.py
--rw-r--r--   0 root         (0) root         (0)    13446 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/torch_api/test_low_precision_decentralized.py
--rw-r--r--   0 root         (0) root         (0)     8679 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/torch_api/test_multi_models.py
--rw-r--r--   0 root         (0) root         (0)     4172 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/torch_api/test_process_group.py
--rw-r--r--   0 root         (0) root         (0)     1413 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/torch_api/test_qadam.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-04-15 10:00:33.000000 bagua-0.9.3.dev4/tests/torch_api/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/.buildkite/
+-rw-r--r--   0 root         (0) root         (0)     1715 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/.buildkite/pipeline.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/.buildkite/scripts/
+-rw-r--r--   0 root         (0) root         (0)      970 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/.buildkite/scripts/benchmark.sh
+-rw-r--r--   0 root         (0) root         (0)     5373 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/.buildkite/scripts/benchmark_master.sh
+-rw-r--r--   0 root         (0) root         (0)     2001 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/.buildkite/scripts/benchmark_worker.sh
+-rwxr-xr-x   0 root         (0) root         (0)      112 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/.buildkite/scripts/example.sh
+-rw-r--r--   0 root         (0) root         (0)      435 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/.buildkite/scripts/install_bagua.sh
+-rwxr-xr-x   0 root         (0) root         (0)      358 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/.buildkite/scripts/run_pytest.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/.github/
+-rw-r--r--   0 root         (0) root         (0)      748 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/.github/CODEOWNERS
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      723 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 root         (0) root         (0)      595 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 root         (0) root         (0)      708 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/.github/dependabot.yml
+-rw-r--r--   0 root         (0) root         (0)      756 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/.github/issue-close-app.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      286 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/.github/workflows/bagua-net-ci.yml
+-rw-r--r--   0 root         (0) root         (0)     4668 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/.github/workflows/bagua-pypi-publish.yml
+-rw-r--r--   0 root         (0) root         (0)      907 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/.github/workflows/bagua-python-package-check.yml
+-rw-r--r--   0 root         (0) root         (0)      482 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/.github/workflows/black.yml
+-rw-r--r--   0 root         (0) root         (0)     2558 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/.github/workflows/dockerhub.yml
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/.github/workflows/flake8.yml
+-rw-r--r--   0 root         (0) root         (0)     1159 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/.github/workflows/pytype.yml
+-rw-r--r--   0 root         (0) root         (0)      535 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/.github/workflows/rustfmt.yml
+-rw-r--r--   0 root         (0) root         (0)      246 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      200 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/.gitmodules
+-rw-r--r--   0 root         (0) root         (0)    11029 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1087 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     1087 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      805 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      637 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/Makefile
+-rw-r--r--   0 root         (0) root         (0)    10292 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9791 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/bagua/
+-rw-r--r--   0 root         (0) root         (0)      339 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1289 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/bagua_define.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/bagua/distributed/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/distributed/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12057 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/distributed/launch.py
+-rw-r--r--   0 root         (0) root         (0)    24025 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/distributed/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/bagua/script/
+-rw-r--r--   0 root         (0) root         (0)       37 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/script/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4533 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/script/bagua_sys_perf
+-rw-r--r--   0 root         (0) root         (0)     7437 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/script/baguarun.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/bagua/service/
+-rw-r--r--   0 root         (0) root         (0)       76 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/service/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15639 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/service/autotune_service.py
+-rw-r--r--   0 root         (0) root         (0)     4775 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/service/autotune_system.py
+-rw-r--r--   0 root         (0) root         (0)     5726 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/service/autotune_task_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/service/bayesian_optimizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/bagua/torch_api/
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/bagua/torch_api/algorithms/
+-rw-r--r--   0 root         (0) root         (0)     1101 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/algorithms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13830 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/algorithms/async_model_average.py
+-rw-r--r--   0 root         (0) root         (0)     9202 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/algorithms/base.py
+-rw-r--r--   0 root         (0) root         (0)     2795 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/algorithms/bytegrad.py
+-rw-r--r--   0 root         (0) root         (0)    10572 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/algorithms/decentralized.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/algorithms/gradient_allreduce.py
+-rw-r--r--   0 root         (0) root         (0)     9992 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/algorithms/q_adam.py
+-rw-r--r--   0 root         (0) root         (0)    16103 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/bucket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/bagua/torch_api/checkpoint/
+-rw-r--r--   0 root         (0) root         (0)      114 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/checkpoint/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12238 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/checkpoint/checkpointing.py
+-rw-r--r--   0 root         (0) root         (0)    46828 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/communication.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/bagua/torch_api/contrib/
+-rw-r--r--   0 root         (0) root         (0)      302 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/contrib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4737 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/contrib/cache_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2582 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/contrib/cached_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/bagua/torch_api/contrib/fuse/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/contrib/fuse/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20240 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/contrib/fuse/optimizer.py
+-rw-r--r--   0 root         (0) root         (0)    13250 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/contrib/load_balancing_data_loader.py
+-rw-r--r--   0 root         (0) root         (0)    10981 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/contrib/sync_batchnorm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/bagua/torch_api/contrib/utils/
+-rw-r--r--   0 root         (0) root         (0)       35 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/contrib/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7057 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/contrib/utils/redis_store.py
+-rw-r--r--   0 root         (0) root         (0)     4140 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/contrib/utils/store.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/bagua/torch_api/data_parallel/
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/data_parallel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20686 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/data_parallel/bagua_distributed.py
+-rw-r--r--   0 root         (0) root         (0)    15123 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/data_parallel/distributed.py
+-rw-r--r--   0 root         (0) root         (0)     2253 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/data_parallel/functional.py
+-rw-r--r--   0 root         (0) root         (0)     5570 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/distributed.py
+-rw-r--r--   0 root         (0) root         (0)     3292 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/env.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/bagua/torch_api/model_parallel/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/model_parallel/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/bagua/torch_api/model_parallel/moe/
+-rw-r--r--   0 root         (0) root         (0)       83 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/model_parallel/moe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/model_parallel/moe/experts.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/model_parallel/moe/layer.py
+-rw-r--r--   0 root         (0) root         (0)    13628 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/model_parallel/moe/sharded_moe.py
+-rw-r--r--   0 root         (0) root         (0)      149 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/model_parallel/moe/utils.py
+-rw-r--r--   0 root         (0) root         (0)    11765 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     7731 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua/torch_api/utils.py
+-rw-r--r--   0 root         (0) root         (0)       27 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/bagua/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/bagua.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10292 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/bagua.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    36352 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/bagua.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/bagua.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/bagua.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/bagua.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      254 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/bagua.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/bagua.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/bagua_core/
+-rw-r--r--   0 root         (0) root         (0)      181 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua_core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      262 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua_core/_environment.py
+-rw-r--r--   0 root         (0) root         (0)     4471 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/bagua_core/bagua_install_deps.py
+-rw-r--r--   0 root         (0) root         (0)     1630 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/cliff.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/docker/
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/docker/Dockerfile.manylinux-cuda102
+-rw-r--r--   0 root         (0) root         (0)     1217 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/docker/Dockerfile.manylinux-cuda111
+-rw-r--r--   0 root         (0) root         (0)     1217 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/docker/Dockerfile.manylinux-cuda113
+-rw-r--r--   0 root         (0) root         (0)     1218 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/docker/Dockerfile.manylinux-cuda115
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/docker/Dockerfile.manylinux-cuda116
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/docker/Dockerfile.manylinux-cuda117
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/docker/Dockerfile.pytorch-1.10.0-cuda11.3-cudnn8
+-rw-r--r--   0 root         (0) root         (0)     2962 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/docker/Dockerfile.pytorch-1.11.0-cuda11.3-cudnn8
+-rw-r--r--   0 root         (0) root         (0)     2840 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/docker/Dockerfile.pytorch-1.12.0-cuda11.3-cudnn8
+-rw-r--r--   0 root         (0) root         (0)     2840 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/docker/Dockerfile.pytorch-1.13.0-cuda11.6-cudnn8
+-rw-r--r--   0 root         (0) root         (0)     2698 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/docker/Dockerfile.pytorch-1.9.0-cuda10.2-cudnn7
+-rw-r--r--   0 root         (0) root         (0)     2698 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/docker/Dockerfile.pytorch-1.9.0-cuda11.1-cudnn8
+-rw-r--r--   0 root         (0) root         (0)     2839 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/docker/Dockerfile.pytorch-2.0.0-cuda11.7-cudnn8
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/docs/_autoapi_templates/
+-rw-r--r--   0 root         (0) root         (0)      673 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/docs/_autoapi_templates/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/docs/_autoapi_templates/python/
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/docs/_autoapi_templates/python/attribute.rst
+-rw-r--r--   0 root         (0) root         (0)     2008 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/docs/_autoapi_templates/python/class.rst
+-rw-r--r--   0 root         (0) root         (0)      765 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/docs/_autoapi_templates/python/data.rst
+-rw-r--r--   0 root         (0) root         (0)       33 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/docs/_autoapi_templates/python/exception.rst
+-rw-r--r--   0 root         (0) root         (0)      594 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/docs/_autoapi_templates/python/function.rst
+-rw-r--r--   0 root         (0) root         (0)      847 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/docs/_autoapi_templates/python/method.rst
+-rw-r--r--   0 root         (0) root         (0)     2454 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/docs/_autoapi_templates/python/module.rst
+-rw-r--r--   0 root         (0) root         (0)       34 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/docs/_autoapi_templates/python/package.rst
+-rw-r--r--   0 root         (0) root         (0)     7076 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)       70 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/docs/doc-requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      673 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/docs/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/examples/
+-rw-r--r--   0 root         (0) root         (0)     1089 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/examples/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      189 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/examples/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/examples/benchmark/
+-rw-r--r--   0 root         (0) root         (0)      338 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/examples/benchmark/README.md
+-rw-r--r--   0 root         (0) root         (0)       35 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/examples/benchmark/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     6520 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/examples/benchmark/synthetic_benchmark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/examples/communication_primitives/
+-rw-r--r--   0 root         (0) root         (0)      235 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/examples/communication_primitives/README.md
+-rw-r--r--   0 root         (0) root         (0)     6662 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/examples/communication_primitives/main.py
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/examples/communication_primitives/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/examples/elastic_training/
+-rw-r--r--   0 root         (0) root         (0)      412 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/examples/elastic_training/README.md
+-rw-r--r--   0 root         (0) root         (0)     8178 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/examples/elastic_training/main.py
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/examples/elastic_training/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/examples/imagenet/
+-rw-r--r--   0 root         (0) root         (0)     1382 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/examples/imagenet/README.md
+-rw-r--r--   0 root         (0) root         (0)    17552 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/examples/imagenet/main.py
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/examples/imagenet/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/examples/mnist/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/examples/mnist/README.md
+-rw-r--r--   0 root         (0) root         (0)     8644 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/examples/mnist/main.py
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/examples/mnist/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/examples/moe/
+-rw-r--r--   0 root         (0) root         (0)      199 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/examples/moe/README.md
+-rw-r--r--   0 root         (0) root         (0)     8884 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/examples/moe/mnist_main.py
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/examples/moe/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/examples/squad/
+-rw-r--r--   0 root         (0) root         (0)      958 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/examples/squad/README.md
+-rw-r--r--   0 root         (0) root         (0)    41793 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/examples/squad/main.py
+-rw-r--r--   0 root         (0) root         (0)       56 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/examples/squad/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/figures/
+-rw-r--r--   0 root         (0) root         (0)    14450 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/figures/logo.png
+-rw-r--r--   0 root         (0) root         (0)     3036 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/install.sh
+-rw-r--r--   0 root         (0) root         (0)     4374 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/install_master.sh
+-rw-r--r--   0 root         (0) root         (0)      334 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/
+-rw-r--r--   0 root         (0) root         (0)      109 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/.gitignore
+-rw-r--r--   0 root         (0) root         (0)    67240 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/Cargo.lock
+-rw-r--r--   0 root         (0) root         (0)      139 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/Cargo.toml
+-rw-r--r--   0 root         (0) root         (0)      188 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-c/
+-rw-r--r--   0 root         (0) root         (0)      730 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-c/Cargo.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-c/src/
+-rw-r--r--   0 root         (0) root         (0)     8640 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-c/src/lib.rs
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/Cargo.toml
+-rw-r--r--   0 root         (0) root         (0)     4349 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/build.rs
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/cpp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/cpp/include/
+-rw-r--r--   0 root         (0) root         (0)      895 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/cpp/include/bagua_utils.h
+-rw-r--r--   0 root         (0) root         (0)    24308 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/cpp/include/dbg.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/kernels/
+-rw-r--r--   0 root         (0) root         (0)    25551 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/kernels/bagua_kernels.cu
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/comm_ops/
+-rw-r--r--   0 root         (0) root         (0)     2222 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/comm_ops/centralized_full_precision_synchronous.rs
+-rw-r--r--   0 root         (0) root         (0)     2903 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/comm_ops/centralized_low_precision_synchronous.rs
+-rw-r--r--   0 root         (0) root         (0)     7645 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/comm_ops/decentralized_full_precision_asynchronous.rs
+-rw-r--r--   0 root         (0) root         (0)     4806 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/comm_ops/decentralized_full_precision_synchronous.rs
+-rw-r--r--   0 root         (0) root         (0)     6375 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/comm_ops/decentralized_low_precision_synchronous.rs
+-rw-r--r--   0 root         (0) root         (0)      571 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/comm_ops/mod.rs
+-rw-r--r--   0 root         (0) root         (0)      665 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/comm_ops/python_ffi_op.rs
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/communicators/
+-rw-r--r--   0 root         (0) root         (0)    53076 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/communicators/mod.rs
+-rw-r--r--   0 root         (0) root         (0)      559 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/cuda_utils.rs
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/datatypes/
+-rw-r--r--   0 root         (0) root         (0)    46518 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/datatypes/mod.rs
+-rw-r--r--   0 root         (0) root         (0)      759 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/events.rs
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/kernels/
+-rw-r--r--   0 root         (0) root         (0)     3917 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/kernels/mod.rs
+-rw-r--r--   0 root         (0) root         (0)    12601 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/lib.rs
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/resource_pool/
+-rw-r--r--   0 root         (0) root         (0)     2182 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/resource_pool/mod.rs
+-rw-r--r--   0 root         (0) root         (0)    66619 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/torch_ffi.rs
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/
+-rw-r--r--   0 root         (0) root         (0)      294 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      110 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/.gitmodules
+-rw-r--r--   0 root         (0) root         (0)    15030 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      329 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/CONTRIBUTORS
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6566 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/
+-rw-r--r--   0 root         (0) root         (0)     3313 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     2282 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/benchmark_events.cpp
+-rw-r--r--   0 root         (0) root         (0)     9764 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/benchmark_ops.cpp
+-rw-r--r--   0 root         (0) root         (0)     8731 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/benchmark_utils.hpp
+-rw-r--r--   0 root         (0) root         (0)     2297 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/benchmark_utils_ht.hpp
+-rw-r--r--   0 root         (0) root         (0)     1587 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/benchmark_utils_mpi.hpp
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/benchmark_utils_nccl.hpp
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/benchmark_waits.cpp
+-rw-r--r--   0 root         (0) root         (0)    12693 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/plot_benchmarks.py
+-rw-r--r--   0 root         (0) root         (0)     9566 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/run_benchmarks.py
+-rw-r--r--   0 root         (0) root         (0)     2244 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/wait.cu
+-rw-r--r--   0 root         (0) root         (0)     1412 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/wait.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/
+-rw-r--r--   0 root         (0) root         (0)      587 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/Al_config.hpp.in
+-rw-r--r--   0 root         (0) root         (0)     2265 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/AluminumConfig.cmake.in
+-rw-r--r--   0 root         (0) root         (0)     1335 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/FindCUB.cmake
+-rw-r--r--   0 root         (0) root         (0)     1625 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/FindHWLOC.cmake
+-rw-r--r--   0 root         (0) root         (0)     2190 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/FindNCCL.cmake
+-rw-r--r--   0 root         (0) root         (0)      755 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/FindNVTX.cmake
+-rw-r--r--   0 root         (0) root         (0)     2002 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/HipBuildSystem.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/
+-rw-r--r--   0 root         (0) root         (0)    47921 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/Al.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     2505 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/base.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/
+-rw-r--r--   0 root         (0) root         (0)      232 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     6578 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/cuda.hpp
+-rw-r--r--   0 root         (0) root         (0)     2536 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/cuda_mempool.hpp
+-rw-r--r--   0 root         (0) root         (0)     2025 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/events.hpp
+-rw-r--r--   0 root         (0) root         (0)     2423 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/gpu_status_flag.hpp
+-rw-r--r--   0 root         (0) root         (0)     2320 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/gpu_wait.hpp
+-rw-r--r--   0 root         (0) root         (0)     1778 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/helper_kernels.hpp
+-rw-r--r--   0 root         (0) root         (0)     3080 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/streams.hpp
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/sync_memory.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/
+-rw-r--r--   0 root         (0) root         (0)      395 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     3258 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/allgather.hpp
+-rw-r--r--   0 root         (0) root         (0)     3581 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/allgatherv.hpp
+-rw-r--r--   0 root         (0) root         (0)     3094 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/allreduce.hpp
+-rw-r--r--   0 root         (0) root         (0)     2862 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/alltoall.hpp
+-rw-r--r--   0 root         (0) root         (0)     4941 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/alltoallv.hpp
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/barrier.hpp
+-rw-r--r--   0 root         (0) root         (0)     6031 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/base_state.hpp
+-rw-r--r--   0 root         (0) root         (0)     2864 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/bcast.hpp
+-rw-r--r--   0 root         (0) root         (0)     2618 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/communicator.hpp
+-rw-r--r--   0 root         (0) root         (0)     3485 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/gather.hpp
+-rw-r--r--   0 root         (0) root         (0)     4058 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/gatherv.hpp
+-rw-r--r--   0 root         (0) root         (0)     7427 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/pt2pt.hpp
+-rw-r--r--   0 root         (0) root         (0)     3137 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/reduce.hpp
+-rw-r--r--   0 root         (0) root         (0)     2979 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/reduce_scatter.hpp
+-rw-r--r--   0 root         (0) root         (0)     3179 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/reduce_scatterv.hpp
+-rw-r--r--   0 root         (0) root         (0)     3772 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/scatter.hpp
+-rw-r--r--   0 root         (0) root         (0)     4362 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/scatterv.hpp
+-rw-r--r--   0 root         (0) root         (0)    36227 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht_impl.hpp
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/internal.hpp
+-rw-r--r--   0 root         (0) root         (0)     4552 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mempool.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/
+-rw-r--r--   0 root         (0) root         (0)      461 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     2861 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/allgather.hpp
+-rw-r--r--   0 root         (0) root         (0)     3535 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/allgatherv.hpp
+-rw-r--r--   0 root         (0) root         (0)    42883 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/allreduce.hpp
+-rw-r--r--   0 root         (0) root         (0)     2847 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/alltoall.hpp
+-rw-r--r--   0 root         (0) root         (0)     4479 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/alltoallv.hpp
+-rw-r--r--   0 root         (0) root         (0)     2240 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/barrier.hpp
+-rw-r--r--   0 root         (0) root         (0)     2151 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/base_state.hpp
+-rw-r--r--   0 root         (0) root         (0)     2617 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/bcast.hpp
+-rw-r--r--   0 root         (0) root         (0)     3067 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/communicator.hpp
+-rw-r--r--   0 root         (0) root         (0)     3221 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/gather.hpp
+-rw-r--r--   0 root         (0) root         (0)     3889 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/gatherv.hpp
+-rw-r--r--   0 root         (0) root         (0)     6043 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/pt2pt.hpp
+-rw-r--r--   0 root         (0) root         (0)     3363 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/reduce.hpp
+-rw-r--r--   0 root         (0) root         (0)     3153 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/reduce_scatter.hpp
+-rw-r--r--   0 root         (0) root         (0)     3480 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/reduce_scatterv.hpp
+-rw-r--r--   0 root         (0) root         (0)     3313 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/scatter.hpp
+-rw-r--r--   0 root         (0) root         (0)     3952 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/scatterv.hpp
+-rw-r--r--   0 root         (0) root         (0)     8509 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/utils.hpp
+-rw-r--r--   0 root         (0) root         (0)     4533 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_comm_and_stream_wrapper.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda/
+-rw-r--r--   0 root         (0) root         (0)      358 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     2396 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda/communicator.hpp
+-rw-r--r--   0 root         (0) root         (0)     5473 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda/rma.hpp
+-rw-r--r--   0 root         (0) root         (0)    10021 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda/rma_ipc.hpp
+-rw-r--r--   0 root         (0) root         (0)     2115 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda/rma_null.hpp
+-rw-r--r--   0 root         (0) root         (0)     2467 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda/rma_self.hpp
+-rw-r--r--   0 root         (0) root         (0)     4933 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda/util.hpp
+-rw-r--r--   0 root         (0) root         (0)     4129 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda_impl.hpp
+-rw-r--r--   0 root         (0) root         (0)    32186 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_impl.hpp
+-rw-r--r--   0 root         (0) root         (0)    51540 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/nccl_impl.hpp
+-rw-r--r--   0 root         (0) root         (0)     2232 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/profiling.hpp
+-rw-r--r--   0 root         (0) root         (0)     5988 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/progress.hpp
+-rw-r--r--   0 root         (0) root         (0)     5096 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/state.hpp
+-rw-r--r--   0 root         (0) root         (0)     3203 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/trace.hpp
+-rw-r--r--   0 root         (0) root         (0)     3055 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/tuning_params.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/utils/
+-rw-r--r--   0 root         (0) root         (0)      291 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     7761 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/utils/caching_allocator.hpp
+-rw-r--r--   0 root         (0) root         (0)     3210 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/utils/locked_resource_pool.hpp
+-rw-r--r--   0 root         (0) root         (0)     3587 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/utils/meta.hpp
+-rw-r--r--   0 root         (0) root         (0)     5256 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/utils/mpsc_queue.hpp
+-rw-r--r--   0 root         (0) root         (0)     4251 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/utils/spsc_queue.hpp
+-rw-r--r--   0 root         (0) root         (0)     1883 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/utils/utils.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/
+-rw-r--r--   0 root         (0) root         (0)     5002 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/Al.cpp
+-rw-r--r--   0 root         (0) root         (0)     3123 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/cuda/
+-rw-r--r--   0 root         (0) root         (0)      414 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/cuda/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     2683 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/cuda/cuda.cpp
+-rw-r--r--   0 root         (0) root         (0)     3163 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/cuda/gpu_status_flag.cpp
+-rw-r--r--   0 root         (0) root         (0)     2493 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/cuda/gpu_wait.cpp
+-rw-r--r--   0 root         (0) root         (0)     2109 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/cuda/helper_kernels.cu
+-rw-r--r--   0 root         (0) root         (0)     3928 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/cuda/streams.cpp
+-rw-r--r--   0 root         (0) root         (0)     1744 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/ht_impl.cpp
+-rw-r--r--   0 root         (0) root         (0)     1385 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/mempool.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/mpi_cuda/
+-rw-r--r--   0 root         (0) root         (0)      403 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/mpi_cuda/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1706 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/mpi_cuda/communicator.cpp
+-rw-r--r--   0 root         (0) root         (0)     3542 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/mpi_cuda/rma.cpp
+-rw-r--r--   0 root         (0) root         (0)     1474 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/mpi_cuda_impl.cpp
+-rw-r--r--   0 root         (0) root         (0)     2522 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/mpi_impl.cpp
+-rw-r--r--   0 root         (0) root         (0)     2864 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/nccl_impl.cpp
+-rw-r--r--   0 root         (0) root         (0)     2219 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/profiling.cpp
+-rw-r--r--   0 root         (0) root         (0)    20918 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/progress.cpp
+-rw-r--r--   0 root         (0) root         (0)     2830 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/trace.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/
+-rw-r--r--   0 root         (0) root         (0)     3286 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     4685 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/cuda_vector.hpp
+-rw-r--r--   0 root         (0) root         (0)     4017 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/hang_watchdog.hpp
+-rw-r--r--   0 root         (0) root         (0)    34118 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/op_dispatcher.hpp
+-rw-r--r--   0 root         (0) root         (0)    44646 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/op_runner_impl.hpp
+-rw-r--r--   0 root         (0) root         (0)     8572 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/run_tests.py
+-rw-r--r--   0 root         (0) root         (0)     5802 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_exchange.cpp
+-rw-r--r--   0 root         (0) root         (0)    18155 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_ops.cpp
+-rw-r--r--   0 root         (0) root         (0)     9380 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_rma_halo_exchange.cpp
+-rw-r--r--   0 root         (0) root         (0)     4467 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_rma_ring.cpp
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_stream_mem_ops.cpp
+-rw-r--r--   0 root         (0) root         (0)    12514 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_utils.hpp
+-rw-r--r--   0 root         (0) root         (0)    10487 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_utils_ht.hpp
+-rw-r--r--   0 root         (0) root         (0)     8385 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_utils_mpi.hpp
+-rw-r--r--   0 root         (0) root         (0)     2648 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_utils_mpi_cuda.hpp
+-rw-r--r--   0 root         (0) root         (0)     9815 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_utils_nccl.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/
+-rw-r--r--   0 root         (0) root         (0)      127 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/.git
+-rw-r--r--   0 root         (0) root         (0)       98 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1839 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/.travis.yml
+-rw-r--r--   0 root         (0) root         (0)     3168 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     4430 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      656 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/INSTALL
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4955 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/README.md
+-rw-r--r--   0 root         (0) root         (0)      114 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/cxxopts-config.cmake.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/include/
+-rw-r--r--   0 root         (0) root         (0)    42643 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/include/cxxopts.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/src/
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/src/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1212 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/src/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     4831 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/src/example.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1359 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/add-subdirectory-test/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/add-subdirectory-test/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)   377366 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/catch.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/find-package-test/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/find-package-test/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/link_a.cpp
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/link_b.cpp
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/main.cpp
+-rw-r--r--   0 root         (0) root         (0)    18892 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/options.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/
+-rw-r--r--   0 root         (0) root         (0)    65123 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/.cproject
+-rw-r--r--   0 root         (0) root         (0)      835 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/.project
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/.settings/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/.settings/.gitignore
+-rw-r--r--   0 root         (0) root         (0)    10954 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/.settings/org.eclipse.cdt.codan.core.prefs
+-rw-r--r--   0 root         (0) root         (0)    14273 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/.settings/org.eclipse.cdt.core.prefs
+-rw-r--r--   0 root         (0) root         (0)       86 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/.settings/org.eclipse.cdt.ui.prefs
+-rw-r--r--   0 root         (0) root         (0)      190 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/.settings/org.eclipse.core.runtime.prefs
+-rw-r--r--   0 root         (0) root         (0)    22309 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/CHANGE_LOG.TXT
+-rw-r--r--   0 root         (0) root         (0)     1600 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/LICENSE.TXT
+-rw-r--r--   0 root         (0) root         (0)     6051 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     7688 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/common.mk
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/
+-rw-r--r--   0 root         (0) root         (0)    33331 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_histogram.cuh
+-rw-r--r--   0 root         (0) root         (0)    28525 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_radix_sort_downsweep.cuh
+-rw-r--r--   0 root         (0) root         (0)    17917 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_radix_sort_upsweep.cuh
+-rw-r--r--   0 root         (0) root         (0)    16916 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_reduce.cuh
+-rw-r--r--   0 root         (0) root         (0)    24791 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_reduce_by_key.cuh
+-rw-r--r--   0 root         (0) root         (0)    35663 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_rle.cuh
+-rw-r--r--   0 root         (0) root         (0)    18729 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_scan.cuh
+-rw-r--r--   0 root         (0) root         (0)    16655 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_segment_fixup.cuh
+-rw-r--r--   0 root         (0) root         (0)    29594 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_select_if.cuh
+-rw-r--r--   0 root         (0) root         (0)    27377 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_spmv_orig.cuh
+-rw-r--r--   0 root         (0) root         (0)    27444 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/single_pass_scan_operators.cuh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/
+-rw-r--r--   0 root         (0) root         (0)    25011 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_adjacent_difference.cuh
+-rw-r--r--   0 root         (0) root         (0)    54550 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_discontinuity.cuh
+-rw-r--r--   0 root         (0) root         (0)    52305 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_exchange.cuh
+-rw-r--r--   0 root         (0) root         (0)    16291 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_histogram.cuh
+-rw-r--r--   0 root         (0) root         (0)    53671 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_load.cuh
+-rw-r--r--   0 root         (0) root         (0)    25230 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_radix_rank.cuh
+-rw-r--r--   0 root         (0) root         (0)    38342 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_radix_sort.cuh
+-rw-r--r--   0 root         (0) root         (0)     6181 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_raking_layout.cuh
+-rw-r--r--   0 root         (0) root         (0)    25300 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_reduce.cuh
+-rw-r--r--   0 root         (0) root         (0)   102978 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_scan.cuh
+-rw-r--r--   0 root         (0) root         (0)    11964 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_shuffle.cuh
+-rw-r--r--   0 root         (0) root         (0)    41449 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_store.cuh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/
+-rw-r--r--   0 root         (0) root         (0)     3285 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_histogram_atomic.cuh
+-rw-r--r--   0 root         (0) root         (0)     8198 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_histogram_sort.cuh
+-rw-r--r--   0 root         (0) root         (0)     9731 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_reduce_raking.cuh
+-rw-r--r--   0 root         (0) root         (0)     8369 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_reduce_raking_commutative_only.cuh
+-rw-r--r--   0 root         (0) root         (0)     9769 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_reduce_warp_reductions.cuh
+-rw-r--r--   0 root         (0) root         (0)    28460 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_scan_raking.cuh
+-rw-r--r--   0 root         (0) root         (0)    19117 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_scan_warp_scans.cuh
+-rw-r--r--   0 root         (0) root         (0)    20949 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_scan_warp_scans2.cuh
+-rw-r--r--   0 root         (0) root         (0)    19463 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_scan_warp_scans3.cuh
+-rw-r--r--   0 root         (0) root         (0)     3626 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/cub.cuh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/
+-rw-r--r--   0 root         (0) root         (0)    54347 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_histogram.cuh
+-rw-r--r--   0 root         (0) root         (0)    13891 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_partition.cuh
+-rw-r--r--   0 root         (0) root         (0)    42384 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_radix_sort.cuh
+-rw-r--r--   0 root         (0) root         (0)    38904 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_reduce.cuh
+-rw-r--r--   0 root         (0) root         (0)    14817 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_run_length_encode.cuh
+-rw-r--r--   0 root         (0) root         (0)    21786 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_scan.cuh
+-rw-r--r--   0 root         (0) root         (0)    54689 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_segmented_radix_sort.cuh
+-rw-r--r--   0 root         (0) root         (0)    36523 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_segmented_reduce.cuh
+-rw-r--r--   0 root         (0) root         (0)    18838 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_select.cuh
+-rw-r--r--   0 root         (0) root         (0)     8523 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_spmv.cuh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/
+-rw-r--r--   0 root         (0) root         (0)    57226 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_histogram.cuh
+-rw-r--r--   0 root         (0) root         (0)    80406 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_radix_sort.cuh
+-rw-r--r--   0 root         (0) root         (0)    42707 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_reduce.cuh
+-rw-r--r--   0 root         (0) root         (0)    25478 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_reduce_by_key.cuh
+-rw-r--r--   0 root         (0) root         (0)    23601 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_rle.cuh
+-rw-r--r--   0 root         (0) root         (0)    22778 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_scan.cuh
+-rw-r--r--   0 root         (0) root         (0)    24454 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_select_if.cuh
+-rw-r--r--   0 root         (0) root         (0)    33269 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_spmv_orig.cuh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/grid/
+-rw-r--r--   0 root         (0) root         (0)     5861 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/grid/grid_barrier.cuh
+-rw-r--r--   0 root         (0) root         (0)     8198 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/grid/grid_even_share.cuh
+-rw-r--r--   0 root         (0) root         (0)     4827 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/grid/grid_mapping.cuh
+-rw-r--r--   0 root         (0) root         (0)     7475 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/grid/grid_queue.cuh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/host/
+-rw-r--r--   0 root         (0) root         (0)     4581 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/host/mutex.cuh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/
+-rw-r--r--   0 root         (0) root         (0)     8781 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/arg_index_input_iterator.cuh
+-rw-r--r--   0 root         (0) root         (0)     8104 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/cache_modified_input_iterator.cuh
+-rw-r--r--   0 root         (0) root         (0)     8322 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/cache_modified_output_iterator.cuh
+-rw-r--r--   0 root         (0) root         (0)     7650 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/constant_input_iterator.cuh
+-rw-r--r--   0 root         (0) root         (0)     7369 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/counting_input_iterator.cuh
+-rw-r--r--   0 root         (0) root         (0)     6817 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/discard_output_iterator.cuh
+-rw-r--r--   0 root         (0) root         (0)    10546 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/tex_obj_input_iterator.cuh
+-rw-r--r--   0 root         (0) root         (0)    12430 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/tex_ref_input_iterator.cuh
+-rw-r--r--   0 root         (0) root         (0)     8611 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/transform_input_iterator.cuh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/thread/
+-rw-r--r--   0 root         (0) root         (0)    18869 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/thread/thread_load.cuh
+-rw-r--r--   0 root         (0) root         (0)     9228 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/thread/thread_operators.cuh
+-rw-r--r--   0 root         (0) root         (0)     6037 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/thread/thread_reduce.cuh
+-rw-r--r--   0 root         (0) root         (0)    10566 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/thread/thread_scan.cuh
+-rw-r--r--   0 root         (0) root         (0)     4797 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/thread/thread_search.cuh
+-rw-r--r--   0 root         (0) root         (0)    17932 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/thread/thread_store.cuh
+-rw-r--r--   0 root         (0) root         (0)    28716 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_allocator.cuh
+-rw-r--r--   0 root         (0) root         (0)     6955 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_arch.cuh
+-rw-r--r--   0 root         (0) root         (0)     5061 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_debug.cuh
+-rw-r--r--   0 root         (0) root         (0)    10658 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_device.cuh
+-rw-r--r--   0 root         (0) root         (0)     3710 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_macro.cuh
+-rw-r--r--   0 root         (0) root         (0)     2100 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_namespace.cuh
+-rw-r--r--   0 root         (0) root         (0)    22318 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_ptx.cuh
+-rw-r--r--   0 root         (0) root         (0)    40178 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_type.cuh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/warp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/warp/specializations/
+-rw-r--r--   0 root         (0) root         (0)    21412 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/warp/specializations/warp_reduce_shfl.cuh
+-rw-r--r--   0 root         (0) root         (0)    14280 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/warp/specializations/warp_reduce_smem.cuh
+-rw-r--r--   0 root         (0) root         (0)    25284 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/warp/specializations/warp_scan_shfl.cuh
+-rw-r--r--   0 root         (0) root         (0)    16153 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/warp/specializations/warp_scan_smem.cuh
+-rw-r--r--   0 root         (0) root         (0)    25032 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/warp/warp_reduce.cuh
+-rw-r--r--   0 root         (0) root         (0)    38915 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/warp/warp_scan.cuh
+-rw-r--r--   0 root         (0) root         (0)    16543 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/eclipse code style profile.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/block/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/block/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     5255 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/block/Makefile
+-rw-r--r--   0 root         (0) root         (0)    10724 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/block/example_block_radix_sort.cu
+-rw-r--r--   0 root         (0) root         (0)     9644 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/block/example_block_reduce.cu
+-rw-r--r--   0 root         (0) root         (0)    11329 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/block/example_block_scan.cu
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/block/reduce_by_key.cu
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     8830 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/Makefile
+-rw-r--r--   0 root         (0) root         (0)     8173 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_partition_flagged.cu
+-rw-r--r--   0 root         (0) root         (0)     8236 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_partition_if.cu
+-rw-r--r--   0 root         (0) root         (0)     8303 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_radix_sort.cu
+-rw-r--r--   0 root         (0) root         (0)     5825 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_reduce.cu
+-rw-r--r--   0 root         (0) root         (0)     6007 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_scan.cu
+-rw-r--r--   0 root         (0) root         (0)     8156 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_select_flagged.cu
+-rw-r--r--   0 root         (0) root         (0)     8210 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_select_if.cu
+-rw-r--r--   0 root         (0) root         (0)     7493 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_select_unique.cu
+-rw-r--r--   0 root         (0) root         (0)    13277 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_sort_find_non_trivial_runs.cu
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     4949 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/defunct/
+-rw-r--r--   0 root         (0) root         (0)    37185 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/defunct/example_coo_spmv.cu
+-rw-r--r--   0 root         (0) root         (0)    95317 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/defunct/test_device_seg_reduce.cu
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/histogram/
+-rw-r--r--   0 root         (0) root         (0)     4374 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/histogram/histogram_cub.h
+-rw-r--r--   0 root         (0) root         (0)     6368 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/histogram/histogram_gmem_atomics.h
+-rw-r--r--   0 root         (0) root         (0)     6812 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/histogram/histogram_smem_atomics.h
+-rw-r--r--   0 root         (0) root         (0)    21778 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/histogram_compare.cu
+-rw-r--r--   0 root         (0) root         (0)    39231 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/sparse_matrix.h
+-rw-r--r--   0 root         (0) root         (0)    30656 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/spmv_compare.cu
+-rwxr-xr-x   0 root         (0) root         (0)      749 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/spmv_script.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/.gitignore
+-rw-r--r--   0 root         (0) root         (0)    18927 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/Makefile
+-rw-r--r--   0 root         (0) root         (0)     8397 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/half.h
+-rw-r--r--   0 root         (0) root         (0)      315 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/link_a.cu
+-rw-r--r--   0 root         (0) root         (0)      315 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/link_b.cu
+-rw-r--r--   0 root         (0) root         (0)      113 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/link_main.cpp
+-rw-r--r--   0 root         (0) root         (0)     5148 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/mersenne.h
+-rw-r--r--   0 root         (0) root         (0)    16564 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_allocator.cu
+-rw-r--r--   0 root         (0) root         (0)     9623 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_block_histogram.cu
+-rw-r--r--   0 root         (0) root         (0)    19496 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_block_load_store.cu
+-rw-r--r--   0 root         (0) root         (0)    25392 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_block_radix_sort.cu
+-rw-r--r--   0 root         (0) root         (0)    26628 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_block_reduce.cu
+-rw-r--r--   0 root         (0) root         (0)    34810 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_block_scan.cu
+-rw-r--r--   0 root         (0) root         (0)    70313 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_histogram.cu
+-rw-r--r--   0 root         (0) root         (0)    46469 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_radix_sort.cu
+-rw-r--r--   0 root         (0) root         (0)    49902 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_reduce.cu
+-rw-r--r--   0 root         (0) root         (0)    30363 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_reduce_by_key.cu
+-rw-r--r--   0 root         (0) root         (0)    31192 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_run_length_encode.cu
+-rw-r--r--   0 root         (0) root         (0)    33600 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_scan.cu
+-rw-r--r--   0 root         (0) root         (0)    37640 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_select_if.cu
+-rw-r--r--   0 root         (0) root         (0)    21518 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_select_unique.cu
+-rw-r--r--   0 root         (0) root         (0)     5132 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_grid_barrier.cu
+-rw-r--r--   0 root         (0) root         (0)    25549 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_iterator.cu
+-rw-r--r--   0 root         (0) root         (0)    54847 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_util.h
+-rw-r--r--   0 root         (0) root         (0)    27186 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_warp_reduce.cu
+-rw-r--r--   0 root         (0) root         (0)    20350 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_warp_scan.cu
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/tune/
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/tune/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     6388 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/tune/Makefile
+-rw-r--r--   0 root         (0) root         (0)    27663 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/tune/tune_device_reduce.cu
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-py/
+-rw-r--r--   0 root         (0) root         (0)      783 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-py/Cargo.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-py/src/
+-rw-r--r--   0 root         (0) root         (0)    18099 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-core-py/src/lib.rs
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-opentelemetry/
+-rw-r--r--   0 root         (0) root         (0)      629 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-opentelemetry/Cargo.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-opentelemetry/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-opentelemetry/src/exporter/
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-opentelemetry/src/exporter/agent.rs
+-rw-r--r--   0 root         (0) root         (0)     1815 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-opentelemetry/src/exporter/mod.rs
+-rw-r--r--   0 root         (0) root         (0)      720 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-core/bagua-opentelemetry/src/lib.rs
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-net/
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-net/.gitignore
+-rw-r--r--   0 root         (0) root         (0)    47812 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-net/Cargo.lock
+-rw-r--r--   0 root         (0) root         (0)      873 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-net/Cargo.toml
+-rw-r--r--   0 root         (0) root         (0)     2792 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-net/README.md
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-net/cbindgen.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-net/cc/
+-rw-r--r--   0 root         (0) root         (0)      617 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-net/cc/Makefile
+-rw-r--r--   0 root         (0) root         (0)     4307 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-net/cc/bagua_net.cc
+-rw-r--r--   0 root         (0) root         (0)     3652 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-net/cc/bagua_net.h
+-rw-r--r--   0 root         (0) root         (0)     2013 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-net/cc/nccl_types.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-net/cc/v3/
+-rw-r--r--   0 root         (0) root         (0)     6979 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-net/cc/v3/nccl_net_v3.cc
+-rw-r--r--   0 root         (0) root         (0)     5237 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-net/cc/v3/nccl_net_v3.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-net/cc/v4/
+-rw-r--r--   0 root         (0) root         (0)     6974 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-net/cc/v4/nccl_net_v4.cc
+-rw-r--r--   0 root         (0) root         (0)     5293 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-net/cc/v4/nccl_net_v4.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-net/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/rust/bagua-net/src/implement/
+-rw-r--r--   0 root         (0) root         (0)       59 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-net/src/implement/mod.rs
+-rw-r--r--   0 root         (0) root         (0)    24303 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-net/src/implement/nthread_per_socket_backend.rs
+-rw-r--r--   0 root         (0) root         (0)    26153 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-net/src/implement/tokio_backend.rs
+-rw-r--r--   0 root         (0) root         (0)     1991 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-net/src/interface.rs
+-rw-r--r--   0 root         (0) root         (0)     9189 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-net/src/lib.rs
+-rw-r--r--   0 root         (0) root         (0)    10872 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/rust/bagua-net/src/utils.rs
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4329 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/tests/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/tests/comm/
+-rw-r--r--   0 root         (0) root         (0)     7695 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/comm/test_communicator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/tests/contrib/
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/contrib/test_cached_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    16758 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/contrib/test_fused_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     2258 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/contrib/test_load_balancing_data_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2487 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/contrib/test_store.py
+-rw-r--r--   0 root         (0) root         (0)     7260 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/contrib/test_sync_bn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/tests/internal/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/internal/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      328 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/internal/common_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1368 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/internal/compressor.py
+-rw-r--r--   0 root         (0) root         (0)     1568 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/internal/multi_process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/tests/internal/torch/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/internal/torch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19031 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/internal/torch/_core.py
+-rw-r--r--   0 root         (0) root         (0)     9668 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/internal/torch/common_cuda.py
+-rw-r--r--   0 root         (0) root         (0)    28169 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/internal/torch/common_distributed.py
+-rw-r--r--   0 root         (0) root         (0)   103561 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/internal/torch/common_utils.py
+-rw-r--r--   0 root         (0) root         (0)    13117 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/internal/torch/expecttest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/tests/pytorch_lightning/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/pytorch_lightning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5803 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/pytorch_lightning/boring_model.py
+-rw-r--r--   0 root         (0) root         (0)     3013 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/pytorch_lightning/test_bagua_strategy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/tests/service/
+-rw-r--r--   0 root         (0) root         (0)    12336 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/service/test_autotune_service.py
+-rw-r--r--   0 root         (0) root         (0)     1180 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/service/test_bayesian_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)      764 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/test_bagua_define.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/tests/torch_api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:29:13.000000 bagua-0.9.3.dev5/tests/torch_api/data_parallel/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/torch_api/data_parallel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4178 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/torch_api/data_parallel/test_async_model_average.py
+-rw-r--r--   0 root         (0) root         (0)     4645 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/torch_api/data_parallel/test_bagua_ddp.py
+-rw-r--r--   0 root         (0) root         (0)     6109 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/torch_api/data_parallel/test_bagua_module.py
+-rw-r--r--   0 root         (0) root         (0)     7880 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/torch_api/data_parallel/test_broadcast_state.py
+-rw-r--r--   0 root         (0) root         (0)    38585 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/torch_api/data_parallel/test_c10d_common.py
+-rw-r--r--   0 root         (0) root         (0)    13349 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/torch_api/data_parallel/test_decentralized.py
+-rw-r--r--   0 root         (0) root         (0)     3761 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/torch_api/data_parallel/test_gradient_allreduce.py
+-rw-r--r--   0 root         (0) root         (0)    13542 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/torch_api/data_parallel/test_low_precision_decentralized.py
+-rw-r--r--   0 root         (0) root         (0)     8782 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/torch_api/data_parallel/test_multi_models.py
+-rw-r--r--   0 root         (0) root         (0)     4160 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/torch_api/test_async_model_average.py
+-rw-r--r--   0 root         (0) root         (0)     5972 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/torch_api/test_bagua_module.py
+-rw-r--r--   0 root         (0) root         (0)     7824 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/torch_api/test_broadcast_state.py
+-rw-r--r--   0 root         (0) root         (0)    13237 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/torch_api/test_decentralized.py
+-rw-r--r--   0 root         (0) root         (0)     3665 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/torch_api/test_gradient_allreduce.py
+-rw-r--r--   0 root         (0) root         (0)    13446 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/torch_api/test_low_precision_decentralized.py
+-rw-r--r--   0 root         (0) root         (0)     8679 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/torch_api/test_multi_models.py
+-rw-r--r--   0 root         (0) root         (0)     4172 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/torch_api/test_process_group.py
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/torch_api/test_qadam.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-04-15 12:29:05.000000 bagua-0.9.3.dev5/tests/torch_api/test_utils.py
```

### Comparing `bagua-0.9.3.dev4/.buildkite/pipeline.yml` & `bagua-0.9.3.dev5/.buildkite/pipeline.yml`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/.buildkite/scripts/benchmark.sh` & `bagua-0.9.3.dev5/.buildkite/scripts/benchmark.sh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/.buildkite/scripts/benchmark_master.sh` & `bagua-0.9.3.dev5/.buildkite/scripts/benchmark_master.sh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/.buildkite/scripts/benchmark_worker.sh` & `bagua-0.9.3.dev5/.buildkite/scripts/benchmark_worker.sh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/.github/CODEOWNERS` & `bagua-0.9.3.dev5/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/.github/ISSUE_TEMPLATE/bug_report.md` & `bagua-0.9.3.dev5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/.github/ISSUE_TEMPLATE/feature_request.md` & `bagua-0.9.3.dev5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/.github/dependabot.yml` & `bagua-0.9.3.dev5/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/.github/issue-close-app.yml` & `bagua-0.9.3.dev5/.github/issue-close-app.yml`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/.github/workflows/bagua-pypi-publish.yml` & `bagua-0.9.3.dev5/.github/workflows/bagua-pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/.github/workflows/bagua-python-package-check.yml` & `bagua-0.9.3.dev5/.github/workflows/bagua-python-package-check.yml`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/.github/workflows/dockerhub.yml` & `bagua-0.9.3.dev5/.github/workflows/dockerhub.yml`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/.github/workflows/flake8.yml` & `bagua-0.9.3.dev5/.github/workflows/flake8.yml`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/.github/workflows/pytype.yml` & `bagua-0.9.3.dev5/.github/workflows/pytype.yml`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/.github/workflows/rustfmt.yml` & `bagua-0.9.3.dev5/.github/workflows/rustfmt.yml`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/CHANGELOG.md` & `bagua-0.9.3.dev5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/CONTRIBUTING.md` & `bagua-0.9.3.dev5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/LICENSE` & `bagua-0.9.3.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/MANIFEST.in` & `bagua-0.9.3.dev5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/Makefile` & `bagua-0.9.3.dev5/Makefile`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/PKG-INFO` & `bagua-0.9.3.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bagua
-Version: 0.9.3.dev4
+Version: 0.9.3.dev5
 Summary: Bagua is a deep learning training acceleration framework for PyTorch. It provides a one-stop training acceleration solution, including faster distributed training compared to PyTorch DDP, faster dataloader, kernel fusion, and more.
 Home-page: https://github.com/BaguaSys/bagua
 Author: Kuaishou AI Platform & DS3 Lab
 Author-email: admin@mail.xrlian.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bagua Version: 0.9.3.dev4 Summary: Bagua is a deep
+Metadata-Version: 2.1 Name: bagua Version: 0.9.3.dev5 Summary: Bagua is a deep
 learning training acceleration framework for PyTorch. It provides a one-stop
 training acceleration solution, including faster distributed training compared
 to PyTorch DDP, faster dataloader, kernel fusion, and more. Home-page: https://
 github.com/BaguaSys/bagua Author: Kuaishou AI Platform & DS3 Lab Author-email:
 admin@mail.xrlian.com Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE
  [https://user-images.githubusercontent.com/18649508/141055752-2f429618-2707-
```

### Comparing `bagua-0.9.3.dev4/README.md` & `bagua-0.9.3.dev5/README.md`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/bagua_define.py` & `bagua-0.9.3.dev5/bagua/bagua_define.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/distributed/launch.py` & `bagua-0.9.3.dev5/bagua/distributed/launch.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/distributed/run.py` & `bagua-0.9.3.dev5/bagua/distributed/run.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/script/bagua_sys_perf` & `bagua-0.9.3.dev5/bagua/script/bagua_sys_perf`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/script/baguarun.py` & `bagua-0.9.3.dev5/bagua/script/baguarun.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/service/autotune_service.py` & `bagua-0.9.3.dev5/bagua/service/autotune_service.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/service/autotune_system.py` & `bagua-0.9.3.dev5/bagua/service/autotune_system.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/service/autotune_task_manager.py` & `bagua-0.9.3.dev5/bagua/service/autotune_task_manager.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/service/bayesian_optimizer.py` & `bagua-0.9.3.dev5/bagua/service/bayesian_optimizer.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/torch_api/__init__.py` & `bagua-0.9.3.dev5/bagua/torch_api/__init__.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/torch_api/algorithms/__init__.py` & `bagua-0.9.3.dev5/bagua/torch_api/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/torch_api/algorithms/async_model_average.py` & `bagua-0.9.3.dev5/bagua/torch_api/algorithms/async_model_average.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/torch_api/algorithms/base.py` & `bagua-0.9.3.dev5/bagua/torch_api/algorithms/base.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/torch_api/algorithms/bytegrad.py` & `bagua-0.9.3.dev5/bagua/torch_api/algorithms/bytegrad.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/torch_api/algorithms/decentralized.py` & `bagua-0.9.3.dev5/bagua/torch_api/algorithms/decentralized.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/torch_api/algorithms/gradient_allreduce.py` & `bagua-0.9.3.dev5/bagua/torch_api/algorithms/gradient_allreduce.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/torch_api/algorithms/q_adam.py` & `bagua-0.9.3.dev5/bagua/torch_api/algorithms/q_adam.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/torch_api/bucket.py` & `bagua-0.9.3.dev5/bagua/torch_api/bucket.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/torch_api/checkpoint/checkpointing.py` & `bagua-0.9.3.dev5/bagua/torch_api/checkpoint/checkpointing.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/torch_api/communication.py` & `bagua-0.9.3.dev5/bagua/torch_api/communication.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from functools import lru_cache
 from datetime import timedelta
 from typing import Optional, List
 import torch.distributed.distributed_c10d as c10d
 from torch.distributed import ProcessGroup as TorchProcessGroup
 import gorilla
 import weakref
+import os
 
 # fmt: off
 __all__ = [
     "ReduceOp", "new_group", "from_torch_group", "init_process_group",
     "is_initialized", "send", "recv", "broadcast", "broadcast_object",
     "reduce", "reduce_inplace", "allreduce", "allreduce_inplace",
     "allgather", "allgather_inplace", "gather", "gather_inplace",
@@ -379,15 +380,14 @@
     backend.model_name = model_name
     return backend
 
 
 def run_flask_app(port):
     from flask import Flask
     from gevent.pywsgi import WSGIServer
-    import os
 
     os.environ["WERKZEUG_RUN_MAIN"] = "true"
 
     autotune_service = AutotuneService(
         world_size=get_world_size(),
         autotune_level=env.get_autotune_level(),
         max_samples=env.get_autotune_max_samples(),
@@ -439,23 +439,28 @@
         store.set("bagua_service_port", str(service_port))
     else:
         service_port = int(store.get("bagua_service_port"))
 
     return service_port
 
 
-def init_process_group(store: Optional[torch.distributed.Store] = None):
+def init_process_group(store: Optional[torch.distributed.Store] = None, rank: int = -1,
+                       world_size: int = -1, local_world_size: int = -1):
     """Initializes the PyTorch builtin distributed process group, and this will
     also initialize the distributed package, should be executed before all the
     APIs of Bagua.
 
     Args:
         store: Key/value store accessible to all workers, used to exchange
             connection/address information. If ``None``, a TCP-based store will be created.
             Default: ``None``.
+        rank: Rank of the current process (it should be a number between 0 and world_size-1).
+            Required if store is specified.
+        world_size: Number of processes participating in the job. Required if store is specified.
+        local_world_size: Number of processes per node. Required if store is specified.
 
     Examples::
         >>> import torch
         >>> import bagua.torch_api as bagua
         >>>
         >>> torch.cuda.set_device(bagua.get_local_rank()) # THIS LINE IS IMPORTANT. See the notes below.
         >>> bagua.init_process_group()
@@ -470,19 +475,18 @@
         ...    lr=0.01,
         ...    momentum=0.9
         ...    )
         >>> model = model.with_bagua([optimizer], ...)
 
     .. note::
         Each process should be associated to a CUDA device using `torch.cuda.set_device()`,
-        before calling :meth:`init_process_group`. Otherwise you may encounter the
+        before calling :meth:`init_process_group`. Otherwise, you may encounter the
         `fatal runtime error: Rust cannot catch foreign exceptions` error.
     """
 
-
     global _default_pg
     global _default_store
     global _autotune_service_port
 
     if _default_pg is not None:
         raise RuntimeError("trying to initialize the default process group twice!")
 
@@ -491,19 +495,32 @@
 
     if store is None:
         timeout = timedelta(minutes=30)
         store, _, _ = next(torch.distributed.rendezvous(url="env://", timeout=timeout))
         store.set_timeout(timeout)
         _default_store = store
     else:
+        assert rank >= 0
+        assert world_size > 0
+        assert local_world_size > 0
+
+        os.environ["RANK"] = str(rank)
+        os.environ["WORLD_SIZE"] = str(world_size)
+        os.environ["LOCAL_RANK"] = str(rank % local_world_size)
+        os.environ["LOCAL_WORLD_SIZE"] = str(local_world_size)
+
         _default_store = store
 
-    _autotune_service_port = _find_free_bagua_service_port(_default_store)
-    if get_rank() == 0 and _autotune_server is None:
-        start_autotune_server(_autotune_service_port)
+    if _autotune_service_port is None:
+        if get_rank() == 0:
+            _autotune_service_port = _find_free_bagua_service_port(_default_store)
+            store.set("bagua_autotune_service_port", str(_autotune_service_port))
+            start_autotune_server(_autotune_service_port)
+        else:
+            _autotune_service_port = int(store.get("bagua_autotune_service_port"))
 
     AUTOTUNE_SERVER_WAIT_TIME = 30
     wait_time = get_autotune_server_wait_time()
     # at least wait 30 seconds
     if wait_time < AUTOTUNE_SERVER_WAIT_TIME:
         wait_time = AUTOTUNE_SERVER_WAIT_TIME
```

### Comparing `bagua-0.9.3.dev4/bagua/torch_api/contrib/cache_loader.py` & `bagua-0.9.3.dev5/bagua/torch_api/contrib/cache_loader.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/torch_api/contrib/cached_dataset.py` & `bagua-0.9.3.dev5/bagua/torch_api/contrib/cached_dataset.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/torch_api/contrib/fuse/optimizer.py` & `bagua-0.9.3.dev5/bagua/torch_api/contrib/fuse/optimizer.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/torch_api/contrib/load_balancing_data_loader.py` & `bagua-0.9.3.dev5/bagua/torch_api/contrib/load_balancing_data_loader.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/torch_api/contrib/sync_batchnorm.py` & `bagua-0.9.3.dev5/bagua/torch_api/contrib/sync_batchnorm.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/torch_api/contrib/utils/redis_store.py` & `bagua-0.9.3.dev5/bagua/torch_api/contrib/utils/redis_store.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/torch_api/contrib/utils/store.py` & `bagua-0.9.3.dev5/bagua/torch_api/contrib/utils/store.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/torch_api/data_parallel/bagua_distributed.py` & `bagua-0.9.3.dev5/bagua/torch_api/data_parallel/bagua_distributed.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/torch_api/data_parallel/distributed.py` & `bagua-0.9.3.dev5/bagua/torch_api/data_parallel/distributed.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/torch_api/data_parallel/functional.py` & `bagua-0.9.3.dev5/bagua/torch_api/data_parallel/functional.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/torch_api/distributed.py` & `bagua-0.9.3.dev5/bagua/torch_api/distributed.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/torch_api/env.py` & `bagua-0.9.3.dev5/bagua/torch_api/env.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/torch_api/model_parallel/moe/experts.py` & `bagua-0.9.3.dev5/bagua/torch_api/model_parallel/moe/experts.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/torch_api/model_parallel/moe/layer.py` & `bagua-0.9.3.dev5/bagua/torch_api/model_parallel/moe/layer.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/torch_api/model_parallel/moe/sharded_moe.py` & `bagua-0.9.3.dev5/bagua/torch_api/model_parallel/moe/sharded_moe.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/torch_api/tensor.py` & `bagua-0.9.3.dev5/bagua/torch_api/tensor.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua/torch_api/utils.py` & `bagua-0.9.3.dev5/bagua/torch_api/utils.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua.egg-info/PKG-INFO` & `bagua-0.9.3.dev5/bagua.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bagua
-Version: 0.9.3.dev4
+Version: 0.9.3.dev5
 Summary: Bagua is a deep learning training acceleration framework for PyTorch. It provides a one-stop training acceleration solution, including faster distributed training compared to PyTorch DDP, faster dataloader, kernel fusion, and more.
 Home-page: https://github.com/BaguaSys/bagua
 Author: Kuaishou AI Platform & DS3 Lab
 Author-email: admin@mail.xrlian.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bagua Version: 0.9.3.dev4 Summary: Bagua is a deep
+Metadata-Version: 2.1 Name: bagua Version: 0.9.3.dev5 Summary: Bagua is a deep
 learning training acceleration framework for PyTorch. It provides a one-stop
 training acceleration solution, including faster distributed training compared
 to PyTorch DDP, faster dataloader, kernel fusion, and more. Home-page: https://
 github.com/BaguaSys/bagua Author: Kuaishou AI Platform & DS3 Lab Author-email:
 admin@mail.xrlian.com Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE
  [https://user-images.githubusercontent.com/18649508/141055752-2f429618-2707-
```

### Comparing `bagua-0.9.3.dev4/bagua.egg-info/SOURCES.txt` & `bagua-0.9.3.dev5/bagua.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/bagua_core/bagua_install_deps.py` & `bagua-0.9.3.dev5/bagua_core/bagua_install_deps.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/cliff.toml` & `bagua-0.9.3.dev5/cliff.toml`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/docker/Dockerfile.manylinux-cuda102` & `bagua-0.9.3.dev5/docker/Dockerfile.manylinux-cuda102`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/docker/Dockerfile.manylinux-cuda111` & `bagua-0.9.3.dev5/docker/Dockerfile.manylinux-cuda111`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/docker/Dockerfile.manylinux-cuda113` & `bagua-0.9.3.dev5/docker/Dockerfile.manylinux-cuda113`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/docker/Dockerfile.manylinux-cuda115` & `bagua-0.9.3.dev5/docker/Dockerfile.manylinux-cuda115`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/docker/Dockerfile.manylinux-cuda116` & `bagua-0.9.3.dev5/docker/Dockerfile.manylinux-cuda116`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/docker/Dockerfile.manylinux-cuda117` & `bagua-0.9.3.dev5/docker/Dockerfile.manylinux-cuda117`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/docker/Dockerfile.pytorch-1.10.0-cuda11.3-cudnn8` & `bagua-0.9.3.dev5/docker/Dockerfile.pytorch-1.10.0-cuda11.3-cudnn8`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/docker/Dockerfile.pytorch-1.11.0-cuda11.3-cudnn8` & `bagua-0.9.3.dev5/docker/Dockerfile.pytorch-1.11.0-cuda11.3-cudnn8`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/docker/Dockerfile.pytorch-1.12.0-cuda11.3-cudnn8` & `bagua-0.9.3.dev5/docker/Dockerfile.pytorch-1.12.0-cuda11.3-cudnn8`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/docker/Dockerfile.pytorch-1.13.0-cuda11.6-cudnn8` & `bagua-0.9.3.dev5/docker/Dockerfile.pytorch-1.13.0-cuda11.6-cudnn8`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/docker/Dockerfile.pytorch-1.9.0-cuda10.2-cudnn7` & `bagua-0.9.3.dev5/docker/Dockerfile.pytorch-1.9.0-cuda10.2-cudnn7`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/docker/Dockerfile.pytorch-1.9.0-cuda11.1-cudnn8` & `bagua-0.9.3.dev5/docker/Dockerfile.pytorch-1.9.0-cuda11.1-cudnn8`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/docker/Dockerfile.pytorch-2.0.0-cuda11.7-cudnn8` & `bagua-0.9.3.dev5/docker/Dockerfile.pytorch-2.0.0-cuda11.7-cudnn8`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/docs/_autoapi_templates/index.rst` & `bagua-0.9.3.dev5/docs/_autoapi_templates/index.rst`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/docs/_autoapi_templates/python/class.rst` & `bagua-0.9.3.dev5/docs/_autoapi_templates/python/class.rst`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/docs/_autoapi_templates/python/data.rst` & `bagua-0.9.3.dev5/docs/_autoapi_templates/python/data.rst`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/docs/_autoapi_templates/python/function.rst` & `bagua-0.9.3.dev5/docs/_autoapi_templates/python/function.rst`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/docs/_autoapi_templates/python/method.rst` & `bagua-0.9.3.dev5/docs/_autoapi_templates/python/method.rst`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/docs/_autoapi_templates/python/module.rst` & `bagua-0.9.3.dev5/docs/_autoapi_templates/python/module.rst`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/docs/conf.py` & `bagua-0.9.3.dev5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/docs/index.rst` & `bagua-0.9.3.dev5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/examples/LICENSE` & `bagua-0.9.3.dev5/examples/LICENSE`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/examples/benchmark/synthetic_benchmark.py` & `bagua-0.9.3.dev5/examples/benchmark/synthetic_benchmark.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/examples/communication_primitives/main.py` & `bagua-0.9.3.dev5/examples/communication_primitives/main.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/examples/elastic_training/main.py` & `bagua-0.9.3.dev5/examples/elastic_training/main.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/examples/imagenet/README.md` & `bagua-0.9.3.dev5/examples/imagenet/README.md`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/examples/imagenet/main.py` & `bagua-0.9.3.dev5/examples/imagenet/main.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/examples/mnist/main.py` & `bagua-0.9.3.dev5/examples/mnist/main.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/examples/moe/mnist_main.py` & `bagua-0.9.3.dev5/examples/moe/mnist_main.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/examples/squad/README.md` & `bagua-0.9.3.dev5/examples/squad/README.md`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/examples/squad/main.py` & `bagua-0.9.3.dev5/examples/squad/main.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/figures/logo.png` & `bagua-0.9.3.dev5/figures/logo.png`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/install.sh` & `bagua-0.9.3.dev5/install.sh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/install_master.sh` & `bagua-0.9.3.dev5/install_master.sh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/Cargo.lock` & `bagua-0.9.3.dev5/rust/bagua-core/Cargo.lock`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-c/Cargo.toml` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-c/Cargo.toml`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-c/src/lib.rs` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-c/src/lib.rs`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/Cargo.toml` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/Cargo.toml`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/build.rs` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/build.rs`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/cpp/include/bagua_utils.h` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/cpp/include/bagua_utils.h`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/cpp/include/dbg.h` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/cpp/include/dbg.h`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/kernels/bagua_kernels.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/kernels/bagua_kernels.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/comm_ops/centralized_full_precision_synchronous.rs` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/comm_ops/centralized_full_precision_synchronous.rs`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/comm_ops/centralized_low_precision_synchronous.rs` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/comm_ops/centralized_low_precision_synchronous.rs`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/comm_ops/decentralized_full_precision_asynchronous.rs` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/comm_ops/decentralized_full_precision_asynchronous.rs`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/comm_ops/decentralized_full_precision_synchronous.rs` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/comm_ops/decentralized_full_precision_synchronous.rs`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/comm_ops/decentralized_low_precision_synchronous.rs` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/comm_ops/decentralized_low_precision_synchronous.rs`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/comm_ops/mod.rs` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/comm_ops/mod.rs`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/comm_ops/python_ffi_op.rs` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/comm_ops/python_ffi_op.rs`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/communicators/mod.rs` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/communicators/mod.rs`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/cuda_utils.rs` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/cuda_utils.rs`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/datatypes/mod.rs` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/datatypes/mod.rs`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/events.rs` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/events.rs`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/kernels/mod.rs` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/kernels/mod.rs`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/lib.rs` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/lib.rs`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/resource_pool/mod.rs` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/resource_pool/mod.rs`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/src/torch_ffi.rs` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/src/torch_ffi.rs`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/CMakeLists.txt` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/LICENSE` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/LICENSE`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/README.md` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/README.md`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/CMakeLists.txt` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/benchmark_events.cpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/benchmark_events.cpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/benchmark_ops.cpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/benchmark_ops.cpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/benchmark_utils.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/benchmark_utils.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/benchmark_utils_ht.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/benchmark_utils_ht.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/benchmark_utils_mpi.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/benchmark_utils_mpi.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/benchmark_utils_nccl.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/benchmark_utils_nccl.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/benchmark_waits.cpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/benchmark_waits.cpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/plot_benchmarks.py` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/plot_benchmarks.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/run_benchmarks.py` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/run_benchmarks.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/wait.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/wait.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/wait.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/benchmark/wait.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/Al_config.hpp.in` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/Al_config.hpp.in`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/AluminumConfig.cmake.in` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/AluminumConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/FindCUB.cmake` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/FindCUB.cmake`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/FindHWLOC.cmake` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/FindHWLOC.cmake`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/FindNCCL.cmake` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/FindNCCL.cmake`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/FindNVTX.cmake` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/FindNVTX.cmake`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/HipBuildSystem.cmake` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/cmake/HipBuildSystem.cmake`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/Al.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/Al.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/CMakeLists.txt` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/base.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/base.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/cuda.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/cuda.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/cuda_mempool.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/cuda_mempool.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/events.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/events.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/gpu_status_flag.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/gpu_status_flag.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/gpu_wait.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/gpu_wait.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/helper_kernels.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/helper_kernels.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/streams.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/streams.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/sync_memory.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/cuda/sync_memory.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/allgather.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/allgather.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/allgatherv.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/allgatherv.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/allreduce.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/allreduce.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/alltoall.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/alltoall.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/alltoallv.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/alltoallv.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/barrier.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/barrier.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/base_state.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/base_state.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/bcast.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/bcast.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/communicator.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/communicator.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/gather.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/gather.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/gatherv.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/gatherv.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/pt2pt.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/pt2pt.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/reduce.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/reduce.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/reduce_scatter.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/reduce_scatter.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/reduce_scatterv.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/reduce_scatterv.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/scatter.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/scatter.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/scatterv.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht/scatterv.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht_impl.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/ht_impl.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/internal.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/internal.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mempool.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mempool.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/allgather.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/allgather.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/allgatherv.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/allgatherv.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/allreduce.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/allreduce.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/alltoall.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/alltoall.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/alltoallv.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/alltoallv.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/barrier.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/barrier.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/base_state.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/base_state.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/bcast.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/bcast.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/communicator.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/communicator.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/gather.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/gather.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/gatherv.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/gatherv.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/pt2pt.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/pt2pt.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/reduce.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/reduce.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/reduce_scatter.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/reduce_scatter.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/reduce_scatterv.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/reduce_scatterv.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/scatter.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/scatter.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/scatterv.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/scatterv.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/utils.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi/utils.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_comm_and_stream_wrapper.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_comm_and_stream_wrapper.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda/communicator.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda/communicator.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda/rma.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda/rma.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda/rma_ipc.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda/rma_ipc.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda/rma_null.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda/rma_null.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda/rma_self.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda/rma_self.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda/util.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda/util.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda_impl.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_cuda_impl.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_impl.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/mpi_impl.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/nccl_impl.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/nccl_impl.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/profiling.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/profiling.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/progress.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/progress.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/state.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/state.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/trace.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/trace.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/tuning_params.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/tuning_params.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/utils/caching_allocator.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/utils/caching_allocator.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/utils/locked_resource_pool.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/utils/locked_resource_pool.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/utils/meta.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/utils/meta.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/utils/mpsc_queue.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/utils/mpsc_queue.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/utils/spsc_queue.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/utils/spsc_queue.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/utils/utils.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/include/aluminum/utils/utils.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/Al.cpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/Al.cpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/CMakeLists.txt` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/cuda/cuda.cpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/cuda/cuda.cpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/cuda/gpu_status_flag.cpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/cuda/gpu_status_flag.cpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/cuda/gpu_wait.cpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/cuda/gpu_wait.cpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/cuda/helper_kernels.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/cuda/helper_kernels.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/cuda/streams.cpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/cuda/streams.cpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/ht_impl.cpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/ht_impl.cpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/mempool.cpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/mempool.cpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/mpi_cuda/communicator.cpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/mpi_cuda/communicator.cpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/mpi_cuda/rma.cpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/mpi_cuda/rma.cpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/mpi_cuda_impl.cpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/mpi_cuda_impl.cpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/mpi_impl.cpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/mpi_impl.cpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/nccl_impl.cpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/nccl_impl.cpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/profiling.cpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/profiling.cpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/progress.cpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/progress.cpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/trace.cpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/src/trace.cpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/CMakeLists.txt` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/cuda_vector.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/cuda_vector.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/hang_watchdog.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/hang_watchdog.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/op_dispatcher.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/op_dispatcher.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/op_runner_impl.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/op_runner_impl.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/run_tests.py` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/run_tests.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_exchange.cpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_exchange.cpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_ops.cpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_ops.cpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_rma_halo_exchange.cpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_rma_halo_exchange.cpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_rma_ring.cpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_rma_ring.cpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_stream_mem_ops.cpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_stream_mem_ops.cpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_utils.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_utils.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_utils_ht.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_utils_ht.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_utils_mpi.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_utils_mpi.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_utils_mpi_cuda.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_utils_mpi_cuda.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_utils_nccl.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/test/test_utils_nccl.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/.travis.yml` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/.travis.yml`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/CHANGELOG.md` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/CMakeLists.txt` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/INSTALL` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/INSTALL`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/LICENSE` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/LICENSE`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/README.md` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/README.md`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/include/cxxopts.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/include/cxxopts.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/src/CMakeLists.txt` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/src/example.cpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/src/example.cpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/CMakeLists.txt` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/catch.hpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/catch.hpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/options.cpp` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/Aluminum/third_party/cxxopts/test/options.cpp`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/.cproject` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/.cproject`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/.project` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/.project`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/.settings/org.eclipse.cdt.codan.core.prefs` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/.settings/org.eclipse.cdt.codan.core.prefs`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/.settings/org.eclipse.cdt.core.prefs` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/.settings/org.eclipse.cdt.core.prefs`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/CHANGE_LOG.TXT` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/CHANGE_LOG.TXT`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/LICENSE.TXT` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/README.md` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/common.mk` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/common.mk`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_histogram.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_histogram.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_radix_sort_downsweep.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_radix_sort_downsweep.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_radix_sort_upsweep.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_radix_sort_upsweep.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_reduce.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_reduce.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_reduce_by_key.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_reduce_by_key.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_rle.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_rle.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_scan.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_scan.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_segment_fixup.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_segment_fixup.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_select_if.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_select_if.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_spmv_orig.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/agent_spmv_orig.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/single_pass_scan_operators.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/agent/single_pass_scan_operators.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_adjacent_difference.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_adjacent_difference.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_discontinuity.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_discontinuity.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_exchange.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_exchange.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_histogram.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_histogram.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_load.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_load.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_radix_rank.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_radix_rank.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_radix_sort.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_radix_sort.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_raking_layout.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_raking_layout.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_reduce.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_reduce.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_scan.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_scan.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_shuffle.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_shuffle.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_store.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/block_store.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_histogram_atomic.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_histogram_atomic.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_histogram_sort.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_histogram_sort.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_reduce_raking.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_reduce_raking.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_reduce_raking_commutative_only.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_reduce_raking_commutative_only.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_reduce_warp_reductions.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_reduce_warp_reductions.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_scan_raking.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_scan_raking.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_scan_warp_scans.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_scan_warp_scans.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_scan_warp_scans2.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_scan_warp_scans2.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_scan_warp_scans3.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/block/specializations/block_scan_warp_scans3.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/cub.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/cub.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_histogram.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_histogram.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_partition.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_partition.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_radix_sort.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_radix_sort.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_reduce.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_reduce.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_run_length_encode.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_run_length_encode.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_scan.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_scan.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_segmented_radix_sort.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_segmented_radix_sort.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_segmented_reduce.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_segmented_reduce.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_select.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_select.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_spmv.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/device_spmv.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_histogram.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_histogram.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_radix_sort.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_radix_sort.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_reduce.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_reduce.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_reduce_by_key.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_reduce_by_key.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_rle.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_rle.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_scan.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_scan.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_select_if.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_select_if.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_spmv_orig.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/device/dispatch/dispatch_spmv_orig.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/grid/grid_barrier.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/grid/grid_barrier.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/grid/grid_even_share.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/grid/grid_even_share.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/grid/grid_mapping.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/grid/grid_mapping.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/grid/grid_queue.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/grid/grid_queue.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/host/mutex.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/host/mutex.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/arg_index_input_iterator.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/arg_index_input_iterator.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/cache_modified_input_iterator.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/cache_modified_input_iterator.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/cache_modified_output_iterator.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/cache_modified_output_iterator.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/constant_input_iterator.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/constant_input_iterator.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/counting_input_iterator.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/counting_input_iterator.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/discard_output_iterator.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/discard_output_iterator.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/tex_obj_input_iterator.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/tex_obj_input_iterator.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/tex_ref_input_iterator.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/tex_ref_input_iterator.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/transform_input_iterator.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/iterator/transform_input_iterator.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/thread/thread_load.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/thread/thread_load.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/thread/thread_operators.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/thread/thread_operators.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/thread/thread_reduce.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/thread/thread_reduce.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/thread/thread_scan.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/thread/thread_scan.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/thread/thread_search.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/thread/thread_search.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/thread/thread_store.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/thread/thread_store.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_allocator.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_allocator.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_arch.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_arch.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_debug.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_debug.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_device.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_device.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_macro.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_macro.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_namespace.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_namespace.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_ptx.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_ptx.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_type.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/util_type.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/warp/specializations/warp_reduce_shfl.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/warp/specializations/warp_reduce_shfl.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/warp/specializations/warp_reduce_smem.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/warp/specializations/warp_reduce_smem.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/warp/specializations/warp_scan_shfl.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/warp/specializations/warp_scan_shfl.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/warp/specializations/warp_scan_smem.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/warp/specializations/warp_scan_smem.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/warp/warp_reduce.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/warp/warp_reduce.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/warp/warp_scan.cuh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/cub/warp/warp_scan.cuh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/eclipse code style profile.xml` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/eclipse code style profile.xml`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/block/Makefile` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/block/Makefile`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/block/example_block_radix_sort.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/block/example_block_radix_sort.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/block/example_block_reduce.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/block/example_block_reduce.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/block/example_block_scan.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/block/example_block_scan.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/block/reduce_by_key.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/block/reduce_by_key.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/Makefile` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/Makefile`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_partition_flagged.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_partition_flagged.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_partition_if.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_partition_if.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_radix_sort.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_radix_sort.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_reduce.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_reduce.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_scan.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_scan.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_select_flagged.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_select_flagged.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_select_if.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_select_if.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_select_unique.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_select_unique.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_sort_find_non_trivial_runs.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/examples/device/example_device_sort_find_non_trivial_runs.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/Makefile` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/Makefile`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/defunct/example_coo_spmv.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/defunct/example_coo_spmv.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/defunct/test_device_seg_reduce.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/defunct/test_device_seg_reduce.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/histogram/histogram_cub.h` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/histogram/histogram_cub.h`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/histogram/histogram_gmem_atomics.h` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/histogram/histogram_gmem_atomics.h`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/histogram/histogram_smem_atomics.h` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/histogram/histogram_smem_atomics.h`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/histogram_compare.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/histogram_compare.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/sparse_matrix.h` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/sparse_matrix.h`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/spmv_compare.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/spmv_compare.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/spmv_script.sh` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/experimental/spmv_script.sh`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/Makefile` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/Makefile`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/half.h` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/half.h`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/mersenne.h` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/mersenne.h`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_allocator.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_allocator.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_block_histogram.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_block_histogram.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_block_load_store.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_block_load_store.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_block_radix_sort.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_block_radix_sort.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_block_reduce.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_block_reduce.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_block_scan.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_block_scan.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_histogram.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_histogram.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_radix_sort.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_radix_sort.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_reduce.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_reduce.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_reduce_by_key.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_reduce_by_key.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_run_length_encode.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_run_length_encode.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_scan.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_scan.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_select_if.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_select_if.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_select_unique.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_device_select_unique.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_grid_barrier.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_grid_barrier.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_iterator.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_iterator.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_util.h` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_util.h`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_warp_reduce.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_warp_reduce.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_warp_scan.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/test/test_warp_scan.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/tune/Makefile` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/tune/Makefile`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/tune/tune_device_reduce.cu` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-internal/third_party/cub-1.8.0/tune/tune_device_reduce.cu`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-py/Cargo.toml` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-py/Cargo.toml`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-core-py/src/lib.rs` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-core-py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-opentelemetry/Cargo.toml` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-opentelemetry/Cargo.toml`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-opentelemetry/src/exporter/agent.rs` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-opentelemetry/src/exporter/agent.rs`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-opentelemetry/src/exporter/mod.rs` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-opentelemetry/src/exporter/mod.rs`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-core/bagua-opentelemetry/src/lib.rs` & `bagua-0.9.3.dev5/rust/bagua-core/bagua-opentelemetry/src/lib.rs`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-net/Cargo.lock` & `bagua-0.9.3.dev5/rust/bagua-net/Cargo.lock`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-net/Cargo.toml` & `bagua-0.9.3.dev5/rust/bagua-net/Cargo.toml`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-net/README.md` & `bagua-0.9.3.dev5/rust/bagua-net/README.md`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-net/cc/Makefile` & `bagua-0.9.3.dev5/rust/bagua-net/cc/Makefile`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-net/cc/bagua_net.cc` & `bagua-0.9.3.dev5/rust/bagua-net/cc/bagua_net.cc`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-net/cc/bagua_net.h` & `bagua-0.9.3.dev5/rust/bagua-net/cc/bagua_net.h`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-net/cc/nccl_types.h` & `bagua-0.9.3.dev5/rust/bagua-net/cc/nccl_types.h`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-net/cc/v3/nccl_net_v3.cc` & `bagua-0.9.3.dev5/rust/bagua-net/cc/v3/nccl_net_v3.cc`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-net/cc/v3/nccl_net_v3.h` & `bagua-0.9.3.dev5/rust/bagua-net/cc/v3/nccl_net_v3.h`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-net/cc/v4/nccl_net_v4.cc` & `bagua-0.9.3.dev5/rust/bagua-net/cc/v4/nccl_net_v4.cc`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-net/cc/v4/nccl_net_v4.h` & `bagua-0.9.3.dev5/rust/bagua-net/cc/v4/nccl_net_v4.h`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-net/src/implement/nthread_per_socket_backend.rs` & `bagua-0.9.3.dev5/rust/bagua-net/src/implement/nthread_per_socket_backend.rs`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-net/src/implement/tokio_backend.rs` & `bagua-0.9.3.dev5/rust/bagua-net/src/implement/tokio_backend.rs`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-net/src/interface.rs` & `bagua-0.9.3.dev5/rust/bagua-net/src/interface.rs`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-net/src/lib.rs` & `bagua-0.9.3.dev5/rust/bagua-net/src/lib.rs`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/rust/bagua-net/src/utils.rs` & `bagua-0.9.3.dev5/rust/bagua-net/src/utils.rs`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/setup.py` & `bagua-0.9.3.dev5/setup.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/comm/test_communicator.py` & `bagua-0.9.3.dev5/tests/comm/test_communicator.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/contrib/test_cached_dataset.py` & `bagua-0.9.3.dev5/tests/contrib/test_cached_dataset.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/contrib/test_fused_optimizer.py` & `bagua-0.9.3.dev5/tests/contrib/test_fused_optimizer.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/contrib/test_load_balancing_data_loader.py` & `bagua-0.9.3.dev5/tests/contrib/test_load_balancing_data_loader.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/contrib/test_store.py` & `bagua-0.9.3.dev5/tests/contrib/test_store.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/contrib/test_sync_bn.py` & `bagua-0.9.3.dev5/tests/contrib/test_sync_bn.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/internal/compressor.py` & `bagua-0.9.3.dev5/tests/internal/compressor.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/internal/multi_process.py` & `bagua-0.9.3.dev5/tests/internal/multi_process.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/internal/torch/_core.py` & `bagua-0.9.3.dev5/tests/internal/torch/_core.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/internal/torch/common_cuda.py` & `bagua-0.9.3.dev5/tests/internal/torch/common_cuda.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/internal/torch/common_distributed.py` & `bagua-0.9.3.dev5/tests/internal/torch/common_distributed.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/internal/torch/common_utils.py` & `bagua-0.9.3.dev5/tests/internal/torch/common_utils.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/internal/torch/expecttest.py` & `bagua-0.9.3.dev5/tests/internal/torch/expecttest.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/pytorch_lightning/boring_model.py` & `bagua-0.9.3.dev5/tests/pytorch_lightning/boring_model.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/pytorch_lightning/test_bagua_strategy.py` & `bagua-0.9.3.dev5/tests/pytorch_lightning/test_bagua_strategy.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/service/test_autotune_service.py` & `bagua-0.9.3.dev5/tests/service/test_autotune_service.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/service/test_bayesian_optimizer.py` & `bagua-0.9.3.dev5/tests/service/test_bayesian_optimizer.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/test_bagua_define.py` & `bagua-0.9.3.dev5/tests/test_bagua_define.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/torch_api/data_parallel/test_async_model_average.py` & `bagua-0.9.3.dev5/tests/torch_api/data_parallel/test_async_model_average.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/torch_api/data_parallel/test_bagua_ddp.py` & `bagua-0.9.3.dev5/tests/torch_api/data_parallel/test_bagua_ddp.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/torch_api/data_parallel/test_bagua_module.py` & `bagua-0.9.3.dev5/tests/torch_api/data_parallel/test_bagua_module.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/torch_api/data_parallel/test_broadcast_state.py` & `bagua-0.9.3.dev5/tests/torch_api/data_parallel/test_broadcast_state.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/torch_api/data_parallel/test_c10d_common.py` & `bagua-0.9.3.dev5/tests/torch_api/data_parallel/test_c10d_common.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/torch_api/data_parallel/test_decentralized.py` & `bagua-0.9.3.dev5/tests/torch_api/data_parallel/test_decentralized.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/torch_api/data_parallel/test_gradient_allreduce.py` & `bagua-0.9.3.dev5/tests/torch_api/data_parallel/test_gradient_allreduce.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/torch_api/data_parallel/test_low_precision_decentralized.py` & `bagua-0.9.3.dev5/tests/torch_api/data_parallel/test_low_precision_decentralized.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/torch_api/data_parallel/test_multi_models.py` & `bagua-0.9.3.dev5/tests/torch_api/data_parallel/test_multi_models.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/torch_api/test_async_model_average.py` & `bagua-0.9.3.dev5/tests/torch_api/test_async_model_average.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/torch_api/test_bagua_module.py` & `bagua-0.9.3.dev5/tests/torch_api/test_bagua_module.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/torch_api/test_broadcast_state.py` & `bagua-0.9.3.dev5/tests/torch_api/test_broadcast_state.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/torch_api/test_decentralized.py` & `bagua-0.9.3.dev5/tests/torch_api/test_decentralized.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/torch_api/test_gradient_allreduce.py` & `bagua-0.9.3.dev5/tests/torch_api/test_gradient_allreduce.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/torch_api/test_low_precision_decentralized.py` & `bagua-0.9.3.dev5/tests/torch_api/test_low_precision_decentralized.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/torch_api/test_multi_models.py` & `bagua-0.9.3.dev5/tests/torch_api/test_multi_models.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/torch_api/test_process_group.py` & `bagua-0.9.3.dev5/tests/torch_api/test_process_group.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/torch_api/test_qadam.py` & `bagua-0.9.3.dev5/tests/torch_api/test_qadam.py`

 * *Files identical despite different names*

### Comparing `bagua-0.9.3.dev4/tests/torch_api/test_utils.py` & `bagua-0.9.3.dev5/tests/torch_api/test_utils.py`

 * *Files identical despite different names*

