# Comparing `tmp/explainaboard-api-client-0.4.1.tar.gz` & `tmp/explainaboard-api-client-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "explainaboard-api-client-0.4.1.tar", last modified: Mon Mar 20 19:09:53 2023, max compression
+gzip compressed data, was "explainaboard-api-client-0.4.2.tar", last modified: Sat Apr 15 10:28:31 2023, max compression
```

## Comparing `explainaboard-api-client-0.4.1.tar` & `explainaboard-api-client-0.4.2.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:09:53.284647 explainaboard-api-client-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-20 19:09:53.284647 explainaboard-api-client-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10653 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:09:53.272647 explainaboard-api-client-0.4.1/explainaboard_api_client/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:09:53.272647 explainaboard-api-client-0.4.1/explainaboard_api_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   106116 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/api/default_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    37655 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:09:53.272647 explainaboard-api-client-0.4.1/explainaboard_api_client/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17099 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:09:53.280647 explainaboard-api-client-0.4.1/explainaboard_api_client/model/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    11020 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/analysis_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/analysis_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    11899 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/analysis_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    10802 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/any_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11331 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/api_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    11291 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/api_systems_analyses_feature_to_bucket_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/benchmark_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/benchmark_config_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    16041 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/benchmark_create_props.py
--rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/benchmark_dataset_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11505 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/benchmark_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/benchmark_operation_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12653 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/benchmark_table_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    15649 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/benchmark_update_props.py
--rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/benchmark_view_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13010 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/class_label.py
--rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/combo_count.py
--rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/confidence_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/dataset_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/dataset_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    11593 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/datasets_return.py
--rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/feature_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12025 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/inline_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/inline_response200.py
--rw-r--r--   0 runner    (1001) docker     (123)    11485 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/language_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    11312 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/metric_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/metric_result_values.py
--rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/paper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/score.py
--rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/significance_test_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11868 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/single_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    17003 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/system.py
--rw-r--r--   0 runner    (1001) docker     (123)    15595 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/system_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/system_all_of_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12158 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/system_analyses_return.py
--rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/system_create_props.py
--rw-r--r--   0 runner    (1001) docker     (123)    15622 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/system_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/system_info_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/system_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/system_metadata_updatable.py
--rw-r--r--   0 runner    (1001) docker     (123)    11015 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/system_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/system_output_props.py
--rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/system_update_props.py
--rw-r--r--   0 runner    (1001) docker     (123)    11513 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/systems_return.py
--rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/task_category.py
--rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/task_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    11472 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/task_supported_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/time.py
--rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12158 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12535 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model/value.py
--rw-r--r--   0 runner    (1001) docker     (123)    82049 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:09:53.280647 explainaboard-api-client-0.4.1/explainaboard_api_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14152 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/explainaboard_api_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:09:53.272647 explainaboard-api-client-0.4.1/explainaboard_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-20 19:09:53.000000 explainaboard-api-client-0.4.1/explainaboard_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-03-20 19:09:53.000000 explainaboard-api-client-0.4.1/explainaboard_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 19:09:53.000000 explainaboard-api-client-0.4.1/explainaboard_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-20 19:09:53.000000 explainaboard-api-client-0.4.1/explainaboard_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-20 19:09:53.000000 explainaboard-api-client-0.4.1/explainaboard_api_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-20 19:09:53.284647 explainaboard-api-client-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:09:53.284647 explainaboard-api-client-0.4.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_analysis_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_analysis_level.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_analysis_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_any_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_api_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_api_systems_analyses_feature_to_bucket_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_benchmark_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_benchmark_config_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_benchmark_create_props.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_benchmark_dataset_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_benchmark_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_benchmark_operation_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_benchmark_table_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_benchmark_update_props.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_benchmark_view_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_class_label.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_combo_count.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_confidence_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_dataset_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_dataset_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_datasets_return.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_default_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_feature_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_inline_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_inline_response200.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_language_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_metric_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_metric_result_values.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_paper.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_score.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_significance_test_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_single_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_system_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_system_all_of_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_system_analyses_return.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_system_create_props.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_system_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_system_info_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_system_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_system_metadata_updatable.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_system_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_system_output_props.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_system_update_props.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_systems_return.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_task_category.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_task_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_task_supported_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-20 19:09:49.000000 explainaboard-api-client-0.4.1/test/test_value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:28:31.901709 explainaboard-api-client-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-15 10:28:31.901709 explainaboard-api-client-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10653 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:28:31.881709 explainaboard-api-client-0.4.2/explainaboard_api_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:28:31.885709 explainaboard-api-client-0.4.2/explainaboard_api_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106116 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/api/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37655 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:28:31.885709 explainaboard-api-client-0.4.2/explainaboard_api_client/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17099 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:28:31.893709 explainaboard-api-client-0.4.2/explainaboard_api_client/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11020 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/analysis_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/analysis_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11899 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/analysis_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10802 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/any_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11331 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/api_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11291 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/api_systems_analyses_feature_to_bucket_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/benchmark_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/benchmark_config_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16041 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/benchmark_create_props.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/benchmark_dataset_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11505 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/benchmark_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/benchmark_operation_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12653 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/benchmark_table_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15649 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/benchmark_update_props.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/benchmark_view_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13010 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/class_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/combo_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11453 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/confidence_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/dataset_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/dataset_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11593 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/datasets_return.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/feature_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12025 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/inline_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/inline_response200.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11485 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/language_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11312 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/metric_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/metric_result_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/paper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/score.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/significance_test_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11868 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/single_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17003 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15595 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/system_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/system_all_of_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12158 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/system_analyses_return.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/system_create_props.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15622 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/system_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/system_info_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/system_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/system_metadata_updatable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11015 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/system_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/system_output_props.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/system_update_props.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11513 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/systems_return.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/task_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/task_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11472 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/task_supported_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12158 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12535 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82049 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:28:31.893709 explainaboard-api-client-0.4.2/explainaboard_api_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14152 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/explainaboard_api_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:28:31.885709 explainaboard-api-client-0.4.2/explainaboard_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-15 10:28:31.000000 explainaboard-api-client-0.4.2/explainaboard_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-15 10:28:31.000000 explainaboard-api-client-0.4.2/explainaboard_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 10:28:31.000000 explainaboard-api-client-0.4.2/explainaboard_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-15 10:28:31.000000 explainaboard-api-client-0.4.2/explainaboard_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-15 10:28:31.000000 explainaboard-api-client-0.4.2/explainaboard_api_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-15 10:28:31.901709 explainaboard-api-client-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:28:31.901709 explainaboard-api-client-0.4.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_analysis_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_analysis_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_analysis_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_any_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_api_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_api_systems_analyses_feature_to_bucket_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_benchmark_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_benchmark_config_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_benchmark_create_props.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_benchmark_dataset_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_benchmark_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_benchmark_operation_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_benchmark_table_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_benchmark_update_props.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_benchmark_view_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_class_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_combo_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_confidence_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_dataset_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_dataset_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_datasets_return.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_default_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_feature_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_inline_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_inline_response200.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_language_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_metric_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_metric_result_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_paper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_significance_test_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_single_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_system_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_system_all_of_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_system_analyses_return.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_system_create_props.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_system_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_system_info_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_system_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_system_metadata_updatable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_system_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_system_output_props.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_system_update_props.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_systems_return.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_task_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_task_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_task_supported_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-15 10:28:27.000000 explainaboard-api-client-0.4.2/test/test_value.py
```

### Comparing `explainaboard-api-client-0.4.1/README.md` & `explainaboard-api-client-0.4.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # explainaboard-api-client
 Backend APIs for ExplainaBoard
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.4.1
-- Package version: 0.4.1
+- API version: 0.4.2
+- Package version: 0.4.2
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python >=3.6
 
 ## Installation & Usage
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/__init__.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # flake8: noqa
 
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 
 # import ApiClient
 from explainaboard_api_client.api_client import ApiClient
 
 # import Configuration
 from explainaboard_api_client.configuration import Configuration
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/api/default_api.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/api/default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/api_client.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
 import mimetypes
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.4.1/python'
+        self.user_agent = 'OpenAPI-Generator/0.4.2/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/configuration.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
 import multiprocessing
@@ -406,16 +406,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.4.1\n"\
-               "SDK Package Version: 0.4.1".\
+               "Version of the API: 0.4.2\n"\
+               "SDK Package Version: 0.4.2".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/exceptions.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/analysis.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/analysis_case.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/analysis_case.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/analysis_level.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/analysis_level.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/analysis_result.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/analysis_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/any_type.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/any_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/api_error.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/api_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/api_systems_analyses_feature_to_bucket_info.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/api_systems_analyses_feature_to_bucket_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/benchmark.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/benchmark.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/benchmark_config.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/benchmark_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/benchmark_config_all_of.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/benchmark_config_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/benchmark_create_props.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/benchmark_create_props.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/benchmark_dataset_config.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/benchmark_dataset_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/benchmark_metric.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/benchmark_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/benchmark_operation_config.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/benchmark_operation_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/benchmark_table_data.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/benchmark_table_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/benchmark_update_props.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/benchmark_update_props.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/benchmark_view_config.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/benchmark_view_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/class_label.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/class_label.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/combo_count.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/combo_count.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/confidence_interval.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/confidence_interval.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/dataset_feature.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/dataset_feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/dataset_metadata.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/value.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -25,20 +25,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from explainaboard_api_client.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from explainaboard_api_client.model.dataset_feature import DatasetFeature
-    globals()['DatasetFeature'] = DatasetFeature
 
-
-class DatasetMetadata(ModelNormal):
+class Value(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -68,90 +64,63 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'dataset_id': (str,),  # noqa: E501
-            'dataset_name': (str,),  # noqa: E501
-            'tasks': ([str],),  # noqa: E501
-            'sub_dataset': (str, none_type,),  # noqa: E501
-            'split': ({str: (int,)},),  # noqa: E501
-            'summary': (str,),  # noqa: E501
-            'homepage': (str, none_type,),  # noqa: E501
-            'repository': (str, none_type,),  # noqa: E501
-            'leaderboard': (str,),  # noqa: E501
-            'person_of_contact': (str, none_type,),  # noqa: E501
-            'task_categories': ([str],),  # noqa: E501
-            'languages': ([str],),  # noqa: E501
-            'features': ({str: (DatasetFeature,)},),  # noqa: E501
-            'speaker_demographic': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'annotator_demographic': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'speech_situation': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),  # noqa: E501
-            'huggingface_link': (str,),  # noqa: E501
+            'dtype': (str,),  # noqa: E501
+            'description': (str, none_type,),  # noqa: E501
+            'is_bucket': (bool,),  # noqa: E501
+            'require_training_set': (bool,),  # noqa: E501
+            'bucket_info': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
+            'id': (str, none_type,),  # noqa: E501
+            'cls_name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
     attribute_map = {
-        'dataset_id': 'dataset_id',  # noqa: E501
-        'dataset_name': 'dataset_name',  # noqa: E501
-        'tasks': 'tasks',  # noqa: E501
-        'sub_dataset': 'sub_dataset',  # noqa: E501
-        'split': 'split',  # noqa: E501
-        'summary': 'summary',  # noqa: E501
-        'homepage': 'homepage',  # noqa: E501
-        'repository': 'repository',  # noqa: E501
-        'leaderboard': 'leaderboard',  # noqa: E501
-        'person_of_contact': 'person_of_contact',  # noqa: E501
-        'task_categories': 'task_categories',  # noqa: E501
-        'languages': 'languages',  # noqa: E501
-        'features': 'features',  # noqa: E501
-        'speaker_demographic': 'speaker_demographic',  # noqa: E501
-        'annotator_demographic': 'annotator_demographic',  # noqa: E501
-        'speech_situation': 'speech_situation',  # noqa: E501
-        'huggingface_link': 'huggingface_link',  # noqa: E501
+        'dtype': 'dtype',  # noqa: E501
+        'description': 'description',  # noqa: E501
+        'is_bucket': 'is_bucket',  # noqa: E501
+        'require_training_set': 'require_training_set',  # noqa: E501
+        'bucket_info': 'bucket_info',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'cls_name': 'cls_name',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, dataset_id, dataset_name, tasks, *args, **kwargs):  # noqa: E501
-        """DatasetMetadata - a model defined in OpenAPI
-
-        Args:
-            dataset_id (str):
-            dataset_name (str):
-            tasks ([str]):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """Value - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -177,28 +146,21 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
 
-            sub_dataset (str, none_type): sub dataset id (TODO). [optional]  # noqa: E501
-            split ({str: (int,)}): [optional]  # noqa: E501
-            summary (str): [optional]  # noqa: E501
-            homepage (str, none_type): [optional]  # noqa: E501
-            repository (str, none_type): [optional]  # noqa: E501
-            leaderboard (str): [optional]  # noqa: E501
-            person_of_contact (str, none_type): [optional]  # noqa: E501
-            task_categories ([str]): [optional]  # noqa: E501
-            languages ([str]): [optional]  # noqa: E501
-            features ({str: (DatasetFeature,)}): [optional]  # noqa: E501
-            speaker_demographic ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            annotator_demographic ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            speech_situation ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            huggingface_link (str): [optional]  # noqa: E501
+            dtype (str): [optional]  # noqa: E501
+            description (str, none_type): [optional]  # noqa: E501
+            is_bucket (bool): [optional]  # noqa: E501
+            require_training_set (bool): [optional]  # noqa: E501
+            bucket_info ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): [optional]  # noqa: E501
+            id (str, none_type): [optional]  # noqa: E501
+            cls_name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -220,17 +182,14 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
 
-        self.dataset_id = dataset_id
-        self.dataset_name = dataset_name
-        self.tasks = tasks
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -244,21 +203,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, dataset_id, dataset_name, tasks, *args, **kwargs):  # noqa: E501
-        """DatasetMetadata - a model defined in OpenAPI
-
-        Args:
-            dataset_id (str):
-            dataset_name (str):
-            tasks ([str]):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """Value - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -284,28 +238,21 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
 
-            sub_dataset (str, none_type): sub dataset id (TODO). [optional]  # noqa: E501
-            split ({str: (int,)}): [optional]  # noqa: E501
-            summary (str): [optional]  # noqa: E501
-            homepage (str, none_type): [optional]  # noqa: E501
-            repository (str, none_type): [optional]  # noqa: E501
-            leaderboard (str): [optional]  # noqa: E501
-            person_of_contact (str, none_type): [optional]  # noqa: E501
-            task_categories ([str]): [optional]  # noqa: E501
-            languages ([str]): [optional]  # noqa: E501
-            features ({str: (DatasetFeature,)}): [optional]  # noqa: E501
-            speaker_demographic ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            annotator_demographic ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            speech_situation ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
-            huggingface_link (str): [optional]  # noqa: E501
+            dtype (str): [optional]  # noqa: E501
+            description (str, none_type): [optional]  # noqa: E501
+            is_bucket (bool): [optional]  # noqa: E501
+            require_training_set (bool): [optional]  # noqa: E501
+            bucket_info ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): [optional]  # noqa: E501
+            id (str, none_type): [optional]  # noqa: E501
+            cls_name (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -325,17 +272,14 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
 
-        self.dataset_id = dataset_id
-        self.dataset_name = dataset_name
-        self.tasks = tasks
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/datasets_return.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/datasets_return.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/feature_type.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/feature_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/inline_object.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/inline_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/inline_response200.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/inline_response200.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/language_code.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/language_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/metric_result.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/metric_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/metric_result_values.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/metric_result_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/paper.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/paper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/score.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/score.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/significance_test_info.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/significance_test_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/single_analysis.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/single_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/system.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/system.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/system_all_of.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/system_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/system_all_of_dataset.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/system_all_of_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/system_analyses_return.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/system_analyses_return.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/system_create_props.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/system_create_props.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/system_info.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/system_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/system_info_results.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/system_info_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/system_metadata.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/system_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/system_metadata_updatable.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/system_metadata_updatable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/system_output.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/system_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/system_output_props.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/system_output_props.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/system_update_props.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/system_update_props.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/systems_return.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/systems_return.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/task.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/task_category.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/task_category.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/task_metadata.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/task_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/task_supported_formats.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/task_supported_formats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/time.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/time.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/tokenizer.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/tokenizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/user.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model/value.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model/dataset_metadata.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from explainaboard_api_client.exceptions import ApiAttributeError
 
 
 
-class Value(ModelNormal):
+class DatasetMetadata(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -79,48 +79,51 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'dtype': (str,),  # noqa: E501
-            'description': (str, none_type,),  # noqa: E501
-            'is_bucket': (bool,),  # noqa: E501
-            'require_training_set': (bool,),  # noqa: E501
-            'bucket_info': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
-            'id': (str, none_type,),  # noqa: E501
-            'cls_name': (str,),  # noqa: E501
+            'dataset_id': (str,),  # noqa: E501
+            'dataset_name': (str,),  # noqa: E501
+            'tasks': ([str],),  # noqa: E501
+            'sub_dataset': (str, none_type,),  # noqa: E501
+            'split': ({str: (int,)},),  # noqa: E501
+            'languages': ([str],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
 
     attribute_map = {
-        'dtype': 'dtype',  # noqa: E501
-        'description': 'description',  # noqa: E501
-        'is_bucket': 'is_bucket',  # noqa: E501
-        'require_training_set': 'require_training_set',  # noqa: E501
-        'bucket_info': 'bucket_info',  # noqa: E501
-        'id': 'id',  # noqa: E501
-        'cls_name': 'cls_name',  # noqa: E501
+        'dataset_id': 'dataset_id',  # noqa: E501
+        'dataset_name': 'dataset_name',  # noqa: E501
+        'tasks': 'tasks',  # noqa: E501
+        'sub_dataset': 'sub_dataset',  # noqa: E501
+        'split': 'split',  # noqa: E501
+        'languages': 'languages',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Value - a model defined in OpenAPI
+    def _from_openapi_data(cls, dataset_id, dataset_name, tasks, *args, **kwargs):  # noqa: E501
+        """DatasetMetadata - a model defined in OpenAPI
+
+        Args:
+            dataset_id (str):
+            dataset_name (str):
+            tasks ([str]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -146,21 +149,17 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
 
-            dtype (str): [optional]  # noqa: E501
-            description (str, none_type): [optional]  # noqa: E501
-            is_bucket (bool): [optional]  # noqa: E501
-            require_training_set (bool): [optional]  # noqa: E501
-            bucket_info ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): [optional]  # noqa: E501
-            id (str, none_type): [optional]  # noqa: E501
-            cls_name (str): [optional]  # noqa: E501
+            sub_dataset (str, none_type): sub dataset id (TODO). [optional]  # noqa: E501
+            split ({str: (int,)}): [optional]  # noqa: E501
+            languages ([str]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -182,14 +181,17 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
 
+        self.dataset_id = dataset_id
+        self.dataset_name = dataset_name
+        self.tasks = tasks
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -203,16 +205,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *args, **kwargs):  # noqa: E501
-        """Value - a model defined in OpenAPI
+    def __init__(self, dataset_id, dataset_name, tasks, *args, **kwargs):  # noqa: E501
+        """DatasetMetadata - a model defined in OpenAPI
+
+        Args:
+            dataset_id (str):
+            dataset_name (str):
+            tasks ([str]):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -238,21 +245,17 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
 
-            dtype (str): [optional]  # noqa: E501
-            description (str, none_type): [optional]  # noqa: E501
-            is_bucket (bool): [optional]  # noqa: E501
-            require_training_set (bool): [optional]  # noqa: E501
-            bucket_info ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): [optional]  # noqa: E501
-            id (str, none_type): [optional]  # noqa: E501
-            cls_name (str): [optional]  # noqa: E501
+            sub_dataset (str, none_type): sub dataset id (TODO). [optional]  # noqa: E501
+            split ({str: (int,)}): [optional]  # noqa: E501
+            languages ([str]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -272,14 +275,17 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
 
+        self.dataset_id = dataset_id
+        self.dataset_name = dataset_name
+        self.tasks = tasks
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/model_utils.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/models/__init__.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client/rest.py` & `explainaboard-api-client-0.4.2/explainaboard_api_client/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
 import logging
```

### Comparing `explainaboard-api-client-0.4.1/explainaboard_api_client.egg-info/SOURCES.txt` & `explainaboard-api-client-0.4.2/explainaboard_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `explainaboard-api-client-0.4.1/setup.py` & `explainaboard-api-client-0.4.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "explainaboard-api-client"
-VERSION = "0.4.1"
+VERSION = "0.4.2"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `explainaboard-api-client-0.4.1/test/test_analysis.py` & `explainaboard-api-client-0.4.2/test/test_analysis.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_analysis_case.py` & `explainaboard-api-client-0.4.2/test/test_analysis_case.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_analysis_level.py` & `explainaboard-api-client-0.4.2/test/test_analysis_level.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_analysis_result.py` & `explainaboard-api-client-0.4.2/test/test_task.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import explainaboard_api_client
-from explainaboard_api_client.model.analysis_result import AnalysisResult
+from explainaboard_api_client.model.task_supported_formats import TaskSupportedFormats
+globals()['TaskSupportedFormats'] = TaskSupportedFormats
+from explainaboard_api_client.model.task import Task
 
 
-class TestAnalysisResult(unittest.TestCase):
-    """AnalysisResult unit test stubs"""
+class TestTask(unittest.TestCase):
+    """Task unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAnalysisResult(self):
-        """Test AnalysisResult"""
+    def testTask(self):
+        """Test Task"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = AnalysisResult()  # noqa: E501
+        # model = Task()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `explainaboard-api-client-0.4.1/test/test_any_type.py` & `explainaboard-api-client-0.4.2/test/test_any_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_api_error.py` & `explainaboard-api-client-0.4.2/test/test_api_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_api_systems_analyses_feature_to_bucket_info.py` & `explainaboard-api-client-0.4.2/test/test_api_systems_analyses_feature_to_bucket_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_benchmark.py` & `explainaboard-api-client-0.4.2/test/test_benchmark.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_benchmark_config.py` & `explainaboard-api-client-0.4.2/test/test_benchmark_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_benchmark_config_all_of.py` & `explainaboard-api-client-0.4.2/test/test_benchmark_config_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_benchmark_create_props.py` & `explainaboard-api-client-0.4.2/test/test_benchmark_create_props.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_benchmark_dataset_config.py` & `explainaboard-api-client-0.4.2/test/test_benchmark_dataset_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_benchmark_metric.py` & `explainaboard-api-client-0.4.2/test/test_benchmark_metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_benchmark_operation_config.py` & `explainaboard-api-client-0.4.2/test/test_benchmark_operation_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_benchmark_table_data.py` & `explainaboard-api-client-0.4.2/test/test_benchmark_table_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_benchmark_update_props.py` & `explainaboard-api-client-0.4.2/test/test_benchmark_update_props.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_benchmark_view_config.py` & `explainaboard-api-client-0.4.2/test/test_benchmark_view_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_class_label.py` & `explainaboard-api-client-0.4.2/test/test_class_label.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_combo_count.py` & `explainaboard-api-client-0.4.2/test/test_combo_count.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_confidence_interval.py` & `explainaboard-api-client-0.4.2/test/test_confidence_interval.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_dataset_feature.py` & `explainaboard-api-client-0.4.2/test/test_dataset_feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_dataset_metadata.py` & `explainaboard-api-client-0.4.2/test/test_analysis_result.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import explainaboard_api_client
-from explainaboard_api_client.model.dataset_feature import DatasetFeature
-globals()['DatasetFeature'] = DatasetFeature
-from explainaboard_api_client.model.dataset_metadata import DatasetMetadata
+from explainaboard_api_client.model.analysis_result import AnalysisResult
 
 
-class TestDatasetMetadata(unittest.TestCase):
-    """DatasetMetadata unit test stubs"""
+class TestAnalysisResult(unittest.TestCase):
+    """AnalysisResult unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testDatasetMetadata(self):
-        """Test DatasetMetadata"""
+    def testAnalysisResult(self):
+        """Test AnalysisResult"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = DatasetMetadata()  # noqa: E501
+        # model = AnalysisResult()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `explainaboard-api-client-0.4.1/test/test_datasets_return.py` & `explainaboard-api-client-0.4.2/test/test_datasets_return.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_default_api.py` & `explainaboard-api-client-0.4.2/test/test_default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
 
 import explainaboard_api_client
```

### Comparing `explainaboard-api-client-0.4.1/test/test_feature_type.py` & `explainaboard-api-client-0.4.2/test/test_feature_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_inline_object.py` & `explainaboard-api-client-0.4.2/test/test_inline_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_inline_response200.py` & `explainaboard-api-client-0.4.2/test/test_inline_response200.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_language_code.py` & `explainaboard-api-client-0.4.2/test/test_language_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_metric_result.py` & `explainaboard-api-client-0.4.2/test/test_metric_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_metric_result_values.py` & `explainaboard-api-client-0.4.2/test/test_metric_result_values.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_paper.py` & `explainaboard-api-client-0.4.2/test/test_paper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_score.py` & `explainaboard-api-client-0.4.2/test/test_score.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_significance_test_info.py` & `explainaboard-api-client-0.4.2/test/test_significance_test_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_single_analysis.py` & `explainaboard-api-client-0.4.2/test/test_single_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_system.py` & `explainaboard-api-client-0.4.2/test/test_system.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_system_all_of.py` & `explainaboard-api-client-0.4.2/test/test_system_all_of.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_system_all_of_dataset.py` & `explainaboard-api-client-0.4.2/test/test_system_all_of_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_system_analyses_return.py` & `explainaboard-api-client-0.4.2/test/test_system_analyses_return.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_system_create_props.py` & `explainaboard-api-client-0.4.2/test/test_system_create_props.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_system_info.py` & `explainaboard-api-client-0.4.2/test/test_system_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_system_info_results.py` & `explainaboard-api-client-0.4.2/test/test_system_info_results.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_system_metadata.py` & `explainaboard-api-client-0.4.2/test/test_system_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_system_metadata_updatable.py` & `explainaboard-api-client-0.4.2/test/test_system_metadata_updatable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_system_output.py` & `explainaboard-api-client-0.4.2/test/test_system_output.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_system_output_props.py` & `explainaboard-api-client-0.4.2/test/test_system_output_props.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_system_update_props.py` & `explainaboard-api-client-0.4.2/test/test_system_update_props.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_systems_return.py` & `explainaboard-api-client-0.4.2/test/test_systems_return.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_task.py` & `explainaboard-api-client-0.4.2/test/test_task_supported_formats.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import explainaboard_api_client
 from explainaboard_api_client.model.task_supported_formats import TaskSupportedFormats
-globals()['TaskSupportedFormats'] = TaskSupportedFormats
-from explainaboard_api_client.model.task import Task
 
 
-class TestTask(unittest.TestCase):
-    """Task unit test stubs"""
+class TestTaskSupportedFormats(unittest.TestCase):
+    """TaskSupportedFormats unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTask(self):
-        """Test Task"""
+    def testTaskSupportedFormats(self):
+        """Test TaskSupportedFormats"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = Task()  # noqa: E501
+        # model = TaskSupportedFormats()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `explainaboard-api-client-0.4.1/test/test_task_category.py` & `explainaboard-api-client-0.4.2/test/test_task_category.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_task_metadata.py` & `explainaboard-api-client-0.4.2/test/test_task_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_task_supported_formats.py` & `explainaboard-api-client-0.4.2/test/test_value.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import explainaboard_api_client
-from explainaboard_api_client.model.task_supported_formats import TaskSupportedFormats
+from explainaboard_api_client.model.value import Value
 
 
-class TestTaskSupportedFormats(unittest.TestCase):
-    """TaskSupportedFormats unit test stubs"""
+class TestValue(unittest.TestCase):
+    """Value unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTaskSupportedFormats(self):
-        """Test TaskSupportedFormats"""
+    def testValue(self):
+        """Test Value"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = TaskSupportedFormats()  # noqa: E501
+        # model = Value()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `explainaboard-api-client-0.4.1/test/test_time.py` & `explainaboard-api-client-0.4.2/test/test_time.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_tokenizer.py` & `explainaboard-api-client-0.4.2/test/test_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_user.py` & `explainaboard-api-client-0.4.2/test/test_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
```

### Comparing `explainaboard-api-client-0.4.1/test/test_value.py` & `explainaboard-api-client-0.4.2/test/test_dataset_metadata.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """
     ExplainaBoard
 
     Backend APIs for ExplainaBoard  # noqa: E501
 
-    The version of the OpenAPI document: 0.4.1
+    The version of the OpenAPI document: 0.4.2
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import explainaboard_api_client
-from explainaboard_api_client.model.value import Value
+from explainaboard_api_client.model.dataset_metadata import DatasetMetadata
 
 
-class TestValue(unittest.TestCase):
-    """Value unit test stubs"""
+class TestDatasetMetadata(unittest.TestCase):
+    """DatasetMetadata unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testValue(self):
-        """Test Value"""
+    def testDatasetMetadata(self):
+        """Test DatasetMetadata"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = Value()  # noqa: E501
+        # model = DatasetMetadata()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

