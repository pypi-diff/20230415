# Comparing `tmp/neuralprophet-0.5.4.tar.gz` & `tmp/neuralprophet-0.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralprophet-0.5.4.tar", last modified: Sat Apr  8 02:01:17 2023, max compression
+gzip compressed data, was "neuralprophet-0.6.0rc1.tar", max compression
```

## Comparing `neuralprophet-0.5.4.tar` & `neuralprophet-0.6.0rc1.tar`

### file list

```diff
@@ -1,55 +1,44 @@
-drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-04-08 02:01:17.911363 neuralprophet-0.5.4/
--rw-r--r--   0 richard    (501) staff       (20)     1070 2022-11-24 05:34:19.000000 neuralprophet-0.5.4/LICENSE
--rw-r--r--   0 richard    (501) staff       (20)       55 2023-01-09 09:27:15.000000 neuralprophet-0.5.4/MANIFEST.in
--rw-r--r--   0 richard    (501) staff       (20)     8393 2023-04-08 02:01:17.911636 neuralprophet-0.5.4/PKG-INFO
--rw-r--r--   0 richard    (501) staff       (20)     7464 2023-03-04 23:25:03.000000 neuralprophet-0.5.4/README.md
-drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-04-08 02:01:17.898722 neuralprophet-0.5.4/neuralprophet/
--rw-r--r--   0 richard    (501) staff       (20)     1394 2023-04-07 19:13:56.000000 neuralprophet-0.5.4/neuralprophet/__init__.py
--rw-r--r--   0 richard    (501) staff       (20)      398 2023-03-04 23:25:03.000000 neuralprophet-0.5.4/neuralprophet/__main__.py
--rw-r--r--   0 richard    (501) staff       (20)       22 2023-04-08 01:58:46.000000 neuralprophet-0.5.4/neuralprophet/_version.py
-drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-04-08 02:01:17.903052 neuralprophet-0.5.4/neuralprophet/components/
--rw-r--r--   0 richard    (501) staff       (20)       46 2023-03-04 23:25:03.000000 neuralprophet-0.5.4/neuralprophet/components/__init__.py
--rw-r--r--   0 richard    (501) staff       (20)      931 2023-03-04 23:25:03.000000 neuralprophet-0.5.4/neuralprophet/components/base.py
-drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-04-08 02:01:17.904700 neuralprophet-0.5.4/neuralprophet/components/future_regressors/
--rw-r--r--   0 richard    (501) staff       (20)       49 2023-04-07 19:13:56.000000 neuralprophet-0.5.4/neuralprophet/components/future_regressors/__init__.py
--rw-r--r--   0 richard    (501) staff       (20)     1475 2023-04-07 19:13:56.000000 neuralprophet-0.5.4/neuralprophet/components/future_regressors/base.py
--rw-r--r--   0 richard    (501) staff       (20)     3681 2023-03-04 23:25:03.000000 neuralprophet-0.5.4/neuralprophet/components/future_regressors/linear.py
--rw-r--r--   0 richard    (501) staff       (20)     4037 2023-03-04 23:25:03.000000 neuralprophet-0.5.4/neuralprophet/components/router.py
-drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-04-08 02:01:17.906870 neuralprophet-0.5.4/neuralprophet/components/seasonality/
--rw-r--r--   0 richard    (501) staff       (20)       44 2023-04-07 19:13:56.000000 neuralprophet-0.5.4/neuralprophet/components/seasonality/__init__.py
--rw-r--r--   0 richard    (501) staff       (20)      546 2023-04-07 19:13:56.000000 neuralprophet-0.5.4/neuralprophet/components/seasonality/base.py
--rw-r--r--   0 richard    (501) staff       (20)     6220 2023-03-04 23:25:03.000000 neuralprophet-0.5.4/neuralprophet/components/seasonality/fourier.py
-drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-04-08 02:01:17.910775 neuralprophet-0.5.4/neuralprophet/components/trend/
--rw-r--r--   0 richard    (501) staff       (20)       38 2023-04-07 19:13:56.000000 neuralprophet-0.5.4/neuralprophet/components/trend/__init__.py
--rw-r--r--   0 richard    (501) staff       (20)     1057 2023-04-07 19:13:56.000000 neuralprophet-0.5.4/neuralprophet/components/trend/base.py
--rw-r--r--   0 richard    (501) staff       (20)     3826 2023-03-04 23:25:03.000000 neuralprophet-0.5.4/neuralprophet/components/trend/linear.py
--rw-r--r--   0 richard    (501) staff       (20)    16977 2023-03-04 23:25:03.000000 neuralprophet-0.5.4/neuralprophet/components/trend/piecewise_linear.py
--rw-r--r--   0 richard    (501) staff       (20)     1183 2023-03-04 23:25:03.000000 neuralprophet-0.5.4/neuralprophet/components/trend/static.py
--rw-r--r--   0 richard    (501) staff       (20)    16531 2023-04-07 19:13:56.000000 neuralprophet-0.5.4/neuralprophet/configure.py
--rw-r--r--   0 richard    (501) staff       (20)     1841 2023-03-04 23:25:03.000000 neuralprophet-0.5.4/neuralprophet/custom_loss_metrics.py
--rw-r--r--   0 richard    (501) staff       (20)    60172 2023-04-07 23:40:37.000000 neuralprophet-0.5.4/neuralprophet/df_utils.py
--rw-r--r--   0 richard    (501) staff       (20)   149943 2023-04-07 23:38:38.000000 neuralprophet-0.5.4/neuralprophet/forecaster.py
--rw-r--r--   0 richard    (501) staff       (20)      849 2023-03-04 23:25:03.000000 neuralprophet-0.5.4/neuralprophet/hdays_utils.py
--rw-r--r--   0 richard    (501) staff       (20)     2635 2023-03-04 23:25:03.000000 neuralprophet-0.5.4/neuralprophet/logger.py
--rw-r--r--   0 richard    (501) staff       (20)      601 2023-03-04 23:25:03.000000 neuralprophet-0.5.4/neuralprophet/np_types.py
--rw-r--r--   0 richard    (501) staff       (20)    18079 2023-03-04 23:25:03.000000 neuralprophet-0.5.4/neuralprophet/plot_forecast_matplotlib.py
--rw-r--r--   0 richard    (501) staff       (20)    25864 2023-03-04 23:25:03.000000 neuralprophet-0.5.4/neuralprophet/plot_forecast_plotly.py
--rw-r--r--   0 richard    (501) staff       (20)    28828 2023-03-04 23:25:03.000000 neuralprophet-0.5.4/neuralprophet/plot_model_parameters_matplotlib.py
--rw-r--r--   0 richard    (501) staff       (20)    33617 2023-03-04 23:25:03.000000 neuralprophet-0.5.4/neuralprophet/plot_model_parameters_plotly.py
--rw-r--r--   0 richard    (501) staff       (20)    25987 2023-03-04 23:25:03.000000 neuralprophet-0.5.4/neuralprophet/plot_utils.py
--rw-r--r--   0 richard    (501) staff       (20)    27597 2023-04-07 23:38:38.000000 neuralprophet-0.5.4/neuralprophet/time_dataset.py
--rw-r--r--   0 richard    (501) staff       (20)    42383 2023-04-07 19:13:56.000000 neuralprophet-0.5.4/neuralprophet/time_net.py
--rw-r--r--   0 richard    (501) staff       (20)    20958 2023-03-05 02:52:12.000000 neuralprophet-0.5.4/neuralprophet/torch_prophet.py
--rw-r--r--   0 richard    (501) staff       (20)    14246 2023-04-08 01:54:58.000000 neuralprophet-0.5.4/neuralprophet/uncertainty.py
--rw-r--r--   0 richard    (501) staff       (20)    31119 2023-04-07 19:13:56.000000 neuralprophet-0.5.4/neuralprophet/utils.py
--rw-r--r--   0 richard    (501) staff       (20)     1679 2023-03-04 23:25:03.000000 neuralprophet-0.5.4/neuralprophet/utils_metrics.py
--rw-r--r--   0 richard    (501) staff       (20)     4542 2023-03-04 23:25:03.000000 neuralprophet-0.5.4/neuralprophet/utils_torch.py
-drwxr-xr-x   0 richard    (501) staff       (20)        0 2023-04-08 02:01:17.901437 neuralprophet-0.5.4/neuralprophet.egg-info/
--rw-r--r--   0 richard    (501) staff       (20)     8393 2023-04-08 02:01:17.000000 neuralprophet-0.5.4/neuralprophet.egg-info/PKG-INFO
--rw-r--r--   0 richard    (501) staff       (20)     1546 2023-04-08 02:01:17.000000 neuralprophet-0.5.4/neuralprophet.egg-info/SOURCES.txt
--rw-r--r--   0 richard    (501) staff       (20)        1 2023-04-08 02:01:17.000000 neuralprophet-0.5.4/neuralprophet.egg-info/dependency_links.txt
--rw-r--r--   0 richard    (501) staff       (20)      638 2023-04-08 02:01:17.000000 neuralprophet-0.5.4/neuralprophet.egg-info/requires.txt
--rw-r--r--   0 richard    (501) staff       (20)       14 2023-04-08 02:01:17.000000 neuralprophet-0.5.4/neuralprophet.egg-info/top_level.txt
--rw-r--r--   0 richard    (501) staff       (20)      601 2023-04-07 21:28:32.000000 neuralprophet-0.5.4/pyproject.toml
--rw-r--r--   0 richard    (501) staff       (20)       96 2023-04-08 02:01:17.912530 neuralprophet-0.5.4/setup.cfg
--rw-r--r--   0 richard    (501) staff       (20)     2014 2023-01-09 09:27:16.000000 neuralprophet-0.5.4/setup.py
+-rw-r--r--   0        0        0     1070 2022-11-24 05:34:19.680929 neuralprophet-0.6.0rc1/LICENSE
+-rw-r--r--   0        0        0     7464 2023-04-15 04:16:53.611613 neuralprophet-0.6.0rc1/README.md
+-rw-r--r--   0        0        0     1394 2023-04-15 04:16:53.703131 neuralprophet-0.6.0rc1/neuralprophet/__init__.py
+-rw-r--r--   0        0        0      398 2023-04-15 04:16:53.703711 neuralprophet-0.6.0rc1/neuralprophet/__main__.py
+-rw-r--r--   0        0        0       25 2023-04-15 04:17:20.775326 neuralprophet-0.6.0rc1/neuralprophet/_version.py
+-rw-r--r--   0        0        0      683 2023-04-15 04:16:53.704907 neuralprophet-0.6.0rc1/neuralprophet/components/README.md
+-rw-r--r--   0        0        0       46 2023-04-15 04:16:53.705091 neuralprophet-0.6.0rc1/neuralprophet/components/__init__.py
+-rw-r--r--   0        0        0      931 2023-04-15 04:16:53.706486 neuralprophet-0.6.0rc1/neuralprophet/components/base.py
+-rw-r--r--   0        0        0       49 2023-04-15 04:16:53.707158 neuralprophet-0.6.0rc1/neuralprophet/components/future_regressors/__init__.py
+-rw-r--r--   0        0        0     1475 2023-04-15 04:16:53.707535 neuralprophet-0.6.0rc1/neuralprophet/components/future_regressors/base.py
+-rw-r--r--   0        0        0     3681 2023-04-15 04:16:53.708049 neuralprophet-0.6.0rc1/neuralprophet/components/future_regressors/linear.py
+-rw-r--r--   0        0        0     4037 2023-04-15 04:16:53.708543 neuralprophet-0.6.0rc1/neuralprophet/components/router.py
+-rw-r--r--   0        0        0       44 2023-04-15 04:16:53.708862 neuralprophet-0.6.0rc1/neuralprophet/components/seasonality/__init__.py
+-rw-r--r--   0        0        0      546 2023-04-15 04:16:53.709089 neuralprophet-0.6.0rc1/neuralprophet/components/seasonality/base.py
+-rw-r--r--   0        0        0     6220 2023-04-15 04:16:53.709368 neuralprophet-0.6.0rc1/neuralprophet/components/seasonality/fourier.py
+-rw-r--r--   0        0        0       38 2023-04-15 04:16:53.709633 neuralprophet-0.6.0rc1/neuralprophet/components/trend/__init__.py
+-rw-r--r--   0        0        0     1057 2023-04-15 04:16:53.709985 neuralprophet-0.6.0rc1/neuralprophet/components/trend/base.py
+-rw-r--r--   0        0        0     3826 2023-04-15 04:16:53.710238 neuralprophet-0.6.0rc1/neuralprophet/components/trend/linear.py
+-rw-r--r--   0        0        0    16977 2023-04-15 04:16:53.710507 neuralprophet-0.6.0rc1/neuralprophet/components/trend/piecewise_linear.py
+-rw-r--r--   0        0        0     1198 2023-04-15 04:16:53.711296 neuralprophet-0.6.0rc1/neuralprophet/components/trend/static.py
+-rw-r--r--   0        0        0    16531 2023-04-15 04:16:53.712670 neuralprophet-0.6.0rc1/neuralprophet/configure.py
+-rw-r--r--   0        0        0     1841 2023-04-15 04:16:53.714315 neuralprophet-0.6.0rc1/neuralprophet/custom_loss_metrics.py
+-rw-r--r--   0        0        0    23809 2023-04-15 04:16:53.715073 neuralprophet-0.6.0rc1/neuralprophet/data/process.py
+-rw-r--r--   0        0        0     6803 2023-04-15 04:16:53.716051 neuralprophet-0.6.0rc1/neuralprophet/data/split.py
+-rw-r--r--   0        0        0      878 2023-04-15 04:16:53.716561 neuralprophet-0.6.0rc1/neuralprophet/data/transform.py
+-rw-r--r--   0        0        0    63826 2023-04-15 04:16:53.717906 neuralprophet-0.6.0rc1/neuralprophet/df_utils.py
+-rw-r--r--   0        0        0   121126 2023-04-15 04:16:53.719900 neuralprophet-0.6.0rc1/neuralprophet/forecaster.py
+-rw-r--r--   0        0        0      849 2023-04-15 04:16:53.721434 neuralprophet-0.6.0rc1/neuralprophet/hdays_utils.py
+-rw-r--r--   0        0        0     2635 2023-04-15 04:16:53.722875 neuralprophet-0.6.0rc1/neuralprophet/logger.py
+-rw-r--r--   0        0        0      601 2023-04-14 18:24:09.467754 neuralprophet-0.6.0rc1/neuralprophet/np_types.py
+-rw-r--r--   0        0        0    20046 2023-04-15 04:16:53.724158 neuralprophet-0.6.0rc1/neuralprophet/plot_forecast_matplotlib.py
+-rw-r--r--   0        0        0    28793 2023-04-15 04:16:53.725746 neuralprophet-0.6.0rc1/neuralprophet/plot_forecast_plotly.py
+-rw-r--r--   0        0        0    28822 2023-04-15 04:16:53.726943 neuralprophet-0.6.0rc1/neuralprophet/plot_model_parameters_matplotlib.py
+-rw-r--r--   0        0        0    33617 2023-04-15 04:16:53.728146 neuralprophet-0.6.0rc1/neuralprophet/plot_model_parameters_plotly.py
+-rw-r--r--   0        0        0    25987 2023-04-15 04:16:53.729478 neuralprophet-0.6.0rc1/neuralprophet/plot_utils.py
+-rw-r--r--   0        0        0    29297 2023-04-15 04:16:53.731451 neuralprophet-0.6.0rc1/neuralprophet/time_dataset.py
+-rw-r--r--   0        0        0    42383 2023-04-15 04:16:53.734947 neuralprophet-0.6.0rc1/neuralprophet/time_net.py
+-rw-r--r--   0        0        0    20958 2023-04-14 18:24:09.472906 neuralprophet-0.6.0rc1/neuralprophet/torch_prophet.py
+-rw-r--r--   0        0        0    19981 2023-04-15 04:16:53.737476 neuralprophet-0.6.0rc1/neuralprophet/uncertainty.py
+-rw-r--r--   0        0        0    31119 2023-04-15 04:16:53.738755 neuralprophet-0.6.0rc1/neuralprophet/utils.py
+-rw-r--r--   0        0        0     1679 2023-04-15 04:16:53.739371 neuralprophet-0.6.0rc1/neuralprophet/utils_metrics.py
+-rw-r--r--   0        0        0     4542 2023-04-15 04:16:53.740338 neuralprophet-0.6.0rc1/neuralprophet/utils_torch.py
+-rw-r--r--   0        0        0     1773 2023-04-15 04:17:13.016717 neuralprophet-0.6.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     8535 1970-01-01 00:00:00.000000 neuralprophet-0.6.0rc1/PKG-INFO
```

### Comparing `neuralprophet-0.5.4/LICENSE` & `neuralprophet-0.6.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.5.4/PKG-INFO` & `neuralprophet-0.6.0rc1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: neuralprophet
-Version: 0.5.4
-Summary: Explainable Forecasting at Scale
-Home-page: https://github.com/ourownstory/neural_prophet
-Author: Oskar Triebe
-Author-email: trieb@stanford.edu
-License: MIT
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: live
-License-File: LICENSE
-
 [![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/ourownstory/neural_prophet?logo=github)](https://github.com/ourownstory/neural_prophet/releases)
 [![Pypi_Version](https://img.shields.io/pypi/v/neuralprophet.svg)](https://pypi.python.org/pypi/neuralprophet)
 [![Python Version](https://img.shields.io/badge/python-3.7+-blue?logo=python)](https://www.python.org/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License](https://img.shields.io/badge/license-MIT-brightgreen)](https://opensource.org/licenses/MIT)
 [![Tests](https://github.com/ourownstory/neural_prophet/actions/workflows/ci.yml/badge.svg)](https://github.com/ourownstory/neural_prophet/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/ourownstory/neural_prophet/branch/master/graph/badge.svg?token=U5KXCL55DW)](https://codecov.io/gh/ourownstory/neural_prophet)
```

### Comparing `neuralprophet-0.5.4/README.md` & `neuralprophet-0.6.0rc1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,34 @@
+Metadata-Version: 2.1
+Name: neuralprophet
+Version: 0.6.0rc1
+Summary: NeuralProphet is an easy to learn framework for interpretable time series forecasting.
+License: MIT
+Author: Oskar Triebe
+Author-email: triebe@stanford.edu
+Requires-Python: >=3.7.1,<3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: captum (>=0.6.0,<0.7.0)
+Requires-Dist: holidays (>=0.21,<0.22)
+Requires-Dist: matplotlib (>=3.5.3,<4.0.0)
+Requires-Dist: numpy (>=1.21.6,<1.24.0)
+Requires-Dist: pandas (>=1.3.5,<2.0.0)
+Requires-Dist: plotly (>=5.13.1,<6.0.0)
+Requires-Dist: plotly-resampler (>=0.8.3.1,<0.9.0.0)
+Requires-Dist: pytorch-lightning (>=1.9.4,<2.0.0)
+Requires-Dist: tensorboard (>=2.11.2,<3.0.0)
+Requires-Dist: torch (>=1.13.1,<2.0.0)
+Requires-Dist: torchmetrics (>=0.11.3,<0.12.0)
+Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
+Description-Content-Type: text/markdown
+
 [![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/ourownstory/neural_prophet?logo=github)](https://github.com/ourownstory/neural_prophet/releases)
 [![Pypi_Version](https://img.shields.io/pypi/v/neuralprophet.svg)](https://pypi.python.org/pypi/neuralprophet)
 [![Python Version](https://img.shields.io/badge/python-3.7+-blue?logo=python)](https://www.python.org/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License](https://img.shields.io/badge/license-MIT-brightgreen)](https://opensource.org/licenses/MIT)
 [![Tests](https://github.com/ourownstory/neural_prophet/actions/workflows/ci.yml/badge.svg)](https://github.com/ourownstory/neural_prophet/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/ourownstory/neural_prophet/branch/master/graph/badge.svg?token=U5KXCL55DW)](https://codecov.io/gh/ourownstory/neural_prophet)
@@ -133,7 +160,8 @@
       primaryClass={cs.LG}
 }
 ```
 
 ## About
 NeuralProphet is and open-source community project, supported by awesome people like you. 
 If you are interested in joining the project, please feel free to reach out to me (Oskar) - you can find my email on the [NeuralProphet Paper](https://arxiv.org/abs/2111.15397).
+
```

### Comparing `neuralprophet-0.5.4/neuralprophet/__init__.py` & `neuralprophet-0.6.0rc1/neuralprophet/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.5.4/neuralprophet/components/base.py` & `neuralprophet-0.6.0rc1/neuralprophet/components/base.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.5.4/neuralprophet/components/future_regressors/base.py` & `neuralprophet-0.6.0rc1/neuralprophet/components/future_regressors/base.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.5.4/neuralprophet/components/future_regressors/linear.py` & `neuralprophet-0.6.0rc1/neuralprophet/components/future_regressors/linear.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.5.4/neuralprophet/components/router.py` & `neuralprophet-0.6.0rc1/neuralprophet/components/router.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.5.4/neuralprophet/components/seasonality/base.py` & `neuralprophet-0.6.0rc1/neuralprophet/components/seasonality/base.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.5.4/neuralprophet/components/seasonality/fourier.py` & `neuralprophet-0.6.0rc1/neuralprophet/components/seasonality/fourier.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.5.4/neuralprophet/components/trend/base.py` & `neuralprophet-0.6.0rc1/neuralprophet/components/trend/base.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.5.4/neuralprophet/components/trend/linear.py` & `neuralprophet-0.6.0rc1/neuralprophet/components/trend/linear.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.5.4/neuralprophet/components/trend/piecewise_linear.py` & `neuralprophet-0.6.0rc1/neuralprophet/components/trend/piecewise_linear.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.5.4/neuralprophet/components/trend/static.py` & `neuralprophet-0.6.0rc1/neuralprophet/components/trend/static.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,15 @@
                 Metadata about the all the samples of the model input batch. Contains the following:
                     * ``df_name`` (list, str), time series ID corresponding to each sample of the input batch.
         Returns
         -------
             torch.Tensor
                 Trend component, same dimensions as input t
         """
-        return self.bias.unsqueeze(dim=0).repeat(t.shape[0], 1, 1)
+        return self.bias.unsqueeze(dim=0).repeat(t.shape[0], self.n_forecasts, 1)
 
     @property
     def get_trend_deltas(self):
         pass
 
     def add_regularization(self):
         pass
```

### Comparing `neuralprophet-0.5.4/neuralprophet/configure.py` & `neuralprophet-0.6.0rc1/neuralprophet/configure.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.5.4/neuralprophet/custom_loss_metrics.py` & `neuralprophet-0.6.0rc1/neuralprophet/custom_loss_metrics.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.5.4/neuralprophet/df_utils.py` & `neuralprophet-0.6.0rc1/neuralprophet/df_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,17 +204,21 @@
             norm_type=normalize,
         )
 
     if config_lagged_regressors is not None:
         for covar in config_lagged_regressors.keys():
             if covar not in df.columns:
                 raise ValueError(f"Lagged regressor {covar} not found in DataFrame.")
+            norm_type_lag = config_lagged_regressors[covar].normalize
+            if local_run_despite_global:
+                if len(df[covar].unique()) < 2:
+                    norm_type_lag = "soft"
             data_params[covar] = get_normalization_params(
                 array=df[covar].values,
-                norm_type=config_lagged_regressors[covar].normalize,
+                norm_type=norm_type_lag,
             )
 
     if config_regressors is not None:
         for reg in config_regressors.keys():
             if reg not in df.columns:
                 raise ValueError(f"Regressor {reg} not found in DataFrame.")
             norm_type = config_regressors[reg].normalize
@@ -453,14 +457,21 @@
     if regressors is not None:
         for reg in regressors:
             if len(df[reg].unique()) < 2:
                 log.warning(
                     "Encountered future regressor with only unique values in training set. "
                     "Variable will be removed for global modeling if this is true for all time series."
                 )
+    if covariates is not None:
+        for covar in covariates:
+            if len(df[covar].unique()) < 2:
+                log.warning(
+                    "Encountered lagged regressor with only unique values in training set. "
+                    "Variable will be removed for global modeling if this is true for all time series."
+                )
 
     columns = []
     if check_y:
         columns.append("y")
     if covariates is not None:
         if type(covariates) is list:
             columns.extend(covariates)
@@ -499,15 +510,21 @@
         df.index.name = None
     df = df.sort_values("ds")
     df = df.reset_index(drop=True)
     return df
 
 
 def check_dataframe(
-    df: pd.DataFrame, check_y: bool = True, covariates=None, regressors=None, events=None, seasonalities=None
+    df: pd.DataFrame,
+    check_y: bool = True,
+    covariates=None,
+    regressors=None,
+    events=None,
+    seasonalities=None,
+    future: Optional[bool] = None,
 ) -> Tuple[pd.DataFrame, List]:
     """Performs basic data sanity checks and ordering,
     as well as prepare dataframe for fitting or predicting.
 
     Parameters
     ----------
         df : pd.DataFrame
@@ -519,14 +536,16 @@
             covariate column names
         regressors : list or dict
             regressor column names
         events : list or dict
             event column names
         seasonalities : list or dict
             seasonalities column names
+        future : bool
+            if df is a future dataframe
 
     Returns
     -------
         pd.DataFrame or dict
             checked dataframe
     """
     df, _, _, _ = prep_or_copy_df(df)
@@ -541,14 +560,24 @@
         for reg in regressors:
             if len(df[reg].unique()) < 2:
                 log.warning(
                     "Encountered future regressor with only unique values in training set across all IDs."
                     "Automatically removed variable."
                 )
                 regressors_to_remove.append(reg)
+    if future:
+        return checked_df, regressors_to_remove
+    if covariates is not None:
+        for covar in covariates:
+            if len(df[covar].unique()) < 2:
+                log.warning(
+                    "Encountered lagged regressor with only unique values in training set across all IDs."
+                    "Automatically removed variable."
+                )
+                regressors_to_remove.append(covar)
     if len(regressors_to_remove) > 0:
         regressors_to_remove = list(set(regressors_to_remove))
         checked_df = checked_df.drop(*regressors_to_remove, axis=1)
         assert checked_df is not None
     return checked_df, regressors_to_remove
 
 
@@ -1232,14 +1261,37 @@
     # get distribution considering the two most common frequencies - useful for monthly and business day
     f1 = dist.max()
     dist = np.delete(dist, np.argmax(dist))
     f2 = dist.max()
     return f1 + f2
 
 
+def _get_dominant_frequency_percentage(frequencies, distribution, filter_list) -> float:
+    """Calculate dominant frequency percentage of dataframe.
+
+    Parameters
+    ----------
+        frequencies : list
+            list of numeric delta values (``ms``) of frequencies
+        distribution : list
+            list of occasions of frequencies
+        filter_list : list
+            list of frequencies to be filtered
+
+    Returns
+    -------
+        float
+            Percentage of dominant frequency within the whole dataframe
+
+    """
+    dominant_frequencies = [freq for freq in frequencies if freq in filter_list]
+    dominant_distribution = [distribution[np.where(frequencies == freq)] for freq in dominant_frequencies]
+    return sum(dominant_distribution) / sum(distribution)
+
+
 def _infer_frequency(df, freq, min_freq_percentage=0.7):
     """Automatically infers frequency of dataframe.
 
     Parameters
     ----------
         df : pd.DataFrame
             Dataframe with columns ``ds`` datestamps and ``y`` time series values
@@ -1257,53 +1309,53 @@
     Returns
     -------
         str
             Valid frequency tag according to major frequency.
 
     """
     frequencies, distribution = get_freq_dist(df["ds"])
-    # exception - monthly df (31 days freq or 30 days freq)
-    if frequencies[np.argmax(distribution)] == 2.6784e15 or frequencies[np.argmax(distribution)] == 2.592e15:
-        dominant_freq_percentage = get_dist_considering_two_freqs(distribution) / len(df["ds"])
+    argmax_frequency = frequencies[np.argmax(distribution)]
+
+    # exception - monthly df (28, 29, 30 or 31 days freq)
+    MONTHLY_FREQUENCIES = [2.4192e15, 2.5056e15, 2.5920e15, 2.6784e15]
+    if argmax_frequency in MONTHLY_FREQUENCIES:
+        dominant_freq_percentage = _get_dominant_frequency_percentage(frequencies, distribution, MONTHLY_FREQUENCIES)
         num_freq = 2.6784e15
         inferred_freq = "MS" if pd.to_datetime(df["ds"].iloc[0]).day < 15 else "M"
     # exception - yearly df (365 days freq or 366 days freq)
-    elif frequencies[np.argmax(distribution)] == 3.1536e16 or frequencies[np.argmax(distribution)] == 3.16224e16:
+    elif argmax_frequency == 3.1536e16 or argmax_frequency == 3.16224e16:
         dominant_freq_percentage = get_dist_considering_two_freqs(distribution) / len(df["ds"])
         num_freq = 3.1536e16
         inferred_freq = "YS" if pd.to_datetime(df["ds"].iloc[0]).day < 15 else "Y"
     # exception - quarterly df (most common == 92 days - 3rd,4th quarters and second most common == 91 days 2nd quarter and 1st quarter in leap year)
-    elif (
-        frequencies[np.argmax(distribution)] == 7.9488e15
-        and frequencies[np.argsort(distribution, axis=0)[-2]] == 7.8624e15
-    ):
+    elif argmax_frequency == 7.9488e15 and frequencies[np.argsort(distribution, axis=0)[-2]] == 7.8624e15:
         dominant_freq_percentage = get_dist_considering_two_freqs(distribution) / len(df["ds"])
         num_freq = 7.9488e15
         inferred_freq = "QS" if pd.to_datetime(df["ds"].iloc[0]).day < 15 else "Q"
     # exception - Business day (most common == day delta and second most common == 3 days delta and second most common is at least 12% of the deltas)
     elif (
-        frequencies[np.argmax(distribution)] == 8.64e13
+        argmax_frequency == 8.64e13
         and frequencies[np.argsort(distribution, axis=0)[-2]] == 2.592e14
         and distribution[np.argsort(distribution, axis=0)[-2]] / len(df["ds"]) >= 0.12
     ):
         dominant_freq_percentage = get_dist_considering_two_freqs(distribution) / len(df["ds"])
         num_freq = 8.64e13
         inferred_freq = "B"
     # exception - Business hour (most common == hour delta and second most common == 17 hours delta and second most common is at least 8% of the deltas)
     elif (
-        frequencies[np.argmax(distribution)] == 3.6e12
+        argmax_frequency == 3.6e12
         and frequencies[np.argsort(distribution, axis=0)[-2]] == 6.12e13
         and distribution[np.argsort(distribution, axis=0)[-2]] / len(df["ds"]) >= 0.08
     ):
         dominant_freq_percentage = get_dist_considering_two_freqs(distribution) / len(df["ds"])
         num_freq = 3.6e12
         inferred_freq = "BH"
     else:
         dominant_freq_percentage = distribution.max() / len(df["ds"])
-        num_freq = frequencies[np.argmax(distribution)]  # get value of most common diff
+        num_freq = argmax_frequency  # get value of most common diff
         inferred_freq = convert_num_to_str_freq(num_freq, df["ds"].iloc[0])
 
     log.info(
         f"Major frequency {inferred_freq} corresponds to {np.round(dominant_freq_percentage * 100, 3)}% of the data."
     )
     ideal_freq_exists = True if dominant_freq_percentage >= min_freq_percentage else False
     if ideal_freq_exists:
@@ -1598,7 +1650,57 @@
         pd.DataFrame
             dataframe with added columns for conditional seasonalities
     """
     df["ds"] = pd.to_datetime(df["ds"])
     df["weekend"] = df["ds"].apply(lambda x: x.weekday() in [5, 6]).astype(int)
     df["weekday"] = df["ds"].apply(lambda x: x.weekday() in [0, 1, 2, 3, 4]).astype(int)
     return df
+
+
+def create_mask_for_prediction_frequency(prediction_frequency, ds, forecast_lag):
+    """Creates a mask for the yhat array, to select the correct values for the prediction frequency.
+    This method is only called in _reshape_raw_predictions_to_forecst_df within NeuralProphet.predict().
+
+    Parameters
+    ----------
+        prediction_frequency : dict
+            identical to NeuralProphet
+        ds : pd.Series
+            datestamps of the predictions
+        forecast_lag : int
+            current forecast lag
+
+    Returns
+    -------
+        np.array
+            mask for the yhat array
+    """
+    masks = []
+    for count, (key, value) in enumerate(prediction_frequency.items()):
+        if count > 0 and forecast_lag > 1:
+            target_time = value + 1
+        else:
+            target_time = value + forecast_lag
+        if key == "daily-hour":
+            target_time = target_time % 24
+            mask = ds.dt.hour == target_time
+        elif key == "weekly-day":
+            target_time = target_time % 7
+            mask = ds.dt.dayofweek == target_time
+        elif key == "monthly-day":
+            num_days = ds.dt.daysinmonth
+            target_time = target_time % num_days
+            mask = (ds.dt.day == target_time).reset_index(drop=True)
+        elif key == "yearly-month":
+            target_time = target_time % 12 if target_time > 12 else target_time
+            target_time = 1 if target_time == 0 else target_time
+            mask = ds.dt.month == target_time
+        elif key == "hourly-minute":
+            target_time = target_time % 60
+            mask = ds.dt.minute == target_time
+        else:
+            raise ValueError(f"prediction_frequency {key} not supported")
+        masks.append(mask)
+    mask = np.ones((len(ds),), dtype=bool)
+    for m in masks:
+        mask = mask & m
+    return mask
```

### Comparing `neuralprophet-0.5.4/neuralprophet/forecaster.py` & `neuralprophet-0.6.0rc1/neuralprophet/forecaster.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,25 @@
 import pytorch_lightning as pl
 import torch
 from matplotlib import pyplot
 from matplotlib.axes import Axes
 from torch.utils.data import DataLoader
 
 from neuralprophet import configure, df_utils, np_types, time_dataset, time_net, utils, utils_metrics
+from neuralprophet.data.process import (
+    _check_dataframe,
+    _convert_raw_predictions_to_raw_df,
+    _create_dataset,
+    _handle_missing_data,
+    _prepare_dataframe_to_predict,
+    _reshape_raw_predictions_to_forecst_df,
+    _validate_column_name,
+)
+from neuralprophet.data.split import _make_future_dataframe, _maybe_extend_df
+from neuralprophet.data.transform import _normalize
 from neuralprophet.logger import MetricsLogger
 from neuralprophet.plot_forecast_matplotlib import plot, plot_components
 from neuralprophet.plot_forecast_plotly import plot as plot_plotly
 from neuralprophet.plot_forecast_plotly import plot_components as plot_components_plotly
 from neuralprophet.plot_model_parameters_matplotlib import plot_parameters
 from neuralprophet.plot_model_parameters_plotly import plot_parameters as plot_parameters_plotly
 from neuralprophet.plot_utils import get_valid_configuration, log_warning_deprecation_plotly, select_plotting_backend
@@ -292,20 +303,29 @@
                 * ``True``: test data is normalized with global data params even if trained with local data params (global modeling with local normalization)
                 * (default) ``False``: no global modeling with local normalization
         accelerator: str
             Name of accelerator from pytorch_lightning.accelerators to use for training. Use "auto" to automatically select an available accelerator.
             Provide `None` to deactivate the use of accelerators.
         trainer_config: dict
             Dictionary of additional trainer configuration parameters.
-        prediction_frequency: int
+        prediction_frequency: dict
             periodic interval in which forecasts should be made.
+            More than one item only allowed for {"daily-hour": x, "weekly-day": y"} to forecast on a specific hour of a specific day of week.
 
-            Note
-            ----
-            E.g. if prediction_frequency=7, forecasts are only made on every 7th step (once in a week in case of daily resolution).
+            Key: str
+                periodicity of the predictions to be made.
+            value: int
+                forecast origin of the predictions to be made, e.g. 7 for 7am in case of 'daily-hour'.
+
+            Options
+                * ``'hourly-minute'``: forecast once per hour at a specified minute
+                * ``'daily-hour'``: forecast once per day at a specified hour
+                * ``'weekly-day'``: forecast once per week at a specified day
+                * ``'monthly-day'``: forecast once per month at a specified day
+                * ``'yearly-month'``: forecast once per year at a specified month
     """
 
     model: time_net.TimeNet
     trainer: pl.Trainer
 
     def __init__(
         self,
@@ -342,15 +362,15 @@
         collect_metrics: np_types.CollectMetricsMode = True,
         normalize: np_types.NormalizeMode = "auto",
         global_normalization: bool = False,
         global_time_normalization: bool = True,
         unknown_data_normalization: bool = False,
         accelerator: Optional[str] = None,
         trainer_config: dict = {},
-        prediction_frequency: Optional[int] = None,
+        prediction_frequency: Optional[dict] = None,
     ):
         self.config = locals()
         self.config.pop("self")
 
         # General
         self.name = "NeuralProphet"
         self.n_forecasts = n_forecasts
@@ -485,14 +505,15 @@
                 optional  scale for regularization strength
             normalize : bool
                 optional, specify whether this regressor will benormalized prior to fitting.
                 if ``auto``, binary regressors will not be normalized.
         """
         if num_hidden_layers is None:
             num_hidden_layers = self.config_model.num_hidden_layers
+
         if d_hidden is None:
             d_hidden = self.config_model.d_hidden
         if n_lags == 0 or n_lags is None:
             n_lags = 0
             log.warning(
                 "Please, set n_lags to a value greater than 0 or to the options 'scalar' or 'auto'. No lags will be added to regressors when n_lags = 0 or n_lags is None"
             )
@@ -512,15 +533,15 @@
             log.info("n_lags = 'scalar', number of lags for regressor is set to 1")
         only_last_value = False if n_lags > 1 else True
         if self.fitted:
             raise Exception("Regressors must be added prior to model fitting.")
         if not isinstance(names, list):
             names = [names]
         for name in names:
-            self._validate_column_name(name)
+            _validate_column_name(self, name)
             if self.config_lagged_regressors is None:
                 self.config_lagged_regressors = OrderedDict()
             self.config_lagged_regressors[name] = configure.LaggedRegressor(
                 reg_lambda=regularization,
                 normalize=normalize,
                 as_scalar=only_last_value,
                 n_lags=n_lags,
@@ -580,15 +601,15 @@
         if self.fitted:
             raise Exception("Regressors must be added prior to model fitting.")
         if regularization is not None:
             if regularization < 0:
                 raise ValueError("regularization must be >= 0")
             if regularization == 0:
                 regularization = None
-        self._validate_column_name(name)
+        _validate_column_name(self, name)
 
         if self.config_regressors is None:
             self.config_regressors = OrderedDict()
         self.config_regressors[name] = configure.Regressor(reg_lambda=regularization, normalize=normalize, mode=mode)
         return self
 
     def add_events(
@@ -629,15 +650,15 @@
             if regularization == 0:
                 regularization = None
 
         if not isinstance(events, list):
             events = [events]
 
         for event_name in events:
-            self._validate_column_name(event_name)
+            _validate_column_name(self, event_name)
             self.config_events[event_name] = configure.Event(
                 lower_window=lower_window, upper_window=upper_window, reg_lambda=regularization, mode=mode
             )
         return self
 
     def add_country_holidays(
         self,
@@ -736,17 +757,17 @@
             >>> m.add_seasonality(name="weekly_fall", period=7, fourier_order=4, condition_name="fall")
         """
         if self.fitted:
             raise Exception("Seasonality must be added prior to model fitting.")
         if name in ["daily", "weekly", "yearly"]:
             log.error("Please use inbuilt daily, weekly, or yearly seasonality or set another name.")
         # Do not Allow overwriting built-in seasonalities
-        self._validate_column_name(name, seasons=True)
+        _validate_column_name(self, name, seasons=True)
         if condition_name is not None:
-            self._validate_column_name(condition_name)
+            _validate_column_name(self, condition_name)
         if fourier_order <= 0:
             raise ValueError("Fourier Order must be > 0")
         self.config_seasonality.append(
             name=name, period=period, resolution=fourier_order, condition_name=condition_name, arg="custom"
         )
         return self
 
@@ -863,17 +884,17 @@
             checkpointing = False
             self.metrics = False
             progress = None
 
         # Pre-processing
         # Copy df and save list of unique time series IDs (the latter for global-local modelling if enabled)
         df, _, _, self.id_list = df_utils.prep_or_copy_df(df)
-        df = self._check_dataframe(df, check_y=True, exogenous=True)
+        df = _check_dataframe(self, df, check_y=True, exogenous=True)
         self.data_freq = df_utils.infer_frequency(df, n_lags=self.max_lags, freq=freq)
-        df = self._handle_missing_data(df, freq=self.data_freq)
+        df = _handle_missing_data(self, df, freq=self.data_freq)
 
         # Setup for global-local modelling: If there is only a single time series, then self.id_list = ['__df__']
         self.num_trends_modelled = len(self.id_list) if self.config_trend.trend_global_local == "local" else 1
         self.num_seasonalities_modelled = len(self.id_list) if self.config_seasonality.global_local == "local" else 1
         self.meta_used_in_model = self.num_trends_modelled != 1 or self.num_seasonalities_modelled != 1
 
         if self.fitted is True and not continue_training:
@@ -895,16 +916,16 @@
                 metrics_enabled=bool(self.metrics),
                 checkpointing_enabled=checkpointing,
                 continue_training=continue_training,
                 num_workers=num_workers,
             )
         else:
             df_val, _, _, _ = df_utils.prep_or_copy_df(validation_df)
-            df_val = self._check_dataframe(df_val, check_y=False, exogenous=False)
-            df_val = self._handle_missing_data(df_val, freq=self.data_freq)
+            df_val = _check_dataframe(self, df_val, check_y=False, exogenous=False)
+            df_val = _handle_missing_data(self, df_val, freq=self.data_freq)
             metrics_df = self._train(
                 df,
                 df_val=df_val,
                 progress_bar_enabled=bool(progress),
                 metrics_enabled=bool(self.metrics),
                 checkpointing_enabled=checkpointing,
                 continue_training=continue_training,
@@ -964,33 +985,33 @@
         """
         if raw:
             log.warning("Raw forecasts are incompatible with plotting utilities")
         if self.fitted is False:
             raise ValueError("Model has not been fitted. Predictions will be random.")
         df, received_ID_col, received_single_time_series, _ = df_utils.prep_or_copy_df(df)
         # to get all forecasteable values with df given, maybe extend into future:
-        df, periods_added = self._maybe_extend_df(df)
-        df = self._prepare_dataframe_to_predict(df)
+        df, periods_added = _maybe_extend_df(self, df)
+        df = _prepare_dataframe_to_predict(self, df)
         # normalize
-        df = self._normalize(df)
+        df = _normalize(self, df)
         forecast = pd.DataFrame()
         for df_name, df_i in df.groupby("ID"):
             dates, predicted, components = self._predict_raw(
                 df_i, df_name, include_components=decompose, prediction_frequency=self.prediction_frequency
             )
             df_i = df_utils.drop_missing_from_df(
                 df_i, self.config_missing.drop_missing, self.predict_steps, self.n_lags
             )
             if raw:
-                fcst = self._convert_raw_predictions_to_raw_df(dates, predicted, components)
+                fcst = _convert_raw_predictions_to_raw_df(self, dates, predicted, components)
                 if periods_added[df_name] > 0:
                     fcst = fcst[:-1]
             else:
-                fcst = self._reshape_raw_predictions_to_forecst_df(
-                    df_i, predicted, components, self.prediction_frequency
+                fcst = _reshape_raw_predictions_to_forecst_df(
+                    self, df_i, predicted, components, self.prediction_frequency, dates
                 )
                 if periods_added[df_name] > 0:
                     fcst = fcst[: -periods_added[df_name]]
             forecast = pd.concat((forecast, fcst), ignore_index=True)
         df = df_utils.return_df_in_original_format(forecast, received_ID_col, received_single_time_series)
         self.predict_steps = self.n_forecasts
         return df
@@ -1006,17 +1027,17 @@
         -------
             pd.DataFrame
                 evaluation metrics
         """
         df, _, _, _ = df_utils.prep_or_copy_df(df)
         if self.fitted is False:
             log.warning("Model has not been fitted. Test results will be random.")
-        df = self._check_dataframe(df, check_y=True, exogenous=True)
+        df = _check_dataframe(self, df, check_y=True, exogenous=True)
         _ = df_utils.infer_frequency(df, n_lags=self.max_lags, freq=self.data_freq)
-        df = self._handle_missing_data(df, freq=self.data_freq)
+        df = _handle_missing_data(self, df, freq=self.data_freq)
         loader = self._init_val_loader(df)
         # Use Lightning to calculate metrics
         val_metrics = self.trainer.test(self.model, dataloaders=loader)
         val_metrics_df = pd.DataFrame(val_metrics)
         # TODO Check whether supported by Lightning
         if not self.config_normalization.global_normalization:
             log.warning("Note that the metrics are displayed in normalized scale because of local normalization.")
@@ -1131,17 +1152,17 @@
             >>> df_val
                 ds	y	ID
             0	2022-12-05	7.89	data1
             1	2022-12-13	8.02	data2
             2	2022-12-13	8.30	data3
         """
         df, received_ID_col, received_single_time_series, _ = df_utils.prep_or_copy_df(df)
-        df = self._check_dataframe(df, check_y=False, exogenous=False)
+        df = _check_dataframe(self, df, check_y=False, exogenous=False)
         freq = df_utils.infer_frequency(df, n_lags=self.max_lags, freq=freq)
-        df = self._handle_missing_data(df, freq=freq, predicting=False)
+        df = _handle_missing_data(self, df, freq=freq, predicting=False)
         df_train, df_val = df_utils.split_df(
             df,
             n_lags=self.max_lags,
             n_forecasts=self.n_forecasts,
             valid_p=valid_p,
             inputs_overbleed=True,
             local_split=local_split,
@@ -1299,17 +1320,17 @@
             >>> folds[1][1]
                 ds	y	ID
             0	2022-12-10	8.09	data1
             1	2022-12-10	8.25	data2
             2	2022-12-10	7.55	data3
         """
         df, received_ID_col, received_single_time_series, _ = df_utils.prep_or_copy_df(df)
-        df = self._check_dataframe(df, check_y=False, exogenous=False)
+        df = _check_dataframe(self, df, check_y=False, exogenous=False)
         freq = df_utils.infer_frequency(df, n_lags=self.max_lags, freq=freq)
-        df = self._handle_missing_data(df, freq=freq, predicting=False)
+        df = _handle_missing_data(self, df, freq=freq, predicting=False)
         folds = df_utils.crossvalidation_split_df(
             df,
             n_lags=self.max_lags,
             n_forecasts=self.n_forecasts,
             k=k,
             fold_pct=fold_pct,
             fold_overlap_pct=fold_overlap_pct,
@@ -1351,17 +1372,17 @@
 
         Returns
         -------
             tuple of k tuples [(folds_val, folds_test), …]
                 elements same as :meth:`crossvalidation_split_df` returns
         """
         df, _, _, _ = df_utils.prep_or_copy_df(df)
-        df = self._check_dataframe(df, check_y=False, exogenous=False)
+        df = _check_dataframe(self, df, check_y=False, exogenous=False)
         freq = df_utils.infer_frequency(df, n_lags=self.max_lags, freq=freq)
-        df = self._handle_missing_data(df, freq=freq, predicting=False)
+        df = _handle_missing_data(self, df, freq=freq, predicting=False)
         folds_val, folds_test = df_utils.double_crossvalidation_split_df(
             df,
             n_lags=self.max_lags,
             n_forecasts=self.n_forecasts,
             k=k,
             valid_pct=valid_pct,
             test_pct=test_pct,
@@ -1386,15 +1407,15 @@
         """
         if self.config_events is None:
             raise Exception(
                 "The events configs should be added to the NeuralProphet object (add_events fn)"
                 "before creating the data with events features"
             )
         df, received_ID_col, received_single_time_series, _ = df_utils.prep_or_copy_df(df)
-        df = self._check_dataframe(df, check_y=True, exogenous=False)
+        df = _check_dataframe(self, df, check_y=True, exogenous=False)
         df_dict_events = df_utils.create_dict_for_events_or_regressors(df, events_df, "events")
         df_created = pd.DataFrame()
         for df_name, df_i in df.groupby("ID"):
             for name in df_dict_events[df_name]["event"].unique():
                 assert name in self.config_events
             df_aux = df_utils.convert_events_to_features(
                 df_i,
@@ -1466,15 +1487,16 @@
         """
         df, received_ID_col, received_single_time_series, _ = df_utils.prep_or_copy_df(df)
         events_dict = df_utils.create_dict_for_events_or_regressors(df, events_df, "events")
         regressors_dict = df_utils.create_dict_for_events_or_regressors(df, regressors_df, "regressors")
 
         df_future_dataframe = pd.DataFrame()
         for df_name, df_i in df.groupby("ID"):
-            df_aux = self._make_future_dataframe(
+            df_aux = _make_future_dataframe(
+                self,
                 df=df_i,
                 events_df=events_dict[df_name],
                 regressors_df=regressors_dict[df_name],
                 periods=periods,
                 n_historic_predictions=n_historic_predictions,
             )
             df_aux["ID"] = df_name
@@ -1540,16 +1562,16 @@
             pd.DataFrame, dict
                 trend on prediction dates.
         """
         if quantile is not None and not (0 < quantile < 1):
             raise ValueError("The quantile specified need to be a float in-between (0,1)")
 
         df, received_ID_col, received_single_time_series, _ = df_utils.prep_or_copy_df(df)
-        df = self._check_dataframe(df, check_y=False, exogenous=False)
-        df = self._normalize(df)
+        df = _check_dataframe(self, df, check_y=False, exogenous=False)
+        df = _normalize(self, df)
         df_trend = pd.DataFrame()
         for df_name, df_i in df.groupby("ID"):
             t = torch.from_numpy(np.expand_dims(df_i["t"].values, 1))  # type: ignore
 
             # Creating and passing meta, in this case the meta['df_name'] is the ID of the dataframe
             # Note: meta is only used on the trend method if trend_global_local is not "global"
             meta = OrderedDict()
@@ -1584,16 +1606,16 @@
             pd.DataFrame, dict
                 seasonal components with columns of name <seasonality component name>
         """
         if quantile is not None and not (0 < quantile < 1):
             raise ValueError("The quantile specified need to be a float in-between (0,1)")
 
         df, received_ID_col, received_single_time_series, _ = df_utils.prep_or_copy_df(df)
-        df = self._check_dataframe(df, check_y=False, exogenous=False)
-        df = self._normalize(df)
+        df = _check_dataframe(self, df, check_y=False, exogenous=False)
+        df = _normalize(self, df)
         df_seasonal = pd.DataFrame()
         for df_name, df_i in df.groupby("ID"):
             dataset = time_dataset.TimeDataset(
                 df_i,
                 name=df_name,
                 config_seasonality=self.config_seasonality,
                 # n_lags=0,
@@ -2320,336 +2342,14 @@
             num_trends_modelled=self.num_trends_modelled,
             num_seasonalities_modelled=self.num_seasonalities_modelled,
             meta_used_in_model=self.meta_used_in_model,
         )
         log.debug(self.model)
         return self.model
 
-    def _create_dataset(self, df, predict_mode, prediction_frequency=None):
-        """Construct dataset from dataframe.
-
-        (Configured Hyperparameters can be overridden by explicitly supplying them.
-        Useful to predict a single model component.)
-
-        Parameters
-        ----------
-            df : pd.DataFrame
-                dataframe containing column ``ds``, ``y``, and optionally``ID`` and
-                normalized columns normalized columns ``ds``, ``y``, ``t``, ``y_scaled``
-            predict_mode : bool
-                specifies predict mode
-
-                Options
-                    * ``False``: includes target values.
-                    * ``True``: does not include targets but includes entire dataset as input
-
-        Returns
-        -------
-            TimeDataset
-        """
-        df, _, _, _ = df_utils.prep_or_copy_df(df)
-        return time_dataset.GlobalTimeDataset(
-            df,
-            predict_mode=predict_mode,
-            n_lags=self.n_lags,
-            n_forecasts=self.n_forecasts,
-            predict_steps=self.predict_steps,
-            config_seasonality=self.config_seasonality,
-            config_events=self.config_events,
-            config_country_holidays=self.config_country_holidays,
-            config_lagged_regressors=self.config_lagged_regressors,
-            config_regressors=self.config_regressors,
-            config_missing=self.config_missing,
-            prediction_frequency=prediction_frequency,
-        )
-
-    def __handle_missing_data(self, df, freq, predicting):
-        """Checks and normalizes new data
-
-        Data is also auto-imputed, unless impute_missing is set to ``False``.
-
-        Parameters
-        ----------
-            df : pd.DataFrame
-                dataframe containing column ``ds``, ``y`` with all data
-            freq : str
-                data step sizes. Frequency of data recording,
-
-                Note
-                ----
-                Any valid frequency for pd.date_range, such as ``5min``, ``D``, ``MS`` or ``auto`` (default) to automatically set frequency.
-            predicting : bool
-                when no lags, allow NA values in ``y`` of forecast series or ``y`` to miss completely
-
-        Returns
-        -------
-            pd.DataFrame
-                preprocessed dataframe
-        """
-        # Receives df with single ID column
-        assert len(df["ID"].unique()) == 1
-        if self.n_lags == 0 and not predicting:
-            # we can drop rows with NA in y
-            sum_na = sum(df["y"].isna())
-            if sum_na > 0:
-                df = df[df["y"].notna()]
-                log.info(f"dropped {sum_na} NAN row in 'y'")
-
-        # add missing dates for autoregression modelling
-        if self.n_lags > 0:
-            df, missing_dates = df_utils.add_missing_dates_nan(df, freq=freq)
-            if missing_dates > 0:
-                if self.config_missing.impute_missing:
-                    log.info(f"{missing_dates} missing dates added.")
-                # FIX Issue#52
-                # Comment error raising to allow missing data for autoregression flow.
-                # else:
-                #     raise ValueError(f"{missing_dates} missing dates found. Please preprocess data manually or set impute_missing to True.")
-                # END FIX
-
-        if self.config_regressors is not None:
-            # if future regressors, check that they are not nan at end, else drop
-            # we ignore missing events, as those will be filled in with zeros.
-            reg_nan_at_end = 0
-            for col, regressor in self.config_regressors.items():
-                # check for completeness of the regressor values
-                col_nan_at_end = 0
-                while len(df) > col_nan_at_end and df[col].isnull().iloc[-(1 + col_nan_at_end)]:
-                    col_nan_at_end += 1
-                reg_nan_at_end = max(reg_nan_at_end, col_nan_at_end)
-            if reg_nan_at_end > 0:
-                # drop rows at end due to missing future regressors
-                df = df[:-reg_nan_at_end]
-                log.info(f"Dropped {reg_nan_at_end} rows at end due to missing future regressor values.")
-
-        df_end_to_append = None
-        nan_at_end = 0
-        while len(df) > nan_at_end and df["y"].isnull().iloc[-(1 + nan_at_end)]:
-            nan_at_end += 1
-        if nan_at_end > 0:
-            if predicting:
-                # allow nans at end - will re-add at end
-                if self.n_forecasts > 1 and self.n_forecasts < nan_at_end:
-                    # check that not more than n_forecasts nans, else drop surplus
-                    df = df[: -(nan_at_end - self.n_forecasts)]
-                    # correct new length:
-                    nan_at_end = self.n_forecasts
-                    log.info(
-                        "Detected y to have more NaN values than n_forecast can predict. "
-                        f"Dropped {nan_at_end - self.n_forecasts} rows at end."
-                    )
-                df_end_to_append = df[-nan_at_end:]
-                df = df[:-nan_at_end]
-            else:
-                # training - drop nans at end
-                df = df[:-nan_at_end]
-                log.info(
-                    f"Dropped {nan_at_end} consecutive nans at end. "
-                    "Training data can only be imputed up to last observation."
-                )
-
-        # impute missing values
-        data_columns = []
-        if self.n_lags > 0:
-            data_columns.append("y")
-        if self.config_lagged_regressors is not None:
-            data_columns.extend(self.config_lagged_regressors.keys())
-        if self.config_regressors is not None:
-            data_columns.extend(self.config_regressors.keys())
-        if self.config_events is not None:
-            data_columns.extend(self.config_events.keys())
-        conditional_cols = []
-        if self.config_seasonality is not None:
-            conditional_cols = list(
-                set(
-                    [
-                        value.condition_name
-                        for key, value in self.config_seasonality.periods.items()
-                        if value.condition_name is not None
-                    ]
-                )
-            )
-            data_columns.extend(conditional_cols)
-        for column in data_columns:
-            sum_na = sum(df[column].isnull())
-            if sum_na > 0:
-                log.warning(f"{sum_na} missing values in column {column} were detected in total. ")
-                if self.config_missing.impute_missing:
-                    # use 0 substitution for holidays and events missing values
-                    if self.config_events is not None and column in self.config_events.keys():
-                        df[column].fillna(0, inplace=True)
-                        remaining_na = 0
-                    else:
-                        df.loc[:, column], remaining_na = df_utils.fill_linear_then_rolling_avg(
-                            df[column],
-                            limit_linear=self.config_missing.impute_linear,
-                            rolling=self.config_missing.impute_rolling,
-                        )
-                    log.info(f"{sum_na - remaining_na} NaN values in column {column} were auto-imputed.")
-                    if remaining_na > 0:
-                        log.warning(
-                            f"More than {2 * self.config_missing.impute_linear + self.config_missing.impute_rolling} consecutive missing values encountered in column {column}. "
-                            f"{remaining_na} NA remain after auto-imputation. "
-                        )
-                # FIX Issue#52
-                # Comment error raising to allow missing data for autoregression flow.
-                # else:  # fail because set to not impute missing
-                #    raise ValueError(
-                #        "Missing values found. " "Please preprocess data manually or set impute_missing to True."
-                #    )
-                # END FIX
-        if df_end_to_append is not None:
-            df = pd.concat([df, df_end_to_append])
-            if self.config_seasonality is not None and len(conditional_cols) > 0:
-                df[conditional_cols] = df[conditional_cols].ffill()  # type: ignore
-        return df
-
-    def _handle_missing_data(self, df, freq, predicting=False):
-        """Checks and normalizes new data
-
-        Data is also auto-imputed, unless impute_missing is set to ``False``.
-
-        Parameters
-        ----------
-            df : pd.DataFrame
-                dataframe containing column ``ds``, ``y``, and optionally``ID`` with all data
-            freq : str
-                data step sizes. Frequency of data recording,
-
-                Note
-                ----
-                Any valid frequency for pd.date_range, such as ``5min``, ``D``, ``MS`` or ``auto`` (default) to automatically set frequency.
-            predicting (bool): when no lags, allow NA values in ``y`` of forecast series or ``y`` to miss completely
-
-        Returns
-        -------
-            pre-processed df
-        """
-        df, _, _, _ = df_utils.prep_or_copy_df(df)
-        df_handled_missing = pd.DataFrame()
-        for df_name, df_i in df.groupby("ID"):
-            df_handled_missing_aux = self.__handle_missing_data(df_i, freq, predicting).copy(deep=True)
-            df_handled_missing_aux["ID"] = df_name
-            df_handled_missing = pd.concat((df_handled_missing, df_handled_missing_aux), ignore_index=True)
-        return df_handled_missing
-
-    def _check_dataframe(self, df: pd.DataFrame, check_y: bool = True, exogenous: bool = True):
-        """Performs basic data sanity checks and ordering
-
-        Prepare dataframe for fitting or predicting.
-
-        Parameters
-        ----------
-            df : pd.DataFrame
-                dataframe containing column ``ds``, ``y``, and optionally``ID`` with all data
-            check_y : bool
-                if df must have series values
-
-                Note
-                ----
-                set to True if training or predicting with autoregression
-            exogenous : bool
-                whether to check covariates, regressors and events column names
-
-        Returns
-        -------
-            pd.DataFrame
-                checked dataframe
-        """
-        df, _, _, _ = df_utils.prep_or_copy_df(df)
-        df, regressors_to_remove = df_utils.check_dataframe(
-            df=df,
-            check_y=check_y,
-            covariates=self.config_lagged_regressors if exogenous else None,
-            regressors=self.config_regressors if exogenous else None,
-            events=self.config_events if exogenous else None,
-            seasonalities=self.config_seasonality if exogenous else None,
-        )
-        if self.config_regressors is not None:
-            for reg in regressors_to_remove:
-                log.warning(f"Removing regressor {reg} because it is not present in the data.")
-                self.config_regressors.pop(reg)
-        return df
-
-    def _validate_column_name(self, name, events=True, seasons=True, regressors=True, covariates=True):
-        """Validates the name of a seasonality, event, or regressor.
-
-        Parameters
-        ----------
-            name : str
-                name of seasonality, event or regressor
-            events : bool
-                check if name already used for event
-            seasons : bool
-                check if name already used for seasonality
-            regressors : bool
-                check if name already used for regressor
-        """
-        reserved_names = [
-            "trend",
-            "additive_terms",
-            "daily",
-            "weekly",
-            "yearly",
-            "events",
-            "holidays",
-            "zeros",
-            "extra_regressors_additive",
-            "yhat",
-            "extra_regressors_multiplicative",
-            "multiplicative_terms",
-            "ID",
-        ]
-        rn_l = [n + "_lower" for n in reserved_names]
-        rn_u = [n + "_upper" for n in reserved_names]
-        reserved_names.extend(rn_l)
-        reserved_names.extend(rn_u)
-        reserved_names.extend(["ds", "y", "cap", "floor", "y_scaled", "cap_scaled"])
-        if name in reserved_names:
-            raise ValueError(f"Name {name!r} is reserved.")
-        if events and self.config_events is not None:
-            if name in self.config_events.keys():
-                raise ValueError(f"Name {name!r} already used for an event.")
-        if events and self.config_country_holidays is not None:
-            if name in self.config_country_holidays.holiday_names:
-                raise ValueError(f"Name {name!r} is a holiday name in {self.config_country_holidays.country}.")
-        if seasons and self.config_seasonality is not None:
-            if name in self.config_seasonality.periods:
-                raise ValueError(f"Name {name!r} already used for a seasonality.")
-        if covariates and self.config_lagged_regressors is not None:
-            if name in self.config_lagged_regressors:
-                raise ValueError(f"Name {name!r} already used for an added covariate.")
-        if regressors and self.config_regressors is not None:
-            if name in self.config_regressors.keys():
-                raise ValueError(f"Name {name!r} already used for an added regressor.")
-
-    def _normalize(self, df):
-        """Apply data scales.
-
-        Applies data scaling factors to df using data_params.
-
-        Parameters
-        ----------
-            df : pd.DataFrame
-                dataframe containing column ``ds``, ``y``, and optionally``ID`` with all data
-
-        Returns
-        -------
-            df: pd.DataFrame, normalized
-        """
-        df, _, _, _ = df_utils.prep_or_copy_df(df)
-        df_norm = pd.DataFrame()
-        for df_name, df_i in df.groupby("ID"):
-            data_params = self.config_normalization.get_data_params(df_name)
-            df_i.drop("ID", axis=1, inplace=True)
-            df_aux = df_utils.normalize(df_i, data_params).copy(deep=True)
-            df_aux["ID"] = df_name
-            df_norm = pd.concat((df_norm, df_aux), ignore_index=True)
-        return df_norm
-
     def _init_train_loader(self, df, num_workers=0):
         """Executes data preparation steps and initiates training procedure.
 
         Parameters
         ----------
             df : pd.DataFrame
                 dataframe containing column ``ds``, ``y``, and optionally``ID`` with all data
@@ -2666,31 +2366,31 @@
             df=df,
             config_lagged_regressors=self.config_lagged_regressors,
             config_regressors=self.config_regressors,
             config_events=self.config_events,
             config_seasonality=self.config_seasonality,
         )
 
-        df = self._normalize(df)
+        df = _normalize(self, df)
         # if not self.fitted:
         if self.config_trend.changepoints is not None:
             # scale user-specified changepoint times
             df_aux = pd.DataFrame({"ds": pd.Series(self.config_trend.changepoints)})
-            self.config_trend.changepoints = self._normalize(df_aux)["t"].values  # type: ignore # types are numpy.ArrayLike and list
+            self.config_trend.changepoints = _normalize(self, df_aux)["t"].values  # type: ignore # types are numpy.ArrayLike and list
 
         # df_merged, _ = df_utils.join_dataframes(df)
         # df_merged = df_merged.sort_values("ds")
         # df_merged.drop_duplicates(inplace=True, keep="first", subset=["ds"])
         df_merged = df_utils.merge_dataframes(df)
         self.config_seasonality = utils.set_auto_seasonalities(df_merged, config_seasonality=self.config_seasonality)
         if self.config_country_holidays is not None:
             self.config_country_holidays.init_holidays(df_merged)
 
-        dataset = self._create_dataset(
-            df, predict_mode=False, prediction_frequency=self.prediction_frequency
+        dataset = _create_dataset(
+            self, df, predict_mode=False, prediction_frequency=self.prediction_frequency
         )  # needs to be called after set_auto_seasonalities
 
         # Determine the max_number of epochs
         self.config_train.set_auto_batch_epoch(n_data=len(dataset))
 
         loader = DataLoader(dataset, batch_size=self.config_train.batch_size, shuffle=True, num_workers=num_workers)
 
@@ -2705,16 +2405,16 @@
                 dataframe containing column ``ds``, ``y``, and optionally``ID`` with all data
 
         Returns
         -------
             torch DataLoader
         """
         df, _, _, _ = df_utils.prep_or_copy_df(df)
-        df = self._normalize(df)
-        dataset = self._create_dataset(df, predict_mode=False)
+        df = _normalize(self, df)
+        dataset = _create_dataset(self, df, predict_mode=False)
         loader = DataLoader(dataset, batch_size=min(1024, len(dataset)), shuffle=False, drop_last=False)
         return loader
 
     def _train(
         self,
         df: pd.DataFrame,
         df_val: Optional[pd.DataFrame] = None,
@@ -2867,226 +2567,57 @@
             forecast_pos = self.highlight_forecast_step_n
         weights = self.model.ar_weights.detach().numpy()  # type: ignore
         weights = weights[forecast_pos - 1, :][::-1]
         sTPE = utils.symmetric_total_percentage_error(self.true_ar_weights, weights)
         log.info("AR parameters: ", self.true_ar_weights, "\n", "Model weights: ", weights)
         return sTPE
 
-    def _make_future_dataframe(self, df, events_df, regressors_df, periods, n_historic_predictions):
-        # Receives df with single ID column
-        assert len(df["ID"].unique()) == 1
-        if periods == 0 and n_historic_predictions is True:
-            log.warning(
-                "Not extending df into future as no periods specified." "You can call predict directly instead."
-            )
-        df = df.copy(deep=True)
-        _ = df_utils.infer_frequency(df, n_lags=self.max_lags, freq=self.data_freq)
-        last_date = pd.to_datetime(df["ds"].copy(deep=True).dropna()).sort_values().max()
-        if events_df is not None:
-            events_df = events_df.copy(deep=True).reset_index(drop=True)
-        if regressors_df is not None:
-            regressors_df = regressors_df.copy(deep=True).reset_index(drop=True)
-        if periods is None:
-            periods = 1 if self.max_lags == 0 else self.n_forecasts
-        else:
-            assert periods >= 0
-
-        if isinstance(n_historic_predictions, bool):
-            if n_historic_predictions:
-                n_historic_predictions = len(df) - self.max_lags
-            else:
-                n_historic_predictions = 0
-        elif not isinstance(n_historic_predictions, int):
-            log.error("non-integer value for n_historic_predictions set to zero.")
-            n_historic_predictions = 0
-
-        if periods == 0 and n_historic_predictions == 0:
-            raise ValueError("Set either history or future to contain more than zero values.")
-
-        # check for external regressors known in future
-        if self.config_regressors is not None and periods > 0:
-            if regressors_df is None:
-                raise ValueError("Future values of all user specified regressors not provided")
-            else:
-                for regressor in self.config_regressors.keys():
-                    if regressor not in regressors_df.columns:
-                        raise ValueError(f"Future values of user specified regressor {regressor} not provided")
-
-        if len(df) < self.max_lags:
-            raise ValueError(
-                "Insufficient input data for a prediction."
-                "Please supply historic observations (number of rows) of at least max_lags (max of number of n_lags)."
-            )
-        elif len(df) < self.max_lags + n_historic_predictions:
-            log.warning(
-                f"Insufficient data for {n_historic_predictions} historic forecasts, reduced to {len(df) - self.max_lags}."
-            )
-            n_historic_predictions = len(df) - self.max_lags
-        if (n_historic_predictions + self.max_lags) == 0:
-            df = pd.DataFrame(columns=df.columns)
-        else:
-            df = df[-(self.max_lags + n_historic_predictions) :]
-            nan_at_end = 0
-            while len(df) > nan_at_end and df["y"].isnull().iloc[-(1 + nan_at_end)]:
-                nan_at_end += 1
-            if nan_at_end > 0:
-                if self.max_lags > 0 and (nan_at_end + 1) >= self.max_lags:
-                    raise ValueError(
-                        f"{nan_at_end + 1} missing values were detected at the end of df before df was extended into the future. "
-                        "Please make sure there are no NaN values at the end of df."
-                    )
-                df["y"].iloc[-(nan_at_end + 1) :].ffill(inplace=True)
-                log.warning(
-                    f"{nan_at_end + 1} missing values were forward-filled at the end of df before df was extended into the future. "
-                    "Please make sure there are no NaN values at the end of df."
-                )
-
-        if len(df) > 0:
-            if len(df.columns) == 1 and "ds" in df:
-                assert self.max_lags == 0
-                df = self._check_dataframe(df, check_y=False, exogenous=False)
-            else:
-                df = self._check_dataframe(df, check_y=self.max_lags > 0, exogenous=True)
-        # future data
-        # check for external events known in future
-        if self.config_events is not None and periods > 0 and events_df is None:
-            log.warning(
-                "Future values not supplied for user specified events. "
-                "All events being treated as not occurring in future"
-            )
-
-        if self.max_lags > 0:
-            if periods > 0 and periods != self.n_forecasts:
-                periods = self.n_forecasts
-                log.warning(f"Number of forecast steps is defined by n_forecasts. Adjusted to {self.n_forecasts}.")
-
-        if periods > 0:
-            future_df = df_utils.make_future_df(
-                df_columns=df.columns,
-                last_date=last_date,
-                periods=periods,
-                freq=self.data_freq,
-                config_events=self.config_events,
-                events_df=events_df,
-                config_regressors=self.config_regressors,
-                regressors_df=regressors_df,
-            )
-            if len(df) > 0:
-                df = pd.concat([df, future_df])
-            else:
-                df = future_df
-        df = df.reset_index(drop=True)
-        self.predict_steps = periods
-        return df
-
-    def _get_maybe_extend_periods(self, df):
-        # Receives df with single ID column
-        assert len(df["ID"].unique()) == 1
-        periods_add = 0
-        nan_at_end = 0
-        while len(df) > nan_at_end and df["y"].isnull().iloc[-(1 + nan_at_end)]:
-            nan_at_end += 1
-        if self.max_lags > 0:
-            if self.config_regressors is None:
-                # if dataframe has already been extended into future,
-                # don't extend beyond n_forecasts.
-                periods_add = max(0, self.n_forecasts - nan_at_end)
-            else:
-                # can not extend as we lack future regressor values.
-                periods_add = 0
-        return periods_add
-
-    def _maybe_extend_df(self, df):
-        # Receives df with ID column
-        periods_add = {}
-        extended_df = pd.DataFrame()
-        for df_name, df_i in df.groupby("ID"):
-            _ = df_utils.infer_frequency(df_i, n_lags=self.max_lags, freq=self.data_freq)
-            # to get all forecasteable values with df given, maybe extend into future:
-            periods_add[df_name] = self._get_maybe_extend_periods(df_i)
-            if periods_add[df_name] > 0:
-                # This does not include future regressors or events.
-                # periods should be 0 if those are configured.
-                last_date = pd.to_datetime(df_i["ds"].copy(deep=True)).sort_values().max()
-                future_df = df_utils.make_future_df(
-                    df_columns=df_i.columns,
-                    last_date=last_date,
-                    periods=periods_add[df_name],
-                    freq=self.data_freq,
-                    config_events=self.config_events,
-                )
-                future_df["ID"] = df_name
-                df_i = pd.concat([df_i, future_df])
-                df_i.reset_index(drop=True, inplace=True)
-            extended_df = pd.concat((extended_df, df_i.copy(deep=True)), ignore_index=True)
-        return extended_df, periods_add
-
-    def _prepare_dataframe_to_predict(self, df):
-        # Receives df with ID column
-        df_prepared = pd.DataFrame()
-        for df_name, df_i in df.groupby("ID"):
-            df_i = df_i.copy(deep=True)
-            _ = df_utils.infer_frequency(df_i, n_lags=self.max_lags, freq=self.data_freq)
-            # check if received pre-processed df
-            if "y_scaled" in df_i.columns or "t" in df_i.columns:
-                raise ValueError(
-                    "DataFrame has already been normalized. " "Please provide raw dataframe or future dataframe."
-                )
-            # Checks
-            if len(df_i) == 0 or len(df_i) < self.max_lags:
-                raise ValueError(
-                    "Insufficient input data for a prediction."
-                    "Please supply historic observations (number of rows) of at least max_lags (max of number of n_lags)."
-                )
-            if len(df_i.columns) == 1 and "ds" in df_i:
-                if self.max_lags != 0:
-                    raise ValueError("only datestamps provided but y values needed for auto-regression.")
-                df_i = self._check_dataframe(df_i, check_y=False, exogenous=False)
-            else:
-                df_i = self._check_dataframe(df_i, check_y=self.max_lags > 0, exogenous=False)
-                # fill in missing nans except for nans at end
-                df_i = self._handle_missing_data(df_i, freq=self.data_freq, predicting=True)
-            df_prepared = pd.concat((df_prepared, df_i.copy(deep=True).reset_index(drop=True)), ignore_index=True)
-        return df_prepared
-
     def _predict_raw(self, df, df_name, include_components=False, prediction_frequency=None):
         """Runs the model to make predictions.
 
         Predictions are returned in raw vector format without decomposition.
         Predictions are given on a forecast origin basis, not on a target basis.
 
         Parameters
         ----------
             df : pd.DataFrame
                 dataframe containing column ``ds``, ``y``, and optionally``ID`` with all data
             df_name : str
                 name of the data params from which the current dataframe refers to (only in case of local_normalization)
             include_components : bool
                 whether to return individual components of forecast
-            prediction_frequency : int
-                periodic interval in which forecasts should be made.
+        prediction_frequency: dict
+            periodic interval in which forecasts should be made.
+            Key: str
+                periodicity of the predictions to be made, e.g. 'daily-hour'.
 
-                Note
-                ----
-                E.g. if prediction_frequency=7, forecasts are only made on every 7th step (once in a week in case of daily resolution).
+            Options
+                * ``'hourly-minute'``: forecast once per hour at a specified minute
+                * ``'daily-hour'``: forecast once per day at a specified hour
+                * ``'weekly-day'``: forecast once per week at a specified day
+                * ``'monthly-day'``: forecast once per month at a specified day
+                * ``'yearly-month'``: forecast once per year at a specified month
+
+            value: int
+                forecast origin of the predictions to be made, e.g. 7 for 7am in case of 'daily-hour'.
 
         Returns
         -------
             pd.Series
                 timestamps referring to the start of the predictions.
             np.array
                 array containing the forecasts
             dict[np.array]
                 Dictionary of components containing an array of each components contribution to the forecast
         """
         # Receives df with single ID column
         assert len(df["ID"].unique()) == 1
         if "y_scaled" not in df.columns or "t" not in df.columns:
             raise ValueError("Received unprepared dataframe to predict. " "Please call predict_dataframe_to_predict.")
-        dataset = self._create_dataset(df, predict_mode=True, prediction_frequency=prediction_frequency)
+        dataset = _create_dataset(self, df, predict_mode=True, prediction_frequency=prediction_frequency)
         loader = DataLoader(dataset, batch_size=min(1024, len(df)), shuffle=False, drop_last=False)
         if self.n_forecasts > 1:
             dates = df["ds"].iloc[self.max_lags : -self.n_forecasts + 1]
         else:
             dates = df["ds"].iloc[self.max_lags :]
 
         # Pass the include_components flag to the model
@@ -3150,179 +2681,34 @@
                     components[name] = value * trend * scale_y  # type: ignore # output absolute value of respective additive component
 
         else:
             components = None
 
         return dates, predicted, components
 
-    def _convert_raw_predictions_to_raw_df(self, dates, predicted, components=None):
-        """Turns forecast-origin-wise predictions into forecast-target-wise predictions.
-
-        Parameters
-        ----------
-            dates : pd.Series
-                timestamps referring to the start of the predictions.
-            predicted : np.array
-                Array containing the forecasts
-            components : dict[np.array]
-                Dictionary of components containing an array of each components' contribution to the forecast
-
-        Returns
-        -------
-            pd. DataFrame
-                columns ``ds``, ``y``, and [``step<i>``]
-
-                Note
-                ----
-                where step<i> refers to the i-step-ahead prediction *made at* this row's datetime.
-                e.g. the first forecast step0 is the prediction for this timestamp,
-                the step1 is for the timestamp after, ...
-                ... step3 is the prediction for 3 steps into the future,
-                predicted using information up to (excluding) this datetime.
-        """
-        all_data = predicted
-        df_raw = pd.DataFrame()
-        df_raw.insert(0, "ds", dates.values)
-        df_raw.insert(1, "ID", "__df__")  # type: ignore
-        for forecast_lag in range(self.n_forecasts):
-            for quantile_idx in range(len(self.config_train.quantiles)):
-                # 0 is the median quantile index
-                if quantile_idx == 0:
-                    step_name = f"step{forecast_lag}"
-                else:
-                    step_name = f"step{forecast_lag} {self.config_train.quantiles[quantile_idx] * 100}%"
-                data = all_data[:, forecast_lag, quantile_idx]
-                ser = pd.Series(data=data, name=step_name)
-                df_raw = df_raw.merge(ser, left_index=True, right_index=True)
-            if components is not None:
-                for comp_name, comp_data in components.items():
-                    comp_name_ = f"{comp_name}{forecast_lag}"
-                    data = comp_data[:, forecast_lag, 0]  # for components the quantiles are ignored for now
-                    ser = pd.Series(data=data, name=comp_name_)
-                    df_raw = df_raw.merge(ser, left_index=True, right_index=True)
-        return df_raw
-
-    def _reshape_raw_predictions_to_forecst_df(self, df, predicted, components, prediction_frequency):
-        """Turns forecast-origin-wise predictions into forecast-target-wise predictions.
-
-        Parameters
-        ----------
-            df : pd.DataFrame
-                input dataframe
-            predicted : np.array
-                Array containing the forecasts
-            components : dict[np.array]
-                Dictionary of components containing an array of each components' contribution to the forecast
-
-        Returns
-        -------
-            pd.DataFrame
-                columns ``ds``, ``y``, ``trend`` and [``yhat<i>``]
-
-                Note
-                ----
-                where yhat<i> refers to the i-step-ahead prediction for this row's datetime.
-                e.g. yhat3 is the prediction for this datetime, predicted 3 steps ago, "3 steps old".
-        """
-        # Receives df with single ID column
-        assert len(df["ID"].unique()) == 1
-        cols = ["ds", "y", "ID"]  # cols to keep from df
-        df_forecast = pd.concat((df[cols],), axis=1)
-        # create a line for each forecast_lag
-        # 'yhat<i>' is the forecast for 'y' at 'ds' from i steps ago.
-        for j in range(len(self.config_train.quantiles)):
-            for forecast_lag in range(1, self.n_forecasts + 1):
-                forecast = predicted[:, forecast_lag - 1, j]
-                pad_before = self.max_lags + forecast_lag - 1
-                pad_after = self.n_forecasts - forecast_lag
-                yhat = np.concatenate(([np.NaN] * pad_before, forecast, [np.NaN] * pad_after))
-                if prediction_frequency is not None:
-                    yhat = np.full(pad_before, np.NaN)
-                    for el in forecast:
-                        yhat = np.concatenate((yhat, [el], [np.NaN] * (prediction_frequency - 1)))
-                    if len(yhat) < len(df_forecast):
-                        yhat = np.concatenate((yhat, [np.NaN] * (len(df_forecast) - len(yhat))))
-                    else:
-                        yhat = yhat[: len(df_forecast)]
-                # 0 is the median quantile index
-                if j == 0:
-                    name = f"yhat{forecast_lag}"
-                else:
-                    name = f"yhat{forecast_lag} {round(self.config_train.quantiles[j] * 100, 1)}%"
-                df_forecast[name] = yhat
-
-        if components is None:
-            return df_forecast
-
-        # else add components
-        lagged_components = [
-            "ar",
-        ]
-        if self.config_lagged_regressors is not None:
-            for name in self.config_lagged_regressors.keys():
-                lagged_components.append(f"lagged_regressor_{name}")
-        for comp in lagged_components:
-            if comp in components:
-                for j in range(len(self.config_train.quantiles)):
-                    for forecast_lag in range(1, self.n_forecasts + 1):
-                        forecast = components[comp][:, forecast_lag - 1, j]  # 0 is the median quantile
-                        pad_before = self.max_lags + forecast_lag - 1
-                        pad_after = self.n_forecasts - forecast_lag
-                        yhat = np.concatenate(([np.NaN] * pad_before, forecast, [np.NaN] * pad_after))
-                        if prediction_frequency is not None:
-                            yhat = np.full(pad_before, np.NaN)
-                            for el in forecast:
-                                yhat = np.concatenate((yhat, [el], [np.NaN] * (prediction_frequency - 1)))
-                            if len(yhat) < len(df_forecast):
-                                yhat = np.concatenate((yhat, [np.NaN] * (len(df_forecast) - len(yhat))))
-                            else:
-                                yhat = yhat[: len(df_forecast)]
-                        if j == 0:  # temporary condition to add only the median component
-                            name = f"{comp}{forecast_lag}"
-                            df_forecast[name] = yhat
-
-        # only for non-lagged components
-        for comp in components:
-            if comp not in lagged_components:
-                for j in range(len(self.config_train.quantiles)):
-                    forecast_0 = components[comp][0, :, j]
-                    forecast_rest = components[comp][1:, self.n_forecasts - 1, j]
-                    yhat = np.concatenate(([np.NaN] * self.max_lags, forecast_0, forecast_rest))
-                    if prediction_frequency is not None:
-                        forecast_rest = components[comp][1:, :, j]
-                        yhat = np.concatenate(([np.NaN] * self.max_lags, forecast_0, forecast_rest.flatten()))
-                        if len(yhat) < len(df_forecast):
-                            yhat = np.concatenate((yhat, [np.NaN] * (len(df_forecast) - len(yhat))))
-                        else:
-                            yhat = yhat[: len(df_forecast)]
-                    if j == 0:  # temporary condition to add only the median component
-                        # add yhat into dataframe, using df_forecast indexing
-                        yhat_df = pd.Series(yhat, name=comp).set_axis(df_forecast.index)
-                        df_forecast = pd.concat([df_forecast, yhat_df], axis=1, ignore_index=False)
-        return df_forecast
-
     def conformal_predict(
         self,
         df: pd.DataFrame,
         calibration_df: pd.DataFrame,
-        alpha: float,
+        alpha: Union[float, Tuple[float, float]],
         method: str = "naive",
         plotting_backend: Optional[str] = None,
         **kwargs,
     ) -> pd.DataFrame:
         """Apply a given conformal prediction technique to get the uncertainty prediction intervals (or q-hats). Then predict.
 
         Parameters
         ----------
             df : pd.DataFrame
                 test dataframe containing column ``ds``, ``y``, and optionally ``ID`` with data
             calibration_df : pd.DataFrame
                 holdout calibration dataframe for split conformal prediction
-            alpha : float
-                user-specified significance level of the prediction interval
+            alpha : float or tuple
+                user-specified significance level of the prediction interval, float if coverage error spread arbitrarily over
+                left and right tails, tuple of two floats for different coverage error over left and right tails respectively
             method : str
                 name of conformal prediction technique used
 
                 Options
                     * (default) ``naive``: Naive or Absolute Residual
                     * ``cqr``: Conformalized Quantile Regression
             plotting_backend : str
```

### Comparing `neuralprophet-0.5.4/neuralprophet/hdays_utils.py` & `neuralprophet-0.6.0rc1/neuralprophet/hdays_utils.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.5.4/neuralprophet/logger.py` & `neuralprophet-0.6.0rc1/neuralprophet/logger.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.5.4/neuralprophet/np_types.py` & `neuralprophet-0.6.0rc1/neuralprophet/np_types.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.5.4/neuralprophet/plot_forecast_matplotlib.py` & `neuralprophet-0.6.0rc1/neuralprophet/plot_forecast_matplotlib.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,18 +23,18 @@
     ax=None,
     xlabel="ds",
     ylabel="y",
     highlight_forecast=None,
     line_per_origin=False,
     figsize=(10, 6),
 ):
-    """Plot the NeuralProphet forecast
+    """Plot the NeuralProphet forecast.
 
     Parameters
-    ---------
+    ----------
         fcst : pd.DataFrame
             Output of m.predict
         quantiles: list
             Quantiles for which the forecasts are to be plotted
         ax : matplotlib axes
             Axes to plot on
         xlabel : str
@@ -49,34 +49,34 @@
             Width, height in inches.
 
     Returns
     -------
         matplotlib.pyplot.figure
             Figure showing the NeuralProphet forecast
 
-            Examples
-            --------
-            Base usage
-
-            >>> from neuralprophet import NeuralProphet
-            >>> m = NeuralProphet()
-            >>> metrics = m.fit(df, freq="D")
-            >>> future = m.make_future_dataframe(df=df, periods=365)
-            >>> forecast = m.predict(df=future)
-            >>> fig_forecast = m.plot(forecast)
-
-            Additional plot specifications
-
-            >>> fig_forecast = m.plot(forecast,
-            >>>                       xlabel="ds",
-            >>>                       ylabel="y",
-            >>>                       highlight_forecast=None,
-            >>>                       line_per_origin=False,
-            >>>                       figsize=(10, 6)
-            >>>                       )
+    Examples
+    --------
+        Base usage
+
+        >>> from neuralprophet import NeuralProphet
+        >>> m = NeuralProphet()
+        >>> metrics = m.fit(df, freq="D")
+        >>> future = m.make_future_dataframe(df=df, periods=365)
+        >>> forecast = m.predict(df=future)
+        >>> fig_forecast = m.plot(forecast)
+
+        Additional plot specifications
+
+        >>> m.plot(forecast,
+        >>>    xlabel="ds",
+        >>>    ylabel="y",
+        >>>    highlight_forecast=None,
+        >>>    line_per_origin=False,
+        >>>    figsize=(10, 6)
+        >>>    )
 
     """
     fcst = fcst.fillna(value=np.nan)
     if ax is None:
         fig = plt.figure(facecolor="w", figsize=figsize)
         ax = fig.add_subplot(111)
     else:
@@ -138,15 +138,18 @@
                         alpha=0.2,
                     )
 
     # Plot any conformal prediction intervals
     if any("+ qhat" in col for col in yhat_col_names) and any("- qhat" in col for col in yhat_col_names):
         quantile_hi = str(max(quantiles) * 100)
         quantile_lo = str(min(quantiles) * 100)
-        if f"yhat1 {quantile_hi}% + qhat1" in fcst.columns and f"yhat1 {quantile_hi}% - qhat1" in fcst.columns:
+        if f"yhat1 {quantile_hi}% + qhat_hi1" in fcst.columns and f"yhat1 {quantile_lo}% - qhat_lo1" in fcst.columns:
+            ax.plot(ds, fcst[f"yhat1 {quantile_hi}% + qhat_hi1"], c="r", label=f"yhat1 {quantile_hi}% + qhat_hi1")
+            ax.plot(ds, fcst[f"yhat1 {quantile_lo}% - qhat_lo1"], c="r", label=f"yhat1 {quantile_lo}% - qhat_lo1")
+        elif f"yhat1 {quantile_hi}% + qhat1" in fcst.columns and f"yhat1 {quantile_hi}% - qhat1" in fcst.columns:
             ax.plot(ds, fcst[f"yhat1 {quantile_hi}% + qhat1"], c="r", label=f"yhat1 {quantile_hi}% + qhat1")
             ax.plot(ds, fcst[f"yhat1 {quantile_lo}% - qhat1"], c="r", label=f"yhat1 {quantile_lo}% - qhat1")
         else:
             ax.plot(ds, fcst["yhat1 + qhat1"], c="r", label="yhat1 + qhat1")
             ax.plot(ds, fcst["yhat1 - qhat1"], c="r", label="yhat1 - qhat1")
 
     ax.plot(ds, fcst["y"], "k.", label="actual y")
@@ -161,15 +164,15 @@
     ax.set_ylabel(ylabel)
     handles, labels = ax.axes.get_legend_handles_labels()
     if len(labels) > 10:
         ax.legend(handles[:10] + [handles[-1]], labels[:10] + [labels[-1]])
         log.warning("Legend is available only for the ten first handles")
     else:
         ax.legend(handles, labels)
-    fig.tight_layout()
+    fig = fig.tight_layout()
     return fig
 
 
 def plot_components(
     m,
     fcst,
     plot_configuration,
@@ -250,15 +253,15 @@
                     plot_custom_season(m=m, ax=ax, quantile=quantile, comp_name=comp_name, df_name=df_name)
             else:
                 comp_name = f"season_{comp['comp_name']}"
                 plot_forecast_component(fcst=fcst, ax=ax, comp_name=comp_name, plot_name=comp["plot_name"])
         elif "auto-regression" in name or "lagged regressor" in name:
             plot_multiforecast_component(fcst=fcst, ax=ax, **comp)
 
-    fig.tight_layout()
+    fig = fig.tight_layout()
     # Reset multiplicative axes labels after tight_layout adjustment
     for ax in multiplicative_axes:
         ax = set_y_as_percent(ax)
     return fig
 
 
 def plot_forecast_component(
@@ -443,64 +446,102 @@
 
 
 def plot_nonconformity_scores(scores, alpha, q, method):
     """Plot the nonconformity scores as well as the one-sided interval width (q).
 
     Parameters
     ----------
-        scores : list
+        scores : dict
             nonconformity scores
-        alpha : float
-            user-specified significance level of the prediction interval
-        q : float
+        alpha : float or tuple
+                user-specified significance level of the prediction interval, float if coverage error spread arbitrarily over
+                left and right tails, tuple of two floats for different coverage error over left and right tails respectively
+        q : float or list
             prediction interval width (or q)
         method : str
             name of conformal prediction technique used
 
             Options
                 * (default) ``naive``: Naive or Absolute Residual
                 * ``cqr``: Conformalized Quantile Regression
 
     Returns
     -------
         matplotlib.pyplot.figure
             Figure showing the nonconformity score with horizontal line for q-value based on the significance level or alpha
     """
-    confidence_levels = np.arange(len(scores)) / len(scores)
-    fig, ax = plt.subplots()
-    ax.plot(confidence_levels, scores, label="score")
-    ax.axvline(x=1 - alpha, color="g", linestyle="-", label=f"(1-alpha) = {1-alpha}", linewidth=1)
-    ax.axhline(y=q, color="r", linestyle="-", label=f"q1 = {round(q, 2)}", linewidth=1)
+    if not isinstance(q, list):
+        q_sym = q
+        scores = scores["noncon_scores"]
+        confidence_levels = np.arange(len(scores)) / len(scores)
+        fig, ax = plt.subplots()
+        ax.plot(confidence_levels, scores, label="score")
+        ax.axvline(x=1 - alpha, color="g", linestyle="-", label=f"(1-alpha) = {1 - alpha}", linewidth=1)
+        ax.axhline(y=q, color="r", linestyle="-", label=f"q1 = {round(q_sym, 2)}", linewidth=1)
+    else:
+        q_lo, q_hi = q
+        scores_lo = scores["noncon_scores_lo"]
+        scores_hi = scores["noncon_scores_hi"]
+        alpha_lo, alpha_hi = alpha
+        confidence_levels = np.arange(len(scores_lo)) / len(scores_lo)
+        fig, ax = plt.subplots()
+        ax.plot(confidence_levels, scores_lo, label="lower score")
+        ax.plot(confidence_levels, scores_hi, label="upper score")
+        ax.axvline(
+            x=1 - alpha_lo,
+            color="darkgreen",
+            linestyle="-",
+            label=f"(1-alpha_lo) = {round(1.0-alpha_lo, 10)}",
+            linewidth=1,
+        )
+        ax.axvline(
+            x=1 - alpha_hi,
+            color="lightgreen",
+            linestyle="-",
+            label=f"(1-alpha_hi) = {round(1.0-alpha_hi, 10)}",
+            linewidth=1,
+        )
+        ax.axhline(y=q_lo, color="darkred", linestyle="-", label=f"q1 = {round(q_lo, 2)}", linewidth=1)
+        ax.axhline(y=q_hi, color="red", linestyle="-", label=f"q2 = {round(q_hi, 2)}", linewidth=1)
     ax.set_title(f"{method} One-Sided Interval Width with q")
     ax.set_xlabel("Confidence Level")
     ax.set_ylabel("One-Sided Interval Width")
     ax.legend()
     return fig
 
 
 def plot_interval_width_per_timestep(q_hats, method):
     """Plot the nonconformity scores as well as the one-sided interval width (q).
 
     Parameters
     ----------
-        q_hats : list
-            prediction interval widths (or q) for each timestep
+        q_hats : dataframe
+            prediction interval widths (or q) for each timestep, contains column ``q_hat_sym`` for symmetric q or
+            ``q_hat_lo`` and ``q_hat_hi`` for asymmetric q
         method : str
             name of conformal prediction technique used
 
             Options
                 * (default) ``naive``: Naive or Absolute Residual
                 * ``cqr``: Conformalized Quantile Regression
 
     Returns
     -------
         matplotlib.pyplot.figure
             Figure showing the q-values for each timestep
     """
     fig, ax = plt.subplots()
-    ax.plot(range(1, len(q_hats) + 1), q_hats)
+    # check if q_hats contains q_hat_sym
+    if "q_hat_sym" in q_hats.columns:
+        q_hats_sym = q_hats["q_hat_sym"]
+        ax.plot(range(1, len(q_hats_sym) + 1), q_hats_sym)
+    else:
+        q_hats_lo = q_hats["q_hat_lo"]
+        q_hats_hi = q_hats["q_hat_hi"]
+        ax.plot(range(1, len(q_hats_lo) + 1), q_hats_lo, label="lower q")
+        ax.plot(range(1, len(q_hats_hi) + 1), q_hats_hi, label="upper q")
     ax.set_title(f"{method} One-Sided Interval Width with q per Timestep")
     ax.set_xlabel("Timestep Number")
     ax.set_ylabel("One-Sided Interval Width")
     # ax.set_xlim(left=1)
     ax.set_ylim(bottom=0)
     return fig
```

### Comparing `neuralprophet-0.5.4/neuralprophet/plot_forecast_plotly.py` & `neuralprophet-0.6.0rc1/neuralprophet/plot_forecast_plotly.py`

 * *Files 8% similar despite different names*

```diff
@@ -708,20 +708,21 @@
 
 
 def plot_nonconformity_scores(scores, alpha, q, method, resampler_active=False):
     """Plot the NeuralProphet forecast components.
 
     Parameters
     ----------
-        scores : list
+        scores : dict
             nonconformity scores
         alpha : float
             user-specified significance level of the prediction interval
-        q : float
-            prediction interval width (or q)
+        q : float or list
+            prediction interval width (or q) for symmetric prediction interval or
+            for upper and lower prediction interval, respectively
         method : str
             name of conformal prediction technique used
 
             Options
                 * (default) ``naive``: Naive or Absolute Residual
                 * ``cqr``: Conformalized Quantile Regression
         resampler_active : bool
@@ -732,43 +733,100 @@
         plotly.graph_objects.Figure
             Figure showing the nonconformity score with horizontal line for q-value based on the significance level or alpha
     """
     if resampler_active:
         register_plotly_resampler(mode="auto")
     else:
         unregister_plotly_resampler()
-    confidence_levels = np.arange(len(scores)) / len(scores)
-    fig = px.line(
-        pd.DataFrame({"Confidence Level": confidence_levels, "One-Sided Interval Width": scores}),
-        x="Confidence Level",
-        y="One-Sided Interval Width",
-        title=f"{method} One-Sided Interval Width with q",
-        width=600,
-        height=400,
-    )
-    fig.add_vline(
-        x=1 - alpha,
-        annotation_text=f"(1-alpha) = {1-alpha}",
-        annotation_position="top left",
-        line_width=1,
-        line_color="green",
-    )
-    fig.add_hline(
-        y=q, annotation_text=f"q1 = {round(q, 2)}", annotation_position="top left", line_width=1, line_color="red"
-    )
-    fig.update_layout(margin=dict(l=70, r=70, t=60, b=50))
-    return fig
+    if not isinstance(q, list):
+        q_sym = q
+        scores = scores["noncon_scores"]
+        confidence_levels = np.arange(len(scores)) / len(scores)
+        fig = px.line(
+            pd.DataFrame({"Confidence Level": confidence_levels, "One-Sided Interval Width": scores}),
+            x="Confidence Level",
+            y="One-Sided Interval Width",
+            title=f"{method} One-Sided Interval Width with q",
+            width=600,
+            height=400,
+        )
+        fig.add_vline(
+            x=1 - alpha,
+            annotation_text=f"(1-alpha) = {1 - alpha}",
+            annotation_position="top left",
+            line_width=1,
+            line_color="green",
+        )
+        fig.add_hline(
+            y=q,
+            annotation_text=f"q1 = {round(q_sym, 2)}",
+            annotation_position="top left",
+            line_width=1,
+            line_color="red",
+        )
+        fig.update_layout(margin=dict(l=70, r=70, t=60, b=50))
+        return fig
+    else:
+        q_lo, q_hi = q
+        scores_lo = scores["noncon_scores_lo"]
+        scores_hi = scores["noncon_scores_hi"]
+        alpha_lo, alpha_hi = alpha
+        confidence_levels = np.arange(len(scores_lo)) / len(scores_lo)
+        fig = px.line(
+            pd.DataFrame(
+                {
+                    "Confidence Level": confidence_levels,
+                    "One-Sided Lower Interval Width": scores_lo,
+                    "One-Sided Upper Interval Width": scores_hi,
+                }
+            ),
+            x="Confidence Level",
+            y=["One-Sided Lower Interval Width", "One-Sided Upper Interval Width"],
+            title=f"{method} One-Sided Interval Width with q",
+            width=600,
+            height=400,
+        )
+        fig.add_vline(
+            x=1 - alpha_lo,
+            annotation_text=f"(1-alpha) = {round(1-alpha_lo, 10)}",
+            annotation_position="top left",
+            line_width=1,
+            line_color="green",
+        )
+        fig.add_vline(
+            x=1 - alpha_hi,
+            annotation_text=f"(1-alpha) = {round(1 - alpha_hi, 10)}",
+            annotation_position="bottom left",
+            line_width=1,
+            line_color="green",
+        )
+        fig.add_hline(
+            y=q_lo,
+            annotation_text=f"q1_lo = {round(q_lo, 2)}",
+            annotation_position="top left",
+            line_width=1,
+            line_color="red",
+        )
+        fig.add_hline(
+            y=q_hi,
+            annotation_text=f"q1_hi = {round(q_hi, 2)}",
+            annotation_position="bottom left",
+            line_width=1,
+            line_color="red",
+        )
+        fig.update_layout(margin=dict(l=70, r=70, t=60, b=50))
+        return fig
 
 
 def plot_interval_width_per_timestep(q_hats, method, resampler_active=False):
     """Plot the nonconformity scores as well as the one-sided interval width (q).
 
     Parameters
     ----------
-        q_hats : list
+        q_hats : dataframe
             prediction interval widths (or q) for each timestep
         method : str
             name of conformal prediction technique used
 
             Options
                 * (default) ``naive``: Naive or Absolute Residual
                 * ``cqr``: Conformalized Quantile Regression
@@ -780,18 +838,39 @@
         plotly.graph_objects.Figure
             Figure showing the q-values for each timestep
     """
     if resampler_active:
         register_plotly_resampler(mode="auto")
     else:
         unregister_plotly_resampler()
-    timestep_numbers = list(range(1, len(q_hats) + 1))
-    fig = px.line(
-        pd.DataFrame({"Timestep Number": timestep_numbers, "One-Sided Interval Width": q_hats}),
-        x="Timestep Number",
-        y="One-Sided Interval Width",
-        title=f"{method} One-Sided Interval Width with q per Timestep",
-        width=600,
-        height=400,
-    )
+    # check if q_hats contains q_hat_sym
+    if "q_hat_sym" in q_hats.columns:
+        q_hats_sym = q_hats["q_hat_sym"]
+        timestep_numbers = list(range(1, len(q_hats_sym) + 1))
+        fig = px.line(
+            pd.DataFrame({"Timestep Number": timestep_numbers, "One-Sided Interval Width": q_hats_sym}),
+            x="Timestep Number",
+            y="One-Sided Interval Width",
+            title=f"{method} One-Sided Interval Width with q per Timestep",
+            width=600,
+            height=400,
+        )
+    else:
+        q_hats_lo = q_hats["q_hat_lo"]
+        q_hats_hi = q_hats["q_hat_hi"]
+        timestep_numbers = list(range(1, len(q_hats_lo) + 1))
+        fig = px.line(
+            pd.DataFrame(
+                {
+                    "Timestep Number": timestep_numbers,
+                    "One-Sided Lower Interval Width": q_hats_lo,
+                    "One-Sided Upper Interval Width": q_hats_hi,
+                }
+            ),
+            x="Timestep Number",
+            y=["One-Sided Lower Interval Width", "One-Sided Upper Interval Width"],
+            title=f"{method} One-Sided Interval Width with q per Timestep",
+            width=600,
+            height=400,
+        )
     fig.update_layout(margin=dict(l=70, r=70, t=60, b=50))
     return fig
```

### Comparing `neuralprophet-0.5.4/neuralprophet/plot_model_parameters_matplotlib.py` & `neuralprophet-0.6.0rc1/neuralprophet/plot_model_parameters_matplotlib.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     Base usage of :meth:`plot_parameters`
 
     >>> from neuralprophet import NeuralProphet
     >>> m = NeuralProphet()
     >>> metrics = m.fit(df, freq="D")
     >>> future = m.make_future_dataframe(df=df, periods=365)
     >>> forecast = m.predict(df=future)
-    >>> fig_param = m.plot_parameters()
+    >>> m.plot_parameters()
 
     """
     components_to_plot = plot_configuration["components_list"]
     additive_future_regressors = plot_configuration["additive_future_regressors"]
     additive_events = plot_configuration["additive_events"]
     multiplicative_future_regressors = plot_configuration["multiplicative_future_regressors"]
     multiplicative_events = plot_configuration["multiplicative_events"]
@@ -133,15 +133,15 @@
                 weights = lagged_scalar_regressors
             elif plot_name == "additive event":
                 weights = additive_events
             elif plot_name == "multiplicative event":
                 multiplicative_axes.append(ax)
                 weights = multiplicative_events
             plot_scalar_weights(weights=weights, plot_name=comp["plot_name"], focus=forecast_in_focus, ax=ax)
-    fig.tight_layout()
+    fig = fig.tight_layout()
     # Reset multiplicative axes labels after tight_layout adjustment
     for ax in multiplicative_axes:
         ax = set_y_as_percent(ax)
     if overwriting_unknown_data_normalization:
         # if overwriting_unknown_data_normalization is True, we get back to the initial False state
         m.config_normalization.unknown_data_normalization = False
```

### Comparing `neuralprophet-0.5.4/neuralprophet/plot_model_parameters_plotly.py` & `neuralprophet-0.6.0rc1/neuralprophet/plot_model_parameters_plotly.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.5.4/neuralprophet/plot_utils.py` & `neuralprophet-0.6.0rc1/neuralprophet/plot_utils.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.5.4/neuralprophet/time_dataset.py` & `neuralprophet-0.6.0rc1/neuralprophet/time_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -119,14 +119,15 @@
             inputs : ordered dict
                 Identical to returns from :meth:`tabularize_univariate_datetime`
             targets : np.array, float
                 Identical to returns from :meth:`tabularize_univariate_datetime`
         """
         inputs_dtype = {
             "time": torch.float,
+            "timestamps": np.datetime64,
             # "changepoints": torch.bool,
             "seasonalities": torch.float,
             "events": torch.float,
             "lags": torch.float,
             "covariates": torch.float,
             "regressors": torch.float,
         }
@@ -135,15 +136,18 @@
 
         for key, data in inputs.items():
             if key in self.two_level_inputs or key == "events" or key == "regressors":
                 self.inputs[key] = OrderedDict({})
                 for name, features in data.items():
                     self.inputs[key][name] = torch.from_numpy(features.astype(float)).type(inputs_dtype[key])
             else:
-                self.inputs[key] = torch.from_numpy(data).type(inputs_dtype[key])
+                if key == "timestamps":
+                    self.inputs[key] = data
+                else:
+                    self.inputs[key] = torch.from_numpy(data).type(inputs_dtype[key])
         self.targets = torch.from_numpy(targets).type(targets_dtype).unsqueeze(dim=2)
         self.meta["df_name"] = self.name
         # Pre-compute all samples for faster iteration in __getitem__
         self.samples = []
         for index in range(self.length):
             sample = OrderedDict({})
             for key, data in self.inputs.items():
@@ -172,15 +176,40 @@
 
             Note
             ----
             E.g. if prediction_frequency=7, forecasts are only made on every 7th step (once in a week in case of daily resolution).
         """
         if prediction_frequency is None or prediction_frequency == 1:
             return
-        self.samples = self.samples[::prediction_frequency]
+        # Only the first target timestamp is of interest for filtering
+        timestamps = pd.to_datetime([sample["timestamps"][0] for sample in self.samples])
+        masks = []
+        for key, value in prediction_frequency.items():
+            if key == "daily-hour":
+                mask = timestamps.hour == value + 1  # + 1 because prediction starts one step after origin
+            elif key == "weekly-day":
+                mask = timestamps.dayofweek == value + 1
+            elif key == "monthly-day":
+                mask = timestamps.day == value + 1
+            elif key == "yearly-month":
+                mask = timestamps.month == value + 1
+            elif key == "hourly-minute":
+                mask = timestamps.minute == value + 1
+            else:
+                raise ValueError(f"Invalid prediction frequency: {key}")
+            masks.append(mask)
+        mask = np.ones((len(timestamps),), dtype=bool)
+        for m in masks:
+            mask = mask & m
+        self.samples = [self.samples[i] for i in range(len(self.samples)) if mask[i]]
+
+        # Exact timestamps are not needed anymore
+        self.inputs.pop("timestamps")
+        for sample in self.samples:
+            sample.pop("timestamps")
         self.length = len(self.samples)
 
     def __getitem__(self, index):
         """Overrides parent class method to get an item at index.
 
         Parameters
         ----------
@@ -292,25 +321,37 @@
     max_lags = get_max_num_lags(config_lagged_regressors, n_lags)
     n_samples = len(df) - max_lags + 1 - n_forecasts
     # data is stored in OrderedDict
     inputs = OrderedDict({})
 
     def _stride_time_features_for_forecasts(x):
         # only for case where n_lags > 0
-        return np.array([x[max_lags + i : max_lags + i + n_forecasts] for i in range(n_samples)], dtype=np.float64)
+        if x.dtype != np.float64:
+            dtype = np.datetime64
+        else:
+            dtype = np.float64
+        return np.array([x[max_lags + i : max_lags + i + n_forecasts] for i in range(n_samples)], dtype=dtype)
 
     # time is the time at each forecast step
     t = df.loc[:, "t"].values
     if max_lags == 0:
         assert n_forecasts == 1
         time = np.expand_dims(t, 1)
     else:
         time = _stride_time_features_for_forecasts(t)
     inputs["time"] = time
 
+    if prediction_frequency is not None:
+        ds = df.loc[:, "ds"].values
+        if max_lags == 0:
+            timestamps = np.expand_dims(ds, 1)
+        else:
+            timestamps = _stride_time_features_for_forecasts(ds)
+        inputs["timestamps"] = timestamps
+
     if config_seasonality is not None:
         seasonalities = seasonal_features_from_dates(df, config_seasonality)
         for name, features in seasonalities.items():
             if max_lags == 0:
                 seasonalities[name] = np.expand_dims(features, axis=1)
             else:
                 # stride into num_forecast at dim=1 for each sample, just like we did with time
```

### Comparing `neuralprophet-0.5.4/neuralprophet/time_net.py` & `neuralprophet-0.6.0rc1/neuralprophet/time_net.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.5.4/neuralprophet/torch_prophet.py` & `neuralprophet-0.6.0rc1/neuralprophet/torch_prophet.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.5.4/neuralprophet/utils.py` & `neuralprophet-0.6.0rc1/neuralprophet/utils.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.5.4/neuralprophet/utils_metrics.py` & `neuralprophet-0.6.0rc1/neuralprophet/utils_metrics.py`

 * *Files identical despite different names*

### Comparing `neuralprophet-0.5.4/neuralprophet/utils_torch.py` & `neuralprophet-0.6.0rc1/neuralprophet/utils_torch.py`

 * *Files identical despite different names*

