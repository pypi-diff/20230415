# Comparing `tmp/danling-0.2.1.tar.gz` & `tmp/danling-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danling-0.2.1.tar", last modified: Thu Apr 13 10:33:52 2023, max compression
+gzip compressed data, was "danling-0.2.3.tar", last modified: Fri Apr 14 17:19:19 2023, max compression
```

## Comparing `danling-0.2.1.tar` & `danling-0.2.3.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.336945 danling-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-13 10:33:46.000000 danling-0.2.1/.github/merge_rules.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-13 10:33:46.000000 danling-0.2.1/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-13 10:33:46.000000 danling-0.2.1/.github/workflows/push.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-04-13 10:33:46.000000 danling-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 10:33:46.000000 danling-0.2.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 10:33:46.000000 danling-0.2.1/LICENSES/LICENSE.Apache2
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-13 10:33:46.000000 danling-0.2.1/LICENSES/LICENSE.BSD2
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-13 10:33:46.000000 danling-0.2.1/LICENSES/LICENSE.BSD3
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-13 10:33:46.000000 danling-0.2.1/LICENSES/LICENSE.BSD4
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-13 10:33:46.000000 danling-0.2.1/LICENSES/LICENSE.GPL2
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 10:33:46.000000 danling-0.2.1/LICENSES/LICENSE.GPL3
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-13 10:33:46.000000 danling-0.2.1/LICENSES/LICENSE.MIT
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-13 10:33:46.000000 danling-0.2.1/LICENSES/LICENSE.Unlicense
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-13 10:33:52.336945 danling-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-13 10:33:46.000000 danling-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-13 10:33:46.000000 danling-0.2.1/anaconda-project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/danling/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-13 10:33:46.000000 danling-0.2.1/danling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 10:33:51.000000 danling-0.2.1/danling/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/danling/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-13 10:33:46.000000 danling-0.2.1/danling/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-13 10:33:46.000000 danling-0.2.1/danling/metrics/average_meter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-13 10:33:46.000000 danling-0.2.1/danling/metrics/average_meters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/danling/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-13 10:33:46.000000 danling-0.2.1/danling/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/danling/modules/mlp/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 10:33:46.000000 danling-0.2.1/danling/modules/mlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-13 10:33:46.000000 danling-0.2.1/danling/modules/mlp/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-13 10:33:46.000000 danling-0.2.1/danling/modules/mlp/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/danling/modules/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-13 10:33:46.000000 danling-0.2.1/danling/modules/transformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/danling/modules/transformer/attention/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-13 10:33:46.000000 danling-0.2.1/danling/modules/transformer/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-04-13 10:33:46.000000 danling-0.2.1/danling/modules/transformer/attention/multihead_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-04-13 10:33:46.000000 danling-0.2.1/danling/modules/transformer/attention/simple_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-04-13 10:33:46.000000 danling-0.2.1/danling/modules/transformer/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-04-13 10:33:46.000000 danling-0.2.1/danling/modules/transformer/encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/danling/modules/transformer/ffn/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 10:33:46.000000 danling-0.2.1/danling/modules/transformer/ffn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-13 10:33:46.000000 danling-0.2.1/danling/modules/transformer/ffn/fcn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/danling/modules/transformer/pos_embed/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-13 10:33:46.000000 danling-0.2.1/danling/modules/transformer/pos_embed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-13 10:33:46.000000 danling-0.2.1/danling/modules/transformer/pos_embed/pos_embed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/danling/optim/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 10:33:46.000000 danling-0.2.1/danling/optim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/danling/optim/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 10:33:46.000000 danling-0.2.1/danling/optim/lr_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-13 10:33:46.000000 danling-0.2.1/danling/optim/lr_scheduler/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-04-13 10:33:46.000000 danling-0.2.1/danling/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/danling/runner/
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-04-13 10:33:46.000000 danling-0.2.1/danling/runner/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-13 10:33:46.000000 danling-0.2.1/danling/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-04-13 10:33:46.000000 danling-0.2.1/danling/runner/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-04-13 10:33:46.000000 danling-0.2.1/danling/runner/runner_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12475 2023-04-13 10:33:46.000000 danling-0.2.1/danling/runner/runner_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-04-13 10:33:46.000000 danling-0.2.1/danling/runner/torch_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-13 10:33:46.000000 danling-0.2.1/danling/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.324945 danling-0.2.1/danling/tensors/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-13 10:33:46.000000 danling-0.2.1/danling/tensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21621 2023-04-13 10:33:46.000000 danling-0.2.1/danling/tensors/nested_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-13 10:33:46.000000 danling-0.2.1/danling/tensors/torch_func_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-13 10:33:46.000000 danling-0.2.1/danling/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.324945 danling-0.2.1/danling/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-13 10:33:46.000000 danling-0.2.1/danling/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-13 10:33:46.000000 danling-0.2.1/danling/utils/basex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-13 10:33:46.000000 danling-0.2.1/danling/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-13 10:33:46.000000 danling-0.2.1/danling/utils/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.320945 danling-0.2.1/danling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-13 10:33:52.000000 danling-0.2.1/danling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-04-13 10:33:52.000000 danling-0.2.1/danling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 10:33:52.000000 danling-0.2.1/danling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 10:33:52.000000 danling-0.2.1/danling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 10:33:52.000000 danling-0.2.1/danling.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.324945 danling-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 10:33:46.000000 danling-0.2.1/docs/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.324945 danling-0.2.1/docs/blog/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 10:33:46.000000 danling-0.2.1/docs/blog/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-13 10:33:46.000000 danling-0.2.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-13 10:33:46.000000 danling-0.2.1/docs/manifest.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.324945 danling-0.2.1/docs/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-13 10:33:46.000000 danling-0.2.1/docs/metrics/average_meter.md
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-13 10:33:46.000000 danling-0.2.1/docs/package.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-13 10:33:46.000000 danling-0.2.1/docs/registry.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.324945 danling-0.2.1/docs/runner/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-13 10:33:46.000000 danling-0.2.1/docs/runner/base_runner.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 10:33:46.000000 danling-0.2.1/docs/runner/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-13 10:33:46.000000 danling-0.2.1/docs/runner/runner_base.md
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-13 10:33:46.000000 danling-0.2.1/docs/runner/runner_state.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 10:33:46.000000 danling-0.2.1/docs/runner/torch_runner.md
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 10:33:46.000000 danling-0.2.1/docs/runner/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.324945 danling-0.2.1/docs/tensors/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 10:33:46.000000 danling-0.2.1/docs/tensors/nested_tensor.md
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-13 10:33:46.000000 danling-0.2.1/docs/tensors/pn_tensor.md
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-13 10:33:46.000000 danling-0.2.1/docs/tensors/torch_func_registry.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.324945 danling-0.2.1/docs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-13 10:33:46.000000 danling-0.2.1/docs/utils/basex.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-13 10:33:46.000000 danling-0.2.1/docs/utils/decorators.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-13 10:33:46.000000 danling-0.2.1/docs/utils/io.md
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-13 10:33:46.000000 danling-0.2.1/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.324945 danling-0.2.1/overrides/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.316945 danling-0.2.1/overrides/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.324945 danling-0.2.1/overrides/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-13 10:33:46.000000 danling-0.2.1/overrides/assets/css/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-13 10:33:46.000000 danling-0.2.1/overrides/assets/css/fonts.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.332945 danling-0.2.1/overrides/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   213368 2023-04-13 10:33:46.000000 danling-0.2.1/overrides/assets/fonts/CascadiaCodePL.woff2
--rw-r--r--   0 runner    (1001) docker     (123)  8530056 2023-04-13 10:33:46.000000 danling-0.2.1/overrides/assets/fonts/HYQiHei.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   118704 2023-04-13 10:33:46.000000 danling-0.2.1/overrides/assets/fonts/HelveticaNowDisplay.otf
--rw-r--r--   0 runner    (1001) docker     (123)   656232 2023-04-13 10:33:46.000000 danling-0.2.1/overrides/assets/fonts/HelveticaWorld.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.332945 danling-0.2.1/overrides/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-13 10:33:46.000000 danling-0.2.1/overrides/assets/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    21972 2023-04-13 10:33:46.000000 danling-0.2.1/overrides/assets/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.332945 danling-0.2.1/overrides/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-13 10:33:46.000000 danling-0.2.1/overrides/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-13 10:33:46.000000 danling-0.2.1/overrides/javascripts/shortcuts.js
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-13 10:33:46.000000 danling-0.2.1/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-13 10:33:46.000000 danling-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-13 10:33:46.000000 danling-0.2.1/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-13 10:33:46.000000 danling-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 10:33:52.336945 danling-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 10:33:46.000000 danling-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:33:52.332945 danling-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-04-13 10:33:46.000000 danling-0.2.1/tests/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.397458 danling-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.373458 danling-0.2.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-14 17:19:11.000000 danling-0.2.3/.github/merge_rules.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.373458 danling-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-14 17:19:11.000000 danling-0.2.3/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-14 17:19:11.000000 danling-0.2.3/.github/workflows/push.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-04-14 17:19:11.000000 danling-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-14 17:19:11.000000 danling-0.2.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.373458 danling-0.2.3/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-14 17:19:11.000000 danling-0.2.3/LICENSES/LICENSE.Apache2
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-14 17:19:11.000000 danling-0.2.3/LICENSES/LICENSE.BSD2
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-14 17:19:11.000000 danling-0.2.3/LICENSES/LICENSE.BSD3
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-14 17:19:11.000000 danling-0.2.3/LICENSES/LICENSE.BSD4
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-14 17:19:11.000000 danling-0.2.3/LICENSES/LICENSE.GPL2
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-14 17:19:11.000000 danling-0.2.3/LICENSES/LICENSE.GPL3
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-14 17:19:11.000000 danling-0.2.3/LICENSES/LICENSE.MIT
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-14 17:19:11.000000 danling-0.2.3/LICENSES/LICENSE.Unlicense
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-14 17:19:19.397458 danling-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-14 17:19:11.000000 danling-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-14 17:19:11.000000 danling-0.2.3/anaconda-project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.373458 danling-0.2.3/danling/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-14 17:19:11.000000 danling-0.2.3/danling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-14 17:19:18.000000 danling-0.2.3/danling/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.373458 danling-0.2.3/danling/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-14 17:19:11.000000 danling-0.2.3/danling/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-14 17:19:11.000000 danling-0.2.3/danling/metrics/average_meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-14 17:19:11.000000 danling-0.2.3/danling/metrics/average_meters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.373458 danling-0.2.3/danling/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-14 17:19:11.000000 danling-0.2.3/danling/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.377458 danling-0.2.3/danling/modules/mlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-14 17:19:11.000000 danling-0.2.3/danling/modules/mlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-14 17:19:11.000000 danling-0.2.3/danling/modules/mlp/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-14 17:19:11.000000 danling-0.2.3/danling/modules/mlp/mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.377458 danling-0.2.3/danling/modules/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-14 17:19:11.000000 danling-0.2.3/danling/modules/transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.377458 danling-0.2.3/danling/modules/transformer/attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-14 17:19:11.000000 danling-0.2.3/danling/modules/transformer/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-04-14 17:19:11.000000 danling-0.2.3/danling/modules/transformer/attention/multihead_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-04-14 17:19:11.000000 danling-0.2.3/danling/modules/transformer/attention/simple_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-04-14 17:19:11.000000 danling-0.2.3/danling/modules/transformer/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-04-14 17:19:11.000000 danling-0.2.3/danling/modules/transformer/encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.377458 danling-0.2.3/danling/modules/transformer/ffn/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-14 17:19:11.000000 danling-0.2.3/danling/modules/transformer/ffn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-14 17:19:11.000000 danling-0.2.3/danling/modules/transformer/ffn/fcn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.377458 danling-0.2.3/danling/modules/transformer/pos_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-14 17:19:11.000000 danling-0.2.3/danling/modules/transformer/pos_embed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-14 17:19:11.000000 danling-0.2.3/danling/modules/transformer/pos_embed/pos_embed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.377458 danling-0.2.3/danling/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-14 17:19:11.000000 danling-0.2.3/danling/optim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.377458 danling-0.2.3/danling/optim/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-14 17:19:11.000000 danling-0.2.3/danling/optim/lr_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-04-14 17:19:11.000000 danling-0.2.3/danling/optim/lr_scheduler/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-04-14 17:19:11.000000 danling-0.2.3/danling/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.377458 danling-0.2.3/danling/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-04-14 17:19:11.000000 danling-0.2.3/danling/runner/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-14 17:19:11.000000 danling-0.2.3/danling/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-04-14 17:19:11.000000 danling-0.2.3/danling/runner/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-04-14 17:19:11.000000 danling-0.2.3/danling/runner/runner_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-04-14 17:19:11.000000 danling-0.2.3/danling/runner/runner_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-14 17:19:11.000000 danling-0.2.3/danling/runner/torch_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-14 17:19:11.000000 danling-0.2.3/danling/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.377458 danling-0.2.3/danling/tensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-14 17:19:11.000000 danling-0.2.3/danling/tensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21621 2023-04-14 17:19:11.000000 danling-0.2.3/danling/tensors/nested_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-14 17:19:11.000000 danling-0.2.3/danling/tensors/torch_func_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-14 17:19:11.000000 danling-0.2.3/danling/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.377458 danling-0.2.3/danling/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-14 17:19:11.000000 danling-0.2.3/danling/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-14 17:19:11.000000 danling-0.2.3/danling/utils/basex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-14 17:19:11.000000 danling-0.2.3/danling/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-14 17:19:11.000000 danling-0.2.3/danling/utils/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.373458 danling-0.2.3/danling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-14 17:19:19.000000 danling-0.2.3/danling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-04-14 17:19:19.000000 danling-0.2.3/danling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:19:19.000000 danling-0.2.3/danling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-14 17:19:19.000000 danling-0.2.3/danling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 17:19:19.000000 danling-0.2.3/danling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.381458 danling-0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 17:19:11.000000 danling-0.2.3/docs/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.381458 danling-0.2.3/docs/blog/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 17:19:11.000000 danling-0.2.3/docs/blog/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-14 17:19:11.000000 danling-0.2.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-14 17:19:11.000000 danling-0.2.3/docs/manifest.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.381458 danling-0.2.3/docs/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-14 17:19:11.000000 danling-0.2.3/docs/metrics/average_meter.md
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-14 17:19:11.000000 danling-0.2.3/docs/package.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-14 17:19:11.000000 danling-0.2.3/docs/registry.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.381458 danling-0.2.3/docs/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-14 17:19:11.000000 danling-0.2.3/docs/runner/base_runner.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 17:19:11.000000 danling-0.2.3/docs/runner/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-14 17:19:11.000000 danling-0.2.3/docs/runner/runner_base.md
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-14 17:19:11.000000 danling-0.2.3/docs/runner/runner_state.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-14 17:19:11.000000 danling-0.2.3/docs/runner/torch_runner.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 17:19:11.000000 danling-0.2.3/docs/runner/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.381458 danling-0.2.3/docs/tensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-14 17:19:11.000000 danling-0.2.3/docs/tensors/nested_tensor.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-14 17:19:11.000000 danling-0.2.3/docs/tensors/pn_tensor.md
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-14 17:19:11.000000 danling-0.2.3/docs/tensors/torch_func_registry.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.381458 danling-0.2.3/docs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-14 17:19:11.000000 danling-0.2.3/docs/utils/basex.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-14 17:19:11.000000 danling-0.2.3/docs/utils/decorators.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-14 17:19:11.000000 danling-0.2.3/docs/utils/io.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-14 17:19:11.000000 danling-0.2.3/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.381458 danling-0.2.3/overrides/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.369458 danling-0.2.3/overrides/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.381458 danling-0.2.3/overrides/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-14 17:19:11.000000 danling-0.2.3/overrides/assets/css/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-14 17:19:11.000000 danling-0.2.3/overrides/assets/css/fonts.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.397458 danling-0.2.3/overrides/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   213368 2023-04-14 17:19:11.000000 danling-0.2.3/overrides/assets/fonts/CascadiaCodePL.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)  8530056 2023-04-14 17:19:11.000000 danling-0.2.3/overrides/assets/fonts/HYQiHei.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   118704 2023-04-14 17:19:11.000000 danling-0.2.3/overrides/assets/fonts/HelveticaNowDisplay.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   656232 2023-04-14 17:19:11.000000 danling-0.2.3/overrides/assets/fonts/HelveticaWorld.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.397458 danling-0.2.3/overrides/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-14 17:19:11.000000 danling-0.2.3/overrides/assets/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    21972 2023-04-14 17:19:11.000000 danling-0.2.3/overrides/assets/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.397458 danling-0.2.3/overrides/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-14 17:19:11.000000 danling-0.2.3/overrides/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-14 17:19:11.000000 danling-0.2.3/overrides/javascripts/shortcuts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-14 17:19:11.000000 danling-0.2.3/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-14 17:19:11.000000 danling-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-14 17:19:11.000000 danling-0.2.3/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-14 17:19:11.000000 danling-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 17:19:19.397458 danling-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 17:19:11.000000 danling-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.397458 danling-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-04-14 17:19:11.000000 danling-0.2.3/tests/test_runner.py
```

### Comparing `danling-0.2.1/.github/workflows/docs.yaml` & `danling-0.2.3/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/.github/workflows/push.yaml` & `danling-0.2.3/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/.gitignore` & `danling-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/LICENSES/LICENSE.Apache2` & `danling-0.2.3/LICENSES/LICENSE.Apache2`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/LICENSES/LICENSE.BSD2` & `danling-0.2.3/LICENSES/LICENSE.BSD2`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/LICENSES/LICENSE.BSD3` & `danling-0.2.3/LICENSES/LICENSE.BSD3`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/LICENSES/LICENSE.BSD4` & `danling-0.2.3/LICENSES/LICENSE.BSD4`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/LICENSES/LICENSE.GPL2` & `danling-0.2.3/LICENSES/LICENSE.GPL2`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/LICENSES/LICENSE.GPL3` & `danling-0.2.3/LICENSES/LICENSE.GPL3`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/LICENSES/LICENSE.MIT` & `danling-0.2.3/LICENSES/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/LICENSES/LICENSE.Unlicense` & `danling-0.2.3/LICENSES/LICENSE.Unlicense`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/PKG-INFO` & `danling-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danling
-Version: 0.2.1
+Version: 0.2.3
 Summary: Scaffold for experienced Machine Learning Researchers
 Author-email: Zhiyuan Chen <this@zyc.ai>
 Maintainer-email: Zhiyuan Chen <this@zyc.ai>
 License: Unlicense OR GPL-2.0-or-later OR MIT OR Apache-2.0 OR BSD-2-Clause OR BSD-3-Clause OR BSD-4-Clause
 Project-URL: homepage, https://danling.org
 Project-URL: repository, https://github.com/ZhiyuanChen/DanLing
 Project-URL: documentation, https://danling.org
```

### Comparing `danling-0.2.1/README.md` & `danling-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/anaconda-project.yml` & `danling-0.2.3/anaconda-project.yml`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/danling/__init__.py` & `danling-0.2.3/danling/__init__.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/danling/metrics/average_meter.py` & `danling-0.2.3/danling/metrics/average_meter.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/danling/metrics/average_meters.py` & `danling-0.2.3/danling/metrics/average_meters.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/danling/modules/__init__.py` & `danling-0.2.3/danling/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/danling/modules/mlp/dense.py` & `danling-0.2.3/danling/modules/mlp/dense.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/danling/modules/mlp/mlp.py` & `danling-0.2.3/danling/modules/mlp/mlp.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/danling/modules/transformer/__init__.py` & `danling-0.2.3/danling/modules/transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/danling/modules/transformer/attention/multihead_attention.py` & `danling-0.2.3/danling/modules/transformer/attention/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/danling/modules/transformer/attention/simple_attention.py` & `danling-0.2.3/danling/modules/transformer/attention/simple_attention.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/danling/modules/transformer/decoder.py` & `danling-0.2.3/danling/modules/transformer/decoder.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/danling/modules/transformer/encoder.py` & `danling-0.2.3/danling/modules/transformer/encoder.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/danling/modules/transformer/ffn/fcn.py` & `danling-0.2.3/danling/modules/transformer/ffn/fcn.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/danling/modules/transformer/pos_embed/pos_embed.py` & `danling-0.2.3/danling/modules/transformer/pos_embed/pos_embed.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/danling/registry.py` & `danling-0.2.3/danling/registry.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/danling/runner/README.md` & `danling-0.2.3/danling/runner/README.md`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/danling/runner/base_runner.py` & `danling-0.2.3/danling/runner/base_runner.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import logging
 import logging.config
 import os
 import random
 import shutil
-from typing import Callable, Mapping, Optional, Tuple, Union
+from typing import Callable, Mapping, Optional, Union
 from warnings import warn
 
 import numpy as np
 from chanfig import FlatDict, NestedDict
 
 from danling.utils import catch
 
@@ -64,15 +64,15 @@
                         "class": "logging.StreamHandler",
                         "stream": "ext://sys.stdout",
                     },
                     "logfile": {
                         "level": "DEBUG",
                         "formatter": "standard",
                         "class": "logging.FileHandler",
-                        "filename": self.state.log_path,
+                        "filename": self.log_path,
                         "mode": "a",
                     },
                 },
                 "loggers": {
                     "": {
                         "handlers": ["stdout", "logfile"],
                         "level": "DEBUG",
@@ -154,18 +154,17 @@
         """
 
         raise NotImplementedError
 
     def scale_lr(
         self,
         lr: float,  # pylint: disable=C0103
-        lr_final: float = 1e-6,
         lr_scale_factor: Optional[float] = None,
         batch_size_base: Optional[int] = None,
-    ) -> Tuple[float, float]:
+    ) -> float:
         r"""
         Scale learning rate according to [linear scaling rule](https://arxiv.org/abs/1706.02677).
         """
 
         # pylint: disable=W0201
 
         if lr_scale_factor is None:
@@ -176,17 +175,16 @@
             lr_scale_factor = self.batch_size_equivalent / batch_size_base
         elif batch_size_base is not None:
             warn(
                 "batch_size_base will be ignored if lr_scale_factor is specified",
                 RuntimeWarning,
             )
         lr = lr * lr_scale_factor  # pylint: disable=C0103, E1101
-        lr_final = lr_final * lr_scale_factor  # pylint: disable=E1101
         self.lr_scale_factor = lr_scale_factor
-        return lr, lr_final
+        return lr
 
     def step(self, zero_grad: bool = True, batch_size: Optional[int] = None) -> None:
         r"""
         Step optimizer and scheduler.
 
         This method increment `self.state.steps`.
 
@@ -215,60 +213,60 @@
 
         raise NotImplementedError
 
     @catch
     @on_main_process
     def save_checkpoint(self) -> None:
         r"""
-        Save checkpoint to `self.state.checkpoint_dir`.
+        Save checkpoint to `self.checkpoint_dir`.
 
-        The checkpoint will be saved to `self.state.checkpoint_dir/latest.pth`.
+        The checkpoint will be saved to `self.checkpoint_dir/latest.pth`.
 
         If `self.state.save_interval` is positive and `self.state.epochs + 1` is a multiple of `save_interval`,
-        the checkpoint will also be copied to `self.state.checkpoint_dir/epoch-{self.state.epochs}.pth`.
+        the checkpoint will also be copied to `self.checkpoint_dir/epoch-{self.state.epochs}.pth`.
 
-        If `self.state.is_best` is `True`, the checkpoint will also be copied to `self.state.checkpoint_dir/best.pth`.
+        If `self.state.is_best` is `True`, the checkpoint will also be copied to `self.checkpoint_dir/best.pth`.
         """
 
-        latest_path = os.path.join(self.state.checkpoint_dir, "latest.pth")
+        latest_path = os.path.join(self.checkpoint_dir, "latest.pth")
         self.save(self.state_dict(), latest_path)
         if (
             hasattr(self, "save_interval")
             and self.save_interval > 0
             and (self.state.epochs + 1) % self.save_interval == 0
         ):
-            save_path = os.path.join(self.state.checkpoint_dir, f"epoch-{self.state.epochs}.pth")
+            save_path = os.path.join(self.checkpoint_dir, f"epoch-{self.state.epochs}.pth")
             shutil.copy(latest_path, save_path)
         if self.is_best:
-            best_path = os.path.join(self.state.checkpoint_dir, "best.pth")
+            best_path = os.path.join(self.checkpoint_dir, "best.pth")
             shutil.copy(latest_path, best_path)
 
     def load_checkpoint(  # pylint: disable=W1113
         self, checkpoint: Optional[Union[Mapping, str]] = None, override_config: bool = True, *args, **kwargs
     ) -> None:
         """
         Load info from checkpoint.
 
         Args:
             checkpoint: Checkpoint (or its path) to load.
-                Defaults to `self.state.checkpoint_dir/latest.pth`.
+                Defaults to `self.checkpoint_dir/latest.pth`.
             override_config: If True, override runner config with checkpoint config.
             *args: Additional arguments to pass to `self.load`.
             **kwargs: Additional keyword arguments to pass to `self.load`.
 
         Raises:
             FileNotFoundError: If `checkpoint` does not exists.
 
         See Also:
             [`from_checkpoint`][danling.BaseRunner.from_checkpoint]: Build runner from checkpoint.
             [`load_pretrained`][danling.BaseRunner.load_pretrained]: Load parameters from pretrained checkpoint.
         """
 
         if checkpoint is None:
-            checkpoint = os.path.join(self.state.checkpoint_dir, "latest.pth")  # type: ignore
+            checkpoint = os.path.join(self.checkpoint_dir, "latest.pth")  # type: ignore
         # TODO: Support loading checkpoints in other format
         if isinstance(checkpoint, str):
             if not os.path.exists(checkpoint):
                 raise FileNotFoundError(f"checkpoint is set to {checkpoint} but does not exist.")
             self.checkpoint = checkpoint  # pylint: disable=W0201
             checkpoint: Mapping = self.load(checkpoint, *args, **kwargs)  # type: ignore
         # TODO: Wrap state_dict in a dataclass
@@ -311,15 +309,15 @@
     @classmethod
     def from_checkpoint(cls, checkpoint: Union[Mapping, str], *args, **kwargs) -> BaseRunner:
         r"""
         Build BaseRunner from checkpoint.
 
         Args:
             checkpoint: Checkpoint (or its path) to load.
-                Defaults to `self.state.checkpoint_dir/latest.pth`.
+                Defaults to `self.checkpoint_dir/latest.pth`.
             *args: Additional arguments to pass to `self.load`.
             **kwargs: Additional keyword arguments to pass to `self.load`.
 
         Returns:
             (BaseRunner):
         """
 
@@ -343,31 +341,31 @@
 
     def print_result(self) -> None:
         r"""
         Print latest and best result.
         """
 
         print(f"results: {self.state.results}")
-        print(f"latest result: {self.state.latest_result}")
-        print(f"best result: {self.state.best_result}")
+        print(f"latest result: {self.latest_result}")
+        print(f"best result: {self.best_result}")
 
     @catch
     @on_main_process
     def save_result(self) -> None:
         r"""
-        Save result to `self.state.dir`.
+        Save result to `self.dir`.
 
         This method will save latest and best result to
-        `self.state.dir/latest.json` and `self.state.dir/best.json` respectively.
+        `self.dir/latest.json` and `self.dir/best.json` respectively.
         """
 
-        results_path = os.path.join(self.state.dir, "results.json")
+        results_path = os.path.join(self.dir, "results.json")
         self.save({"id": self.state.id, "name": self.state.name, "results": self.state.results}, results_path, indent=4)
         ret = {"id": self.state.id, "name": self.state.name}
-        result = self.state.latest_result  # type: ignore
+        result = self.latest_result  # type: ignore
         if isinstance(result, FlatDict):
             result = result.dict()  # type: ignore
         # This is slower but ensure id is the first key
         if result is not None:
             ret.update(result)  # type: ignore
         latest_path = os.path.join(self.dir, "latest.json")
         self.save(ret, latest_path, indent=4)
```

### Comparing `danling-0.2.1/danling/runner/runner_base.py` & `danling-0.2.3/danling/runner/runner_base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 import logging
 import logging.config
 import os
-from typing import IO, Any, Callable, Mapping, Optional, Union
+from typing import IO, Any, Callable, List, Mapping, Optional, Union
 
-from chanfig import Config, FlatDict, Variable
+from chanfig import Config, FlatDict, NestedDict, Variable
 
-from danling.utils import catch, load, save
+from danling.utils import catch, ensure_dir, load, save
 
 from .runner_state import RunnerState
 
 PathStr = Union[os.PathLike, str, bytes]
 File = Union[PathStr, IO]
 
 DEFAULT_EXPERIMENT_NAME = "DanLing"
@@ -40,14 +40,38 @@
         dataloaders (FlatDict): All dataloaders, should be in the form of ``{subset: dataloader}``.
         batch_size (int, property): Number of samples per batch in train dataloader or the first dataloader.
         batch_size_equivalent (int, property): Total batch_size (`batch_size * world_size * accum_steps`).
 
     `datasets`, `datasamplers`, `dataloaders` should be a dict with the same keys.
     Their keys should be `split` (e.g. `train`, `val`, `test`).
 
+    Attributes: Progress:
+        progress (float, property): Running Progress, in `range(0, 1)`.
+
+    Attributes: Results:
+        latest_result (NestedDict, property): Most recent results,
+            should be in the form of ``{subset: {index: score}}``.
+        best_result (NestedDict, property): Best recent results, should be in the form of ``{subset: {index: score}}``.
+        scores (List[float], property): All scores.
+        latest_score (float, property): Most recent score.
+        best_score (float, property): Best score.
+        index_set (Optional[str]): The subset to calculate the core score.
+            If is `None`, will use the last set of the result.
+        index (str): The index to calculate the core score.
+            Defaults to `"loss"`.
+        is_best (bool, property): If `latest_score == best_score`.
+
+    Attributes: IO:
+        dir (str, property): Directory of the run.
+            Defaults to `os.path.join(self.project_root, f"{self.name}-{self.id}")`.
+        checkpoint_dir (str, property): Directory of checkpoints.
+        log_path (str, property):  Path of log file.
+        checkpoint_dir_name (str): The name of the directory under `runner.dir` to save checkpoints.
+            Defaults to `"checkpoints"`.
+
     Attributes: Parallel Training:
         world_size (int, property): Number of processes.
         rank (int, property): Process index of all processes.
         local_rank (int, property): Process index of local processes.
         distributed (bool, property): If runner is running in distributed mode.
         is_main_process (bool, property): If current process is the main process of all processes.
         is_local_main_process (bool, property): If current process is the main process of local processes.
@@ -293,20 +317,143 @@
     def from_yamls(cls, string: str, *args, **kwargs) -> RunnerBase:
         r"""
         Construct Runner from yaml string.
         """
 
         return cls(Config.from_yamls(string, *args, **kwargs))
 
+    @property
+    def progress(self) -> float:
+        r"""
+        Training Progress.
+
+        Returns:
+            (float):
+
+        Raises:
+            RuntimeError: If no terminal is defined.
+        """
+
+        if hasattr(self.state, "iter_end"):
+            return self.state.iters / self.state.iter_end
+        if hasattr(self.state, "step_end"):
+            return self.state.steps / self.state.step_end
+        if hasattr(self.state, "epoch_end"):
+            return self.state.epochs / self.state.epoch_end
+        raise RuntimeError("DanLing cannot determine progress since no terminal is defined.")
+
+    @property
+    def best_fn(self) -> Callable:  # pylint: disable=C0103
+        r"""
+        Function to determine the best score from a list of scores.
+
+        Subclass can override this method to accommodate needs, such as `min`.
+
+        Returns:
+            (callable): `max`
+        """
+
+        return max
+
+    @property
+    def latest_result(self) -> Optional[NestedDict]:
+        r"""
+        Latest result.
+        """
+
+        return self.state.results[-1] if self.state.results else None
+
+    @property
+    def best_result(self) -> Optional[NestedDict]:
+        r"""
+        Best result.
+        """
+        if not self.state.results:
+            return None
+        return self.state.results[-1 - self.scores[::-1].index(self.best_score)]  # type: ignore
+
+    @property
+    def scores(self) -> List[float]:
+        r"""
+        All scores.
+
+        Scores are extracted from results by `index_set` and `runner.index`,
+        following `[r[index_set][self.state.index] for r in self.state.results]`.
+
+        By default, `index_set` points to `self.state.index_set` and is set to `val`,
+        if `self.state.index_set` is not set, it will be the last key of the last result.
+
+        Scores are considered as the index of the performance of the model.
+        It is useful to determine the best model and the best hyper-parameters.
+        """
+
+        if not self.state.results:
+            return []
+        index_set = self.state.index_set or next(reversed(self.state.results[-1]))
+        return [r[index_set][self.state.index] for r in self.state.results]
+
+    @property
+    def latest_score(self) -> Optional[float]:
+        r"""
+        Latest score.
+        """
+
+        return self.scores[-1] if self.state.results else None
+
+    @property
+    def best_score(self) -> Optional[float]:
+        r"""
+        Best score.
+        """
+
+        return self.best_fn(self.scores) if self.results else None
+
+    @property
+    def is_best(self) -> bool:
+        r"""
+        If current epoch is the best epoch.
+        """
+
+        try:
+            return abs(self.latest_score - self.best_score) < 1e-7  # type: ignore
+        except TypeError:
+            return True
+
+    @property  # type: ignore
+    @ensure_dir
+    def dir(self) -> str:
+        r"""
+        Directory of the run.
+        """
+
+        return os.path.join(self.project_root, f"{self.name}-{self.id}")
+
+    @property
+    def log_path(self) -> str:
+        r"""
+        Path of log file.
+        """
+
+        return os.path.join(self.dir, "run.log")
+
+    @property  # type: ignore
+    @ensure_dir
+    def checkpoint_dir(self) -> str:
+        r"""
+        Directory of checkpoints.
+        """
+
+        return os.path.join(self.dir, self.checkpoint_dir_name)
+
     def __getattr__(self, name) -> Any:
         if name in self.state:
             return self.state[name]
         if name in dir(self.state):
             return getattr(self.state, name)
-        raise AttributeError(f"'{self.__class__.__name__}' object has no attribute '{name}'")
+        raise super().__getattribute__(name)
 
     def __setattr__(self, name, value) -> None:
         if name in self.__dict__ and isinstance(self.__dict__[name], Variable):
             self.__dict__[name].set(value)
         else:
             self.__dict__[name] = value
```

### Comparing `danling-0.2.1/danling/runner/torch_runner.py` & `danling-0.2.3/danling/runner/torch_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,8 +242,8 @@
     def __getattr__(self, name: str) -> Any:
         try:
             return super().__getattr__(name)
         except AttributeError:
             pass
         if self.accelerator is not None and hasattr(self.accelerator, name):
             return getattr(self.accelerator, name)
-        raise AttributeError(f"'{self.__class__.__name__}' object has no attribute '{name}'")
+        raise super().__getattribute__(name)
```

### Comparing `danling-0.2.1/danling/runner/utils.py` & `danling-0.2.3/danling/runner/utils.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/danling/tensors/nested_tensor.py` & `danling-0.2.3/danling/tensors/nested_tensor.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/danling/tensors/torch_func_registry.py` & `danling-0.2.3/danling/tensors/torch_func_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from functools import wraps
 from typing import Callable
 
-from ..registry import Registry
+from chanfig import Registry
 
 
 class TorchFuncRegistry(Registry):
     """
     `TorchFuncRegistry` for extending PyTorch Tensor.
     """
```

### Comparing `danling-0.2.1/danling/utils/basex.py` & `danling-0.2.3/danling/utils/basex.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/danling/utils/decorators.py` & `danling-0.2.3/danling/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/danling/utils/io.py` & `danling-0.2.3/danling/utils/io.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/danling.egg-info/PKG-INFO` & `danling-0.2.3/danling.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danling
-Version: 0.2.1
+Version: 0.2.3
 Summary: Scaffold for experienced Machine Learning Researchers
 Author-email: Zhiyuan Chen <this@zyc.ai>
 Maintainer-email: Zhiyuan Chen <this@zyc.ai>
 License: Unlicense OR GPL-2.0-or-later OR MIT OR Apache-2.0 OR BSD-2-Clause OR BSD-3-Clause OR BSD-4-Clause
 Project-URL: homepage, https://danling.org
 Project-URL: repository, https://github.com/ZhiyuanChen/DanLing
 Project-URL: documentation, https://danling.org
```

### Comparing `danling-0.2.1/danling.egg-info/SOURCES.txt` & `danling-0.2.3/danling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/mkdocs.yml` & `danling-0.2.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/overrides/assets/fonts/CascadiaCodePL.woff2` & `danling-0.2.3/overrides/assets/fonts/CascadiaCodePL.woff2`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/overrides/assets/fonts/HYQiHei.ttf` & `danling-0.2.3/overrides/assets/fonts/HYQiHei.ttf`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/overrides/assets/fonts/HelveticaNowDisplay.otf` & `danling-0.2.3/overrides/assets/fonts/HelveticaNowDisplay.otf`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/overrides/assets/fonts/HelveticaWorld.ttf` & `danling-0.2.3/overrides/assets/fonts/HelveticaWorld.ttf`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/overrides/assets/images/favicon.ico` & `danling-0.2.3/overrides/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/overrides/assets/images/logo.png` & `danling-0.2.3/overrides/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/overrides/main.html` & `danling-0.2.3/overrides/main.html`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/pyproject.toml` & `danling-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `danling-0.2.1/tests/test_runner.py` & `danling-0.2.3/tests/test_runner.py`

 * *Files identical despite different names*

