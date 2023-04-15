# Comparing `tmp/danling-0.2.3.tar.gz` & `tmp/danling-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danling-0.2.3.tar", last modified: Fri Apr 14 17:19:19 2023, max compression
+gzip compressed data, was "danling-0.2.4.tar", last modified: Sat Apr 15 07:40:42 2023, max compression
```

## Comparing `danling-0.2.3.tar` & `danling-0.2.4.tar`

### file list

```diff
@@ -1,127 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.397458 danling-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.373458 danling-0.2.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-14 17:19:11.000000 danling-0.2.3/.github/merge_rules.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.373458 danling-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-14 17:19:11.000000 danling-0.2.3/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-14 17:19:11.000000 danling-0.2.3/.github/workflows/push.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-04-14 17:19:11.000000 danling-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-14 17:19:11.000000 danling-0.2.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.373458 danling-0.2.3/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-14 17:19:11.000000 danling-0.2.3/LICENSES/LICENSE.Apache2
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-14 17:19:11.000000 danling-0.2.3/LICENSES/LICENSE.BSD2
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-14 17:19:11.000000 danling-0.2.3/LICENSES/LICENSE.BSD3
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-14 17:19:11.000000 danling-0.2.3/LICENSES/LICENSE.BSD4
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-14 17:19:11.000000 danling-0.2.3/LICENSES/LICENSE.GPL2
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-14 17:19:11.000000 danling-0.2.3/LICENSES/LICENSE.GPL3
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-14 17:19:11.000000 danling-0.2.3/LICENSES/LICENSE.MIT
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-14 17:19:11.000000 danling-0.2.3/LICENSES/LICENSE.Unlicense
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-14 17:19:19.397458 danling-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-14 17:19:11.000000 danling-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-14 17:19:11.000000 danling-0.2.3/anaconda-project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.373458 danling-0.2.3/danling/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-14 17:19:11.000000 danling-0.2.3/danling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-14 17:19:18.000000 danling-0.2.3/danling/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.373458 danling-0.2.3/danling/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-14 17:19:11.000000 danling-0.2.3/danling/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-14 17:19:11.000000 danling-0.2.3/danling/metrics/average_meter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-14 17:19:11.000000 danling-0.2.3/danling/metrics/average_meters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.373458 danling-0.2.3/danling/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-14 17:19:11.000000 danling-0.2.3/danling/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.377458 danling-0.2.3/danling/modules/mlp/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-14 17:19:11.000000 danling-0.2.3/danling/modules/mlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-14 17:19:11.000000 danling-0.2.3/danling/modules/mlp/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-14 17:19:11.000000 danling-0.2.3/danling/modules/mlp/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.377458 danling-0.2.3/danling/modules/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-14 17:19:11.000000 danling-0.2.3/danling/modules/transformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.377458 danling-0.2.3/danling/modules/transformer/attention/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-14 17:19:11.000000 danling-0.2.3/danling/modules/transformer/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-04-14 17:19:11.000000 danling-0.2.3/danling/modules/transformer/attention/multihead_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-04-14 17:19:11.000000 danling-0.2.3/danling/modules/transformer/attention/simple_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-04-14 17:19:11.000000 danling-0.2.3/danling/modules/transformer/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-04-14 17:19:11.000000 danling-0.2.3/danling/modules/transformer/encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.377458 danling-0.2.3/danling/modules/transformer/ffn/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-14 17:19:11.000000 danling-0.2.3/danling/modules/transformer/ffn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-14 17:19:11.000000 danling-0.2.3/danling/modules/transformer/ffn/fcn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.377458 danling-0.2.3/danling/modules/transformer/pos_embed/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-14 17:19:11.000000 danling-0.2.3/danling/modules/transformer/pos_embed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-14 17:19:11.000000 danling-0.2.3/danling/modules/transformer/pos_embed/pos_embed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.377458 danling-0.2.3/danling/optim/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-14 17:19:11.000000 danling-0.2.3/danling/optim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.377458 danling-0.2.3/danling/optim/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-14 17:19:11.000000 danling-0.2.3/danling/optim/lr_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-04-14 17:19:11.000000 danling-0.2.3/danling/optim/lr_scheduler/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-04-14 17:19:11.000000 danling-0.2.3/danling/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.377458 danling-0.2.3/danling/runner/
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-04-14 17:19:11.000000 danling-0.2.3/danling/runner/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-14 17:19:11.000000 danling-0.2.3/danling/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-04-14 17:19:11.000000 danling-0.2.3/danling/runner/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-04-14 17:19:11.000000 danling-0.2.3/danling/runner/runner_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-04-14 17:19:11.000000 danling-0.2.3/danling/runner/runner_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-14 17:19:11.000000 danling-0.2.3/danling/runner/torch_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-14 17:19:11.000000 danling-0.2.3/danling/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.377458 danling-0.2.3/danling/tensors/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-14 17:19:11.000000 danling-0.2.3/danling/tensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21621 2023-04-14 17:19:11.000000 danling-0.2.3/danling/tensors/nested_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-14 17:19:11.000000 danling-0.2.3/danling/tensors/torch_func_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-14 17:19:11.000000 danling-0.2.3/danling/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.377458 danling-0.2.3/danling/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-14 17:19:11.000000 danling-0.2.3/danling/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-14 17:19:11.000000 danling-0.2.3/danling/utils/basex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-14 17:19:11.000000 danling-0.2.3/danling/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-14 17:19:11.000000 danling-0.2.3/danling/utils/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.373458 danling-0.2.3/danling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-14 17:19:19.000000 danling-0.2.3/danling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-04-14 17:19:19.000000 danling-0.2.3/danling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 17:19:19.000000 danling-0.2.3/danling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-14 17:19:19.000000 danling-0.2.3/danling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 17:19:19.000000 danling-0.2.3/danling.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.381458 danling-0.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 17:19:11.000000 danling-0.2.3/docs/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.381458 danling-0.2.3/docs/blog/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 17:19:11.000000 danling-0.2.3/docs/blog/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-14 17:19:11.000000 danling-0.2.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-14 17:19:11.000000 danling-0.2.3/docs/manifest.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.381458 danling-0.2.3/docs/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-14 17:19:11.000000 danling-0.2.3/docs/metrics/average_meter.md
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-14 17:19:11.000000 danling-0.2.3/docs/package.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-14 17:19:11.000000 danling-0.2.3/docs/registry.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.381458 danling-0.2.3/docs/runner/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-14 17:19:11.000000 danling-0.2.3/docs/runner/base_runner.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 17:19:11.000000 danling-0.2.3/docs/runner/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-14 17:19:11.000000 danling-0.2.3/docs/runner/runner_base.md
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-14 17:19:11.000000 danling-0.2.3/docs/runner/runner_state.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-14 17:19:11.000000 danling-0.2.3/docs/runner/torch_runner.md
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 17:19:11.000000 danling-0.2.3/docs/runner/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.381458 danling-0.2.3/docs/tensors/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-14 17:19:11.000000 danling-0.2.3/docs/tensors/nested_tensor.md
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-14 17:19:11.000000 danling-0.2.3/docs/tensors/pn_tensor.md
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-14 17:19:11.000000 danling-0.2.3/docs/tensors/torch_func_registry.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.381458 danling-0.2.3/docs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-14 17:19:11.000000 danling-0.2.3/docs/utils/basex.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-14 17:19:11.000000 danling-0.2.3/docs/utils/decorators.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-14 17:19:11.000000 danling-0.2.3/docs/utils/io.md
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-14 17:19:11.000000 danling-0.2.3/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.381458 danling-0.2.3/overrides/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.369458 danling-0.2.3/overrides/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.381458 danling-0.2.3/overrides/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-14 17:19:11.000000 danling-0.2.3/overrides/assets/css/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-14 17:19:11.000000 danling-0.2.3/overrides/assets/css/fonts.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.397458 danling-0.2.3/overrides/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   213368 2023-04-14 17:19:11.000000 danling-0.2.3/overrides/assets/fonts/CascadiaCodePL.woff2
--rw-r--r--   0 runner    (1001) docker     (123)  8530056 2023-04-14 17:19:11.000000 danling-0.2.3/overrides/assets/fonts/HYQiHei.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   118704 2023-04-14 17:19:11.000000 danling-0.2.3/overrides/assets/fonts/HelveticaNowDisplay.otf
--rw-r--r--   0 runner    (1001) docker     (123)   656232 2023-04-14 17:19:11.000000 danling-0.2.3/overrides/assets/fonts/HelveticaWorld.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.397458 danling-0.2.3/overrides/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-14 17:19:11.000000 danling-0.2.3/overrides/assets/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    21972 2023-04-14 17:19:11.000000 danling-0.2.3/overrides/assets/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.397458 danling-0.2.3/overrides/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-14 17:19:11.000000 danling-0.2.3/overrides/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-14 17:19:11.000000 danling-0.2.3/overrides/javascripts/shortcuts.js
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-14 17:19:11.000000 danling-0.2.3/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-14 17:19:11.000000 danling-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-14 17:19:11.000000 danling-0.2.3/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-14 17:19:11.000000 danling-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 17:19:19.397458 danling-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 17:19:11.000000 danling-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 17:19:19.397458 danling-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-04-14 17:19:11.000000 danling-0.2.3/tests/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.167348 danling-0.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.147348 danling-0.2.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-15 07:40:36.000000 danling-0.2.4/.github/merge_rules.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.147348 danling-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-15 07:40:36.000000 danling-0.2.4/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-15 07:40:36.000000 danling-0.2.4/.github/workflows/push.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-04-15 07:40:36.000000 danling-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-15 07:40:36.000000 danling-0.2.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.151348 danling-0.2.4/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-15 07:40:36.000000 danling-0.2.4/LICENSES/LICENSE.Apache2
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-15 07:40:36.000000 danling-0.2.4/LICENSES/LICENSE.BSD2
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-15 07:40:36.000000 danling-0.2.4/LICENSES/LICENSE.BSD3
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-15 07:40:36.000000 danling-0.2.4/LICENSES/LICENSE.BSD4
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-15 07:40:36.000000 danling-0.2.4/LICENSES/LICENSE.GPL2
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-15 07:40:36.000000 danling-0.2.4/LICENSES/LICENSE.GPL3
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-15 07:40:36.000000 danling-0.2.4/LICENSES/LICENSE.MIT
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-15 07:40:36.000000 danling-0.2.4/LICENSES/LICENSE.Unlicense
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-15 07:40:42.167348 danling-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-15 07:40:36.000000 danling-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-15 07:40:36.000000 danling-0.2.4/anaconda-project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.151348 danling-0.2.4/danling/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-15 07:40:36.000000 danling-0.2.4/danling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-15 07:40:41.000000 danling-0.2.4/danling/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.151348 danling-0.2.4/danling/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-15 07:40:36.000000 danling-0.2.4/danling/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-15 07:40:36.000000 danling-0.2.4/danling/metrics/average_meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-15 07:40:36.000000 danling-0.2.4/danling/metrics/average_meters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.151348 danling-0.2.4/danling/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-15 07:40:36.000000 danling-0.2.4/danling/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.151348 danling-0.2.4/danling/modules/mlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-15 07:40:36.000000 danling-0.2.4/danling/modules/mlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-15 07:40:36.000000 danling-0.2.4/danling/modules/mlp/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-15 07:40:36.000000 danling-0.2.4/danling/modules/mlp/mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.151348 danling-0.2.4/danling/modules/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-15 07:40:36.000000 danling-0.2.4/danling/modules/transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.151348 danling-0.2.4/danling/modules/transformer/attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-15 07:40:36.000000 danling-0.2.4/danling/modules/transformer/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-04-15 07:40:36.000000 danling-0.2.4/danling/modules/transformer/attention/multihead_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-04-15 07:40:36.000000 danling-0.2.4/danling/modules/transformer/attention/simple_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-04-15 07:40:36.000000 danling-0.2.4/danling/modules/transformer/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-04-15 07:40:36.000000 danling-0.2.4/danling/modules/transformer/encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.151348 danling-0.2.4/danling/modules/transformer/ffn/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-15 07:40:36.000000 danling-0.2.4/danling/modules/transformer/ffn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-15 07:40:36.000000 danling-0.2.4/danling/modules/transformer/ffn/fcn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.151348 danling-0.2.4/danling/modules/transformer/pos_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-15 07:40:36.000000 danling-0.2.4/danling/modules/transformer/pos_embed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-15 07:40:36.000000 danling-0.2.4/danling/modules/transformer/pos_embed/pos_embed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.151348 danling-0.2.4/danling/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-15 07:40:36.000000 danling-0.2.4/danling/optim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.151348 danling-0.2.4/danling/optim/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-15 07:40:36.000000 danling-0.2.4/danling/optim/lr_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-04-15 07:40:36.000000 danling-0.2.4/danling/optim/lr_scheduler/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-04-15 07:40:36.000000 danling-0.2.4/danling/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.151348 danling-0.2.4/danling/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-04-15 07:40:36.000000 danling-0.2.4/danling/runner/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-15 07:40:36.000000 danling-0.2.4/danling/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-04-15 07:40:36.000000 danling-0.2.4/danling/runner/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14755 2023-04-15 07:40:36.000000 danling-0.2.4/danling/runner/runner_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-04-15 07:40:36.000000 danling-0.2.4/danling/runner/runner_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-15 07:40:36.000000 danling-0.2.4/danling/runner/torch_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-15 07:40:36.000000 danling-0.2.4/danling/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.151348 danling-0.2.4/danling/tensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-15 07:40:36.000000 danling-0.2.4/danling/tensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21621 2023-04-15 07:40:36.000000 danling-0.2.4/danling/tensors/nested_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-15 07:40:36.000000 danling-0.2.4/danling/tensors/torch_func_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-15 07:40:36.000000 danling-0.2.4/danling/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.155348 danling-0.2.4/danling/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-15 07:40:36.000000 danling-0.2.4/danling/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-15 07:40:36.000000 danling-0.2.4/danling/utils/basex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-15 07:40:36.000000 danling-0.2.4/danling/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-15 07:40:36.000000 danling-0.2.4/danling/utils/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.151348 danling-0.2.4/danling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-15 07:40:42.000000 danling-0.2.4/danling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-15 07:40:42.000000 danling-0.2.4/danling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 07:40:42.000000 danling-0.2.4/danling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-15 07:40:42.000000 danling-0.2.4/danling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-15 07:40:42.000000 danling-0.2.4/danling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.155348 danling-0.2.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-15 07:40:36.000000 danling-0.2.4/docs/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.155348 danling-0.2.4/docs/blog/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-15 07:40:36.000000 danling-0.2.4/docs/blog/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-15 07:40:36.000000 danling-0.2.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-15 07:40:36.000000 danling-0.2.4/docs/manifest.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.155348 danling-0.2.4/docs/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-15 07:40:36.000000 danling-0.2.4/docs/metrics/average_meter.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.155348 danling-0.2.4/docs/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-15 07:40:36.000000 danling-0.2.4/docs/optim/lr_scheduler.md
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-15 07:40:36.000000 danling-0.2.4/docs/package.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-15 07:40:36.000000 danling-0.2.4/docs/registry.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.155348 danling-0.2.4/docs/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-15 07:40:36.000000 danling-0.2.4/docs/runner/base_runner.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 07:40:36.000000 danling-0.2.4/docs/runner/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-15 07:40:36.000000 danling-0.2.4/docs/runner/runner_base.md
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-15 07:40:36.000000 danling-0.2.4/docs/runner/runner_state.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-15 07:40:36.000000 danling-0.2.4/docs/runner/torch_runner.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-15 07:40:36.000000 danling-0.2.4/docs/runner/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.155348 danling-0.2.4/docs/tensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-15 07:40:36.000000 danling-0.2.4/docs/tensors/nested_tensor.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-15 07:40:36.000000 danling-0.2.4/docs/tensors/pn_tensor.md
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-15 07:40:36.000000 danling-0.2.4/docs/tensors/torch_func_registry.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.155348 danling-0.2.4/docs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-15 07:40:36.000000 danling-0.2.4/docs/utils/basex.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-15 07:40:36.000000 danling-0.2.4/docs/utils/decorators.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-15 07:40:36.000000 danling-0.2.4/docs/utils/io.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-04-15 07:40:36.000000 danling-0.2.4/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.155348 danling-0.2.4/overrides/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.147348 danling-0.2.4/overrides/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.155348 danling-0.2.4/overrides/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-15 07:40:36.000000 danling-0.2.4/overrides/assets/css/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-15 07:40:36.000000 danling-0.2.4/overrides/assets/css/fonts.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.167348 danling-0.2.4/overrides/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   213368 2023-04-15 07:40:36.000000 danling-0.2.4/overrides/assets/fonts/CascadiaCodePL.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)  8530056 2023-04-15 07:40:37.000000 danling-0.2.4/overrides/assets/fonts/HYQiHei.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   118704 2023-04-15 07:40:37.000000 danling-0.2.4/overrides/assets/fonts/HelveticaNowDisplay.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   656232 2023-04-15 07:40:37.000000 danling-0.2.4/overrides/assets/fonts/HelveticaWorld.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.167348 danling-0.2.4/overrides/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-15 07:40:37.000000 danling-0.2.4/overrides/assets/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    21972 2023-04-15 07:40:37.000000 danling-0.2.4/overrides/assets/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.167348 danling-0.2.4/overrides/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-15 07:40:37.000000 danling-0.2.4/overrides/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-15 07:40:37.000000 danling-0.2.4/overrides/javascripts/shortcuts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-15 07:40:37.000000 danling-0.2.4/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-15 07:40:37.000000 danling-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-15 07:40:37.000000 danling-0.2.4/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-15 07:40:37.000000 danling-0.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 07:40:42.167348 danling-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 07:40:37.000000 danling-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 07:40:42.167348 danling-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-04-15 07:40:37.000000 danling-0.2.4/tests/test_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-04-15 07:40:37.000000 danling-0.2.4/tests/test_runner.py
```

### Comparing `danling-0.2.3/.github/workflows/docs.yaml` & `danling-0.2.4/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/.github/workflows/push.yaml` & `danling-0.2.4/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/.gitignore` & `danling-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/LICENSES/LICENSE.Apache2` & `danling-0.2.4/LICENSES/LICENSE.Apache2`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/LICENSES/LICENSE.BSD2` & `danling-0.2.4/LICENSES/LICENSE.BSD2`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/LICENSES/LICENSE.BSD3` & `danling-0.2.4/LICENSES/LICENSE.BSD3`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/LICENSES/LICENSE.BSD4` & `danling-0.2.4/LICENSES/LICENSE.BSD4`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/LICENSES/LICENSE.GPL2` & `danling-0.2.4/LICENSES/LICENSE.GPL2`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/LICENSES/LICENSE.GPL3` & `danling-0.2.4/LICENSES/LICENSE.GPL3`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/LICENSES/LICENSE.MIT` & `danling-0.2.4/LICENSES/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/LICENSES/LICENSE.Unlicense` & `danling-0.2.4/LICENSES/LICENSE.Unlicense`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/PKG-INFO` & `danling-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danling
-Version: 0.2.3
+Version: 0.2.4
 Summary: Scaffold for experienced Machine Learning Researchers
 Author-email: Zhiyuan Chen <this@zyc.ai>
 Maintainer-email: Zhiyuan Chen <this@zyc.ai>
 License: Unlicense OR GPL-2.0-or-later OR MIT OR Apache-2.0 OR BSD-2-Clause OR BSD-3-Clause OR BSD-4-Clause
 Project-URL: homepage, https://danling.org
 Project-URL: repository, https://github.com/ZhiyuanChen/DanLing
 Project-URL: documentation, https://danling.org
```

### Comparing `danling-0.2.3/README.md` & `danling-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/anaconda-project.yml` & `danling-0.2.4/anaconda-project.yml`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/danling/__init__.py` & `danling-0.2.4/danling/__init__.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/danling/metrics/average_meter.py` & `danling-0.2.4/danling/metrics/average_meter.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/danling/metrics/average_meters.py` & `danling-0.2.4/danling/metrics/average_meters.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/danling/modules/__init__.py` & `danling-0.2.4/danling/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/danling/modules/mlp/dense.py` & `danling-0.2.4/danling/modules/mlp/dense.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/danling/modules/mlp/mlp.py` & `danling-0.2.4/danling/modules/mlp/mlp.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/danling/modules/transformer/__init__.py` & `danling-0.2.4/danling/modules/transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/danling/modules/transformer/attention/multihead_attention.py` & `danling-0.2.4/danling/modules/transformer/attention/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/danling/modules/transformer/attention/simple_attention.py` & `danling-0.2.4/danling/modules/transformer/attention/simple_attention.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/danling/modules/transformer/decoder.py` & `danling-0.2.4/danling/modules/transformer/decoder.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/danling/modules/transformer/encoder.py` & `danling-0.2.4/danling/modules/transformer/encoder.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/danling/modules/transformer/ffn/fcn.py` & `danling-0.2.4/danling/modules/transformer/ffn/fcn.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/danling/modules/transformer/pos_embed/pos_embed.py` & `danling-0.2.4/danling/modules/transformer/pos_embed/pos_embed.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/danling/registry.py` & `danling-0.2.4/danling/registry.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/danling/runner/README.md` & `danling-0.2.4/danling/runner/README.md`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/danling/runner/base_runner.py` & `danling-0.2.4/danling/runner/base_runner.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/danling/runner/runner_base.py` & `danling-0.2.4/danling/runner/runner_base.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/danling/runner/runner_state.py` & `danling-0.2.4/danling/runner/runner_state.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/danling/runner/torch_runner.py` & `danling-0.2.4/danling/runner/torch_runner.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/danling/runner/utils.py` & `danling-0.2.4/danling/runner/utils.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/danling/tensors/nested_tensor.py` & `danling-0.2.4/danling/tensors/nested_tensor.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/danling/tensors/torch_func_registry.py` & `danling-0.2.4/danling/tensors/torch_func_registry.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/danling/utils/basex.py` & `danling-0.2.4/danling/utils/basex.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/danling/utils/decorators.py` & `danling-0.2.4/danling/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/danling/utils/io.py` & `danling-0.2.4/danling/utils/io.py`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/danling.egg-info/PKG-INFO` & `danling-0.2.4/danling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danling
-Version: 0.2.3
+Version: 0.2.4
 Summary: Scaffold for experienced Machine Learning Researchers
 Author-email: Zhiyuan Chen <this@zyc.ai>
 Maintainer-email: Zhiyuan Chen <this@zyc.ai>
 License: Unlicense OR GPL-2.0-or-later OR MIT OR Apache-2.0 OR BSD-2-Clause OR BSD-3-Clause OR BSD-4-Clause
 Project-URL: homepage, https://danling.org
 Project-URL: repository, https://github.com/ZhiyuanChen/DanLing
 Project-URL: documentation, https://danling.org
```

### Comparing `danling-0.2.3/danling.egg-info/SOURCES.txt` & `danling-0.2.4/danling.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 docs/CNAME
 docs/index.md
 docs/manifest.webmanifest
 docs/package.md
 docs/registry.md
 docs/blog/index.md
 docs/metrics/average_meter.md
+docs/optim/lr_scheduler.md
 docs/runner/base_runner.md
 docs/runner/index.md
 docs/runner/runner_base.md
 docs/runner/runner_state.md
 docs/runner/torch_runner.md
 docs/runner/utils.md
 docs/tensors/nested_tensor.md
@@ -87,8 +88,9 @@
 overrides/assets/fonts/HYQiHei.ttf
 overrides/assets/fonts/HelveticaNowDisplay.otf
 overrides/assets/fonts/HelveticaWorld.ttf
 overrides/assets/images/favicon.ico
 overrides/assets/images/logo.png
 overrides/javascripts/mathjax.js
 overrides/javascripts/shortcuts.js
+tests/test_lr_scheduler.py
 tests/test_runner.py
```

### Comparing `danling-0.2.3/mkdocs.yml` & `danling-0.2.4/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,16 @@
       - BaseRunner: runner/base_runner.md
       - TorchRunner: runner/torch_runner.md
       - Utilities: runner/utils.md
   - Tensors:
     - NestedTensor: tensors/nested_tensor.md
     - PNTensor: tensors/pn_tensor.md
     - TorchFuncRegistry: tensors/torch_func_registry.md
-  - Registry: registry.md
+  - Optim:
+    - LRScheduler: optim/lr_scheduler.md
   - Metrics:
     - AverageMeter: metrics/average_meter.md
   - Utils:
       - Decorator: utils/decorators.md
       - IO: utils/io.md
       - basex: utils/basex.md
   - package: package.md
```

#### html2text {}

```diff
@@ -2,16 +2,16 @@
 Contributors site_description: Easier Configuration copyright: All rights
 reserved © 2021-2023, DanLing Contributors repo_name: DanLing repo_url: https:/
 /github.com/ZhiyuanChen/DanLing nav: - DanLing: index.md - Runner: - runner/
 index.md - RunnerState: runner/runner_state.md - RunnerBase: runner/
 runner_base.md - BaseRunner: runner/base_runner.md - TorchRunner: runner/
 torch_runner.md - Utilities: runner/utils.md - Tensors: - NestedTensor:
 tensors/nested_tensor.md - PNTensor: tensors/pn_tensor.md - TorchFuncRegistry:
-tensors/torch_func_registry.md - Registry: registry.md - Metrics: -
-AverageMeter: metrics/average_meter.md - Utils: - Decorator: utils/
+tensors/torch_func_registry.md - Optim: - LRScheduler: optim/lr_scheduler.md -
+Metrics: - AverageMeter: metrics/average_meter.md - Utils: - Decorator: utils/
 decorators.md - IO: utils/io.md - basex: utils/basex.md - package: package.md #
 - Blog: blog/index.md theme: name: material custom_dir: overrides language:
 "zh" palette: - media: "(prefers-color-scheme: dark)" scheme: slate primary:
 blue grey accent: teal toggle: icon: material/brightness-4 name: Switch to
 light mode - media: "(prefers-color-scheme: light)" scheme: default primary:
 blue grey accent: teal toggle: icon: material/brightness-7 name: Switch to dark
 mode logo: "assets/images/logo.png" favicon: "assets/images/logo.ico" features:
```

### Comparing `danling-0.2.3/overrides/assets/fonts/CascadiaCodePL.woff2` & `danling-0.2.4/overrides/assets/fonts/CascadiaCodePL.woff2`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/overrides/assets/fonts/HYQiHei.ttf` & `danling-0.2.4/overrides/assets/fonts/HYQiHei.ttf`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/overrides/assets/fonts/HelveticaNowDisplay.otf` & `danling-0.2.4/overrides/assets/fonts/HelveticaNowDisplay.otf`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/overrides/assets/fonts/HelveticaWorld.ttf` & `danling-0.2.4/overrides/assets/fonts/HelveticaWorld.ttf`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/overrides/assets/images/favicon.ico` & `danling-0.2.4/overrides/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/overrides/assets/images/logo.png` & `danling-0.2.4/overrides/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/overrides/main.html` & `danling-0.2.4/overrides/main.html`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/pyproject.toml` & `danling-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `danling-0.2.3/tests/test_runner.py` & `danling-0.2.4/tests/test_runner.py`

 * *Files identical despite different names*

