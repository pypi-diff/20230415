# Comparing `tmp/tavern-2.0.6.tar.gz` & `tmp/tavern-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tavern-2.0.6.tar", last modified: Mon Mar 13 11:49:26 2023, max compression
+gzip compressed data, was "tavern-2.0.7.tar", last modified: Sat Apr 15 15:36:11 2023, max compression
```

## Comparing `tavern-2.0.6.tar` & `tavern-2.0.7.tar`

### file list

```diff
@@ -1,188 +1,188 @@
--rw-r--r--   0        0        0     1271 2023-02-21 15:50:54.811198 tavern-2.0.6/.dockerignore
--rw-r--r--   0        0        0     2217 2023-02-21 15:50:54.811198 tavern-2.0.6/.github/workflows/main.yml
--rw-r--r--   0        0        0     1291 2023-02-21 15:50:54.811198 tavern-2.0.6/.gitignore
--rw-r--r--   0        0        0      434 2023-02-21 15:50:54.811198 tavern-2.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0       43 2023-02-21 15:50:54.811198 tavern-2.0.6/.prettierignore
--rw-r--r--   0        0        0    16043 2023-03-13 11:49:19.115698 tavern-2.0.6/CHANGELOG.md
--rw-r--r--   0        0        0     1677 2023-02-21 15:50:54.811198 tavern-2.0.6/CONTRIBUTING.md
--rw-r--r--   0        0        0     1055 2023-02-21 15:50:54.811198 tavern-2.0.6/LICENSE
--rw-r--r--   0        0        0      111 2023-02-28 14:53:18.079807 tavern-2.0.6/MANIFEST.in
--rw-r--r--   0        0        0     8342 2023-02-21 15:50:54.811198 tavern-2.0.6/README.md
--rw-r--r--   0        0        0     5765 2023-02-28 14:53:18.079807 tavern-2.0.6/constraints.txt
--rw-r--r--   0        0        0        9 2019-12-13 13:22:50.199802 tavern-2.0.6/docs/.gitignore
--rw-r--r--   0        0        0      607 2020-04-05 16:12:15.549603 tavern-2.0.6/docs/Makefile
--rw-r--r--   0        0        0        6 2019-12-13 13:22:50.199802 tavern-2.0.6/docs/source/.gitignore
--rw-r--r--   0        0        0      851 2020-04-05 16:12:15.549603 tavern-2.0.6/docs/source/_static/favicon.png
--rw-r--r--   0        0        0     1448 2020-04-05 16:12:15.549603 tavern-2.0.6/docs/source/_static/icon.png
--rw-r--r--   0        0        0    67428 2023-02-21 15:50:54.811198 tavern-2.0.6/docs/source/basics.md
--rw-r--r--   0        0        0     5825 2023-03-13 11:49:18.025699 tavern-2.0.6/docs/source/conf.py
--rw-r--r--   0        0        0     4200 2023-02-21 15:50:54.811198 tavern-2.0.6/docs/source/cookbook.md
--rw-r--r--   0        0        0     7667 2023-02-21 15:50:54.811198 tavern-2.0.6/docs/source/debugging.md
--rw-r--r--   0        0        0     7883 2023-02-21 15:50:54.814531 tavern-2.0.6/docs/source/examples.md
--rw-r--r--   0        0        0    12310 2023-02-21 15:50:54.814531 tavern-2.0.6/docs/source/http.md
--rw-r--r--   0        0        0     1494 2023-02-21 15:50:54.814531 tavern-2.0.6/docs/source/index.md
--rw-r--r--   0        0        0     9433 2023-02-21 15:50:54.814531 tavern-2.0.6/docs/source/mqtt.md
--rw-r--r--   0        0        0    11359 2023-02-21 15:50:54.814531 tavern-2.0.6/docs/source/plugins.md
--rw-r--r--   0        0        0      130 2023-02-21 15:50:54.814531 tavern-2.0.6/docs/source/requirements.txt
--rw-r--r--   0        0        0     2895 2020-04-05 16:12:15.552937 tavern-2.0.6/docs/source/server.md
--rw-r--r--   0        0        0      213 2023-02-21 15:50:54.814531 tavern-2.0.6/example/advanced/Dockerfile
--rw-r--r--   0        0        0      401 2021-09-25 13:51:36.584969 tavern-2.0.6/example/advanced/advanced.md
--rw-r--r--   0        0        0      149 2021-09-25 13:51:36.584969 tavern-2.0.6/example/advanced/common.yaml
--rw-r--r--   0        0        0      126 2023-01-27 12:05:17.735245 tavern-2.0.6/example/advanced/docker-compose.yaml
--rw-r--r--   0        0        0     3552 2023-02-21 15:50:54.814531 tavern-2.0.6/example/advanced/server.py
--rw-r--r--   0        0        0     4046 2023-02-21 15:50:54.814531 tavern-2.0.6/example/advanced/test_server.tavern.yaml
--rw-r--r--   0        0        0      673 2023-02-21 15:50:54.814531 tavern-2.0.6/example/advanced/testing_utils.py
--rw-r--r--   0        0        0      210 2023-02-21 15:50:54.814531 tavern-2.0.6/example/components/Dockerfile
--rw-r--r--   0        0        0      168 2021-09-25 13:51:36.584969 tavern-2.0.6/example/components/common.yaml
--rw-r--r--   0        0        0      717 2021-09-25 13:51:36.584969 tavern-2.0.6/example/components/components.md
--rw-r--r--   0        0        0      594 2021-09-25 13:51:36.584969 tavern-2.0.6/example/components/components/auth_stage.yaml
--rw-r--r--   0        0        0      126 2023-01-27 12:05:17.735245 tavern-2.0.6/example/components/docker-compose.yaml
--rw-r--r--   0        0        0     1642 2023-02-21 15:50:54.814531 tavern-2.0.6/example/components/server.py
--rw-r--r--   0        0        0      633 2021-09-25 13:51:36.584969 tavern-2.0.6/example/components/test_hello.tavern.yaml
--rw-r--r--   0        0        0      612 2021-09-25 13:51:36.584969 tavern-2.0.6/example/components/test_ping.tavern.yaml
--rw-r--r--   0        0        0      195 2023-02-21 15:50:54.814531 tavern-2.0.6/example/cookies/Dockerfile
--rw-r--r--   0        0        0      117 2021-09-25 13:51:36.584969 tavern-2.0.6/example/cookies/common.yaml
--rw-r--r--   0        0        0      147 2021-09-25 13:51:36.584969 tavern-2.0.6/example/cookies/cookies.md
--rw-r--r--   0        0        0      126 2023-01-27 12:05:17.735245 tavern-2.0.6/example/cookies/docker-compose.yaml
--rw-r--r--   0        0        0     2964 2023-02-21 15:50:54.814531 tavern-2.0.6/example/cookies/server.py
--rw-r--r--   0        0        0     3245 2021-09-25 13:51:36.584969 tavern-2.0.6/example/cookies/test_server.tavern.yaml
--rw-r--r--   0        0        0      202 2020-04-05 16:12:15.552937 tavern-2.0.6/example/generate_from_openapi/Pipfile
--rw-r--r--   0        0        0    13687 2023-02-21 15:50:54.814531 tavern-2.0.6/example/generate_from_openapi/Pipfile.lock
--rw-r--r--   0        0        0     2101 2022-08-06 15:34:31.364607 tavern-2.0.6/example/generate_from_openapi/pub_tavern.py
--rw-r--r--   0        0        0      144 2020-04-05 16:12:15.552937 tavern-2.0.6/example/generate_from_openapi/readme.md
--rw-r--r--   0        0        0      566 2020-04-05 16:12:15.552937 tavern-2.0.6/example/generate_from_openapi/test_example_output.tavern.yaml
--rw-r--r--   0        0        0      195 2023-02-21 15:50:54.814531 tavern-2.0.6/example/hooks/Dockerfile
--rw-r--r--   0        0        0      990 2022-08-06 15:34:31.364607 tavern-2.0.6/example/hooks/conftest.py
--rw-r--r--   0        0        0      126 2023-02-21 15:50:54.814531 tavern-2.0.6/example/hooks/docker-compose.yaml
--rw-r--r--   0        0        0      465 2023-01-27 12:05:17.735245 tavern-2.0.6/example/hooks/server.py
--rw-r--r--   0        0        0      620 2023-02-21 15:50:54.814531 tavern-2.0.6/example/hooks/test_server.tavern.yaml
--rw-r--r--   0        0        0      844 2020-04-05 16:12:15.556270 tavern-2.0.6/example/mqtt/README.md
--rw-r--r--   0        0        0      158 2020-04-05 16:12:15.556270 tavern-2.0.6/example/mqtt/common.yaml
--rw-r--r--   0        0        0     2600 2023-02-21 15:50:54.814531 tavern-2.0.6/example/mqtt/conftest.py
--rw-r--r--   0        0        0      984 2023-03-13 11:47:58.622373 tavern-2.0.6/example/mqtt/docker-compose.yaml
--rw-r--r--   0        0        0      135 2020-04-05 16:12:15.556270 tavern-2.0.6/example/mqtt/fluent.conf
--rw-r--r--   0        0        0      158 2023-02-21 15:50:54.814531 tavern-2.0.6/example/mqtt/listener.Dockerfile
--rw-r--r--   0        0        0     4826 2023-03-13 11:47:58.625706 tavern-2.0.6/example/mqtt/listener.py
--rw-r--r--   0        0        0      169 2023-03-13 11:47:58.625706 tavern-2.0.6/example/mqtt/mosquitto.conf
--rw-r--r--   0        0        0      120 2023-03-13 11:47:58.625706 tavern-2.0.6/example/mqtt/mosquitto_passwd
--rw-r--r--   0        0        0      393 2023-02-21 15:50:54.814531 tavern-2.0.6/example/mqtt/server.Dockerfile
--rw-r--r--   0        0        0     4466 2023-03-13 11:47:58.625706 tavern-2.0.6/example/mqtt/server.py
--rw-r--r--   0        0        0    15145 2023-03-13 11:47:58.625706 tavern-2.0.6/example/mqtt/test_mqtt.tavern.yaml
--rw-r--r--   0        0        0     3316 2023-03-13 11:47:58.625706 tavern-2.0.6/example/mqtt/test_mqtt_failures.tavern.yaml
--rw-r--r--   0        0        0      193 2023-02-21 15:50:54.814531 tavern-2.0.6/example/mqtt/testing_utils.py
--rw-r--r--   0        0        0     1167 2021-09-25 13:51:36.584969 tavern-2.0.6/example/simple/running_tests.md
--rw-r--r--   0        0        0      465 2023-01-27 12:05:17.735245 tavern-2.0.6/example/simple/server.py
--rw-r--r--   0        0        0     1996 2021-09-25 13:51:36.584969 tavern-2.0.6/example/simple/test_server.tavern.yaml
--rw-r--r--   0        0        0     4036 2023-03-13 11:49:18.025699 tavern-2.0.6/pyproject.toml
--rw-r--r--   0        0        0    57130 2023-02-28 14:53:18.079807 tavern-2.0.6/requirements.txt
--rwxr-xr-x   0        0        0      222 2023-02-21 15:50:54.814531 tavern-2.0.6/scripts/coverage.sh
--rwxr-xr-x   0        0        0      407 2023-02-21 15:50:54.814531 tavern-2.0.6/scripts/release.sh
--rwxr-xr-x   0        0        0      374 2023-02-28 14:53:18.079807 tavern-2.0.6/scripts/smoke.bash
--rwxr-xr-x   0        0        0      616 2023-02-21 15:50:54.814531 tavern-2.0.6/scripts/update-changelog.bash
--rw-r--r--   0        0        0       99 2023-03-13 11:49:18.025699 tavern-2.0.6/tavern/__init__.py
--rw-r--r--   0        0        0        0 2023-02-21 16:06:58.930000 tavern-2.0.6/tavern/_core/__init__.py
--rw-r--r--   0        0        0    19780 2023-02-21 15:50:54.814531 tavern-2.0.6/tavern/_core/dict_util.py
--rw-r--r--   0        0        0     3842 2023-02-28 14:53:18.079807 tavern-2.0.6/tavern/_core/exceptions.py
--rw-r--r--   0        0        0     4737 2023-02-21 15:50:54.814531 tavern-2.0.6/tavern/_core/extfunctions.py
--rw-r--r--   0        0        0       96 2023-02-21 15:50:54.814531 tavern-2.0.6/tavern/_core/formatted_str.py
--rw-r--r--   0        0        0      951 2023-02-21 15:50:54.814531 tavern-2.0.6/tavern/_core/general.py
--rw-r--r--   0        0        0     2612 2023-02-21 15:50:54.814531 tavern-2.0.6/tavern/_core/jmesutils.py
--rw-r--r--   0        0        0    12257 2023-02-21 15:50:54.814531 tavern-2.0.6/tavern/_core/loader.py
--rw-r--r--   0        0        0     9200 2023-02-28 14:53:18.079807 tavern-2.0.6/tavern/_core/plugins.py
--rw-r--r--   0        0        0      275 2023-02-21 15:50:54.814531 tavern-2.0.6/tavern/_core/pytest/__init__.py
--rw-r--r--   0        0        0     1617 2023-02-21 15:50:54.814531 tavern-2.0.6/tavern/_core/pytest/config.py
--rw-r--r--   0        0        0     7393 2023-03-13 11:47:58.625706 tavern-2.0.6/tavern/_core/pytest/error.py
--rw-r--r--   0        0        0    13187 2023-02-21 16:10:45.238832 tavern-2.0.6/tavern/_core/pytest/file.py
--rw-r--r--   0        0        0     1471 2023-02-21 16:10:45.238832 tavern-2.0.6/tavern/_core/pytest/hooks.py
--rw-r--r--   0        0        0     9469 2023-02-21 16:10:45.238832 tavern-2.0.6/tavern/_core/pytest/item.py
--rw-r--r--   0        0        0     2101 2023-02-21 15:50:54.814531 tavern-2.0.6/tavern/_core/pytest/newhooks.py
--rw-r--r--   0        0        0     5941 2023-02-28 14:53:18.079807 tavern-2.0.6/tavern/_core/pytest/util.py
--rw-r--r--   0        0        0     1833 2023-02-21 15:50:54.814531 tavern-2.0.6/tavern/_core/report.py
--rw-r--r--   0        0        0    10800 2023-02-21 15:50:54.814531 tavern-2.0.6/tavern/_core/run.py
--rw-r--r--   0        0        0        0 2023-02-21 16:06:58.930081 tavern-2.0.6/tavern/_core/schema/__init__.py
--rw-r--r--   0        0        0    14523 2023-02-28 14:53:18.079807 tavern-2.0.6/tavern/_core/schema/extensions.py
--rw-r--r--   0        0        0     4350 2023-02-21 15:50:54.814531 tavern-2.0.6/tavern/_core/schema/files.py
--rw-r--r--   0        0        0     6245 2023-03-13 11:47:55.152372 tavern-2.0.6/tavern/_core/schema/jsonschema.py
--rw-r--r--   0        0        0     9057 2023-02-21 15:50:54.817865 tavern-2.0.6/tavern/_core/schema/tests.jsonschema.yaml
--rw-r--r--   0        0        0     6845 2023-02-28 14:53:18.079807 tavern-2.0.6/tavern/_core/schema/tests.schema.yaml
--rw-r--r--   0        0        0     1100 2023-02-21 15:50:54.817865 tavern-2.0.6/tavern/_core/stage_lines.py
--rw-r--r--   0        0        0     5171 2023-02-21 15:50:54.817865 tavern-2.0.6/tavern/_core/strict_util.py
--rw-r--r--   0        0        0      383 2023-02-21 15:50:54.817865 tavern-2.0.6/tavern/_core/strtobool.py
--rw-r--r--   0        0        0     3958 2023-02-21 15:50:54.817865 tavern-2.0.6/tavern/_core/testhelpers.py
--rw-r--r--   0        0        0        0 2023-02-21 16:06:58.930000 tavern-2.0.6/tavern/_plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-02-21 16:06:58.930000 tavern-2.0.6/tavern/_plugins/mqtt/__init__.py
--rw-r--r--   0        0        0    17697 2023-03-13 11:47:58.625706 tavern-2.0.6/tavern/_plugins/mqtt/client.py
--rw-r--r--   0        0        0     4013 2023-02-21 15:50:54.817865 tavern-2.0.6/tavern/_plugins/mqtt/jsonschema.yaml
--rw-r--r--   0        0        0     2523 2023-02-21 15:50:54.817865 tavern-2.0.6/tavern/_plugins/mqtt/request.py
--rw-r--r--   0        0        0    11363 2023-02-21 15:50:54.817865 tavern-2.0.6/tavern/_plugins/mqtt/response.py
--rw-r--r--   0        0        0     3233 2023-02-21 15:50:54.817865 tavern-2.0.6/tavern/_plugins/mqtt/schema.yaml
--rw-r--r--   0        0        0     1267 2023-02-21 15:50:54.817865 tavern-2.0.6/tavern/_plugins/mqtt/tavernhook.py
--rw-r--r--   0        0        0        0 2023-02-21 16:06:58.930000 tavern-2.0.6/tavern/_plugins/rest/__init__.py
--rw-r--r--   0        0        0    19370 2023-02-21 15:50:54.817865 tavern-2.0.6/tavern/_plugins/rest/request.py
--rw-r--r--   0        0        0     8291 2023-02-21 15:50:54.817865 tavern-2.0.6/tavern/_plugins/rest/response.py
--rw-r--r--   0        0        0      860 2023-02-21 15:50:54.817865 tavern-2.0.6/tavern/_plugins/rest/tavernhook.py
--rw-r--r--   0        0        0     2969 2023-02-28 14:53:18.079807 tavern-2.0.6/tavern/core.py
--rw-r--r--   0        0        0     2739 2023-02-21 15:50:54.817865 tavern-2.0.6/tavern/entry.py
--rw-r--r--   0        0        0     7575 2023-02-21 15:50:54.817865 tavern-2.0.6/tavern/helpers.py
--rw-r--r--   0        0        0      466 2023-02-21 15:50:54.817865 tavern-2.0.6/tavern/request.py
--rw-r--r--   0        0        0     9571 2023-02-21 15:50:54.817865 tavern-2.0.6/tavern/response.py
--rw-r--r--   0        0        0      919 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/conftest.py
--rw-r--r--   0        0        0      195 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/Dockerfile
--rw-r--r--   0        0        0       33 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/OK.json.gz
--rw-r--r--   0        0        0        3 2020-12-19 13:25:29.031794 tavern-2.0.6/tests/integration/OK.txt
--rw-r--r--   0        0        0      504 2021-09-25 13:51:36.591636 tavern-2.0.6/tests/integration/README.md
--rw-r--r--   0        0        0      608 2022-02-25 15:36:43.966205 tavern-2.0.6/tests/integration/common.yaml
--rw-r--r--   0        0        0      621 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/conftest.py
--rw-r--r--   0        0        0      126 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/docker-compose.yaml
--rw-r--r--   0        0        0      167 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/ext_functions.py
--rw-r--r--   0        0        0      203 2020-04-05 16:12:15.572937 tavern-2.0.6/tests/integration/extra.yaml
--rw-r--r--   0        0        0      254 2021-05-01 10:23:38.259754 tavern-2.0.6/tests/integration/global_cfg.yaml
--rw-r--r--   0        0        0       91 2021-03-07 14:36:40.846310 tavern-2.0.6/tests/integration/parametrize_includes.yaml
--rw-r--r--   0        0        0    11475 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/server.py
--rw-r--r--   0        0        0      297 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/test_allure.tavern.yaml
--rw-r--r--   0        0        0      659 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/test_auth_key.tavern.yaml
--rw-r--r--   0        0        0      624 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/test_certs.tavern.yaml
--rw-r--r--   0        0        0     1569 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/test_cookie_remember.tavern.yaml
--rw-r--r--   0        0        0     6106 2021-12-20 17:04:04.340877 tavern-2.0.6/tests/integration/test_cookies.tavern.yaml
--rw-r--r--   0        0        0     2448 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/test_data_key.tavern.yaml
--rw-r--r--   0        0        0       29 2022-08-06 15:34:18.544082 tavern-2.0.6/tests/integration/test_dummy.py
--rw-r--r--   0        0        0      331 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/test_env_var_format.tavern.yaml
--rw-r--r--   0        0        0      277 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/test_error.tavern.yaml
--rw-r--r--   0        0        0     3152 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/test_external_functions.tavern.yaml
--rw-r--r--   0        0        0     4086 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/test_files.tavern.yaml
--rw-r--r--   0        0        0     2398 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/test_fixtures.tavern.yaml
--rw-r--r--   0        0        0      799 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/test_follow_redirects.tavern.yaml
--rw-r--r--   0        0        0     1028 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/test_header_comparisons.tavern.yaml
--rw-r--r--   0        0        0     1269 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/test_helpers.tavern.yaml
--rw-r--r--   0        0        0     4837 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/test_jmes.tavern.yaml
--rw-r--r--   0        0        0      750 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/test_minimal.tavern.yaml
--rw-r--r--   0        0        0    14838 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/test_parametrize.tavern.yaml
--rw-r--r--   0        0        0     2167 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/test_regex.tavern.yaml
--rw-r--r--   0        0        0     2031 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/test_response_types.tavern.yaml
--rw-r--r--   0        0        0     2372 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/test_retry.tavern.yaml
--rw-r--r--   0        0        0      575 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/test_save_dict_value.tavern.yaml
--rw-r--r--   0        0        0      970 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/test_selective_tests.tavern.yaml
--rw-r--r--   0        0        0     2432 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/test_skipped_tests.tavern.yaml
--rw-r--r--   0        0        0     1506 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/test_status_codes.tavern.yaml
--rw-r--r--   0        0        0      235 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/test_stream.tavern.yaml
--rw-r--r--   0        0        0    10926 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/test_strict_key_checks.tavern.yaml
--rw-r--r--   0        0        0     1951 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/test_timeout.tavern.yaml
--rw-r--r--   0        0        0    12933 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/test_typetokens.tavern.yaml
--rw-r--r--   0        0        0     1415 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/integration/test_validate_pykwalify.tavern.yaml
--rw-r--r--   0        0        0        0 2020-04-05 16:12:15.572937 tavern-2.0.6/tests/integration/testfile.txt
--rw-r--r--   0        0        0      650 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/logging.yaml
--rw-r--r--   0        0        0      915 2023-02-28 14:53:18.079807 tavern-2.0.6/tests/unit/conftest.py
--rw-r--r--   0        0        0     9612 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/unit/response/test_mqtt_response.py
--rw-r--r--   0        0        0    12296 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/unit/response/test_rest.py
--rw-r--r--   0        0        0     1483 2023-02-28 14:53:18.079807 tavern-2.0.6/tests/unit/test_call_run.py
--rw-r--r--   0        0        0    16186 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/unit/test_core.py
--rw-r--r--   0        0        0    14289 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/unit/test_helpers.py
--rw-r--r--   0        0        0     7161 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/unit/test_mqtt.py
--rw-r--r--   0        0        0     5791 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/unit/test_pytest_hooks.py
--rw-r--r--   0        0        0    14990 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/unit/test_request.py
--rw-r--r--   0        0        0     6131 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/unit/test_schema.py
--rw-r--r--   0        0        0     1030 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/unit/test_strict_util.py
--rw-r--r--   0        0        0    14898 2023-02-21 15:50:54.817865 tavern-2.0.6/tests/unit/test_utilities.py
--rw-r--r--   0        0        0     2434 2023-02-28 16:04:49.019403 tavern-2.0.6/tox-integration.ini
--rw-r--r--   0        0        0      625 2023-02-21 15:50:54.817865 tavern-2.0.6/tox.ini
--rw-r--r--   0        0        0    10615 1970-01-01 00:00:00.000000 tavern-2.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1271 2023-04-15 14:36:17.314374 tavern-2.0.7/.dockerignore
+-rw-r--r--   0        0        0     2217 2023-04-15 14:36:17.314374 tavern-2.0.7/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1291 2023-04-15 14:36:17.314374 tavern-2.0.7/.gitignore
+-rw-r--r--   0        0        0      434 2023-04-08 18:45:13.188074 tavern-2.0.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       43 2023-02-21 15:50:54.811198 tavern-2.0.7/.prettierignore
+-rw-r--r--   0        0        0    16105 2023-04-15 15:35:53.610178 tavern-2.0.7/CHANGELOG.md
+-rw-r--r--   0        0        0     1677 2023-04-08 18:45:13.188074 tavern-2.0.7/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1055 2023-02-21 15:50:54.811198 tavern-2.0.7/LICENSE
+-rw-r--r--   0        0        0      111 2023-04-15 14:36:17.314374 tavern-2.0.7/MANIFEST.in
+-rw-r--r--   0        0        0     8342 2023-02-21 15:50:54.811198 tavern-2.0.7/README.md
+-rw-r--r--   0        0        0     5800 2023-04-15 15:35:19.443117 tavern-2.0.7/constraints.txt
+-rw-r--r--   0        0        0        9 2019-12-13 13:22:50.199802 tavern-2.0.7/docs/.gitignore
+-rw-r--r--   0        0        0      607 2020-04-05 16:12:15.549603 tavern-2.0.7/docs/Makefile
+-rw-r--r--   0        0        0        6 2019-12-13 13:22:50.199802 tavern-2.0.7/docs/source/.gitignore
+-rw-r--r--   0        0        0      851 2020-04-05 16:12:15.549603 tavern-2.0.7/docs/source/_static/favicon.png
+-rw-r--r--   0        0        0     1448 2020-04-05 16:12:15.549603 tavern-2.0.7/docs/source/_static/icon.png
+-rw-r--r--   0        0        0    67428 2023-02-21 15:50:54.811198 tavern-2.0.7/docs/source/basics.md
+-rw-r--r--   0        0        0     5825 2023-04-15 15:35:52.443498 tavern-2.0.7/docs/source/conf.py
+-rw-r--r--   0        0        0     4200 2023-02-21 15:50:54.811198 tavern-2.0.7/docs/source/cookbook.md
+-rw-r--r--   0        0        0     7667 2023-02-21 15:50:54.811198 tavern-2.0.7/docs/source/debugging.md
+-rw-r--r--   0        0        0     7883 2023-02-21 15:50:54.814531 tavern-2.0.7/docs/source/examples.md
+-rw-r--r--   0        0        0    12310 2023-04-08 18:45:13.188074 tavern-2.0.7/docs/source/http.md
+-rw-r--r--   0        0        0     1494 2023-02-21 15:50:54.814531 tavern-2.0.7/docs/source/index.md
+-rw-r--r--   0        0        0     9433 2023-02-21 15:50:54.814531 tavern-2.0.7/docs/source/mqtt.md
+-rw-r--r--   0        0        0    11359 2023-02-21 15:50:54.814531 tavern-2.0.7/docs/source/plugins.md
+-rw-r--r--   0        0        0      130 2023-02-21 15:50:54.814531 tavern-2.0.7/docs/source/requirements.txt
+-rw-r--r--   0        0        0     2895 2020-04-05 16:12:15.552937 tavern-2.0.7/docs/source/server.md
+-rw-r--r--   0        0        0      213 2023-04-15 14:36:17.314374 tavern-2.0.7/example/advanced/Dockerfile
+-rw-r--r--   0        0        0      401 2021-09-25 13:51:36.584969 tavern-2.0.7/example/advanced/advanced.md
+-rw-r--r--   0        0        0      149 2021-09-25 13:51:36.584969 tavern-2.0.7/example/advanced/common.yaml
+-rw-r--r--   0        0        0      126 2023-04-15 14:36:17.314374 tavern-2.0.7/example/advanced/docker-compose.yaml
+-rw-r--r--   0        0        0     3552 2023-04-15 14:36:17.314374 tavern-2.0.7/example/advanced/server.py
+-rw-r--r--   0        0        0     4046 2023-02-21 15:50:54.814531 tavern-2.0.7/example/advanced/test_server.tavern.yaml
+-rw-r--r--   0        0        0      673 2023-02-21 15:50:54.814531 tavern-2.0.7/example/advanced/testing_utils.py
+-rw-r--r--   0        0        0      210 2023-04-15 14:36:17.314374 tavern-2.0.7/example/components/Dockerfile
+-rw-r--r--   0        0        0      168 2021-09-25 13:51:36.584969 tavern-2.0.7/example/components/common.yaml
+-rw-r--r--   0        0        0      717 2021-09-25 13:51:36.584969 tavern-2.0.7/example/components/components.md
+-rw-r--r--   0        0        0      594 2021-09-25 13:51:36.584969 tavern-2.0.7/example/components/components/auth_stage.yaml
+-rw-r--r--   0        0        0      126 2023-04-15 14:36:17.314374 tavern-2.0.7/example/components/docker-compose.yaml
+-rw-r--r--   0        0        0     1642 2023-04-15 14:36:17.314374 tavern-2.0.7/example/components/server.py
+-rw-r--r--   0        0        0      633 2021-09-25 13:51:36.584969 tavern-2.0.7/example/components/test_hello.tavern.yaml
+-rw-r--r--   0        0        0      612 2021-09-25 13:51:36.584969 tavern-2.0.7/example/components/test_ping.tavern.yaml
+-rw-r--r--   0        0        0      195 2023-04-15 14:36:17.314374 tavern-2.0.7/example/cookies/Dockerfile
+-rw-r--r--   0        0        0      117 2021-09-25 13:51:36.584969 tavern-2.0.7/example/cookies/common.yaml
+-rw-r--r--   0        0        0      147 2021-09-25 13:51:36.584969 tavern-2.0.7/example/cookies/cookies.md
+-rw-r--r--   0        0        0      126 2023-04-15 14:36:17.314374 tavern-2.0.7/example/cookies/docker-compose.yaml
+-rw-r--r--   0        0        0     2964 2023-04-15 14:36:17.314374 tavern-2.0.7/example/cookies/server.py
+-rw-r--r--   0        0        0     3245 2021-09-25 13:51:36.584969 tavern-2.0.7/example/cookies/test_server.tavern.yaml
+-rw-r--r--   0        0        0      202 2020-04-05 16:12:15.552937 tavern-2.0.7/example/generate_from_openapi/Pipfile
+-rw-r--r--   0        0        0    13687 2023-02-21 15:50:54.814531 tavern-2.0.7/example/generate_from_openapi/Pipfile.lock
+-rw-r--r--   0        0        0     2101 2022-08-06 15:34:31.364607 tavern-2.0.7/example/generate_from_openapi/pub_tavern.py
+-rw-r--r--   0        0        0      144 2020-04-05 16:12:15.552937 tavern-2.0.7/example/generate_from_openapi/readme.md
+-rw-r--r--   0        0        0      566 2020-04-05 16:12:15.552937 tavern-2.0.7/example/generate_from_openapi/test_example_output.tavern.yaml
+-rw-r--r--   0        0        0      195 2023-04-15 14:36:17.314374 tavern-2.0.7/example/hooks/Dockerfile
+-rw-r--r--   0        0        0      990 2022-08-06 15:34:31.364607 tavern-2.0.7/example/hooks/conftest.py
+-rw-r--r--   0        0        0      126 2023-04-15 14:36:17.314374 tavern-2.0.7/example/hooks/docker-compose.yaml
+-rw-r--r--   0        0        0      465 2023-04-15 14:36:17.314374 tavern-2.0.7/example/hooks/server.py
+-rw-r--r--   0        0        0      620 2023-02-21 15:50:54.814531 tavern-2.0.7/example/hooks/test_server.tavern.yaml
+-rw-r--r--   0        0        0      844 2020-04-05 16:12:15.556270 tavern-2.0.7/example/mqtt/README.md
+-rw-r--r--   0        0        0      158 2020-04-05 16:12:15.556270 tavern-2.0.7/example/mqtt/common.yaml
+-rw-r--r--   0        0        0     2600 2023-04-08 18:45:13.188074 tavern-2.0.7/example/mqtt/conftest.py
+-rw-r--r--   0        0        0      984 2023-04-15 14:36:17.314374 tavern-2.0.7/example/mqtt/docker-compose.yaml
+-rw-r--r--   0        0        0      135 2020-04-05 16:12:15.556270 tavern-2.0.7/example/mqtt/fluent.conf
+-rw-r--r--   0        0        0      158 2023-04-15 14:36:17.314374 tavern-2.0.7/example/mqtt/listener.Dockerfile
+-rw-r--r--   0        0        0     4863 2023-04-15 15:04:25.003592 tavern-2.0.7/example/mqtt/listener.py
+-rw-r--r--   0        0        0      169 2023-04-08 18:45:13.188074 tavern-2.0.7/example/mqtt/mosquitto.conf
+-rw-r--r--   0        0        0      120 2023-04-08 18:45:13.188074 tavern-2.0.7/example/mqtt/mosquitto_passwd
+-rw-r--r--   0        0        0      393 2023-04-15 14:36:17.314374 tavern-2.0.7/example/mqtt/server.Dockerfile
+-rw-r--r--   0        0        0     4707 2023-04-15 15:04:25.003592 tavern-2.0.7/example/mqtt/server.py
+-rw-r--r--   0        0        0    15165 2023-04-15 15:04:25.003592 tavern-2.0.7/example/mqtt/test_mqtt.tavern.yaml
+-rw-r--r--   0        0        0     3381 2023-04-15 15:04:25.003592 tavern-2.0.7/example/mqtt/test_mqtt_failures.tavern.yaml
+-rw-r--r--   0        0        0      193 2023-04-08 18:45:13.188074 tavern-2.0.7/example/mqtt/testing_utils.py
+-rw-r--r--   0        0        0     1167 2021-09-25 13:51:36.584969 tavern-2.0.7/example/simple/running_tests.md
+-rw-r--r--   0        0        0      465 2023-04-15 14:36:17.314374 tavern-2.0.7/example/simple/server.py
+-rw-r--r--   0        0        0     1996 2021-09-25 13:51:36.584969 tavern-2.0.7/example/simple/test_server.tavern.yaml
+-rw-r--r--   0        0        0     4038 2023-04-15 15:35:52.443498 tavern-2.0.7/pyproject.toml
+-rw-r--r--   0        0        0    57165 2023-04-15 15:35:19.443117 tavern-2.0.7/requirements.txt
+-rwxr-xr-x   0        0        0      222 2023-02-21 15:50:54.814531 tavern-2.0.7/scripts/coverage.sh
+-rwxr-xr-x   0        0        0      407 2023-02-21 15:50:54.814531 tavern-2.0.7/scripts/release.sh
+-rwxr-xr-x   0        0        0      374 2023-04-08 18:45:13.188074 tavern-2.0.7/scripts/smoke.bash
+-rwxr-xr-x   0        0        0      616 2023-02-21 15:50:54.814531 tavern-2.0.7/scripts/update-changelog.bash
+-rw-r--r--   0        0        0       99 2023-04-15 15:35:52.443498 tavern-2.0.7/tavern/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-21 16:06:58.930000 tavern-2.0.7/tavern/_core/__init__.py
+-rw-r--r--   0        0        0    19780 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_core/dict_util.py
+-rw-r--r--   0        0        0     3842 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_core/exceptions.py
+-rw-r--r--   0        0        0     4737 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_core/extfunctions.py
+-rw-r--r--   0        0        0       96 2023-02-21 15:50:54.814531 tavern-2.0.7/tavern/_core/formatted_str.py
+-rw-r--r--   0        0        0      951 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_core/general.py
+-rw-r--r--   0        0        0     2612 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_core/jmesutils.py
+-rw-r--r--   0        0        0    12257 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_core/loader.py
+-rw-r--r--   0        0        0     9200 2023-04-15 14:36:17.314374 tavern-2.0.7/tavern/_core/plugins.py
+-rw-r--r--   0        0        0      275 2023-02-21 15:50:54.814531 tavern-2.0.7/tavern/_core/pytest/__init__.py
+-rw-r--r--   0        0        0     1617 2023-04-15 14:36:17.314374 tavern-2.0.7/tavern/_core/pytest/config.py
+-rw-r--r--   0        0        0     7393 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_core/pytest/error.py
+-rw-r--r--   0        0        0    13187 2023-04-15 14:36:17.314374 tavern-2.0.7/tavern/_core/pytest/file.py
+-rw-r--r--   0        0        0     1471 2023-04-15 15:35:15.079734 tavern-2.0.7/tavern/_core/pytest/hooks.py
+-rw-r--r--   0        0        0     9469 2023-04-15 15:35:15.079734 tavern-2.0.7/tavern/_core/pytest/item.py
+-rw-r--r--   0        0        0     2101 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_core/pytest/newhooks.py
+-rw-r--r--   0        0        0     5941 2023-04-15 15:35:15.079734 tavern-2.0.7/tavern/_core/pytest/util.py
+-rw-r--r--   0        0        0     1833 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_core/report.py
+-rw-r--r--   0        0        0    10800 2023-04-15 14:36:17.314374 tavern-2.0.7/tavern/_core/run.py
+-rw-r--r--   0        0        0        0 2023-02-21 16:06:58.930081 tavern-2.0.7/tavern/_core/schema/__init__.py
+-rw-r--r--   0        0        0    14523 2023-04-15 14:36:17.314374 tavern-2.0.7/tavern/_core/schema/extensions.py
+-rw-r--r--   0        0        0     4350 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_core/schema/files.py
+-rw-r--r--   0        0        0     6245 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_core/schema/jsonschema.py
+-rw-r--r--   0        0        0     9057 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_core/schema/tests.jsonschema.yaml
+-rw-r--r--   0        0        0     6845 2023-04-08 18:44:26.927400 tavern-2.0.7/tavern/_core/schema/tests.schema.yaml
+-rw-r--r--   0        0        0     1100 2023-02-21 15:50:54.817865 tavern-2.0.7/tavern/_core/stage_lines.py
+-rw-r--r--   0        0        0     5171 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_core/strict_util.py
+-rw-r--r--   0        0        0      383 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_core/strtobool.py
+-rw-r--r--   0        0        0     3958 2023-04-15 14:36:17.314374 tavern-2.0.7/tavern/_core/testhelpers.py
+-rw-r--r--   0        0        0        0 2023-02-21 16:06:58.930000 tavern-2.0.7/tavern/_plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-21 16:06:58.930000 tavern-2.0.7/tavern/_plugins/mqtt/__init__.py
+-rw-r--r--   0        0        0    17697 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_plugins/mqtt/client.py
+-rw-r--r--   0        0        0     4013 2023-02-21 15:50:54.817865 tavern-2.0.7/tavern/_plugins/mqtt/jsonschema.yaml
+-rw-r--r--   0        0        0     2523 2023-04-15 14:36:17.317707 tavern-2.0.7/tavern/_plugins/mqtt/request.py
+-rw-r--r--   0        0        0    11430 2023-04-15 15:04:25.003592 tavern-2.0.7/tavern/_plugins/mqtt/response.py
+-rw-r--r--   0        0        0     3233 2023-02-21 15:50:54.817865 tavern-2.0.7/tavern/_plugins/mqtt/schema.yaml
+-rw-r--r--   0        0        0     1267 2023-04-02 13:10:37.687090 tavern-2.0.7/tavern/_plugins/mqtt/tavernhook.py
+-rw-r--r--   0        0        0        0 2023-02-21 16:06:58.930000 tavern-2.0.7/tavern/_plugins/rest/__init__.py
+-rw-r--r--   0        0        0    19370 2023-04-15 14:36:17.317707 tavern-2.0.7/tavern/_plugins/rest/request.py
+-rw-r--r--   0        0        0     8291 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_plugins/rest/response.py
+-rw-r--r--   0        0        0      860 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/_plugins/rest/tavernhook.py
+-rw-r--r--   0        0        0     2969 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/core.py
+-rw-r--r--   0        0        0     2739 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/entry.py
+-rw-r--r--   0        0        0     7575 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/helpers.py
+-rw-r--r--   0        0        0      466 2023-04-08 18:45:13.188074 tavern-2.0.7/tavern/request.py
+-rw-r--r--   0        0        0     9571 2023-04-15 14:36:17.317707 tavern-2.0.7/tavern/response.py
+-rw-r--r--   0        0        0      919 2023-04-02 12:34:26.285355 tavern-2.0.7/tests/conftest.py
+-rw-r--r--   0        0        0      195 2023-04-15 14:36:17.317707 tavern-2.0.7/tests/integration/Dockerfile
+-rw-r--r--   0        0        0       33 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/OK.json.gz
+-rw-r--r--   0        0        0        3 2020-12-19 13:25:29.031794 tavern-2.0.7/tests/integration/OK.txt
+-rw-r--r--   0        0        0      504 2021-09-25 13:51:36.591636 tavern-2.0.7/tests/integration/README.md
+-rw-r--r--   0        0        0      608 2022-02-25 15:36:43.966205 tavern-2.0.7/tests/integration/common.yaml
+-rw-r--r--   0        0        0      621 2023-04-08 18:45:13.191407 tavern-2.0.7/tests/integration/conftest.py
+-rw-r--r--   0        0        0      126 2023-04-15 14:36:17.317707 tavern-2.0.7/tests/integration/docker-compose.yaml
+-rw-r--r--   0        0        0      167 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/ext_functions.py
+-rw-r--r--   0        0        0      203 2020-04-05 16:12:15.572937 tavern-2.0.7/tests/integration/extra.yaml
+-rw-r--r--   0        0        0      254 2021-05-01 10:23:38.259754 tavern-2.0.7/tests/integration/global_cfg.yaml
+-rw-r--r--   0        0        0       91 2021-03-07 14:36:40.846310 tavern-2.0.7/tests/integration/parametrize_includes.yaml
+-rw-r--r--   0        0        0    11475 2023-04-15 14:36:17.317707 tavern-2.0.7/tests/integration/server.py
+-rw-r--r--   0        0        0      297 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_allure.tavern.yaml
+-rw-r--r--   0        0        0      659 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_auth_key.tavern.yaml
+-rw-r--r--   0        0        0      624 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_certs.tavern.yaml
+-rw-r--r--   0        0        0     1569 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_cookie_remember.tavern.yaml
+-rw-r--r--   0        0        0     6106 2021-12-20 17:04:04.340877 tavern-2.0.7/tests/integration/test_cookies.tavern.yaml
+-rw-r--r--   0        0        0     2448 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_data_key.tavern.yaml
+-rw-r--r--   0        0        0       29 2022-08-06 15:34:18.544082 tavern-2.0.7/tests/integration/test_dummy.py
+-rw-r--r--   0        0        0      331 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_env_var_format.tavern.yaml
+-rw-r--r--   0        0        0      277 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_error.tavern.yaml
+-rw-r--r--   0        0        0     3152 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_external_functions.tavern.yaml
+-rw-r--r--   0        0        0     4086 2023-04-15 14:36:17.317707 tavern-2.0.7/tests/integration/test_files.tavern.yaml
+-rw-r--r--   0        0        0     2398 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_fixtures.tavern.yaml
+-rw-r--r--   0        0        0      799 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_follow_redirects.tavern.yaml
+-rw-r--r--   0        0        0     1028 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_header_comparisons.tavern.yaml
+-rw-r--r--   0        0        0     1269 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_helpers.tavern.yaml
+-rw-r--r--   0        0        0     4837 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_jmes.tavern.yaml
+-rw-r--r--   0        0        0      750 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_minimal.tavern.yaml
+-rw-r--r--   0        0        0    14838 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_parametrize.tavern.yaml
+-rw-r--r--   0        0        0     2167 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_regex.tavern.yaml
+-rw-r--r--   0        0        0     2031 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_response_types.tavern.yaml
+-rw-r--r--   0        0        0     2372 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_retry.tavern.yaml
+-rw-r--r--   0        0        0      575 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_save_dict_value.tavern.yaml
+-rw-r--r--   0        0        0      970 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_selective_tests.tavern.yaml
+-rw-r--r--   0        0        0     2432 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_skipped_tests.tavern.yaml
+-rw-r--r--   0        0        0     1506 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_status_codes.tavern.yaml
+-rw-r--r--   0        0        0      235 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_stream.tavern.yaml
+-rw-r--r--   0        0        0    10926 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_strict_key_checks.tavern.yaml
+-rw-r--r--   0        0        0     1951 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_timeout.tavern.yaml
+-rw-r--r--   0        0        0    12933 2023-04-08 18:45:13.191407 tavern-2.0.7/tests/integration/test_typetokens.tavern.yaml
+-rw-r--r--   0        0        0     1415 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/integration/test_validate_pykwalify.tavern.yaml
+-rw-r--r--   0        0        0        0 2020-04-05 16:12:15.572937 tavern-2.0.7/tests/integration/testfile.txt
+-rw-r--r--   0        0        0      650 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/logging.yaml
+-rw-r--r--   0        0        0      915 2023-04-15 14:36:17.317707 tavern-2.0.7/tests/unit/conftest.py
+-rw-r--r--   0        0        0     9612 2023-04-08 18:45:13.191407 tavern-2.0.7/tests/unit/response/test_mqtt_response.py
+-rw-r--r--   0        0        0    12296 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/unit/response/test_rest.py
+-rw-r--r--   0        0        0     1483 2023-04-08 18:44:26.930733 tavern-2.0.7/tests/unit/test_call_run.py
+-rw-r--r--   0        0        0    16186 2023-04-09 16:32:29.620833 tavern-2.0.7/tests/unit/test_core.py
+-rw-r--r--   0        0        0    14289 2023-04-15 14:36:17.317707 tavern-2.0.7/tests/unit/test_helpers.py
+-rw-r--r--   0        0        0     7161 2023-04-08 18:45:13.191407 tavern-2.0.7/tests/unit/test_mqtt.py
+-rw-r--r--   0        0        0     5791 2023-04-08 18:45:13.191407 tavern-2.0.7/tests/unit/test_pytest_hooks.py
+-rw-r--r--   0        0        0    14990 2023-04-08 18:45:13.191407 tavern-2.0.7/tests/unit/test_request.py
+-rw-r--r--   0        0        0     6131 2023-04-15 14:36:17.317707 tavern-2.0.7/tests/unit/test_schema.py
+-rw-r--r--   0        0        0     1030 2023-02-21 15:50:54.817865 tavern-2.0.7/tests/unit/test_strict_util.py
+-rw-r--r--   0        0        0    14898 2023-04-08 18:45:13.191407 tavern-2.0.7/tests/unit/test_utilities.py
+-rw-r--r--   0        0        0     2434 2023-04-08 18:44:26.930733 tavern-2.0.7/tox-integration.ini
+-rw-r--r--   0        0        0      625 2023-04-15 14:36:17.317707 tavern-2.0.7/tox.ini
+-rw-r--r--   0        0        0    10617 1970-01-01 00:00:00.000000 tavern-2.0.7/PKG-INFO
```

### Comparing `tavern-2.0.6/.dockerignore` & `tavern-2.0.7/.dockerignore`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/.github/workflows/main.yml` & `tavern-2.0.7/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/.gitignore` & `tavern-2.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/CHANGELOG.md` & `tavern-2.0.7/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -402,7 +402,9 @@
 ##  2.0.2           Fix saving in MQTT (2023-02-08)
 
 ##  2.0.3           Add type annotations (internal change) (2023-02-10)
 
 ##  2.0.4           Fix using ext functions in MQTT publish (2023-02-16)
 
 ##  2.0.5           Attempt to fix deadlock in subscribe locks (2023-02-16)
+
+##  2.0.6           Fix a few small MQTT issues (2023-03-13)
```

### Comparing `tavern-2.0.6/CONTRIBUTING.md` & `tavern-2.0.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/LICENSE` & `tavern-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/README.md` & `tavern-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/constraints.txt` & `tavern-2.0.7/constraints.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --all-extras --output-file=constraints.txt --resolver=backtracking --strip-extras pyproject.toml
 #
 allure-pytest==2.12.0
     # via tavern (pyproject.toml)
 allure-python-commons==2.12.0
@@ -88,14 +88,15 @@
     # via tavern (pyproject.toml)
 identify==2.5.10
     # via pre-commit
 idna==3.4
     # via requests
 importlib-metadata==5.2.0
     # via
+    #   flask
     #   keyring
     #   twine
 iniconfig==1.1.1
     # via pytest
 itsdangerous==2.1.2
     # via
     #   flask
@@ -266,15 +267,17 @@
 tox-travis==0.12
     # via tavern (pyproject.toml)
 twine==4.0.2
     # via tavern (pyproject.toml)
 types-pyyaml==6.0.12.2
     # via tavern (pyproject.toml)
 typing-extensions==4.4.0
-    # via mypy
+    # via
+    #   black
+    #   mypy
 urllib3==1.26.13
     # via
     #   docker
     #   requests
     #   twine
 virtualenv==20.17.1
     # via
```

### Comparing `tavern-2.0.6/docs/Makefile` & `tavern-2.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/docs/source/_static/favicon.png` & `tavern-2.0.7/docs/source/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/docs/source/_static/icon.png` & `tavern-2.0.7/docs/source/_static/icon.png`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/docs/source/basics.md` & `tavern-2.0.7/docs/source/basics.md`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/docs/source/conf.py` & `tavern-2.0.7/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = "1.0"
 # The full version, including alpha/beta/rc tags.
-release = "2.0.6"
+release = "2.0.7"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
```

### Comparing `tavern-2.0.6/docs/source/cookbook.md` & `tavern-2.0.7/docs/source/cookbook.md`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/docs/source/debugging.md` & `tavern-2.0.7/docs/source/debugging.md`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/docs/source/examples.md` & `tavern-2.0.7/docs/source/examples.md`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/docs/source/http.md` & `tavern-2.0.7/docs/source/http.md`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/docs/source/index.md` & `tavern-2.0.7/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/docs/source/mqtt.md` & `tavern-2.0.7/docs/source/mqtt.md`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/docs/source/plugins.md` & `tavern-2.0.7/docs/source/plugins.md`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/docs/source/server.md` & `tavern-2.0.7/docs/source/server.md`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/example/advanced/server.py` & `tavern-2.0.7/example/advanced/server.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/example/advanced/test_server.tavern.yaml` & `tavern-2.0.7/example/advanced/test_server.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/example/advanced/testing_utils.py` & `tavern-2.0.7/example/advanced/testing_utils.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/example/components/components.md` & `tavern-2.0.7/example/components/components.md`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/example/components/components/auth_stage.yaml` & `tavern-2.0.7/example/components/components/auth_stage.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/example/components/server.py` & `tavern-2.0.7/example/components/server.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/example/components/test_hello.tavern.yaml` & `tavern-2.0.7/example/components/test_hello.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/example/components/test_ping.tavern.yaml` & `tavern-2.0.7/example/components/test_ping.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/example/cookies/server.py` & `tavern-2.0.7/example/cookies/server.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/example/cookies/test_server.tavern.yaml` & `tavern-2.0.7/example/cookies/test_server.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/example/generate_from_openapi/Pipfile.lock` & `tavern-2.0.7/example/generate_from_openapi/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/example/generate_from_openapi/pub_tavern.py` & `tavern-2.0.7/example/generate_from_openapi/pub_tavern.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/example/generate_from_openapi/test_example_output.tavern.yaml` & `tavern-2.0.7/example/generate_from_openapi/test_example_output.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/example/hooks/conftest.py` & `tavern-2.0.7/example/hooks/conftest.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/example/hooks/test_server.tavern.yaml` & `tavern-2.0.7/example/hooks/test_server.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/example/mqtt/README.md` & `tavern-2.0.7/example/mqtt/README.md`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/example/mqtt/conftest.py` & `tavern-2.0.7/example/mqtt/conftest.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/example/mqtt/docker-compose.yaml` & `tavern-2.0.7/example/mqtt/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/example/mqtt/listener.py` & `tavern-2.0.7/example/mqtt/listener.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
         elif "ping" in message.topic:
             handle_ping_topic(client, message)
         elif "status" in message.topic:
             handle_status_topic(client, message)
         else:
             logging.warning("Got unexpected MQTT topic '%s'", message.topic)
     except Exception as e:
-        logging.exception(e)
+        logging.exception("error handling message: {}".format(e))
 
 
 def wait_for_messages():
     setup_logging()
     mqtt_client = get_client()
     mqtt_client.on_message = on_message_callback
     mqtt_client.reconnect()
```

### Comparing `tavern-2.0.6/example/mqtt/server.py` & `tavern-2.0.7/example/mqtt/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,19 +153,27 @@
     db = get_cached_db()
     with db:
         row = db.execute(
             "SELECT device_id from devices_table where device_id is :device_id", r
         )
 
     try:
-        next(row)
-    except StopIteration:
-        pass
+        r["clean"]
+    except (TypeError):
+        return jsonify({"error": "checking for clean key"}), 500
+    except KeyError:
+        try:
+            next(row)
+        except StopIteration:
+            pass
+        else:
+            return jsonify({"error": "device already exists"}), 400
     else:
-        return jsonify({"error": "device already exists"}), 400
+        with db:
+            db.execute("DELETE FROM devices_table")
 
     new_device = dict(lights_on=False, **r)
 
     logging.info("Creating new device: %s", new_device)
 
     with db:
         db.execute(
```

### Comparing `tavern-2.0.6/example/mqtt/test_mqtt.tavern.yaml` & `tavern-2.0.7/example/mqtt/test_mqtt.tavern.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
   - &setup_device_for_test
     name: create device
     request:
       url: "{host}/create_device"
       method: PUT
       json:
         device_id: "{random_device_id}"
+        clean: True
     response:
       status_code: 201
 
   - name: Echo text
     mqtt_publish:
       topic: /device/{random_device_id}/echo
       payload: hello world
```

### Comparing `tavern-2.0.6/example/mqtt/test_mqtt_failures.tavern.yaml` & `tavern-2.0.7/example/mqtt/test_mqtt_failures.tavern.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
   - &setup_device_for_test
     name: create device
     request:
       url: "{host}/create_device"
       method: PUT
       json:
         device_id: "{random_device_id}"
+        clean: True
     response:
       status_code: 201
 
   - name: step 1 - ping/pong
     mqtt_publish:
       topic: /device/123/ping
       payload: ping
@@ -160,15 +161,16 @@
     mqtt_publish:
       topic: /devices/status
     mqtt_response:
       - topic: /device/456/status/response
         payload: !anything
         timeout: 2
         qos: 1
-      - topic: /device/123/status/response
+        unexpected: true
+      - topic: /device/{random_device_id}/status/response
         payload: !anything
         timeout: 2
         qos: 1
         unexpected: true
 
 ---
 
@@ -184,12 +186,12 @@
 stages:
   - *setup_device_for_test
 
   - name: step 1 - ping/pong
     mqtt_publish:
       topic: /devices/status
     mqtt_response:
-      - topic: /device/123/status/response
+      - topic: /device/88466412/status/response
         payload: !anything
         timeout: 3
         qos: 1
         unexpected: true
```

### Comparing `tavern-2.0.6/example/simple/running_tests.md` & `tavern-2.0.7/example/simple/running_tests.md`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/example/simple/test_server.tavern.yaml` & `tavern-2.0.7/example/simple/test_server.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/pyproject.toml` & `tavern-2.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,24 +17,24 @@
     "License :: OSI Approved :: MIT License",
 ]
 
 keywords = ["testing", "pytest"]
 
 name = "tavern"
 description = "Simple testing of RESTful APIs"
-version = "2.0.6"
+version = "2.0.7"
 
 dependencies = [
     "PyYAML>=5.3.1,<7",
     "jmespath>=1,<2",
     "jsonschema>=3.2.0,<5",
     "paho-mqtt>=1.3.1,<=1.6.1",
     "pyjwt>=2.4.0,<3",
     "pykwalify>=1.8.0,<2",
-    "pytest>=7,<8",
+    "pytest>=7,<7.3",
     "python-box>=6,<7",
     "requests>=2.22.0,<3",
     "stevedore>=4,<5",
 ]
 
 requires-python = ">=3.8"
 
@@ -154,15 +154,15 @@
 [tool.ruff.per-file-ignores]
 "tests/*" = ["S"]
 
 [tool.ruff.isort]
 known-first-party = ["tavern"]
 
 [tool.tbump.version]
-current = "2.0.6"
+current = "2.0.7"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `tavern-2.0.6/requirements.txt` & `tavern-2.0.7/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --all-extras --generate-hashes --output-file=requirements.txt --resolver=backtracking pyproject.toml
 #
 allure-pytest==2.12.0 \
     --hash=sha256:1a10b2b78334443097d7be890a53c991e857e13d14781377c2f8d11eb4b5582c \
     --hash=sha256:85b73b1dbe9908ba4f84b80118a93e1049c02dd593209260d8c1c950cf286f6c
@@ -328,14 +328,15 @@
     --hash=sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4 \
     --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
     # via requests
 importlib-metadata==5.2.0 \
     --hash=sha256:0eafa39ba42bf225fc00e67f701d71f85aead9f878569caf13c3724f704b970f \
     --hash=sha256:404d48d62bba0b7a77ff9d405efd91501bef2e67ff4ace0bed40a0cf28c3c7cd
     # via
+    #   flask
     #   keyring
     #   twine
 iniconfig==1.1.1 \
     --hash=sha256:011e24c64b7f47f6ebd835bb12a743f2fbe9a26d4cecaa7f53bc4f35ee9da8b3 \
     --hash=sha256:bc3af051d7d14b2ee5ef9969666def0cd1a000e121eaea580d4a313df4b37f32
     # via pytest
 itsdangerous==2.1.2 \
@@ -855,15 +856,17 @@
 types-pyyaml==6.0.12.2 \
     --hash=sha256:1e94e80aafee07a7e798addb2a320e32956a373f376655128ae20637adb2655b \
     --hash=sha256:6840819871c92deebe6a2067fb800c11b8a063632eb4e3e755914e7ab3604e83
     # via tavern (pyproject.toml)
 typing-extensions==4.4.0 \
     --hash=sha256:1511434bb92bf8dd198c12b1cc812e800d4181cfcb867674e0f8279cc93087aa \
     --hash=sha256:16fa4864408f655d35ec496218b85f79b3437c829e93320c7c9215ccfd92489e
-    # via mypy
+    # via
+    #   black
+    #   mypy
 urllib3==1.26.13 \
     --hash=sha256:47cc05d99aaa09c9e72ed5809b60e7ba354e64b59c9c173ac3018642d8bb41fc \
     --hash=sha256:c083dd0dce68dbfbe1129d5271cb90f9447dea7d52097c6e0126120c521ddea8
     # via
     #   docker
     #   requests
     #   twine
```

### Comparing `tavern-2.0.6/scripts/update-changelog.bash` & `tavern-2.0.7/scripts/update-changelog.bash`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_core/dict_util.py` & `tavern-2.0.7/tavern/_core/dict_util.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_core/exceptions.py` & `tavern-2.0.7/tavern/_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_core/extfunctions.py` & `tavern-2.0.7/tavern/_core/extfunctions.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_core/general.py` & `tavern-2.0.7/tavern/_core/general.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_core/jmesutils.py` & `tavern-2.0.7/tavern/_core/jmesutils.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_core/loader.py` & `tavern-2.0.7/tavern/_core/loader.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_core/plugins.py` & `tavern-2.0.7/tavern/_core/plugins.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_core/pytest/config.py` & `tavern-2.0.7/tavern/_core/pytest/config.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_core/pytest/error.py` & `tavern-2.0.7/tavern/_core/pytest/error.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_core/pytest/file.py` & `tavern-2.0.7/tavern/_core/pytest/file.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_core/pytest/hooks.py` & `tavern-2.0.7/tavern/_core/pytest/hooks.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_core/pytest/item.py` & `tavern-2.0.7/tavern/_core/pytest/item.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_core/pytest/newhooks.py` & `tavern-2.0.7/tavern/_core/pytest/newhooks.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_core/pytest/util.py` & `tavern-2.0.7/tavern/_core/pytest/util.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_core/report.py` & `tavern-2.0.7/tavern/_core/report.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_core/run.py` & `tavern-2.0.7/tavern/_core/run.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_core/schema/extensions.py` & `tavern-2.0.7/tavern/_core/schema/extensions.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_core/schema/files.py` & `tavern-2.0.7/tavern/_core/schema/files.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_core/schema/jsonschema.py` & `tavern-2.0.7/tavern/_core/schema/jsonschema.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_core/schema/tests.jsonschema.yaml` & `tavern-2.0.7/tavern/_core/schema/tests.jsonschema.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_core/schema/tests.schema.yaml` & `tavern-2.0.7/tavern/_core/schema/tests.schema.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_core/stage_lines.py` & `tavern-2.0.7/tavern/_core/stage_lines.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_core/strict_util.py` & `tavern-2.0.7/tavern/_core/strict_util.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_core/testhelpers.py` & `tavern-2.0.7/tavern/_core/testhelpers.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_plugins/mqtt/client.py` & `tavern-2.0.7/tavern/_plugins/mqtt/client.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_plugins/mqtt/jsonschema.yaml` & `tavern-2.0.7/tavern/_plugins/mqtt/jsonschema.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_plugins/mqtt/request.py` & `tavern-2.0.7/tavern/_plugins/mqtt/request.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_plugins/mqtt/response.py` & `tavern-2.0.7/tavern/_plugins/mqtt/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import concurrent.futures
 import contextlib
 import itertools
 import json
 import logging
 import time
 from dataclasses import dataclass
-from typing import List, Optional, Tuple, Union
+from typing import Dict, List, Mapping, Optional, Tuple, Union
 
 from paho.mqtt.client import MQTTMessage
 
 from tavern._core import exceptions
 from tavern._core.dict_util import check_keys_match_recursive
 from tavern._core.loader import ANYTHING
 from tavern._core.pytest.newhooks import call_hook
@@ -131,21 +131,22 @@
                 ),
                 failures=self.errors,
             )
 
         return saved
 
     def _await_messages_on_topic(
-        self, topic: str, expected
+        self, topic: str, expected: List[Dict]
     ) -> Tuple[List["_ReturnedMessage"], List[str]]:
         """
         Waits for the specific message
 
         Args:
-            expected (list): expected response for this block
+            topic: topic to listen on
+            expected: expected response for this block
 
         Returns:
             tuple(msg, list): The correct message (if any) and warnings from processing the message
         """
 
         timeout = max(m.get("timeout", _default_timeout) for m in expected)
 
@@ -313,15 +314,15 @@
             )
             logger.debug("Matched payload was '%s", msg.payload)
             return True
 
         return False
 
     @staticmethod
-    def _get_payload_vals(expected) -> Tuple[Optional[Union[str, dict]], bool]:
+    def _get_payload_vals(expected: Mapping) -> Tuple[Optional[Union[str, dict]], bool]:
         """Gets the payload from the 'expected' block
 
         Returns:
             tuple: First element is the expected payload, second element is whether it's
                 expected to be json or not
         """
         # TODO move this check to initialisation/schema checking
```

### Comparing `tavern-2.0.6/tavern/_plugins/mqtt/schema.yaml` & `tavern-2.0.7/tavern/_plugins/mqtt/schema.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_plugins/mqtt/tavernhook.py` & `tavern-2.0.7/tavern/_plugins/mqtt/tavernhook.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_plugins/rest/request.py` & `tavern-2.0.7/tavern/_plugins/rest/request.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_plugins/rest/response.py` & `tavern-2.0.7/tavern/_plugins/rest/response.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/_plugins/rest/tavernhook.py` & `tavern-2.0.7/tavern/_plugins/rest/tavernhook.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/core.py` & `tavern-2.0.7/tavern/core.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/entry.py` & `tavern-2.0.7/tavern/entry.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/helpers.py` & `tavern-2.0.7/tavern/helpers.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tavern/response.py` & `tavern-2.0.7/tavern/response.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/conftest.py` & `tavern-2.0.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/integration/common.yaml` & `tavern-2.0.7/tests/integration/common.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/integration/conftest.py` & `tavern-2.0.7/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/integration/server.py` & `tavern-2.0.7/tests/integration/server.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/integration/test_auth_key.tavern.yaml` & `tavern-2.0.7/tests/integration/test_auth_key.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/integration/test_certs.tavern.yaml` & `tavern-2.0.7/tests/integration/test_certs.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/integration/test_cookie_remember.tavern.yaml` & `tavern-2.0.7/tests/integration/test_cookie_remember.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/integration/test_cookies.tavern.yaml` & `tavern-2.0.7/tests/integration/test_cookies.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/integration/test_data_key.tavern.yaml` & `tavern-2.0.7/tests/integration/test_data_key.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/integration/test_external_functions.tavern.yaml` & `tavern-2.0.7/tests/integration/test_external_functions.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/integration/test_files.tavern.yaml` & `tavern-2.0.7/tests/integration/test_files.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/integration/test_fixtures.tavern.yaml` & `tavern-2.0.7/tests/integration/test_fixtures.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/integration/test_follow_redirects.tavern.yaml` & `tavern-2.0.7/tests/integration/test_follow_redirects.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/integration/test_header_comparisons.tavern.yaml` & `tavern-2.0.7/tests/integration/test_header_comparisons.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/integration/test_helpers.tavern.yaml` & `tavern-2.0.7/tests/integration/test_helpers.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/integration/test_jmes.tavern.yaml` & `tavern-2.0.7/tests/integration/test_jmes.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/integration/test_minimal.tavern.yaml` & `tavern-2.0.7/tests/integration/test_minimal.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/integration/test_parametrize.tavern.yaml` & `tavern-2.0.7/tests/integration/test_parametrize.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/integration/test_regex.tavern.yaml` & `tavern-2.0.7/tests/integration/test_regex.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/integration/test_response_types.tavern.yaml` & `tavern-2.0.7/tests/integration/test_response_types.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/integration/test_retry.tavern.yaml` & `tavern-2.0.7/tests/integration/test_retry.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/integration/test_save_dict_value.tavern.yaml` & `tavern-2.0.7/tests/integration/test_save_dict_value.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/integration/test_selective_tests.tavern.yaml` & `tavern-2.0.7/tests/integration/test_selective_tests.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/integration/test_skipped_tests.tavern.yaml` & `tavern-2.0.7/tests/integration/test_skipped_tests.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/integration/test_status_codes.tavern.yaml` & `tavern-2.0.7/tests/integration/test_status_codes.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/integration/test_strict_key_checks.tavern.yaml` & `tavern-2.0.7/tests/integration/test_strict_key_checks.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/integration/test_timeout.tavern.yaml` & `tavern-2.0.7/tests/integration/test_timeout.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/integration/test_typetokens.tavern.yaml` & `tavern-2.0.7/tests/integration/test_typetokens.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/integration/test_validate_pykwalify.tavern.yaml` & `tavern-2.0.7/tests/integration/test_validate_pykwalify.tavern.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/logging.yaml` & `tavern-2.0.7/tests/logging.yaml`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/unit/conftest.py` & `tavern-2.0.7/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/unit/response/test_mqtt_response.py` & `tavern-2.0.7/tests/unit/response/test_mqtt_response.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/unit/response/test_rest.py` & `tavern-2.0.7/tests/unit/response/test_rest.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/unit/test_call_run.py` & `tavern-2.0.7/tests/unit/test_call_run.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/unit/test_core.py` & `tavern-2.0.7/tests/unit/test_core.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/unit/test_helpers.py` & `tavern-2.0.7/tests/unit/test_helpers.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/unit/test_mqtt.py` & `tavern-2.0.7/tests/unit/test_mqtt.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/unit/test_pytest_hooks.py` & `tavern-2.0.7/tests/unit/test_pytest_hooks.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/unit/test_request.py` & `tavern-2.0.7/tests/unit/test_request.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/unit/test_schema.py` & `tavern-2.0.7/tests/unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/unit/test_strict_util.py` & `tavern-2.0.7/tests/unit/test_strict_util.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tests/unit/test_utilities.py` & `tavern-2.0.7/tests/unit/test_utilities.py`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tox-integration.ini` & `tavern-2.0.7/tox-integration.ini`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/tox.ini` & `tavern-2.0.7/tox.ini`

 * *Files identical despite different names*

### Comparing `tavern-2.0.6/PKG-INFO` & `tavern-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tavern
-Version: 2.0.6
+Version: 2.0.7
 Summary: Simple testing of RESTful APIs
 Keywords: testing,pytest
 Author: Michael Boulton
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -18,15 +18,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: PyYAML>=5.3.1,<7
 Requires-Dist: jmespath>=1,<2
 Requires-Dist: jsonschema>=3.2.0,<5
 Requires-Dist: paho-mqtt>=1.3.1,<=1.6.1
 Requires-Dist: pyjwt>=2.4.0,<3
 Requires-Dist: pykwalify>=1.8.0,<2
-Requires-Dist: pytest>=7,<8
+Requires-Dist: pytest>=7,<7.3
 Requires-Dist: python-box>=6,<7
 Requires-Dist: requests>=2.22.0,<3
 Requires-Dist: stevedore>=4,<5
 Requires-Dist: Faker ; extra == "dev"
 Requires-Dist: allure-pytest ; extra == "dev"
 Requires-Dist: black==23.1.0 ; extra == "dev"
 Requires-Dist: bump2version ; extra == "dev"
```

