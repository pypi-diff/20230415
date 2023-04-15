# Comparing `tmp/starwhale-0.4.1.tar.gz` & `tmp/starwhale-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/starwhale-0.4.1.tar", last modified: Tue Mar 14 02:09:25 2023, max compression
+gzip compressed data, was "dist/starwhale-0.4.2.tar", last modified: Sat Apr 15 13:36:38 2023, max compression
```

## Comparing `starwhale-0.4.1.tar` & `starwhale-0.4.2.tar`

### file list

```diff
@@ -1,173 +1,283 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    18911 2023-03-14 02:09:25.000000 starwhale-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-14 02:05:44.000000 starwhale-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-03-14 02:05:44.000000 starwhale-0.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5098 2023-03-14 02:05:44.000000 starwhale-0.4.1/scripts/sw-docker-entrypoint
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 02:09:25.000000 starwhale-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-03-14 02:05:44.000000 starwhale-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale/
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale/api/_impl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/api/_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51602 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/api/_impl/data_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale/api/_impl/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/api/_impl/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18841 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/api/_impl/dataset/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/api/_impl/dataset/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    28436 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/api/_impl/dataset/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/api/_impl/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/api/_impl/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/api/_impl/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/api/_impl/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/api/_impl/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale/api/_impl/track/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/api/_impl/track/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/api/_impl/track/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/api/_impl/track/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/api/_impl/track/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/api/_impl/track/hooker.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/api/_impl/track/syncer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20174 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/api/_impl/track/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9636 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/api/_impl/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/api/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/api/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/api/job.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/api/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/api/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/api/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/api/track.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale/base/blob/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/base/blob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/base/blob/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/base/blob/store.py
--rw-r--r--   0 runner    (1001) docker     (123)    10859 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/base/bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)    17007 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/base/bundle_copy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11236 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/base/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/base/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/base/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/base/store.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/base/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/base/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/base/uri.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale/base/uricomponents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/base/uricomponents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/base/uricomponents/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/base/uricomponents/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/base/uricomponents/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/base/uricomponents/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/base/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale/cli/assistance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/cli/assistance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10607 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/cli/assistance/broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/cli/assistance/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10886 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/cli/assistance/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/cli/assistance/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/cli/assistance/remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale/cli/board/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/cli/board/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/cli/board/board.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/cli/board/project_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/cli/board/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/cli/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/cli/mngt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale/consts/
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/consts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/consts/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale/core/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/dataset/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/dataset/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)    19160 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/dataset/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    23494 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/dataset/store.py
--rw-r--r--   0 runner    (1001) docker     (123)    20797 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/dataset/tabular.py
--rw-r--r--   0 runner    (1001) docker     (123)    32376 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/dataset/type.py
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/dataset/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale/core/eval/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/eval/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/eval/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    15691 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/eval/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/eval/store.py
--rw-r--r--   0 runner    (1001) docker     (123)    14685 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/eval/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale/core/instance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/instance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/instance/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/instance/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/instance/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale/core/job/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/job/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/job/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/job/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale/core/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/model/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/model/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/model/default_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    25957 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/model/store.py
--rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/model/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale/core/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/project/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/project/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/project/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale/core/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17215 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/runtime/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    64203 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/runtime/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/runtime/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/runtime/store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale/core/runtime/template/
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/runtime/template/Dockerfile.tmpl
--rw-r--r--   0 runner    (1001) docker     (123)    12361 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/runtime/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale/core/track/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/core/track/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale/integrations/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/integrations/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/integrations/pytorch/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/integrations/pytorch/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale/integrations/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/integrations/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/integrations/tensorflow/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale/mngt/
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/mngt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/utils/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/utils/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/utils/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/utils/load.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/utils/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/utils/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    24420 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/utils/venv.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/utils/venv_pack.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-14 02:05:44.000000 starwhale-0.4.1/starwhale/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18911 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 02:06:16.000000 starwhale-0.4.1/starwhale.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-14 02:09:25.000000 starwhale-0.4.1/starwhale.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    18824 2023-04-15 13:36:38.000000 starwhale-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-15 13:26:11.000000 starwhale-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-15 13:26:11.000000 starwhale-0.4.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5554 2023-04-15 13:26:11.000000 starwhale-0.4.2/scripts/sw-docker-entrypoint
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 13:36:38.000000 starwhale-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-15 13:26:11.000000 starwhale-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/api/_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53386 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/_impl/data_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/api/_impl/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/_impl/dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/api/_impl/dataset/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/_impl/dataset/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/_impl/dataset/builder/mapping_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/_impl/dataset/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37919 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/_impl/dataset/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21471 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/_impl/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/_impl/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/_impl/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/_impl/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/_impl/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/_impl/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/api/_impl/track/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/_impl/track/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/_impl/track/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/_impl/track/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/_impl/track/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/_impl/track/hooker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/_impl/track/syncer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20174 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/_impl/track/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10219 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/_impl/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/api/track.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/base/blob/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/base/blob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/base/blob/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/base/blob/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10838 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/base/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17411 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/base/bundle_copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/base/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/base/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/base/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/base/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/base/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/base/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/base/uri.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/base/uricomponents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/base/uricomponents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/base/uricomponents/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/base/uricomponents/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/base/uricomponents/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/base/uricomponents/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/base/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/cli/assistance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/cli/assistance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10607 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/cli/assistance/broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/cli/assistance/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10886 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/cli/assistance/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/cli/assistance/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/cli/assistance/remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/cli/board/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/cli/board/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/cli/board/board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/cli/board/project_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/cli/board/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/cli/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/cli/mngt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/consts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/consts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/consts/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/core/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10569 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/dataset/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/dataset/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/dataset/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23718 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/dataset/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20052 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/dataset/tabular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31032 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/dataset/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/dataset/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/core/eval/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/eval/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/eval/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15691 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/eval/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/eval/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15756 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/eval/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/core/instance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/instance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/instance/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/instance/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/instance/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/core/job/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/job/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/job/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/job/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/job/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/job/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/core/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/model/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/model/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27394 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/model/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13025 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/model/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/core/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/project/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/project/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/project/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/core/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24573 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/runtime/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69301 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/runtime/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/runtime/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/runtime/store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/core/runtime/template/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/runtime/template/Dockerfile.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)    15287 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/runtime/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/core/track/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/core/track/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/integrations/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/integrations/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/integrations/pytorch/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/integrations/pytorch/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/integrations/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/integrations/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/integrations/tensorflow/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/mngt/
+-rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/mngt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/utils/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/utils/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/utils/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/utils/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24420 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/utils/venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/utils/venv_pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/web/data_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/web/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/web/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/web/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/web/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/web/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/web/ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale/web/ui/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/BlockLabel.73476e4e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/CarouselItem.svelte_svelte_type_style_lang.4dd79b13.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/Column.696be89b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/File.218f371b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/Image.467ef809.js
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/Image2.677caf30.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1555639 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/JobDAG.0f060ddc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/JobDAG.9e7d9907.css
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/Model3D.87675a80.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/ModifyUpload.62c93b6f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/RobotoMono-Regular.5c4ca672.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/Tabs.6cd99b38.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/Upload.2295877e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    52070 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/Webcam.42d3de51.js
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/_commonjs-dynamic-modules.30ae7933.js
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/_commonjsHelpers.38432da5.js
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/bg-1920x1080.8b0d8feb.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/bg-2560x1440.c97cffa5.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/bg-3840x2160.f974f4b1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/color.68638319.js
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/csv.61a85bcd.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/dsv.396f62d0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/empty-chart.1e62901a.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/empty.f3091520.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/google.9d1a8b2b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/iconfont.0c5fdd4d.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/iconfont.6c404e0d.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/iconfont.9d477487.woff
+-rw-r--r--   0 runner    (1001) docker     (123)  3810379 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index.18f95905.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3277898 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index.881b9b68.js
+-rw-r--r--   0 runner    (1001) docker     (123)   253364 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index.c4eaac00.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index.e20ea34b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index10.bd426b18.js
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index11.26352100.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21113 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index12.aaad6797.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18559 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index13.9dace264.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index14.4ac02339.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index15.2fe323db.js
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index16.f5c4652a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11192 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index17.e4553bc2.js
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index18.b0959820.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index19.845f5573.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33634 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index2.456adea0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index20.11ae6bc1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    40218 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index21.81abfe15.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17924 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index22.6f73fd2b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index23.ecb1c872.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index24.a3fade65.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index25.6c1dd252.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3546601 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index26.7399988d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index27.e5971322.js
+-rw-r--r--   0 runner    (1001) docker     (123)  4618041 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index28.472081c6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index29.26cb76b8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index3.d13f8a82.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index30.731864f0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index31.58dbdc5f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index32.293573af.js
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index33.91c5a38f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index34.059902fd.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index35.e7bd1ba8.js
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index36.b6d4bb0d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18667 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index37.26191220.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index38.6f7ef489.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17343 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index39.75276adc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index4.b06c166c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index5.76f18de8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index6.039574df.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index7.d422bfde.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index8.45cb32d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/index9.9980ce7d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/invalid-file.82d62dec.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/left-shadow.e0fdfe32.png
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/left.8c88a49a.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    23151 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/linear.80285bdf.js
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/logo_normal_en_blue.18b013e7.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/logo_normal_en_gray.163de1a0.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/logo_normal_en_white.ec11283c.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/logo_small_en_white.782559aa.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    94167 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/module.554fb39c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/module2.c313c5e8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/module3.9dea3bf0.js
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/project.863f66b0.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/right-shadow.58dd9abc.png
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/right.aefe3c24.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/search-empty.13cbde15.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/setting.6d098443.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/utils.eaa949ca.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/assets/web-vitals.d62816c8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-04-15 13:36:24.000000 starwhale-0.4.2/starwhale/web/ui/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-04-15 13:36:24.000000 starwhale-0.4.2/starwhale/web/ui/favicon_white.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    25155 2023-04-15 13:36:24.000000 starwhale-0.4.2/starwhale/web/ui/iconfont.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20273 2023-04-15 13:36:33.000000 starwhale-0.4.2/starwhale/web/ui/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-15 13:36:24.000000 starwhale-0.4.2/starwhale/web/ui/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-15 13:26:11.000000 starwhale-0.4.2/starwhale/web/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18824 2023-04-15 13:36:37.000000 starwhale-0.4.2/starwhale.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-04-15 13:36:38.000000 starwhale-0.4.2/starwhale.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 13:36:37.000000 starwhale-0.4.2/starwhale.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-15 13:36:37.000000 starwhale-0.4.2/starwhale.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 13:26:52.000000 starwhale-0.4.2/starwhale.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-15 13:36:37.000000 starwhale-0.4.2/starwhale.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-15 13:36:37.000000 starwhale-0.4.2/starwhale.egg-info/top_level.txt
```

### Comparing `starwhale-0.4.1/PKG-INFO` & `starwhale-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starwhale
-Version: 0.4.1
+Version: 0.4.2
 Summary: An MLOps Platform for Model Evaluation
 Home-page: https://github.com/star-whale/starwhale
 Author: Starwhale Team
 Author-email: developer@starwhale.ai
 License: Apache License 2.0
 Keywords: MLOps,AI,Starwhale,Model Evaluation
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -153,15 +153,14 @@
     > extra-index-url = https://pypi.doubanio.com/simple
     > ```
 
     ```bash
     swcli runtime build example/runtime/pytorch
     swcli runtime list
     swcli runtime info pytorch/version/latest
-    swcli runtime restore pytorch/version/latest
     ```
 
 - 🍞 **STEP4**: Building a model
 
   - Download pre-trained model file:
 
     ```bash
@@ -173,15 +172,15 @@
     ```
 
   - [Code Example]Write some code with Starwhale Python SDK. Complete code is [here](https://github.com/star-whale/starwhale/blob/main/example/mnist/mnist/evaluator.py).
 
     ```python
     import typing as t
     import torch
-    from starwhale import Image, PipelineHandler, PPLResultIterator, multi_classification
+    from starwhale import Image, PipelineHandler, multi_classification
 
     class MNISTInference(PipelineHandler):
             def __init__(self) -> None:
                 super().__init__()
                 self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
                 self.model = self._load_model(self.device)
 
@@ -194,15 +193,15 @@
                 confusion_matrix_normalize="all",
                 show_hamming_loss=True,
                 show_cohen_kappa_score=True,
                 show_roc_auc=True,
                 all_labels=[i for i in range(0, 10)],
             )
             def cmp(
-                self, ppl_result: PPLResultIterator
+                self, ppl_result
             ) -> t.Tuple[t.List[int], t.List[int], t.List[t.List[float]]]:
                 result, label, pr = [], [], []
                 for _data in ppl_result:
                     label.append(_data["ds_data"]["label"])
                     result.append(_data["result"][0])
                     pr.append(_data["result"][1])
                 return label, result, pr
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: starwhale Version: 0.4.1 Summary: An MLOps Platform
+Metadata-Version: 2.1 Name: starwhale Version: 0.4.2 Summary: An MLOps Platform
 for Model Evaluation Home-page: https://github.com/star-whale/starwhale Author:
 Starwhale Team Author-email: developer@starwhale.ai License: Apache License 2.0
 Keywords: MLOps,AI,Starwhale,Model Evaluation Classifier: Development Status ::
 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
@@ -77,74 +77,73 @@
 the network environment of the machine and the number of packages in the
 runtime.yaml. Using the befitting pypi mirror and cache config in the `~/.pip/
 pip.conf` file is a recommended practice. > > For users in the mainland of
 China, the following conf file is an option: > > ```conf > [global] > cache-dir
 = ~/.cache/pip > index-url = https://mirrors.aliyun.com/pypi/simple/ > extra-
 index-url = https://pypi.doubanio.com/simple > ``` ```bash swcli runtime build
 example/runtime/pytorch swcli runtime list swcli runtime info pytorch/version/
-latest swcli runtime restore pytorch/version/latest ``` - ð **STEP4**:
-Building a model - Download pre-trained model file: ```bash cd example/mnist
-make download-model # For users in the mainland of China, please add `CN=1`
-environment for make command: # CN=1 make download-model cd - ``` - [Code
-Example]Write some code with Starwhale Python SDK. Complete code is [here]
-(https://github.com/star-whale/starwhale/blob/main/example/mnist/mnist/
-evaluator.py). ```python import typing as t import torch from starwhale import
-Image, PipelineHandler, PPLResultIterator, multi_classification class
+latest ``` - ð **STEP4**: Building a model - Download pre-trained model
+file: ```bash cd example/mnist make download-model # For users in the mainland
+of China, please add `CN=1` environment for make command: # CN=1 make download-
+model cd - ``` - [Code Example]Write some code with Starwhale Python SDK.
+Complete code is [here](https://github.com/star-whale/starwhale/blob/main/
+example/mnist/mnist/evaluator.py). ```python import typing as t import torch
+from starwhale import Image, PipelineHandler, multi_classification class
 MNISTInference(PipelineHandler): def __init__(self) -> None: super().__init__()
 self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 self.model = self._load_model(self.device) def ppl(self, data: t.Dict[str,
 t.Any], **kw: t.Any) -> t.Tuple[float, t.List[float]]: data_tensor = self._pre
 (data["img"]) output = self.model(data_tensor) return self._post(output)
 @multi_classification( confusion_matrix_normalize="all",
 show_hamming_loss=True, show_cohen_kappa_score=True, show_roc_auc=True,
-all_labels=[i for i in range(0, 10)], ) def cmp( self, ppl_result:
-PPLResultIterator ) -> t.Tuple[t.List[int], t.List[int], t.List[t.List
-[float]]]: result, label, pr = [], [], [] for _data in ppl_result: label.append
-(_data["ds_data"]["label"]) result.append(_data["result"][0]) pr.append(_data
-["result"][1]) return label, result, pr def _pre(self, input:bytes): """write
-some mnist preprocessing code""" def _post(self, input:bytes): """write some
-mnist post-processing code""" def _load_model(): """load your pre trained
-model""" ``` - [Code Example]Define `model.yaml`. ```yaml name: mnist run:
-handler: mnist.evaluator:MNISTInference ``` - Run one command to build the
-model. ```bash swcli model build example/mnist --runtime pytorch/version/latest
-swcli model list swcli model info mnist/version/latest ``` - ðº **STEP5**:
-Building a dataset - Download MNIST RAW data files. ```bash cd example/mnist
-make download-data # For users in the mainland of China, please add `CN=1`
-environment for make command: # CN=1 make download-data cd - ``` - [Code
-Example]Write some code with Starwhale Python SDK. Full code is [here](https://
-github.com/star-whale/starwhale/blob/main/example/mnist/mnist/dataset.py).
-```python import struct from pathlib import Path from starwhale import
-GrayscaleImage def iter_swds_bin_item(): root_dir = Path
-(__file__).parent.parent / "data" with (root_dir / "t10k-images-idx3-
-ubyte").open("rb") as data_file, ( root_dir / "t10k-labels-idx1-ubyte" ).open
-("rb") as label_file: _, data_number, height, width = struct.unpack(">IIII",
-data_file.read(16)) _, label_number = struct.unpack(">II", label_file.read(8))
-print( f">data({data_file.name}) split data:{data_number}, label:{label_number}
-group" ) image_size = height * width for i in range(0, min(data_number,
-label_number)): _data = data_file.read(image_size) _label = struct.unpack(">B",
-label_file.read(1))[0] yield { "img": GrayscaleImage( _data, display_name=f"
-{i}", shape=(height, width, 1), ), "label": _label, } ``` - Run one command to
-build the dataset. ```bash swcli dataset build example/mnist --handler
-mnist.dataset:iter_swds_bin_item --runtime pytorch/version/latest swcli dataset
-info mnist/version/latest swcli dataset head mnist/version/latest ``` Starwhale
-also supports build dataset with pure python sdk. You can try it in [Google
-Colab](https://colab.research.google.com/github/star-whale/starwhale/blob/main/
-example/notebooks/dataset-sdk.ipynb). - ð **STEP6**: Running an evaluation
-job ```bash swcli eval run --model mnist/version/latest --dataset mnist/
-version/latest --runtime pytorch/version/latest swcli eval list swcli eval info
-$(swcli eval list | grep mnist | grep success | awk '{print $1}' | head -n 1)
-``` **ð Now, you have completed the fundamental steps for Starwhale
-standalone. Let's go ahead and finish the tutorial on the on-premises
-instance.** ## MNIST Quick Tour for on-premises instance ![Create Job Workflow]
-(docs/docs/img/console-create-job.gif) - ð° **STEP1**: Install minikube and
-helm - [Minikube](https://minikube.sigs.k8s.io/docs/start/) 1.25+ - [Helm]
-(https://helm.sh/docs/intro/install/) 3.2.0+ - ðµ **STEP2**: Start minikube
-```bash minikube start ``` > For users in the mainland of China, please add
-some external parameters. The following command was well tested; you may also
-try another kubernetes version. > > ```bash > minikube start --image-mirror-
+all_labels=[i for i in range(0, 10)], ) def cmp( self, ppl_result ) -> t.Tuple
+[t.List[int], t.List[int], t.List[t.List[float]]]: result, label, pr = [], [],
+[] for _data in ppl_result: label.append(_data["ds_data"]["label"])
+result.append(_data["result"][0]) pr.append(_data["result"][1]) return label,
+result, pr def _pre(self, input:bytes): """write some mnist preprocessing
+code""" def _post(self, input:bytes): """write some mnist post-processing
+code""" def _load_model(): """load your pre trained model""" ``` - [Code
+Example]Define `model.yaml`. ```yaml name: mnist run: handler: mnist.evaluator:
+MNISTInference ``` - Run one command to build the model. ```bash swcli model
+build example/mnist --runtime pytorch/version/latest swcli model list swcli
+model info mnist/version/latest ``` - ðº **STEP5**: Building a dataset -
+Download MNIST RAW data files. ```bash cd example/mnist make download-data #
+For users in the mainland of China, please add `CN=1` environment for make
+command: # CN=1 make download-data cd - ``` - [Code Example]Write some code
+with Starwhale Python SDK. Full code is [here](https://github.com/star-whale/
+starwhale/blob/main/example/mnist/mnist/dataset.py). ```python import struct
+from pathlib import Path from starwhale import GrayscaleImage def
+iter_swds_bin_item(): root_dir = Path(__file__).parent.parent / "data" with
+(root_dir / "t10k-images-idx3-ubyte").open("rb") as data_file, ( root_dir /
+"t10k-labels-idx1-ubyte" ).open("rb") as label_file: _, data_number, height,
+width = struct.unpack(">IIII", data_file.read(16)) _, label_number =
+struct.unpack(">II", label_file.read(8)) print( f">data({data_file.name}) split
+data:{data_number}, label:{label_number} group" ) image_size = height * width
+for i in range(0, min(data_number, label_number)): _data = data_file.read
+(image_size) _label = struct.unpack(">B", label_file.read(1))[0] yield { "img":
+GrayscaleImage( _data, display_name=f"{i}", shape=(height, width, 1), ),
+"label": _label, } ``` - Run one command to build the dataset. ```bash swcli
+dataset build example/mnist --handler mnist.dataset:iter_swds_bin_item --
+runtime pytorch/version/latest swcli dataset info mnist/version/latest swcli
+dataset head mnist/version/latest ``` Starwhale also supports build dataset
+with pure python sdk. You can try it in [Google Colab](https://
+colab.research.google.com/github/star-whale/starwhale/blob/main/example/
+notebooks/dataset-sdk.ipynb). - ð **STEP6**: Running an evaluation job
+```bash swcli eval run --model mnist/version/latest --dataset mnist/version/
+latest --runtime pytorch/version/latest swcli eval list swcli eval info $(swcli
+eval list | grep mnist | grep success | awk '{print $1}' | head -n 1) ```
+**ð Now, you have completed the fundamental steps for Starwhale standalone.
+Let's go ahead and finish the tutorial on the on-premises instance.** ## MNIST
+Quick Tour for on-premises instance ![Create Job Workflow](docs/docs/img/
+console-create-job.gif) - ð° **STEP1**: Install minikube and helm -
+[Minikube](https://minikube.sigs.k8s.io/docs/start/) 1.25+ - [Helm](https://
+helm.sh/docs/intro/install/) 3.2.0+ - ðµ **STEP2**: Start minikube ```bash
+minikube start ``` > For users in the mainland of China, please add some
+external parameters. The following command was well tested; you may also try
+another kubernetes version. > > ```bash > minikube start --image-mirror-
 country=cn --kubernetes-version=1.25.3 > ``` If there is no kubectl bin in your
 machine, you may use `minikube kubectl` or `alias kubectl="minikube kubectl --
 "` alias command. - ðµ **STEP3**: Installing Starwhale ```bash helm repo add
 starwhale https://star-whale.github.io/charts helm repo update helm pull
 starwhale/starwhale --untar --untardir ./charts helm upgrade --install
 starwhale ./charts/starwhale -n starwhale --create-namespace -f ./charts/
 starwhale/values.minikube.global.yaml ``` > For users in the mainland of China,
```

### Comparing `starwhale-0.4.1/pyproject.toml` & `starwhale-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/scripts/sw-docker-entrypoint` & `starwhale-0.4.2/scripts/sw-docker-entrypoint`

 * *Files 16% similar despite different names*

```diff
@@ -56,19 +56,19 @@
     python3 -m pip config set global.cache-dir ${PIP_CACHE_DIR} || true
     python3 -m pip cache dir || true
 }
 
 set_py_and_sw() {
     pre_config
 
-    _MANIFEST_RUNTIME=$(swcli -o json runtime info ${SW_RUNTIME_VERSION} | jq -r ".config.environment.python") || exit 1
+    _MANIFEST_RUNTIME=$(swcli -o json runtime info ${SW_RUNTIME_VERSION} -of manifest | jq -r ".manifest.environment.python") || exit 1
     _RUNTIME="python${_MANIFEST_RUNTIME}"
 
     ORIGIN_SW_VER=$(swcli --version)
-    DETECTED_SW_VER=$(swcli -o json runtime info ${SW_RUNTIME_VERSION} | jq -r ".config.environment.lock.starwhale_version") || exit 1
+    DETECTED_SW_VER=$(swcli -o json runtime info ${SW_RUNTIME_VERSION} -of manifest | jq -r ".manifest.environment.lock.starwhale_version") || exit 1
     DETECTED_SW_VER=${DETECTED_SW_VER:-$ORIGIN_SW_VER}
 
     echo "**** DETECT RUNTIME: python version: ${_RUNTIME}, starwhale version: ${DETECTED_SW_VER}"
 
     # default python version
     PY_VER="python3.8"
     if [ "$_RUNTIME" = "python3.7" ] || [ "$_RUNTIME" = "python3.9" ] || [ "$_RUNTIME" = "python3.10" ] || [ "$_RUNTIME" = "python3.11" ] ; then
@@ -84,15 +84,15 @@
           echo "-->[Preparing] start to install starwhale:${DETECTED_SW_VER}"
           # install starwhale for current python
           python3 -m pip install "starwhale==${DETECTED_SW_VER}" || exit 1
         fi
     fi
 }
 
-run() {
+eval() {
     echo "-->[Running] start to run evaluation: ${STEP}, use $(which swcli) cli ..."
     if [ "${RUNTIME_RESTORED}" != "1" ]; then
         swcli ${VERBOSE} eval run --step=${STEP} --task-index=${TASK_INDEX} --override-task-num=${TASK_NUM} --model ${SW_MODEL_VERSION} --version=${SW_EVALUATION_VERSION} --runtime ${SW_RUNTIME_VERSION} || exit 1
     else
         swcli ${VERBOSE} eval run --step=${STEP} --task-index=${TASK_INDEX} --override-task-num=${TASK_NUM} --model ${SW_MODEL_VERSION} --version=${SW_EVALUATION_VERSION} || exit 1
     fi
 
@@ -104,14 +104,24 @@
     if [ "${RUNTIME_RESTORED}" != "1" ]; then
         swcli ${VERBOSE} model serve --model "${SW_MODEL_VERSION}" --runtime "${SW_RUNTIME_VERSION}" --host 0.0.0.0 || exit 1
     else
         swcli ${VERBOSE} model serve --model "${SW_MODEL_VERSION}" --host 0.0.0.0 || exit 1
     fi
 }
 
+fine_tune() {
+    echo "-->[Fine-Tuning] start to fine-tune, use $(which swcli) cli ..."
+    export
+    if [ "${RUNTIME_RESTORED}" != "1" ]; then
+        swcli ${VERBOSE} model ft --model "${SW_MODEL_VERSION}" --runtime "${SW_RUNTIME_VERSION}" || exit 1
+    else
+        swcli ${VERBOSE} model ft --model "${SW_MODEL_VERSION}" || exit 1
+    fi
+}
+
 welcome() {
     echo "===================================="
     echo "StarWhale Docker Entrypoint"
     echo "Date: `date -u +%Y-%m-%dT%H:%M:%SZ`"
     echo "Version: `swcli --version`"
     echo "Run: $1 "
     echo "Model Version: ${SW_MODEL_VERSION}"
@@ -145,17 +155,20 @@
 }
 
 welcome $1
 case "$1" in
     pre_config)
         pre_config
         ;;
-    run)
-        prepare $1 && run
+    run|evaluation)
+        prepare $1 && eval
         ;;
-    serve)
+    serve|serving)
         prepare $1 && serve
         ;;
+    fine_tune)
+        prepare $1 && fine_tune
+        ;;
     *)
         prepare "starwhale" && exec "$@"
         ;;
 esac
```

### Comparing `starwhale-0.4.1/setup.py` & `starwhale-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,16 @@
     "pyarrow>=8.0.0",
     "Jinja2>=3.1.2",
     "tenacity>=8.0.1",
     "gradio~=3.15.0",
     # for system monitor
     "psutil>=5.5.0",
     "GitPython>=3.1.24",
+    "fastapi>=0.71.0",
+    "filelock",
 ]
 
 extras_require = {
     "image": ["pillow"],
     "audio": ["soundfile"],
 }
 
@@ -67,15 +69,15 @@
     description="An MLOps Platform for Model Evaluation",
     long_description=open("../README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="MLOps, AI, Starwhale, Model Evaluation",
     url="https://github.com/star-whale/starwhale",
     license="Apache License 2.0",
     packages=find_packages(exclude=["ez_setup", "tests*"]),
-    package_data={"": ["core/runtime/template/Dockerfile.tmpl"]},
+    package_data={"": ["core/runtime/template/Dockerfile.tmpl", "web/ui/**"]},
     include_package_data=True,
     install_requires=install_requires,
     extras_require=extras_require,
     zip_safe=False,
     entry_points="""
       [console_scripts]
       swcli = starwhale.cli:cli
```

### Comparing `starwhale-0.4.1/starwhale/api/_impl/data_store.py` & `starwhale-0.4.2/starwhale/api/_impl/data_store.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,27 @@
+from __future__ import annotations
+
 import os
 import re
+import abc
+import sys
+import copy
 import json
+import time
 import atexit
 import base64
 import struct
 import urllib
-import pathlib
+import inspect
+import zipfile
 import binascii
+import tempfile
 import importlib
 import threading
+import contextlib
 from abc import ABCMeta, abstractmethod
 from http import HTTPStatus
 from typing import (
     Any,
     Set,
     cast,
     Dict,
@@ -20,58 +29,36 @@
     Type,
     Tuple,
     Union,
     Callable,
     Iterator,
     Optional,
 )
+from pathlib import Path
+from collections import UserDict, OrderedDict
 
 import dill
 import numpy as np
 import pyarrow as pa  # type: ignore
 import requests
-import pyarrow.parquet as pq  # type: ignore
+import jsonlines
 from loguru import logger
+from filelock import FileLock
+from jsonlines import Writer
 from typing_extensions import Protocol
 
 from starwhale.consts import STANDALONE_INSTANCE
 from starwhale.utils.fs import ensure_dir
 from starwhale.consts.env import SWEnv
 from starwhale.utils.dict import flatten as flatten_dict
 from starwhale.utils.error import MissingFieldError, FieldTypeOrValueError
 from starwhale.utils.retry import http_retry
 from starwhale.utils.config import SWCliConfigMixed
 
-try:
-    import fcntl
-
-    has_fcntl = True
-except ImportError:
-    has_fcntl = False
-
-
-def _check_move(src: str, dest: str) -> bool:
-    if has_fcntl:
-        with open(os.path.join(os.path.dirname(src), ".lock"), "w") as f:
-            try:
-                fcntl.flock(f, fcntl.LOCK_EX)  # type: ignore
-            except OSError:
-                return False
-            try:
-                os.rename(src, dest)
-                return True
-            finally:
-                fcntl.flock(f, fcntl.LOCK_UN)  # type: ignore
-    else:
-        # windows
-        try:
-            os.rename(src, dest)
-            return True
-        except FileExistsError:
-            return False
+datastore_table_file_ext = ".sw-datastore"
 
 
 class SwType(metaclass=ABCMeta):
     def __init__(self, name: str, pa_type: pa.DataType) -> None:
         self.name = name
         self.pa_type = pa_type
 
@@ -580,19 +567,46 @@
     def __eq__(self, other: Any) -> bool:
         return (
             isinstance(other, ColumnSchema)
             and self.name == other.name
             and self.type == other.type
         )
 
+    def dumps(self) -> Dict[str, Any]:
+        return {"name": self.name, "type": SwType.encode_schema(self.type)}
+
+    @staticmethod
+    def loads(obj: Dict[str, Any]) -> ColumnSchema:
+        return ColumnSchema(obj["name"], SwType.decode_schema(obj["type"]))
+
 
 class TableEmptyException(Exception):
     pass
 
 
+class Record(UserDict):
+    def dumps(self) -> Dict[str, Dict]:
+        return {
+            "schema": {k: SwType.encode_schema(_get_type(v)) for k, v in self.items()},
+            "data": {k: _get_type(v).encode(v) for k, v in self.items()},
+        }
+
+    @staticmethod
+    def loads(obj: Dict[str, Dict]) -> Record:
+        schema = obj["schema"]
+        data = obj["data"]
+        record = Record()
+        for k, v in schema.items():
+            record[k] = SwType.decode_schema(v).decode(data[k])
+        return record
+
+
+Records = List[Record]
+
+
 class TableSchemaDesc:
     def __init__(
         self, key_column: Optional[str], columns: Optional[List[ColumnSchema]]
     ) -> None:
         self.key_column = key_column
         self.columns = columns
 
@@ -652,126 +666,39 @@
         return (
             isinstance(other, TableSchema)
             and self.key_column == other.key_column
             and self.columns == other.columns
         )
 
 
-def _get_table_path(root_path: str, table_name: str) -> str:
-    return str(pathlib.Path(root_path) / table_name)
-
-
-def _parse_parquet_name(name: str) -> Tuple[str, int]:
-    try:
-        if name.endswith(".parquet"):
-            if name.startswith("base-"):
-                return "base", int(name[5:-8])
-            elif name.startswith("patch-"):
-                return "patch", int(name[6:-8])
-    except ValueError:
-        # ignore invalid filename
-        pass
-    return "", 0
-
-
-def _write_parquet_file(filename: str, table: pa.Table) -> None:
-    with pq.ParquetWriter(filename, table.schema) as writer:
-        writer.write_table(table)
-
-
-def _scan_parquet_file(
-    path: str,
-    columns: Optional[Dict[str, str]] = None,
-    start: Optional[Any] = None,
-    end: Optional[Any] = None,
-    keep_none: bool = False,
-    end_inclusive: bool = False,
-) -> Iterator[dict]:
-    f = pq.ParquetFile(path)
-    schema_arrow = f.schema_arrow
-    if columns is None:
-        columns = {
-            name: name
-            for name in schema_arrow.names
-            if name != "-" and not name.startswith("~")
-        }
-    schema = TableSchema.parse(f.metadata.metadata[b"schema"].decode("utf-8"))
-    key_index = schema_arrow.get_field_index(schema.key_column)
-    if key_index < 0:
-        raise RuntimeError(
-            f"key {schema.key_column} is not found in names: {schema_arrow.names}"
-        )
-    key_alias = columns.get(schema.key_column, None)
-    all_cols = [schema.key_column]
-    if schema_arrow.get_field_index("-") >= 0:
-        all_cols.append("-")
-    for name, alias in columns.items():
-        if (
-            name != schema.key_column
-            and name != "-"
-            and schema_arrow.get_field_index(name) >= 0
-        ):
-            all_cols.append(name)
-    for name in schema_arrow.names:
-        if name.startswith("~") and name[1:] in columns:
-            all_cols.append(name)
-
-    for i in range(f.num_row_groups):
-        stats = f.metadata.row_group(i).column(key_index).statistics
-        _end_check: Callable = lambda x, y: x > y if end_inclusive else x >= y
-        if (end is not None and _end_check(stats.min, end)) or (
-            start is not None and stats.max < start
-        ):
-            continue
-        table = f.read_row_group(i, all_cols)
-        names = table.schema.names
-        types = [schema.columns[name].type for name in names]
-        n_rows = table[0].length()
-        n_cols = len(names)
-        for j in range(n_rows):
-            key = types[0].deserialize(table[0][j].as_py())
-            if (start is not None and key < start) or (
-                end is not None and _end_check(key, end)
-            ):
-                continue
-            d = {"*": key}
-            if key_alias is not None:
-                d[key_alias] = key
-            for k in range(1, n_cols):
-                name = names[k]
-                value = types[k].deserialize(table[k][j].as_py())
-                if name == "-":
-                    if value is not None:
-                        d["-"] = value
-                elif name.startswith("~") and value:
-                    alias = columns.get(name[1:], "")
-                    if alias != "":
-                        if keep_none:
-                            d[alias] = None
-                        else:
-                            d.pop(alias, "")
-                else:
-                    alias = columns.get(name, "")
-                    if alias != "" and value is not None:
-                        d[alias] = value
-            yield d
+def _get_table_path(root_path: str | Path, table_name: str) -> Path:
+    """
+    get table path from table name, return the matched file path if there is only one file match the table name
+    """
+    expect_prefix = Path(root_path) / (table_name.strip("/") + datastore_table_file_ext)
+    paths = list(expect_prefix.parent.glob(f"{expect_prefix.name}*"))
+    if len(paths) > 1:
+        raise RuntimeError(f"can not find table {table_name}, get files {paths}")
+    if len(paths) == 1:
+        return paths[0]
+    return expect_prefix
 
 
 def _merge_scan(
     iters: List[Iterator[Dict[str, Any]]], keep_none: bool
 ) -> Iterator[dict]:
     class Node:
         def __init__(self, index: int, iter: Iterator[dict]) -> None:
             self.index = index
             self.iter = iter
             self.item: Optional[Dict[str, Any]] = None
             self.exhausted = False
-            self.nextItem()
+            self.next_item()
 
-        def nextItem(self) -> None:
+        def next_item(self) -> None:
             try:
                 self.item = next(self.iter)
                 self.exhausted = False
                 self.key = cast(str, self.item["*"])
             except StopIteration:
                 self.exhausted = True
                 self.item = None
@@ -792,251 +719,357 @@
                 assert item is not None
                 removal = item.pop("-", False)
                 item.pop("*", None)
                 if removal:
                     d.clear()
                 else:
                     d.update(item)
-                nodes[i].nextItem()
+                nodes[i].next_item()
         if len(d) > 0:
             d["*"] = key
             if not keep_none:
                 d = {k: v for k, v in d.items() if v is not None}
             yield d
         nodes = [node for node in nodes if not node.exhausted]
 
 
-def _get_table_files(path: str) -> List[str]:
-    ensure_dir(path)
+def _update_schema(key_column: str, record: Dict[str, Any]) -> TableSchema:
+    new_schema = TableSchema(key_column, [])
+    for col, value in record.items():
+        value_type = _get_type(value)
+        new_schema.columns[col] = ColumnSchema(col, value_type)
+    return new_schema
 
-    patches = []
-    base_index = -1
-    for file in os.listdir(path):
-        type, index = _parse_parquet_name(file)
-        if type == "base" and index > base_index:
-            base_index = index
-        elif type == "patch":
-            patches.append(index)
-    if base_index >= 0:
-        ret = [os.path.join(path, f"base-{base_index}.parquet")]
-    else:
-        ret = []
-    patches.sort()
-    for i in patches:
-        if i > base_index:
-            ret.append(os.path.join(path, f"patch-{i}.parquet"))
-    return ret
 
+class InnerRecord:
+    def __init__(self, key_column: str, record: Optional[Record] = None) -> None:
+        self.key = ""
+        self.key_column = key_column
+        self.records: OrderedDict[int, Record] = OrderedDict()
+        self.ordered = True
+        if record is not None:
+            self.append(record)
+
+    def append(self, record: Record) -> str:
+        if not self.key:
+            self.key = record[self.key_column]
+        seq = self._get_seq_num()
+        if len(self.records) > 0:
+            last = self.get_record()
+            # get diff of the last and record
+            # let the record only contains the diff or None
+            diff = {
+                k: v for k, v in record.items() if v is None or last.get(k, None) != v
+            }
+            if not diff:
+                return str(seq)
+            record = Record(diff)
+        self.ordered = False
+        self.records[seq] = record
+        return str(seq)
+
+    def update(self, other: InnerRecord | None) -> None:
+        if other is None:
+            return
+        self.records.update(other.records)
+
+    def _reorder(self) -> None:
+        if not self.ordered:
+            self.records = OrderedDict(sorted(self.records.items()))
+            self.ordered = True
+
+    def get_record(
+        self, revision: Optional[str] = None, deep_copy: Optional[bool] = None
+    ) -> Dict[str, Any]:
+        self._reorder()
+        ret: Dict[str, Any] = dict()
+        for seq, record in self.records.items():
+            if revision is None or revision == "" or seq <= int(revision):
+                if "-" in record and record["-"]:
+                    ret = record.data
+                else:
+                    if "-" in ret:
+                        ret = dict()
+                    ret.update(record)
+        ret.update({self.key_column: self.key})
+        if deep_copy:
+            ret = copy.deepcopy(ret)
+        return ret
 
-def _read_table_schema(path: str) -> TableSchema:
-    ensure_dir(path)
+    def dumps(self) -> Dict[str, Any]:
+        self._reorder()
+        return {
+            "key": self.key_column,
+            "records": {seq: record.dumps() for seq, record in self.records.items()},
+        }
 
-    files = _get_table_files(path)
-    if len(files) == 0:
-        raise TableEmptyException(f"table path: {path}")
-
-    schema = pq.read_schema(files[-1])
-    if schema.metadata is None:
-        raise RuntimeError(f"no metadata for file {files[-1]}")
-
-    schema_data = schema.metadata.get(b"schema", None)
-    if schema_data is None:
-        raise RuntimeError(f"no schema for file {files[-1]}")
-
-    return TableSchema.parse(schema_data.decode())
-
-
-def _scan_table(
-    path: str,
-    columns: Optional[Dict[str, str]] = None,
-    start: Optional[Any] = None,
-    end: Optional[Any] = None,
-    keep_none: bool = False,
-    end_inclusive: bool = False,
-) -> Iterator[dict]:
-    iters = []
-    for file in _get_table_files(path):
-        if os.path.basename(file).startswith("patch"):
-            keep = True
-        else:
-            keep = keep_none
-        iters.append(_scan_parquet_file(file, columns, start, end, keep, end_inclusive))
-    return _merge_scan(iters, keep_none)
-
-
-def _records_to_table(
-    schema: TableSchema, records: List[Dict[str, Any]], deletes: List[Any]
-) -> pa.Table:
-    if len(records) == 0:
-        return
-    schema = schema.copy()
-    if len(deletes) > 0:
-        schema.columns["-"] = ColumnSchema("-", BOOL)
-        for key in deletes:
-            records.append({schema.key_column: key, "-": True})
-    records.sort(key=lambda x: cast(str, x.get(schema.key_column)), reverse=True)
-    d: Dict[str, Any] = {}
-    nulls: Dict[str, List[int]] = {}
-    for i in range(len(records)):
-        record = records[len(records) - 1 - i]
-        for col, col_schema in schema.columns.items():
-            if col in record:
-                value = record.get(col)
-                if value is None:
-                    nulls.setdefault(col, []).append(i)
-            else:
-                value = None
-            d.setdefault(col, []).append(col_schema.type.serialize(value))
-    for col, indexes in nulls.items():
-        schema.columns["~" + col] = ColumnSchema("~" + col, BOOL)
-        data = [False] * len(records)
-        for i in indexes:
-            data[i] = True
-        d["~" + col] = data
-    pa_schema = pa.schema(
-        [(k, v.type.pa_type) for k, v in schema.columns.items()],
-        {"schema": str(schema)},
-    )
-    return pa.Table.from_pydict(d, schema=pa_schema)
+    @staticmethod
+    def loads(data: Dict[str, Any]) -> InnerRecord:
+        ret = InnerRecord(data["key"])
+        ret.ordered = False
+        ret.records = OrderedDict(
+            {int(seq): Record.loads(record) for seq, record in data["records"].items()}
+        )
+        first = ret.records[next(iter(ret.records))]
 
+        ret.key = first[data["key"]]
+        return ret
 
-def _update_schema(schema: TableSchema, record: Dict[str, Any]) -> TableSchema:
-    new_schema = schema.copy()
-    for col, value in record.items():
-        value_type = _get_type(value)
-        column_schema = schema.columns.get(col, None)
-        if column_schema is None:
-            new_schema.columns[col] = ColumnSchema(col, value_type)
-        else:
+    @staticmethod
+    def _get_seq_num() -> int:
+        return time.monotonic_ns()
+
+
+class Compressor(abc.ABC):
+    @abc.abstractmethod
+    def extension(self) -> str:
+        """
+        Return the extension of the compressed file.
+        """
+        ...
+
+    @abc.abstractmethod
+    def compress(self, source: Path) -> Path:
+        """
+        Compress the file and return the path to the compressed file.
+        """
+        ...
+
+    @contextlib.contextmanager
+    @abc.abstractmethod
+    def decompress(self, source: Path) -> Iterator[Path]:
+        """
+        Decompress the file and return the path to the temp decompressed file.
+        And the temp file will be deleted after the context manager exits.
+        """
+        ...
+
+
+class NoCompressor(Compressor):
+    def extension(self) -> str:
+        return ".json"
+
+    def compress(self, source: Path) -> Path:
+        # never be called
+        # we need to duplicate the file because the dump method will remove the source file
+        raise RuntimeError("should not be called")
+
+    @contextlib.contextmanager
+    def decompress(self, source: Path) -> Iterator[Path]:
+        # compatible with the existing json file
+        yield source
+
+
+class ZipCompressor(Compressor):
+    def extension(self) -> str:
+        return ".zip"
+
+    def compress(self, source: Path) -> Path:
+        # use the same dir as the source file
+        output = source.with_suffix(self.extension())
+        with zipfile.ZipFile(output, "w", compression=zipfile.ZIP_DEFLATED) as zipf:
+            zipf.write(source, source.name)
+        return Path(output)
+
+    @contextlib.contextmanager
+    def decompress(self, source: Path) -> Iterator[Path]:
+        with zipfile.ZipFile(source, "r") as zipf:
+            # extract to tmp dir
+            tmp_dir = tempfile.TemporaryDirectory()
+            zipf.extractall(tmp_dir.name)
+            file_name = zipf.namelist()[0]
             try:
-                new_schema.columns[col].type = new_schema.columns[col].type.merge(
-                    value_type
-                )
-            except RuntimeError as e:
-                raise RuntimeError(f"can not insert a record with field {col}") from e
+                yield Path(tmp_dir.name) / file_name
+            finally:
+                tmp_dir.cleanup()
+
+
+# get all the compressors in this module
+compressors: Dict[str, Compressor] = {}
+for name, obj in inspect.getmembers(sys.modules[__name__]):
+    if inspect.isclass(obj) and issubclass(obj, Compressor) and obj != Compressor:
+        compressors[obj.__name__] = obj()
 
-    return new_schema
+
+def get_compressor(file: Path) -> Compressor:
+    for compressor in compressors.values():
+        if file.suffix == compressor.extension():
+            return compressor
+    raise ValueError(f"Unknown compressor for file {file}")
 
 
 class MemoryTable:
-    def __init__(self, table_name: str, schema: TableSchema) -> None:
+    def __init__(self, table_name: str, key_column: ColumnSchema) -> None:
         self.table_name = table_name
-        self.schema = schema.copy()
-        self.records: Dict[Any, Dict[str, Any]] = {}
-        self.deletes: Set[Any] = set()
+        self.key_column = key_column
+        self.records: Dict[Any, InnerRecord] = {}
         self.lock = threading.Lock()
-
-    def get_schema(self) -> TableSchema:
-        with self.lock:
-            return self.schema.copy()
+        self.dirty = False
+        self.compressor = ZipCompressor()
 
     def scan(
         self,
         columns: Optional[Dict[str, str]] = None,
         start: Optional[Any] = None,
         end: Optional[Any] = None,
         keep_none: bool = False,
         end_inclusive: bool = False,
+        revision: Optional[str] = None,
+        deep_copy: Optional[bool] = None,
     ) -> Iterator[Dict[str, Any]]:
         _end_check: Callable = lambda x, y: x <= y if end_inclusive else x < y
+        if deep_copy is None:
+            env = os.getenv("SW_DATASTORE_SCAN_DEEP_COPY")
+            # make deep copy to True as default if env is not set
+            deep_copy = True if env is None else env.strip().upper() == "TRUE"
 
         with self.lock:
-            schema = self.schema.copy()
-
             records = []
-            for key in self.deletes:
-                if (start is None or key >= start) and (
-                    end is None or _end_check(key, end)
-                ):
-                    records.append({self.schema.key_column: key, "-": True})
-
             for k, v in self.records.items():
                 if (start is None or k >= start) and (
                     end is None or _end_check(k, end)
                 ):
                     records.append(v)
-        records.sort(key=lambda x: cast(str, x[self.schema.key_column]))
-        for r in records:
+        records.sort(key=lambda x: x.key)
+        for ir in records:
+            r = ir.get_record(revision, deep_copy)
             if columns is None:
                 d = dict(r)
             else:
                 d = {columns[k]: v for k, v in r.items() if k in columns}
                 if "-" in r:
                     d["-"] = r["-"]
-            d["*"] = r[schema.key_column]
+            d["*"] = r[self.key_column.name]
             if not keep_none:
                 d = {k: v for k, v in d.items() if v is not None}
             yield d
 
-    def insert(self, record: Dict[str, Any]) -> None:
+    def insert(self, record: Dict[str, Any]) -> str:
+        self.dirty = True
         with self.lock:
-            self.schema = _update_schema(self.schema, record)
-            key = record.get(self.schema.key_column)
-            r = self.records.setdefault(key, record)
-            if r is not record:
-                r.update(record)
-
-    def delete(self, keys: List[Any]) -> None:
+            key = record.get(self.key_column.name)
+            r = self.records.setdefault(key, InnerRecord(self.key_column.name))
+            return r.append(Record(copy.deepcopy(record)))
+
+    def delete(self, keys: List[Any]) -> str | None:
+        """
+        Delete records by keys. If the key is not found, it will be ignored.
+        Returns the sequence number of the last delete operation, or None if no delete operation is performed.
+        """
+        revision = None
         with self.lock:
             for key in keys:
-                self.deletes.add(key)
-                self.records.pop(key, None)
+                r = self.records.get(key, None)
+                if r is not None:
+                    self.dirty = True
+                    revision = r.append(Record({self.key_column.name: key, "-": True}))
+        return revision
+
+    def _dump_meta(self) -> Dict[str, Any]:
+        return {
+            "key_column": self.key_column.dumps(),
+            "version": "0.1",
+        }
 
-    def dump(self, root_path: str) -> None:
-        with self.lock:
-            schema = self.schema.copy()
-        path = _get_table_path(root_path, self.table_name)
-        ensure_dir(path)
-        while True:
-            max_index = -1
-            for file in os.listdir(path):
-                type, index = _parse_parquet_name(file)
-                if type != "" and index > max_index:
-                    max_index = index
-            if max_index < 0:
-                filename = "base-0.parquet"
-            else:
-                filename = f"base-{max_index + 1}.parquet"
-            temp_filename = f"temp.{os.getpid()}"
-            if max_index >= 0:
-                s = _read_table_schema(os.path.join(path))
-                s.merge(schema)
-                schema = s
-            _write_parquet_file(
-                os.path.join(path, temp_filename),
-                _records_to_table(
-                    schema,
-                    list(
-                        _merge_scan(
-                            [
-                                _scan_table(path, keep_none=True),
-                                self.scan(keep_none=True),
-                            ],
-                            True,
-                        )
-                    ),
-                    [],
-                ),
-            )
-            if _check_move(
-                os.path.join(path, temp_filename), os.path.join(path, filename)
-            ):
-                break
+    @classmethod
+    def _parse_meta(cls, meta: Any) -> ColumnSchema:
+        if not isinstance(meta, dict):
+            raise RuntimeError(f"Invalid meta data {meta}")
+        if meta["version"] != "0.1":
+            raise ValueError(f"Unsupported version {meta['version']}")
+        return ColumnSchema.loads(meta["key_column"])
+
+    @classmethod
+    def loads(cls, file: Path, table_name: str) -> MemoryTable:
+        if not file.exists() or not file.is_file():
+            raise RuntimeError(f"File {file} does not exist")
+
+        with get_compressor(file).decompress(file) as f:
+            with jsonlines.open(f) as reader:
+                meta = reader.read()
+                key_column = cls._parse_meta(meta)
+                table = MemoryTable(table_name, key_column)
+                for record in reader:
+                    ir = InnerRecord.loads(record)
+                    table.records[ir.key] = ir
+        return table
+
+    def dump(self, root_path: str, if_dirty: bool = True) -> None:
+        root = Path(root_path)
+        lock = root / ".lock"
+        with FileLock(lock):
+            return self._dump(root, if_dirty)
+
+    def _dump(self, root_path: Path, if_dirty: bool = True) -> None:
+        if if_dirty and not self.dirty:
+            return
+
+        dst = Path(_get_table_path(root_path, self.table_name))
+        base = dst.parent
+        temp_filename = base / f"temp.{os.getpid()}"
+        ensure_dir(base)
+
+        with jsonlines.open(temp_filename, mode="w") as writer:
+            writer.write(self._dump_meta())
+            dumped_keys = self._dump_from_local_file(dst, writer)
+
+            for k, ir in self.records.items():
+                if k in dumped_keys:
+                    continue
+                writer.write(ir.dumps())
+
+        compressed = self.compressor.compress(temp_filename)
+        os.unlink(temp_filename)
+        if dst.suffix == datastore_table_file_ext:
+            # the dst file is must not exist, we never save a table as a sw-datastore file
+            # use the same extension as compressed file
+            ext = datastore_table_file_ext + self.compressor.extension()
+        else:
+            # the dst file is a compressed file, change the extension
+            ext = self.compressor.extension()
+
+        # make dst file have the same extension as compressed file
+        new_dst = dst.with_suffix(ext)
+        os.rename(compressed, new_dst)
+        if new_dst != dst and dst.exists():
+            # remove the old file if it is not the new file name
+            dst.unlink()
+        self.dirty = False
+
+    def _dump_from_local_file(self, existing: Path, output: Writer) -> Set[str]:
+        dumped_keys: Set[str] = set()
+
+        if not existing.exists():
+            return dumped_keys
+
+        with get_compressor(existing).decompress(existing) as f:
+            with jsonlines.open(f, mode="r") as reader:
+                self._parse_meta(reader.read())
+                for i in reader:
+                    ir = InnerRecord.loads(i)
+                    r = self.records.get(ir.key)
+                    ir.update(r)
+                    dumped_keys.add(ir.key)
+                    output.write(ir.dumps())
+
+        return dumped_keys
 
 
 class TableDesc:
     def __init__(
         self,
         table_name: str,
         columns: Union[Dict[str, str], List[str], None] = None,
         keep_none: bool = False,
+        revision: Optional[str] = None,
     ) -> None:
         self.table_name = table_name
         self.columns: Optional[Dict[str, str]] = None
         self.keep_none = keep_none
+        self.revision = revision
         if columns is not None:
             self.columns = {}
             if isinstance(columns, dict):
                 alias_map: Dict[str, str] = {}
                 for col, alias in columns.items():
                     key = alias_map.setdefault(alias, col)
                     if key != col:
@@ -1057,14 +1090,16 @@
         if self.columns is not None:
             ret["columns"] = [
                 {"columnName": col, "alias": alias}
                 for col, alias in self.columns.items()
             ]
         if self.keep_none:
             ret["keepNone"] = True
+        if self.revision is not None:
+            ret["revision"] = self.revision
         return ret
 
 
 class LocalDataStore:
     _instance = None
     _lock = threading.Lock()
 
@@ -1090,53 +1125,69 @@
         self.lock = threading.Lock()
 
     def update_table(
         self,
         table_name: str,
         schema: TableSchema,
         records: List[Dict[str, Any]],
-    ) -> None:
+    ) -> str:
+        if len(records) == 0:
+            return ""
         if self.name_pattern.match(table_name) is None:
             raise RuntimeError(
                 f"invalid table name {table_name}, only letters(A-Z, a-z), digits(0-9), hyphen('-'), and underscore('_') are allowed"
             )
         for r in records:
             for k in r.keys():
                 if k != "-" and self.name_pattern.match(k) is None:
                     raise RuntimeError(
                         f"invalid column name {k}, only letters(A-Z, a-z), digits(0-9), hyphen('-'), and underscore('_') are allowed"
                     )
-        table = self._get_table(table_name, schema)
-        if schema.key_column != table.schema.key_column:
+        table = self._get_table(table_name, schema.columns[schema.key_column])
+        # this will never happen, makes mypy happy
+        if table is None:
             raise RuntimeError(
-                f"invalid key column, expected {table.schema.key_column}, actual {schema.key_column}"
+                f"table {table_name} does not exist and can not be created"
+            )
+        if schema.key_column != table.key_column.name:
+            raise RuntimeError(
+                f"invalid key column, expected {table.key_column}, actual {schema.key_column}"
             )
 
+        revision = None
         for r in records:
             key = r.get(schema.key_column, None)
             if key is None:
                 raise RuntimeError(
                     f"key {schema.key_column} should not be none, record: {r.keys()}"
                 )
             if "-" in r:
-                table.delete([key])
+                revision = table.delete([key])
             else:
-                table.insert(r)
-
-    def _get_table(self, table_name: str, schema: TableSchema) -> MemoryTable:
+                revision = table.insert(r)
+        # revision will never be None or empty (len(records) > 0), makes mypy happy
+        return revision or ""
+
+    def _get_table(
+        self, table_name: str, key_column: ColumnSchema | None, create: bool = True
+    ) -> MemoryTable | None:
         with self.lock:
             table = self.tables.get(table_name, None)
             if table is None:
-                table_path = _get_table_path(self.root_path, table_name)
-                if _get_table_files(table_path):
-                    table_schema = _read_table_schema(table_path)
-                    table_schema.merge(schema)
+                file = Path(_get_table_path(self.root_path, table_name))
+                if file.exists():
+                    table = MemoryTable.loads(file, table_name)
                 else:
-                    table_schema = schema
-                table = MemoryTable(table_name, table_schema)
+                    if not create:
+                        return None
+                    if key_column is None:
+                        raise RuntimeError(
+                            f"key column is required for table {table_name}"
+                        )
+                    table = MemoryTable(table_name, key_column)
                 self.tables[table_name] = table
         return table
 
     def scan_tables(
         self,
         tables: List[TableDesc],
         start: Optional[Any] = None,
@@ -1144,101 +1195,64 @@
         keep_none: bool = False,
         end_inclusive: bool = False,
     ) -> Iterator[Dict[str, Any]]:
         class TableInfo:
             def __init__(
                 self,
                 name: str,
-                key_column_type: pa.DataType,
+                key_column_type: SwType,
                 columns: Optional[Dict[str, str]],
                 keep_none: bool,
+                revision: Optional[str],
             ) -> None:
                 self.name = name
                 self.key_column_type = key_column_type
                 self.columns = columns
                 self.keep_none = keep_none
+                self.revision = revision
 
         infos: List[TableInfo] = []
         for table_desc in tables:
-            table = self.tables.get(table_desc.table_name, None)
-            if table is not None:
-                schema = table.get_schema()
-            else:
-                schema = _read_table_schema(
-                    _get_table_path(self.root_path, table_desc.table_name)
-                )
-            key_column_type = schema.columns[schema.key_column].type.pa_type
+            table = self._get_table(table_desc.table_name, None, create=False)
+            if table is None:
+                continue
+            key_column_type = table.key_column.type
             infos.append(
                 TableInfo(
                     table_desc.table_name,
                     key_column_type,
                     table_desc.columns,
                     table_desc.keep_none,
+                    table_desc.revision,
                 )
             )
 
-        # check for key type conflictions
+        # check for key type conflicts
         for info in infos:
             if info is infos[0]:
                 continue
             if info.key_column_type != infos[0].key_column_type:
                 raise RuntimeError(
                     "conflicting key field type. "
                     f"{info.name} has a key of type {info.key_column_type},"
                     f" while {infos[0].name} has a key of type {infos[0].key_column_type}"
                 )
 
         iters = []
         for info in infos:
-            table_path = _get_table_path(self.root_path, info.name)
-            if info.name in self.tables:
-                if _get_table_files(table_path):
-                    iters.append(
-                        _merge_scan(
-                            [
-                                _scan_table(
-                                    table_path,
-                                    info.columns,
-                                    start,
-                                    end,
-                                    info.keep_none,
-                                    end_inclusive,
-                                ),
-                                self.tables[info.name].scan(
-                                    info.columns,
-                                    start,
-                                    end,
-                                    True,
-                                    end_inclusive,
-                                ),
-                            ],
-                            info.keep_none,
-                        )
-                    )
-                else:
-                    iters.append(
-                        self.tables[info.name].scan(
-                            info.columns,
-                            start,
-                            end,
-                            info.keep_none,
-                            end_inclusive,
-                        )
-                    )
-            else:
-                iters.append(
-                    _scan_table(
-                        table_path,
-                        info.columns,
-                        start,
-                        end,
-                        info.keep_none,
-                        end_inclusive,
-                    )
+            iters.append(
+                self.tables[info.name].scan(
+                    info.columns,
+                    start,
+                    end,
+                    info.keep_none,
+                    end_inclusive,
+                    revision=info.revision,
                 )
+            )
         for record in _merge_scan(iters, keep_none):
             record.pop("*", None)
             r: Dict[str, Any] = {}
             for k, v in record.items():
                 if k != "*":
                     r[k] = v
             yield r
@@ -1266,15 +1280,15 @@
 
     @http_retry
     def update_table(
         self,
         table_name: str,
         schema: TableSchema,
         records: List[Dict[str, Any]],
-    ) -> None:
+    ) -> str:
         data: Dict[str, Any] = {"tableName": table_name}
         column_schemas = []
         for col in schema.columns.values():
             d = SwType.encode_schema(col.type)
             d["name"] = col.name
             column_schemas.append(d)
         data["tableSchemaDesc"] = {
@@ -1307,14 +1321,15 @@
         )
 
         if resp.status_code != HTTPStatus.OK:
             logger.error(
                 f"[update-table]Table:{table_name}, resp code:{resp.status_code}, \n resp text: {resp.text}, \n records: {records}"
             )
         resp.raise_for_status()
+        return resp.json()["data"]  # type: ignore
 
     @http_retry
     def _do_scan_table_request(self, post_data: Dict[str, Any]) -> Dict[str, Any]:
         resp = requests.post(
             urllib.parse.urljoin(self.instance_uri, "/api/v1/datastore/scanTable"),
             data=json.dumps(post_data, separators=(",", ":")),
             headers={
@@ -1376,15 +1391,18 @@
 
 class DataStore(Protocol):
     def update_table(
         self,
         table_name: str,
         schema: TableSchema,
         records: List[Dict[str, Any]],
-    ) -> None:
+    ) -> str:
+        """
+        Update a table with records, and return the revision of the table.
+        """
         ...
 
     def scan_tables(
         self,
         tables: List[TableDesc],
         start: Optional[Any] = None,
         end: Optional[Any] = None,
@@ -1420,21 +1438,22 @@
         table_name: str,
         key_column: str = "id",
         data_store: Optional[DataStore] = None,
         run_exceptions_limits: int = 100,
     ) -> None:
         super().__init__(name=f"TableWriter-{table_name}")
         self.table_name = table_name
-        self.schema = TableSchema(key_column, [])
+        self.key_column = key_column
         self.data_store = data_store or get_data_store()
+        self.latest_revision = ""
 
         self._cond = threading.Condition()
         self._stopped = False
-        self._records: List[Dict[str, Any]] = []
-        self._updating_records: List[Dict[str, Any]] = []
+        self._records: List[Tuple[TableSchema, List[Dict[str, Any]]]] = []
+        self._updating_records: List[Tuple[TableSchema, List[Dict[str, Any]]]] = []
         self._queue_run_exceptions: List[Exception] = []
         self._run_exceptions_limits = max(run_exceptions_limits, 0)
 
         self.daemon = True
         atexit.register(self.close)
         self.start()
 
@@ -1471,49 +1490,69 @@
                     and ch != ":"
                     and not ch.isspace()
                 ):
                     raise RuntimeError(f"invalid field {k}")
         self._insert(record)
 
     def delete(self, key: Any) -> None:
-        self._insert({self.schema.key_column: key, "-": True})
+        self._insert({self.key_column: key, "-": True})
 
     def _insert(self, record: Dict[str, Any]) -> None:
         self._raise_run_exceptions(self._run_exceptions_limits)
 
-        key = record.get(self.schema.key_column, None)
+        key = record.get(self.key_column, None)
         if key is None:
             raise RuntimeError(
-                f"the key {self.schema.key_column} should not be none, record:{record}"
+                f"the key {self.key_column} should not be none, record:{record}"
             )
         with self._cond:
-            self.schema = _update_schema(self.schema, record)
-            self._records.append(record)
+            schema = _update_schema(self.key_column, record)
+            # TODO: group the records with the same schema
+            self._records.append((schema, [record]))
             self._cond.notify()
 
-    def flush(self) -> None:
+    def flush(self) -> str:
+        """
+        Flush the records to the data store, and return the revision of the table.
+        """
         while True:
             with self._cond:
                 if len(self._records) == 0 and len(self._updating_records) == 0:
                     break
+            time.sleep(0.1)
+        return self.latest_revision
 
     def run(self) -> None:
         while True:
             with self._cond:
                 while not self._stopped and len(self._records) == 0:
                     self._cond.wait()
                 if len(self._records) == 0:
                     break
                 self._updating_records = self._records
                 self._records = []
 
             try:
-                self.data_store.update_table(
-                    self.table_name, self.schema, self._updating_records
-                )
+                to_submit: List[Dict[str, Any]] = []
+                last_schema = None
+                for schema, records in self._updating_records:
+                    # group the records with the same schema
+                    if last_schema is None:
+                        last_schema = schema
+                    elif last_schema != schema:
+                        self.latest_revision = self.data_store.update_table(
+                            self.table_name, last_schema, to_submit
+                        )
+                        to_submit = []
+                        last_schema = schema
+                    to_submit.extend(records)
+                if len(to_submit) > 0 and last_schema is not None:
+                    self.latest_revision = self.data_store.update_table(
+                        self.table_name, last_schema, to_submit
+                    )
             except Exception as e:
                 logger.exception(e)
                 self._queue_run_exceptions.append(e)
                 if len(self._queue_run_exceptions) > self._run_exceptions_limits:
                     break
             finally:
                 self._updating_records = []
```

### Comparing `starwhale-0.4.1/starwhale/api/_impl/dataset/__init__.py` & `starwhale-0.4.2/starwhale/api/_impl/dataset/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,27 +19,23 @@
     GrayscaleImage,
     LocalFSLinkAuth,
     DefaultS3LinkAuth,
     COCOObjectAnnotation,
 )
 
 from .model import Dataset
-from .loader import get_data_loader
-from .builder import BuildExecutor
 
 __all__ = [
-    "get_data_loader",
     "Link",
     "LinkAuth",
     "DefaultS3LinkAuth",
     "LocalFSLinkAuth",
     "S3LinkAuth",
     "MIMEType",
     "LinkType",
-    "BuildExecutor",
     "Binary",
     "NumpyBinary",
     "Text",
     "Line",
     "Point",
     "Polygon",
     "Audio",
```

### Comparing `starwhale-0.4.1/starwhale/api/_impl/dataset/builder.py` & `starwhale-0.4.2/starwhale/core/dataset/tabular.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,583 +1,614 @@
 from __future__ import annotations
 
-import io
 import os
-import time
-import queue
-import struct
+import json
 import typing as t
-import inspect
-import tempfile
+import urllib
 import threading
-from abc import ABCMeta, abstractmethod
+from copy import deepcopy
+from enum import Enum, unique
+from queue import Queue
 from types import TracebackType
-from pathlib import Path
-from binascii import crc32
+from functools import partial
+from collections import UserDict, defaultdict
 
-import jsonlines
+import requests
 from loguru import logger
 from typing_extensions import Protocol
 
-from starwhale.consts import DEFAULT_PROJECT, STANDALONE_INSTANCE
+from starwhale.utils import validate_obj_name
+from starwhale.consts import ENV_POD_NAME, STANDALONE_INSTANCE
 from starwhale.base.uri import URI
-from starwhale.utils.fs import empty_dir, ensure_dir
-from starwhale.base.type import InstanceType, DataFormatType, DataOriginType
-from starwhale.utils.error import FormatError, NoSupportError
-from starwhale.core.dataset import model
-from starwhale.core.dataset.type import (
-    Link,
-    MIMEType,
-    DatasetSummary,
-    D_ALIGNMENT_SIZE,
-    D_FILE_VOLUME_SIZE,
+from starwhale.base.type import URIType, InstanceType
+from starwhale.base.mixin import ASDictMixin, _do_asdict_convert
+from starwhale.consts.env import SWEnv
+from starwhale.utils.error import (
+    FormatError,
+    NoSupportError,
+    InvalidObjectName,
+    FieldTypeOrValueError,
 )
-from starwhale.core.dataset.store import DatasetStorage
-from starwhale.core.dataset.tabular import TabularDataset, TabularDatasetRow
-from starwhale.api._impl.dataset.loader import DataRow
-
-# TODO: tune header size
-_header_magic = struct.unpack(">I", b"SWDS")[0]
-_data_magic = struct.unpack(">I", b"SDWS")[0]
-_header_struct = struct.Struct(">IIQIIII")
-_header_size = _header_struct.size
-_header_version = 0
-
-_BDType = t.TypeVar("_BDType", bound="BaseBuildExecutor")
+from starwhale.utils.retry import http_retry
+from starwhale.utils.config import SWCliConfigMixed
+from starwhale.api._impl.wrapper import Dataset as DatastoreWrapperDataset
+from starwhale.api._impl.wrapper import DatasetTableKind
+from starwhale.core.dataset.type import Link, JsonDict, BaseArtifact
+from starwhale.api._impl.data_store import TableEmptyException
+
+DEFAULT_CONSUMPTION_BATCH_SIZE = 50
+
+_DR_DATA_KEY = "data_datastore_revision"
+_DR_INFO_KEY = "info_datastore_revision"
+
+
+class DatastoreRevision(t.NamedTuple):
+    data: str
+    info: str
+
+    def asdict(self) -> t.Dict:
+        return {
+            _DR_DATA_KEY: self.data,
+            _DR_INFO_KEY: self.info,
+        }
 
+    @classmethod
+    def from_manifest(cls, manifest: t.Dict | None) -> DatastoreRevision:
+        manifest = manifest or {}
+        return DatastoreRevision(
+            data=manifest.get(_DR_DATA_KEY, ""),
+            info=manifest.get(_DR_INFO_KEY, ""),
+        )
 
-class BinWriter(Protocol):
-    total_bin_size: int
 
-    def write_row(self, row: TabularDatasetRow) -> None:
-        """
-        Find large bytes or local fs file in row data. Convert them to accessible link
-        """
-        ...
+class TabularDatasetInfo(UserDict):
+    _ROW_ID = 0
 
-    def flush(self) -> None:
-        ...
+    def __init__(self, mapping: t.Any = None, **kwargs: t.Any) -> None:
+        mapping = mapping or {}
+        if not isinstance(mapping, dict):
+            raise TypeError(f"data is not dict type: {mapping}")
+
+        if kwargs:
+            mapping.update(kwargs)
+
+        converted_mapping: t.Dict[str, t.Any] = {}
+        for k, v in mapping.items():
+            if not isinstance(k, str):
+                raise TypeError(f"key:{k} is not str type")
+
+            # TODO： add validator for value?
+            converted_mapping[k] = JsonDict.from_data(v)
+        super().__init__(converted_mapping)
+
+    def __getitem__(self, k: str) -> t.Any:
+        return JsonDict.to_data(super().__getitem__(k))
+
+    def __setitem__(self, k: str, v: t.Any) -> None:
+        if not isinstance(k, str):
+            raise TypeError(f"key:{k} is not str type")
+        super().__setitem__(k, JsonDict.from_data(v))
+
+    @classmethod
+    def load_from_datastore(
+        cls, ds_wrapper: DatastoreWrapperDataset
+    ) -> TabularDatasetInfo:
+        try:
+            rows = list(ds_wrapper.scan(cls._ROW_ID, cls._ROW_ID, end_inclusive=True))
+            rows_cnt = len(rows)
+            if rows_cnt == 1:
+                d = rows[0]
+            elif rows_cnt > 1:
+                raise RuntimeError(f"fetch multi info rows: {rows}")
+            else:
+                d = {}
+        except TableEmptyException:
+            d = {}
 
-    def __enter__(self) -> BinWriter:
-        return self
+        d.pop("id", None)
+        return cls(d)
 
-    def __exit__(
-        self,
-        type: t.Optional[t.Type[BaseException]],
-        value: t.Optional[BaseException],
-        trace: TracebackType,
-    ) -> None:
-        ...
+    def save_to_datastore(self, ds_wrapper: DatastoreWrapperDataset) -> str:
+        ds_wrapper.put(data_id=self._ROW_ID, **self.data)
+        return ds_wrapper.flush()
 
 
-class SWDSBinWriter:
+class TabularDatasetRow(ASDictMixin):
 
-    """
-    bin format:
-        header_magic    uint32  I
-        crc             uint32  I
-        _reserved       uint64  Q
-        size            uint32  I
-        padding_size    uint32  I
-        header_version  uint32  I
-        data_magic      uint32  I --> above 32 bytes
-        data bytes...
-        padding bytes...        --> default 4K padding
-    """
-
-    class _BinSection(t.NamedTuple):
-        offset: int
-        size: int
-        raw_data_offset: int
-        raw_data_size: int
-
-    class _SrcPathSpec(t.NamedTuple):
-        src_path: Path
-        remove_src: bool
+    _FEATURES_PREFIX = "features/"
 
     def __init__(
         self,
-        work_dir: Path,
-        data_output_dir: Path,
-        tabular_dataset: TabularDataset,
-        alignment_bytes_size: int = D_ALIGNMENT_SIZE,
-        volume_bytes_size: int = D_FILE_VOLUME_SIZE,
+        id: t.Union[str, int],
+        features: t.Optional[t.Dict[str, t.Any]] = None,
+        **kw: t.Union[str, int, float],
     ) -> None:
-        self.tabular_dataset = tabular_dataset
-        self.work_dir = work_dir
-        self.data_output_dir = data_output_dir
-        self.volume_bytes_size = volume_bytes_size
-        self.alignment_bytes_size = alignment_bytes_size
-        self.ds_copy_candidates: t.Dict[str, SWDSBinWriter._SrcPathSpec] = {}
-        self.wrote_size = 0
-        _, bin_writer_path = tempfile.mkstemp(
-            prefix="bin-writer-", dir=str(self.work_dir.absolute())
-        )
-        self.dwriter_path = Path(bin_writer_path)
-        self.dwriter = self.dwriter_path.open("wb")
-        self.total_bin_size = 0
-        self._to_update_rows: t.List[TabularDatasetRow] = []
-        self._lock = threading.Lock()
+        self.id = id
+        self.features = features or {}
+        self.extra_kw = kw
+        # TODO: add non-starwhale object store related fields, such as address, authority
+        # TODO: add data uri crc for versioning
+        self._do_validate()
+
+    @classmethod
+    def from_datastore(
+        cls,
+        id: t.Union[str, int],
+        **kw: t.Any,
+    ) -> TabularDatasetRow:
+        _content = {}
+        _extra_kw = {}
+        for k, v in kw.items():
+            if k.startswith(cls._FEATURES_PREFIX):
+                _, name = k.split(cls._FEATURES_PREFIX, 1)
+                _content[name] = JsonDict.to_data(v)
+            else:
+                _extra_kw[k] = v
 
-    def __enter__(self) -> SWDSBinWriter:
-        return self
+        return cls(
+            id=id,
+            features=_content,
+            **_extra_kw,
+        )
 
-    def __exit__(
-        self,
-        type: t.Optional[t.Type[BaseException]],
-        value: t.Optional[BaseException],
-        trace: TracebackType,
-    ) -> None:
-        if value:  # pragma: no cover
-            logger.warning(f"type:{type}, exception:{value}, traceback:{trace}")
+    def __eq__(self, o: object) -> bool:
+        s = deepcopy(self.__dict__)
+        o = deepcopy(o.__dict__)
+        return s == o
+
+    def _do_validate(self) -> None:
+        if not isinstance(self.id, (str, int)):
+            raise FieldTypeOrValueError(f"id is not int or str type: {self.id}")
+
+        if self.id == "":
+            raise FieldTypeOrValueError("id is empty")
+
+        if not isinstance(self.features, dict) or not self.features:
+            raise FieldTypeOrValueError("no data field")
+
+    def __str__(self) -> str:
+        return f"row-{self.id}"
+
+    def __repr__(self) -> str:
+        return f"row-{self.id}" f"{self.features} "
+
+    def asdict(self, ignore_keys: t.Optional[t.List[str]] = None) -> t.Dict:
+        d = super().asdict(ignore_keys=ignore_keys or ["features", "extra_kw"])
+        d.update(_do_asdict_convert(self.extra_kw))
+        for k, v in self.features.items():
+            d[f"{self._FEATURES_PREFIX}{k}"] = JsonDict.from_data(v)
+        return d
+
+    @classmethod
+    def artifacts_of(cls, features: t.Dict) -> t.List[BaseArtifact]:
+        artifacts = []
+        for v in features.values():
+            if isinstance(v, dict):
+                artifacts.extend(cls.artifacts_of(v))
+            elif isinstance(v, BaseArtifact):
+                artifacts.append(v)
+        return artifacts
 
-        self.close()
+    @property
+    def artifacts(self) -> t.List[BaseArtifact]:
+        return TabularDatasetRow.artifacts_of(self.features)
 
-    def write_row(self, row: TabularDatasetRow) -> None:
-        with self._lock:
-            artifacts = row.artifacts()
-            artifacts_with_bin = False
-            for v in artifacts:
-                if not v.link and isinstance(v.fp, (str, Path)):
-                    # convert user local file path to Starwhale link
-                    v.link = Link(v.fp, with_local_fs_data=True)
-                    #  BaseArtifact reads from BaseArtifact.fp prior to any other sources like link
-                    #  When BaseArtifact.fp is user local file path , it is unreliable and should be removed.
-                    v.fp = ""
-                if v.link and v.link.with_local_fs_data:
-                    v.link.uri = self._copy_file(v.link.uri, False)
-                if (
-                    not v.link
-                    and v.fp
-                    and (isinstance(v.fp, bytes) or isinstance(v.fp, io.IOBase))
-                ):
-                    artifacts_with_bin = True
-                    _bin_section = self._write(v.to_bytes())
-                    v.link = Link(
-                        self.dwriter_path,
-                        offset=_bin_section.raw_data_offset,
-                        size=_bin_section.raw_data_size,
-                        bin_offset=_bin_section.offset,
-                        bin_size=_bin_section.size,
-                    )
-                    v.clear_bytes()
 
-            if not artifacts_with_bin:
-                self.tabular_dataset.put(row)
-            else:
-                self._to_update_rows.append(row)
-            if self.wrote_size > self.volume_bytes_size:
-                self._roll_bin()
+_TDType = t.TypeVar("_TDType", bound="TabularDataset")
 
-    def _roll_bin(self) -> None:
-        if self.wrote_size == 0:
-            return
-        self.wrote_size = 0
-        self.dwriter.close()
-        self._update_link(self.dwriter_path, self._copy_file(self.dwriter_path, True))
-        _, bin_writer_path = tempfile.mkstemp(
-            prefix="bin-writer-", dir=str(self.work_dir.absolute())
-        )
-        self.dwriter_path = Path(bin_writer_path)
-        self.dwriter = self.dwriter_path.open("wb")
-
-    def _update_link(self, old_path: Path, new_path: str) -> None:
-        for row in self._to_update_rows:
-            artifacts = row.artifacts()
-            for at in artifacts:
-                if at.link and str(at.link.uri) == str(old_path):
-                    at.link.uri = new_path
-            self.tabular_dataset.put(row)
-        self._to_update_rows.clear()
-
-    def _write(self, data: bytes) -> SWDSBinWriter._BinSection:
-        size = len(data)
-        crc = crc32(data)  # TODO: crc is right?
-        start = self.dwriter.tell()
-        padding_size = self._get_padding_size(size + _header_size)
-
-        _header = _header_struct.pack(
-            _header_magic, crc, 0, size, padding_size, _header_version, _data_magic
-        )
-        _padding = b"\0" * padding_size
-        self.dwriter.write(_header + data + _padding)
-        _bin_section = SWDSBinWriter._BinSection(
-            offset=start,
-            size=_header_size + size + padding_size,
-            raw_data_offset=start + _header_size,
-            raw_data_size=size,
-        )
-        self.total_bin_size += _bin_section.size
-        self.wrote_size += _bin_section.size
-        return _bin_section
 
-    def _copy_file(
+class TabularDataset:
+    def __init__(
         self,
-        path: t.Union[Path, str],
-        remove_src: bool = False,
-    ) -> str:
-        _sign_name, _obj_path = DatasetStorage.save_data_file(
-            path, remove_src=remove_src
+        name: str,
+        project: str,
+        start: t.Optional[t.Any] = None,
+        end: t.Optional[t.Any] = None,
+        instance_name: str = "",
+        token: str = "",
+        data_datastore_revision: str = "",
+        info_datastore_revision: str = "",
+    ) -> None:
+        _ok, _reason = validate_obj_name(name)
+        if not _ok:
+            raise InvalidObjectName(f"{name}: {_reason}")
+        self.name = name
+
+        self.project = project
+        self.instance_name = instance_name
+
+        dwd = partial(
+            DatastoreWrapperDataset,
+            dataset_name=name,
+            project=project,
+            instance_name=instance_name,
+            token=token,
+        )
+        self._ds_wrapper = dwd(
+            kind=DatasetTableKind.META, dataset_scan_revision=data_datastore_revision
+        )
+        self._info_ds_wrapper = dwd(
+            kind=DatasetTableKind.INFO, dataset_scan_revision=info_datastore_revision
         )
 
-        _dest_path = self.data_output_dir / _sign_name[: DatasetStorage.short_sign_cnt]
-        _obj_path = _obj_path.resolve().absolute()
+        self._info_changed = False
+        self._info: t.Optional[TabularDatasetInfo] = None
+        self._info_lock = threading.Lock()
 
-        if _dest_path.exists():
-            _dest_path.unlink()
+        self.start = start
+        self.end = end
 
-        _dest_path.symlink_to(_obj_path)
-        return _sign_name
+    def __str__(self) -> str:
+        return f"Dataset Table: {self._ds_wrapper}"
 
-    def close(self) -> None:
-        with self._lock:
-            try:
-                empty = self.dwriter.tell() == 0
-                self.dwriter.close()
-                if empty:
-                    # last file is empty
-                    os.unlink(self.dwriter_path)
-                else:
-                    self._roll_bin()
-            except Exception as e:
-                print(f"data write close exception: {e}")
+    __repr__ = __str__
 
-    def flush(self) -> None:
-        with self._lock:
-            self._roll_bin()
+    def update(
+        self, row_id: t.Union[str, int], **kw: t.Union[int, str, bytes, Link]
+    ) -> None:
+        self._ds_wrapper.put(row_id, **kw)
 
-    def _get_padding_size(self, size: int) -> int:
-        remain = (size + _header_size) % self.alignment_bytes_size
-        return 0 if remain == 0 else (self.alignment_bytes_size - remain)
+    def put(self, row: TabularDatasetRow) -> None:
+        self._ds_wrapper.put(row.id, **row.asdict())
 
+    def delete(self, row_id: t.Union[str, int]) -> None:
+        self._ds_wrapper.delete(row_id)
 
-class BaseBuildExecutor(metaclass=ABCMeta):
-    def __init__(
+    def flush(self) -> t.Tuple[str, str]:
+        info_revision = ""
+        if self._info is not None and self._info_changed:
+            info_revision = self._info.save_to_datastore(self._info_ds_wrapper)
+
+        data_revision = self._ds_wrapper.flush()
+        return data_revision, info_revision
+
+    def scan(
         self,
-        dataset_name: str,
-        dataset_version: str,
-        project_name: str,
-        workdir: Path = Path("./sw_output"),
-        alignment_bytes_size: int = D_ALIGNMENT_SIZE,
-        volume_bytes_size: int = D_FILE_VOLUME_SIZE,
-        append: bool = False,
-        append_from_version: str = "",
-        append_from_uri: t.Optional[URI] = None,
-        data_mime_type: MIMEType = MIMEType.UNDEFINED,
-        instance_name: str = STANDALONE_INSTANCE,
-        bin_writer: t.Optional[BinWriter] = None,
-    ) -> None:
-        # TODO: add more docstring for args
-        # TODO: validate group upper and lower?
-        self.workdir = workdir
-        self.data_output_dir = workdir / "data"
-        ensure_dir(self.data_output_dir)
-        _tmpdir = tempfile.mkdtemp(
-            prefix=".data-tmp-", dir=str(self.workdir.absolute())
-        )
-        self.data_tmpdir = Path(_tmpdir)
-
-        self.alignment_bytes_size = alignment_bytes_size
-        self.volume_bytes_size = volume_bytes_size
-        self.default_data_mime_type = data_mime_type
-
-        self.project_name = project_name
-        self.dataset_name = dataset_name
-        self.dataset_version = dataset_version
-        self.tabular_dataset = TabularDataset(
-            dataset_name,
-            dataset_version,
-            project_name,
-            instance_name=instance_name,
-        )
-        if bin_writer:
-            self.bin_writer = bin_writer
-        else:
-            self.bin_writer = SWDSBinWriter(
-                self.data_tmpdir,
-                self.data_output_dir,
-                self.tabular_dataset,
-                self.alignment_bytes_size,
-                self.volume_bytes_size,
-            )
+        start: t.Optional[t.Any] = None,
+        end: t.Optional[t.Any] = None,
+        end_inclusive: bool = False,
+        revision: str = "",
+    ) -> t.Generator[TabularDatasetRow, None, None]:
+        if start is None or (self.start is not None and start < self.start):
+            start = self.start
 
-        self._forked_summary: t.Optional[DatasetSummary]
-        if append and append_from_uri:
-            # TODO： controller supports cloud dataset fork api
-            if append_from_uri.instance_type == InstanceType.CLOUD:
-                raise NoSupportError(
-                    f"Can't build dataset from existed cloud dataset: {append_from_uri}"
-                )
+        if end is None or (self.end is not None and end > self.end):
+            end = self.end
 
-            self._forked_last_seq_id, self._forked_rows = self.tabular_dataset.fork(
-                append_from_version
-            )
-            self._forked_summary = model.Dataset.get_dataset(append_from_uri).summary()
-        else:
-            self._forked_last_seq_id = -1
-            self._forked_rows = 0
-            self._forked_summary = None
+        for _d in self._ds_wrapper.scan(start, end, end_inclusive, revision=revision):
+            yield TabularDatasetRow.from_datastore(**_d)
 
-        self._index_writer: t.Optional[jsonlines.Writer] = None
+    def scan_batch(
+        self,
+        start: t.Optional[t.Any] = None,
+        end: t.Optional[t.Any] = None,
+        batch_size: int = 32,
+        revision: str = "",
+    ) -> t.Generator[t.List[TabularDatasetRow], None, None]:
+        batch = []
+        for r in self.scan(start, end, revision=revision):
+            batch.append(r)
+            if len(batch) % batch_size == 0:
+                yield batch
+                batch = []
+        if batch:
+            yield batch
+
+    def close(self) -> None:
+        self.flush()
+        self._ds_wrapper.close()
+        self._info_ds_wrapper.close()
 
-    def __enter__(self: _BDType) -> _BDType:
+    def __enter__(self: _TDType) -> _TDType:
         return self
 
     def __exit__(
         self,
         type: t.Optional[t.Type[BaseException]],
         value: t.Optional[BaseException],
         trace: TracebackType,
     ) -> None:
         if value:  # pragma: no cover
-            print(f"type:{type}, exception:{value}, traceback:{trace}")
-        self.close()
-
-    def close(self) -> None:
-        try:
-            self.tabular_dataset.close()
-        except Exception as e:
-            print(f"tabular dataset close exception: {e}")
-
-        try:
-            empty_dir(self.data_tmpdir)
-        except Exception as e:
-            print(f"empty {self.data_tmpdir} exception: {e}")
-
-        print("cleanup done.")
-
-    def flush(self) -> None:
-        self.bin_writer.flush()
-        self.tabular_dataset.flush()
-
-    def get_info(self) -> t.Optional[t.Dict[str, t.Any]]:
-        return None
-
-    @abstractmethod
-    def iter_item(
-        self,
-    ) -> t.Generator[t.Union[t.Tuple, t.Dict[str, t.Any]], None, None]:
-        raise NotImplementedError
+            logger.warning(f"type:{type}, exception:{value}, traceback:{trace}")
 
-    @abstractmethod
-    def make_swds(self) -> DatasetSummary:
-        raise NotImplementedError
-
-    def _merge_forked_summary(self, s: DatasetSummary) -> DatasetSummary:
-        _fs = self._forked_summary
-        if _fs:
-            s.rows += _fs.rows
-            s.unchanged_rows += _fs.rows
-            s.data_byte_size += _fs.data_byte_size
+        self.close()
 
-        return s
+    @classmethod
+    def from_uri(
+        cls: t.Type[_TDType],
+        uri: URI,
+        start: t.Optional[t.Any] = None,
+        end: t.Optional[t.Any] = None,
+        data_datastore_revision: str = "",
+        info_datastore_revision: str = "",
+    ) -> _TDType:
+        return cls(
+            name=uri.object.name,
+            project=uri.project,
+            start=start,
+            end=end,
+            instance_name=uri.instance,
+            data_datastore_revision=data_datastore_revision,
+            info_datastore_revision=info_datastore_revision,
+        )
 
     @property
-    def data_format_type(self) -> DataFormatType:
-        raise NotImplementedError
+    def info(self) -> TabularDatasetInfo:
+        if self._info is not None:
+            return self._info
+
+        with self._info_lock:
+            self._info = TabularDatasetInfo.load_from_datastore(self._info_ds_wrapper)
+        return self._info
+
+    @info.setter
+    def info(self, data: t.Optional[t.Dict[str, t.Any]]) -> None:
+        if data is None:
+            return
 
-    def _unpack_row_content(
-        self, row_data: t.Union[t.Tuple, DataRow, t.Dict], append_seq_id: int
-    ) -> t.Tuple[t.Union[str, int], t.Dict]:
-        if isinstance(row_data, DataRow):
-            idx, row = row_data.index, row_data.data
-        elif isinstance(row_data, dict):
-            idx, row = append_seq_id, row_data
-        elif isinstance(row_data, tuple):
-            if len(row_data) == 1:
-                idx = append_seq_id
-                row = row_data[0]
-            elif len(row_data) == 2:
-                idx, row = row_data
-            else:
-                raise FormatError(
-                    f"iter_item must return data, (data) or (id, data): {row_data}"
-                )
-        else:
-            raise FormatError(
-                f"row content not return tuple or DataRow type: {row_data}"
+        if not isinstance(data, dict):
+            raise TypeError(
+                f"data:{type(data)} {data} is not dict type for info update"
             )
 
-        if not isinstance(row, dict):
-            raise FormatError(f"content({row}) must be dict type")
-
-        return idx, row
-
-
-class BuildExecutor(BaseBuildExecutor):
-    def make_swds(self) -> DatasetSummary:
-        increased_rows = 0
-        with self.bin_writer as bw:
-            for append_seq_id, item_content in enumerate(
-                self.iter_item(), start=self._forked_last_seq_id + 1
-            ):
-                idx, row_data = self._unpack_row_content(item_content, append_seq_id)
-                bw.write_row(
-                    TabularDatasetRow(
-                        id=idx,
-                        data_origin=DataOriginType.NEW,
-                        data=row_data,
-                        _append_seq_id=append_seq_id,
-                    )
-                )
-                increased_rows += 1
-        self.flush()
-        self.tabular_dataset.info = self.get_info()  # type: ignore
-
-        summary = DatasetSummary(
-            rows=increased_rows,
-            increased_rows=increased_rows,
-            data_byte_size=self.bin_writer.total_bin_size,
+        with self._info_lock:
+            self._info_changed = True
+            self._info = TabularDatasetInfo(data)
+
+
+@unique
+class _RunEnvType(Enum):
+    POD = "pod"
+    THREAD = "thread"
+    PROCESS = "process"
+
+
+class TabularDatasetSessionConsumption(Protocol):
+    batch_size: int
+
+    def get_scan_range(
+        self, processed_keys: t.Optional[t.List[t.Tuple[t.Any, t.Any]]] = None
+    ) -> t.Optional[t.Tuple[t.Any, t.Any]]:
+        ...  # pragma: no cover
+
+
+local_standalone_tdsc: t.Dict[str, StandaloneTDSC] = {}
+lock_s_tdsc = threading.Lock()
+
+
+def get_dataset_consumption(
+    dataset_uri: t.Union[str, URI],
+    session_id: str,
+    batch_size: t.Optional[int] = None,
+    session_start: t.Optional[t.Any] = None,
+    session_end: t.Optional[t.Any] = None,
+    instance_uri: str = "",
+    instance_token: str = "",
+) -> TabularDatasetSessionConsumption:
+    # TODO: tune factory class arguments
+    _uri = instance_uri or os.environ.get(SWEnv.instance_uri)
+
+    if isinstance(dataset_uri, str):
+        dataset_uri = URI(dataset_uri, expected_type=URIType.DATASET)
+
+    batch_size = batch_size or int(
+        os.environ.get(
+            "DATASET_CONSUMPTION_BATCH_SIZE",
+            DEFAULT_CONSUMPTION_BATCH_SIZE,
         )
-        return self._merge_forked_summary(summary)
-
-
-def create_generic_cls(
-    handler: t.Callable,
-) -> t.Type[BaseBuildExecutor]:
-    res = handler()
-
-    if inspect.isgenerator(res):
-        items_iter = res
-    elif getattr(res, "__getitem__", None):
-        items_iter = iter(res)
+    )
+    if _uri is None or _uri == STANDALONE_INSTANCE:
+        global local_standalone_tdsc
+        key = f"{dataset_uri}-{session_id}-{session_start}-{session_end}-{batch_size}"
+        with lock_s_tdsc:
+            _obj = local_standalone_tdsc.get(key)
+            if not _obj:
+                _obj = StandaloneTDSC(
+                    dataset_uri=dataset_uri,
+                    session_id=session_id,
+                    batch_size=batch_size,
+                    session_start=session_start,
+                    session_end=session_end,
+                )
+                local_standalone_tdsc[key] = _obj
+            return _obj
     else:
-        raise RuntimeError(
-            f"{handler} function return is not generator or iterable object"
+        _token = (
+            instance_token
+            or SWCliConfigMixed().get_sw_token(instance=_uri)
+            or os.getenv(SWEnv.instance_token, "")
+        )
+        return CloudTDSC(
+            instance_uri=_uri,
+            dataset_uri=dataset_uri,
+            session_id=session_id,
+            batch_size=batch_size,
+            session_start=session_start,
+            session_end=session_end,
+            instance_token=_token,
         )
 
-    item = next(items_iter)
-
-    def _do_iter_item(self: t.Any) -> t.Generator:
-        yield item
-        for _item in items_iter:
-            yield _item
-
-    return create_generic_cls_by_mode(_do_iter_item)
-
-
-def create_generic_cls_by_mode(iter_func: t.Callable) -> t.Type[BaseBuildExecutor]:
-    return type(
-        "GenericSWDSBinHandler",
-        (BuildExecutor,),
-        {"iter_item": iter_func},
-    )
 
+class StandaloneTDSC(TabularDatasetSessionConsumption):
+    class _BatchTask:
+        def __init__(self, start: t.Any, end: t.Any) -> None:
+            self.start = start
+            self.end = end
 
-class RowWriter(threading.Thread):
     def __init__(
         self,
-        dataset_name: str,
-        dataset_version: str,
-        project_name: str = DEFAULT_PROJECT,
-        workdir: Path = Path(".dataset_tmp"),
-        alignment_bytes_size: int = D_ALIGNMENT_SIZE,
-        volume_bytes_size: int = D_FILE_VOLUME_SIZE,
-        append: bool = False,
-        append_from_version: str = "",
-        append_from_uri: t.Optional[URI] = None,
-        instance_name: str = STANDALONE_INSTANCE,
+        dataset_uri: URI,
+        session_id: str,
+        batch_size: int = DEFAULT_CONSUMPTION_BATCH_SIZE,
+        session_start: t.Optional[t.Any] = None,
+        session_end: t.Optional[t.Any] = None,
     ) -> None:
-        super().__init__(
-            name=f"RowWriter-{dataset_name}-{dataset_version}-{project_name}"
-        )
+        if dataset_uri.instance_type != InstanceType.STANDALONE:
+            raise NoSupportError(
+                f"StandaloneTDSC only supports standalone dataset: {dataset_uri}"
+            )
 
-        self._kw = {
-            "dataset_name": dataset_name,
-            "dataset_version": dataset_version,
-            "project_name": project_name,
-            "workdir": workdir,
-            "alignment_bytes_size": alignment_bytes_size,
-            "volume_bytes_size": volume_bytes_size,
-            "append": append,
-            "append_from_version": append_from_version,
-            "append_from_uri": append_from_uri,
-            "instance_name": instance_name,
-        }
+        self.project = dataset_uri.project
+        self.dataset_name = dataset_uri.object.name
+        self.dataset_version = dataset_uri.object.version
+
+        self.session_id = session_id
+        if batch_size <= 0:
+            raise FieldTypeOrValueError(f"batch_size is invalid: {batch_size}")
+        self.batch_size = batch_size
+        self.session_start = session_start
+        self.session_end = session_end
+        self.run_env = _RunEnvType.THREAD
 
-        self._queue: queue.Queue[t.Optional[DataRow]] = queue.Queue()
-        self._summary = DatasetSummary()
         self._lock = threading.Lock()
+        self._todo_queue = self._init_dataset_todo_queue()
+        self._doing_consumption: t.Dict[str, t.Dict[str, t.Any]] = defaultdict(dict)
 
-        self._run_exception: t.Optional[Exception] = None
-
-        self.daemon = True
-        self._builder: t.Optional[BaseBuildExecutor] = None
-        if append and append_from_version:
-            _cls = create_generic_cls_by_mode(self.__iter__)
-            self._builder = _cls(**self._kw)  # type: ignore
-            self.start()
-
-    def _raise_run_exception(self) -> None:
-        if self._run_exception is not None:
-            _e = self._run_exception
-            self._run_exception = None
-            raise threading.ThreadError(f"RowWriter Thread raise exception: {_e}")
-
-    @property
-    def summary(self) -> DatasetSummary:
-        return self._summary
+        # TODO: support sidecar thread monitor
+        # TODO: support max_retries
 
-    def __enter__(self) -> RowWriter:
-        return self
+    def _init_dataset_todo_queue(self) -> Queue:
+        # TODO: support datastore revision
+        wrapper = DatastoreWrapperDataset(
+            dataset_name=self.dataset_name,
+            project=self.project,
+        )
+        ids = [i["id"] for i in wrapper.scan_id(self.session_start, self.session_end)]
+        id_cnt = len(ids)
+        queue: Queue[StandaloneTDSC._BatchTask] = Queue(maxsize=id_cnt)
+        for start in range(0, id_cnt, self.batch_size):
+            end = start + self.batch_size
+            # TODO: add put block?
+            start_key = ids[start]
+            end_key = ids[end] if end < id_cnt else None
+            queue.put(StandaloneTDSC._BatchTask(start=start_key, end=end_key))
+        return queue
 
-    def __exit__(
+    def get_scan_range(
         self,
-        type: t.Optional[t.Type[BaseException]],
-        value: t.Optional[BaseException],
-        trace: TracebackType,
-    ) -> None:
-        if value:  # pragma: no cover
-            logger.warning(f"type:{type}, exception:{value}, traceback:{trace}")
+        processed_keys: t.Optional[t.List[t.Tuple[t.Any, t.Any]]] = None,
+    ) -> t.Optional[t.Tuple[t.Any, t.Any]]:
+        processed_keys = processed_keys or []
+        consumer_id = self.consumer_id
 
-        self.close()
+        with self._lock:
+            consumer: t.Dict = self._doing_consumption.get(consumer_id, {})
+            if consumer:
+                for k in processed_keys:
+                    if not k:
+                        continue
+                    consumer.pop(f"{k[0]}-{k[1]}", None)
+
+            if not self._todo_queue.empty():
+                task: StandaloneTDSC._BatchTask = self._todo_queue.get()
+                self._doing_consumption[consumer_id][f"{task.start}-{task.end}"] = task
+                logger.info(
+                    f"{consumer_id} handle scan-range: ({task.start}, {task.end})"
+                )
+                return task.start, task.end
 
-    def flush(self) -> None:
-        while not self._queue.empty():
-            # TODO: tune flush with thread condition
-            time.sleep(0.1)
+            for cid in list(self._doing_consumption.keys()):
+                if len(self._doing_consumption[cid]) == 0:
+                    self._doing_consumption.pop(cid, None)
 
-        if self._builder:
-            self._builder.flush()
+        return None
 
-    def close(self) -> None:
-        self._queue.put(None)
+    def __str__(self) -> str:
+        return f"[Standalone]Dataset Consumption: id-{self.session_id}, range-[{self.session_start},{self.session_end}], consumer:{self.consumer_id}@{self.run_env}"
 
-        self.join()
-        if self._builder:
-            self._builder.close()
+    def __repr__(self) -> str:
+        return f"[Standalone]Dataset Consumption: id-{self.session_id}, range-[{self.session_start},{self.session_end}], consumer:{self.consumer_id}@{self.run_env}, batch:{self.batch_size}"
 
-        self._raise_run_exception()
+    @property
+    def consumer_id(self) -> str:
+        if self.run_env == _RunEnvType.THREAD:
+            return f"thread-{id(threading.current_thread())}"
+        else:
+            return f"process-{os.getpid()}"  # pragma: no cover
 
-    def update(self, row_item: DataRow) -> None:
-        self._raise_run_exception()
-        self._queue.put(row_item)
 
-        with self._lock:
-            if self._builder is None:
-                _cls = create_generic_cls(self.__iter__)
-                self._builder = _cls(**self._kw)  # type: ignore
-                self.start()
-
-    def __iter__(self) -> t.Generator[DataRow, None, None]:
-        while True:
-            item = self._queue.get(block=True, timeout=None)
-            if item is None:
-                if self._queue.qsize() > 0:
-                    continue
-                else:
-                    break
+class CloudTDSC(TabularDatasetSessionConsumption):
+    def __init__(
+        self,
+        instance_uri: str,
+        dataset_uri: URI,
+        session_id: str,
+        batch_size: int = DEFAULT_CONSUMPTION_BATCH_SIZE,
+        session_start: t.Optional[t.Any] = None,
+        session_end: t.Optional[t.Any] = None,
+        instance_token: str = "",
+    ) -> None:
+        self.instance_uri = instance_uri
+        self.instance_token = instance_token
+        self.session_id = session_id
+        self.batch_size = batch_size
+        self.session_start = session_start
+        self.session_end = session_end
+        self.dataset_uri = dataset_uri
+        self.run_env = _RunEnvType.POD
+        self.consumer_id = os.environ.get(ENV_POD_NAME)
+
+        self._do_validate()
+
+    def _do_validate(self) -> None:
+        if not self.instance_token:
+            raise FieldTypeOrValueError("instance token is empty")
+
+        if (
+            not self.dataset_uri.project
+            or not self.dataset_uri.object.name
+            or not self.dataset_uri.object.version
+        ):
+            raise FormatError(f"wrong dataset uri format: {self.dataset_uri}")
+
+        if not self.consumer_id:
+            raise RuntimeError("failed to get pod name")
+
+    @http_retry
+    def get_scan_range(
+        self, processed_keys: t.Optional[t.List[t.Tuple[t.Any, t.Any]]] = None
+    ) -> t.Optional[t.Tuple[t.Any, t.Any]]:
+        post_data = {
+            "batchSize": self.batch_size,
+            "sessionId": self.session_id,
+            "consumerId": self.consumer_id,
+        }
+        if processed_keys is not None:
+            post_data["processedData"] = [
+                {"start": p[0], "end": p[1]} for p in processed_keys
+            ]
+
+        if self.session_start is not None:
+            post_data["start"] = self.session_start
+
+        if self.session_end is not None:
+            post_data["end"] = self.session_end
+
+        resp = requests.post(
+            urllib.parse.urljoin(
+                self.instance_uri,
+                f"api/v1/project/{self.dataset_uri.project}/dataset/{self.dataset_uri.object.name}/version/{self.dataset_uri.object.version}/consume",
+            ),
+            data=json.dumps(post_data),
+            headers={
+                "Content-Type": "application/json; charset=utf-8",
+                "Authorization": self.instance_token,  # type: ignore
+            },
+            timeout=300,
+        )
+        resp.raise_for_status()
+        range_data = resp.json()["data"]
 
-            if not isinstance(item, DataRow):
-                continue
+        return None if range_data is None else (range_data["start"], range_data["end"])
 
-            yield item
+    def __str__(self) -> str:
+        return (
+            f"[Cloud:{self.instance_uri}]Dataset Consumption: id-{self.session_id}, "
+            f"range-[{self.session_start},{self.session_end}], consumer:{self.consumer_id}@{self.run_env}"
+        )
 
-    def run(self) -> None:
-        try:
-            if self._builder is None:
-                raise RuntimeError("dataset builder object wasn't initialized")
-            self._summary = self._builder.make_swds()
-        except Exception as e:
-            logger.exception(e)
-            self._run_exception = e
-            raise
+    def __repr__(self) -> str:
+        return (
+            f"[Cloud:{self.instance_uri}]Dataset Consumption: id-{self.session_id}, "
+            f"range-[{self.session_start},{self.session_end}], consumer:{self.consumer_id}@{self.run_env}, "
+            f"batch-{self.batch_size}, dataset-{self.dataset_uri}"
+        )
```

### Comparing `starwhale-0.4.1/starwhale/api/_impl/dataset/model.py` & `starwhale-0.4.2/starwhale/api/_impl/dataset/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,82 @@
 from __future__ import annotations
 
+import os
+import json
 import typing as t
+import platform
+import tempfile
 import threading
 from http import HTTPStatus
 from types import TracebackType
 from pathlib import Path
-from functools import wraps
+from functools import wraps, partial, lru_cache
 from itertools import islice
-from contextlib import ExitStack
 
+import yaml
 from loguru import logger
 
-from starwhale.utils import gen_uniq_version
+from starwhale.utils import now_str, convert_to_bytes, gen_uniq_version
 from starwhale.consts import (
+    FileDesc,
     HTTPMethod,
+    CREATED_AT_KEY,
+    SW_TMP_DIR_NAME,
     DEFAULT_PAGE_IDX,
     DEFAULT_PAGE_SIZE,
     STANDALONE_INSTANCE,
+    DEFAULT_MANIFEST_NAME,
 )
+from starwhale.version import STARWHALE_VERSION
 from starwhale.base.uri import URI, URIType
-from starwhale.utils.fs import move_dir, empty_dir
+from starwhale.utils.fs import copy_file, empty_dir, ensure_dir, ensure_file
 from starwhale.base.type import InstanceType
 from starwhale.base.cloud import CloudRequestMixed
-from starwhale.utils.error import ExistedError, NotFoundError, NoSupportError
-from starwhale.core.dataset.type import DatasetConfig, DatasetSummary
+from starwhale.utils.error import NoSupportError
+from starwhale.utils.config import SWCliConfigMixed
+from starwhale.core.dataset.type import (
+    DatasetSummary,
+    D_ALIGNMENT_SIZE,
+    D_FILE_VOLUME_SIZE,
+)
 from starwhale.core.dataset.model import Dataset as CoreDataset
 from starwhale.core.dataset.model import StandaloneDataset
 from starwhale.core.dataset.store import DatasetStorage
 from starwhale.api._impl.data_store import TableEmptyException
 from starwhale.core.dataset.tabular import (
     TabularDataset,
+    DatastoreRevision,
     TabularDatasetInfo,
     DatastoreWrapperDataset,
     get_dataset_consumption,
     DEFAULT_CONSUMPTION_BATCH_SIZE,
     TabularDatasetSessionConsumption,
 )
 
 from .loader import DataRow, DataLoader, get_data_loader
-from .builder import RowWriter, BaseBuildExecutor
+from .builder import MappingDatasetBuilder
 
 if t.TYPE_CHECKING:
     import tensorflow as tf
     from torch.utils.data import Dataset as TorchDataset
 
 _DType = t.TypeVar("_DType", bound="Dataset")
 _ItemType = t.Union[str, int, slice]
-_HandlerType = t.Optional[t.Union[t.Callable, BaseBuildExecutor]]
 _GItemType = t.Optional[t.Union[DataRow, t.List[DataRow]]]
 
 _DEFAULT_LOADER_WORKERS = 2
 _DEFAULT_LOADER_CACHE_SIZE = 20
 
 
+class _DatasetCreateMode:
+    auto = "auto"
+    empty = "empty"
+    forbid = "forbid"
+
+
 class _Tags:
     def __init__(self, core_dataset: CoreDataset) -> None:
         self.__core_dataset = core_dataset
 
     def add(self, tags: t.Union[str, t.List[str]], ignore_errors: bool = False) -> None:
         if isinstance(tags, str):
             tags = [tags]
@@ -81,146 +101,140 @@
 
 class Dataset:
     def __init__(
         self,
         name: str,
         version: str,
         project_uri: URI,
-        create: bool = False,
+        readonly: bool = False,
+        create: str = _DatasetCreateMode.auto,
     ) -> None:
         self.name = name
         self.project_uri = project_uri
+        self.__readonly = readonly
+        self._pending_commit_version = gen_uniq_version()
 
-        _origin_uri = URI.capsulate_uri(
-            self.project_uri.instance,
-            self.project_uri.project,
-            URIType.DATASET,
-            self.name,
-            version,
-        )
-
-        if create:
-            self.version = gen_uniq_version()
-        else:
-            self.version = self._auto_complete_version(version)
-
-        if not self.version:
-            raise ValueError("version field is empty")
-
-        self.uri = URI.capsulate_uri(
-            self.project_uri.instance,
-            self.project_uri.project,
-            URIType.DATASET,
-            self.name,
-            self.version,
+        self._make_capsulated_uri = partial(
+            URI.capsulate_uri,
+            instance=self.project_uri.instance,
+            project=self.project_uri.project,
+            obj_type=URIType.DATASET,
+            obj_name=self.name,
         )
 
-        self.__readonly = not create
-        self.__core_dataset = CoreDataset.get_dataset(self.uri)
-        if create:
-            setattr(self.__core_dataset, "_version", self.version)
+        if create not in (
+            _DatasetCreateMode.auto,
+            _DatasetCreateMode.empty,
+            _DatasetCreateMode.forbid,
+        ):
+            raise ValueError(
+                f"the current create mode is not in the accept options: {create}"
+            )
 
-        _summary = None
+        _origin_uri = self._make_capsulated_uri(obj_ver=version or "latest")
         origin_uri_exists = self._check_uri_exists(_origin_uri)
         if origin_uri_exists:
-            if create:
-                # TODO: support build cloud dataset from the existed dataset
-                if self.project_uri.instance_type == InstanceType.CLOUD:
-                    raise NoSupportError(
-                        f"Can't build dataset from the existed cloud dataset uri:{_origin_uri}"
-                    )
+            if create == _DatasetCreateMode.empty:
+                raise RuntimeError(
+                    f"dataset already existed, failed to create by the {create} create mode: {self.name}"
+                )
 
-                self._append_from_version = version
-                self._create_by_append = True
-                self._fork_dataset()
-                _summary = CoreDataset.get_dataset(_origin_uri).summary()
-            else:
-                self._append_from_version = ""
-                self._create_by_append = False
+            self._loading_version = self._auto_complete_version(
+                _origin_uri.object.version
+            )
         else:
-            if create:
-                self._append_from_version = ""
-                self._create_by_append = False
-            else:
-                raise ExistedError(f"{self.uri} was not found fo load")
+            # TODO: call server or standalone api to create an empty dataset before committing.
+            if create == _DatasetCreateMode.forbid:
+                raise RuntimeError(
+                    "dataset doest not exist, we have already use {create} create mode to ensure dataset existence: {self.name}"
+                )
 
-        self._summary: t.Optional[DatasetSummary]
-        if _summary:
-            self._summary = _summary
-        else:
-            if origin_uri_exists:
-                self._summary = self.__core_dataset.summary()
-            else:
-                self._summary = DatasetSummary()
+            if readonly:
+                raise ValueError(
+                    f"no support to set a non-existed dataset to the readonly mode: {self.name}"
+                )
+
+            if version != "":
+                raise NoSupportError(
+                    f"no support to create a specified version dataset: {version}"
+                )
+
+            self._loading_version = self._pending_commit_version
+
+        self._loading_uri = self._make_capsulated_uri(obj_ver=self._loading_version)
+        self.__loading_core_dataset = CoreDataset.get_dataset(self._loading_uri)
+
+        self._pending_commit_uri = self._make_capsulated_uri(
+            obj_ver=self._pending_commit_version
+        )
+        self.__pending_commit_core_dataset = CoreDataset.get_dataset(
+            self._pending_commit_uri
+        )
 
-        self._rows_cnt = self._summary.rows if self._summary else 0
         self._consumption: t.Optional[TabularDatasetSessionConsumption] = None
-        self._lock = threading.Lock()
+        self._loader_lock = threading.Lock()
         self.__data_loaders: t.Dict[str, DataLoader] = {}
-        self.__build_handler: _HandlerType = None
-        self._trigger_handler_build = False
-        self._trigger_icode_build = False
-        self._writer_lock = threading.Lock()
-        self._row_writer: t.Optional[RowWriter] = None
-        self._enable_copy_src = False
+        self._loader_cache_size = _DEFAULT_LOADER_CACHE_SIZE
+        self._loader_num_workers = _DEFAULT_LOADER_WORKERS
+
+        self._builder_blob_alignment_size = D_ALIGNMENT_SIZE
+        self._builder_blob_volume_size = D_FILE_VOLUME_SIZE
+        self._builder_lock = threading.Lock()
+        self._dataset_builder: t.Optional[MappingDatasetBuilder] = None
+        self._commit_lock = threading.Lock()
+        self.__has_committed = False
+
         self._info_lock = threading.Lock()
         self._info_ds_wrapper: t.Optional[DatastoreWrapperDataset] = None
         self.__info: t.Optional[TabularDatasetInfo] = None
 
-        self._loader_cache_size = _DEFAULT_LOADER_CACHE_SIZE
-        self._loader_num_workers = _DEFAULT_LOADER_WORKERS
-
-    def _fork_dataset(self) -> None:
-        # TODO: support cloud dataset prepare in the tmp dir
-        # TODO: lazy fork dataset
-        if not isinstance(self.__core_dataset, StandaloneDataset):
-            raise NoSupportError(
-                f"only support standalone dataset fork: {self.__core_dataset}"
-            )
+        self._tmpdir: t.Optional[Path] = None
 
-        def _when_exit() -> None:
-            self.__core_dataset.store.building = False
+        self._updated_rows_by_commit = 0
+        self._deleted_rows_by_commit = 0
+        if origin_uri_exists:
+            _summary = self.__loading_core_dataset.summary()
+            # TODO: raise none summary exception for existed dataset
+            if _summary is None:
+                self._total_rows = 0
+                self._total_blobs_size = 0
+            else:
+                self._total_rows = _summary.rows
+                self._total_blobs_size = _summary.blobs_byte_size
+        else:
+            self._total_rows = 0
+            self._total_blobs_size = 0
 
-        with ExitStack() as stack:
-            stack.callback(_when_exit)
-            self.__core_dataset.store.building = True
-            self.__core_dataset._prepare_snapshot()
-            self.__core_dataset._fork_swds(
-                self._create_by_append, self._append_from_version
-            )
+        self._last_data_datastore_revision = ""
+        self._last_info_datastore_revision = ""
 
     def _auto_complete_version(self, version: str) -> str:
         version = version.strip()
         if not version:
             return version
 
+        # TODO: auto complete for cloud instance
         if self.project_uri.instance_type == InstanceType.CLOUD:
             return version
 
-        _uri = URI.capsulate_uri(
-            instance=self.project_uri.instance,
-            project=self.project_uri.project,
-            obj_type=URIType.DATASET,
-            obj_name=self.name,
-            obj_ver=version,
-        )
+        _uri = self._make_capsulated_uri(obj_ver=version)
         store = DatasetStorage(_uri)
         if not store.snapshot_workdir.exists():
             return version
         else:
             return store.id
 
     def __str__(self) -> str:
-        return f"Dataset: {self.name}-{self.version}"
+        return f"Dataset: {self.name}, stash version: {self._pending_commit_version}, loading version: {self._loading_version}"
 
     def __repr__(self) -> str:
-        return f"Dataset: uri-{self.uri}"
+        return f"Dataset: {self.name}, loading uri: {self._loading_uri}, pending commit uri: {self._pending_commit_uri}"
 
     def __len__(self) -> int:
-        return self._rows_cnt
+        return self._total_rows
 
     def __enter__(self: _DType) -> _DType:
         return self
 
     def __bool__(self) -> bool:
         return True
 
@@ -239,77 +253,145 @@
         self, session_id: str, batch_size: int = DEFAULT_CONSUMPTION_BATCH_SIZE
     ) -> Dataset:
         if self._consumption is not None:
             raise RuntimeError(
                 f"distributed consumption has already been created ({self._consumption})"
             )
 
-        with self._lock:
+        with self._loader_lock:
             self._consumption = get_dataset_consumption(
                 self.uri, session_id=session_id, batch_size=batch_size
             )
         return self
 
     def _clear_data_loader(self) -> None:
-        with self._lock:
+        with self._loader_lock:
             self.__data_loaders = {}
 
     def with_loader_config(
         self, num_workers: t.Optional[int] = None, cache_size: t.Optional[int] = None
     ) -> Dataset:
-        if len(self.__data_loaders) != 0:
-            raise RuntimeError(
-                f"loaders({list(self.__data_loaders)}) have already been initialized"
-            )
+        with self._loader_lock:
+            if len(self.__data_loaders) != 0:
+                raise RuntimeError(
+                    f"loaders({list(self.__data_loaders)}) have already been initialized"
+                )
 
-        with self._lock:
             if num_workers is not None:
                 self._loader_num_workers = num_workers
 
             if cache_size is not None:
                 self._loader_cache_size = cache_size
 
         return self
 
+    def with_builder_blob_config(
+        self,
+        volume_size: int | str = D_FILE_VOLUME_SIZE,
+        alignment_size: int | str = D_ALIGNMENT_SIZE,
+    ) -> Dataset:
+        """Config blob attributes for the dataset builder.
+
+        If you want to config blob attributes, you should call the function before appending, updating or deleting dataset records.
+
+        Arguments:
+            volume_size: (str, int, optional) The max bytes size of the single blob file.
+                When blob file size exceeds the value of volume_size argument, a new blob file is created automatically.
+                The default is 64MB. The argument accepts int(bytes) or str(32K, 64MB, 1GB...) format.
+            alignment_size: (str, int, optional) The alignment size of every bin section in the blob file.
+                The remaining part will be filled with `\0`. Default is 64 bytes.
+
+        Examples:
+        ```python
+        from starwhale import dataset, Binary
+
+        ds = dataset("mnist").with_builder_blob_config(volume_size="32M", alignment_size=128)
+        ds.append({"data": Binary(b"123")})
+        ds.commit()
+        ds.close()
+        ```
+
+        Returns:
+            A Dataset Object
+        """
+        with self._builder_lock:
+            if self._dataset_builder is not None:
+                raise RuntimeError(
+                    "dataset has already accept some changed rows, forbid to config dataset blob attributes"
+                )
+
+            self._builder_blob_volume_size = convert_to_bytes(volume_size)
+            self._builder_blob_alignment_size = convert_to_bytes(alignment_size)
+
+        return self
+
     def _get_data_loader(
         self, recreate: bool = False, disable_consumption: bool = False
     ) -> DataLoader:
-        with self._lock:
-            key = f"consumption-{disable_consumption}"
-
+        with self._loader_lock:
+            key = f"consumption-{disable_consumption}-{self.uri.object.version}"
             _loader = self.__data_loaders.get(key)
             if _loader is None or recreate:
                 if disable_consumption:
                     consumption = None
                 else:
                     consumption = self._consumption
 
+                data_revision = self._last_data_datastore_revision
+                if data_revision == "":
+                    data_revision = self._get_datastore_revision(self.uri).data
+
                 _loader = get_data_loader(
                     self.uri,
                     session_consumption=consumption,
                     cache_size=self._loader_cache_size,
                     num_workers=self._loader_num_workers,
+                    dataset_scan_revision=data_revision,
                 )
                 self.__data_loaders[key] = _loader
 
         return _loader
 
+    @lru_cache(maxsize=32)
+    def _get_datastore_revision(self, uri: URI) -> DatastoreRevision:
+        if uri.object.typ != URIType.DATASET:
+            raise NoSupportError(
+                f"only support to fetch dataset datastore revision: {uri}"
+            )
+
+        if uri.object.version == "":
+            raise RuntimeError(f"cannot get version of uri: {uri}")
+
+        if uri.instance_type == InstanceType.CLOUD:
+            crm = CloudRequestMixed()
+            r = crm.do_http_request(
+                path=f"/project/{uri.project}/dataset/{uri.object.name}",
+                instance_uri=uri,
+                params={"versionUrl": uri.object.version},
+            ).json()
+            manifest = yaml.safe_load(r["data"]["versionMeta"])
+        else:
+            manifest = DatasetStorage(uri).manifest
+
+        return DatastoreRevision.from_manifest(manifest)
+
     def batch_iter(
         self, batch_size: int = 1, drop_not_full: bool = False
     ) -> t.Iterator[t.List[DataRow]]:
         """Batch data into lists of length n. The last batch may be shorter."""
         it = self.__iter__()
         while True:
             batch_data = list(islice(it, batch_size))
             if not batch_data or (drop_not_full and len(batch_data) < batch_size):
                 return
             yield batch_data
 
     def __iter__(self) -> t.Iterator[DataRow]:
         for row in self._get_data_loader():
+            row._patch_shadow_dataset(self)
             yield row
 
     def __getitem__(
         self,
         item: _ItemType,
     ) -> _GItemType:
         """
@@ -327,27 +409,33 @@
         item: _ItemType,
         skip_fetch_data: bool = False,
     ) -> _GItemType:
         def _run() -> _GItemType:
             loader = self._get_data_loader(disable_consumption=True)
             if isinstance(item, (int, str)):
                 row = next(loader.tabular_dataset.scan(item, item, end_inclusive=True))
-                return loader._unpack_row(row, skip_fetch_data)
+                return loader._unpack_row(row, skip_fetch_data, shadow_dataset=self)
             elif isinstance(item, slice):
                 step = item.step or 1
                 if step <= 0:
                     raise ValueError(
                         f"Dataset slice step({step}) cannot be zero or negative number"
                     )
                 cnt = 0
                 # TODO: batch signed urls
                 rows = []
                 for row in loader.tabular_dataset.scan(item.start, item.stop):
                     if cnt % step == 0:
-                        rows.append(loader._unpack_row(row, skip_fetch_data))
+                        rows.append(
+                            loader._unpack_row(
+                                row,
+                                skip_fetch_data,
+                                shadow_dataset=self,
+                            )
+                        )
                     cnt += 1
                 return rows
             else:
                 raise ValueError(f"{item} type is not int, str or slice")
 
         try:
             return _run()
@@ -367,54 +455,17 @@
             self: Dataset = args[0]
             if self.readonly:
                 raise RuntimeError(f"{func} does not work in the readonly mode")
             return func(*args, **kwargs)
 
         return _wrapper
 
-    def _forbid_handler_build(func: t.Callable):  # type: ignore
-        @wraps(func)
-        def _wrapper(*args: t.Any, **kwargs: t.Any) -> t.Any:
-            self: Dataset = args[0]
-            if self._trigger_handler_build:
-                raise NoSupportError(
-                    "no support build from handler and from cache code at the same time, build from handler has already been activated"
-                )
-            return func(*args, **kwargs)
-
-        return _wrapper
-
-    def _forbid_icode_build(func: t.Callable):  # type: ignore
-        @wraps(func)
-        def _wrapper(*args: t.Any, **kwargs: t.Any) -> t.Any:
-            self: Dataset = args[0]
-            if self._trigger_icode_build:
-                raise NoSupportError(
-                    "no support build from handler and from cache code at the same time, build from interactive code has already been activated"
-                )
-            return func(*args, **kwargs)
-
-        return _wrapper
-
-    @property
-    def build_handler(self) -> _HandlerType:
-        return self.__build_handler
-
-    @build_handler.setter
-    def build_handler(self, handler: _HandlerType) -> None:
-        if self._trigger_icode_build:
-            raise RuntimeError(
-                "dataset append by interactive code has already been called"
-            )
-        self._trigger_handler_build = True
-        self.__build_handler = handler
-
     @property
     def tags(self) -> _Tags:
-        return _Tags(self.__core_dataset)
+        return _Tags(self.__loading_core_dataset)
 
     @staticmethod
     def _check_uri_exists(uri: t.Optional[URI]) -> bool:
         if uri is None or uri.object.version == "":
             return False
 
         if uri.instance_type == InstanceType.CLOUD:
@@ -431,78 +482,102 @@
             return _store.manifest_path.exists()
 
     def exists(self) -> bool:
         return self._check_uri_exists(self.uri)
 
     @property
     def info(self) -> TabularDatasetInfo:
-        if self.__info is not None:
-            return self.__info
-
         with self._info_lock:
-            self._info_ds_wrapper = TabularDataset.from_uri(self.uri)._info_ds_wrapper
-            self.__info = TabularDatasetInfo.load_from_datastore(self._info_ds_wrapper)
+            if self.__info is None:
+                info_revision = self._last_info_datastore_revision
+                if info_revision == "":
+                    info_revision = self._get_datastore_revision(self.uri).info
+
+                self._info_ds_wrapper = TabularDataset.from_uri(
+                    self.uri, info_datastore_revision=info_revision
+                )._info_ds_wrapper
+                self.__info = TabularDatasetInfo.load_from_datastore(
+                    self._info_ds_wrapper
+                )
 
-        return self.__info
+            return self.__info
 
     @_check_readonly
-    def flush(self) -> None:
-        loader = self._get_data_loader(disable_consumption=True)
-        loader.tabular_dataset.flush()
+    def flush(self, artifacts_flush: bool = False) -> str:
+        revision = ""
+        if self._dataset_builder:
+            revision = self._dataset_builder.flush(artifacts_flush)
+            self._last_data_datastore_revision = revision
+            self._clear_data_loader()
 
-        if self._row_writer:
-            self._row_writer.flush()
+        return revision
 
     @_check_readonly
     def rehash(self) -> None:
         # TODO: rehash for swds-bin format dataset with append/delete items to reduce volumes size
         raise NotImplementedError
 
     def remove(self, force: bool = False) -> None:
-        ok, reason = self.__core_dataset.remove(force)
+        ok, reason = self.__loading_core_dataset.remove(force)
         if not ok:
             raise RuntimeError(f"failed to remove dataset: {reason}")
 
     def recover(self, force: bool = False) -> None:
-        ok, reason = self.__core_dataset.recover(force)
+        ok, reason = self.__loading_core_dataset.recover(force)
         if not ok:
             raise RuntimeError(f"failed to recover dataset: {reason}")
 
     def summary(self) -> t.Optional[DatasetSummary]:
-        return self._summary
+        return self.__loading_core_dataset.summary()
 
     def history(self) -> t.List[t.Dict]:
-        return self.__core_dataset.history()
+        return self.__loading_core_dataset.history()
 
     def close(self) -> None:
         for _loader in self.__data_loaders.values():
             if not _loader:
                 continue  # pragma: no cover
-
             _loader.tabular_dataset.close()
 
-        if self._row_writer:
-            self._row_writer.close()
+        if self._dataset_builder:
+            self._dataset_builder.close()
 
-        # TODO: flush raw data into disk
+        if self._tmpdir is not None:
+            empty_dir(self._tmpdir)
+
+    @property
+    def tmpdir(self) -> Path:
+        if self._tmpdir is None:
+            _base_dir = SWCliConfigMixed().rootdir / SW_TMP_DIR_NAME
+            ensure_dir(_base_dir)
+            self._tmpdir = Path(
+                tempfile.mkdtemp(prefix=f"dataset-{self.name}-", dir=_base_dir)
+            )
+        return self._tmpdir
 
     def diff(self, cmp: Dataset) -> t.Dict:
-        return self.__core_dataset.diff(cmp.uri)
+        # TODO: wait for datastore diff feature
+        raise NotImplementedError
 
     def manifest(self) -> t.Dict[str, t.Any]:
-        return self.__core_dataset.info()
+        return self.__loading_core_dataset.info()
 
-    def head(self, n: int = 3, show_raw_data: bool = False) -> t.List[t.Dict]:
+    def head(self, n: int = 5, skip_fetch_data: bool = False) -> t.List[DataRow]:
         # TODO: render artifact in JupyterNotebook
-        return self.__core_dataset.head(n, show_raw_data)
+        ret = []
+        loader = self._get_data_loader(disable_consumption=True)
+        for idx, td_row in enumerate(loader._iter_meta()):
+            if idx >= n:
+                break
+            data_row = loader._unpack_row(td_row, skip_fetch_data=skip_fetch_data)
+            ret.append(data_row)
+        return ret
 
     def fetch_one(self, skip_fetch_data: bool = False) -> DataRow:
-        loader = self._get_data_loader(disable_consumption=True)
-        row = next(loader.tabular_dataset.scan())
-        return loader._unpack_row(row, skip_fetch_data)
+        return self.head(1, skip_fetch_data)[0]
 
     def to_pytorch(
         self,
         transform: t.Optional[t.Callable] = None,
         drop_index: bool = True,
         skip_default_transform: bool = False,
     ) -> TorchDataset:
@@ -520,297 +595,452 @@
         drop_index: bool = True,
     ) -> tf.data.Dataset:
         from starwhale.integrations.tensorflow import to_tf_dataset
 
         return to_tf_dataset(dataset=self, drop_index=drop_index)
 
     @_check_readonly
-    @_forbid_handler_build
     def __setitem__(
         self, key: t.Union[str, int], value: t.Union[DataRow, t.Tuple, t.Dict]
     ) -> None:
         # TODO: tune the performance of getitem by cache
-        self._trigger_icode_build = True
-        _row_writer = self._get_row_writer()
-
         if not isinstance(key, (int, str)):
             raise TypeError(f"key must be str or int type: {key}")
 
         if isinstance(value, DataRow):
             value.index = key
             row = value
         elif isinstance(value, dict):
-            row = DataRow(index=key, data=value)
+            row = DataRow(index=key, features=value)
         elif isinstance(value, (tuple, list)):
             if len(value) == 1:
-                data = value[0]
+                features = value[0]
             elif len(value) == 2:
-                _, data = value
+                _, features = value
             else:
                 raise ValueError(f"{value} cannot unpack")
 
-            row = DataRow(index=key, data=data)
+            row = DataRow(index=key, features=features)
         else:
             raise TypeError(f"value only supports tuple, dict or DataRow type: {value}")
 
-        # TODO improve accuracy of _rows_cnt during building
-        self._rows_cnt += 1
-        _row_writer.update(row)
-
-    def _get_row_writer(self) -> RowWriter:
-        if self._row_writer is not None:
-            return self._row_writer
-
-        with self._writer_lock:
-            if self._row_writer is None:
-                if self._create_by_append and self._append_from_version:
-                    append_from_uri = URI.capsulate_uri(
-                        instance=self.project_uri.instance,
-                        project=self.project_uri.project,
-                        obj_type=URIType.DATASET,
-                        obj_name=self.name,
-                        obj_ver=self._append_from_version,
-                    )
-                    store = DatasetStorage(append_from_uri)
-                    if not store.snapshot_workdir.exists():
-                        raise NotFoundError(f"dataset uri: {append_from_uri}")
-                    append_from_version = store.id
-                else:
-                    append_from_uri = None
-                    append_from_version = ""
-
+        # TODO: add gc/rehash for update swds-bin format artifact features
+        # TODO improve accuracy of _total_rows during building
+        self._total_rows += 1
+
+        _ds_builder = self._get_dataset_builder()
+        _ds_builder.put(row)
+        self._updated_rows_by_commit += 1
+
+    def _get_dataset_builder(self) -> MappingDatasetBuilder:
+        with self._builder_lock:
+            if self._dataset_builder is None:
                 # TODO: support alignment_bytes_size, volume_bytes_size arguments
-                self._row_writer = RowWriter(
+                self._dataset_builder = MappingDatasetBuilder(
+                    workdir=self.tmpdir / "builder",
                     dataset_name=self.name,
-                    dataset_version=self.version,
                     project_name=self.project_uri.project,
-                    workdir=self.__core_dataset.store.tmp_dir,
-                    append=self._create_by_append,
-                    append_from_version=append_from_version,
-                    append_from_uri=append_from_uri,
                     instance_name=self.project_uri.instance,
+                    blob_alignment_bytes_size=self._builder_blob_alignment_size,
+                    blob_volume_bytes_size=self._builder_blob_volume_size,
                 )
-        return self._row_writer
-
-    _init_row_writer = _get_row_writer
+            return self._dataset_builder
 
     @_check_readonly
-    @_forbid_handler_build
     def __delitem__(self, key: _ItemType) -> None:
-        self._trigger_icode_build = True
-        self._init_row_writer()  # hack for del item as the first operation
-
         items: t.List
         if isinstance(key, (str, int)):
             items = [self._getitem(key, skip_fetch_data=True)]
         elif isinstance(key, slice):
             items = self._getitem(key, skip_fetch_data=True)  # type: ignore
         else:
             raise TypeError(f"key({key}) is not str, int or slice type")
 
         # TODO: raise not-found key error?
-        loader = self._get_data_loader(disable_consumption=True)
+        _ds_builder = self._get_dataset_builder()
         for item in items:
             if not item or not isinstance(item, DataRow):
                 continue  # pragma: no cover
-            loader.tabular_dataset.delete(item.index)
-            self._rows_cnt -= 1
+            _ds_builder.delete(item.index)
+            self._deleted_rows_by_commit += 1
+            self._total_rows -= 1
 
     @_check_readonly
-    @_forbid_handler_build
     def append(self, item: t.Any) -> None:
         if isinstance(item, DataRow):
             self.__setitem__(item.index, item)
         elif isinstance(item, dict):
-            self.__setitem__(self._rows_cnt, item)
+            self.__setitem__(self._total_rows, item)
         elif isinstance(item, (list, tuple)):
             if len(item) == 1:
-                row = DataRow(self._rows_cnt, item[0])
+                row = DataRow(self._total_rows, item[0])
             elif len(item) == 2:
                 row = DataRow(item[0], item[1])
             else:
                 raise ValueError(
                     f"cannot unpack value({item}), expected sequence is (index, data) or data"
                 )
 
             self.__setitem__(row.index, row)
         else:
             raise TypeError(f"value({item}) is not DataRow, list or tuple type")
 
     @_check_readonly
-    @_forbid_handler_build
     def extend(self, items: t.Sequence[t.Any]) -> None:
         for item in items:
             self.append(item)
 
-    @_check_readonly
-    def build_with_copy_src(
-        self,
-        src_dir: t.Union[str, Path],
-        include_files: t.Optional[t.List[str]] = None,
-        exclude_files: t.Optional[t.List[str]] = None,
-    ) -> Dataset:
-        self._enable_copy_src = True
-        self._build_src_dir = Path(src_dir)
-        self._build_include_files = include_files or []
-        self._build_exclude_files = exclude_files or []
-        return self
+    @property
+    def loading_version(self) -> str:
+        """Loaded dataset version.
+        When loading an existing dataset, the loading_version is the related dataset version.
+        When creating a non-existed dataset, the loading_version is equal to the pending_commit_version.
 
-    commit_with_copy_src = build_with_copy_src
+        Returns:
+            A str version
+        """
+        return self._loading_version
 
-    @_check_readonly
-    @_forbid_handler_build
-    def _do_build_from_interactive_code(self) -> None:
-        if self._row_writer is None:
-            raise RuntimeError("row writer is none, no data was written")
-
-        if self.__info is not None and self._info_ds_wrapper is not None:
-            self.__info.save_to_datastore(self._info_ds_wrapper)
-
-        self.flush()
-        self._row_writer.close()
-        self._summary = self._row_writer.summary
-
-        # TODO: add len api for tabular_dataset to reduce overhead here
-        if self._row_writer._builder:
-            table_rows = [
-                row for row in self._row_writer._builder.tabular_dataset.scan()
-            ]
-            self._summary.rows = len(table_rows)
-
-        if isinstance(self.__core_dataset, StandaloneDataset):
-            local_ds = self.__core_dataset
-            local_uri = self.uri
-        else:
-            local_uri = URI.capsulate_uri(
-                instance=STANDALONE_INSTANCE,
-                project=self.uri.project,
-                obj_type=self.uri.object.typ,
-                obj_name=self.uri.object.name,
-                obj_ver=self.uri.object.version,
-            )
-            local_ds = StandaloneDataset(local_uri)
-            local_ds.store._tmp_dir = self.__core_dataset.store.tmp_dir
-            setattr(local_ds, "_version", self.version)
-
-        def _when_standalone_exit() -> None:
-            local_ds._make_auto_tags()
-            move_dir(local_ds.store.tmp_dir, local_ds.store.snapshot_workdir)
-
-        def _when_cloud_exit() -> None:
-            from starwhale.core.dataset.copy import DatasetCopy
-
-            dc = DatasetCopy(
-                str(local_uri), str(self.uri), URIType.DATASET
-            ).with_disable_datastore()
-            dc._do_upload_bundle_dir(workdir=local_ds.store.tmp_dir)
-            empty_dir(local_ds.store.tmp_dir)
-
-        def _when_exit() -> None:
-            local_ds.store.building = False
-            if isinstance(self.__core_dataset, StandaloneDataset):
-                _when_standalone_exit()
-            else:
-                _when_cloud_exit()
+    @property
+    def pending_commit_version(self) -> str:
+        """Next commit version.
+        When you call the `commit` function, the pending_commit_version will be recorded in
+        the Standalone instance ,or Cloud instance.
 
-        with ExitStack() as stack:
-            stack.callback(_when_exit)
-            local_ds.store.building = True
-            local_ds._manifest["dataset_summary"] = self._summary.asdict()
-            local_ds._calculate_signature()
-            local_ds._render_manifest()
-            local_ds._make_swds_meta_tar()
+        Returns:
+            A str version
+        """
+        return self._pending_commit_version
 
-    @_check_readonly
-    @_forbid_icode_build
-    def _do_build_from_handler(self) -> None:
-        # TODO: support build dataset for cloud uri directly
-        if self.project_uri.instance_type == InstanceType.CLOUD:
-            raise NoSupportError("no support to build cloud dataset directly")
+    @property
+    def committed_version(self) -> str:
+        """Committed version.
 
-        if self.__info is not None and self._info_ds_wrapper is not None:
-            self.__info.save_to_datastore(self._info_ds_wrapper)
+        After the commit function is called, the committed_version will come out, it is equal to the pending_commit_version.
 
-        self._trigger_icode_build = True
-        config = DatasetConfig(
-            name=self.name,
-            handler=self.build_handler,
-            project_uri=self.project_uri.full_uri,
-            append=self._create_by_append,
-            append_from=self._append_from_version,
-        )
+        Returns:
+            A str version
+        """
+        if self.__has_committed:
+            return self._pending_commit_version
+        else:
+            raise RuntimeError("version has not been committed yet")
 
-        kw: t.Dict[str, t.Any] = {"disable_copy_src": not self._enable_copy_src}
-        if self._enable_copy_src:
-            config.pkg_data = self._build_include_files
-            config.exclude_pkg_data = self._build_exclude_files
-            kw["workdir"] = self._build_src_dir
-
-        # TODO: support DatasetAttr config for SDK
-        config.do_validate()
-        kw["config"] = config
-        # TODO: support build tmpdir, follow the swcli dataset build command behavior
-        self.__core_dataset.buildImpl(**kw)
-        _summary = self.__core_dataset.summary()
-        self._rows_cnt = _summary.rows if _summary else 0
+    @property
+    def uri(self) -> URI:
+        """Dataset URI
+
+        Before committing, the uri is for the loading_version.
+        After committing, the uri is for the committed_version.
+
+        Returns:
+            A URI object.
+        """
+        if self.__has_committed:
+            return self._pending_commit_uri
+        else:
+            return self._loading_uri
+
+    @property
+    def changed(self) -> bool:
+        """For the non-readonly dataset, when the users update/delete/add records(rows) or features(columns),
+        changed property will change from False to True.
+
+        Returns:
+            True or False
+        """
+        return self._updated_rows_by_commit != 0 or self._deleted_rows_by_commit != 0
 
     @_check_readonly
-    def build(self) -> None:
-        if self._trigger_icode_build:
-            self._do_build_from_interactive_code()
-        elif self._trigger_handler_build and self.build_handler:
-            self._do_build_from_handler()
+    def commit(self, tags: t.Optional[t.List[str]] = None, message: str = "") -> str:
+        """Commit into dataset
+        Commit will flush and generate a version of the dataset. At the same time, commit
+        operation will also generate auto-increment tag, such as v0, v1, v2. Only one commit is allowed.
+
+        Arguments:
+            tags: (list(str), optional) Specify the tags for the version. Default is None.
+            message: (str, optional) Commit message. Default is empty str.
+
+        Example:
+        ```python
+        from starwhale import dataset
+        with dataset("mnist") as ds:
+            ds.append({"label": 1})
+            ds.commit(message="init commit")
+        ```
+
+        Return:
+            A str of dataset version.
+        """
+        # TODO: forbid commit many times
+        with self._commit_lock:
+            return self._commit(tags or [], message)
+
+    def _commit(self, tags: t.List[str], message: str) -> str:
+        def _save_info() -> str:
+            revision = ""
+            if self.__info is not None and self._info_ds_wrapper is not None:
+                revision = self.__info.save_to_datastore(self._info_ds_wrapper)
+                self._last_info_datastore_revision = revision
+            return revision
+
+        def _dump_manifest(dataset_revision: str, info_revision: str) -> Path:
+            if self._dataset_builder is None:
+                raise RuntimeError("failed to commit, because dataset builder is None")
+
+            increased_blobs_size = sum(
+                [m.size for m in self._dataset_builder.signature_bins_meta]
+            )
+
+            _manifest = {
+                "build": {
+                    "os": platform.system(),
+                    "starwhale": STARWHALE_VERSION,
+                },
+                "version": self._pending_commit_version,
+                CREATED_AT_KEY: now_str(),
+                "dataset_summary": DatasetSummary(
+                    rows=self._dataset_builder.calculate_rows_cnt(),  # maybe slow
+                    updated_rows=self._updated_rows_by_commit,
+                    deleted_rows=self._deleted_rows_by_commit,
+                    blobs_byte_size=self._total_blobs_size + increased_blobs_size,
+                    increased_blobs_byte_size=increased_blobs_size,
+                ).asdict(),
+                "message": message,
+            }
+
+            _manifest.update(
+                DatastoreRevision(data=dataset_revision, info=info_revision).asdict()
+            )
+
+            self._updated_rows_by_commit = 0
+            self._deleted_rows_by_commit = 0
+
+            _m_path = self.tmpdir / DEFAULT_MANIFEST_NAME
+            ensure_file(
+                _m_path,
+                yaml.safe_dump(_manifest, default_flow_style=False),
+                parents=True,
+            )
+            return _m_path
+
+        def _submit_standalone_version(manifest_path: Path) -> None:
+            pccd = self.__pending_commit_core_dataset
+            if not isinstance(pccd, StandaloneDataset):
+                raise RuntimeError(
+                    f"core dataset is not StandaloneDataset instance: {pccd}"
+                )
+
+            _snapshot_dir = pccd.store.snapshot_workdir
+            ensure_dir(_snapshot_dir)
+            copy_file(
+                manifest_path,
+                pccd.store.snapshot_workdir / DEFAULT_MANIFEST_NAME,
+            )
+            pccd.tag.add_fast_tag()
+
+        def _submit_cloud_version(manifest_path: Path) -> None:
+            from starwhale.base.bundle_copy import _UploadPhase
+
+            crm = CloudRequestMixed()
+            params = {
+                "swds": f"{self.name}:{self._pending_commit_version}",
+                "project": self.project_uri.project,
+                "force": "1",  # stash version is unique, use force=1 to make http retry happy
+            }
+            url_path = f"/project/{self.project_uri.project}/dataset/{self.name}/version/{self._pending_commit_version}/file"
+            r = crm.do_multipart_upload_file(
+                url_path=url_path,
+                file_path=manifest_path,
+                instance_uri=self.project_uri,
+                params={
+                    "phase": _UploadPhase.MANIFEST,
+                    "desc": FileDesc.MANIFEST.name,
+                    **params,
+                },
+                use_raise=True,
+            )
+            crm.do_http_request(
+                path=url_path,
+                method=HTTPMethod.POST,
+                instance_uri=self.project_uri,
+                data={
+                    "phase": _UploadPhase.END,
+                    "uploadId": r.json()["data"]["uploadId"],
+                    **params,
+                },
+                use_raise=True,
+                disable_default_content_type=True,
+            )
+
+        if self.__has_committed:
+            raise RuntimeError("Dataset has already committed")
+
+        dataset_revision = self.flush(artifacts_flush=True)
+        info_revision = _save_info()
+        manifest_path = _dump_manifest(dataset_revision, info_revision)
+
+        logger.debug(
+            f"dataset commit: revision-{dataset_revision}, info revision-{info_revision}"
+        )
+        if self.project_uri.instance == STANDALONE_INSTANCE:
+            _submit_standalone_version(manifest_path)
         else:
-            raise RuntimeError("no data to build dataset")
+            _submit_cloud_version(manifest_path)
+        os.unlink(manifest_path)
 
-    commit = build
+        if tags:
+            self.__pending_commit_core_dataset.add_tags(tags)
 
-    def copy(
-        self, dest_uri: str, force: bool = False, dest_local_project_uri: str = ""
-    ) -> None:
+        self.__has_committed = True
+        return self._pending_commit_version
+
+    @property
+    def committed(self) -> bool:
+        """Check If the dataset is committed.
+
+        Returns:
+            True or False
+        """
+        return self.__has_committed
+
+    def copy(self, dest_uri: str, dest_local_project_uri: str = "") -> None:
         CoreDataset.copy(
             str(self.uri),
             dest_uri,
-            force=force,
             dest_local_project_uri=dest_local_project_uri,
         )
 
-    @staticmethod
+    @classmethod
     def list(
+        cls,
         project_uri: t.Union[str, URI] = "",
         fullname: bool = False,
         show_removed: bool = False,
         page_index: int = DEFAULT_PAGE_IDX,
         page_size: int = DEFAULT_PAGE_SIZE,
     ) -> t.Tuple[t.List[t.Dict[str, t.Any]], t.Dict[str, t.Any]]:
         from starwhale.core.dataset.view import DatasetTermView
 
         return DatasetTermView.list(
             project_uri, fullname, show_removed, page_index, page_size
         )
 
-    @staticmethod
+    @classmethod
     def dataset(
+        cls,
         uri: t.Union[str, URI],
-        create: bool = False,
-        create_from_handler: t.Optional[_HandlerType] = None,
+        create: str = _DatasetCreateMode.auto,
+        readonly: bool = False,
     ) -> Dataset:
+        """Create or load a dataset from standalone instance or cloud instance.
+
+        For a non-existed dataset, when you try to load it, you will get an Exception; when you try to append records and commit,
+        the dataset will be created automatically.
+
+        Arguments:
+            uri: (str, URI, required) The dataset uri.
+            create: (str, optional) The mode of dataset creating. The options are `auto`, `empty` and `forbid`.
+                `auto` mode: If the dataset already exists, creation is ignored. If it does not exist, the dataset is created automatically.
+                `empty` mode: If the dataset already exists, an Exception is raised; If it does not exist, an empty dataset is created. This mode ensures the creation of a new, empty dataset.
+                `forbid` mode: If the dataset already exists, nothing is done.If it does not exist, an Exception is raised. This mode ensures the existence of the dataset.
+                The default is `auto`.
+            readonly: (bool, optional) For an existing dataset, you can specify the readonly=True argument to ensure
+                the dataset is in readonly mode. Default is False.
+
+        Returns:
+            A Dataset Object
+
+        Examples:
+        ```python
+        from starwhale import dataset, Image
+
+        # create a new dataset named mnist, and add a row into the dataset
+        # dataset("mnist") is equal to dataset("mnist", create="auto")
+        ds = dataset("mnist")
+        ds.exists()  # return False, "mnist" dataset is not existing.
+        ds.append({"img": Image(), "label": 1})
+        ds.commit()
+        ds.close()
+
+        # load a cloud instance dataset in readonly mode
+        ds = dataset("cloud://remote-instance/project/starwhale/dataset/mnist", readonly=True)
+        labels = [row.features.label in ds]
+        ds.close()
+
+        # load a read/write dataset with a specified version
+        ds = dataset("mnist/version/mrrdczdbmzsw")
+        ds[0].features.label = 1
+        ds.commit()
+        ds.close()
+
+        # create an empty dataset
+        ds = dataset("mnist-empty", create="empty")
+
+        # ensure the dataset existence
+        ds = dataset("mnist-existed", create="forbid")
+        ```
+
+        """
         if isinstance(uri, str):
             _uri = URI(uri, expected_type=URIType.DATASET)
         elif isinstance(uri, URI) and uri.object.typ == URIType.DATASET:
             _uri = uri
         else:
             raise TypeError(
                 f"uri({uri}) argument type is not expected, dataset uri or str is ok"
             )
 
         ds = Dataset(
             name=_uri.object.name,
             version=_uri.object.version,
             project_uri=_uri,  # TODO: cut off dataset resource info?
-            create=create or bool(create_from_handler),
+            readonly=readonly,
+            create=create or _DatasetCreateMode.auto,
         )
 
-        if create_from_handler:
-            ds.build_handler = create_from_handler
+        return ds
 
+    @classmethod
+    def from_json(cls, name: str, json_text: str, field_selector: str = "") -> Dataset:
+        """Create a new dataset from a dict.
+        Arguments:
+            name: (str, required) The dataset name you would like to use.
+            json_text: (str, required) The json text from which you would like to create this dataset
+            field_selector: (str, optional) The filed from which you would like to extract dataset array items.
+                The default value is "" which indicates that the dict is an array contains all the items.
+            Returns:
+                A Dataset Object
+            Examples:
+            ```python
+            from starwhale import Dataset
+            myds = Dataset.from_json("translation", '[{"en":"hello","zh-cn":"你好"},{"en":"how are you","zh-cn":"最近怎么样"}]')
+            print(myds[0].features.en)
+            ```
+            ```python
+            from starwhale import Dataset
+            myds = Dataset.from_json("translation", '{"content":{"child_content":[{"en":"hello","zh-cn":"你好"},{"en":"how are you","zh-cn":"最近怎么样"}]}}',"content.child_content")
+            print(myds[0].features["zh-cn"])
+            ```
+        """
+        data_items = json.loads(json_text)
+        if field_selector:
+            # Split field selector by dots
+            fields = field_selector.split(".")
+            # Iterate over selected fields
+            for field in fields:
+                if field in data_items:
+                    data_items = data_items[field]
+                else:
+                    raise ValueError(
+                        f"The field_selector {field_selector} isn't in json_text: {json_text}"
+                    )
+        if not isinstance(data_items, list):
+            raise ValueError(
+                f"The field selected by field_selector {field_selector} isn't an array: {data_items}"
+            )
+        ds = cls.dataset(name)
+        for item in data_items:
+            ds.append(item)
+        ds.commit()
+        ds.close()
         return ds
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `starwhale-0.4.1/starwhale/api/_impl/job.py` & `starwhale-0.4.2/starwhale/api/_impl/job.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,46 @@
+from __future__ import annotations
+
 import sys
 import typing as t
+import inspect
 import numbers
 import threading
+from copy import deepcopy
 from pathlib import Path
 from functools import wraps
+from collections import defaultdict
 
 import yaml
 from loguru import logger
 
-from starwhale.consts import DEFAULT_EVALUATION_JOB_NAME
+from starwhale.consts import DEFAULT_JOB_NAME, DecoratorInjectAttr
 from starwhale.core.job import dag
 from starwhale.utils.fs import ensure_file
 from starwhale.utils.load import load_module
+from starwhale.utils.error import NoSupportError
+from starwhale.core.job.step import Step
+from starwhale.core.job.context import Context
+
+AFTER_LOAD_HOOKS: t.Dict[str, t.Callable] = defaultdict()
+_T_JOBS = t.Dict[str, t.List[Step]]
+_jobs_global: _T_JOBS = defaultdict(list)
+_jobs_global_lock = threading.Lock()
+
+
+# TODO: refactor _do_resource_transform, move it into Step
+def _do_resource_transform(resources: t.Optional[t.Dict[str, t.Any]]) -> t.List[t.Dict]:
+    attribute_names = ["request", "limit"]
+    resource_names: t.Dict[str, t.List] = {
+        "cpu": [int, float],
+        "nvidia.com/gpu": [int],
+        "memory": [int, float],
+    }
 
-context_holder = threading.local()
-resource_names: t.Dict[str, t.List] = {
-    "cpu": [int, float],
-    "nvidia.com/gpu": [int],
-    "memory": [int, float],
-}
-attribute_names = ["request", "limit"]
-
-
-def do_resource_transform(resources: t.Dict[str, t.Any]) -> t.List[t.Dict]:
+    resources = resources or {}
     results = []
     for _name, _resource in resources.items():
         if _name not in resource_names:
             raise RuntimeError(
                 f"resources name is illegal, name must in {resource_names.keys()}"
             )
 
@@ -35,202 +49,151 @@
         elif isinstance(_resource, dict):
             if not all(n in attribute_names for n in _resource):
                 raise RuntimeError(
                     f"resources value is illegal, attribute's name must in {attribute_names}"
                 )
         else:
             raise RuntimeError(
-                "resources value is illegal, attribute's type must be numer or dict"
+                "resources value is illegal, attribute's type must be number or dict"
             )
 
         for _k, _v in resources[_name].items():
             if type(_v) not in resource_names[_name]:
                 raise RuntimeError(
                     f"resource:{_name} only support type:{resource_names[_name]}, but now is {type(_v)}"
                 )
             if _v <= 0:
                 raise RuntimeError(
-                    f"{_k} only supports non-negative numbers, but now is {_v}"
+                    f"{_k} only supports non-negative number, but now is {_v}"
                 )
         results.append(
             {
                 "type": _name,
                 "request": resources[_name]["request"],
                 "limit": resources[_name]["limit"],
             }
         )
     return results
 
 
 def step(
-    job_name: str = DEFAULT_EVALUATION_JOB_NAME,
+    job_name: str = DEFAULT_JOB_NAME,
     resources: t.Optional[t.Dict[str, t.Any]] = None,
     concurrency: int = 1,
     task_num: int = 1,
     needs: t.Optional[t.List[str]] = None,
-) -> t.Any:
-    _resources = resources or {}
-    _needs = needs or []
-
-    def decorator(func: t.Any) -> t.Any:
-        if Parser.is_parse_stage():
-            cls, _, func_name = func.__qualname__.rpartition(".")
-
-            _step = dict(
-                job_name=job_name,
-                step_name=func_name,
-                cls_name=cls,
-                resources=do_resource_transform(_resources),
-                concurrency=concurrency,
-                task_num=task_num,
-                needs=_needs,
+    extra_args: t.Optional[t.List] = None,
+    extra_kwargs: t.Optional[t.Dict] = None,
+    name: str = "",
+) -> t.Callable:
+    def decorator(func: t.Callable) -> t.Callable:
+        module = inspect.getmodule(func)
+        if module is None:
+            raise RuntimeError(f"cannot get module name from func: {func}")
+
+        if inspect.isclass(func):
+            raise NoSupportError(f"step decorator no support class: {func}")
+
+        cls_name, _, func_name = func.__qualname__.rpartition(".")
+        if "." in cls_name:
+            raise NoSupportError(
+                f"step decorator no supports inner class method:{func.__qualname__}"
             )
-            Parser.add_job(job_name, _step)
 
+        _step = Step(
+            job_name=job_name,
+            name=name or func_name,
+            func_name=func_name,
+            cls_name=cls_name,
+            module_name=module.__name__,
+            concurrency=concurrency,
+            task_num=task_num,
+            needs=needs,
+            resources=_do_resource_transform(resources),
+            extra_args=extra_args,
+            extra_kwargs=extra_kwargs,
+        )
+
+        global _jobs_global, _jobs_global_lock
+        with _jobs_global_lock:
+            _jobs_global[job_name].append(_step)
+
+        setattr(func, DecoratorInjectAttr.Step, True)
         return func
 
     return decorator
 
 
+def _validate_jobs_dag(jobs: _T_JOBS) -> None:
+    for steps in jobs.values():
+        _vertices: t.List[str] = []
+        _edges: t.Dict[str, str] = {}
+        for _step in steps:
+            _vertices.append(_step.name)
+            for _pre in _step.needs:
+                if _pre:
+                    _edges[_pre] = _step.name
+
+        dag.generate_dag(_vertices, _edges)
+
+
+def _preload_to_register_jobs(run_handler: str, workdir: Path) -> None:
+    """
+    run_handler formats:
+    - to.one.module
+    - to.one.module:function  --> with @step, @predict decorator
+    - to.one.module:ArbitraryClass  --> use @step or @predict to decorate some class methods
+    - to.one.module:PipeHandlerSubClass
+    """
+    module_name, _, func_or_cls_name = run_handler.partition(":")
+
+    # reload for the multi model.build in one python process
+    if module_name in sys.modules:
+        del sys.modules[module_name]
+
+    module = load_module(module_name, workdir)
+    func_or_cls = getattr(module, func_or_cls_name, None)
+
+    if func_or_cls is None:
+        logger.debug(f"preload module-{module_name}")
+        return
+
+    for _, _h in AFTER_LOAD_HOOKS.items():
+        _h(run_handler, func_or_cls)
+
+
+def generate_jobs_yaml(
+    run_handler: str, workdir: t.Union[Path, str], yaml_path: t.Union[Path, str]
+) -> None:
+    workdir = Path(workdir)
+    logger.debug(f"ingest steps from run_handler {run_handler} at {workdir}")
+
+    _preload_to_register_jobs(run_handler, workdir)
+
+    global _jobs_global, _jobs_global_lock
+    with _jobs_global_lock:
+        jobs = deepcopy(_jobs_global)
+
+        _names = list(_jobs_global.keys())
+        [_jobs_global.__delitem__(n) for n in _names]  # type: ignore[func-returns-value]
+
+    if not jobs:
+        raise RuntimeError("not found any jobs")
+
+    _validate_jobs_dag(jobs)
+    ensure_file(
+        yaml_path,
+        yaml.safe_dump(
+            {job_name: [s.asdict() for s in steps] for job_name, steps in jobs.items()},
+            default_flow_style=False,
+        ),
+        parents=True,
+    )
+
+
 def pass_context(func: t.Any) -> t.Any:
     @wraps(func)
     def wrap_func(*args: t.Any, **kwargs: t.Any) -> t.Any:
-        kwargs["context"] = context_holder.context
+        kwargs["context"] = Context.get_runtime_context()
         return func(*args, **kwargs)
 
     return wrap_func
-
-
-# TODO: support __setattr__, __getattr__ function for Context
-# TODO: use another Context name, such as JobRunContext
-class Context:
-    def __init__(
-        self,
-        workdir: Path,
-        step: str = "",
-        total: int = 1,
-        index: int = 0,
-        dataset_uris: t.List[str] = [],
-        version: str = "",
-        project: str = "",
-    ):
-        self.project = project
-        self.version = version
-        self.step = step
-        self.total = total
-        self.index = index
-        self.dataset_uris = dataset_uris
-        self.workdir = workdir
-
-    def __str__(self) -> str:
-        return f"step:{self.step}, index:{self.index}/{self.total}"
-
-    def __repr__(self) -> str:
-        return f"step:{self.step}, index:{self.index}/{self.total}, version:{self.version}, dataset_uris:{self.dataset_uris}"
-
-
-class ParseConfig:
-    def __init__(self, is_parse_stage: bool, jobs: t.Dict[str, t.List[t.Dict]]):
-        self.parse_stage = is_parse_stage
-        self.jobs = jobs
-
-    def clear(self) -> None:
-        self.jobs = {}
-
-
-# shared memory, not thread safe
-parse_config = ParseConfig(False, {})
-
-
-class Parser:
-    @staticmethod
-    def set_parse_stage(parse_stage: bool) -> None:
-        parse_config.parse_stage = parse_stage
-
-    @staticmethod
-    def is_parse_stage() -> bool:
-        return parse_config.parse_stage
-
-    @staticmethod
-    def add_job(job_name: str, step: t.Dict) -> None:
-        _jobs = parse_config.jobs
-        if job_name not in _jobs:
-            parse_config.jobs[job_name] = []
-
-        parse_config.jobs[job_name].append(step)
-
-    @staticmethod
-    def get_jobs() -> t.Dict[str, t.List[t.Dict]]:
-        return parse_config.jobs
-
-    # load is unique,so don't need to think multi load and clean
-    @staticmethod
-    def clear_config() -> None:
-        global parse_config
-        parse_config.clear()
-
-    @staticmethod
-    def parse_job_from_module(module: str, path: Path) -> t.Dict[str, t.List[t.Dict]]:
-        """
-        parse @step from module
-        :param module: module name
-        :param path: abs path
-        :return: jobs
-        """
-        Parser.set_parse_stage(True)
-        # parse DAG
-        logger.debug(f"parse @step for module:{module}")
-        if module in sys.modules:
-            del sys.modules[module]
-        load_module(module, path)
-        _jobs = Parser.get_jobs().copy()
-        Parser.clear_config()
-        return _jobs
-
-    @staticmethod
-    def generate_job_yaml(module: str, path: Path, target_file: Path) -> None:
-        """
-        generate job yaml
-        :param target_file: yaml target path
-        :param module: module name
-        :param path: abs path
-        :return: None
-        """
-        _jobs = Parser.parse_job_from_module(module, path)
-        # generate DAG
-        logger.debug("generate DAG")
-        if Parser.check(_jobs):
-            # dump to target
-            ensure_file(
-                target_file,
-                yaml.safe_dump(_jobs, default_flow_style=False),
-                parents=True,
-            )
-            logger.debug("generator DAG success!")
-        else:
-            logger.error("generator DAG error! reason: check is failed.")
-            raise RuntimeError("generator DAG error!")
-
-    @staticmethod
-    def check(jobs: t.Dict[str, t.List[t.Dict]]) -> bool:
-        if not jobs:
-            raise ValueError("EMPTY job specification error!")
-
-        checks = []
-        logger.debug(f"check jobs:{jobs}")
-
-        for name, steps in jobs.items():
-            _vertices: t.List[str] = []
-            _edges: t.Dict[str, str] = {}
-            for _step in steps:
-                _vertices.append(_step["step_name"])
-                for _pre in _step["needs"]:
-                    if _pre:
-                        _edges[_pre] = _step["step_name"]
-            try:
-                dag.generate_dag(_vertices, _edges)
-                checks.append(True)
-            except RuntimeError as e:
-                logger.error(f"check job:{name} failed, error:{e}")
-                checks.append(False)
-
-        return all(checks)
```

### Comparing `starwhale-0.4.1/starwhale/api/_impl/metric.py` & `starwhale-0.4.2/starwhale/api/_impl/metric.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,17 +10,16 @@
     hamming_loss,
     confusion_matrix,
     cohen_kappa_score,
     classification_report,
     multilabel_confusion_matrix,
 )
 
+from starwhale.api import evaluation
 from starwhale.utils.dict import flatten as flatten_dict
-from starwhale.api._impl.job import context_holder
-from starwhale.api._impl.wrapper import Evaluation
 
 
 @unique
 class MetricKind(Enum):
     MultiClassification = "multi_classification"
 
 
@@ -32,16 +31,14 @@
     all_labels: t.Optional[t.List[t.Any]] = None,
 ) -> t.Any:
     def _decorator(func: t.Any) -> t.Any:
         @wraps(func)
         def _wrapper(*args: t.Any, **kwargs: t.Any) -> t.Dict[str, t.Any]:
             y_pr: t.Any = None
 
-            context = context_holder.context
-            evaluation = Evaluation(eval_id=context.version, project=context.project)
             _rt = func(*args, **kwargs)
             if show_roc_auc:
                 y_true, y_pred, y_pr = _rt
             else:
                 y_true, y_pred = _rt
 
             _r: t.Dict[str, t.Any] = {"kind": MetricKind.MultiClassification.value}
@@ -59,15 +56,16 @@
             if show_hamming_loss:
                 _r["summary"]["hamming_loss"] = hamming_loss(y_true, y_pred)
             if show_cohen_kappa_score:
                 _r["summary"]["cohen_kappa_score"] = cohen_kappa_score(y_true, y_pred)
 
             _record_summary = flatten_dict(_r["summary"], extract_sequence=True)
             _record_summary["kind"] = _r["kind"]
-            evaluation.log_metrics(_record_summary)
+
+            evaluation.log_summary(_record_summary)
 
             _r["labels"] = {}
             mcm = multilabel_confusion_matrix(
                 y_true, y_pred, labels=all_labels
             ).tolist()
 
             labels = all_labels or sorted([k for k in cr.keys() if k not in _summary_m])
@@ -83,48 +81,52 @@
                         "FP-False Positive": matrix[0][1],
                         "FN-False Negative": matrix[1][0],
                         "TP-True Positive": matrix[1][1],
                     }
                 )
 
                 _r["labels"][_label] = _report
-                evaluation.log("labels", id=_label, **_report)
+                evaluation.log("labels", id=_label, metrics=_report)
 
             # TODO: tune performance, use intermediated result
             cm = confusion_matrix(
                 y_true, y_pred, labels=all_labels, normalize=confusion_matrix_normalize
             )
             _cm_list = cm.tolist()
             _r["confusion_matrix"] = {"binarylabel": _cm_list}
 
             for _idx, _pa in enumerate(_cm_list):
                 evaluation.log(
                     "confusion_matrix/binarylabel",
                     id=_idx,
-                    **{str(_id): _v for _id, _v in enumerate(_pa)},
+                    metrics={str(_id): _v for _id, _v in enumerate(_pa)},
                 )
 
             if show_roc_auc and all_labels is not None and y_true and y_pr:
                 _r["roc_auc"] = {}
                 for _idx, _label in enumerate(all_labels):
                     _ra_value = _calculate_roc_auc(y_true, y_pr, _label, _idx)
                     _r["roc_auc"][str(_label)] = _ra_value
 
                     for _id, (_fpr, _tpr, _threshold) in enumerate(
                         zip(_ra_value["fpr"], _ra_value["tpr"], _ra_value["thresholds"])
                     ):
                         evaluation.log(
                             f"roc_auc/{_label}",
                             id=_id,
-                            fpr=_fpr,
-                            tpr=_tpr,
-                            threshold=_threshold,
+                            metrics=dict(
+                                tpr=_tpr,
+                                fpr=_fpr,
+                                threshold=_threshold,
+                            ),
                         )
 
-                        evaluation.log("labels", id=str(_label), auc=_ra_value["auc"])
+                        evaluation.log(
+                            "labels", id=str(_label), metrics=dict(auc=_ra_value["auc"])
+                        )
             return _r
 
         return _wrapper
 
     return _decorator
```

### Comparing `starwhale-0.4.1/starwhale/api/_impl/model.py` & `starwhale-0.4.2/starwhale/api/_impl/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,36 +7,39 @@
 from pathlib import Path
 
 import yaml
 
 from starwhale.utils import disable_progress_bar
 from starwhale.consts import DefaultYAMLName
 from starwhale.utils.fs import ensure_file
+from starwhale.consts.env import SWEnv
 
 _path_T = t.Union[str, Path]
 
 
 def build(
     evaluation_handler: t.Any,
-    name: t.Optional[str] = None,
     workdir: t.Optional[_path_T] = None,
-    desc: str = "",
+    name: t.Optional[str] = None,
     project_uri: str = "",
+    desc: str = "",
+    remote_project_uri: t.Optional[str] = None,
 ) -> None:
     """Build Starwhale Model Package.
 
     In common case, you may call `build` function in your experiment scripts.`build` function is a shortcut for the `swcli model build` command.
 
     Arguments:
         evaluation_handler: (str, object, required) The evaluation handler supports object(function, class or module) or str(example: "to.path.module:name").
         name: (str, optional) The name of Starwhale Model Package, default is the current work dir.
         workdir: (str, Pathlib.Path, optional) The path of the rootdir. The default workdir is the current working dir.
         desc: (str, optional) The description of the Starwhale Model Package.
         project_uri: (str, optional) The project uri of the Starwhale Model Package. If the argument is not specified,
             the project_uri is the config value of `swcli project select` command.
+        remote_project_uri: (str, optional) The destination project uri(cloud://remote-instance/project/starwhale) of the Starwhale Model Package
 
     Examples:
     ```python
     from starwhale import model
 
     # class handler
     from .user.code.evaluator import ExamplePipelineHandler
@@ -77,14 +80,29 @@
     try:
         with disable_progress_bar():
             ModelTermView.build(
                 workdir=workdir,
                 project=project_uri,
                 yaml_path=yaml_path,
             )
+
+            from starwhale import URI, URIType
+
+            if remote_project_uri:
+                remote_project_uri = URI(
+                    remote_project_uri, expected_type=URIType.PROJECT
+                ).full_uri
+            elif os.getenv(SWEnv.instance_uri) and os.getenv(SWEnv.project):
+                remote_project_uri = f"{os.getenv(SWEnv.instance_uri)}/project/{os.getenv(SWEnv.project)}"
+
+            if remote_project_uri:
+                ModelTermView.copy(
+                    src_uri=f"{URI(project_uri).full_uri}/model/{name}/version/latest",
+                    dest_uri=remote_project_uri,
+                )
     finally:
         os.unlink(yaml_path)
 
 
 def _ingest_obj_entrypoint_name(
     obj: t.Any,
     workdir: Path,
```

### Comparing `starwhale-0.4.1/starwhale/api/_impl/service.py` & `starwhale-0.4.2/starwhale/api/_impl/service.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/api/_impl/track/base.py` & `starwhale-0.4.2/starwhale/api/_impl/track/base.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/api/_impl/track/collector.py` & `starwhale-0.4.2/starwhale/api/_impl/track/collector.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/api/_impl/track/handler.py` & `starwhale-0.4.2/starwhale/api/_impl/track/handler.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,17 +3,23 @@
 import json
 import queue
 import typing as t
 import threading
 from pathlib import Path
 from collections import defaultdict
 
-from starwhale.utils.fs import ensure_dir, ensure_file
+from starwhale.consts import VERSION_PREFIX_CNT
+from starwhale.utils.fs import (
+    ensure_dir,
+    ensure_file,
+    blake2b_content,
+    BLAKE2B_SIGNATURE_ALGO,
+)
 from starwhale.utils.error import NoSupportError
-from starwhale.core.dataset.type import Link
+from starwhale.core.dataset.type import Link, BaseArtifact
 from starwhale.api._impl.data_store import TableWriter, LocalDataStore
 
 from .base import (
     TrackRecord,
     ParamsRecord,
     MetricsRecord,
     ArtifactsRecord,
@@ -73,20 +79,49 @@
         row = MetricsTabularRow.from_record(record)
         table_name = f"{record.typ.value}/{record.source.value}"
         self._update_table(table_name, row.asdict(), "__step")
 
     def _handle_artifacts(self, record: ArtifactsRecord) -> None:
         table_name = f"{record.typ.value}/{record.source.value}"
         store_dir = self._workdir / record.typ.value / "_files"
+
+        def _convert_data_to_link(data: BaseArtifact) -> Link:
+            raw_content = data.to_bytes()
+            sign_name = blake2b_content(raw_content)
+            fpath = (
+                store_dir
+                / BLAKE2B_SIGNATURE_ALGO
+                / sign_name[:VERSION_PREFIX_CNT]
+                / sign_name
+            )
+            ensure_file(fpath, raw_content, parents=True)
+
+            return Link(
+                uri=sign_name,
+                offset=0,
+                size=len(raw_content),
+                use_plain_type=True,
+                data_type=data,
+            )
+
         for k, v in record.data.items():
+            if isinstance(v, Link):
+                data = v
+            elif isinstance(v, BaseArtifact):
+                data = _convert_data_to_link(v)
+            else:
+                raise NoSupportError(
+                    f"artifact only accepts BaseArtifact or Link type: {v}"
+                )
+
             row = ArtifactsTabularRow(
                 name=k,
                 index=self._artifacts_counter[k],
                 created_at=record.clock_time,
-                data=Link.from_local_artifact(v, store_dir),
+                data=data,
                 link_wrapper=not isinstance(v, Link),
             )
             self._update_table(table_name, row.asdict(), "__key")
             self._artifacts_counter[k] += 1
 
     def _handle_params(self, record: ParamsRecord) -> None:
         self._params[record.source.value].update(record.data)
```

### Comparing `starwhale-0.4.1/starwhale/api/_impl/track/hooker.py` & `starwhale-0.4.2/starwhale/api/_impl/track/hooker.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/api/_impl/track/tracker.py` & `starwhale-0.4.2/starwhale/api/_impl/track/tracker.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/api/_impl/wrapper.py` & `starwhale-0.4.2/starwhale/api/_impl/wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,25 +7,23 @@
 from functools import lru_cache
 
 import dill
 import requests
 from loguru import logger
 
 from starwhale.consts import VERSION_PREFIX_CNT, STANDALONE_INSTANCE
+from starwhale.consts.env import SWEnv
+from starwhale.utils.retry import http_retry
+from starwhale.utils.config import SWCliConfigMixed
 
 from . import data_store
-from ...consts.env import SWEnv
-from ...utils.retry import http_retry
-from ...utils.config import SWCliConfigMixed
 
 
 class Logger:
-    def _init_writers(
-        self, tables: List[str], store: Optional[data_store.DataStore] = None
-    ) -> None:
+    def _init_writers(self, tables: List[str]) -> None:
         self._writers: Dict[str, Optional[data_store.TableWriter]] = {
             table: None for table in tables
         }
         self._lock = threading.Lock()
 
     def close(self) -> None:
         with self._lock:
@@ -54,20 +52,20 @@
                 self._writers[table_name] = writer
         return writer
 
     def _log(self, table_name: str, record: Dict[str, Any]) -> None:
         writer = self._fetch_writer(table_name)
         writer.insert(record)
 
-    def _flush(self, table_name: str) -> None:
+    def _flush(self, table_name: str) -> str:
         with self._lock:
             writer = self._writers.get(table_name)
             if writer is None:
-                return
-        writer.flush()
+                return ""
+        return writer.flush()
 
     def _delete(self, table_name: str, key: Any) -> None:
         writer = self._fetch_writer(table_name)
         writer.delete(key)
 
 
 def _serialize(data: Any) -> Any:
@@ -158,17 +156,17 @@
         super()._log(_storage_table_name, record)
 
     def _get(self, table_name: str) -> Iterator[Dict[str, Any]]:
         return self._data_store.scan_tables(
             [data_store.TableDesc(self._get_storage_table_name(table=table_name))]
         )
 
-    def _flush(self, table_name: str) -> None:
+    def _flush(self, table_name: str) -> str:
         _storage_table_name = self._get_storage_table_name(table_name)
-        super()._flush(_storage_table_name)
+        return super()._flush(_storage_table_name)
 
     def log_result(
         self,
         data_id: Union[int, str],
         result: Any,
         serialize: bool = False,
         **kwargs: Any,
@@ -235,32 +233,35 @@
     META = "meta"
     INFO = "info"
 
 
 class Dataset(Logger):
     def __init__(
         self,
-        dataset_id: str,
+        dataset_name: str,
         project: str,
+        dataset_scan_revision: str = "",
         instance_name: str = "",
         token: str = "",
         kind: DatasetTableKind = DatasetTableKind.META,
     ) -> None:
-        if not dataset_id:
+        if not dataset_name:
             raise RuntimeError("id should not be None")
 
         if not project:
             raise RuntimeError("project is not set")
 
-        self.dataset_id = dataset_id
+        self.dataset_scan_revision = dataset_scan_revision
         self.project = project
-        self._kind = kind
+        self.kind = kind
+
+        # _current is only holder part of the dataset table name
         self._table_name = _gen_storage_table_name(
             project=project,
-            table=f"dataset/{self.dataset_id}/{kind.value}",
+            table=f"dataset/{dataset_name}/_current/{kind.value}",
             instance_uri=instance_name,
         )
         self._data_store = data_store.get_data_store(instance_name, token)
         self._init_writers([self._table_name])
 
     def put(self, data_id: Union[str, int], **kwargs: Any) -> None:
         record = {"id": data_id}
@@ -268,33 +269,52 @@
             record[k.lower()] = v
         self._log(self._table_name, record)
 
     def delete(self, data_id: Union[str, int]) -> None:
         self._delete(self._table_name, data_id)
 
     def scan(
-        self, start: Any, end: Any, end_inclusive: bool = False
+        self,
+        start: Any,
+        end: Any,
+        end_inclusive: bool = False,
+        revision: str = "",
     ) -> Iterator[Dict[str, Any]]:
         return self._data_store.scan_tables(
-            [data_store.TableDesc(self._table_name)],
+            [
+                data_store.TableDesc(
+                    table_name=self._table_name,
+                    revision=revision or self.dataset_scan_revision,
+                )
+            ],
             start=start,
             end=end,
             end_inclusive=end_inclusive,
         )
 
     def scan_id(
-        self, start: Any, end: Any, end_inclusive: bool = False
+        self,
+        start: Any,
+        end: Any,
+        end_inclusive: bool = False,
+        revision: str = "",
     ) -> Iterator[Any]:
         return self._data_store.scan_tables(
-            [data_store.TableDesc(self._table_name, columns=["id"])],
+            [
+                data_store.TableDesc(
+                    table_name=self._table_name,
+                    columns=["id"],
+                    revision=revision or self.dataset_scan_revision,
+                )
+            ],
             start=start,
             end=end,
             end_inclusive=end_inclusive,
         )
 
-    def flush(self) -> None:
-        self._flush(self._table_name)
+    def flush(self) -> str:
+        return self._flush(self._table_name)
 
     def __str__(self) -> str:
-        return f"Dataset Wrapper, table:{self._table_name}, store:{self._data_store}, kind: {self._kind}"
+        return f"Dataset Wrapper, table:{self._table_name}, store:{self._data_store}, kind: {self.kind}, revision: {self.dataset_scan_revision}"
 
     __repr__ = __str__
```

### Comparing `starwhale-0.4.1/starwhale/api/dataset.py` & `starwhale-0.4.2/starwhale/api/dataset.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,35 +13,31 @@
     LinkType,
     MIMEType,
     ClassLabel,
     S3LinkAuth,
     BoundingBox,
     NumpyBinary,
     BoundingBox3D,
-    BuildExecutor,
     GrayscaleImage,
-    get_data_loader,
     LocalFSLinkAuth,
     DefaultS3LinkAuth,
     COCOObjectAnnotation,
 )
 
 # TODO: add dataset build/push/list/info api
 
 
 __all__ = [
-    "get_data_loader",
     "Link",
     "LinkAuth",
     "DefaultS3LinkAuth",
     "LocalFSLinkAuth",
     "S3LinkAuth",
     "MIMEType",
     "LinkType",
-    "BuildExecutor",
     "Binary",
     "NumpyBinary",
     "Text",
     "Line",
     "Point",
     "Polygon",
     "Audio",
```

### Comparing `starwhale-0.4.1/starwhale/base/blob/file.py` & `starwhale-0.4.2/starwhale/base/blob/file.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/base/blob/store.py` & `starwhale-0.4.2/starwhale/base/blob/store.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/base/bundle.py` & `starwhale-0.4.2/starwhale/base/bundle.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         return True
 
     @abstractclassmethod
     def _get_cls(cls, uri: URI) -> t.Any:
         raise NotImplementedError
 
     @classmethod
-    def copy(cls, src_uri: str, dest_uri: str, force: bool = False) -> None:
+    def copy(cls, src_uri: str, dest_uri: str) -> None:
         raise NotImplementedError
 
     def extract(self, force: bool = False, target: t.Union[str, Path] = "") -> Path:
         raise NotImplementedError
 
     def build(self, *args: t.Any, **kwargs: t.Any) -> None:
         self.store.building = True  # type: ignore
```

### Comparing `starwhale-0.4.1/starwhale/base/bundle_copy.py` & `starwhale-0.4.2/starwhale/base/bundle_copy.py`

 * *Files 6% similar despite different names*

```diff
@@ -126,43 +126,46 @@
             path=self._get_remote_bundle_api_url(for_head=True),
             method=HTTPMethod.HEAD,
             instance_uri=instance_uri,
             ignore_status_codes=[HTTPStatus.NOT_FOUND],
         )
         return ok
 
-    def _get_target_path(self, uri: URI) -> Path:
+    def _get_versioned_resource_path(self, uri: URI) -> Path:
         if uri.instance_type != InstanceType.STANDALONE:
             raise NoSupportError(f"{uri} to get target dir path")
 
         resource_name = uri.object.name or self.bundle_name
         return (
             self._sw_config.rootdir
             / uri.project
             / self.typ
             / resource_name
             / self.bundle_version[:VERSION_PREFIX_CNT]
             / f"{self.bundle_version}{get_bundle_type_by_uri(self.typ)}"
         )
 
-    def _is_existed(self, uri: URI) -> bool:
+    def _check_version_existed(self, uri: URI) -> bool:
         if uri.instance_type == InstanceType.CLOUD:
             return self._check_cloud_obj_existed(uri)
         else:
-            return self._get_target_path(uri).exists()
+            return self._get_versioned_resource_path(uri).exists()
 
-    def _get_remote_bundle_console_url(self) -> str:
-        version = self.src_uri.object.version
+    def _get_remote_bundle_console_url(self, with_version: bool = True) -> str:
         if self.src_uri.instance_type == InstanceType.CLOUD:
             remote = self.src_uri
             resource_name = self.src_uri.object.name
         else:
             remote = self.dest_uri
             resource_name = self.dest_uri.object.name or self.src_uri.object.name
-        return f"{remote.instance}/projects/{remote.project}/{self.typ}s/{resource_name}/versions/{version}/overview"
+
+        url = f"{remote.instance}/projects/{remote.project}/{self.typ}s/{resource_name}"
+        if with_version:
+            url = f"{url}/versions/{self.src_uri.object.version}/overview"
+        return url
 
     def _get_remote_bundle_api_url(self, for_head: bool = False) -> str:
         version = self.src_uri.object.version
         if not version:
             raise FieldTypeOrValueError(
                 f"cannot fetch version from src uri:{self.src_uri}"
             )
@@ -183,15 +186,15 @@
         if not for_head:
             # uri for head request contains no 'file'
             base.append("file")
 
         return "/".join(base)
 
     def _do_upload_bundle_tar(self, progress: Progress) -> None:
-        file_path = self._get_target_path(self.src_uri)
+        file_path = self._get_versioned_resource_path(self.src_uri)
         task_id = progress.add_task(
             f":bowling: upload {file_path.name}",
             total=file_path.stat().st_size,
         )
 
         self.do_multipart_upload_file(
             url_path=self._get_remote_bundle_api_url(),
@@ -204,15 +207,15 @@
             },
             use_raise=True,
             progress=progress,
             task_id=task_id,
         )
 
     def _do_download_bundle_tar(self, progress: Progress) -> None:
-        file_path = self._get_target_path(self.dest_uri)
+        file_path = self._get_versioned_resource_path(self.dest_uri)
         ensure_dir(os.path.dirname(file_path))
         task_id = progress.add_task(f":bowling: download to {file_path}...")
 
         self.do_download_file(
             url_path=self._get_remote_bundle_api_url(),
             dest_path=file_path,
             instance_uri=self.src_uri,
@@ -222,68 +225,75 @@
             },
             progress=progress,
             task_id=task_id,
         )
 
     def do(self) -> None:
         remote_url = self._get_remote_bundle_console_url()
-        if self._is_existed(self.dest_uri) and not self.force:
+        if self._check_version_existed(self.dest_uri) and not self.force:
             console.print(f":tea: {remote_url} was already existed, skip copy")
             return
 
-        if not self._is_existed(self.src_uri):
+        if not self._check_version_existed(self.src_uri):
             raise NotFoundError(str(self.src_uri))
 
-        console.print(
-            f":construction: start to copy {self.src_uri} -> {self.dest_uri}..."
-        )
+        console.print(f":construction: start to copy {self.src_uri} -> {self.dest_uri}")
 
         with Progress(
             SpinnerColumn(),
             TextColumn("[progress.description]{task.description}"),
             BarColumn(),
             TextColumn("[progress.percentage]{task.percentage:>3.0f}%"),
             TimeElapsedColumn(),
             TotalFileSizeColumn(),
             TransferSpeedColumn(),
             console=console,
             refresh_per_second=0.2,
         ) as progress:
             if self.src_uri.instance_type == InstanceType.STANDALONE:
-                if self.typ == URIType.DATASET or self.typ == URIType.MODEL:
+                if self.typ == URIType.MODEL:
                     self._do_upload_bundle_dir(progress)
-                else:
+                elif self.typ == URIType.RUNTIME:
                     self._do_upload_bundle_tar(progress)
+                else:
+                    raise NoSupportError(
+                        f"no support to copy {self.typ} from standalone to server"
+                    )
             else:
-                if self.typ == URIType.DATASET or self.typ == URIType.MODEL:
+                if self.typ == URIType.MODEL:
                     self._do_download_bundle_dir(progress)
-                else:
+                elif self.typ == URIType.RUNTIME:
                     self._do_download_bundle_tar(progress)
+                else:
+                    raise NoSupportError(
+                        f"no support to copy {self.typ} from server to standalone"
+                    )
 
                 _dest_uri = URI.capsulate_uri(
                     instance=STANDALONE_INSTANCE,
                     project=self.dest_uri.project,
                     obj_type=self.typ,
                     obj_name=self.dest_uri.object.name or self.bundle_name,
                     obj_ver=self.bundle_version,
                 )
                 StandaloneTag(_dest_uri).add_fast_tag()
                 self._update_manifest(
-                    self._get_target_path(_dest_uri), {CREATED_AT_KEY: now_str()}
+                    self._get_versioned_resource_path(_dest_uri),
+                    {CREATED_AT_KEY: now_str()},
                 )
         console.print(f":tea: console url of the remote bundle: {remote_url}")
 
     def upload_files(self, workdir: Path) -> t.Iterator[FileNode]:
         raise NotImplementedError
 
     def download_files(self, workdir: Path) -> t.Iterator[FileNode]:
         raise NotImplementedError
 
     def _do_download_bundle_dir(self, progress: Progress) -> None:
-        _workdir = self._get_target_path(self.dest_uri)
+        _workdir = self._get_versioned_resource_path(self.dest_uri)
 
         def _download(_tid: TaskID, fd: FileNode) -> None:
             if fd.signature:
                 f = self._object_store.get(fd.signature)
                 if f is not None and f.exists():
                     f.link(_workdir / fd.path / fd.name)
                     progress.update(_tid, completed=fd.size)
@@ -413,17 +423,14 @@
             futures = [
                 executor.submit(_upload_blob, _tid, _file_desc)
                 for _tid, _file_desc in _p_map.items()
             ]
             # TODO throw errors
             wait(futures)
 
-    def _do_ubd_datastore(self) -> None:
-        raise NotImplementedError
-
     def _do_ubd_end(self, upload_id: str, url_path: str, ok: bool) -> None:
         phase = _UploadPhase.END if ok else _UploadPhase.CANCEL
         self.do_http_request(
             path=url_path,
             method=HTTPMethod.POST,
             instance_uri=self.dest_uri,
             data={
@@ -437,28 +444,27 @@
         )
 
     def _do_upload_bundle_dir(
         self,
         progress: t.Optional[Progress] = None,
         workdir: t.Optional[Path] = None,
     ) -> None:
-        workdir = workdir or self._get_target_path(self.src_uri)
+        workdir = workdir or self._get_versioned_resource_path(self.src_uri)
         url_path = self._get_remote_bundle_api_url()
 
         res_data = self._do_ubd_bundle_prepare(
             progress=progress,
             workdir=workdir,
             url_path=url_path,
         )
         upload_id: str = res_data.get("uploadId", "")
         if not upload_id:
             raise Exception("upload id is empty")
         exists_files: list = res_data.get("existed", [])
         try:
-            self._do_ubd_datastore()
             self._do_ubd_blobs(
                 progress=progress,
                 workdir=workdir,
                 upload_id=upload_id,
                 url_path=url_path,
                 existed_files=exists_files,
             )
```

### Comparing `starwhale-0.4.1/starwhale/base/cloud.py` & `starwhale-0.4.2/starwhale/base/cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,15 +176,15 @@
         _manifest: t.Dict[str, t.Any] = {
             "uri": uri.full_uri,
             "project": uri.project,
             "name": uri.object.name,
         }
 
         if uri.object.version:
-            # TODO: add manifest info by controller api
+            # TODO: add manifest, lock(runtime), model/dataset/runtime yaml info by controller api
             _manifest["version"] = uri.object.version
             _info = self._fetch_bundle_version_info(uri, typ)
             _manifest[CREATED_AT_KEY] = self.fmt_timestamp(_info["createdTime"])
             _manifest["size"] = _info["files"][0]["size"]
         else:
             _manifest["history"] = self._fetch_bundle_history(
                 name=uri.object.name,
@@ -279,15 +279,17 @@
             return default_size
 
         meta = yaml.safe_load(meta_str)
         if not isinstance(meta, dict):
             return default_size
 
         if typ == "dataset":
-            return int(meta.get("dataset_byte_size", default_size))
+            return int(
+                meta.get("dataset_summary", {}).get("blobs_byte_size", default_size)
+            )
         if typ == "runtime":
             # no size info in meta for now
             return default_size
 
         return default_size
```

### Comparing `starwhale-0.4.1/starwhale/base/mixin.py` & `starwhale-0.4.2/starwhale/base/mixin.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/base/store.py` & `starwhale-0.4.2/starwhale/base/store.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/base/tag.py` & `starwhale-0.4.2/starwhale/base/tag.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/base/type.py` & `starwhale-0.4.2/starwhale/base/type.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,34 +72,14 @@
     elif uri_type == URIType.RUNTIME:
         return BundleType.RUNTIME
     else:
         raise NoSupportError(uri_type)
 
 
 @unique
-class DataFormatType(Enum):
-    SWDS_BIN = "swds_bin"
-    USER_RAW = "user_raw"
-    UNDEFINED = "undefined"
-
-
-@unique
-class ObjectStoreType(Enum):
-    LOCAL = "local"
-    REMOTE = "remote"
-    UNDEFINED = "undefined"
-
-
-@unique
-class DataOriginType(Enum):
-    NEW = "+"
-    INHERIT = "~"
-
-
-@unique
 class DependencyType(Enum):
     PIP_PKG = "pip_pkg"
     PIP_REQ_FILE = "pip_req_file"
     CONDA_PKG = "conda_pkg"
     CONDA_ENV_FILE = "conda_env_file"
     WHEEL = "wheel"
     NATIVE_FILE = "native_file"
```

### Comparing `starwhale-0.4.1/starwhale/base/uri.py` & `starwhale-0.4.2/starwhale/base/uri.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/base/uricomponents/instance.py` & `starwhale-0.4.2/starwhale/base/uricomponents/instance.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/base/uricomponents/project.py` & `starwhale-0.4.2/starwhale/base/uricomponents/project.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/base/uricomponents/resource.py` & `starwhale-0.4.2/starwhale/base/uricomponents/resource.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/base/view.py` & `starwhale-0.4.2/starwhale/base/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,28 +128,30 @@
             icon = ":clap:"
         elif status in ("fail", "failed"):
             style = "red"
             icon = ":fearful:"
         return status, style, icon
 
     @staticmethod
-    def prepare_build_bundle(project: str, bundle_name: str, typ: str) -> URI:
+    def prepare_build_bundle(
+        project: str, bundle_name: str, typ: str, auto_gen_version: bool = True
+    ) -> URI:
         console.print(f":construction: start to build {typ} bundle...")
         _project_uri = URI(project, expected_type=URIType.PROJECT)
         if not bundle_name:
             raise FieldTypeOrValueError("no bundle_name")
 
         _uri = URI.capsulate_uri(
             instance=_project_uri.instance,
             project=_project_uri.project,
             obj_type=typ,
             obj_name=bundle_name,
-            obj_ver=gen_uniq_version(),
+            obj_ver=gen_uniq_version() if auto_gen_version else "",
         )
-        console.print(f":construction_worker: uri:{_uri}")
+        console.print(f":construction_worker: uri {_uri}")
         return _uri
 
     @staticmethod
     def _print_history(
         title: str,
         history: t.List[t.Dict[str, t.Any]],
         fullname: bool = False,
```

### Comparing `starwhale-0.4.1/starwhale/cli/__init__.py` & `starwhale-0.4.2/starwhale/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/cli/assistance/broker.py` & `starwhale-0.4.2/starwhale/cli/assistance/broker.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/cli/assistance/cli.py` & `starwhale-0.4.2/starwhale/cli/assistance/cli.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/cli/assistance/common.py` & `starwhale-0.4.2/starwhale/cli/assistance/common.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/cli/assistance/host.py` & `starwhale-0.4.2/starwhale/cli/assistance/host.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/cli/assistance/remote.py` & `starwhale-0.4.2/starwhale/cli/assistance/remote.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/cli/board/board.py` & `starwhale-0.4.2/starwhale/cli/board/board.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/cli/board/project_tree.py` & `starwhale-0.4.2/starwhale/cli/board/project_tree.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/cli/board/widgets.py` & `starwhale-0.4.2/starwhale/cli/board/widgets.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/cli/completion.py` & `starwhale-0.4.2/starwhale/cli/completion.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/cli/mngt.py` & `starwhale-0.4.2/starwhale/cli/mngt.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/consts/__init__.py` & `starwhale-0.4.2/starwhale/consts/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,18 +13,26 @@
 ENV_SW_IMAGE_REPO = "SW_IMAGE_REPO"
 # SW_LOCAL_STORAGE env used for generating default swcli config
 # and overriding 'storage.root' swcli config in runtime
 ENV_SW_LOCAL_STORAGE = "SW_LOCAL_STORAGE"
 
 DEFAULT_STARWHALE_API_VERSION = "1.0"
 DEFAULT_MANIFEST_NAME = "_manifest.yaml"
-DEFAULT_EVALUATION_JOB_NAME = "default"
-DEFAULT_EVALUATION_JOBS_FNAME = "eval_jobs.yaml"
-DEFAULT_EVALUATION_SVC_META_FNAME = "svc.json"
-DEFAULT_EVALUATION_PIPELINE = "starwhale.core.model.default_handler"
+
+# evaluation related constants
+DEFAULT_JOB_NAME = "default"
+DEFAULT_EVALUATION_JOB_NAME = "evaluation"
+DEFAULT_FINETUNE_JOB_NAME = "fine_tune"
+DEFAULT_JOBS_FILE_NAME = "jobs.yaml"
+EVALUATION_SVC_META_FILE_NAME = "svc.json"
+# auto generated evaluation panel layout file name from yaml or local console
+EVALUATION_PANEL_LAYOUT_JSON_FILE_NAME = "eval_panel_layout.json"
+# user defined evaluation panel layout file name
+EVALUATION_PANEL_LAYOUT_YAML_FILE_NAME = "eval_panel_layout.yaml"
+
 DEFAULT_LOCAL_SW_CONTROLLER_ADDR = "localhost:7827"
 LOCAL_CONFIG_VERSION = "2.0"
 DEFAULT_FILE_SIZE_THRESHOLD_TO_TAR_IN_MODEL = 10 * 1024  # 10KB
 
 SW_AUTO_DIRNAME = ".starwhale"
 SW_EVALUATION_EXAMPLE_DIR = "examples"
 
@@ -97,19 +105,14 @@
 class SWDSBackendType:
     S3 = "s3"
     LocalFS = "local_fs"
     SignedUrl = "signed_url"
     Http = "http"
 
 
-class EvalHandlerType:
-    DEFAULT = "default"
-    CUSTOM = "custom"
-
-
 class DataLoaderKind:
     SWDS = "swds"
     JSONL = "jsonl"
     RAW = "raw"
 
 
 class EvaluationResultKind:
@@ -127,21 +130,36 @@
     MANIFEST = "MANIFEST"
     SRC = "SRC"
     SRC_TAR = "SRC_TAR"
     MODEL = "MODEL"
     DATA = "DATA"
 
 
+class RunStatus:
+    INIT = "init"
+    START = "start"
+    RUNNING = "running"
+    SUCCESS = "success"
+    FAILED = "failed"
+
+
 class FileFlag:
     UNCHANGED = "unchanged"
     ADDED = "added"
     UPDATED = "updated"
     DELETED = "deleted"
 
 
+class DecoratorInjectAttr:
+    Step = "_starwhale_inject_step_decorator"
+    Predict = "_starwhale_inject_predict_decorator"
+    Evaluate = "_starwhale_inject_evaluate_decorator"
+    FineTune = "_starwhale_inject_finetune_decorator"
+
+
 @dataclass
 class FileNode:
     path: pathlib.Path
     name: str
     size: int
     file_desc: FileDesc
     signature: str = ""
```

### Comparing `starwhale-0.4.1/starwhale/core/dataset/cli.py` & `starwhale-0.4.2/starwhale/core/dataset/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from starwhale.consts import DefaultYAMLName, DEFAULT_PAGE_IDX, DEFAULT_PAGE_SIZE
 from starwhale.base.uri import URI
 from starwhale.base.type import URIType
 from starwhale.utils.cli import AliasedGroup
 from starwhale.utils.load import import_object
 from starwhale.utils.error import NotFoundError
-from starwhale.core.dataset.type import MIMEType, DatasetAttr, DatasetConfig
+from starwhale.core.dataset.type import DatasetAttr, DatasetConfig
 
 from .view import get_term_view, DatasetTermView
 
 
 @click.group(
     "dataset",
     cls=AliasedGroup,
@@ -29,53 +29,49 @@
 @click.argument("workdir", type=click.Path(exists=True, file_okay=False))
 @click.option(
     "-h",
     "--handler",
     help="Dataset build executor handler: [module path]:[class or function name]",
 )
 @click.option("-n", "--name", help="Dataset name")
-@click.option("-p", "--project", help="Project URI")
+@click.option(
+    "-p",
+    "--project",
+    help="Project URI, the default is the current selected project. The dataset will store in the specified project",
+)
 @click.option("--desc", help="Dataset description")
 @click.option(
     "-as",
     "--alignment-size",
     help="swds-bin format dataset: alignment size",
 )
 @click.option(
     "-vs",
     "--volume-size",
     help="swds-bin format dataset: volume size",
 )
-@click.option("-dmt", "--data-mime-type", help="Dataset global default data mime type")
 @click.option(
     "-f",
     "--dataset-yaml",
     default=DefaultYAMLName.DATASET,
     help="Dataset yaml filename, default use ${WORKDIR}/dataset.yaml file",
 )
-@click.option("-a", "--append", is_flag=True, default=None, help="Only append new data")
-@click.option("-af", "--append-from", help="Append from dataset version")
 @click.option("-r", "--runtime", help="runtime uri")
-@click.option("-dcs", "--disable-copy-src", help="disable copy src dir")
 @click.pass_obj
 def _build(
     view: DatasetTermView,
     workdir: str,
     handler: str,
     name: str,
     project: str,
     desc: str,
     dataset_yaml: str,
     alignment_size: str,
     volume_size: str,
-    data_mime_type: str,
-    append: bool,
-    append_from: str,
     runtime: str,
-    disable_copy_src: bool,
 ) -> None:
     # TODO: add dry-run
     # TODO: add compress args
     if not os.path.exists(workdir):
         raise NotFoundError(workdir)
 
     yaml_path = Path(workdir) / dataset_yaml
@@ -86,27 +82,22 @@
     config.name = name or config.name or Path(workdir).absolute().name
     handler = handler or config.handler
     config.handler = import_object(workdir, handler)
     config.runtime_uri = runtime or config.runtime_uri
     config.project_uri = project or config.project_uri
     # TODO: support README.md as the default desc
     config.desc = desc or config.desc
-    config.append_from = append_from or config.append_from
 
     config.attr = DatasetAttr(
         volume_size=volume_size or config.attr.volume_size,
         alignment_size=alignment_size or config.attr.alignment_size,
-        data_mime_type=MIMEType(data_mime_type or config.attr.data_mime_type),
     )
 
-    if append is not None:
-        config.append = append
-
     config.do_validate()
-    view.build(workdir, config, disable_copy_src)
+    view.build(workdir, config)
 
 
 @dataset_cmd.command("diff", help="Dataset version diff")
 @click.argument("base_uri", required=True)
 @click.argument("compare_uri", required=True)
 @click.option(
     "--show-details", is_flag=True, help="Show data different detail by the row"
@@ -115,15 +106,20 @@
 def _diff(
     view: t.Type[DatasetTermView], base_uri: str, compare_uri: str, show_details: bool
 ) -> None:
     view(base_uri).diff(URI(compare_uri, expected_type=URIType.DATASET), show_details)
 
 
 @dataset_cmd.command("list", aliases=["ls"])
-@click.option("-p", "--project", default="", help="Project URI")
+@click.option(
+    "-p",
+    "--project",
+    default="",
+    help="Project URI, the default is the current selected project.",
+)
 @click.option("-f", "--fullname", is_flag=True, help="Show fullname of dataset version")
 @click.option("-sr", "--show-removed", is_flag=True, help="Show removed datasets")
 @click.option(
     "--page", type=int, default=DEFAULT_PAGE_IDX, help="Page number for dataset list"
 )
 @click.option(
     "--size", type=int, default=DEFAULT_PAGE_SIZE, help="Page size for dataset list"
@@ -142,15 +138,15 @@
     fullname: bool,
     show_removed: bool,
     page: int,
     size: int,
     filters: list,
 ) -> None:
     """
-    List Dataset
+    List Dataset of the specified project.
 
     The filtering flag (-fl or --filter) format is a key=value pair or a flag.
     If there is more than one filter, then pass multiple flags.\n
     (e.g. --filter name=mnist --filter latest)
 
     \b
     The currently supported filters are:
@@ -220,17 +216,16 @@
 def _summary(view: t.Type[DatasetTermView], dataset: str) -> None:
     view(dataset).summary()
 
 
 @dataset_cmd.command("copy", aliases=["cp"])
 @click.argument("src")
 @click.argument("dest")
-@click.option("-f", "--force", is_flag=True, help="Force copy dataset")
 @click.option("-dlp", "--dest-local-project", help="dest local project uri")
-def _copy(src: str, dest: str, force: bool, dest_local_project: str) -> None:
+def _copy(src: str, dest: str, dest_local_project: str) -> None:
     """
     Copy Dataset between Standalone Instance and Cloud Instance
 
     SRC: dataset uri with version
 
     DEST: project uri or dataset uri with name.
 
@@ -268,15 +263,15 @@
         - copy standalone instance(local) default project(self)'s mnist-local dataset to cloud instance(pre-k8s) mnist project without 'cloud://' prefix
             swcli dataset cp mnist-local/version/latest pre-k8s/project/mnist
 
         \b
         - copy standalone instance(local) project(myproject)'s mnist-local dataset to cloud instance(pre-k8s) mnist project with standalone instance dataset name 'mnist-local'
             swcli dataset cp local/project/myproject/dataset/mnist-local/version/latest cloud://pre-k8s/project/mnist
     """
-    DatasetTermView.copy(src, dest, force, dest_local_project)
+    DatasetTermView.copy(src, dest, dest_local_project)
 
 
 @dataset_cmd.command("tag", help="Dataset tag management, add or remove")
 @click.argument("dataset")
 @click.argument("tags", nargs=-1)
 @click.option("-r", "--remove", is_flag=True, help="Remove tags")
 @click.option(
@@ -292,15 +287,15 @@
     tags: t.List[str],
     remove: bool,
     quiet: bool,
 ) -> None:
     view(dataset).tag(tags, remove, quiet)
 
 
-@dataset_cmd.command("head", help="Print the first 10 rows of the dataset")
+@dataset_cmd.command("head", help="Print the first 5 rows of the dataset")
 @click.argument("dataset")
 @click.option("-n", "--rows", default=5, help="Print the first NUM rows of the dataset")
 @click.option(
     "-d",
     "--show-raw-data",
     is_flag=True,
     help="Fetch raw data content",
```

### Comparing `starwhale-0.4.1/starwhale/core/dataset/store.py` & `starwhale-0.4.2/starwhale/core/dataset/store.py`

 * *Files 5% similar despite different names*

```diff
@@ -433,15 +433,15 @@
     def __str__(self) -> str:
         return f"StorageBackend for {self.kind}"
 
     __repr__ = __str__
 
     @abstractmethod
     def _make_file(
-        self, bucket: str, key_compose: t.Tuple[Link, int, int]
+        self, key_compose: t.Tuple[Link, int, int], **kw: t.Any
     ) -> FileLikeObj:
         raise NotImplementedError
 
 
 class S3StorageBackend(StorageBackend):
     lock_s3_creation = threading.Lock()
 
@@ -466,68 +466,73 @@
                         "mode": "standard",
                     },
                 ),
                 region_name=conn.region,
             )
 
     def _make_file(
-        self, bucket: str, key_compose: t.Tuple[Link, int, int]
+        self, key_compose: t.Tuple[Link, int, int], **kw: t.Any
     ) -> FileLikeObj:
         # TODO: merge connections for s3
         _key, _start, _end = key_compose
         return S3BufferedFileLike(
             s3=self.s3,
-            bucket=bucket,
+            bucket=kw["bucket"],
             key=_key.uri,
             start=_start,
             end=_end,
         )
 
 
 class LocalFSStorageBackend(StorageBackend):
     def __init__(self) -> None:
         super().__init__(kind=SWDSBackendType.LocalFS)
 
     def _make_file(
-        self, bucket: str, key_compose: t.Tuple[Link, int, int]
+        self, key_compose: t.Tuple[Link, int, int], **kw: t.Any
     ) -> FileLikeObj:
         _key_l, _start, _end = key_compose
         _key = _key_l.uri
-        bucket_path = (
-            Path(bucket).expanduser() if bucket.startswith("~/") else Path(bucket)
-        )
         # TODO: tune reopen file performance, merge files
-        data_path = bucket_path / _key[: DatasetStorage.short_sign_cnt]
+        data_path = DatasetStorage._get_object_store_path(_key)
+        # TODO: remove dataset data_dir
         if not data_path.exists():
-            data_path = bucket_path / _key
+            bucket = kw["bucket"]
+            bucket_path = (
+                Path(bucket).expanduser() if bucket.startswith("~/") else Path(bucket)
+            )
+            data_path = bucket_path / _key[: DatasetStorage.short_sign_cnt]
+            if not data_path.exists():
+                data_path = bucket_path / _key
 
+        _end = min(_end, data_path.stat().st_size)
         with data_path.open("rb") as f:
             f.seek(_start)
-            return io.BytesIO(f.read(_end - _start + 1))
+            return io.BytesIO(f.read(_end - _start + 1))  # type: ignore
 
 
 class SignedUrlBackend(StorageBackend, CloudRequestMixed):
     def __init__(self, dataset_uri: URI) -> None:
         super().__init__(kind=SWDSBackendType.SignedUrl)
         self.dataset_uri = dataset_uri
 
     @http_retry
     def _make_file(
-        self, key_compose: t.Tuple[Link, int, int], **kwargs: t.Any
+        self, key_compose: t.Tuple[Link, int, int], **kw: t.Any
     ) -> FileLikeObj:
         _key, _start, _end = key_compose
         return HttpBufferedFileLike(
             url=_key.signed_uri or self.sign_uri(_key.uri),
             headers={"Range": f"bytes={_start or 0}-{_end or sys.maxsize}"},
             timeout=90,
         )
 
     def sign_uri(self, uri: str) -> str:
         r = self.do_http_request(
-            f"/project/{self.dataset_uri.project}/{self.dataset_uri.object.typ}/{self.dataset_uri.object.name}/version/{self.dataset_uri.object.version}/sign-links",
+            f"/project/{self.dataset_uri.project}/{self.dataset_uri.object.typ}/{self.dataset_uri.object.name}/uri/sign-links",
             method=HTTPMethod.POST,
             instance_uri=self.dataset_uri,
             params={
                 "expTimeMillis": int(
                     os.environ.get("SW_MODEL_PROCESS_UNIT_TIME_MILLIS", "60000")
                 ),
             },
@@ -539,15 +544,15 @@
 
 class HttpBackend(StorageBackend, CloudRequestMixed):
     def __init__(self) -> None:
         super().__init__(kind=SWDSBackendType.Http)
 
     @http_retry
     def _make_file(
-        self, key_compose: t.Tuple[Link, int, int], **kwargs: t.Any
+        self, key_compose: t.Tuple[Link, int, int], **kw: t.Any
     ) -> FileLikeObj:
         _key, _start, _end = key_compose
         return HttpBufferedFileLike(
             url=_key.uri,
             headers={"Range": f"bytes={_start or 0}-{_end or sys.maxsize}"},
             timeout=90,
         )
```

### Comparing `starwhale-0.4.1/starwhale/core/dataset/type.py` & `starwhale-0.4.2/starwhale/core/dataset/type.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,39 +10,28 @@
 from pathlib import Path
 from functools import partial
 from urllib.parse import urlparse
 
 import numpy
 
 from starwhale.utils import load_yaml, convert_to_bytes, validate_obj_name
-from starwhale.consts import (
-    LATEST_TAG,
-    SHORT_VERSION_CNT,
-    VERSION_PREFIX_CNT,
-    DEFAULT_STARWHALE_API_VERSION,
-)
+from starwhale.consts import SHORT_VERSION_CNT, DEFAULT_STARWHALE_API_VERSION
 from starwhale.base.uri import URI
-from starwhale.utils.fs import (
-    ensure_dir,
-    ensure_file,
-    FilePosition,
-    blake2b_content,
-    BLAKE2B_SIGNATURE_ALGO,
-)
+from starwhale.utils.fs import FilePosition
 from starwhale.base.mixin import ASDictMixin
 from starwhale.utils.error import (
     NoSupportError,
     FieldTypeOrValueError,
     MissingDependencyError,
 )
 from starwhale.utils.retry import http_retry
 from starwhale.api._impl.data_store import SwObject, _TYPE_DICT
 
 D_FILE_VOLUME_SIZE = 64 * 1024 * 1024  # 64MB
-D_ALIGNMENT_SIZE = 4 * 1024  # 4k for page cache
+D_ALIGNMENT_SIZE = 128  # for page cache
 
 
 @unique
 class LinkType(Enum):
     LocalFS = "local_fs"
     S3 = "s3"
     UNDEFINED = "undefined"
@@ -247,15 +236,15 @@
         return MIMEType(self._mime_type)
 
     def to_bytes(self, encoding: str = "utf-8") -> bytes:
         return self.fetch_data(encoding)
 
     def clear_bytes(self) -> None:
         self.clear_cache()
-        if isinstance(self.fp, (bytes, io.IOBase)):
+        if isinstance(self.fp, (bytes, io.IOBase, str)):
             self.fp = ""
 
     def clear_cache(self) -> None:
         self.__cache_bytes = bytes()
 
     def fetch_data(self, encoding: str = "utf-8") -> bytes:
         if self.__cache_bytes:
@@ -824,22 +813,21 @@
 class Link(ASDictMixin, SwObject):
     def __init__(
         self,
         uri: t.Union[str, Path] = "",
         offset: int = FilePosition.START.value,
         size: int = -1,
         data_type: t.Optional[t.Union[BaseArtifact, t.Dict]] = None,
-        with_local_fs_data: bool = False,
         use_plain_type: bool = False,
         owner: t.Optional[t.Union[str, URI]] = None,
         **kwargs: t.Any,
     ) -> None:
         self._type = "link"
         self.owner = owner.raw if (owner and isinstance(owner, URI)) else owner
-        self.uri = (str(uri)).strip()
+        self.uri = str(uri).strip()
         _up = urlparse(self.uri)
         self.scheme = _up.scheme
         if offset < 0:
             raise FieldTypeOrValueError(f"offset({offset}) must be non-negative")
 
         self.offset = offset
         self.size = size
@@ -852,29 +840,19 @@
         if isinstance(data_type, BaseArtifact):
             data_type = data_type.drop_data()
             if use_plain_type:
                 data_type = data_type.astype()
 
         self.data_type = data_type
 
-        self.with_local_fs_data = with_local_fs_data
-        self._local_fs_uri = ""
         self._signed_uri = ""
 
         self.extra_info = kwargs
 
     @property
-    def local_fs_uri(self) -> str:
-        return self._local_fs_uri
-
-    @local_fs_uri.setter
-    def local_fs_uri(self, value: str) -> None:
-        self._local_fs_uri = value
-
-    @property
     def signed_uri(self) -> str:
         return self._signed_uri
 
     @signed_uri.setter
     def signed_uri(self, value: str) -> None:
         self._signed_uri = value
 
@@ -891,95 +869,69 @@
             "data_type": data_type,
         }
 
     def __str__(self) -> str:
         return f"Link {self.uri}"
 
     def __repr__(self) -> str:
-        return f"Link uri:{self.uri}, offset:{self.offset}, size:{self.size}, with localFS data:{self.with_local_fs_data}"
+        return f"Link uri:{self.uri}, offset:{self.offset}, size:{self.size}"
 
     @http_retry
     def to_bytes(self) -> bytes:
         # TODO: cache store
         from .store import ObjectStore
 
         key_compose = (
-            Link(self.local_fs_uri) if self.local_fs_uri else self,
+            self,
             self.offset or 0,
-            self.size + self.offset - 1 if self.size else sys.maxsize,
+            self.size + self.offset - 1 if self.size != -1 else sys.maxsize,
         )
         store = ObjectStore.get_store(self, self.owner)
         with store.backend._make_file(
             key_compose=key_compose, bucket=store.bucket
         ) as f:
             return f.read(self.size)  # type: ignore
 
-    @classmethod
-    def from_local_artifact(
-        cls, data: t.Union[BaseArtifact, Link], store_dir: Path
-    ) -> Link:
-        if isinstance(data, Link):
-            return data
-
-        raw_content = data.to_bytes()
-        sign_name = blake2b_content(raw_content)
-        fpath = (
-            store_dir
-            / BLAKE2B_SIGNATURE_ALGO
-            / sign_name[:VERSION_PREFIX_CNT]
-            / sign_name
-        )
-        ensure_dir(fpath.parent)
-        ensure_file(fpath, raw_content)
-
-        return Link(
-            uri=fpath,
-            offset=0,
-            size=len(raw_content),
-            data_type=data,
-            with_local_fs_data=True,
-            use_plain_type=True,
-        )
-
 
 class DatasetSummary(ASDictMixin):
     def __init__(
         self,
         rows: int = 0,
-        increased_rows: int = 0,
-        data_byte_size: int = 0,
+        updated_rows: int = 0,
+        deleted_rows: int = 0,
+        blobs_byte_size: int = 0,
+        increased_blobs_byte_size: int = 0,
         **kw: t.Any,
     ) -> None:
         self.rows = rows
-        self.increased_rows = increased_rows
-        self.unchanged_rows = rows - increased_rows
-        self.data_byte_size = data_byte_size
+        self.updated_rows = updated_rows
+        self.deleted_rows = deleted_rows
+        self.blobs_byte_size = blobs_byte_size
+        self.increased_blobs_byte_size = increased_blobs_byte_size
 
     def __str__(self) -> str:
         return f"Dataset Summary: rows({self.rows})"
 
     def __repr__(self) -> str:
         return (
-            f"Dataset Summary: rows({self.rows}, increased: {self.increased_rows}), "
-            f"size(data:{self.data_byte_size})"
+            f"Dataset Summary: rows(total: {self.rows}, updated: {self.updated_rows}, deleted: {self.deleted_rows}), "
+            f"size(blobs:{self.blobs_byte_size})"
         )
 
 
 # TODO: use attr to tune code
 class DatasetAttr(ASDictMixin):
     def __init__(
         self,
         volume_size: t.Union[int, str] = D_FILE_VOLUME_SIZE,
         alignment_size: t.Union[int, str] = D_ALIGNMENT_SIZE,
-        data_mime_type: MIMEType = MIMEType.UNDEFINED,
         **kw: t.Any,
     ) -> None:
         self.volume_size = convert_to_bytes(volume_size)
         self.alignment_size = convert_to_bytes(alignment_size)
-        self.data_mime_type = data_mime_type
         self.kw = kw
 
     def asdict(self, ignore_keys: t.Optional[t.List[str]] = None) -> t.Dict:
         return super().asdict(ignore_keys=ignore_keys or ["kw"])
 
 
 # TODO: abstract base class from DatasetConfig and ModelConfig
@@ -992,29 +944,25 @@
         pkg_data: t.List[str] = [],
         exclude_pkg_data: t.List[str] = [],
         desc: str = "",
         version: str = DEFAULT_STARWHALE_API_VERSION,
         attr: t.Dict[str, t.Any] = {},
         project_uri: str = "",
         runtime_uri: str = "",
-        append: bool = False,
-        append_from: str = LATEST_TAG,
         **kw: t.Any,
     ) -> None:
         self.name = name
         self.handler = handler
         self.desc = desc
         self.version = version
         self.attr = DatasetAttr(**attr)
         self.pkg_data = pkg_data
         self.exclude_pkg_data = exclude_pkg_data
         self.project_uri = project_uri
         self.runtime_uri = runtime_uri
-        self.append = append
-        self.append_from = append_from
 
         self.kw = kw
 
     def do_validate(self) -> None:
         _ok, _reason = validate_obj_name(self.name)
         if not _ok:
             raise FieldTypeOrValueError(f"name field:({self.name}) error: {_reason}")
```

### Comparing `starwhale-0.4.1/starwhale/core/dataset/view.py` & `starwhale-0.4.2/starwhale/core/dataset/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,42 +154,41 @@
 
     @classmethod
     @BaseTermView._only_standalone
     def build(
         cls,
         workdir: str,
         config: DatasetConfig,
-        disable_copy_src: bool = False,
     ) -> URI:
         dataset_uri = cls.prepare_build_bundle(
-            project=config.project_uri, bundle_name=config.name, typ=URIType.DATASET
+            project=config.project_uri,
+            bundle_name=config.name,
+            typ=URIType.DATASET,
+            auto_gen_version=False,
         )
         ds = Dataset.get_dataset(dataset_uri)
 
-        kwargs = dict(
-            workdir=Path(workdir), config=config, disable_copy_src=disable_copy_src
-        )
+        kwargs = dict(workdir=Path(workdir), config=config)
 
         if config.runtime_uri:
             RuntimeProcess.from_runtime_uri(
                 uri=config.runtime_uri, target=ds.build, kwargs=kwargs
             ).run()
         else:
             ds.build(**kwargs)
-        return dataset_uri
+        return ds.uri
 
     @classmethod
     def copy(
         cls,
         src_uri: str,
         dest_uri: str,
-        force: bool = False,
         dest_local_project_uri: str = "",
     ) -> None:
-        Dataset.copy(src_uri, dest_uri, force, dest_local_project_uri)
+        Dataset.copy(src_uri, dest_uri, dest_local_project_uri)
         console.print(":clap: copy done")
 
     @BaseTermView._header
     def tag(
         self, tags: t.List[str], remove: bool = False, ignore_errors: bool = False
     ) -> None:
         if remove:
@@ -204,17 +203,17 @@
         from starwhale.api._impl.data_store import _get_type
 
         for row in self.dataset.head(rows, show_raw_data):
             console.rule(f"row [{row['index']}]", align="left")
             output = (
                 f":deciduous_tree: id: {row['index']} \n"
                 ":cyclone: data:\n"
-                f"\t :dim_button: type: {row['data']} \n"
+                f"\t :dim_button: type: {row['features']} \n"
             )
-            for _k, _v in row["data"].items():
+            for _k, _v in row["features"].items():
                 ds_type: t.Any
                 try:
                     ds_type = _get_type(_v)
                 except RuntimeError:
                     ds_type = type(_v)
                 output += (
                     f"\t :droplet: {_k}: value[{_v}], type[{ds_type} | {type(_v)}] \n"
```

### Comparing `starwhale-0.4.1/starwhale/core/eval/cli.py` & `starwhale-0.4.2/starwhale/core/eval/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,25 +13,30 @@
     DEFAULT_REPORT_COLS,
 )
 
 
 @click.group(
     "eval",
     cls=AliasedGroup,
-    help="Evaluation management, create/list/info/compare evaluation job",
+    help="Evaluation management, run/list/info/compare evaluation job",
 )
 @click.pass_context
 def eval_job_cmd(ctx: click.Context) -> None:
     ctx.obj = get_term_view(ctx.obj)
 
 
 @eval_job_cmd.command(
-    "list", aliases=["ls"], help="List all jobs in the current project"
+    "list", aliases=["ls"], help="List all jobs in the specified project"
+)
+@click.option(
+    "-p",
+    "--project",
+    default="",
+    help="Project URI, default is the current selected project.",
 )
-@click.option("-p", "--project", default="", help="Project URI")
 @click.option("--fullname", is_flag=True, help="Show fullname of swmp version")
 @click.option("--show-removed", is_flag=True, help="Show removed dataset")
 @click.option(
     "--page", type=int, default=DEFAULT_PAGE_IDX, help="Page number for job list"
 )
 @click.option(
     "--size", type=int, default=DEFAULT_PAGE_SIZE, help="Page size for job list"
@@ -46,30 +51,31 @@
     size: int,
 ) -> None:
     view.list(
         project, fullname=fullname, show_removed=show_removed, page=page, size=size
     )
 
 
+# make the internal options hidden in the `--help` output.
 @eval_job_cmd.command("run", help="Run job")
 @click.option(
     "-p",
     "--project",
     envvar=SWEnv.project,
     default="",
-    help=f"project name, env is {SWEnv.project}",
+    help=f"Project URI, env is {SWEnv.project}.The evaluation result will store in the specified project. Default is the current selected project.",
 )
 @click.option(
     "--version",
     envvar=SWEnv.eval_version,
     default=None,
     help=f"Evaluation job version, env is {SWEnv.eval_version}",
+    hidden=True,
 )
 @click.option("--model", required=True, help="model uri or model.yaml dir path")
-# TODO:support multi dataset
 @click.option(
     "datasets",
     "--dataset",
     required=True,
     envvar=SWEnv.dataset_uri,
     multiple=True,
     help=f"dataset uri, env is {SWEnv.dataset_uri}",
@@ -77,34 +83,43 @@
 @click.option("--runtime", default="", help="runtime uri")
 @click.option("--name", default="default", help="job name")
 @click.option("--desc", help="job description")
 @click.option(
     "--step-spec",
     default="",
     type=str,
-    help="[Cloud_ONLY] A file contains the specification for steps of the job",
+    help="[Cloud_ONLY]a file contains the specification for steps of the job",
+    hidden=True,
 )
 @click.option(
     "--resource-pool",
     default="default",
     type=str,
-    help="[Cloud_ONLY] The node group you would like to run your job on",
+    help="[Cloud_ONLY]the job runs in the specified resource pool",
 )
 @click.option(
     "--use-docker",
     is_flag=True,
     help="[ONLY Standalone]use docker to run evaluation job",
 )
-@click.option("--gencmd", is_flag=True, help="[ONLY Standalone]gen docker run command")
-@click.option("--step", default="", help="Evaluation run step")
-@click.option("--task-index", default=-1, help="Index of tasks in the current step")
+@click.option(
+    "--gencmd",
+    is_flag=True,
+    help="[ONLY Standalone]gen docker run command",
+    hidden=True,
+)
+@click.option("--step", default="", help="Evaluation run step", hidden=True)
+@click.option(
+    "--task-index", default=-1, help="Index of tasks in the current step", hidden=True
+)
 @click.option(
     "--override-task-num",
     default=0,
     help="Total num of tasks in the current step",
+    hidden=True,
 )
 def _run(
     project: str,
     version: str,
     model: str,
     datasets: list,
     runtime: str,
@@ -190,19 +205,25 @@
 )
 @click.option(
     "--max-report-cols",
     type=int,
     default=DEFAULT_REPORT_COLS,
     help="Max table column size for print",
 )
+@click.option("--web", is_flag=True, help="Open job info page in browser")
 @click.pass_obj
 def _info(
-    view: t.Type[JobTermView], job: str, page: int, size: int, max_report_cols: int
+    view: t.Type[JobTermView],
+    job: str,
+    page: int,
+    size: int,
+    max_report_cols: int,
+    web: bool,
 ) -> None:
-    view(job).info(page, size, max_report_cols)
+    view(job).info(page, size, max_report_cols, web)
 
 
 @eval_job_cmd.command("compare", aliases=["cmp"])
 @click.argument("base_job", nargs=1)
 @click.argument("job", nargs=-1)
 def _compare(base_job: str, job: t.List[str]) -> None:
     """
```

### Comparing `starwhale-0.4.1/starwhale/core/eval/executor.py` & `starwhale-0.4.2/starwhale/core/eval/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 from starwhale.utils.config import SWCliConfigMixed
 from starwhale.utils.process import check_call
 from starwhale.utils.progress import run_with_progress_bar
 from starwhale.core.eval.store import EvaluationStorage
 from starwhale.core.model.model import StandaloneModel
 from starwhale.core.runtime.model import StandaloneRuntime
 
-_CNTR_WORKDIR = "/opt/starwhale"
-
 
 class EvalExecutor:
     def __init__(
         self,
         model_uri: str,
         dataset_uris: t.List[str],
         runtime_uri: str,
```

### Comparing `starwhale-0.4.1/starwhale/core/eval/model.py` & `starwhale-0.4.2/starwhale/core/eval/model.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/core/eval/store.py` & `starwhale-0.4.2/starwhale/core/eval/store.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/core/eval/view.py` & `starwhale-0.4.2/starwhale/core/eval/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     DEFAULT_MANIFEST_NAME,
 )
 from starwhale.base.uri import URI
 from starwhale.base.type import URIType, InstanceType, JobOperationType
 from starwhale.base.view import BaseTermView
 from starwhale.core.eval.model import EvaluationJob
 from starwhale.api._impl.metric import MetricKind
+from starwhale.base.uricomponents.instance import Instance
 
 
 class JobTermView(BaseTermView):
     def __init__(self, job_uri: str) -> None:
         super().__init__()
         self.raw_uri = job_uri
         self.uri = URI(job_uri, expected_type=URIType.EVALUATION)
@@ -115,21 +116,49 @@
 
     @BaseTermView._header
     def info(
         self,
         page: int = DEFAULT_PAGE_IDX,
         size: int = DEFAULT_PAGE_SIZE,
         max_report_cols: int = DEFAULT_REPORT_COLS,
+        web: bool = False,
     ) -> None:
         _rt = self.job.info(page, size)
         if not _rt:
             console.print(":tea: not found info")
             return
 
-        if _rt.get("manifest"):
+        manifest = _rt.get("manifest", {})
+        if web:
+            from starwhale.web.server import Server
+
+            ver = manifest.get("id")
+
+            # if id is numeric, it's a remote eval
+            if ver and ver.isnumeric():
+                svr = Server.proxy(Instance())
+            else:
+                # local eval
+                if not manifest.get("version"):
+                    console.print(":tea: eval id not found")
+                    sys.exit(1)
+                ver = manifest.get("version")
+                svr = Server.default()
+
+            # TODO support changing host and port
+            host = "127.0.0.1"
+            port = 8000
+            url = f"http://{host}:{port}/projects/{self.uri.project}/evaluations/{ver}/results?token=local"
+            console.print(f":tea: open {url} in browser")
+            import uvicorn
+
+            uvicorn.run(svr, host=host, port=port, log_level="error")
+            return
+
+        if manifest:
             console.rule(
                 f"[green bold]Inspect {DEFAULT_MANIFEST_NAME} for eval:{self.uri}"
             )
             console.print(Pretty(_rt["manifest"], expand_all=True))
 
         if "location" in _rt:
             console.rule("Evaluation process dirs")
@@ -365,15 +394,15 @@
             _datasets = "--"
             if _m.get("datasets"):
                 _datasets = "\n".join([_s(d) for d in _m["datasets"]])
 
             _model = "--"
             if "model" in _m:
                 _model = _s(_m["model"])
-            else:
+            elif "modelName" in _m:
                 _model = f"{_m['modelName']}:{_s(_m['modelVersion'])}"
 
             _name = "--"
             if "id" in _m:
                 _name = _m["id"]
             else:
                 _name = _m["version"] if show_removed else _s(_m["version"])
@@ -416,14 +445,15 @@
         cls.pretty_json(_data)
 
     def info(
         self,
         page: int = DEFAULT_PAGE_IDX,
         size: int = DEFAULT_PAGE_SIZE,
         max_report_cols: int = DEFAULT_REPORT_COLS,
+        web: bool = False,
     ) -> None:
         _rt = self.job.info(page, size)
         if not _rt:
             console.print(":tea: not found info")
             return
         self.pretty_json(_rt)
```

### Comparing `starwhale-0.4.1/starwhale/core/instance/cli.py` & `starwhale-0.4.2/starwhale/core/instance/cli.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/core/instance/model.py` & `starwhale-0.4.2/starwhale/core/instance/model.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/core/instance/view.py` & `starwhale-0.4.2/starwhale/core/instance/view.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/core/job/dag.py` & `starwhale-0.4.2/starwhale/core/job/dag.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/core/job/scheduler.py` & `starwhale-0.4.2/starwhale/core/job/scheduler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,148 +1,137 @@
 import time
 import typing as t
 from pathlib import Path
+from concurrent.futures import as_completed, ThreadPoolExecutor
 
 from loguru import logger
 
+from starwhale.consts import RunStatus
 from starwhale.core.job.dag import DAG
-from starwhale.api._impl.job import Context
-from starwhale.core.job.model import (
-    Step,
-    STATUS,
-    Generator,
-    StepResult,
-    TaskResult,
-    StepExecutor,
-    TaskExecutor,
-    MultiThreadProcessor,
-)
+from starwhale.core.job.step import Step
+
+from .step import StepResult, StepExecutor
+from .task import TaskResult, TaskExecutor
+from .context import Context
 
 
 class Scheduler:
     def __init__(
         self,
         project: str,
         version: str,
-        module: str,
         workdir: Path,
         dataset_uris: t.List[str],
         steps: t.List[Step],
     ) -> None:
-        self._steps: t.Dict[str, Step] = {s.step_name: s for s in steps}
-        self.dag: DAG = Generator.generate_dag_from_steps(steps)
+        self._steps: t.Dict[str, Step] = {s.name: s for s in steps}
+        self.dag: DAG = Step.generate_dag(steps)
         self.project = project
         self.dataset_uris = dataset_uris
-        self.module = module
         self.workdir = workdir
         self.version = version
 
-    def schedule(self) -> t.List[StepResult]:
+    def run(
+        self, step_name: str = "", task_num: int = 0, task_index: t.Optional[int] = None
+    ) -> t.List[StepResult]:
+        if not step_name:
+            return self._schedule_all()
+
+        if task_index is None or task_index < 0:
+            return [self._schedule_one_step(step_name=step_name, task_num=task_num)]
+        else:
+            return [self._schedule_one_task(step_name=step_name, task_index=task_index)]
+
+    def _schedule_all(self) -> t.List[StepResult]:
         _results: t.List[StepResult] = []
         # record all vertex's in degree
         indegree_dict = {}
         for vtx in self.dag.vertices():
             indegree_dict[vtx] = self.dag.in_degree(vtx)
 
         vertices_running: t.Set[str] = set()
         prepared_vertices = self.dag.all_starts()
 
         while prepared_vertices:
             vertices_to_run = prepared_vertices - vertices_running
 
-            processor = MultiThreadProcessor(
-                "",
-                len(vertices_to_run),
-                list(
-                    StepExecutor(
-                        self._steps[v],
-                        project=self.project,
-                        dataset_uris=self.dataset_uris,
-                        module=self.module,
-                        workdir=self.workdir,
-                        version=self.version,
-                    )
-                    for v in vertices_to_run
-                ),
-            )
+            tasks = [
+                StepExecutor(
+                    self._steps[v],
+                    project=self.project,
+                    dataset_uris=self.dataset_uris,
+                    workdir=self.workdir,
+                    version=self.version,
+                )
+                for v in vertices_to_run
+            ]
+            with ThreadPoolExecutor(max_workers=len(vertices_to_run)) as pool:
+                future_tasks = [pool.submit(t.execute) for t in tasks]
+                step_results = [t.result() for t in as_completed(future_tasks)]
 
             vertices_running |= set(vertices_to_run)
-            # execute and get results
-            step_results: t.List[StepResult] = processor.execute()
             _results += step_results
-            vertices_finished = [result.step_name for result in step_results]
+            vertices_finished = [result.name for result in step_results]
             vertices_running -= set(vertices_finished)
             prepared_vertices -= set(vertices_finished)
 
             # update dag
             for result in step_results:
-                for v_to in self.dag.successors(result.step_name):
+                for v_to in self.dag.successors(result.name):
                     indegree_dict[v_to] -= 1
                     if indegree_dict[v_to] == 0:
                         prepared_vertices.add(v_to)
 
             if not all(
                 [
-                    all(tr.status == STATUS.SUCCESS for tr in sr.task_results)
+                    all(tr.status == RunStatus.SUCCESS for tr in sr.task_results)
                     for sr in step_results
                 ]
             ):
                 break
         return _results
 
-    def schedule_single_step(self, step_name: str, task_num: int = 0) -> StepResult:
-        _step = self._steps[step_name]
-        if not _step:
-            raise RuntimeError(f"step:{step_name} not found")
-        _step_executor = StepExecutor(
-            _step,
+    def _schedule_one_step(self, step_name: str, task_num: int = 0) -> StepResult:
+        step = self._steps[step_name]
+        start_time = time.time()
+        result = StepExecutor(
+            step=step,
             project=self.project,
             dataset_uris=self.dataset_uris,
-            module=self.module,
             workdir=self.workdir,
             version=self.version,
             task_num=task_num,
-        )
-        start_time = time.time()
-        _result = _step_executor.execute()
+        ).execute()
 
         logger.info(
-            f"step:{step_name} {_step.status}, result:{_result}, run time:{time.time() - start_time}"
+            f"step:{step_name}, result:{result}, run time:{time.time() - start_time}"
         )
-        return _result
+        return result
 
-    def schedule_single_task(
-        self, step_name: str, task_index: int, task_num: int = 0
-    ) -> StepResult:
+    def _schedule_one_task(self, step_name: str, task_index: int) -> StepResult:
         _step = self._steps[step_name]
-        if not _step:
-            raise RuntimeError(f"step:{step_name} not found")
-
-        total = task_num or _step.task_num
-        if task_index >= total:
+        if task_index >= _step.task_num:
             raise RuntimeError(
                 f"task_index:{task_index} out of bounds, total:{_step.task_num}"
             )
+
         _task = TaskExecutor(
             index=task_index,
             context=Context(
                 project=self.project,
                 version=self.version,
-                step=_step.step_name,
-                total=total,
+                step=_step.name,
+                total=_step.task_num,
                 index=task_index,
                 dataset_uris=self.dataset_uris,
                 workdir=self.workdir,
             ),
-            status=STATUS.INIT,
-            module=self.module,
-            func=_step.step_name,
-            cls_name=_step.cls_name,
+            step=_step,
             workdir=self.workdir,
         )
         start_time = time.time()
         task_result: TaskResult = _task.execute()
 
         logger.info(
-            f"step:{step_name} {_step.status}, task result:{task_result}, run time:{time.time() - start_time}"
+            f"step:{step_name}, task result:{task_result}, run time:{time.time() - start_time}"
         )
-        return StepResult(step_name=step_name, task_results=[task_result])
+        return StepResult(name=step_name, task_results=[task_result])
```

### Comparing `starwhale-0.4.1/starwhale/core/model/cli.py` & `starwhale-0.4.2/starwhale/core/model/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,20 @@
 @click.pass_context
 def model_cmd(ctx: click.Context) -> None:
     ctx.obj = get_term_view(ctx.obj)
 
 
 @model_cmd.command("build", help="[ONLY Standalone]Build starwhale model")
 @click.argument("workdir", type=click.Path(exists=True, file_okay=False))
-@click.option("-p", "--project", default="", help="Project URI")
+@click.option(
+    "-p",
+    "--project",
+    default="",
+    help="Project URI, default is the current selected project. The model package will store in the specified project.",
+)
 @click.option(
     "-f",
     "--model-yaml",
     default=None,
     help="mode yaml path, default use ${workdir}/model.yaml file",
 )
 @click.option("--runtime", default="", help="runtime uri")
@@ -125,15 +130,20 @@
 def _diff(
     view: t.Type[ModelTermView], base_uri: str, compare_uri: str, show_details: bool
 ) -> None:
     view(base_uri).diff(URI(compare_uri, expected_type=URIType.MODEL), show_details)
 
 
 @model_cmd.command("list", aliases=["ls"])
-@click.option("-p", "--project", default="", help="Project URI")
+@click.option(
+    "-p",
+    "--project",
+    default="",
+    help="Project URI, default is the current selected project.",
+)
 @click.option("-f", "--fullname", is_flag=True, help="Show fullname of model version")
 @click.option("-sr", "--show-removed", is_flag=True, help="Show removed model")
 @click.option(
     "--page", type=int, default=DEFAULT_PAGE_IDX, help="Page number for model list"
 )
 @click.option(
     "--size", type=int, default=DEFAULT_PAGE_SIZE, help="Page size for model list"
@@ -152,15 +162,15 @@
     fullname: bool,
     show_removed: bool,
     page: int,
     size: int,
     filters: list,
 ) -> None:
     """
-    List Model
+    List Model of the specified project.
 
     The filtering flag (-fl or --filter) format is a key=value pair or a flag.
     If there is more than one filter, then pass multiple flags.\n
     (e.g. --filter name=mnist --filter latest)
 
     \b
     The currently supported filters are:
@@ -206,31 +216,38 @@
     "-f",
     "--model-yaml",
     default=DefaultYAMLName.MODEL,
     help="Model yaml filename, default use ${MODEL_DIR}/model.yaml file",
 )
 @click.option(
     "-p",
-    "--project",
+    "--evaluation-project",
     envvar=SWEnv.project,
     default="",
-    help=f"project name, env is {SWEnv.project}",
+    help=f"Project URI, env is {SWEnv.project}.The model evaluation result will store in the specified project. Default is the current selected project.",
 )
 @click.option(
     "--version",
     envvar=SWEnv.eval_version,
     default=None,
     help=f"Evaluation job version, env is {SWEnv.eval_version}",
+    hidden=True,
+)
+@click.option("--step", default="", help="Evaluation run step", hidden=True)
+@click.option(
+    "--task-index",
+    default=None,
+    help="Index of tasks in the current step",
+    hidden=True,
 )
-@click.option("--step", default="", help="Evaluation run step")
-@click.option("--task-index", default=-1, help="Index of tasks in the current step")
 @click.option(
     "--override-task-num",
     default=0,
     help="Total num of tasks in the current step",
+    hidden=True,
 )
 @click.option("--runtime", default="", help="runtime uri")
 @click.option(
     "datasets",
     "--dataset",
     required=True,
     envvar=SWEnv.dataset_uri,
@@ -245,15 +262,15 @@
 @click.option("--gencmd", is_flag=True, help="[ONLY Standalone]gen docker run command")
 @click.option(
     "--image",
     default="",
     help="[ONLY Standalone]the image used when use docker",
 )
 def _eval(
-    project: str,
+    evaluation_project: str,
     target: str,
     model_yaml: str,
     version: str,
     datasets: list,
     step: str,
     task_index: int,
     override_task_num: int,
@@ -264,29 +281,77 @@
 ) -> None:
     """
     [ONLY Standalone]Run evaluation processing with root dir of {target}.
 
     TARGET: model uri or model workdir path, in Starwhale Agent Docker Environment, only support workdir path.
     """
     ModelTermView.eval(
-        project=project,
+        project=evaluation_project,
         target=target,
         version=version,
         yaml_name=model_yaml,
         runtime_uri=runtime,
         step=step,
         task_index=task_index,
         task_num=override_task_num,
         dataset_uris=datasets,
         use_docker=use_docker,
         gencmd=gencmd,
         image=image,
     )
 
 
+@model_cmd.command("fine-tune", aliases=["ft"])
+@click.argument("target", required=False, default="")
+@click.option(
+    "-f",
+    "--model-yaml",
+    default=DefaultYAMLName.MODEL,
+    help="Model yaml filename, default use ${MODEL_DIR}/model.yaml file",
+)
+@click.option(
+    "-p",
+    "--project",
+    envvar=SWEnv.project,
+    default="",
+    help=f"Project URI, env is {SWEnv.project}. Default is the current selected project.",
+)
+@click.option("-r", "--runtime", default="", help="runtime uri")
+@click.option("-m", "--model", default="", help="model uri")
+@click.option(
+    "datasets",
+    "--dataset",
+    required=True,
+    envvar=SWEnv.dataset_uri,
+    multiple=True,
+    help=f"dataset uri, env is {SWEnv.dataset_uri}",
+)
+def _fine_tune(
+    target: str,
+    model_yaml: str,
+    project: str,
+    datasets: list,
+    runtime: str,
+    model: str,
+) -> None:
+    """
+    [ONLY Standalone]Run fine tuning with root dir of {target}.
+
+    TARGET: model uri or model workdir path, in Starwhale Agent Docker Environment, only support workdir path.
+    """
+    ModelTermView.fine_tune(
+        target=target,
+        project=project,
+        yaml_name=model_yaml,
+        dataset_uris=datasets,
+        runtime_uri=runtime,
+        model_uri=model,
+    )
+
+
 @model_cmd.command("serve")
 @click.argument("target", required=False, default="")
 @click.option(
     "-f",
     "--model-yaml",
     default=DefaultYAMLName.MODEL,
     help="Model yaml filename, default use ${MODEL_DIR}/model.yaml file",
```

### Comparing `starwhale-0.4.1/starwhale/core/model/copy.py` & `starwhale-0.4.2/starwhale/core/model/copy.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,10 +64,7 @@
                 name=_m["name"],
                 file_desc=FileDesc.MODEL,
             )
             # TODO use unified storage
             # Path(workdir / _m["path"]).symlink_to(
             #     _dest # the unify dir
             # )
-
-    def _do_ubd_datastore(self) -> None:
-        ...
```

### Comparing `starwhale-0.4.1/starwhale/core/model/model.py` & `starwhale-0.4.2/starwhale/core/model/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,28 +17,31 @@
 
 from starwhale import PipelineHandler
 from starwhale.utils import console, now_str, load_yaml, gen_uniq_version
 from starwhale.consts import (
     FileDesc,
     FileFlag,
     FileNode,
+    RunStatus,
     CREATED_AT_KEY,
     SWMP_SRC_FNAME,
     DefaultYAMLName,
-    EvalHandlerType,
     SW_AUTO_DIRNAME,
     DEFAULT_PAGE_IDX,
     DEFAULT_PAGE_SIZE,
     SW_IGNORE_FILE_NAME,
     DEFAULT_MANIFEST_NAME,
+    DEFAULT_JOBS_FILE_NAME,
+    DEFAULT_FINETUNE_JOB_NAME,
     SW_EVALUATION_EXAMPLE_DIR,
-    DEFAULT_EVALUATION_PIPELINE,
-    DEFAULT_EVALUATION_JOBS_FNAME,
+    DEFAULT_EVALUATION_JOB_NAME,
     DEFAULT_STARWHALE_API_VERSION,
-    DEFAULT_EVALUATION_SVC_META_FNAME,
+    EVALUATION_SVC_META_FILE_NAME,
+    EVALUATION_PANEL_LAYOUT_JSON_FILE_NAME,
+    EVALUATION_PANEL_LAYOUT_YAML_FILE_NAME,
     DEFAULT_FILE_SIZE_THRESHOLD_TO_TAR_IN_MODEL,
 )
 from starwhale.base.tag import StandaloneTag
 from starwhale.base.uri import URI
 from starwhale.utils.fs import (
     move_dir,
     copy_file,
@@ -51,38 +54,36 @@
 from starwhale.base.cloud import CloudRequestMixed, CloudBundleModelMixin
 from starwhale.base.mixin import ASDictMixin
 from starwhale.utils.http import ignore_error
 from starwhale.utils.load import load_module
 from starwhale.api.service import Service
 from starwhale.base.bundle import BaseBundle, LocalStorageBundleMixin
 from starwhale.utils.error import NoSupportError, FileFormatError
-from starwhale.api._impl.job import Parser, Context, context_holder
-from starwhale.core.job.model import STATUS, Generator
+from starwhale.api._impl.job import generate_jobs_yaml
+from starwhale.core.job.step import Step
 from starwhale.utils.progress import run_with_progress_bar
 from starwhale.base.blob.store import LocalFileStore
 from starwhale.core.eval.store import EvaluationStorage
 from starwhale.core.model.copy import ModelCopy
+from starwhale.core.job.context import Context
 from starwhale.core.model.store import ModelStorage
 from starwhale.api._impl.service import Hijack
 from starwhale.core.job.scheduler import Scheduler
 
 
 class ModelRunConfig(ASDictMixin):
-
     # TODO: use attr to tune class
     def __init__(
         self,
         handler: str,
-        type: str = EvalHandlerType.DEFAULT,
         runtime: str = "",
         envs: t.Union[t.List[str], None] = None,
         **kw: t.Any,
     ):
         self.handler = handler.strip()
-        self.typ = type
         self.runtime = runtime.strip()
         self.envs = envs or []
         self.kw = kw
 
         self._do_validate()
 
     def _do_validate(self) -> None:
@@ -93,15 +94,14 @@
         return f"Model Run Config: ppl -> {self.handler}"
 
     def __repr__(self) -> str:
         return f"Model Run Config: ppl -> {self.handler}, runtime -> {self.runtime}"
 
 
 class ModelConfig(ASDictMixin):
-
     # TODO: use attr to tune class
     def __init__(
         self,
         name: str,
         run: t.Dict[str, t.Any],
         desc: str = "",
         tag: t.Optional[t.List[str]] = None,
@@ -214,30 +214,22 @@
 
     def add_tags(self, tags: t.List[str], ignore_errors: bool = False) -> None:
         self.tag.add(tags, ignore_errors)
 
     def remove_tags(self, tags: t.List[str], ignore_errors: bool = False) -> None:
         self.tag.remove(tags, ignore_errors)
 
-    def _gen_steps(self, typ: str, ppl: str, workdir: Path) -> None:
-        if typ == EvalHandlerType.DEFAULT:
-            # use default
-            ppl = DEFAULT_EVALUATION_PIPELINE
-        _f = self.store.hidden_sw_dir / DEFAULT_EVALUATION_JOBS_FNAME
-        logger.debug(f"job ppl path:{_f}, ppl is {ppl}")
-        Parser.generate_job_yaml(ppl, workdir, _f)
-
     def _gen_model_serving(self, ppl: str, workdir: Path) -> None:
         rc_dir = str(
             self.store.hidden_sw_dir.relative_to(self.store.snapshot_workdir)
             / SW_EVALUATION_EXAMPLE_DIR
         )
         # render spec
         svc = self._get_service(ppl, workdir, hijack=Hijack(True, rc_dir))
-        file = self.store.hidden_sw_dir / DEFAULT_EVALUATION_SVC_META_FNAME
+        file = self.store.hidden_sw_dir / EVALUATION_SVC_META_FILE_NAME
         ensure_file(file, json.dumps(svc.get_spec(), indent=4), parents=True)
 
         if len(svc.example_resources) == 0:
             return
 
         # check duplicate file names, do not support using examples with same name in different dir
         names = set([os.path.basename(i) for i in svc.example_resources])
@@ -246,27 +238,35 @@
 
         # copy example resources for online evaluation in server instance
         dst = self.store.hidden_sw_dir / SW_EVALUATION_EXAMPLE_DIR
         ensure_dir(dst)
         for f in svc.example_resources:
             shutil.copy2(f, dst)
 
+    def _render_eval_layout(self, workdir: Path) -> None:
+        # render eval layout
+        eval_layout = workdir / SW_AUTO_DIRNAME / EVALUATION_PANEL_LAYOUT_YAML_FILE_NAME
+        if eval_layout.exists():
+            content = load_yaml(eval_layout)
+            dst = self.store.hidden_sw_dir / EVALUATION_PANEL_LAYOUT_JSON_FILE_NAME
+            ensure_file(dst, json.dumps(content), parents=True)
+
     @staticmethod
     def _get_service(
         module: str, pkg: Path, hijack: t.Optional[Hijack] = None
     ) -> Service:
         module, _, attr = module.partition(":")
         m = load_module(module, pkg)
         apis = dict()
         ins: t.Any = None
         svc: t.Optional[Service] = None
 
         # TODO: refine this ugly ad hoc
-        context_holder.context = Context(
-            pkg, version="-1", project="tmp-project-for-build"
+        Context.set_runtime_context(
+            Context(pkg, version="-1", project="tmp-project-for-build")
         )
 
         # TODO: check duplication
         for k, v in m.__dict__.items():
             if isinstance(v, Service):
                 apis.update(v.apis)
                 # use Service in module
@@ -295,115 +295,86 @@
         for api in apis.values():
             svc.add_api_instance(api)
         svc.api_instance = ins
         svc.hijack = hijack
         return svc
 
     @classmethod
-    def get_pipeline_handler(
-        cls,
-        workdir: Path,
-        yaml_name: str = DefaultYAMLName.MODEL,
-    ) -> str:
-        _mp = workdir / yaml_name
-        _model_config = cls.load_model_config(_mp, workdir)
-        return cls._get_module(_model_config)
-
-    @classmethod
     def eval_user_handler(
         cls,
         project: str,
         version: str,
         workdir: Path,
         dataset_uris: t.List[str],
         model_yaml_name: str = DefaultYAMLName.MODEL,
-        job_name: str = "default",
+        job_name: str = DEFAULT_EVALUATION_JOB_NAME,
         step_name: str = "",
-        task_index: int = 0,
+        task_index: t.Optional[int] = None,
         task_num: int = 0,
         base_info: t.Optional[t.Dict[str, t.Any]] = None,
     ) -> None:
         base_info = base_info or {}
-        # init manifest
         _manifest: t.Dict[str, t.Any] = {
             CREATED_AT_KEY: now_str(),
-            "status": STATUS.START,
+            "status": RunStatus.START,
             "step": step_name,
             "task_index": task_index,
             "task_num": task_num,
         }
-        # load model config by yaml
         _model_config = cls.load_model_config(workdir / model_yaml_name, workdir)
 
         if not version:
             version = gen_uniq_version()
 
         _project_uri = URI(project, expected_type=URIType.PROJECT)
         _run_dir = EvaluationStorage.local_run_dir(_project_uri.project, version)
         ensure_dir(_run_dir)
 
-        _module = cls._get_module(_model_config)
-        _yaml_path = str(workdir / SW_AUTO_DIRNAME / DEFAULT_EVALUATION_JOBS_FNAME)
-
-        # generate if not exists
-        if not os.path.exists(_yaml_path):
-            _new_yaml_path = _run_dir / SW_AUTO_DIRNAME / DEFAULT_EVALUATION_JOBS_FNAME
-            Parser.generate_job_yaml(_module, workdir, _new_yaml_path)
-            _yaml_path = str(_new_yaml_path)
-
-        # parse job steps from yaml
-        logger.debug(f"parse job from yaml:{_yaml_path}")
-        _jobs = Generator.generate_job_from_yaml(_yaml_path)
+        yaml_path = workdir / SW_AUTO_DIRNAME / DEFAULT_JOBS_FILE_NAME
 
-        if job_name not in _jobs:
-            raise RuntimeError(f"job:{job_name} not found")
+        if not yaml_path.exists():
+            # do not auto generate eval_job.yaml in the user workdir
+            generate_jobs_yaml(
+                run_handler=_model_config.run.handler,
+                workdir=workdir,
+                yaml_path=yaml_path,
+            )
 
-        _steps = _jobs[job_name]
+        logger.debug(f"parse job from yaml:{yaml_path}")
 
         console.print(
             f":hourglass_not_done: start to run evaluation[{job_name}:{version}]..."
         )
-        logger.debug(f"-->[Running] start to run evaluation[{job_name}:{version}].")
         _scheduler = Scheduler(
             project=_project_uri.project,
             version=version,
-            module=_module,
             workdir=workdir,
             dataset_uris=dataset_uris,
-            steps=_steps,
+            steps=Step.get_steps_from_yaml(job_name, yaml_path),
         )
-        _status = STATUS.START
+        _status = RunStatus.START
         try:
-            if not step_name:
-                _step_results = _scheduler.schedule()
-            elif task_index < 0:
-                _step_results = [
-                    _scheduler.schedule_single_step(
-                        step_name=step_name, task_num=task_num
-                    )
-                ]
-            else:
-                _step_results = [
-                    _scheduler.schedule_single_task(step_name, task_index, task_num)
-                ]
-
-            _status = STATUS.SUCCESS
+            _results = _scheduler.run(
+                step_name=step_name, task_index=task_index, task_num=task_num
+            )
+            _status = RunStatus.SUCCESS
 
             exceptions: t.List[Exception] = []
-            for _sr in _step_results:
-                for _tr in _sr.task_results:
+            for _r in _results:
+                for _tr in _r.task_results:
                     if _tr.exception:
                         exceptions.append(_tr.exception)
             if exceptions:
                 raise Exception(*exceptions)
+
             logger.debug(
-                f"-->[Finished] evaluation[{job_name}:{version}] execute finished, results info:{_step_results}"
+                f"-->[Finished] evaluation[{job_name}:{version}] execute finished, results info:{_results}"
             )
         except Exception as e:
-            _status = STATUS.FAILED
+            _status = RunStatus.FAILED
             _manifest["error_message"] = str(e)
             logger.error(
                 f"-->[Failed] evaluation[{job_name}:{version}] execute failed, error info:{e}"
             )
             raise
         finally:
             _manifest.update(
@@ -419,23 +390,83 @@
                     **base_info,
                 }
             )
             _f = _run_dir / DEFAULT_MANIFEST_NAME
             ensure_file(_f, yaml.safe_dump(_manifest, default_flow_style=False))
 
             console.print(
-                f":{100 if _status == STATUS.SUCCESS else 'broken_heart'}: finish run, {_status}!"
+                f":{100 if _status == RunStatus.SUCCESS else 'broken_heart'}: finish run, {_status}!"
             )
 
     @classmethod
-    def _get_module(cls, _model_config: ModelConfig) -> str:
-        if _model_config.run.typ == EvalHandlerType.DEFAULT:
-            return DEFAULT_EVALUATION_PIPELINE
-        else:
-            return _model_config.run.handler
+    def fine_tune(
+        cls,
+        project: str,
+        workdir: Path,
+        dataset_uris: t.List[str],
+        model_yaml_name: str = DefaultYAMLName.MODEL,
+        job_name: str = DEFAULT_FINETUNE_JOB_NAME,
+        step_name: str = "fine_tune",
+        task_index: int = 0,
+        task_num: int = 1,
+    ) -> None:
+        _model_config = cls.load_model_config(workdir / model_yaml_name, workdir)
+
+        _project_uri = URI(project, expected_type=URIType.PROJECT)
+
+        yaml_path = workdir / SW_AUTO_DIRNAME / DEFAULT_JOBS_FILE_NAME
+
+        if not yaml_path.exists():
+            # do not auto generate eval_job.yaml in the user workdir
+            generate_jobs_yaml(
+                run_handler=_model_config.run.handler,
+                workdir=workdir,
+                yaml_path=yaml_path,
+            )
+
+        logger.debug(f"parse fine-tune job from yaml:{yaml_path}")
+        version = gen_uniq_version()
+        console.print(
+            f":hourglass_not_done: start to run fine-tune[{job_name}:{version}]..."
+        )
+        _scheduler = Scheduler(
+            project=_project_uri.project,
+            version=version,
+            workdir=workdir,
+            dataset_uris=dataset_uris,
+            steps=Step.get_steps_from_yaml(job_name, yaml_path),
+        )
+        _status = RunStatus.START
+        try:
+            _results = _scheduler.run(
+                step_name=step_name, task_index=task_index, task_num=task_num
+            )
+            _status = RunStatus.SUCCESS
+
+            exceptions: t.List[Exception] = []
+            for _r in _results:
+                for _tr in _r.task_results:
+                    if _tr.exception:
+                        exceptions.append(_tr.exception)
+            if exceptions:
+                raise Exception(*exceptions)
+
+            logger.debug(
+                f"-->[Finished] fine-tune[{job_name}:{version}] execute finished, results info:{_results}"
+            )
+        except Exception as e:
+            _status = RunStatus.FAILED
+            logger.error(
+                f"-->[Failed] fine-tune[{job_name}:{version}] execute failed, error info:{e}"
+            )
+            raise
+        finally:
+            console.print(
+                f":{100 if _status == RunStatus.SUCCESS else 'broken_heart'}: finish run, {_status}!"
+            )
 
     def diff(self, compare_uri: URI) -> t.Dict[str, t.Any]:
         """
         - added: a node that exists in compare but not in base
         - deleted: a node that not exists in compare but in base
         - updated: a node that exists in both of base and compare but signature is different
         - unchanged: a node that exists in both of base and compare, and signature is same
@@ -483,15 +514,15 @@
             "compare_version": compare_file_maps,
         }
 
     def info(self) -> t.Dict[str, t.Any]:
         _manifest = self._get_bundle_info()
         _store = self.store
         _om = {}
-        yaml_path = _store.hidden_sw_dir / DEFAULT_EVALUATION_JOBS_FNAME
+        yaml_path = _store.hidden_sw_dir / DEFAULT_JOBS_FILE_NAME
         if _store.snapshot_workdir.exists():
             if yaml_path.exists():
                 _om = load_yaml(yaml_path)
             else:
                 logger.warning("step_spec not found in model snapshot_workdir")
         else:
             logger.warning("step_spec not found in model")
@@ -500,15 +531,14 @@
         return _manifest
 
     def history(
         self,
         page: int = DEFAULT_PAGE_IDX,
         size: int = DEFAULT_PAGE_SIZE,
     ) -> t.List[t.Dict[str, t.Any]]:
-
         _r = []
         for _bf in self.store.iter_bundle_history():
             _manifest_path = _bf.path / DEFAULT_MANIFEST_NAME
             if not _manifest_path.exists():
                 continue
 
             _manifest = load_yaml(_manifest_path)
@@ -593,30 +623,38 @@
             (
                 self._copy_src,
                 15,
                 "copy src",
                 dict(workdir=workdir, yaml_path=yaml_path),
             ),
             (
-                self._gen_steps,
+                generate_jobs_yaml,
                 5,
-                "generate execute steps",
+                "generate jobs yaml",
                 dict(
-                    typ=_model_config.run.typ,
-                    ppl=_model_config.run.handler,
+                    run_handler=_model_config.run.handler,
                     workdir=workdir,
+                    yaml_path=self.store.src_dir
+                    / SW_AUTO_DIRNAME
+                    / DEFAULT_JOBS_FILE_NAME,
                 ),
             ),
             (
                 self._gen_model_serving,
                 10,
                 "generate model serving",
                 dict(ppl=_model_config.run.handler, workdir=workdir),
             ),
             (
+                self._render_eval_layout,
+                1,
+                "render eval layout",
+                dict(workdir=workdir),
+            ),
+            (
                 self._make_meta_tar,
                 20,
                 "build model bundle",
             ),
             (
                 self._render_manifest,
                 5,
```

### Comparing `starwhale-0.4.1/starwhale/core/model/store.py` & `starwhale-0.4.2/starwhale/core/model/store.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/core/model/view.py` & `starwhale-0.4.2/starwhale/core/model/view.py`

 * *Files 10% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         cls,
         project: str,
         target: str,
         dataset_uris: t.List[str],
         version: str = "",
         yaml_name: str = DefaultYAMLName.MODEL,
         step: str = "",
-        task_index: int = 0,
+        task_index: t.Optional[int] = None,
         task_num: int = 0,
         runtime_uri: str = "",
         use_docker: bool = False,
         gencmd: bool = False,
         image: str = "",
     ) -> None:
         if use_docker:
@@ -180,14 +180,53 @@
                 target=StandaloneModel.eval_user_handler,
                 kwargs=kw,
             ).run()
         else:
             StandaloneModel.eval_user_handler(**kw)  # type: ignore
 
     @classmethod
+    @BaseTermView._only_standalone
+    def fine_tune(
+        cls,
+        project: str,
+        target: str,
+        dataset_uris: t.List[str],
+        yaml_name: str = DefaultYAMLName.MODEL,
+        runtime_uri: str = "",
+        model_uri: str = "",
+    ) -> None:
+        if target and model_uri:
+            console.print("workdir and model can not both set together")
+            sys.exit(1)
+        if not target and not model_uri:
+            console.print("workdir or model needs to be set")
+            sys.exit(1)
+
+        if target:
+            workdir = cls._get_workdir(target)
+        else:
+            _m = StandaloneModel(URI(model_uri, expected_type=URIType.MODEL))
+            workdir = _m.store.src_dir
+
+        kw = dict(
+            project=project,
+            workdir=workdir,
+            dataset_uris=dataset_uris,
+            model_yaml_name=yaml_name,
+        )
+        if not in_production() and runtime_uri:
+            RuntimeProcess.from_runtime_uri(
+                uri=runtime_uri,
+                target=StandaloneModel.fine_tune,
+                kwargs=kw,
+            ).run()
+        else:
+            StandaloneModel.fine_tune(**kw)  # type: ignore
+
+    @classmethod
     def _get_workdir(cls, target: str) -> Path:
         if in_production() or (os.path.exists(target) and os.path.isdir(target)):
             workdir = Path(target)
         else:
             _uri = URI(target, URIType.MODEL)
             _store = ModelStorage(_uri)
             workdir = _store.src_dir
```

### Comparing `starwhale-0.4.1/starwhale/core/project/cli.py` & `starwhale-0.4.2/starwhale/core/project/cli.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/core/project/model.py` & `starwhale-0.4.2/starwhale/core/project/model.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/core/project/view.py` & `starwhale-0.4.2/starwhale/core/project/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
                 otree = tree.add(f"{_o['name']}")
                 for _v in _o["latest_versions"]:
                     _k = "name" if fullname else "short_name"
                     if typ == ProjectObjType.MODEL:
                         # TODO: add model version for every version
                         _size = _o["files"][0]["size"]
                     else:
-                        _size = pretty_bytes(_v["meta"]["dataset_byte_size"])
+                        _size = pretty_bytes(_v["meta"]["blobs_byte_size"])
 
                     otree.add(
                         f"[{_v['id']}][green]{_v[_k]}[/] :timer_clock: {_v['created_at']} :dizzy:{_size}"
                     )
             return tree
 
         console.print(Panel(Pretty(_r), title="Project Details", title_align="left"))
@@ -172,15 +172,15 @@
                 otree = tree.add(f"{_o['name']}")
                 for _v in _o["latest_versions"]:
                     _k = "name" if fullname else "short_name"
                     if typ == ProjectObjType.MODEL:
                         # TODO: add model version for every version
                         _size = _o["files"][0]["size"]
                     else:
-                        _size = pretty_bytes(_v["meta"]["dataset_byte_size"])
+                        _size = pretty_bytes(_v["meta"]["blobs_byte_size"])
 
                     otree.add(
                         f"[{_v['id']}][green]{_v[_k]}[/] :timer_clock: {_v['created_at']} :dizzy:{_size}"
                     )
             return tree
 
         console.print(Panel(Pretty(_r), title="Project Details", title_align="left"))
```

### Comparing `starwhale-0.4.1/starwhale/core/runtime/cli.py` & `starwhale-0.4.2/starwhale/core/runtime/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,23 +10,24 @@
     DefaultYAMLName,
     DEFAULT_PAGE_IDX,
     DEFAULT_PAGE_SIZE,
 )
 from starwhale.base.uri import URI
 from starwhale.base.type import URIType, RuntimeLockFileType
 from starwhale.utils.cli import AliasedGroup
-from starwhale.utils.error import MissingFieldError, ExclusiveArgsError
+from starwhale.core.runtime.model import _SUPPORT_CUDA, _SUPPORT_CUDNN
 
 from .view import get_term_view, RuntimeTermView
+from .model import RuntimeInfoFilter
 
 
 @click.group(
     "runtime",
     cls=AliasedGroup,
-    help="Runtime management, quickstart/build/copy/activate/restore...",
+    help="Runtime management, quickstart/build/copy/activate...",
 )
 @click.pass_context
 def runtime_cmd(ctx: click.Context) -> None:
     ctx.obj = get_term_view(ctx.obj)
 
 
 @click.group(
@@ -125,94 +126,243 @@
     p_workdir = Path(workdir).absolute()
     name = name or p_workdir.name
     RuntimeTermView.quickstart_from_ishell(
         p_workdir, name, python_env, disable_create_env, force, interactive
     )
 
 
-@runtime_cmd.command(
-    "build",
-    help="[Only Standalone]Create and build a relocated, shareable, packaged runtime bundle. Support python and native libs.",
+@runtime_cmd.command("build")
+@optgroup.group(
+    "\n  ** Acceptable build sources",
+    cls=MutuallyExclusiveOptionGroup,
+    help="The selector of the runtime build source, default is runtime.yaml source",
 )
-@click.argument("workdir", type=click.Path(exists=True, file_okay=False))
-@click.option("-p", "--project", default="", help="Project URI")
-@click.option(
-    "-f",
-    "--runtime-yaml",
-    default=DefaultYAMLName.RUNTIME,
-    help="Runtime yaml filename, default use ${workdir}/runtime.yaml file",
+@optgroup.option(  # type: ignore[no-untyped-call]
+    "-c",
+    "--conda",
+    default="",
+    help="from conda environment name",
 )
-@click.option(
-    "-gab",
-    "--gen-all-bundles",
-    is_flag=True,
-    help="Generate conda or venv files into runtime",
+@optgroup.option(  # type: ignore[no-untyped-call]
+    "-cp",
+    "--conda-prefix",
+    default="",
+    help="from conda environment prefix path",
 )
-@click.option(
-    "-ie", "--include-editable", is_flag=True, help="Include editable packages"
+@optgroup.option(  # type: ignore[no-untyped-call]
+    "-v",
+    "--venv",
+    help="from virtualenv or python-venv environment prefix path",
+)
+@optgroup.option(  # type: ignore[no-untyped-call]
+    "-s",
+    "--shell",
+    is_flag=True,
+    help="from current shell, venv or conda environment has been activated",
+)
+@optgroup.option(  # type: ignore[no-untyped-call]
+    "-y",
+    "--yaml",
+    help="from runtime yaml format file path.Default use runtime.yaml in the work directory(pwd)",
+    default=DefaultYAMLName.RUNTIME,
 )
-@click.option(
-    "-ilw", "--include-local-wheel", is_flag=True, help="Include local wheel packages"
+@optgroup.option(  # type: ignore[no-untyped-call]
+    "-d",
+    "--docker",
+    default="",
+    help="from docker image",
 )
-@click.option(
+@optgroup.group(
+    "\n  ** Runtime YAML Source Configuration",
+    help="The configurations only work for `--from-runtime-yaml` source",
+)
+@optgroup.option(  # type: ignore[no-untyped-call]
     "-del",
     "--disable-env-lock",
     is_flag=True,
-    help="Disable virtualenv/conda environment dependencies lock, and the cli supports three methods to lock environment that are shell(auto-detect), prefix_path or env_name",
+    help="Disable virtualenv/conda environment dependencies lock",
 )
-@click.option(
+@optgroup.option(  # type: ignore[no-untyped-call]
     "-nc",
     "--no-cache",
     is_flag=True,
     help="Invalid the cached(installed) packages in the isolate env when env-lock is enabled, \
     only for auto-generated environments",
 )
-@optgroup.group(  # type: ignore
-    "Python environment selectors",
-    cls=MutuallyExclusiveOptionGroup,
-    help="The selector of the python environment, default is the starwhale auto create env prefix path",
+@optgroup.option(  # type: ignore[no-untyped-call]
+    "-dad",
+    "--download-all-deps",
+    is_flag=True,
+    help="Download all python dependencies into the runtime bundle file, the file size of swrt maybe very large.",
+    hidden=True,
 )
-@optgroup.option(  # type: ignore
-    "-ep", "--env-prefix-path", default="", help="Conda or virtualenv prefix path"
+@optgroup.option(  # type: ignore[no-untyped-call]
+    "-ie",
+    "--include-editable",
+    is_flag=True,
+    help="Include editable packages",
+    hidden=True,
 )
-@optgroup.option(  # type: ignore
-    "-en",
-    "--env-name",
+@optgroup.option(  # type: ignore[no-untyped-call]
+    "-ilw",
+    "--include-local-wheel",
+    is_flag=True,
+    help="Include local wheel packages",
+    hidden=True,
+)
+@optgroup.group(
+    "\n  ** Conda/Venv/Shell Sources Configurations",
+    help="The configurations only work for `--from-conda-name`, `--from-conda-prefix-path`, `--from-venv-prefix-path` and `--from-shell` sources",
+)
+@optgroup.option(  # type: ignore[no-untyped-call]
+    "--cuda",
+    type=click.Choice(_SUPPORT_CUDA + [""], case_sensitive=False),
     default="",
-    help="conda name in lock or gen all bundles process",
+    help="cuda version, works for shell, conda name, conda prefix path and venv prefix path sources",
 )
-@optgroup.option(  # type: ignore
-    "-es", "--env-use-shell", is_flag=True, default=False, help="use current shell"
+@optgroup.option(  # type: ignore[no-untyped-call]
+    "--cudnn",
+    default="",
+    type=click.Choice(list(_SUPPORT_CUDNN.keys()) + [""], case_sensitive=False),
+    help="cudnn version, works for shell, conda name, conda prefix path and venv prefix path sources",
+)
+@optgroup.option(  # type: ignore[no-untyped-call]
+    "--arch",
+    type=click.Choice(
+        [SupportArch.AMD64, SupportArch.ARM64, SupportArch.NOARCH],
+        case_sensitive=False,
+    ),
+    default=SupportArch.NOARCH,
+    help="system architecture, works for shell, conda name, conda prefix path and venv prefix path sources",
+)
+@optgroup.option(  # type: ignore[no-untyped-call]
+    "-dad",
+    "--download-all-deps",
+    is_flag=True,
+    help="Download all python dependencies into the runtime bundle file, the file size of swrt maybe very large.",
+    hidden=True,
+)
+@optgroup.option(  # type: ignore[no-untyped-call]
+    "-ie",
+    "--include-editable",
+    is_flag=True,
+    help="Include editable packages",
+    hidden=True,
+)
+@optgroup.option(  # type: ignore[no-untyped-call]
+    "-ilw",
+    "--include-local-wheel",
+    is_flag=True,
+    help="Include local wheel packages",
+    hidden=True,
+)
+@optgroup.group("\n  ** Global Configurations")
+@optgroup.option("-n", "--name", default="", help="runtime name")  # type: ignore[no-untyped-call]
+@optgroup.option(  # type: ignore[no-untyped-call]
+    "-p",
+    "--project",
+    default="",
+    help="Project URI, default is the current selected project. The runtime package will store in the specified project.",
 )
 def _build(
-    workdir: str,
+    name: str,
     project: str,
-    runtime_yaml: str,
-    gen_all_bundles: bool,
+    cuda: str,
+    cudnn: str,
+    arch: str,
+    download_all_deps: bool,
     include_editable: bool,
     include_local_wheel: bool,
     disable_env_lock: bool,
     no_cache: bool,
-    env_prefix_path: str,
-    env_name: str,
-    env_use_shell: bool,
+    conda: str,
+    conda_prefix: str,
+    venv: str,
+    shell: bool,
+    yaml: str,
+    docker: str,
 ) -> None:
-    RuntimeTermView.build(
-        workdir=workdir,
-        project=project,
-        yaml_name=runtime_yaml,
-        gen_all_bundles=gen_all_bundles,
-        include_editable=include_editable,
-        include_local_wheel=include_local_wheel,
-        disable_env_lock=disable_env_lock,
-        no_cache=no_cache,
-        env_prefix_path=env_prefix_path,
-        env_name=env_name,
-        env_use_shell=env_use_shell,
-    )
+    """Create and build a relocated, shareable, packaged runtime bundle(aka `swrt` file). Support python and native libs.
+    Runtime build only works in the Standalone instance.
+
+    Acceptable sources:
+
+        \b
+        - runtime.yaml file: The most flexible and customizable way.By the runtime.yaml file,
+            you can specify the runtime name, python version, conda or venv environment, and the python dependency packages etc.
+        - conda name: Lock the conda environment with conda name and generate the runtime bundle.
+        - conda prefix path: Lock the conda environment with conda prefix path and generate the runtime bundle.
+        - venv prefix path: Lock the virtualenv or python venv environment with venv prefix path and generate the runtime bundle.
+        - shell: Lock the current shell environment and generate the runtime bundle. The current shell must be conda or venv.
+        - docker image: Use the docker image as the runtime directly.
+
+    Examples:
+
+        \b
+        - from runtime.yaml:
+        swcli runtime build  # use the current directory as the workdir and use the default runtime.yaml file
+        swcli runtime build -y example/pytorch/runtime.yaml # use example/pytorch/runtime.yaml as the runtime.yaml file
+        swcli runtime build --yaml runtime.yaml # use runtime.yaml at the current directory as the runtime.yaml file
+
+        \b
+        - from conda name:
+        swcli runtime build -c pytorch # lock pytorch conda environment and use `pytorch` as the runtime name
+        swcli runtime build --conda pytorch --name pytorch-runtime # use `pytorch-runtime` as the runtime name
+        swcli runtime build --conda pytorch --cuda 11.4 # specify the cuda version
+        swcli runtime build --conda pytorch --arch noarch # specify the system architecture
+
+        \b
+        - from conda prefix path:
+        swcli runtime build --conda-prefix /home/starwhale/anaconda3/envs/pytorch # get conda prefix path by `conda info --envs` command
+
+        \b
+        - from venv prefix path:
+        swcli runtime build -v /home/starwhale/.virtualenvs/pytorch
+        swcli runtime build --venv /home/starwhale/.local/share/virtualenvs/pytorch --arch amd64
+
+        \b
+        - from docker image:
+        swcli runtime build --docker pytorch/pytorch:1.9.0-cuda11.1-cudnn8-runtime  # use the docker image as the runtime directly
+
+        \b
+        - from shell:
+        swcli runtime build -s --cuda 11.4 --cudnn 8 # specify the cuda and cudnn version
+        swcli runtime build --shell --name pytorch-runtime # lock the current shell environment and use `pytorch-runtime` as the runtime name
+    """
+    if docker:
+        RuntimeTermView.build_from_docker_image(
+            image=docker, runtime_name=name, project=project
+        )
+    elif conda or conda_prefix or venv or shell:
+        # TODO: support auto mode for cuda, cudnn and arch
+        RuntimeTermView.build_from_python_env(
+            runtime_name=name,
+            conda_name=conda,
+            conda_prefix=conda_prefix,
+            venv_prefix=venv,
+            project=project,
+            cuda=cuda,
+            cudnn=cudnn,
+            arch=arch,
+            download_all_deps=download_all_deps,
+            include_editable=include_editable,
+            include_local_wheel=include_local_wheel,
+        )
+    else:
+        RuntimeTermView.build_from_runtime_yaml(
+            workdir=Path.cwd(),
+            yaml_path=Path(yaml),
+            project=project,
+            runtime_name=name,
+            download_all_deps=download_all_deps,
+            include_editable=include_editable,
+            include_local_wheel=include_local_wheel,
+            no_cache=no_cache,
+            disable_env_lock=disable_env_lock,
+        )
 
 
 @runtime_cmd.command("remove", aliases=["rm"])
 @click.argument("runtime")
 @click.option(
     "-f",
     "--force",
@@ -239,43 +389,80 @@
     Recover runtime
 
     RUNTIME: argument use the `Runtime URI` format, so you can recover the whole runtime or a specified-version runtime.
     """
     RuntimeTermView(runtime).recover(force)
 
 
-@runtime_cmd.command("info", help="Show runtime details")
+@runtime_cmd.command("info")
 @click.argument("runtime")
-@click.option("--fullname", is_flag=True, help="Show version fullname")
+@click.option(
+    "-of",
+    "--output-filter",
+    type=click.Choice([f.value for f in RuntimeInfoFilter], case_sensitive=False),
+    default=RuntimeInfoFilter.basic.value,
+    show_default=True,
+    help="Filter the output content. Only standalone instance supports this option.",
+)
 @click.pass_obj
-def _info(view: t.Type[RuntimeTermView], runtime: str, fullname: bool) -> None:
-    view(runtime).info(fullname)
+def _info(
+    view: t.Type[RuntimeTermView],
+    runtime: str,
+    output_filter: str,
+) -> None:
+    """Show runtime details
+
+    RUNTIME: argument use the `Runtime URI` format. Version is optional for the Runtime URI.
+    If the version is not specified, the latest version will be used.
+
+    Example:
+
+        \b
+          swcli runtime info pytorch # show basic info from the latest version of runtime
+          swcli runtime info pytorch/version/v0  # show basic info
+          swcli runtime info pytorch/version/v0 --output-filter basic  # show basic info
+          swcli runtime info pytorch/version/v1 -of runtime_yaml  # show runtime.yaml content
+          swcli runtime info pytorch/version/v1 -of lock # show auto lock file content
+          swcli runtime info pytorch/version/v1 -of manifest # show _manifest.yaml content
+          swcli runtime info pytorch/version/v1 -of all # show all info of the runtime
+    """
+    uri = URI(runtime, expected_type=URIType.RUNTIME)
+    if not uri.object.version:
+        uri.object.version = "latest"
+
+    view(uri).info(RuntimeInfoFilter(output_filter))
 
 
 @runtime_cmd.command("history", help="Show runtime history")
 @click.argument("runtime", required=True)
 @click.option("--fullname", is_flag=True, help="Show version fullname")
 @click.pass_obj
 def _history(view: t.Type[RuntimeTermView], runtime: str, fullname: bool) -> None:
     view(runtime).history(fullname)
 
 
-@runtime_cmd.command("restore")
+# hide runtime restore command for the users in the command help output.
+@runtime_cmd.command("restore", hidden=True)
 @click.argument("target")
 def _restore(target: str) -> None:
     """
     [Only Standalone]Prepare dirs, restore python environment with virtualenv or conda and show activate command.
 
     TARGET: runtime uri or runtime workdir path, in Starwhale Agent Docker Environment, only support workdir path.
     """
     RuntimeTermView.restore(target)
 
 
 @runtime_cmd.command("list", aliases=["ls"])
-@click.option("-p", "--project", default="", help="Project URI")
+@click.option(
+    "-p",
+    "--project",
+    default="",
+    help="Project URI, the default is the current selected project.",
+)
 @click.option("-f", "--fullname", is_flag=True, help="Show fullname of runtime version")
 @click.option("-sr", "--show-removed", is_flag=True, help="Show removed runtime")
 @click.option(
     "--page", type=int, default=DEFAULT_PAGE_IDX, help="Page number for tasks list"
 )
 @click.option(
     "--size", type=int, default=DEFAULT_PAGE_SIZE, help="Page size for tasks list"
@@ -294,15 +481,15 @@
     fullname: bool,
     show_removed: bool,
     page: int,
     size: int,
     filters: list,
 ) -> None:
     """
-    List Runtime
+    List Runtime of the specified project
 
     The filtering flag (-fl or --filter) format is a key=value pair or a flag.
     If there is more than one filter, then pass multiple flags.\n
     (e.g. --filter name=mnist --filter latest)
 
     \b
     The currently supported filters are:
@@ -395,35 +582,41 @@
 def _tag(runtime: str, tags: t.List[str], remove: bool, quiet: bool) -> None:
     RuntimeTermView(runtime).tag(tags, remove, quiet)
 
 
 @runtime_cmd.command(
     "activate",
     aliases=["actv"],
-    help="[Only Standalone]Activate python runtime environment for development",
+    help="",
 )
-@click.option("-u", "--uri", help="Runtime uri which has already been restored")
-@click.option("-p", "--path", help="User's runtime workdir")
-def _activate(uri: str, path: str) -> None:
-    if uri and path:
-        raise ExclusiveArgsError(f"only uri({uri}) or path({path}) can take effect")
+@click.argument("uri")
+@click.option(
+    "-f",
+    "--force-restore",
+    help="Force to restore runtime into the related snapshot workdir even the runtime has been restored",
+)
+def _activate(uri: str, force_restore: bool) -> None:
+    """
+    [Only Standalone]Activate python runtime environment for development
 
-    if not uri and not path:
-        raise MissingFieldError("uri or path is required.")
+    When the runtime has not been restored, activate command will restore runtime automatically.
 
-    RuntimeTermView.activate(path, uri)
+    URI: Runtime uri in the standalone instance
+    """
+    _uri = URI(uri, expected_type=URIType.RUNTIME)
+    RuntimeTermView.activate(_uri, force_restore)
 
 
 @runtime_cmd.command("lock")
 @click.argument("target_dir", default=".")
 @click.option(
     "-f",
-    "--yaml-name",
+    "--yaml-path",
     default=DefaultYAMLName.RUNTIME,
-    help=f"Runtime YAML file name, default is {DefaultYAMLName.RUNTIME}",
+    help=f"Runtime YAML file path, default is {DefaultYAMLName.RUNTIME} at the current working directory",
 )
 @optgroup.group(  # type: ignore
     "Python environment selectors",
     cls=MutuallyExclusiveOptionGroup,
     help="The selector of the python environment, default is the starwhale auto create env prefix path",
 )
 @optgroup.option("-n", "--env-name", default="", help="conda name")  # type: ignore
@@ -459,33 +652,33 @@
     "--no-cache",
     is_flag=True,
     help="Invalid the cached(installed) packages in the isolate env when env-lock is enabled, \
     only for auto-generated environments",
 )
 def _lock(
     target_dir: str,
-    yaml_name: str,
+    yaml_path: str,
     env_name: str,
     env_prefix_path: str,
     env_use_shell: bool,
     stdout: bool,
     include_editable: bool,
     include_local_wheel: bool,
     emit_pip_options: bool,
     no_cache: bool,
 ) -> None:
     """
     [Only Standalone]Lock Python venv or conda environment
 
-    TARGET_DIR: the runtime.yaml and local file dir, default is "."
+    TARGET_DIR: the lock files will store in the `target_dir` , default is "."
     """
 
     RuntimeTermView.lock(
         target_dir,
-        yaml_name,
+        Path(yaml_path),
         env_name,
         env_prefix_path,
         no_cache,
         stdout,
         include_editable,
         include_local_wheel,
         emit_pip_options,
```

### Comparing `starwhale-0.4.1/starwhale/core/runtime/model.py` & `starwhale-0.4.2/starwhale/core/runtime/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 
 import os
 import shutil
 import typing as t
 import platform
 import tempfile
 from abc import ABCMeta
+from enum import Enum, unique
 from pathlib import Path
 from collections import defaultdict
 
 import yaml
 import jinja2
 from fs import open_fs
 from loguru import logger
 from fs.copy import copy_fs, copy_file
+from fs.tarfs import TarFS
 from typing_extensions import Protocol
 
 from starwhale.utils import (
     docker,
     console,
     load_yaml,
     in_container,
@@ -91,25 +93,25 @@
     trunc_python_version,
     get_conda_prefix_path,
     check_valid_venv_prefix,
     get_user_python_version,
     check_valid_conda_prefix,
     get_python_version_by_bin,
     render_python_env_activate,
+    get_user_runtime_python_bin,
 )
 from starwhale.base.bundle import BaseBundle, LocalStorageBundleMixin
 from starwhale.utils.error import (
     FormatError,
     ExistedError,
     NotFoundError,
     NoSupportError,
     ConfigFormatError,
     MissingFieldError,
     ExclusiveArgsError,
-    FieldTypeOrValueError,
     UnExpectedConfigFieldError,
 )
 from starwhale.utils.progress import run_with_progress_bar
 from starwhale.base.bundle_copy import BundleCopy
 
 from .store import RuntimeStorage
 
@@ -122,14 +124,23 @@
 )
 
 _SUPPORT_CUDA = ["11.3", "11.4", "11.5", "11.6", "11.7"]
 _SUPPORT_CUDNN = {"8": {"support_cuda_versions": ["11.3", "11.4", "11.5", "11.6"]}}
 _SUPPORT_PYTHON_VERSIONS = ["3.7", "3.8", "3.9", "3.10", "3.11"]
 
 
+@unique
+class RuntimeInfoFilter(Enum):
+    basic = "basic"
+    runtime_yaml = "runtime_yaml"
+    manifest = "manifest"
+    lock = "lock"
+    all = "all"
+
+
 class DockerEnv(ASDictMixin):
     def __init__(self, **kwargs: t.Any):
         self.image = kwargs.get("image", "")
 
     def __str__(self) -> str:
         if self.image:
             return f"image:{self.image}"
@@ -648,34 +659,34 @@
             URIType.RUNTIME,
             force,
             dest_local_project_uri=dest_local_project_uri,
         )
         bc.do()
 
     @classmethod
-    def activate(cls, path: str = "", uri: str = "") -> None:
-        StandaloneRuntime.activate(path, uri)
+    def activate(cls, uri: URI, force_restore: bool = False) -> None:
+        StandaloneRuntime.activate(uri, force_restore)
 
     @classmethod
     def lock(
         cls,
-        target_dir: t.Union[str, Path],
-        yaml_name: str = DefaultYAMLName.RUNTIME,
+        target_dir: str | Path,
+        yaml_path: str | Path,
         env_name: str = "",
         env_prefix_path: str = "",
         no_cache: bool = False,
         stdout: bool = False,
         include_editable: bool = False,
         include_local_wheel: bool = False,
         emit_pip_options: bool = False,
         env_use_shell: bool = False,
-    ) -> str:
+    ) -> t.Tuple[str, t.Optional[Path]]:
         return StandaloneRuntime.lock(
             target_dir,
-            yaml_name,
+            yaml_path,
             env_name,
             env_prefix_path,
             no_cache,
             stdout,
             include_editable,
             include_local_wheel,
             emit_pip_options,
@@ -689,27 +700,100 @@
         push: bool = True,
         dry_run: bool = False,
         use_starwhale_builder: bool = False,
         reset_qemu_static: bool = False,
     ) -> None:
         raise NotImplementedError
 
+    def build_from_docker_image(self, image: str, runtime_name: str) -> None:
+        raise NotImplementedError
+
+    def build_from_python_env(
+        self,
+        runtime_name: str,
+        mode: str = "",
+        conda_name: str = "",
+        conda_prefix: str = "",
+        venv_prefix: str = "",
+        cuda: str = "",
+        cudnn: str = "",
+        arch: str = "",
+        download_all_deps: bool = False,
+        include_editable: bool = False,
+        include_local_wheel: bool = False,
+    ) -> None:
+        raise NotImplementedError
+
+    def build_from_runtime_yaml(
+        self,
+        workdir: str | Path,
+        yaml_path: str | Path,
+        download_all_deps: bool = False,
+        include_editable: bool = False,
+        include_local_wheel: bool = False,
+        no_cache: bool = False,
+        disable_env_lock: bool = False,
+        env_prefix_path: str = "",
+        env_name: str = "",
+        env_use_shell: bool = False,
+    ) -> None:
+        raise NotImplementedError
+
 
 class StandaloneRuntime(Runtime, LocalStorageBundleMixin):
     def __init__(self, uri: URI) -> None:
         super().__init__(uri)
         self.typ = InstanceType.STANDALONE
         self.store = RuntimeStorage(uri)
         self.tag = StandaloneTag(uri)
         self._manifest: t.Dict[str, t.Any] = {}
         self._version = uri.object.version
         self._detected_sw_version: str = ""
 
     def info(self) -> t.Dict[str, t.Any]:
-        return self._get_bundle_info()
+        ret: t.Dict[str, t.Any] = {}
+        if not self.store.bundle_path.exists():
+            return ret
+
+        ret["basic"] = {
+            "name": self.uri.object.name,
+            "uri": self.uri.full_uri,
+            "project": self.uri.project,
+            "snapshot_workdir": str(self.store.snapshot_workdir),
+            "bundle_path": str(self.store.bundle_path),
+        }
+
+        ret["basic"]["version"] = self.uri.object.version
+        ret["basic"]["tags"] = StandaloneTag(self.uri).list()
+
+        if self.store.snapshot_workdir.exists():
+            ret["manifest"] = self.store.manifest
+            ret["runtime_yaml"] = (
+                self.store.snapshot_workdir / DefaultYAMLName.RUNTIME
+            ).read_text()
+            ret["lock"] = {}
+            for fname in ret["manifest"]["environment"]["lock"]["files"]:
+                ret["lock"][os.path.basename(fname)] = (
+                    self.store.snapshot_workdir / "dependencies" / fname
+                ).read_text()
+        else:
+            with TarFS(str(self.store.bundle_path)) as tar:
+                with tar.open(DEFAULT_MANIFEST_NAME) as f:
+                    ret["manifest"] = yaml.safe_load(f)
+
+                with tar.open(DefaultYAMLName.RUNTIME) as f:
+                    ret["runtime_yaml"] = f.read()
+
+                ret["lock"] = {}
+                for fname in ret["manifest"]["environment"]["lock"]["files"]:
+                    fpath = os.path.join("dependencies", fname)
+                    with tar.open(fpath) as f:
+                        ret["lock"][os.path.basename(fpath)] = f.read()
+
+        return ret
 
     def list_tags(self) -> t.List[str]:
         return self.tag.list()
 
     def add_tags(self, tags: t.List[str], ignore_errors: bool = False) -> None:
         self.tag.add(tags, ignore_errors)
 
@@ -750,58 +834,134 @@
                     created_at=get_path_created_time(_bf.path),
                     size=_bf.path.stat().st_size,
                     tags=_bf.tags,
                 )
             )
         return _r
 
-    def build(  # type: ignore[override]
+    def build_from_docker_image(self, image: str, runtime_name: str) -> None:
+        # TODO: validate image format
+        workdir = Path(tempfile.mkdtemp(suffix="starwhale-runtime-build-"))
+        try:
+            config: t.Dict[str, t.Any] = dict(
+                name=runtime_name,
+                environment={
+                    "docker": {"image": image},
+                },
+            )
+            yaml_path = workdir / DefaultYAMLName.RUNTIME
+            ensure_file(yaml_path, yaml.dump(config))
+            self.build_from_runtime_yaml(
+                workdir=workdir,
+                yaml_path=yaml_path,
+                disable_env_lock=True,
+            )
+        finally:
+            empty_dir(workdir)
+
+    def build_from_python_env(
         self,
-        workdir: Path,
-        **kw: t.Any,
+        runtime_name: str,
+        mode: str = PythonRunEnv.VENV,
+        conda_name: str = "",
+        conda_prefix: str = "",
+        venv_prefix: str = "",
+        cuda: str = "",
+        cudnn: str = "",
+        arch: str = "",
+        download_all_deps: bool = False,
+        include_editable: bool = False,
+        include_local_wheel: bool = False,
+    ) -> None:
+        if conda_name or conda_prefix:
+            prefix_path = (
+                get_conda_prefix_path(conda_name) if conda_name else conda_prefix
+            )
+            if not check_valid_conda_prefix(prefix_path):
+                raise RuntimeError(f"Invalid conda prefix: {prefix_path}")
+
+            pybin = get_conda_pybin(prefix=prefix_path)
+            env_use_shell = False
+        elif venv_prefix:
+            if not check_valid_venv_prefix(venv_prefix):
+                raise RuntimeError(f"Invalid venv prefix: {venv_prefix}")
+            pybin = os.path.join(venv_prefix, "bin", "python3")
+            env_use_shell = False
+        else:
+            pybin = get_user_runtime_python_bin(mode)
+            env_use_shell = True
+
+        python_version = get_python_version_by_bin(pybin)
+        workdir = Path(tempfile.mkdtemp(suffix="starwhale-runtime-build-"))
+        try:
+            yaml_path = StandaloneRuntime.render_runtime_yaml(
+                workdir,
+                name=runtime_name,
+                mode=mode,
+                python_version=python_version,
+                cuda_version=cuda,
+                cudnn_version=cudnn,
+                arch=arch,
+            )
+
+            self.build_from_runtime_yaml(
+                workdir=workdir,
+                yaml_path=yaml_path,
+                download_all_deps=download_all_deps,
+                include_editable=include_editable,
+                include_local_wheel=include_local_wheel,
+                disable_env_lock=False,
+                env_name=conda_name,
+                env_prefix_path=conda_prefix or venv_prefix,
+                env_use_shell=env_use_shell,
+            )
+        finally:
+            empty_dir(workdir)
+
+    def build_from_runtime_yaml(
+        self,
+        workdir: str | Path,
+        yaml_path: str | Path,
+        download_all_deps: bool = False,
+        include_editable: bool = False,
+        include_local_wheel: bool = False,
+        no_cache: bool = False,
+        disable_env_lock: bool = False,
+        env_prefix_path: str = "",
+        env_name: str = "",
+        env_use_shell: bool = False,
     ) -> None:
-        yaml_name = kw.get("yaml_name", DefaultYAMLName.RUNTIME)
-        disable_env_lock = kw.get("disable_env_lock", False)
-        no_cache = kw.get("no_cache", False)
-        env_name = kw.get("env_name", "")
-        env_prefix_path = kw.get("env_prefix_path", "")
-        env_use_shell = kw.get("env_use_shell", False)
-        include_editable = kw.get("include_editable", False)
-        include_local_wheel = kw.get("include_local_wheel", False)
-        # TODO: tune for no runtime.yaml file
-        swrt_config = self._load_runtime_config(workdir / yaml_name)
+        workdir = Path(workdir)
+        yaml_path = Path(yaml_path)
+        swrt_config = self._load_runtime_config(yaml_path)
 
-        lock_files = []
+        lock_paths: t.List[Path] = []
         if not disable_env_lock:
             console.print(
-                f":alien: try to lock environment dependencies to {yaml_name}@{workdir} ..."
+                f":alien: try to lock environment dependencies to {workdir} ..."
             )
-            content = self.lock(
+            content, lock_fpath = self.lock(
                 target_dir=workdir,
-                yaml_name=yaml_name,
-                env_name=env_name,
-                env_prefix_path=env_prefix_path,
+                yaml_path=yaml_path,
                 no_cache=no_cache,
                 stdout=False,
                 include_editable=include_editable,
                 include_local_wheel=include_local_wheel,
+                env_name=env_name,
+                env_prefix_path=env_prefix_path,
                 env_use_shell=env_use_shell,
             )
             # try getting starwhale version
             for line in content.splitlines():
                 if line.startswith("starwhale=="):
                     self._detected_sw_version = line.split("==")[1].strip()
                     break
 
-            lock_fname = (
-                RuntimeLockFileType.CONDA
-                if swrt_config.mode == PythonRunEnv.CONDA
-                else RuntimeLockFileType.VENV
-            )
-            lock_files.append(f"{SW_AUTO_DIRNAME}/lock/{lock_fname}")
+            if lock_fpath is not None:
+                lock_paths.append(lock_fpath)
 
         operations = [
             (self._gen_version, 5, "gen version"),
             (self._prepare_snapshot, 5, "prepare snapshot"),
             (
                 self._dump_context,
                 5,
@@ -813,23 +973,23 @@
                 10,
                 "lock environment",
                 dict(
                     swrt_config=swrt_config,
                     env_prefix_path=env_prefix_path,
                     env_name=env_name,
                     env_use_shell=env_use_shell,
-                    lock_files=lock_files,
+                    lock_paths=lock_paths,
                 ),
             ),
             (
                 self._dump_dependencies,
                 50,
                 "dump python dependencies",
                 dict(
-                    gen_all_bundles=kw.get("gen_all_bundles", False),
+                    download_all_deps=download_all_deps,
                     deps=swrt_config.dependencies,
                     mode=swrt_config.mode,
                     include_editable=include_editable,
                     env_prefix_path=env_prefix_path,
                     env_name=env_name,
                 ),
             ),
@@ -841,17 +1001,16 @@
             ),
             (
                 self._copy_src,
                 20,
                 "dump src files:wheel, native files",
                 dict(
                     config=swrt_config,
-                    workdir=workdir,
-                    yaml_name=yaml_name,
-                    lock_files=lock_files,
+                    yaml_path=yaml_path,
+                    lock_paths=lock_paths,
                 ),
             ),
             (
                 self._render_manifest,
                 5,
                 "render manifest",
             ),
@@ -863,38 +1022,25 @@
     def _dump_context(self, config: RuntimeConfig) -> None:
         # TODO: refactor docker image in environment
         self._manifest["configs"] = config.configs.asdict()
 
     def _copy_src(
         self,
         config: RuntimeConfig,
-        workdir: Path,
-        yaml_name: str = DefaultYAMLName.RUNTIME,
-        lock_files: t.Optional[t.List[str]] = None,
+        yaml_path: Path,
+        lock_paths: t.Optional[t.List[Path]] = None,
     ) -> None:
-        lock_files = lock_files or []
-
-        conda_file_dups = set(config.dependencies._conda_files) & set(lock_files)
-        if conda_file_dups:
-            raise FieldTypeOrValueError(
-                f"conda files have used the auto-locked dependency files: {conda_file_dups}"
-            )
-
-        pip_file_dups = set(config.dependencies._pip_files) & set(lock_files)
-        if pip_file_dups:
-            raise FieldTypeOrValueError(
-                f"pip files have used the auto-locked dependency files:{pip_file_dups}"
-            )
-
-        workdir_fs = open_fs(str(workdir.resolve()))
+        workdir = yaml_path.parent.resolve()
+        yaml_name = yaml_path.name
+        workdir_fs = open_fs(str(workdir))
         snapshot_fs = open_fs(str(self.store.snapshot_workdir.resolve()))
-        copy_file(workdir_fs, yaml_name, snapshot_fs, yaml_name)
+        copy_file(workdir_fs, yaml_name, snapshot_fs, DefaultYAMLName.RUNTIME)
 
         self._manifest["artifacts"] = {
-            RuntimeArtifactType.RUNTIME: yaml_name,
+            RuntimeArtifactType.RUNTIME: DefaultYAMLName.RUNTIME,
             RuntimeArtifactType.WHEELS: [],
             RuntimeArtifactType.DEPEND: [],
             RuntimeArtifactType.FILES: [],
         }
 
         logger.info("[step:copy-wheels]start to copy wheels...")
         ensure_dir(self.store.snapshot_workdir / RuntimeArtifactType.WHEELS)
@@ -930,19 +1076,15 @@
             elif _src.is_file():
                 ensure_dir((self.store.snapshot_workdir / _dest).parent)
                 copy_file(workdir_fs, _f["src"], snapshot_fs, _dest)
 
         logger.info("[step:copy-deps]start to copy pip/conda requirement files")
         ensure_dir(self.store.snapshot_workdir / RuntimeArtifactType.DEPEND)
 
-        for _fname in (
-            config.dependencies._conda_files
-            + config.dependencies._pip_files
-            + lock_files
-        ):
+        for _fname in config.dependencies._conda_files + config.dependencies._pip_files:
             _fpath = workdir / _fname
             if not _fpath.exists():
                 logger.warning(f"not found dependencies: {_fpath}")
                 continue
 
             _dest = f"{RuntimeArtifactType.DEPEND}/{_fname.lstrip('/')}"
             ensure_dir((self.store.snapshot_workdir / _dest).parent)
@@ -950,14 +1092,34 @@
             copy_file(
                 workdir_fs,
                 _fname,
                 snapshot_fs,
                 _dest,
             )
 
+        lock_paths = lock_paths or []
+        for _fpath in lock_paths:
+            _fname = _fpath.name
+            _dest_name = f"{RuntimeArtifactType.DEPEND}/{SW_AUTO_DIRNAME}/lock/{_fname.lstrip('/')}"
+            _dest_path = self.store.snapshot_workdir / _dest_name
+            if _dest_path.exists():
+                raise RuntimeError(
+                    f"{_dest_name} has already been added into the runtime.yaml, failed to copy the auto-lock file"
+                )
+
+            ensure_dir(_dest_path.parent)
+            self._manifest["artifacts"][RuntimeArtifactType.DEPEND].append(_dest_name)
+
+            copy_file(
+                open_fs(str(_fpath.parent)),
+                _fname,
+                snapshot_fs,
+                _dest_name,
+            )
+
     def _dump_base_image(self, config: RuntimeConfig) -> None:
         # prefer using image configured in runtime.yaml
         base_image = config.environment.docker.image
 
         if not base_image:
             _repo = os.environ.get(ENV_SW_IMAGE_REPO, DEFAULT_IMAGE_REPO)
             _tag = config._starwhale_version or LATEST_TAG
@@ -981,20 +1143,20 @@
 
     def _lock_environment(
         self,
         swrt_config: RuntimeConfig,
         env_prefix_path: str = "",
         env_name: str = "",
         env_use_shell: bool = False,
-        lock_files: t.Optional[t.List[str]] = None,
+        lock_paths: t.Optional[t.List[Path]] = None,
     ) -> None:
         console.print(":bee: dump environment info...")
         sh_py_env = guess_current_py_env()
         sh_py_ver = get_user_python_version(sh_py_env)
-        lock_files = lock_files or []
+        lock_paths = lock_paths or []
 
         self._manifest["environment"] = self._manifest.get("environment") or {}
 
         self._manifest["environment"].update(
             {
                 "lock": {
                     "starwhale_version": self._detected_sw_version or STARWHALE_VERSION,
@@ -1004,48 +1166,48 @@
                         "python_version": sh_py_ver,
                         "use_conda": is_conda(),
                         "use_venv": is_venv(),
                     },
                     "env_prefix_path": env_prefix_path,
                     "env_name": env_name,
                     "env_use_shell": env_use_shell,
-                    "files": lock_files,
+                    "files": [f"{SW_AUTO_DIRNAME}/lock/{p.name}" for p in lock_paths],
                 },
-                "auto_lock_dependencies": bool(lock_files),
+                "auto_lock_dependencies": bool(lock_paths),
                 "python": swrt_config.environment.python,
                 "arch": swrt_config.environment.arch,
                 "mode": swrt_config.mode,
             }
         )
 
     def _dump_dependencies(
         self,
         mode: str = PythonRunEnv.AUTO,
-        gen_all_bundles: bool = False,
+        download_all_deps: bool = False,
         deps: t.Optional[Dependencies] = None,
         include_editable: bool = False,
         env_prefix_path: str = "",
         env_name: str = "",
     ) -> None:
-        console.print("dump dependencies info...")
+        console.print(":bagel: dump dependencies info...")
         deps = deps or Dependencies()
 
         self._manifest["dependencies"] = {
             "raw_deps": deps.flatten_raw_deps(),
             "local_packaged_env": False,
             # compatibility with starwhale <= 0.3.0
             "pip_pkgs": deps._pip_pkgs,
             "conda_pkgs": deps._conda_pkgs,
             "pip_files": deps._pip_files,
             "conda_files": deps._conda_files,
         }
 
         logger.info("[step:dep]finish dump dep")
 
-        if gen_all_bundles:
+        if download_all_deps:
             packaged = package_python_env(
                 export_dir=self.store.export_dir,
                 mode=mode,
                 env_prefix_path=env_prefix_path,
                 env_name=env_name,
                 include_editable=include_editable,
             )
@@ -1238,32 +1400,31 @@
             activate_python_env(
                 mode=mode,
                 identity=str(isolated_env_dir.absolute()),
                 interactive=interactive,
             )
 
     @classmethod
-    def activate(cls, path: str = "", uri: str = "") -> None:
-        if uri:
-            _uri = URI(uri, expected_type=URIType.RUNTIME)
-            if _uri.instance_type != InstanceType.STANDALONE:
-                raise NoSupportError(f"{uri} is not the standalone instance")
-
-            _rt = StandaloneRuntime(_uri)
-            mode = load_yaml(_rt.store.manifest_path)["environment"]["mode"]
-            prefix_path = _rt.store.export_dir / mode
-        elif path:
-            # TODO: support non-standard runtime.yaml name
-            _rf = Path(path) / DefaultYAMLName.RUNTIME
-            _config = RuntimeConfig.create_by_yaml(_rf)
-            mode = _config.mode
-            prefix_path = Path(path) / f".{mode}"
-        else:
-            raise Exception("No uri or path to activate")
+    def activate(cls, uri: URI, force_restore: bool = False) -> None:
+        if uri.instance_type != InstanceType.STANDALONE:
+            raise NoSupportError(f"{uri} is not the standalone instance")
+
+        _rt = StandaloneRuntime(uri)
+        workdir = _rt.store.snapshot_workdir
+        if not workdir.exists():
+            console.print(f":package: extract swrt into {workdir}")
+            _rt.extract(force=True, target=workdir)
+
+        mode = load_yaml(_rt.store.manifest_path)["environment"]["mode"]
+        prefix_path = _rt.store.export_dir / mode
+        if not prefix_path.exists() or force_restore:
+            console.print(f":safety_vest: restore runtime into {workdir}")
+            cls.restore(workdir)
 
+        console.print(f":carrot: activate the current shell for the runtime uri: {uri}")
         activate_python_env(
             mode=mode, identity=str(prefix_path.resolve()), interactive=True
         )
 
     @classmethod
     def _ensure_isolated_python_env(
         cls,
@@ -1296,44 +1457,47 @@
             ensure_dir(env_dir)
 
         cls._setup_python_env(env_dir, mode=mode, python_version=python_version)
 
     @classmethod
     def lock(
         cls,
-        target_dir: t.Union[str, Path],
-        yaml_name: str = DefaultYAMLName.RUNTIME,
+        target_dir: str | Path,
+        yaml_path: str | Path,
         env_name: str = "",
         env_prefix_path: str = "",
         no_cache: bool = False,
         stdout: bool = False,
         include_editable: bool = False,
         include_local_wheel: bool = False,
         emit_pip_options: bool = False,
         env_use_shell: bool = False,
-    ) -> str:
-        """
-        Install dependencies and save or print lock file
-        :param target_dir: runtime work directory which contains the configured runtime.yaml
-        :param yaml_name: runtime config file name
-        :param env_name: conda environment name (used by conda env)
-        :param env_prefix_path: python env prefix path (used by both venv and conda)
-        :param no_cache: invalid all pkgs installed
-        :param stdout: just print the lock info into stdout without saving lock file
-        :param include_editable: include the editable pkg (only for venv)
-        :param include_local_wheel: include local wheel pkg (only for venv)
-        :param emit_pip_options: use user's pip configuration when freeze pkgs (only for venv)
-        :param env_use_shell: automatically detect env in current shell session
-        :return: the lock file content
+    ) -> t.Tuple[str, t.Optional[Path]]:
+        """Install dependencies and save or print lock file
+
+        Arguments:
+            workdir: runtime work directory which contains the configured runtime.yaml
+            yaml_name: runtime config file name
+            env_name: conda environment name (used by conda env)
+            env_prefix_path: python env prefix path (used by both venv and conda)
+            no_cache: invalid all pkgs installed
+            stdout: just print the lock info into stdout without saving lock file
+            include_editable: include the editable pkg (only for venv)
+            include_local_wheel: include local wheel pkg (only for venv)
+            emit_pip_options: use user's pip configuration when freeze pkgs (only for venv)
+            env_use_shell: automatically detect env in current shell session
+
+        Returns:
+            the lock file content(str) and the lock file path(Path)
         """
-        target_dir = Path(target_dir)
-        runtime_fpath = target_dir / yaml_name
-        if not runtime_fpath.exists():
-            raise NotFoundError(runtime_fpath)
-        runtime_yaml = load_yaml(runtime_fpath)
+        yaml_path = Path(yaml_path)
+        if not yaml_path.exists():
+            raise NotFoundError(yaml_path)
+        runtime_yaml = load_yaml(yaml_path)
+
         mode = runtime_yaml.get("mode", PythonRunEnv.VENV)
         expected_pyver = str(runtime_yaml.get("environment", {}).get("python", ""))
         _, temp_lock_path = tempfile.mkstemp(prefix="starwhale-lock-")
         console.print(f":butterfly: lock dependencies at mode {mode}")
 
         set_args = list(filter(bool, (env_name, env_prefix_path, env_use_shell)))
         if len(set_args) >= 2:
@@ -1348,22 +1512,22 @@
                 )
             prefix_path = get_conda_prefix_path(env_name)
         elif env_use_shell:
             prefix_path = get_base_prefix(mode)
         elif env_prefix_path:
             prefix_path = env_prefix_path
         else:
-            _sw_auto_path = target_dir / SW_AUTO_DIRNAME / mode
+            _sw_auto_path = Path(target_dir) / SW_AUTO_DIRNAME / mode
             cls._ensure_isolated_python_env(
                 _sw_auto_path, expected_pyver, mode, no_cache
             )
             prefix_path = str(_sw_auto_path)
 
         cls._install_dependencies_with_runtime_yaml(
-            workdir=target_dir,
+            src_dir=yaml_path.parent,
             runtime_yaml=runtime_yaml,
             env_dir=prefix_path,
             skip_deps=[DependencyType.NATIVE_FILE],
         )
 
         if mode == PythonRunEnv.CONDA:
             if not check_valid_conda_prefix(prefix_path):
@@ -1399,89 +1563,73 @@
         with open(temp_lock_path) as f:
             content = f.read()
 
         if stdout:
             console.rule("dependencies lock")
             console.print(content)
             os.unlink(temp_lock_path)
+            return content, None
         else:
             dest_fname = (
                 RuntimeLockFileType.CONDA
                 if mode == PythonRunEnv.CONDA
                 else RuntimeLockFileType.VENV
             )
             lock_dir = Path(target_dir) / SW_AUTO_DIRNAME / "lock"
             ensure_dir(lock_dir)
             dest_fpath = lock_dir / dest_fname
             shutil.move(temp_lock_path, dest_fpath)
             console.print(f":mouse: dump lock file: {dest_fpath}")
-
-        return content
+            return content, dest_fpath
 
     @staticmethod
     def render_runtime_yaml(
         workdir: t.Union[Path, str],
         name: str,
         mode: str,
         python_version: str = "",
         pkgs: t.Optional[t.List[str]] = None,
         force: bool = False,
         auto_inject_sw: bool = True,
-        cuda_version: t.Optional[str] = None,
-    ) -> None:
+        cuda_version: str = "",
+        cudnn_version: str = "",
+        arch: str = "",
+    ) -> Path:
         workdir = Path(workdir)
         _rm = workdir / DefaultYAMLName.RUNTIME
-
-        if python_version == "":
-            python_version = get_python_version()
-
         if _rm.exists() and not force:
             raise ExistedError(f"{_rm} was already existed")
 
-        if mode == PythonRunEnv.CONDA:
-            lock_fname = RuntimeLockFileType.CONDA
-            lock_content = f"name: {name}"
-        else:
-            lock_fname = RuntimeLockFileType.VENV
-            lock_content = ""
-
-        lock_fpath = workdir / lock_fname
-        if not lock_fpath.exists():
-            ensure_file(lock_fpath, content=lock_content)
-
         pkgs = pkgs or []
         if auto_inject_sw and not any(
             [p.strip().startswith(SW_PYPI_PKG_NAME) for p in pkgs]
         ):
             sw_pkg = SW_PYPI_PKG_NAME
             if STARWHALE_VERSION and STARWHALE_VERSION != SW_DEV_DUMMY_VERSION:
                 sw_pkg = f"{sw_pkg}=={STARWHALE_VERSION}"
             pkgs.append(sw_pkg)
-
         pkgs = [p.strip() for p in pkgs if p.strip()]
 
-        ensure_dir(workdir)
         config: t.Dict[str, t.Any] = dict(
             name=name,
             mode=mode,
             environment={
-                "python": python_version,
-                "arch": SupportArch.NOARCH,
+                "python": python_version or get_python_version(),
+                "arch": arch or SupportArch.NOARCH,
                 "os": SupportOS.UBUNTU,
+                "cuda": cuda_version,
+                "cudnn": cudnn_version,
             },
             dependencies=[
-                lock_fname,
                 {"pip": pkgs},
             ],
             api_version=RUNTIME_API_VERSION,
         )
-        if cuda_version is not None:
-            config["environment"]["cuda"] = cuda_version
-
-        ensure_file(_rm, yaml.safe_dump(config, default_flow_style=False))
+        ensure_file(_rm, yaml.safe_dump(config, default_flow_style=False), parents=True)
+        return _rm
 
     def dockerize(
         self,
         tags: t.Optional[t.List[str]] = None,
         platforms: t.Optional[t.List[str]] = None,
         push: bool = True,
         dry_run: bool = False,
@@ -1659,15 +1807,15 @@
             ]
         )
 
         run_with_progress_bar("runtime restore...", operations)
 
     @staticmethod
     def _install_dependencies_with_runtime_yaml(
-        workdir: Path,
+        src_dir: Path,
         runtime_yaml: t.Any,
         env_dir: t.Union[Path, str],
         skip_deps: t.Optional[t.List[DependencyType]] = None,
     ) -> None:
         env_dir = Path(env_dir)
 
         mode = runtime_yaml.get("mode", PythonRunEnv.VENV)
@@ -1681,15 +1829,15 @@
             if dep.kind in skip_deps:
                 logger.debug(f"skip {dep} to install")
                 continue
 
             _func = (
                 dep.conda_install if PythonRunEnv.CONDA == mode else dep.venv_install
             )
-            _func(workdir, env_dir, configs)
+            _func(src_dir, env_dir, configs)
 
     @staticmethod
     def _install_dependencies_within_restore(
         workdir: Path,
         mode: str,
         deps: t.Dict,
         configs: t.Dict,
@@ -1819,10 +1967,7 @@
         filter_dict: t.Optional[t.Dict[str, t.Any]] = None,
     ) -> t.Tuple[t.Dict[str, t.Any], t.Dict[str, t.Any]]:
         filter_dict = filter_dict or {}
         crm = CloudRequestMixed()
         return crm._fetch_bundle_all_list(
             project_uri, URIType.RUNTIME, page, size, filter_dict
         )
-
-    def build(self, *args: t.Any, **kwargs: t.Any) -> None:
-        raise NoSupportError("no support build runtime in the cloud instance")
```

### Comparing `starwhale-0.4.1/starwhale/core/runtime/process.py` & `starwhale-0.4.2/starwhale/core/runtime/process.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from starwhale.utils.error import NotFoundError, NoSupportError
 from starwhale.utils.process import check_call
 
 from .model import StandaloneRuntime
 
 
 class Process:
-
     EnvInActivatedProcess = "SW_RUNTIME_ACTIVATED_PROCESS"
 
     def __init__(
         self,
         prefix_path: t.Union[Path, str],
         target: t.Callable,
         args: t.Tuple = (),
```

### Comparing `starwhale-0.4.1/starwhale/core/runtime/store.py` & `starwhale-0.4.2/starwhale/core/runtime/store.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/core/runtime/template/Dockerfile.tmpl` & `starwhale-0.4.2/starwhale/core/runtime/template/Dockerfile.tmpl`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/core/runtime/view.py` & `starwhale-0.4.2/starwhale/core/runtime/view.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,42 @@
+from __future__ import annotations
+
 import os
 import typing as t
 from pathlib import Path
 
-import click
+from rich.pretty import Pretty
+from rich.syntax import Syntax
 
 from starwhale.utils import console, load_yaml, pretty_bytes, in_production
 from starwhale.consts import (
     PythonRunEnv,
-    DefaultYAMLName,
     DEFAULT_PAGE_IDX,
     DEFAULT_PAGE_SIZE,
     STANDALONE_INSTANCE,
 )
 from starwhale.base.uri import URI
 from starwhale.base.type import URIType, InstanceType
 from starwhale.base.view import BaseTermView
-from starwhale.utils.venv import get_python_version
-from starwhale.utils.error import NoSupportError
+from starwhale.utils.venv import get_venv_env, get_conda_env, get_python_run_env
+from starwhale.utils.error import NotFoundError, NoSupportError, ExclusiveArgsError
 from starwhale.utils.config import SWCliConfigMixed
 
-from .model import Runtime, _SUPPORT_CUDA, StandaloneRuntime, _SUPPORT_PYTHON_VERSIONS
+from .model import Runtime, RuntimeInfoFilter, StandaloneRuntime
 
 
 class RuntimeTermView(BaseTermView):
-    def __init__(self, runtime_uri: str) -> None:
+    def __init__(self, runtime_uri: str | URI) -> None:
         super().__init__()
 
-        self.raw_uri = runtime_uri
-        self.uri = URI(runtime_uri, expected_type=URIType.RUNTIME)
+        if isinstance(runtime_uri, URI):
+            self.uri = runtime_uri
+        else:
+            self.uri = URI(runtime_uri, expected_type=URIType.RUNTIME)
+
         self.runtime = Runtime.get_runtime(self.uri)
 
     @BaseTermView._simple_action_print
     def remove(self, force: bool = False) -> t.Tuple[bool, str]:
         return self.runtime.remove(force)
 
     @BaseTermView._simple_action_print
@@ -42,22 +47,58 @@
     @BaseTermView._header
     def history(self, fullname: bool = False) -> t.List[t.Dict[str, t.Any]]:
         fullname = fullname or self.uri.instance_type == InstanceType.CLOUD
         return self._print_history(
             title="Runtime History", history=self.runtime.history(), fullname=fullname
         )
 
-    @BaseTermView._header
-    def info(self, fullname: bool = False) -> None:
-        self._print_info(self.runtime.info(), fullname=fullname)
+    def info(
+        self,
+        output_filter: RuntimeInfoFilter = RuntimeInfoFilter.basic,
+    ) -> None:
+        info = self.runtime.info()
+        if not info:
+            console.print(
+                f":anguished_face: No runtime info found: {self.uri}", style="red"
+            )
+            return
+
+        basic_content = Pretty(info["basic"], expand_all=True)
+        runtime_content = Syntax(
+            info.get("runtime_yaml", ""), "yaml", theme="ansi_dark"
+        )
+        manifest_content = Pretty(info.get("manifest", {}), expand_all=True)
+        _locks = []
+        for fname, content in info.get("lock", {}).items():
+            _locks.append(f"#lock file: {fname}")
+            _locks.append(content)
+        lock_content = "\n".join(_locks)
+
+        if output_filter == RuntimeInfoFilter.basic:
+            console.print(basic_content)
+        elif output_filter == RuntimeInfoFilter.runtime_yaml:
+            console.print(runtime_content)
+        elif output_filter == RuntimeInfoFilter.lock:
+            console.print(lock_content)
+        elif output_filter == RuntimeInfoFilter.manifest:
+            console.print(manifest_content)
+        else:
+            console.rule("[green bold] Runtime Basic Info")
+            console.print(basic_content)
+            console.rule("[green bold] runtime.yaml")
+            console.print(runtime_content)
+            console.rule("[green bold] _manifest.yaml")
+            console.print(manifest_content)
+            console.rule("[green bold] Runtime Lock Files")
+            console.print(lock_content)
 
     @classmethod
     @BaseTermView._only_standalone
-    def activate(cls, path: str = "", uri: str = "") -> None:
-        Runtime.activate(path, uri)
+    def activate(cls, uri: URI, force_restore: bool = False) -> None:
+        Runtime.activate(uri, force_restore)
 
     @BaseTermView._only_standalone
     def dockerize(
         self,
         tags: t.List[str],
         push: bool,
         platforms: t.List[str],
@@ -74,129 +115,153 @@
             reset_qemu_static=reset_qemu_static,
         )
 
     @classmethod
     @BaseTermView._only_standalone
     def lock(
         cls,
-        target_dir: str,
-        yaml_name: str = DefaultYAMLName.RUNTIME,
+        target_dir: str | Path,
+        yaml_path: str | Path,
         env_name: str = "",
         env_prefix_path: str = "",
         no_cache: bool = False,
         stdout: bool = False,
         include_editable: bool = False,
         include_local_wheel: bool = False,
         emit_pip_options: bool = False,
         env_use_shell: bool = False,
     ) -> None:
         Runtime.lock(
             target_dir=target_dir,
-            yaml_name=yaml_name,
+            yaml_path=yaml_path,
             env_name=env_name,
             env_prefix_path=env_prefix_path,
             stdout=stdout,
             no_cache=no_cache,
             include_editable=include_editable,
             include_local_wheel=include_local_wheel,
             emit_pip_options=emit_pip_options,
             env_use_shell=env_use_shell,
         )
 
     @classmethod
     @BaseTermView._only_standalone
-    def build(
+    def build_from_docker_image(
+        cls, image: str, runtime_name: str = "", project: str = ""
+    ) -> None:
+        runtime_name = runtime_name or image.split(":")[0].split("/")[-1]
+        runtime_uri = cls.prepare_build_bundle(
+            project=project, bundle_name=runtime_name, typ=URIType.RUNTIME
+        )
+
+        rt = Runtime.get_runtime(runtime_uri)
+        rt.build_from_docker_image(image=image, runtime_name=runtime_name)
+
+    @classmethod
+    @BaseTermView._only_standalone
+    def build_from_python_env(
         cls,
-        workdir: t.Union[str, Path],
+        runtime_name: str = "",
+        conda_name: str = "",
+        conda_prefix: str = "",
+        venv_prefix: str = "",
         project: str = "",
-        yaml_name: str = DefaultYAMLName.RUNTIME,
-        gen_all_bundles: bool = False,
+        cuda: str = "",
+        cudnn: str = "",
+        arch: str = "",
+        download_all_deps: bool = False,
         include_editable: bool = False,
         include_local_wheel: bool = False,
-        disable_env_lock: bool = False,
-        no_cache: bool = False,
-        env_prefix_path: str = "",
-        env_name: str = "",
-        env_use_shell: bool = False,
     ) -> URI:
-        workdir = Path(workdir)
-        yaml_fpath = workdir / yaml_name
-        if not yaml_fpath.exists():
-            click.confirm(
-                f"Do you want to render {yaml_name}@{workdir.absolute()}?",
-                abort=True,
-            )
-            mode = click.prompt(
-                "Choose python env:",
-                type=click.Choice([PythonRunEnv.VENV, PythonRunEnv.CONDA]),
-                default=PythonRunEnv.VENV,
-            )
-            _default_python_version = get_python_version()
-            python_version = click.prompt(
-                "Choose python version:",
-                type=click.Choice(_SUPPORT_PYTHON_VERSIONS),
-                default=_default_python_version,
+        set_args = list(filter(bool, (conda_name, conda_prefix, venv_prefix)))
+        if len(set_args) >= 2:
+            raise ExclusiveArgsError(
+                f"conda_prefix({conda_prefix}), conda_name({conda_name}), venv_prefix({venv_prefix}) are the mutex args."
             )
 
-            pkgs_input = click.prompt(
-                "Input python dependencies, split by the comma",
-                type=str,
-                default="",
-            )
+        if conda_name:
+            mode = PythonRunEnv.CONDA
+            candidate_runtime_name = conda_name
+        elif conda_prefix:
+            mode = PythonRunEnv.CONDA
+            candidate_runtime_name = conda_prefix
+        elif venv_prefix:
+            mode = PythonRunEnv.VENV
+            candidate_runtime_name = venv_prefix
+        else:
+            mode = get_python_run_env()
+            candidate_runtime_name = (
+                get_conda_env() if mode == PythonRunEnv.CONDA else get_venv_env()
+            ) or "default"
+
+        if runtime_name == "":
+            runtime_name = candidate_runtime_name.strip("/").split("/")[-1]
+
+        runtime_uri = cls.prepare_build_bundle(
+            project=project, bundle_name=runtime_name, typ=URIType.RUNTIME
+        )
+        rt = Runtime.get_runtime(runtime_uri)
+        rt.build_from_python_env(
+            runtime_name=runtime_name,
+            mode=mode,
+            conda_name=conda_name,
+            conda_prefix=conda_prefix,
+            venv_prefix=venv_prefix,
+            cuda=cuda,
+            cudnn=cudnn,
+            arch=arch,
+            download_all_deps=download_all_deps,
+            include_editable=include_editable,
+            include_local_wheel=include_local_wheel,
+        )
+        return runtime_uri
 
-            if click.confirm("Do you want to enable cuda?"):
-                cuda_version = click.prompt(
-                    "Choose cuda version:",
-                    type=click.Choice(_SUPPORT_CUDA),
-                    default="11.4",
-                )
-            else:
-                cuda_version = None
-
-            StandaloneRuntime.render_runtime_yaml(
-                workdir=workdir,
-                name=workdir.absolute().name,
-                mode=mode,
-                python_version=python_version,
-                pkgs=pkgs_input.split(","),
-                force=True,
-                auto_inject_sw=True,
-                cuda_version=cuda_version,
-            )
+    @classmethod
+    @BaseTermView._only_standalone
+    def build_from_runtime_yaml(
+        cls,
+        workdir: str | Path,
+        yaml_path: str | Path,
+        runtime_name: str = "",
+        project: str = "",
+        download_all_deps: bool = False,
+        include_editable: bool = False,
+        include_local_wheel: bool = False,
+        no_cache: bool = False,
+        disable_env_lock: bool = False,
+    ) -> URI:
+        workdir = Path(workdir)
+        yaml_path = Path(yaml_path)
 
-            click.confirm(
-                f"{yaml_name} has been generated, do you want to continue build?",
-                abort=True,
-            )
+        if not yaml_path.exists():
+            raise NotFoundError(f"not found runtime yaml:{yaml_path}")
+        _config = load_yaml(yaml_path)
+        runtime_name = runtime_name or _config["name"]
 
-        _config = load_yaml(yaml_fpath)
         _runtime_uri = cls.prepare_build_bundle(
-            project=project, bundle_name=_config.get("name"), typ=URIType.RUNTIME
+            project=project, bundle_name=runtime_name, typ=URIType.RUNTIME
         )
         if include_editable:
             console.print(
                 ":bell: [red bold]runtime will include pypi editable package[/] :bell:"
             )
         else:
             console.print(
                 ":bird: [red bold]runtime will ignore pypi editable package[/]"
             )
 
         _rt = Runtime.get_runtime(_runtime_uri)
-        _rt.build(
-            workdir=Path(workdir),
-            yaml_name=yaml_name,
-            gen_all_bundles=gen_all_bundles,
+        _rt.build_from_runtime_yaml(
+            workdir=workdir,
+            yaml_path=yaml_path,
+            download_all_deps=download_all_deps,
             include_editable=include_editable,
             include_local_wheel=include_local_wheel,
-            disable_env_lock=disable_env_lock,
             no_cache=no_cache,
-            env_prefix_path=env_prefix_path,
-            env_name=env_name,
-            env_use_shell=env_use_shell,
+            disable_env_lock=disable_env_lock,
         )
         return _runtime_uri
 
     @BaseTermView._only_standalone
     def extract(self, force: bool = False, target: t.Union[str, Path] = "") -> None:
         console.print(":oncoming_police_car: try to extract ...")
         path = self.runtime.extract(force, target)
@@ -342,17 +407,30 @@
     ) -> None:
         filters = filters or []
         _data, _pager = super().list(
             project_uri, fullname, show_removed, page, size, filters
         )
         cls.pretty_json(_data)
 
-    def info(self, fullname: bool = False) -> None:
-        _data = self.get_info_data(self.runtime.info(), fullname=fullname)
-        self.pretty_json(_data)
+    def info(
+        self,
+        output_filter: RuntimeInfoFilter = RuntimeInfoFilter.basic,
+    ) -> None:
+        info = self.runtime.info()
+
+        if output_filter == RuntimeInfoFilter.basic:
+            info = {"basic": info.get("basic", {})}
+        elif output_filter == RuntimeInfoFilter.lock:
+            info = {"lock": info.get("lock", {})}
+        elif output_filter == RuntimeInfoFilter.manifest:
+            info = {"manifest": info.get("manifest", {})}
+        elif output_filter == RuntimeInfoFilter.runtime_yaml:
+            info = {"runtime_yaml": info.get("runtime_yaml", "")}
+
+        self.pretty_json(info)
 
     def history(self, fullname: bool = False) -> None:
         fullname = fullname or self.uri.instance_type == InstanceType.CLOUD
         _data = BaseTermView.get_history_data(
             history=self.runtime.history(), fullname=fullname
         )
         self.pretty_json(_data)
```

### Comparing `starwhale-0.4.1/starwhale/integrations/pytorch/dataset.py` & `starwhale-0.4.2/starwhale/integrations/pytorch/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,17 +62,17 @@
 
         self.drop_index = drop_index
 
     def __iter__(self) -> t.Iterator:
         _t = self.transform
         for row in self.dataset:
             if self.drop_index:
-                yield _t(row.data)
+                yield _t(row.features)
             else:
-                yield _t(row.index), _t(row.data)
+                yield _t(row.index), _t(row.features)
 
     def __len__(self) -> int:
         return len(self.dataset)
 
     def __str__(self) -> str:
         return f"TorchIterableDataset from Starwhale Dataset: {self.dataset}, drop_index:{self.drop_index}, transform: {self.transform}"
```

### Comparing `starwhale-0.4.1/starwhale/integrations/tensorflow/dataset.py` & `starwhale-0.4.2/starwhale/integrations/tensorflow/dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -94,22 +94,22 @@
         )
 
 
 def to_tf_dataset(dataset: Dataset, drop_index: bool = True) -> tf.data.Dataset:
     def _generator() -> t.Generator:
         for row in dataset:
             if drop_index:
-                yield _transform(row.data)
+                yield _transform(row.features)
             else:
-                yield _transform(row.index), _transform(row.data)
+                yield _transform(row.index), _transform(row.features)
 
     def _make_signature() -> t.Any:
         row = dataset.fetch_one()
         signature = []
         if not drop_index:
             signature.append(_inspect_spec(row.index))
-            return _inspect_spec(row.index), _inspect_spec(row.data)
-        return _inspect_spec(row.data)
+            return _inspect_spec(row.index), _inspect_spec(row.features)
+        return _inspect_spec(row.features)
 
     return tf.data.Dataset.from_generator(
         _generator, output_signature=_make_signature()
     )
```

### Comparing `starwhale-0.4.1/starwhale/mngt/__init__.py` & `starwhale-0.4.2/starwhale/mngt/__init__.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/utils/__init__.py` & `starwhale-0.4.2/starwhale/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/utils/cli.py` & `starwhale-0.4.2/starwhale/utils/cli.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/utils/config.py` & `starwhale-0.4.2/starwhale/utils/config.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/utils/debug.py` & `starwhale-0.4.2/starwhale/utils/debug.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/utils/dict.py` & `starwhale-0.4.2/starwhale/utils/dict.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/utils/docker.py` & `starwhale-0.4.2/starwhale/utils/docker.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/utils/error.py` & `starwhale-0.4.2/starwhale/utils/error.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/utils/fs.py` & `starwhale-0.4.2/starwhale/utils/fs.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/utils/http.py` & `starwhale-0.4.2/starwhale/utils/http.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/utils/load.py` & `starwhale-0.4.2/starwhale/utils/load.py`

 * *Files 15% similar despite different names*

```diff
@@ -51,44 +51,17 @@
             sys.path[:] = prev_paths
         raise
 
     return _obj
 
 
 def load_module(module: str, path: Path) -> t.Any:
-    """
-    load module from path
-    :param module: module name
-    :param path: abs path
-    :return: module
-    """
     workdir_path = str(path.absolute())
-    # add module path to sys path
+
     external_paths = [workdir_path]
     for _path in external_paths[::-1]:
         if _path not in sys.path:
             logger.debug(f"insert sys.path: '{_path}'")
             sys.path.insert(0, _path)
             pkg_resources.working_set.add_entry(_path)
 
     return importlib.import_module(module, package=workdir_path)
-
-
-def load_cls(module: str, cls_str: str) -> t.Any:
-    _cls = getattr(module, cls_str, None)
-    if not _cls:
-        raise ModuleNotFoundError(f"class:{cls_str} from module:{module}")
-    return _cls
-
-
-def get_func_from_object(obj: t.Any, func_str: str) -> t.Any:
-    _func = getattr(obj, func_str, None)
-    if not _func:
-        raise ModuleNotFoundError(f"function:{func_str} from object:{obj}")
-    return _func
-
-
-def get_func_from_module(module: str, func_str: str) -> t.Any:
-    _func = getattr(module, func_str, None)
-    if not _func:
-        raise ModuleNotFoundError(f"function:{func_str} from module:{module}")
-    return _func
```

### Comparing `starwhale-0.4.1/starwhale/utils/log.py` & `starwhale-0.4.2/starwhale/utils/log.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/utils/process.py` & `starwhale-0.4.2/starwhale/utils/process.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/utils/progress.py` & `starwhale-0.4.2/starwhale/utils/progress.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/utils/retry.py` & `starwhale-0.4.2/starwhale/utils/retry.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/utils/venv.py` & `starwhale-0.4.2/starwhale/utils/venv.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale/utils/venv_pack.py` & `starwhale-0.4.2/starwhale/utils/venv_pack.py`

 * *Files identical despite different names*

### Comparing `starwhale-0.4.1/starwhale.egg-info/PKG-INFO` & `starwhale-0.4.2/starwhale.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starwhale
-Version: 0.4.1
+Version: 0.4.2
 Summary: An MLOps Platform for Model Evaluation
 Home-page: https://github.com/star-whale/starwhale
 Author: Starwhale Team
 Author-email: developer@starwhale.ai
 License: Apache License 2.0
 Keywords: MLOps,AI,Starwhale,Model Evaluation
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -153,15 +153,14 @@
     > extra-index-url = https://pypi.doubanio.com/simple
     > ```
 
     ```bash
     swcli runtime build example/runtime/pytorch
     swcli runtime list
     swcli runtime info pytorch/version/latest
-    swcli runtime restore pytorch/version/latest
     ```
 
 - 🍞 **STEP4**: Building a model
 
   - Download pre-trained model file:
 
     ```bash
@@ -173,15 +172,15 @@
     ```
 
   - [Code Example]Write some code with Starwhale Python SDK. Complete code is [here](https://github.com/star-whale/starwhale/blob/main/example/mnist/mnist/evaluator.py).
 
     ```python
     import typing as t
     import torch
-    from starwhale import Image, PipelineHandler, PPLResultIterator, multi_classification
+    from starwhale import Image, PipelineHandler, multi_classification
 
     class MNISTInference(PipelineHandler):
             def __init__(self) -> None:
                 super().__init__()
                 self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
                 self.model = self._load_model(self.device)
 
@@ -194,15 +193,15 @@
                 confusion_matrix_normalize="all",
                 show_hamming_loss=True,
                 show_cohen_kappa_score=True,
                 show_roc_auc=True,
                 all_labels=[i for i in range(0, 10)],
             )
             def cmp(
-                self, ppl_result: PPLResultIterator
+                self, ppl_result
             ) -> t.Tuple[t.List[int], t.List[int], t.List[t.List[float]]]:
                 result, label, pr = [], [], []
                 for _data in ppl_result:
                     label.append(_data["ds_data"]["label"])
                     result.append(_data["result"][0])
                     pr.append(_data["result"][1])
                 return label, result, pr
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: starwhale Version: 0.4.1 Summary: An MLOps Platform
+Metadata-Version: 2.1 Name: starwhale Version: 0.4.2 Summary: An MLOps Platform
 for Model Evaluation Home-page: https://github.com/star-whale/starwhale Author:
 Starwhale Team Author-email: developer@starwhale.ai License: Apache License 2.0
 Keywords: MLOps,AI,Starwhale,Model Evaluation Classifier: Development Status ::
 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
@@ -77,74 +77,73 @@
 the network environment of the machine and the number of packages in the
 runtime.yaml. Using the befitting pypi mirror and cache config in the `~/.pip/
 pip.conf` file is a recommended practice. > > For users in the mainland of
 China, the following conf file is an option: > > ```conf > [global] > cache-dir
 = ~/.cache/pip > index-url = https://mirrors.aliyun.com/pypi/simple/ > extra-
 index-url = https://pypi.doubanio.com/simple > ``` ```bash swcli runtime build
 example/runtime/pytorch swcli runtime list swcli runtime info pytorch/version/
-latest swcli runtime restore pytorch/version/latest ``` - ð **STEP4**:
-Building a model - Download pre-trained model file: ```bash cd example/mnist
-make download-model # For users in the mainland of China, please add `CN=1`
-environment for make command: # CN=1 make download-model cd - ``` - [Code
-Example]Write some code with Starwhale Python SDK. Complete code is [here]
-(https://github.com/star-whale/starwhale/blob/main/example/mnist/mnist/
-evaluator.py). ```python import typing as t import torch from starwhale import
-Image, PipelineHandler, PPLResultIterator, multi_classification class
+latest ``` - ð **STEP4**: Building a model - Download pre-trained model
+file: ```bash cd example/mnist make download-model # For users in the mainland
+of China, please add `CN=1` environment for make command: # CN=1 make download-
+model cd - ``` - [Code Example]Write some code with Starwhale Python SDK.
+Complete code is [here](https://github.com/star-whale/starwhale/blob/main/
+example/mnist/mnist/evaluator.py). ```python import typing as t import torch
+from starwhale import Image, PipelineHandler, multi_classification class
 MNISTInference(PipelineHandler): def __init__(self) -> None: super().__init__()
 self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 self.model = self._load_model(self.device) def ppl(self, data: t.Dict[str,
 t.Any], **kw: t.Any) -> t.Tuple[float, t.List[float]]: data_tensor = self._pre
 (data["img"]) output = self.model(data_tensor) return self._post(output)
 @multi_classification( confusion_matrix_normalize="all",
 show_hamming_loss=True, show_cohen_kappa_score=True, show_roc_auc=True,
-all_labels=[i for i in range(0, 10)], ) def cmp( self, ppl_result:
-PPLResultIterator ) -> t.Tuple[t.List[int], t.List[int], t.List[t.List
-[float]]]: result, label, pr = [], [], [] for _data in ppl_result: label.append
-(_data["ds_data"]["label"]) result.append(_data["result"][0]) pr.append(_data
-["result"][1]) return label, result, pr def _pre(self, input:bytes): """write
-some mnist preprocessing code""" def _post(self, input:bytes): """write some
-mnist post-processing code""" def _load_model(): """load your pre trained
-model""" ``` - [Code Example]Define `model.yaml`. ```yaml name: mnist run:
-handler: mnist.evaluator:MNISTInference ``` - Run one command to build the
-model. ```bash swcli model build example/mnist --runtime pytorch/version/latest
-swcli model list swcli model info mnist/version/latest ``` - ðº **STEP5**:
-Building a dataset - Download MNIST RAW data files. ```bash cd example/mnist
-make download-data # For users in the mainland of China, please add `CN=1`
-environment for make command: # CN=1 make download-data cd - ``` - [Code
-Example]Write some code with Starwhale Python SDK. Full code is [here](https://
-github.com/star-whale/starwhale/blob/main/example/mnist/mnist/dataset.py).
-```python import struct from pathlib import Path from starwhale import
-GrayscaleImage def iter_swds_bin_item(): root_dir = Path
-(__file__).parent.parent / "data" with (root_dir / "t10k-images-idx3-
-ubyte").open("rb") as data_file, ( root_dir / "t10k-labels-idx1-ubyte" ).open
-("rb") as label_file: _, data_number, height, width = struct.unpack(">IIII",
-data_file.read(16)) _, label_number = struct.unpack(">II", label_file.read(8))
-print( f">data({data_file.name}) split data:{data_number}, label:{label_number}
-group" ) image_size = height * width for i in range(0, min(data_number,
-label_number)): _data = data_file.read(image_size) _label = struct.unpack(">B",
-label_file.read(1))[0] yield { "img": GrayscaleImage( _data, display_name=f"
-{i}", shape=(height, width, 1), ), "label": _label, } ``` - Run one command to
-build the dataset. ```bash swcli dataset build example/mnist --handler
-mnist.dataset:iter_swds_bin_item --runtime pytorch/version/latest swcli dataset
-info mnist/version/latest swcli dataset head mnist/version/latest ``` Starwhale
-also supports build dataset with pure python sdk. You can try it in [Google
-Colab](https://colab.research.google.com/github/star-whale/starwhale/blob/main/
-example/notebooks/dataset-sdk.ipynb). - ð **STEP6**: Running an evaluation
-job ```bash swcli eval run --model mnist/version/latest --dataset mnist/
-version/latest --runtime pytorch/version/latest swcli eval list swcli eval info
-$(swcli eval list | grep mnist | grep success | awk '{print $1}' | head -n 1)
-``` **ð Now, you have completed the fundamental steps for Starwhale
-standalone. Let's go ahead and finish the tutorial on the on-premises
-instance.** ## MNIST Quick Tour for on-premises instance ![Create Job Workflow]
-(docs/docs/img/console-create-job.gif) - ð° **STEP1**: Install minikube and
-helm - [Minikube](https://minikube.sigs.k8s.io/docs/start/) 1.25+ - [Helm]
-(https://helm.sh/docs/intro/install/) 3.2.0+ - ðµ **STEP2**: Start minikube
-```bash minikube start ``` > For users in the mainland of China, please add
-some external parameters. The following command was well tested; you may also
-try another kubernetes version. > > ```bash > minikube start --image-mirror-
+all_labels=[i for i in range(0, 10)], ) def cmp( self, ppl_result ) -> t.Tuple
+[t.List[int], t.List[int], t.List[t.List[float]]]: result, label, pr = [], [],
+[] for _data in ppl_result: label.append(_data["ds_data"]["label"])
+result.append(_data["result"][0]) pr.append(_data["result"][1]) return label,
+result, pr def _pre(self, input:bytes): """write some mnist preprocessing
+code""" def _post(self, input:bytes): """write some mnist post-processing
+code""" def _load_model(): """load your pre trained model""" ``` - [Code
+Example]Define `model.yaml`. ```yaml name: mnist run: handler: mnist.evaluator:
+MNISTInference ``` - Run one command to build the model. ```bash swcli model
+build example/mnist --runtime pytorch/version/latest swcli model list swcli
+model info mnist/version/latest ``` - ðº **STEP5**: Building a dataset -
+Download MNIST RAW data files. ```bash cd example/mnist make download-data #
+For users in the mainland of China, please add `CN=1` environment for make
+command: # CN=1 make download-data cd - ``` - [Code Example]Write some code
+with Starwhale Python SDK. Full code is [here](https://github.com/star-whale/
+starwhale/blob/main/example/mnist/mnist/dataset.py). ```python import struct
+from pathlib import Path from starwhale import GrayscaleImage def
+iter_swds_bin_item(): root_dir = Path(__file__).parent.parent / "data" with
+(root_dir / "t10k-images-idx3-ubyte").open("rb") as data_file, ( root_dir /
+"t10k-labels-idx1-ubyte" ).open("rb") as label_file: _, data_number, height,
+width = struct.unpack(">IIII", data_file.read(16)) _, label_number =
+struct.unpack(">II", label_file.read(8)) print( f">data({data_file.name}) split
+data:{data_number}, label:{label_number} group" ) image_size = height * width
+for i in range(0, min(data_number, label_number)): _data = data_file.read
+(image_size) _label = struct.unpack(">B", label_file.read(1))[0] yield { "img":
+GrayscaleImage( _data, display_name=f"{i}", shape=(height, width, 1), ),
+"label": _label, } ``` - Run one command to build the dataset. ```bash swcli
+dataset build example/mnist --handler mnist.dataset:iter_swds_bin_item --
+runtime pytorch/version/latest swcli dataset info mnist/version/latest swcli
+dataset head mnist/version/latest ``` Starwhale also supports build dataset
+with pure python sdk. You can try it in [Google Colab](https://
+colab.research.google.com/github/star-whale/starwhale/blob/main/example/
+notebooks/dataset-sdk.ipynb). - ð **STEP6**: Running an evaluation job
+```bash swcli eval run --model mnist/version/latest --dataset mnist/version/
+latest --runtime pytorch/version/latest swcli eval list swcli eval info $(swcli
+eval list | grep mnist | grep success | awk '{print $1}' | head -n 1) ```
+**ð Now, you have completed the fundamental steps for Starwhale standalone.
+Let's go ahead and finish the tutorial on the on-premises instance.** ## MNIST
+Quick Tour for on-premises instance ![Create Job Workflow](docs/docs/img/
+console-create-job.gif) - ð° **STEP1**: Install minikube and helm -
+[Minikube](https://minikube.sigs.k8s.io/docs/start/) 1.25+ - [Helm](https://
+helm.sh/docs/intro/install/) 3.2.0+ - ðµ **STEP2**: Start minikube ```bash
+minikube start ``` > For users in the mainland of China, please add some
+external parameters. The following command was well tested; you may also try
+another kubernetes version. > > ```bash > minikube start --image-mirror-
 country=cn --kubernetes-version=1.25.3 > ``` If there is no kubectl bin in your
 machine, you may use `minikube kubectl` or `alias kubectl="minikube kubectl --
 "` alias command. - ðµ **STEP3**: Installing Starwhale ```bash helm repo add
 starwhale https://star-whale.github.io/charts helm repo update helm pull
 starwhale/starwhale --untar --untardir ./charts helm upgrade --install
 starwhale ./charts/starwhale -n starwhale --create-namespace -f ./charts/
 starwhale/values.minikube.global.yaml ``` > For users in the mainland of China,
```

### Comparing `starwhale-0.4.1/starwhale.egg-info/requires.txt` & `starwhale-0.4.2/starwhale.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -20,47 +20,51 @@
 packaging>=21.3
 pyarrow>=8.0.0
 Jinja2>=3.1.2
 tenacity>=8.0.1
 gradio~=3.15.0
 psutil>=5.5.0
 GitPython>=3.1.24
+fastapi>=0.71.0
+filelock
 
 [:python_version < "3.8"]
 importlib-metadata<=4.2.0,>=4.0.0
 
 [all]
-psutil>=5.5.0
-scikit-learn>=0.20.0
-dill>=0.3.6
+requests-toolbelt>=0.9.0
+GitPython>=3.1.24
+fastapi>=0.71.0
+soundfile
 conda-pack==0.6.0
-boto3>=1.26.14
-shellingham>=1.4.0
 pyarrow>=8.0.0
-gradio~=3.15.0
+shellingham>=1.4.0
+click-option-group==0.5.5
+filelock
+click>=8.0.4
+jsonlines==3.0.0
+pillow
+Jinja2>=3.1.2
 cattrs>=1.7.1
-typing-extensions>=4.0.0
 loguru==0.6.0
-click>=8.0.4
-packaging>=21.3
-virtualenv>=13.0.0
 commonmark>=0.9.1
-jsonlines==3.0.0
-pyyaml==6.0
-fs>=2.4.0
-click-option-group==0.5.5
+textual==0.1.18
 attrs>=21.4.0
-Jinja2>=3.1.2
+virtualenv>=13.0.0
+psutil>=5.5.0
+fs>=2.4.0
+typing-extensions>=4.0.0
+scikit-learn>=0.20.0
 requests>=2.1.0
-pillow
-textual==0.1.18
 tenacity>=8.0.1
-requests-toolbelt>=0.9.0
-GitPython>=3.1.24
-soundfile
+gradio~=3.15.0
+packaging>=21.3
+boto3>=1.26.14
+pyyaml==6.0
+dill>=0.3.6
 
 [all:python_version < "3.8"]
 importlib-metadata<=4.2.0,>=4.0.0
 
 [audio]
 soundfile
```

