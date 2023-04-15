# Comparing `tmp/OctoBot-Tentacles-Manager-2.8.5.tar.gz` & `tmp/OctoBot-Tentacles-Manager-2.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OctoBot-Tentacles-Manager-2.8.5.tar", last modified: Mon Mar 27 16:45:40 2023, max compression
+gzip compressed data, was "OctoBot-Tentacles-Manager-2.8.6.tar", last modified: Sat Apr 15 08:55:12 2023, max compression
```

## Comparing `OctoBot-Tentacles-Manager-2.8.5.tar` & `OctoBot-Tentacles-Manager-2.8.6.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:45:40.836829 OctoBot-Tentacles-Manager-2.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:45:40.828829 OctoBot-Tentacles-Manager-2.8.5/OctoBot_Tentacles_Manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-03-27 16:45:40.000000 OctoBot-Tentacles-Manager-2.8.5/OctoBot_Tentacles_Manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-03-27 16:45:40.000000 OctoBot-Tentacles-Manager-2.8.5/OctoBot_Tentacles_Manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 16:45:40.000000 OctoBot-Tentacles-Manager-2.8.5/OctoBot_Tentacles_Manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-27 16:45:40.000000 OctoBot-Tentacles-Manager-2.8.5/OctoBot_Tentacles_Manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 16:45:40.000000 OctoBot-Tentacles-Manager-2.8.5/OctoBot_Tentacles_Manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-27 16:45:40.000000 OctoBot-Tentacles-Manager-2.8.5/OctoBot_Tentacles_Manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-27 16:45:40.000000 OctoBot-Tentacles-Manager-2.8.5/OctoBot_Tentacles_Manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-03-27 16:45:40.836829 OctoBot-Tentacles-Manager-2.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:45:40.828829 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:45:40.828829 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/api/
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/api/configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/api/creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/api/inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/api/installer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/api/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/api/uninstaller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/api/updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/api/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:45:40.828829 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/api/util/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/api/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/api/util/tentacles_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:45:40.832829 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/configuration/config_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/configuration/tentacle_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    21188 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/configuration/tentacles_setup_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:45:40.832829 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/creators/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/creators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/creators/compiled_package_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:45:40.832829 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/creators/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/creators/templates/Mode_config.template
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/creators/templates/Mode_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/creators/templates/RealTime_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/creators/templates/Social_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/creators/templates/Strategies_config.template
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/creators/templates/Strategies_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/creators/templates/TA_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/creators/templates/Util_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/creators/templates/description_tentacle.template
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/creators/tentacle_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:45:40.832829 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/exporters/artifact_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/exporters/tentacle_bundle_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/exporters/tentacle_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/exporters/tentacle_package_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:45:40.832829 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/loaders/tentacle_loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:45:40.832829 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/managers/
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/managers/profiles_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/managers/python_modules_requirements_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/managers/tentacle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/managers/tentacles_init_files_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/managers/tentacles_setup_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:45:40.832829 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/artifact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:45:40.832829 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/metadata/artifact_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/metadata/metadata_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/metadata/profile_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/metadata/tentacle_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/metadata/tentacle_package_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/tentacle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/tentacle_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/tentacle_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/tentacle_requirements_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/tentacle_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:45:40.836829 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/uploaders/
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/uploaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/uploaders/nexus_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/uploaders/s3_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/uploaders/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:45:40.836829 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/util/
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/util/file_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/util/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/util/os_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/util/tentacle_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/util/tentacle_explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/util/tentacle_fetching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/util/tentacle_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:45:40.836829 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/workers/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/workers/install_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/workers/repair_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/workers/single_install_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/workers/tentacles_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/workers/uninstall_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/workers/update_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-03-27 16:45:40.840829 OctoBot-Tentacles-Manager-2.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:45:40.828829 OctoBot-Tentacles-Manager-2.8.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:45:40.836829 OctoBot-Tentacles-Manager-2.8.5/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/tests/api/test_configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/tests/api/test_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/tests/api/test_installer.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/tests/api/test_tentacle_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/tests/api/test_uninstaller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/tests/api/test_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:45:40.836829 OctoBot-Tentacles-Manager-2.8.5/tests/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/tests/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/tests/configuration/test_tentacle_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/tests/configuration/test_tentacles_setup_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:45:40.836829 OctoBot-Tentacles-Manager-2.8.5/tests/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/tests/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/tests/exporters/test_tentacle_bundle_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:45:40.836829 OctoBot-Tentacles-Manager-2.8.5/tests/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/tests/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/tests/loaders/test_tentacle_loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:45:40.836829 OctoBot-Tentacles-Manager-2.8.5/tests/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/tests/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/tests/managers/test_tentacles_setup_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:45:40.836829 OctoBot-Tentacles-Manager-2.8.5/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/tests/util/test_tentacle_fetching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:45:40.836829 OctoBot-Tentacles-Manager-2.8.5/tests/workers/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/tests/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/tests/workers/test_install_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/tests/workers/test_uninstall_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/tests/workers/test_update_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 16:45:40.836829 OctoBot-Tentacles-Manager-2.8.5/upload_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/upload_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/upload_tests/_test_nexus_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-03-27 16:45:14.000000 OctoBot-Tentacles-Manager-2.8.5/upload_tests/test_s3_uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:12.002466 OctoBot-Tentacles-Manager-2.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.994466 OctoBot-Tentacles-Manager-2.8.6/OctoBot_Tentacles_Manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-15 08:55:11.000000 OctoBot-Tentacles-Manager-2.8.6/OctoBot_Tentacles_Manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-04-15 08:55:11.000000 OctoBot-Tentacles-Manager-2.8.6/OctoBot_Tentacles_Manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 08:55:11.000000 OctoBot-Tentacles-Manager-2.8.6/OctoBot_Tentacles_Manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-15 08:55:11.000000 OctoBot-Tentacles-Manager-2.8.6/OctoBot_Tentacles_Manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 08:55:11.000000 OctoBot-Tentacles-Manager-2.8.6/OctoBot_Tentacles_Manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-15 08:55:11.000000 OctoBot-Tentacles-Manager-2.8.6/OctoBot_Tentacles_Manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-15 08:55:11.000000 OctoBot-Tentacles-Manager-2.8.6/OctoBot_Tentacles_Manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-15 08:55:12.002466 OctoBot-Tentacles-Manager-2.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.994466 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.994466 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/uninstaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.994466 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/util/tentacles_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.994466 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/configuration/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/configuration/tentacle_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22307 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/configuration/tentacles_setup_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.994466 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/compiled_package_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.994466 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/templates/Mode_config.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/templates/Mode_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/templates/RealTime_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/templates/Social_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/templates/Strategies_config.template
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/templates/Strategies_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/templates/TA_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/templates/Util_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/templates/description_tentacle.template
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/tentacle_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.998466 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/exporters/artifact_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/exporters/tentacle_bundle_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/exporters/tentacle_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/exporters/tentacle_package_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.998466 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/loaders/tentacle_loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.998466 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/managers/profiles_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/managers/python_modules_requirements_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/managers/tentacle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/managers/tentacles_init_files_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9745 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/managers/tentacles_setup_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.998466 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/artifact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.998466 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/metadata/artifact_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/metadata/metadata_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/metadata/profile_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/metadata/tentacle_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/metadata/tentacle_package_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/tentacle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/tentacle_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/tentacle_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/tentacle_requirements_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/tentacle_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.998466 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/uploaders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/uploaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/uploaders/nexus_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/uploaders/s3_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/uploaders/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.998466 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/os_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/tentacle_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/tentacle_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/tentacle_fetching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/tentacle_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.998466 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/install_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/repair_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/single_install_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6994 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/tentacles_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/uninstall_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/update_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-15 08:55:12.002466 OctoBot-Tentacles-Manager-2.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:11.990466 OctoBot-Tentacles-Manager-2.8.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:12.002466 OctoBot-Tentacles-Manager-2.8.6/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/api/test_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/api/test_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/api/test_installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/api/test_tentacle_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/api/test_uninstaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/api/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:12.002466 OctoBot-Tentacles-Manager-2.8.6/tests/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/configuration/test_tentacle_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/configuration/test_tentacles_setup_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:12.002466 OctoBot-Tentacles-Manager-2.8.6/tests/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/exporters/test_tentacle_bundle_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:12.002466 OctoBot-Tentacles-Manager-2.8.6/tests/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/loaders/test_tentacle_loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:12.002466 OctoBot-Tentacles-Manager-2.8.6/tests/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/managers/test_tentacles_setup_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:12.002466 OctoBot-Tentacles-Manager-2.8.6/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/util/test_tentacle_fetching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:12.002466 OctoBot-Tentacles-Manager-2.8.6/tests/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/workers/test_install_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/workers/test_uninstall_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/tests/workers/test_update_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:55:12.002466 OctoBot-Tentacles-Manager-2.8.6/upload_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/upload_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/upload_tests/_test_nexus_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-04-15 08:54:40.000000 OctoBot-Tentacles-Manager-2.8.6/upload_tests/test_s3_uploader.py
```

### Comparing `OctoBot-Tentacles-Manager-2.8.5/CHANGELOG.md` & `OctoBot-Tentacles-Manager-2.8.6/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [2.8.6] - 2022-04-15
+### Added
+- [API] add deactivate_all 
+
 ## [2.8.5] - 2022-03-27
 ### Added
 - [API] add get_tentacles_classes_names_for_type 
 
 ## [2.8.4] - 2022-02-16
 ### Updated
 - [Configuration] Improve configuration file error management
```

### Comparing `OctoBot-Tentacles-Manager-2.8.5/LICENSE` & `OctoBot-Tentacles-Manager-2.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/OctoBot_Tentacles_Manager.egg-info/PKG-INFO` & `OctoBot-Tentacles-Manager-2.8.6/OctoBot_Tentacles_Manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.2
 Name: OctoBot-Tentacles-Manager
-Version: 2.8.5
+Version: 2.8.6
 Summary: OctoBot project module installer
 Home-page: https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager
 Author: Drakkar-Software
 Author-email: drakkar-software@protonmail.com
 License: LGPL-3.0
-Description: # OctoBot-Tentacles-Manager [2.8.5](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
+Description: # OctoBot-Tentacles-Manager [2.8.6](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
         [![PyPI](https://img.shields.io/pypi/v/OctoBot-Tentacles-Manager.svg)](https://pypi.python.org/pypi/OctoBot-Tentacles-Manager/)
         [![Downloads](https://pepy.tech/badge/OctoBot-Tentacles-Manager/month)](https://pepy.tech/project/OctoBot-Tentacles-Manager)
         [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/workflows/OctoBot-Tentacles-Manager-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/actions)
         
         A module manager for your [OctoBot](https://github.com/Drakkar-Software/OctoBot) ! 
         
         - Install OctoBot-Tentacles-Manager from pip :
```

### Comparing `OctoBot-Tentacles-Manager-2.8.5/OctoBot_Tentacles_Manager.egg-info/SOURCES.txt` & `OctoBot-Tentacles-Manager-2.8.6/OctoBot_Tentacles_Manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/PKG-INFO` & `OctoBot-Tentacles-Manager-2.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.2
 Name: OctoBot-Tentacles-Manager
-Version: 2.8.5
+Version: 2.8.6
 Summary: OctoBot project module installer
 Home-page: https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager
 Author: Drakkar-Software
 Author-email: drakkar-software@protonmail.com
 License: LGPL-3.0
-Description: # OctoBot-Tentacles-Manager [2.8.5](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
+Description: # OctoBot-Tentacles-Manager [2.8.6](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
         [![PyPI](https://img.shields.io/pypi/v/OctoBot-Tentacles-Manager.svg)](https://pypi.python.org/pypi/OctoBot-Tentacles-Manager/)
         [![Downloads](https://pepy.tech/badge/OctoBot-Tentacles-Manager/month)](https://pepy.tech/project/OctoBot-Tentacles-Manager)
         [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/workflows/OctoBot-Tentacles-Manager-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/actions)
         
         A module manager for your [OctoBot](https://github.com/Drakkar-Software/OctoBot) ! 
         
         - Install OctoBot-Tentacles-Manager from pip :
```

### Comparing `OctoBot-Tentacles-Manager-2.8.5/README.md` & `OctoBot-Tentacles-Manager-2.8.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# OctoBot-Tentacles-Manager [2.8.5](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
+# OctoBot-Tentacles-Manager [2.8.6](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/tree/master/CHANGELOG.md)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot-Tentacles-Manager.svg)](https://pypi.python.org/pypi/OctoBot-Tentacles-Manager/)
 [![Downloads](https://pepy.tech/badge/OctoBot-Tentacles-Manager/month)](https://pepy.tech/project/OctoBot-Tentacles-Manager)
 [![Github-Action-CI](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/workflows/OctoBot-Tentacles-Manager-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot-Tentacles-Manager/actions)
 
 A module manager for your [OctoBot](https://github.com/Drakkar-Software/OctoBot) ! 
 
 - Install OctoBot-Tentacles-Manager from pip :
```

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/__init__.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,9 +10,9 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 #  Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public
 #  License along with this library.
 
-VERSION = "2.8.5"
+VERSION = "2.8.6"
 PROJECT_NAME = "OctoBot-Tentacles-Manager"
```

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/api/__init__.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     create_tentacles_setup_config_with_tentacles,
     is_tentacle_activated_in_tentacles_setup_config,
     get_class_from_name_with_activated_required_tentacles,
     get_tentacles_activation,
     get_registered_tentacle_packages,
     unregister_tentacle_packages,
     update_activation_configuration,
+    deactivate_all_tentacles,
     save_tentacles_setup_configuration,
     has_profile_local_configuration,
     get_activated_tentacles,
     update_tentacle_config,
     import_user_tentacles_config_folder,
     get_tentacle_config,
     factory_tentacle_reset_config,
@@ -108,14 +109,15 @@
     "create_tentacles_setup_config_with_tentacles",
     "is_tentacle_activated_in_tentacles_setup_config",
     "get_class_from_name_with_activated_required_tentacles",
     "get_tentacles_activation",
     "get_registered_tentacle_packages",
     "unregister_tentacle_packages",
     "update_activation_configuration",
+    "deactivate_all_tentacles",
     "save_tentacles_setup_configuration",
     "has_profile_local_configuration",
     "get_activated_tentacles",
     "update_tentacle_config",
     "get_tentacle_config",
     "import_user_tentacles_config_folder",
     "factory_tentacle_reset_config",
```

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/api/configurator.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/configurator.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,19 @@
 
 def update_activation_configuration(tentacles_setup_config: configuration.TentaclesSetupConfiguration,
                                     new_config: dict, deactivate_others: bool, add_missing_elements=False) \
         -> bool:
     return tentacles_setup_config.update_activation_configuration(new_config, deactivate_others, add_missing_elements)
 
 
+def deactivate_all_tentacles(tentacles_setup_config: configuration.TentaclesSetupConfiguration,
+                             trading_modes: bool, strategies: bool, evaluators: bool):
+    tentacles_setup_config.deactivate_all(trading_modes, strategies, evaluators)
+
+
 def save_tentacles_setup_configuration(tentacles_setup_config: configuration.TentaclesSetupConfiguration) -> None:
     tentacles_setup_config.save_config()
 
 
 def has_profile_local_configuration(tentacles_setup_config: configuration.TentaclesSetupConfiguration, tentacle_class):
     return path.exists(configuration.get_profile_config_specific_file_path(tentacles_setup_config, tentacle_class))
```

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/api/creator.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/creator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/api/inspector.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/inspector.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/api/installer.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/installer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/api/loader.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/loader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/api/uninstaller.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/uninstaller.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/api/updater.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/api/uploader.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/uploader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/api/util/__init__.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/api/util/tentacles_management.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/api/util/tentacles_management.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/cli.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/cli.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/configuration/__init__.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/configuration/config_file.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/configuration/config_file.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/configuration/tentacle_configuration.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/configuration/tentacle_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 def get_config(tentacles_setup_config, klass) -> dict:
     config_path = _get_config_file_path(tentacles_setup_config, klass)
     if not config_path:
         return {}
     return configuration.read_config(config_path)
 
 
-def update_config(tentacles_setup_config, klass, config_update, keep_existing = True) -> None:
+def update_config(tentacles_setup_config, klass, config_update, keep_existing=True) -> None:
     config_file = _get_config_file_path(tentacles_setup_config, klass)
     current_config = configuration.read_config(config_file)
     # only update values in config update not to erase values in root config (might not be editable)
     if keep_existing:
         # keep inactive settings in nested dicts
         current_config = _recursive_config_update(current_config, config_update)
     else:
```

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/configuration/tentacles_setup_configuration.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/configuration/tentacles_setup_configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,14 +137,30 @@
             tentacle_name = tentacle_class.get_name()
             tentacle = tentacle_by_class_name[tentacle_name]
             try:
                 self.tentacles_activation[tentacle.tentacle_root_type][tentacle_name] = True
             except KeyError:
                 self.tentacles_activation[tentacle.tentacle_root_type] = {tentacle_name: True}
 
+    def deactivate_all(self, trading_modes: bool, strategies: bool, evaluators: bool):
+        to_deactivate_tentacles_types = [constants.TENTACLES_TRADING_MODE_PATH] if trading_modes else []
+        to_deactivate_tentacles_types += [constants.TENTACLES_EVALUATOR_STRATEGIES_PATH] if strategies else []
+        to_deactivate_tentacles_types += [
+            constants.TENTACLES_EVALUATOR_TA_PATH,
+            constants.TENTACLES_EVALUATOR_SOCIAL_PATH,
+            constants.TENTACLES_EVALUATOR_REALTIME_PATH,
+            constants.TENTACLES_EVALUATOR_SCRIPTED_PATH
+        ] if evaluators else []
+        for element_type, element_names in self.tentacles_activation.items():
+            for element_name in element_names:
+                if loaders.get_tentacle_classes()[element_name].get_simple_tentacle_type() \
+                        in to_deactivate_tentacles_types and self.tentacles_activation[element_type][element_name]:
+                    self.logger.info(f"Tentacles configuration updated: {element_name} {'deactivated'}")
+                    self.tentacles_activation[element_type][element_name] = False
+
     def _deactivate_other_evaluators(self, new_config):
         something_changed = False
         for element_type, element_names in self.tentacles_activation.items():
             for element_name in element_names:
                 # for each activated element that is not in new_config
                 if element_name not in new_config and self.tentacles_activation[element_type][element_name]:
                     # only handle evaluator tentacles
```

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/constants.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/constants.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/creators/__init__.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/creators/compiled_package_manager.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/compiled_package_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/creators/templates/Mode_tentacle.template` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/templates/Mode_tentacle.template`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/creators/templates/RealTime_tentacle.template` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/templates/RealTime_tentacle.template`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/creators/templates/Social_tentacle.template` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/templates/Social_tentacle.template`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/creators/tentacle_creator.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/creators/tentacle_creator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/enums.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/enums.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/exporters/__init__.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/exporters/artifact_exporter.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/exporters/artifact_exporter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/exporters/tentacle_bundle_exporter.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/exporters/tentacle_bundle_exporter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/exporters/tentacle_exporter.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/exporters/tentacle_exporter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/exporters/tentacle_package_exporter.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/exporters/tentacle_package_exporter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/loaders/__init__.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/loaders/tentacle_loading.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/loaders/tentacle_loading.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/managers/__init__.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/managers/profiles_manager.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/managers/profiles_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/managers/python_modules_requirements_manager.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/managers/python_modules_requirements_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/managers/tentacle_manager.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/managers/tentacle_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/managers/tentacles_init_files_manager.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/managers/tentacles_init_files_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/managers/tentacles_setup_manager.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/managers/tentacles_setup_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/__init__.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/artifact.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/artifact.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/metadata/__init__.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/metadata/artifact_metadata.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/metadata/artifact_metadata.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/metadata/metadata_factory.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/metadata/metadata_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/metadata/profile_metadata.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/metadata/profile_metadata.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/metadata/tentacle_metadata.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/metadata/tentacle_metadata.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/metadata/tentacle_package_metadata.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/metadata/tentacle_package_metadata.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/profile.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/profile.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/tentacle.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/tentacle.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/tentacle_factory.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/tentacle_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/tentacle_package.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/tentacle_package.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/tentacle_requirements_tree.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/tentacle_requirements_tree.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/models/tentacle_type.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/models/tentacle_type.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/uploaders/__init__.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/uploaders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/uploaders/nexus_uploader.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/uploaders/nexus_uploader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/uploaders/s3_uploader.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/uploaders/s3_uploader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/uploaders/uploader.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/uploaders/uploader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/util/__init__.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/util/file_util.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/file_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/util/hashing.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/hashing.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/util/os_util.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/os_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/util/tentacle_cleaner.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/tentacle_cleaner.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/util/tentacle_explorer.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/tentacle_explorer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/util/tentacle_fetching.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/tentacle_fetching.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/util/tentacle_filter.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/util/tentacle_filter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/workers/__init__.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/workers/install_worker.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/install_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/workers/repair_worker.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/repair_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/workers/single_install_worker.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/single_install_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/workers/tentacles_worker.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/tentacles_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/workers/uninstall_worker.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/uninstall_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/octobot_tentacles_manager/workers/update_worker.py` & `OctoBot-Tentacles-Manager-2.8.6/octobot_tentacles_manager/workers/update_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/setup.py` & `OctoBot-Tentacles-Manager-2.8.6/setup.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/tests/api/__init__.py` & `OctoBot-Tentacles-Manager-2.8.6/tests/api/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/tests/api/test_configurator.py` & `OctoBot-Tentacles-Manager-2.8.6/tests/api/test_configurator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/tests/api/test_creator.py` & `OctoBot-Tentacles-Manager-2.8.6/tests/api/test_creator.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/tests/api/test_installer.py` & `OctoBot-Tentacles-Manager-2.8.6/tests/api/test_installer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/tests/api/test_uninstaller.py` & `OctoBot-Tentacles-Manager-2.8.6/tests/api/test_uninstaller.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/tests/api/test_updater.py` & `OctoBot-Tentacles-Manager-2.8.6/tests/api/test_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/tests/configuration/__init__.py` & `OctoBot-Tentacles-Manager-2.8.6/tests/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/tests/configuration/test_tentacle_configuration.py` & `OctoBot-Tentacles-Manager-2.8.6/tests/configuration/test_tentacle_configuration.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/tests/configuration/test_tentacles_setup_configuration.py` & `OctoBot-Tentacles-Manager-2.8.6/tests/configuration/test_tentacles_setup_configuration.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/tests/exporters/__init__.py` & `OctoBot-Tentacles-Manager-2.8.6/tests/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/tests/exporters/test_tentacle_bundle_exporter.py` & `OctoBot-Tentacles-Manager-2.8.6/tests/exporters/test_tentacle_bundle_exporter.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/tests/loaders/__init__.py` & `OctoBot-Tentacles-Manager-2.8.6/tests/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/tests/loaders/test_tentacle_loading.py` & `OctoBot-Tentacles-Manager-2.8.6/tests/loaders/test_tentacle_loading.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/tests/managers/__init__.py` & `OctoBot-Tentacles-Manager-2.8.6/tests/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/tests/managers/test_tentacles_setup_manager.py` & `OctoBot-Tentacles-Manager-2.8.6/tests/managers/test_tentacles_setup_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/tests/util/__init__.py` & `OctoBot-Tentacles-Manager-2.8.6/tests/util/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/tests/util/test_tentacle_fetching.py` & `OctoBot-Tentacles-Manager-2.8.6/tests/util/test_tentacle_fetching.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/tests/workers/__init__.py` & `OctoBot-Tentacles-Manager-2.8.6/tests/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/tests/workers/test_install_worker.py` & `OctoBot-Tentacles-Manager-2.8.6/tests/workers/test_install_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/tests/workers/test_uninstall_worker.py` & `OctoBot-Tentacles-Manager-2.8.6/tests/workers/test_uninstall_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/tests/workers/test_update_worker.py` & `OctoBot-Tentacles-Manager-2.8.6/tests/workers/test_update_worker.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/upload_tests/__init__.py` & `OctoBot-Tentacles-Manager-2.8.6/upload_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/upload_tests/_test_nexus_uploader.py` & `OctoBot-Tentacles-Manager-2.8.6/upload_tests/_test_nexus_uploader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-Tentacles-Manager-2.8.5/upload_tests/test_s3_uploader.py` & `OctoBot-Tentacles-Manager-2.8.6/upload_tests/test_s3_uploader.py`

 * *Files identical despite different names*

