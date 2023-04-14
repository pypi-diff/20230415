# Comparing `tmp/dkist-processing-common-2.4.1rc1.tar.gz` & `tmp/dkist-processing-common-2.4.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-common-2.4.1rc1.tar", last modified: Fri Apr 14 20:01:30 2023, max compression
+gzip compressed data, was "dkist-processing-common-2.4.1rc2.tar", last modified: Fri Apr 14 21:05:03 2023, max compression
```

## Comparing `dkist-processing-common-2.4.1rc1.tar` & `dkist-processing-common-2.4.1rc2.tar`

### file list

```diff
@@ -1,115 +1,116 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 20:01:30.581338 dkist-processing-common-2.4.1rc1/
--rw-rw-rw-   0 root         (0) root         (0)     2481 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    11805 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4327 2023-04-14 20:01:30.581338 dkist-processing-common-2.4.1rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3732 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2433 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 20:01:30.569337 dkist-processing-common-2.4.1rc1/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/changelog/128.misc.rst
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 20:01:30.569337 dkist-processing-common-2.4.1rc1/dkist_processing_common/
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 20:01:30.573337 dkist-processing-common-2.4.1rc1/dkist_processing_common/_util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1572 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/_util/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2409 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/_util/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/_util/dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     1580 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/_util/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     8215 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/_util/scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     5641 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/_util/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 20:01:30.573337 dkist-processing-common-2.4.1rc1/dkist_processing_common/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/fonts/Lato-Regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/fonts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6987 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/manual.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 20:01:30.573337 dkist-processing-common-2.4.1rc1/dkist_processing_common/models/
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4769 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     3304 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/models/fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     4192 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/models/flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/models/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     1096 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/models/json_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)     1109 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)     3408 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2225 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/models/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     7365 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/models/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 20:01:30.573337 dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6264 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1827 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/dsps_repeat.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/experiment_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1767 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     2451 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/proposal_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/single_value_single_key_flower.py
--rw-rw-rw-   0 root         (0) root         (0)     5598 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1669 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/unique_bud.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 20:01:30.577338 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11470 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     8152 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/base.py
--rw-rw-rw-   0 root         (0) root         (0)    10675 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/l1_output_data.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 20:01:30.577338 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2459 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/fits.py
--rw-rw-rw-   0 root         (0) root         (0)     6718 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/globus.py
--rw-rw-rw-   0 root         (0) root         (0)     6813 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     2421 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/interservice_bus.py
--rw-rw-rw-   0 root         (0) root         (0)    13155 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/metadata_store.py
--rw-rw-rw-   0 root         (0) root         (0)     3612 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/object_store.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 20:01:30.577338 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/quality/
--rw-rw-rw-   0 root         (0) root         (0)      383 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/quality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8226 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/quality/_base.py
--rw-rw-rw-   0 root         (0) root         (0)    47886 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/quality/_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     7123 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     8859 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     1374 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     4863 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)    18801 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 20:01:30.581338 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24490 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3023 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     1587 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     4203 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2291 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     8808 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     9758 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_fits_flowers.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)    19450 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_l1_output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6276 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    10499 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_publish_catalog_messages.py
--rw-rw-rw-   0 root         (0) root         (0)     9168 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    36040 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_quality_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    11282 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     4569 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     5745 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     6666 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2270 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_transfer_l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    11128 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_workflow_task_base.py
--rw-rw-rw-   0 root         (0) root         (0)    14982 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 20:01:30.569337 dkist-processing-common-2.4.1rc1/dkist_processing_common.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4327 2023-04-14 20:01:30.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4166 2023-04-14 20:01:30.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-14 20:01:30.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      603 2023-04-14 20:01:30.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-04-14 20:01:30.000000 dkist-processing-common-2.4.1rc1/dkist_processing_common.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 20:01:30.581338 dkist-processing-common-2.4.1rc1/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1890 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/docs/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 20:01:30.581338 dkist-processing-common-2.4.1rc1/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1690 2023-04-14 20:01:30.581338 dkist-processing-common-2.4.1rc1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-04-14 20:01:24.000000 dkist-processing-common-2.4.1rc1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 21:05:03.839607 dkist-processing-common-2.4.1rc2/
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    11805 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-04-14 21:05:03.839607 dkist-processing-common-2.4.1rc2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3732 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2433 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 21:05:03.827607 dkist-processing-common-2.4.1rc2/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/changelog/128.misc.rst
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 21:05:03.827607 dkist-processing-common-2.4.1rc2/dkist_processing_common/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 21:05:03.827607 dkist-processing-common-2.4.1rc2/dkist_processing_common/_util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/_util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1572 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/_util/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2409 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/_util/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/_util/dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/_util/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     8215 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/_util/scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     5641 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/_util/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 21:05:03.827607 dkist-processing-common-2.4.1rc2/dkist_processing_common/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/fonts/Lato-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/fonts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6987 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/manual.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 21:05:03.831606 dkist-processing-common-2.4.1rc2/dkist_processing_common/models/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4769 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     3304 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/models/fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     4192 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/models/flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/models/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/models/json_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     3408 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2225 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/models/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     7365 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/models/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/models/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 21:05:03.831606 dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6264 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/dsps_repeat.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/experiment_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1767 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     2451 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/proposal_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/single_value_single_key_flower.py
+-rw-rw-rw-   0 root         (0) root         (0)     5598 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/unique_bud.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 21:05:03.831606 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11470 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     8152 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    10675 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/l1_output_data.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 21:05:03.835606 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2459 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)     6718 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/globus.py
+-rw-rw-rw-   0 root         (0) root         (0)     6813 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2421 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/interservice_bus.py
+-rw-rw-rw-   0 root         (0) root         (0)    13155 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/metadata_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     3612 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/object_store.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 21:05:03.835606 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/quality/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/quality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8226 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/quality/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    47886 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/quality/_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     7123 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     8859 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     1374 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     4863 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    18355 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 21:05:03.835606 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24490 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3023 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4203 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     8808 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     9758 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_fits_flowers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)    19450 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_l1_output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6276 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    10499 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_publish_catalog_messages.py
+-rw-rw-rw-   0 root         (0) root         (0)     9168 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    36040 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_quality_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    11282 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     4569 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     5745 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     6666 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2270 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_transfer_l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    11128 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_workflow_task_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    14982 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 21:05:03.827607 dkist-processing-common-2.4.1rc2/dkist_processing_common.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-04-14 21:05:03.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4211 2023-04-14 21:05:03.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-14 21:05:03.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      603 2023-04-14 21:05:03.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-04-14 21:05:03.000000 dkist-processing-common-2.4.1rc2/dkist_processing_common.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 21:05:03.839607 dkist-processing-common-2.4.1rc2/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/docs/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-14 21:05:03.839607 dkist-processing-common-2.4.1rc2/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2023-04-14 21:05:03.839607 dkist-processing-common-2.4.1rc2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-04-14 21:04:55.000000 dkist-processing-common-2.4.1rc2/setup.py
```

### Comparing `dkist-processing-common-2.4.1rc1/.gitignore` & `dkist-processing-common-2.4.1rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/.pre-commit-config.yaml` & `dkist-processing-common-2.4.1rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/CHANGELOG.rst` & `dkist-processing-common-2.4.1rc2/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/PKG-INFO` & `dkist-processing-common-2.4.1rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 2.4.1rc1
+Version: 2.4.1rc2
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-2.4.1rc1/README.rst` & `dkist-processing-common-2.4.1rc2/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/bitbucket-pipelines.yml` & `dkist-processing-common-2.4.1rc2/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/check_changelog_updated.sh` & `dkist-processing-common-2.4.1rc2/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/_util/config.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/_util/config.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/_util/constants.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/_util/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/_util/dkist_location.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/_util/dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/_util/graphql.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/_util/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/_util/scratch.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/_util/scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/_util/tags.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/_util/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/fonts/Lato-Regular.ttf` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/manual.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/manual.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/models/constants.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/models/fits_access.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/models/fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/models/flower_pot.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/models/flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/models/graphql.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/models/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/models/json_encoder.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/models/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/models/message.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/models/message.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/models/parameters.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/models/quality.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/models/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/models/tags.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/cs_step.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/dsps_repeat.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/dsps_repeat.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/experiment_id_bud.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/experiment_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/id_bud.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/l0_fits_access.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/l1_fits_access.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/proposal_id_bud.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/proposal_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/quality.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/single_value_single_key_flower.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/single_value_single_key_flower.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/time.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/parsers/unique_bud.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/parsers/unique_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/assemble_movie.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/base.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/l1_output_data.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/fits.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/globus.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/globus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/input_dataset.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/interservice_bus.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/interservice_bus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/metadata_store.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/metadata_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/object_store.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/object_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/quality/_base.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/quality/_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/mixin/quality/_metrics.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/mixin/quality/_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/parse_l0_input_data.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/quality_metrics.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/teardown.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/transfer_input_data.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tasks/write_l1.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tasks/write_l1.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,50 +15,32 @@
 from dkist_fits_specifications import __version__ as spec_version
 from dkist_fits_specifications.utils.formatter import reformat_spec214_header
 from dkist_header_validator import spec214_validator
 from dkist_header_validator.translator import remove_extra_axis_keys
 from dkist_header_validator.translator import sanitize_to_spec214_level1
 from dkist_spectral_lines.search import get_closest_spectral_line
 from dkist_spectral_lines.search import get_spectral_lines
-from pydantic import BaseModel
-from pydantic import validator
 from scipy.stats import kurtosis
 from scipy.stats import skew
 from sunpy.coordinates import HeliocentricInertial
 
 from dkist_processing_common._util.dkist_location import location_of_dkist
 from dkist_processing_common.models.tags import Tag
+from dkist_processing_common.models.wavelength import WavelengthRange
 from dkist_processing_common.parsers.l0_fits_access import L0FitsAccess
 from dkist_processing_common.tasks import WorkflowTaskBase
 
 logger = logging.getLogger(__name__)
 
-__all__ = ["WriteL1Frame", "WavelengthRange"]
+__all__ = ["WriteL1Frame"]
 
 from dkist_processing_common.tasks.mixin.fits import FitsDataMixin
 from dkist_processing_common.tasks.mixin.metadata_store import MetadataStoreMixin
 
 
-class WavelengthRange(BaseModel):
-    """Model for holding the range of wavelengths assigned to a frame."""
-
-    min: u.Quantity
-    max: u.Quantity
-
-    @validator("min", "max")
-    def convert_to_nanometers(cls, v):
-        """Validate wavelength unit is for distance and convert to nanometers."""
-        return v.to(u.nm)
-
-    class Config:
-        """pydantic.BaseModel configuration."""
-
-        arbitrary_types_allowed = True
-
-
 class WriteL1Frame(WorkflowTaskBase, FitsDataMixin, MetadataStoreMixin, ABC):
     """
     Task to convert final calibrated science frames into spec 214 compliant level 1 frames.
 
     It is intended to be subclassed as the dataset header table is instrument specific.
     """
```

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/conftest.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_assemble_movie.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_base.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_constants.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_cs_step.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_dkist_location.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_fits_access.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_fits_flowers.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_fits_flowers.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_flower_pot.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_input_dataset.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_l1_output_data_base.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_l1_output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_parameters.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_parse_l0_input_data.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_publish_catalog_messages.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_publish_catalog_messages.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_quality.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_quality_mixin.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_quality_mixin.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_scratch.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_tags.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_teardown.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_transfer_input_data.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_transfer_l1_output_data.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_transfer_l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_workflow_task_base.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_workflow_task_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common/tests/test_write_l1.py` & `dkist-processing-common-2.4.1rc2/dkist_processing_common/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common.egg-info/PKG-INFO` & `dkist-processing-common-2.4.1rc2/dkist_processing_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 2.4.1rc1
+Version: 2.4.1rc2
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common.egg-info/SOURCES.txt` & `dkist-processing-common-2.4.1rc2/dkist_processing_common.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 dkist_processing_common/models/flower_pot.py
 dkist_processing_common/models/graphql.py
 dkist_processing_common/models/json_encoder.py
 dkist_processing_common/models/message.py
 dkist_processing_common/models/parameters.py
 dkist_processing_common/models/quality.py
 dkist_processing_common/models/tags.py
+dkist_processing_common/models/wavelength.py
 dkist_processing_common/parsers/__init__.py
 dkist_processing_common/parsers/cs_step.py
 dkist_processing_common/parsers/dsps_repeat.py
 dkist_processing_common/parsers/experiment_id_bud.py
 dkist_processing_common/parsers/id_bud.py
 dkist_processing_common/parsers/l0_fits_access.py
 dkist_processing_common/parsers/l1_fits_access.py
```

### Comparing `dkist-processing-common-2.4.1rc1/dkist_processing_common.egg-info/requires.txt` & `dkist-processing-common-2.4.1rc2/dkist_processing_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/docs/Makefile` & `dkist-processing-common-2.4.1rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/docs/conf.py` & `dkist-processing-common-2.4.1rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/docs/make.bat` & `dkist-processing-common-2.4.1rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/licenses/LICENSE.rst` & `dkist-processing-common-2.4.1rc2/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/pyproject.toml` & `dkist-processing-common-2.4.1rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-2.4.1rc1/setup.cfg` & `dkist-processing-common-2.4.1rc2/setup.cfg`

 * *Files identical despite different names*

