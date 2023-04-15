# Comparing `tmp/django-eveuniverse-0.9.0.tar.gz` & `tmp/django_eveuniverse-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-eveuniverse-0.9.0.tar", last modified: Thu Dec 30 21:08:56 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `django-eveuniverse-0.9.0.tar` & `django_eveuniverse-1.0.0a1.tar`

### file list

```diff
@@ -1,78 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-30 21:08:56.000000 django-eveuniverse-0.9.0/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2020-10-23 18:01:44.000000 django-eveuniverse-0.9.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      237 2020-12-15 20:22:38.000000 django-eveuniverse-0.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3408 2021-12-30 21:08:56.000000 django-eveuniverse-0.9.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2440 2021-04-16 13:52:39.000000 django-eveuniverse-0.9.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-30 21:08:55.000000 django-eveuniverse-0.9.0/django_eveuniverse.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3408 2021-12-30 21:08:55.000000 django-eveuniverse-0.9.0/django_eveuniverse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2117 2021-12-30 21:08:55.000000 django-eveuniverse-0.9.0/django_eveuniverse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-12-30 21:08:55.000000 django-eveuniverse-0.9.0/django_eveuniverse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       72 2021-12-30 21:08:55.000000 django-eveuniverse-0.9.0/django_eveuniverse.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2021-12-30 21:08:55.000000 django-eveuniverse-0.9.0/django_eveuniverse.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-30 21:08:55.000000 django-eveuniverse-0.9.0/eveuniverse/
--rw-rw-rw-   0 root         (0) root         (0)      108 2021-12-30 20:41:23.000000 django-eveuniverse-0.9.0/eveuniverse/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1314 2020-10-23 18:01:44.000000 django-eveuniverse-0.9.0/eveuniverse/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     2209 2021-07-03 13:22:11.000000 django-eveuniverse-0.9.0/eveuniverse/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      200 2021-04-16 13:44:19.000000 django-eveuniverse-0.9.0/eveuniverse/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      528 2021-12-30 20:41:23.000000 django-eveuniverse-0.9.0/eveuniverse/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-30 21:08:55.000000 django-eveuniverse-0.9.0/eveuniverse/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-10-23 18:01:44.000000 django-eveuniverse-0.9.0/eveuniverse/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2020-10-27 23:23:37.000000 django-eveuniverse-0.9.0/eveuniverse/core/esitools.py
--rw-rw-rw-   0 root         (0) root         (0)     4992 2020-12-28 20:25:37.000000 django-eveuniverse-0.9.0/eveuniverse/core/eveimageserver.py
--rw-rw-rw-   0 root         (0) root         (0)     2394 2021-12-30 20:41:23.000000 django-eveuniverse-0.9.0/eveuniverse/core/evemicros.py
--rw-rw-rw-   0 root         (0) root         (0)      409 2020-12-26 22:07:52.000000 django-eveuniverse-0.9.0/eveuniverse/core/eveskinserver.py
--rw-rw-rw-   0 root         (0) root         (0)     1348 2020-10-23 18:01:44.000000 django-eveuniverse-0.9.0/eveuniverse/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-30 21:08:55.000000 django-eveuniverse-0.9.0/eveuniverse/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-30 21:08:56.000000 django-eveuniverse-0.9.0/eveuniverse/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)      102 2020-10-23 18:01:44.000000 django-eveuniverse-0.9.0/eveuniverse/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2596 2021-04-16 13:44:19.000000 django-eveuniverse-0.9.0/eveuniverse/management/commands/eveuniverse_load_data.py
--rw-rw-rw-   0 root         (0) root         (0)     4470 2021-04-16 13:44:19.000000 django-eveuniverse-0.9.0/eveuniverse/management/commands/eveuniverse_load_types.py
--rw-rw-rw-   0 root         (0) root         (0)     1644 2021-04-16 13:44:19.000000 django-eveuniverse-0.9.0/eveuniverse/management/commands/eveuniverse_purge_data.py
--rw-rw-rw-   0 root         (0) root         (0)    36723 2021-11-15 20:28:57.000000 django-eveuniverse-0.9.0/eveuniverse/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-30 21:08:56.000000 django-eveuniverse-0.9.0/eveuniverse/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    51660 2021-04-16 13:44:19.000000 django-eveuniverse-0.9.0/eveuniverse/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      969 2020-10-23 18:01:44.000000 django-eveuniverse-0.9.0/eveuniverse/migrations/0002_load_eveunit.py
--rw-rw-rw-   0 root         (0) root         (0)     1010 2021-04-16 13:44:19.000000 django-eveuniverse-0.9.0/eveuniverse/migrations/0003_evemarketprice.py
--rw-rw-rw-   0 root         (0) root         (0)      479 2020-10-27 23:29:33.000000 django-eveuniverse-0.9.0/eveuniverse/migrations/0004_effect_longer_name.py
--rw-rw-rw-   0 root         (0) root         (0)     2704 2021-04-16 13:44:19.000000 django-eveuniverse-0.9.0/eveuniverse/migrations/0005_type_materials_and_sections.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-10-23 18:01:44.000000 django-eveuniverse-0.9.0/eveuniverse/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5336 2020-11-20 16:10:16.000000 django-eveuniverse-0.9.0/eveuniverse/migrations/eve_unit.json
--rw-rw-rw-   0 root         (0) root         (0)    56030 2021-12-30 20:41:23.000000 django-eveuniverse-0.9.0/eveuniverse/models.py
--rw-rw-rw-   0 root         (0) root         (0)      267 2021-04-16 13:44:19.000000 django-eveuniverse-0.9.0/eveuniverse/providers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-30 21:08:55.000000 django-eveuniverse-0.9.0/eveuniverse/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-30 21:08:56.000000 django-eveuniverse-0.9.0/eveuniverse/static/eveuniverse/
--rw-rw-rw-   0 root         (0) root         (0)    14542 2020-12-18 18:17:56.000000 django-eveuniverse-0.9.0/eveuniverse/static/eveuniverse/skin_generic_128.png
--rw-rw-rw-   0 root         (0) root         (0)     2142 2020-12-18 18:17:56.000000 django-eveuniverse-0.9.0/eveuniverse/static/eveuniverse/skin_generic_32.png
--rw-rw-rw-   0 root         (0) root         (0)     4141 2020-12-18 18:17:56.000000 django-eveuniverse-0.9.0/eveuniverse/static/eveuniverse/skin_generic_64.png
--rw-rw-rw-   0 root         (0) root         (0)     8329 2021-12-30 20:41:23.000000 django-eveuniverse-0.9.0/eveuniverse/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-30 21:08:56.000000 django-eveuniverse-0.9.0/eveuniverse/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-10-23 18:01:44.000000 django-eveuniverse-0.9.0/eveuniverse/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1274 2021-04-16 13:44:19.000000 django-eveuniverse-0.9.0/eveuniverse/tests/pilot.py
--rw-rw-rw-   0 root         (0) root         (0)     5947 2021-04-16 13:44:19.000000 django-eveuniverse-0.9.0/eveuniverse/tests/test_commands.py
--rw-rw-rw-   0 root         (0) root         (0)    11455 2021-12-30 20:41:23.000000 django-eveuniverse-0.9.0/eveuniverse/tests/test_core.py
--rw-rw-rw-   0 root         (0) root         (0)      859 2021-04-16 13:44:19.000000 django-eveuniverse-0.9.0/eveuniverse/tests/test_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    37330 2021-04-16 13:44:19.000000 django-eveuniverse-0.9.0/eveuniverse/tests/test_models_1.py
--rw-rw-rw-   0 root         (0) root         (0)    45692 2021-12-30 20:41:23.000000 django-eveuniverse-0.9.0/eveuniverse/tests/test_models_2.py
--rw-rw-rw-   0 root         (0) root         (0)    45528 2021-12-30 20:41:23.000000 django-eveuniverse-0.9.0/eveuniverse/tests/test_models_3.py
--rw-rw-rw-   0 root         (0) root         (0)     4739 2021-04-16 13:44:19.000000 django-eveuniverse-0.9.0/eveuniverse/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     2958 2021-04-16 13:44:19.000000 django-eveuniverse-0.9.0/eveuniverse/tests/test_tools_testdata.py
--rw-rw-rw-   0 root         (0) root         (0)     3977 2021-11-15 20:28:57.000000 django-eveuniverse-0.9.0/eveuniverse/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-30 21:08:56.000000 django-eveuniverse-0.9.0/eveuniverse/tests/testdata/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-02-21 19:32:52.000000 django-eveuniverse-0.9.0/eveuniverse/tests/testdata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6932 2021-11-15 20:28:57.000000 django-eveuniverse-0.9.0/eveuniverse/tests/testdata/esi.py
--rw-rw-rw-   0 root         (0) root         (0)     3714 2021-12-30 20:41:23.000000 django-eveuniverse-0.9.0/eveuniverse/tests/testdata/factories.py
--rw-rw-rw-   0 root         (0) root         (0)     1381 2021-04-16 13:44:19.000000 django-eveuniverse-0.9.0/eveuniverse/tests/testdata/fetch_esi_raw_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1175 2021-04-16 13:44:19.000000 django-eveuniverse-0.9.0/eveuniverse/tests/testdata/generate_sde.py
--rw-rw-rw-   0 root         (0) root         (0)      584 2021-04-16 13:44:19.000000 django-eveuniverse-0.9.0/eveuniverse/tests/testdata/sde.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-30 21:08:56.000000 django-eveuniverse-0.9.0/eveuniverse/tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-10-23 18:01:44.000000 django-eveuniverse-0.9.0/eveuniverse/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1373 2020-11-20 16:10:16.000000 django-eveuniverse-0.9.0/eveuniverse/tools/drop_tables.sql
--rw-rw-rw-   0 root         (0) root         (0)     5158 2021-04-16 13:44:19.000000 django-eveuniverse-0.9.0/eveuniverse/tools/testdata.py
--rw-rw-rw-   0 root         (0) root         (0)     2944 2021-11-15 20:28:57.000000 django-eveuniverse-0.9.0/eveuniverse/utils.py
--rw-r--r--   0 root         (0) root         (0)       38 2021-12-30 21:08:56.000000 django-eveuniverse-0.9.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1666 2021-10-17 20:48:17.000000 django-eveuniverse-0.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-30 21:08:56.000000 django-eveuniverse-0.9.0/testsite/
--rw-rw-rw-   0 root         (0) root         (0)       46 2020-10-23 18:01:44.000000 django-eveuniverse-0.9.0/testsite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      523 2021-04-16 13:44:19.000000 django-eveuniverse-0.9.0/testsite/celery.py
--rw-rw-rw-   0 root         (0) root         (0)     1314 2020-12-17 01:09:00.000000 django-eveuniverse-0.9.0/testsite/settings.py
--rw-rw-rw-   0 root         (0) root         (0)      688 2020-10-23 18:01:44.000000 django-eveuniverse-0.9.0/testsite/urls.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/__init__.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/admin.py
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/app_settings.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/apps.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/backends.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/constants.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/helpers.py
+-rw-r--r--   0        0        0    41499 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/managers.py
+-rw-r--r--   0        0        0    58930 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/models.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/providers.py
+-rw-r--r--   0        0        0   887006 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/swagger.json
+-rw-r--r--   0        0        0    10500 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tasks.py
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/core/__init__.py
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/core/dotlan.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/core/esitools.py
+-rw-r--r--   0        0        0     5036 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/core/eveimageserver.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/core/eveitems.py
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/core/evemicros.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/core/evesdeapi.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/core/eveskinserver.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/core/evewho.py
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/core/evexml.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/core/zkillboard.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/management/commands/__init__.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/management/commands/eveuniverse_load_data.py
+-rw-r--r--   0        0        0     5348 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/management/commands/eveuniverse_load_types.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/management/commands/eveuniverse_purge_data.py
+-rw-r--r--   0        0        0    51659 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/migrations/0001_initial.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/migrations/0002_load_eveunit.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/migrations/0003_evemarketprice.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/migrations/0004_effect_longer_name.py
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/migrations/0005_type_materials_and_sections.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/migrations/0006_alter_evedogmaeffectmodifier_operator.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/migrations/0007_evetype_description.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/migrations/__init__.py
+-rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/migrations/eve_unit.json
+-rw-r--r--   0        0        0    14542 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/static/eveuniverse/skin_generic_128.png
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/static/eveuniverse/skin_generic_32.png
+-rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/static/eveuniverse/skin_generic_64.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/__init__.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/pilot.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/test_backends.py
+-rw-r--r--   0        0        0    10286 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/test_commands.py
+-rw-r--r--   0        0        0    22388 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/test_core.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/test_helpers.py
+-rw-r--r--   0        0        0    42399 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/test_models_1.py
+-rw-r--r--   0        0        0    28631 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/test_models_2.py
+-rw-r--r--   0        0        0    43206 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/test_models_3.py
+-rw-r--r--   0        0        0    30849 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/test_models_4.py
+-rw-r--r--   0        0        0     6759 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/test_tasks.py
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/test_tools_testdata.py
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/test_utils.py
+-rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata_example.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata/__init__.py
+-rw-r--r--   0        0        0     7725 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata/esi.py
+-rw-r--r--   0        0        0    78321 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata/esi_data.json
+-rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata/factories.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata/fetch_esi_raw_data.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata/generate_sde.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata/sde.py
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata/sde_data.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/tools/__init__.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/tools/clear_celery_once_locks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tools/__init__.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tools/drop_tables.sql
+-rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tools/testdata.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/LICENSE
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/README.md
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-eveuniverse-0.9.0/LICENSE` & `django_eveuniverse-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-eveuniverse-0.9.0/PKG-INFO` & `django_eveuniverse-1.0.0a1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,64 @@
 Metadata-Version: 2.1
 Name: django-eveuniverse
-Version: 0.9.0
+Version: 1.0.0a1
 Summary: Complete set of Eve Universe models with on-demand loading from ESI
-Home-page: https://gitlab.com/ErikKalkoken/django-eveuniverse
-Author: Erik Kalkoken
-Author-email: kalkoken87@gmail.com
-License: MIT
-Platform: UNKNOWN
+Project-URL: Homepage, https://gitlab.com/ErikKalkoken/django-eveuniverse
+Author-email: Erik Kalkoken <kalkoken87@gmail.com>
+License-Expression: MIT
+License-File: LICENSE
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: ~=3.6
+Requires-Python: ~=3.8
+Requires-Dist: celery-once>=3.0.1
+Requires-Dist: celery>=4.0.2
+Requires-Dist: django-bitfield>=2.2
+Requires-Dist: django-esi<5,>=4
+Requires-Dist: django>=3.2
+Requires-Dist: requests
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Eve Universe
 
 Complete set of Eve Online Universe models in Django with on-demand loading from ESI
 
 [![release](https://img.shields.io/pypi/v/django-eveuniverse?label=release)](https://pypi.org/project/django-eveuniverse/)
 [![python](https://img.shields.io/pypi/pyversions/django-eveuniverse)](https://pypi.org/project/django-eveuniverse/)
 [![django](https://img.shields.io/pypi/djversions/django-eveuniverse?label=django)](https://pypi.org/project/django-eveuniverse/)
 [![pipeline](https://gitlab.com/ErikKalkoken/django-eveuniverse/badges/master/pipeline.svg)](https://gitlab.com/ErikKalkoken/django-eveuniverse/-/pipelines)
 [![codecov](https://codecov.io/gl/ErikKalkoken/django-eveuniverse/branch/master/graph/badge.svg?token=YZF6RVSK0P)](https://codecov.io/gl/ErikKalkoken/django-eveuniverse)
+[![Documentation Status](https://readthedocs.org/projects/django-eveuniverse/badge/?version=latest)](https://django-eveuniverse.readthedocs.io/en/latest/?badge=latest)
 [![license](https://img.shields.io/badge/license-MIT-green)](https://gitlab.com/ErikKalkoken/django-eveuniverse/-/blob/master/LICENSE)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![chat](https://img.shields.io/discord/790364535294132234)](https://discord.gg/zmh52wnfvM)
 
 ## Overview
 
 *django-eveuniverse* is a foundation app meant to help speed up the development of Eve Online apps with Django and ESI. It provides all classic "static" Eve classes as Django models, including all relationships, ready to be used in your project. Furthermore, all Eve models have an on-demand loading mechanism for fetching new objects from ESI.
 
 Here is an overview of the main features:
 
-- Complete set of Eve Universe objects as Django models like regions, types or planets.
+- Complete set of ESI's Eve Universe objects as Django models like regions, types or planets.
 - On-demand loading mechanism that allows retrieving Eve universe objects ad-hoc from ESI
 - Management commands for preloading often used sets of data like the map or ships types
 - Eve models come with additional useful features, e.g. a route finder between solar systems or image URLs for types
 - Special model EveEntity for quickly resolving Eve Online IDs to names
 - Optional asynchronous loading of eve models and loading of all related children. (e.g. load all types for a specific group)
+- Additional models for selected data from the SDE that is not covered by ESI, e.g. type materials
 
 ## Documentation
 
 For details on how to install and use *django-eveuniverse* please see the [documentation](https://django-eveuniverse.readthedocs.io/en/latest/).
-
-
```

### Comparing `django-eveuniverse-0.9.0/README.md` & `django_eveuniverse-1.0.0a1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 Complete set of Eve Online Universe models in Django with on-demand loading from ESI
 
 [![release](https://img.shields.io/pypi/v/django-eveuniverse?label=release)](https://pypi.org/project/django-eveuniverse/)
 [![python](https://img.shields.io/pypi/pyversions/django-eveuniverse)](https://pypi.org/project/django-eveuniverse/)
 [![django](https://img.shields.io/pypi/djversions/django-eveuniverse?label=django)](https://pypi.org/project/django-eveuniverse/)
 [![pipeline](https://gitlab.com/ErikKalkoken/django-eveuniverse/badges/master/pipeline.svg)](https://gitlab.com/ErikKalkoken/django-eveuniverse/-/pipelines)
 [![codecov](https://codecov.io/gl/ErikKalkoken/django-eveuniverse/branch/master/graph/badge.svg?token=YZF6RVSK0P)](https://codecov.io/gl/ErikKalkoken/django-eveuniverse)
+[![Documentation Status](https://readthedocs.org/projects/django-eveuniverse/badge/?version=latest)](https://django-eveuniverse.readthedocs.io/en/latest/?badge=latest)
 [![license](https://img.shields.io/badge/license-MIT-green)](https://gitlab.com/ErikKalkoken/django-eveuniverse/-/blob/master/LICENSE)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![chat](https://img.shields.io/discord/790364535294132234)](https://discord.gg/zmh52wnfvM)
 
 ## Overview
 
 *django-eveuniverse* is a foundation app meant to help speed up the development of Eve Online apps with Django and ESI. It provides all classic "static" Eve classes as Django models, including all relationships, ready to be used in your project. Furthermore, all Eve models have an on-demand loading mechanism for fetching new objects from ESI.
 
 Here is an overview of the main features:
 
-- Complete set of Eve Universe objects as Django models like regions, types or planets.
+- Complete set of ESI's Eve Universe objects as Django models like regions, types or planets.
 - On-demand loading mechanism that allows retrieving Eve universe objects ad-hoc from ESI
 - Management commands for preloading often used sets of data like the map or ships types
 - Eve models come with additional useful features, e.g. a route finder between solar systems or image URLs for types
 - Special model EveEntity for quickly resolving Eve Online IDs to names
 - Optional asynchronous loading of eve models and loading of all related children. (e.g. load all types for a specific group)
+- Additional models for selected data from the SDE that is not covered by ESI, e.g. type materials
 
 ## Documentation
 
 For details on how to install and use *django-eveuniverse* please see the [documentation](https://django-eveuniverse.readthedocs.io/en/latest/).
```

### Comparing `django-eveuniverse-0.9.0/eveuniverse/admin.py` & `django_eveuniverse-1.0.0a1/eveuniverse/admin.py`

 * *Files identical despite different names*

### Comparing `django-eveuniverse-0.9.0/eveuniverse/app_settings.py` & `django_eveuniverse-1.0.0a1/eveuniverse/app_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from .utils import clean_setting
 
 EVEUNIVERSE_BULK_METHODS_BATCH_SIZE = clean_setting(
     "EVEUNIVERSE_BULK_METHODS_BATCH_SIZE", 500
 )
-# Technical parameter defining the maximum number of objects processed per run
-# of Django batch methods, e.g. bulk_create and bulk_update
+"""Technical parameter defining the maximum number of objects processed per run
+of Django batch methods, e.g. bulk_create and bulk_update.
+"""
 
+EVEUNIVERSE_ZZEVE_SDE_URL = clean_setting(
+    "EVEUNIVERSE_ZZEVE_SDE_URL", "https://sde.eve-o.tech/latest"
+)
+"""URL to a web site providing the SDE tables as JSON files."""
 
 EVEUNIVERSE_LOAD_ASTEROID_BELTS = clean_setting(
     "EVEUNIVERSE_LOAD_ASTEROID_BELTS", False
 )
 """When true will automatically load astroid belts with every solar system."""
 
 EVEUNIVERSE_LOAD_DOGMAS = clean_setting("EVEUNIVERSE_LOAD_DOGMAS", False)
@@ -37,14 +42,26 @@
 """When true will automatically load stations be with every solar system."""
 
 EVEUNIVERSE_LOAD_TYPE_MATERIALS = clean_setting(
     "EVEUNIVERSE_LOAD_TYPE_MATERIALS", False
 )
 """When true will automatically load type materials be with every type."""
 
+EVEUNIVERSE_LOAD_TASKS_PRIORITY = clean_setting("EVEUNIVERSE_LOAD_TASKS_PRIORITY", 6)
+"""Priority of tasks for data loads.
+This priority should be below 5 to not interfere with normal task operation.
+"""
+
+EVEUNIVERSE_REQUESTS_DEFAULT_TIMEOUT = clean_setting(
+    "EVEUNIVERSE_REQUESTS_DEFAULT_TIMEOUT", 5
+)
+"""Default timeout for HTTP GET requests in seconds."""
+
+
 EVEUNIVERSE_TASKS_TIME_LIMIT = clean_setting("EVEUNIVERSE_TASKS_TIME_LIMIT", 7200)
 """Global timeout for tasks in seconds to reduce task accumulation during outages."""
 
+
 EVEUNIVERSE_USE_EVESKINSERVER = clean_setting("EVEUNIVERSE_USE_EVESKINSERVER", True)
 """When True a call to EveType.icon_url for a SKIN type will return a eveskinserver URL
 else it will return a generic SKIN icon.
 """
```

### Comparing `django-eveuniverse-0.9.0/eveuniverse/core/eveimageserver.py` & `django_eveuniverse-1.0.0a1/eveuniverse/core/eveimageserver.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Fetching image URLs for Eve objects."""
+
 import enum
 
 _EVE_IMAGE_SERVER_URL = "https://images.evetech.net"
 _DEFAULT_IMAGE_SIZE = 32
 
 
 class EsiCategory(enum.Enum):
```

### Comparing `django-eveuniverse-0.9.0/eveuniverse/core/evemicros.py` & `django_eveuniverse-1.0.0a1/eveuniverse/core/evemicros.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,30 @@
-"""Wrapper to access evemicros API"""
-from collections import namedtuple
+"""Wrapper to access evemicros API."""
+
+from dataclasses import dataclass
 from typing import Optional
 from urllib.parse import urlencode
 
 import requests
-
 from django.core.cache import cache
 
+from eveuniverse.app_settings import EVEUNIVERSE_REQUESTS_DEFAULT_TIMEOUT
+
 _CACHE_TIMEOUT = 3_600 * 12
 _BASE_URL = "https://www.kalkoken.org/apps/evemicros/eveUniverse.php"
 
-EveItem = namedtuple("EveItem", ["id", "name", "type_id", "distance"])
+
+@dataclass
+class EveItem:
+    """A celestial item."""
+
+    id: int
+    name: str
+    type_id: int
+    distance: float
 
 
 def nearest_celestial(
     solar_system_id: int, x: int, y: int, z: int, group_id: int = None
 ) -> Optional[EveItem]:
     """Fetch nearest celestial to given coordinates from API. Results are cached.
 
@@ -42,15 +52,17 @@
     Returns None if data from API does not have expected structure.
     """
     params = map(str, map(int, [solar_system_id, x, y, z]))
     query = urlencode({"nearestCelestials": ",".join(params)})
     cache_key = f"EVEUNIVERSE_NEAREST_CELESTIAL_{query}"
     result = cache.get(key=cache_key)
     if not result:
-        r = requests.get(f"{_BASE_URL}?{query}")
+        r = requests.get(
+            f"{_BASE_URL}?{query}", timeout=EVEUNIVERSE_REQUESTS_DEFAULT_TIMEOUT
+        )
         r.raise_for_status()
         data = r.json()
         if "ok" not in data or not data["ok"] or "result" not in data:
             return None
         result = data["result"]
         cache.set(key=cache_key, value=result, timeout=_CACHE_TIMEOUT)
     return result
```

### Comparing `django-eveuniverse-0.9.0/eveuniverse/helpers.py` & `django_eveuniverse-1.0.0a1/eveuniverse/helpers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Dict, Optional
+import hashlib
+import json
+from typing import Any, Dict, Optional
 
 from django.db import models
 
 
 def meters_to_ly(value: float) -> float:
     """converts meters into lightyears"""
     return float(value) / 9_460_730_472_580_800 if value is not None else None
@@ -47,7 +49,15 @@
         """
         try:
             name = self._names_map[id]
         except KeyError:
             name = ""
 
         return name
+
+
+def dict_hash(dictionary: Dict[str, Any]) -> str:
+    """SHA256 hash of a dictionary."""
+    my_hash = hashlib.sha256()
+    encoded = json.dumps(dictionary, sort_keys=True).encode(encoding="utf8")
+    my_hash.update(encoded)
+    return my_hash.hexdigest()
```

### Comparing `django-eveuniverse-0.9.0/eveuniverse/management/commands/eveuniverse_load_types.py` & `django_eveuniverse-1.0.0a1/eveuniverse/management/commands/eveuniverse_load_types.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import logging
 
 from django.core.management.base import BaseCommand
 
-from ... import __title__
-from ...core.esitools import is_esi_online
-from ...tasks import _eve_object_names_to_be_loaded, load_eve_types
-from ...utils import LoggerAddTag
-from . import get_input
+from eveuniverse import __title__, tasks
+from eveuniverse.core.esitools import is_esi_online
+from eveuniverse.models import EveUniverseEntityModel
+from eveuniverse.utils import LoggerAddTag
+
+from . import EXPECTATION_TEXT, get_input
 
 logger = LoggerAddTag(logging.getLogger(__name__), __title__)
 
 
 class Command(BaseCommand):
     help = (
         "Loads large sets of types as specified from ESI into the local database."
@@ -56,16 +57,30 @@
             help="Eve type ID to be loaded  incl. dogma",
         )
         parser.add_argument(
             "--disable_esi_check",
             action="store_true",
             help="Disables checking that ESI is online",
         )
+        parser.add_argument(
+            "--noinput",
+            "--no-input",
+            action="store_true",
+            help="Do NOT prompt the user for input of any kind.",
+        )
+
+    def write_to_be_loaded(self, name, *items):
+        items_count = sum_items(*items)
+        if items_count:
+            self.stdout.write(f"{name} to be loaded: {items_count}")
 
     def handle(self, *args, **options):
+        self.stdout.write("Eve Universe - Types Loader")
+        self.stdout.write("===========================")
+
         app_name = options["app_name"]
         category_ids = options["category_id"]
         category_ids_with_dogma = options["category_id_with_dogma"]
         group_ids = options["group_id"]
         group_ids_with_dogma = options["group_id_with_dogma"]
         type_ids = options["type_id"]
         type_ids_with_dogma = options["type_id_with_dogma"]
@@ -77,47 +92,58 @@
             and not group_ids_with_dogma
             and not type_ids
             and not type_ids_with_dogma
         ):
             self.stdout.write(self.style.WARNING("No IDs specified. Nothing to do."))
             return
 
-        self.stdout.write("Eve Universe - Types Loader")
-        self.stdout.write("===========================")
-
+        self.stdout.write("Checking ESI...", ending="")
         if not options["disable_esi_check"] and not is_esi_online():
             self.stdout.write(
                 "ESI does not appear to be online at this time. Please try again later."
             )
             self.stdout.write(self.style.WARNING("Aborted"))
             return
-
+        self.stdout.write("ONLINE")
         self.stdout.write(
             f"This command will start loading data for the app: {app_name}."
         )
-        additional_objects = _eve_object_names_to_be_loaded()
+        self.write_to_be_loaded("Categories", category_ids, category_ids_with_dogma)
+        self.write_to_be_loaded("Groups", group_ids, group_ids)
+        self.write_to_be_loaded("Types", type_ids, type_ids_with_dogma)
+        additional_objects = list(EveUniverseEntityModel.determine_effective_sections())
         if additional_objects:
             self.stdout.write(
                 "It will also load the following additional entities when related to "
                 "objects loaded for the app: "
                 f"{','.join(additional_objects)}"
             )
-        self.stdout.write(
-            "Note that this process can take a while to complete "
-            "and may cause some significant load to your system."
-        )
-        user_input = get_input("Are you sure you want to proceed? (y/N)?")
-        if user_input.lower() == "y":
+        self.stdout.write(EXPECTATION_TEXT)
+        if not options["noinput"]:
+            user_input = get_input("Are you sure you want to proceed? (Y/n)? ")
+        else:
+            user_input = "y"
+        if user_input.lower() != "n":
             if category_ids or group_ids or type_ids:
-                load_eve_types.delay(
+                tasks.load_eve_types.delay(
                     category_ids=category_ids, group_ids=group_ids, type_ids=type_ids
                 )
             if category_ids_with_dogma or group_ids_with_dogma or type_ids_with_dogma:
-                load_eve_types.delay(
+                tasks.load_eve_types.delay(
                     category_ids=category_ids_with_dogma,
                     group_ids=group_ids_with_dogma,
                     type_ids=type_ids_with_dogma,
                     force_loading_dogma=True,
                 )
-            self.stdout.write(self.style.SUCCESS("Data loading has been started!"))
+            self.stdout.write(self.style.SUCCESS("Data load started!"))
         else:
             self.stdout.write(self.style.WARNING("Aborted"))
+
+
+def sum_items(*items) -> len:
+    total = 0
+    for item in items:
+        try:
+            total += len(item)
+        except TypeError:
+            pass
+    return total
```

### Comparing `django-eveuniverse-0.9.0/eveuniverse/management/commands/eveuniverse_purge_data.py` & `django_eveuniverse-1.0.0a1/eveuniverse/management/commands/eveuniverse_purge_data.py`

 * *Files identical despite different names*

### Comparing `django-eveuniverse-0.9.0/eveuniverse/managers.py` & `django_eveuniverse-1.0.0a1/eveuniverse/managers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import datetime as dt
 import logging
-from collections import namedtuple
+from collections import defaultdict, namedtuple
 from typing import Iterable, List, Optional, Set, Tuple
-from urllib.parse import urljoin
 
 import requests
 from bravado.exception import HTTPNotFound
-
 from django.core.cache import cache
 from django.db import models, transaction
 from django.db.utils import IntegrityError
 from django.utils.timezone import now
 
 from . import __title__
-from .app_settings import EVEUNIVERSE_BULK_METHODS_BATCH_SIZE
+from .app_settings import (
+    EVEUNIVERSE_BULK_METHODS_BATCH_SIZE,
+    EVEUNIVERSE_REQUESTS_DEFAULT_TIMEOUT,
+    EVEUNIVERSE_ZZEVE_SDE_URL,
+)
+from .constants import POST_UNIVERSE_NAMES_MAX_ITEMS
 from .helpers import EveEntityNameResolver, get_or_create_esi_or_none
 from .providers import esi
-from .utils import LoggerAddTag, chunks, make_logger_prefix
+from .utils import LoggerAddTag, chunks
 
 logger = LoggerAddTag(logging.getLogger(__name__), __title__)
 
 FakeResponse = namedtuple("FakeResponse", ["status_code"])
 
-SDE_ZZEVE_URL = "https://sde.zzeve.com"
-
 
 class EveUniverseBaseModelManager(models.Manager):
     def _defaults_from_esi_obj(
         self, eve_data_obj: dict, enabled_sections: Set[str] = None
     ) -> dict:
         """compiles defaults from an esi data object for update/creating the model"""
         defaults = dict()
@@ -81,41 +82,44 @@
     def get_or_create_esi(
         self,
         *,
         id: int,
         include_children: bool = False,
         wait_for_children: bool = True,
         enabled_sections: Iterable[str] = None,
+        task_priority: int = None,
     ) -> Tuple[models.Model, bool]:
         """gets or creates an eve universe object.
 
         The object is automatically fetched from ESI if it does not exist (blocking).
         Will always get/create parent objects.
 
         Args:
             id: Eve Online ID of object
             include_children: if child objects should be updated/created as well (only when a new object is created)
             wait_for_children: when true child objects will be updated/created blocking (if any), else async (only when a new object is created)
             enabled_sections: Sections to load regardless of current settings, e.g. `[EveType.Section.DOGMAS]` will always load dogmas for EveTypes
+            task_priority: priority of started tasks
 
         Returns:
             A tuple consisting of the requested object and a created flag
         """
         id = int(id)
-        enabled_sections = self.model._enabled_sections_union(enabled_sections)
+        enabled_sections = self.model.determine_effective_sections(enabled_sections)
         try:
             enabled_sections_filter = self._enabled_sections_filter(enabled_sections)
             obj = self.filter(**enabled_sections_filter).get(id=id)
             return obj, False
         except self.model.DoesNotExist:
             return self.update_or_create_esi(
                 id=id,
                 include_children=include_children,
                 wait_for_children=wait_for_children,
                 enabled_sections=enabled_sections,
+                task_priority=task_priority,
             )
 
     def _enabled_sections_filter(self, enabled_sections: Iterable[str]) -> dict:
         return {
             "enabled_sections": getattr(self.model.enabled_sections, section)
             for section in enabled_sections
             if str(section) in self.model.Section.values()
@@ -124,83 +128,77 @@
     def update_or_create_esi(
         self,
         *,
         id: int,
         include_children: bool = False,
         wait_for_children: bool = True,
         enabled_sections: Iterable[str] = None,
+        task_priority: int = None,
     ) -> Tuple[models.Model, bool]:
         """updates or creates an Eve universe object by fetching it from ESI (blocking).
         Will always get/create parent objects
 
         Args:
             id: Eve Online ID of object
             include_children: if child objects should be updated/created as well (if any)
             wait_for_children: when true child objects will be updated/created blocking (if any), else async
             enabled_sections: Sections to load regardless of current settings, e.g. `[EveType.Section.DOGMAS]` will always load dogmas for EveTypes
+            task_priority: priority of started tasks
 
         Returns:
             A tuple consisting of the requested object and a created flag
         """
         id = int(id)
-        add_prefix = make_logger_prefix("%s(id=%s)" % (self.model.__name__, id))
-        enabled_sections = self.model._enabled_sections_union(enabled_sections)
-        try:
-            eve_data_obj = self._transform_esi_response_for_list_endpoints(
-                id, self._fetch_from_esi(id=id, enabled_sections=enabled_sections)
-            )
-            if eve_data_obj:
-                defaults = self._defaults_from_esi_obj(eve_data_obj, enabled_sections)
-                obj, created = self.update_or_create(id=id, defaults=defaults)
-                if enabled_sections and hasattr(obj, "enabled_sections"):
-                    updated_sections = False
-                    for section in enabled_sections:
-                        if str(section) in self.model.Section.values():
-                            setattr(obj.enabled_sections, section, True)
-                            updated_sections = True
-                    if updated_sections:
-                        obj.save()
-                inline_objects = self.model._inline_objects(enabled_sections)
-                if inline_objects:
-                    self._update_or_create_inline_objects(
-                        parent_eve_data_obj=eve_data_obj,
-                        parent_obj=obj,
-                        inline_objects=inline_objects,
-                        wait_for_children=wait_for_children,
-                        enabled_sections=enabled_sections,
-                    )
-                if include_children:
-                    self._update_or_create_children(
-                        parent_eve_data_obj=eve_data_obj,
-                        include_children=include_children,
-                        wait_for_children=wait_for_children,
-                        enabled_sections=enabled_sections,
-                    )
-            else:
-                raise HTTPNotFound(
-                    FakeResponse(status_code=404),
-                    message=f"{self.model.__name__} object with id {id} not found",
+        enabled_sections = self.model.determine_effective_sections(enabled_sections)
+        eve_data_obj = self._transform_esi_response_for_list_endpoints(
+            id, self._fetch_from_esi(id=id, enabled_sections=enabled_sections)
+        )
+        if eve_data_obj:
+            defaults = self._defaults_from_esi_obj(eve_data_obj, enabled_sections)
+            obj, created = self.update_or_create(id=id, defaults=defaults)
+            if enabled_sections and hasattr(obj, "enabled_sections"):
+                updated_sections = False
+                for section in enabled_sections:
+                    if str(section) in self.model.Section.values():
+                        setattr(obj.enabled_sections, section, True)
+                        updated_sections = True
+                if updated_sections:
+                    obj.save()
+            inline_objects = self.model._inline_objects(enabled_sections)
+            if inline_objects:
+                self._update_or_create_inline_objects(
+                    parent_eve_data_obj=eve_data_obj,
+                    parent_obj=obj,
+                    inline_objects=inline_objects,
+                    wait_for_children=wait_for_children,
+                    enabled_sections=enabled_sections,
+                    task_priority=task_priority,
                 )
-
-        except Exception as ex:
-            logger.warn(
-                add_prefix("Failed to update or create: %s" % ex),
-                exc_info=True,
+            if include_children:
+                self._update_or_create_children(
+                    parent_eve_data_obj=eve_data_obj,
+                    include_children=include_children,
+                    wait_for_children=wait_for_children,
+                    enabled_sections=enabled_sections,
+                    task_priority=task_priority,
+                )
+        else:
+            raise HTTPNotFound(
+                FakeResponse(status_code=404),
+                message=f"{self.model.__name__} object with id {id} not found",
             )
-            raise ex
-
         return obj, created
 
     def _fetch_from_esi(
         self, id: int = None, enabled_sections: Iterable[str] = None
     ) -> dict:
         """make request to ESI and return response data.
         Can handle raw ESI response from both list and normal endpoints.
         """
-        if id and not self.model._is_list_only_endpoint():
+        if id is not None and not self.model._is_list_only_endpoint():
             args = {self.model._esi_pk(): id}
         else:
             args = dict()
         category, method = self.model._esi_path_object()
         esi_data = getattr(
             getattr(esi.client, category),
             method,
@@ -229,14 +227,15 @@
         self,
         *,
         parent_eve_data_obj: dict,
         parent_obj: models.Model,
         inline_objects: dict,
         wait_for_children: bool,
         enabled_sections: Iterable[str],
+        task_priority: int = None,
     ) -> None:
         """updates_or_creates eve objects that are returned "inline" from ESI
         for the parent eve objects as defined for this parent model (if any)
         """
         from .tasks import (
             update_or_create_inline_object as task_update_or_create_inline_object,
         )
@@ -289,24 +288,29 @@
                             eve_data_obj=eve_data_obj,
                             other_pk_info=other_pk_info,
                             parent2_model_name=parent2_model_name,
                             inline_model_name=model_name,
                             enabled_sections=enabled_sections,
                         )
                     else:
-                        task_update_or_create_inline_object(
-                            parent_obj_id=parent_obj.id,
-                            parent_fk=parent_fk,
-                            eve_data_obj=eve_data_obj,
-                            other_pk_info=other_pk_info,
-                            parent2_model_name=parent2_model_name,
-                            inline_model_name=model_name,
-                            parent_model_name=type(parent_obj).__name__,
-                            enabled_sections=list(enabled_sections),
-                        )
+                        params = {
+                            "kwargs": {
+                                "parent_obj_id": parent_obj.id,
+                                "parent_fk": parent_fk,
+                                "eve_data_obj": eve_data_obj,
+                                "other_pk_info": other_pk_info,
+                                "parent2_model_name": parent2_model_name,
+                                "inline_model_name": model_name,
+                                "parent_model_name": type(parent_obj).__name__,
+                                "enabled_sections": list(enabled_sections),
+                            }
+                        }
+                        if task_priority:
+                            params["priority"] = task_priority
+                        task_update_or_create_inline_object.apply_async(**params)
 
     def _update_or_create_inline_object(
         self,
         parent_obj_id: int,
         parent_fk: str,
         eve_data_obj: dict,
         other_pk_info: dict,
@@ -342,14 +346,15 @@
     def _update_or_create_children(
         self,
         *,
         parent_eve_data_obj: dict,
         include_children: bool,
         wait_for_children: bool,
         enabled_sections: Iterable[str] = None,
+        task_priority: int = None,
     ) -> None:
         """updates or creates child objects as defined for this parent model (if any)"""
         from .tasks import (
             update_or_create_eve_object as task_update_or_create_eve_object,
         )
 
         if not parent_eve_data_obj:
@@ -366,61 +371,64 @@
                     if wait_for_children:
                         ChildClass = self.model.get_model_class(child_class)
                         ChildClass.objects.update_or_create_esi(
                             id=id,
                             include_children=include_children,
                             wait_for_children=wait_for_children,
                             enabled_sections=enabled_sections,
+                            task_priority=task_priority,
                         )
 
                     else:
-                        task_update_or_create_eve_object.delay(
-                            child_class,
-                            id,
-                            include_children=include_children,
-                            wait_for_children=wait_for_children,
-                            enabled_sections=list(enabled_sections),
-                        )
+                        params = {
+                            "kwargs": {
+                                "model_name": child_class,
+                                "id": id,
+                                "include_children": include_children,
+                                "wait_for_children": wait_for_children,
+                                "enabled_sections": list(enabled_sections),
+                                "task_priority": task_priority,
+                            },
+                        }
+                        if task_priority:
+                            params["priority"] = task_priority
+                        task_update_or_create_eve_object.apply_async(**params)
 
     def update_or_create_all_esi(
         self,
         *,
         include_children: bool = False,
         wait_for_children: bool = True,
         enabled_sections: Iterable[str] = None,
+        task_priority: int = None,
     ) -> None:
         """updates or creates all objects of this class from ESI.
 
         Loading all objects can take a long time. Use with care!
 
         Args:
             include_children: if child objects should be updated/created as well (if any)
             wait_for_children: when false all objects will be loaded async, else blocking
             enabled_sections: Sections to load regardless of current settings
         """
-        from .tasks import update_or_create_eve_object
+        from .tasks import (
+            update_or_create_eve_object as task_update_or_create_eve_object,
+        )
 
-        add_prefix = make_logger_prefix(f"{self.model.__name__}")
-        enabled_sections = self.model._enabled_sections_union(enabled_sections)
-        if self.model._is_list_only_endpoint():
-            try:
-                esi_pk = self.model._esi_pk()
-                for eve_data_obj in self._fetch_from_esi():
-                    args = {"id": eve_data_obj[esi_pk]}
-                    args["defaults"] = self._defaults_from_esi_obj(
-                        eve_data_obj=eve_data_obj, enabled_sections=enabled_sections
-                    )
-                    self.update_or_create(**args)
+        enabled_sections = self.model.determine_effective_sections(enabled_sections)
 
-            except Exception as ex:
-                logger.warn(
-                    add_prefix("Failed to update or create: %s" % ex),
-                    exc_info=True,
+        if self.model._is_list_only_endpoint():
+            esi_pk = self.model._esi_pk()
+            for eve_data_obj in self._fetch_from_esi():
+                args = {"id": eve_data_obj[esi_pk]}
+                args["defaults"] = self._defaults_from_esi_obj(
+                    eve_data_obj=eve_data_obj, enabled_sections=enabled_sections
                 )
-                raise ex
+                self.update_or_create(**args)
+
         else:
             if self.model._has_esi_path_list():
                 category, method = self.model._esi_path_list()
                 ids = getattr(
                     getattr(esi.client, category),
                     method,
                 )().results()
@@ -429,33 +437,41 @@
                         self.update_or_create_esi(
                             id=id,
                             include_children=include_children,
                             wait_for_children=wait_for_children,
                             enabled_sections=enabled_sections,
                         )
                     else:
-                        update_or_create_eve_object.delay(
-                            model_name=self.model.__name__,
-                            id=id,
-                            include_children=include_children,
-                            wait_for_children=wait_for_children,
-                            enabled_sections=list(enabled_sections),
-                        )
+                        params = {
+                            "kwargs": {
+                                "model_name": self.model.__name__,
+                                "id": id,
+                                "include_children": include_children,
+                                "wait_for_children": wait_for_children,
+                                "enabled_sections": list(enabled_sections),
+                                "task_priority": task_priority,
+                            },
+                        }
+                        if task_priority:
+                            params["priority"] = task_priority
+                        task_update_or_create_eve_object.apply_async(**params)
+
             else:
                 raise TypeError(
                     f"ESI does not provide a list endpoint for {self.model.__name__}"
                 )
 
     def bulk_get_or_create_esi(
         self,
         *,
         ids: List[int],
         include_children: bool = False,
         wait_for_children: bool = True,
         enabled_sections: Iterable[str] = None,
+        task_priority: int = None,
     ) -> models.QuerySet:
         """Gets or creates objects in bulk.
 
         Nonexisting objects will be fetched from ESI (blocking).
         Will always get/create parent objects.
 
         Args:
@@ -464,27 +480,28 @@
             wait_for_children: when true child objects will be updated/created blocking (if any), else async
             enabled_sections: Sections to load regardless of current settings
 
         Returns:
             Queryset with all requested eve objects
         """
         ids = set(map(int, ids))
-        enabled_sections = self.model._enabled_sections_union(enabled_sections)
+        enabled_sections = self.model.determine_effective_sections(enabled_sections)
         enabled_sections_filter = self._enabled_sections_filter(enabled_sections)
         existing_ids = set(
             self.filter(id__in=ids)
             .filter(**enabled_sections_filter)
             .values_list("id", flat=True)
         )
         for id in ids.difference(existing_ids):
             self.update_or_create_esi(
                 id=int(id),
                 include_children=include_children,
                 wait_for_children=wait_for_children,
                 enabled_sections=enabled_sections,
+                task_priority=task_priority,
             )
 
         return self.filter(id__in=ids)
 
 
 class EvePlanetManager(EveUniverseEntityModelManager):
     def _fetch_from_esi(self, id: int, enabled_sections: Iterable[str] = None) -> dict:
@@ -524,15 +541,15 @@
         super().__init__()
         self._my_property_name = None
 
     def _fetch_from_esi(self, id: int, enabled_sections: Iterable[str] = None) -> dict:
         from .models import EveSolarSystem
 
         if not self._my_property_name:
-            raise RuntimeWarning("my_property_name not initialzed")
+            raise RuntimeWarning("my_property_name not initialized")
 
         esi_data = super()._fetch_from_esi(id=id)
         if "system_id" not in esi_data:
             raise ValueError("system_id not found in moon response - data error")
 
         system_id = esi_data["system_id"]
         solar_system_data = EveSolarSystem.objects._fetch_from_esi(id=system_id)
@@ -572,14 +589,15 @@
     def update_or_create_esi(
         self,
         *,
         id: int,
         include_children: bool = False,
         wait_for_children: bool = True,
         enabled_sections: Iterable[str] = None,
+        task_priority: int = None,
     ) -> Tuple[models.Model, bool]:
         """updates or creates an EveStargate object by fetching it from ESI (blocking).
         Will always get/create parent objects
 
         Args:
             id: Eve Online ID of object
             include_children: (no effect)
@@ -588,14 +606,15 @@
         Returns:
             A tuple consisting of the requested object and a created flag
         """
         obj, created = super().update_or_create_esi(
             id=int(id),
             include_children=include_children,
             wait_for_children=wait_for_children,
+            task_priority=task_priority,
         )
         if obj:
             if obj.destination_eve_stargate is not None:
                 obj.destination_eve_stargate.destination_eve_stargate = obj
 
                 if obj.eve_solar_system is not None:
                     obj.destination_eve_stargate.destination_eve_solar_system = (
@@ -613,14 +632,15 @@
         self,
         *,
         parent_eve_data_obj: dict,
         parent_obj: models.Model,
         inline_objects: dict,
         wait_for_children: bool,
         enabled_sections: Iterable[str],
+        task_priority: int = None,
     ) -> None:
         """updates_or_creates station service objects for EveStations"""
         from .models import EveStationService
 
         if "services" in parent_eve_data_obj:
             services = list()
             for service_name in parent_eve_data_obj["services"]:
@@ -635,90 +655,64 @@
     def update_or_create_esi(
         self,
         *,
         id: int,
         include_children: bool = False,
         wait_for_children: bool = True,
         enabled_sections: Iterable[str] = None,
+        task_priority: int = None,
     ) -> Tuple[models.Model, bool]:
         obj, created = super().update_or_create_esi(
             id=id,
             include_children=include_children,
             wait_for_children=wait_for_children,
             enabled_sections=enabled_sections,
+            task_priority=task_priority,
         )
-        enabled_sections = self.model._enabled_sections_union(enabled_sections)
+        enabled_sections = self.model.determine_effective_sections(enabled_sections)
         if enabled_sections and self.model.Section.TYPE_MATERIALS in enabled_sections:
             from .models import EveTypeMaterial
 
             EveTypeMaterial.objects.update_or_create_api(eve_type=obj)
 
         return obj, created
 
 
 class EveEntityQuerySet(models.QuerySet):
     """Custom queryset for EveEntity"""
 
-    MAX_DEPTH = 5
-
     def update_from_esi(self) -> int:
-        """Updates all Eve entity objects in this queryset from ESI"""
-        ids = list(self.values_list("id", flat=True))
-        if not ids:
-            return 0
-        else:
-            logger.info("Updating %d entities from ESI", len(ids))
-            resolved_counter = 0
-            for chunk_ids in chunks(ids, 1000):
-                logger.debug(
-                    "Trying to resolve the following IDs from ESI:\n%s", chunk_ids
-                )
-                resolved_counter = self._resolve_entities_from_esi(chunk_ids)
-            return resolved_counter
+        """Updates all Eve entity objects in this queryset from ESI."""
+        from .models import EveEntity
 
-    def _resolve_entities_from_esi(self, ids: list, depth: int = 1):
-        resolved_counter = 0
-        try:
-            items = esi.client.Universe.post_universe_names(ids=ids).results()
-        except HTTPNotFound:
-            # if API fails to resolve all IDs, we divide and conquer,
-            # trying to resolve each half of the ids seperately
-            if len(ids) > 1 and depth < self.MAX_DEPTH:
-                resolved_counter += self._resolve_entities_from_esi(ids[::2], depth + 1)
-                resolved_counter += self._resolve_entities_from_esi(
-                    ids[1::2], depth + 1
-                )
-            else:
-                logger.warning("Failed to resolve invalid IDs: %s", ids)
-        else:
-            resolved_counter += len(items)
-            for item in items:
-                try:
-                    self.update_or_create(
-                        id=item["id"],
-                        defaults={"name": item["name"], "category": item["category"]},
-                    )
-                except IntegrityError:
-                    pass
+        return EveEntity.objects.update_from_esi_by_id(self.valid_ids())
 
-        return resolved_counter
+    def valid_ids(self) -> Set[int]:
+        """Determine valid Ids in this Queryset."""
+        return set(
+            self.exclude(id__in=self.model.ESI_INVALID_IDS).values_list("id", flat=True)
+        )
 
 
 class EveEntityManager(EveUniverseEntityModelManager):
     """Custom manager for EveEntity"""
 
+    MAX_DEPTH = 5
+
     def get_queryset(self) -> models.QuerySet:
         return EveEntityQuerySet(self.model, using=self._db)
 
     def get_or_create_esi(
         self,
         *,
         id: int,
         include_children: bool = False,
         wait_for_children: bool = True,
+        enabled_sections: Iterable[str] = None,
+        task_priority: int = None,
     ) -> Tuple[models.Model, bool]:
         """gets or creates an EvEntity object.
 
         The object is automatically fetched from ESI if it does not exist (blocking)
         or if it has not yet been resolved.
 
         Args:
@@ -744,16 +738,17 @@
     def update_or_create_esi(
         self,
         *,
         id: int,
         include_children: bool = False,
         wait_for_children: bool = True,
         enabled_sections: Iterable[str] = None,
+        task_priority: int = None,
     ) -> Tuple[Optional[models.Model], bool]:
-        """updates or creates an EveEntity object by fetching it from ESI (blocking).
+        """Update or create an EveEntity object by fetching it from ESI (blocking).
 
         Args:
             id: Eve Online ID of object
             include_children: (no effect)
             wait_for_children: (no effect)
 
         Returns:
@@ -761,20 +756,22 @@
             When the ID is invalid the returned object will be None
 
         Exceptions:
             Raises all HTTP codes of ESI endpoint /universe/names except 404
         """
         id = int(id)
         logger.info("%s: Trying to resolve ID to EveEntity with ESI", id)
+        if id in self.model.ESI_INVALID_IDS:
+            logger.info("%s: ID is not valid", id)
+            return None, False
         try:
             result = esi.client.Universe.post_universe_names(ids=[id]).results()
         except HTTPNotFound:
             logger.info("%s: ID is not valid", id)
             return None, False
-
         item = result[0]
         return self.update_or_create(
             id=item.get("id"),
             defaults={"name": item.get("name"), "category": item.get("category")},
         )
 
     def bulk_create_esi(self, ids: Iterable[int]) -> int:
@@ -784,37 +781,38 @@
         Args:
             ids: List of valid EveEntity IDs
 
         Returns:
             Count of updated entities
         """
         ids = set(map(int, ids))
-        with transaction.atomic():
-            existing_ids = set(self.filter(id__in=ids).values_list("id", flat=True))
-            new_ids = ids.difference(existing_ids)
+        existing_ids = set(self.filter(id__in=ids).values_list("id", flat=True))
+        new_ids = ids.difference(existing_ids)
 
-        if new_ids:
-            objects = [self.model(id=id) for id in new_ids]
-            self.bulk_create(
-                objects,
-                batch_size=EVEUNIVERSE_BULK_METHODS_BATCH_SIZE,
-                ignore_conflicts=True,
-            )
-            to_update_qs = self.filter(id__in=new_ids) | self.filter(
-                id__in=ids.difference(new_ids), name=""
-            )
-            return to_update_qs.update_from_esi()
+        if not new_ids:
+            return 0
 
-        return 0
+        objects = [self.model(id=id) for id in new_ids]
+        self.bulk_create(
+            objects,
+            batch_size=EVEUNIVERSE_BULK_METHODS_BATCH_SIZE,
+            ignore_conflicts=True,
+        )
+        to_update_qs = self.filter(id__in=new_ids) | self.filter(
+            id__in=ids.difference(new_ids), name=""
+        )
+        return to_update_qs.update_from_esi()
 
     def update_or_create_all_esi(
         self,
         *,
         include_children: bool = False,
         wait_for_children: bool = True,
+        enabled_sections: Iterable[str] = None,
+        task_priority: int = None,
     ) -> None:
         """not implemented - do not use"""
         raise NotImplementedError()
 
     def bulk_update_new_esi(self) -> int:
         """updates all unresolved EveEntity objects in the database from ESI.
 
@@ -828,24 +826,93 @@
 
         Returns:
             Count of updated entities.
         """
         return self.all().update_from_esi()
 
     def resolve_name(self, id: int) -> str:
-        """return the name for the given Eve entity ID
-        or an empty string if ID is not valid
+        """Return the name for the given Eve entity ID
+        or an empty string if ID is not valid.
         """
         if id is not None:
             obj, _ = self.get_or_create_esi(id=int(id))
             if obj:
                 return obj.name
-
         return ""
 
+    def fetch_by_names_esi(
+        self, names: Iterable[str], update: bool = False
+    ) -> models.QuerySet:
+        """Fetch entities matching given names.
+        Will fetch missing entities from ESI if needed or requested.
+
+        Args:
+            names: Names of entities to fetch
+            update: When True will always update from ESI
+
+        Returns:
+            query with matching entities.
+        """
+        names = list(set(names))
+        query = self.filter(name__in=names)
+        if update or not query.exists():
+            result = self._fetch_names_from_esi(names)
+            if result:
+                result_compressed = {
+                    category: entities
+                    for category, entities in result.items()
+                    if entities
+                }
+                for category_key, entities in result_compressed.items():
+                    try:
+                        category = self._map_category_key_to_category(category_key)
+                    except ValueError:
+                        logger.warning(
+                            "Ignoring entities with unknown category %s: %s",
+                            category_key,
+                            entities,
+                        )
+                    else:
+                        for entity in entities:
+                            self.update_or_create(
+                                id=entity["id"],
+                                defaults={"name": entity["name"], "category": category},
+                            )
+        return query
+
+    def _fetch_names_from_esi(self, names: List[str]) -> dict:
+        logger.info("Trying to fetch EveEntities from ESI by name")
+        result = defaultdict(list)
+        for chunk_names in chunks(names, 500):
+            result_chunk = esi.client.Universe.post_universe_ids(
+                names=chunk_names
+            ).results()
+            for category, entities in result_chunk.items():
+                if entities:
+                    result[category] += entities
+        return result
+
+    def _map_category_key_to_category(self, category_key: str) -> str:
+        """Map category keys from ESI result to categories."""
+        my_map = {
+            "alliances": self.model.CATEGORY_ALLIANCE,
+            "characters": self.model.CATEGORY_CHARACTER,
+            "constellations": self.model.CATEGORY_CONSTELLATION,
+            "corporations": self.model.CATEGORY_CORPORATION,
+            "factions": self.model.CATEGORY_FACTION,
+            "inventory_types": self.model.CATEGORY_INVENTORY_TYPE,
+            "regions": self.model.CATEGORY_REGION,
+            "systems": self.model.CATEGORY_SOLAR_SYSTEM,
+            "stations": self.model.CATEGORY_STATION,
+        }
+        try:
+            return my_map[category_key]
+        except KeyError:
+            raise ValueError(f"Invalid category: {category_key}") from None
+
     def bulk_resolve_names(self, ids: Iterable[int]) -> EveEntityNameResolver:
         """returns a map of IDs to names in a resolver object for given IDs
 
         Args:
             ids: List of valid EveEntity IDs
 
         Returns:
@@ -857,14 +924,52 @@
         return EveEntityNameResolver(
             {
                 row[0]: row[1]
                 for row in self.filter(id__in=ids).values_list("id", "name")
             }
         )
 
+    def update_from_esi_by_id(self, ids: Iterable[int]) -> int:
+        """Updates all Eve entity objects by id from ESI."""
+        if not ids:
+            return 0
+        ids = list(set([int(id) for id in ids if id not in self.model.ESI_INVALID_IDS]))
+        logger.info("Updating %d entities from ESI", len(ids))
+        resolved_counter = 0
+        for chunk_ids in chunks(ids, POST_UNIVERSE_NAMES_MAX_ITEMS):
+            logger.debug("Trying to resolve the following IDs from ESI:\n%s", chunk_ids)
+            resolved_counter = self._resolve_entities_from_esi(chunk_ids)
+        return resolved_counter
+
+    def _resolve_entities_from_esi(self, ids: list, depth: int = 1):
+        resolved_counter = 0
+        try:
+            items = esi.client.Universe.post_universe_names(ids=ids).results()
+        except HTTPNotFound:
+            # if API fails to resolve all IDs, we divide and conquer,
+            # trying to resolve each half of the ids separately
+            if len(ids) > 1 and depth < self.MAX_DEPTH:
+                resolved_counter += self._resolve_entities_from_esi(ids[::2], depth + 1)
+                resolved_counter += self._resolve_entities_from_esi(
+                    ids[1::2], depth + 1
+                )
+            else:
+                logger.warning("Failed to resolve invalid IDs: %s", ids)
+        else:
+            resolved_counter += len(items)
+            for item in items:
+                try:
+                    self.update_or_create(
+                        id=item["id"],
+                        defaults={"name": item["name"], "category": item["category"]},
+                    )
+                except IntegrityError:
+                    pass
+        return resolved_counter
+
 
 class EveMarketPriceManager(models.Manager):
     def update_from_esi(self, minutes_until_stale: int = None) -> int:
         """Updates market prices from ESI. Will only create new price objects for EveTypes that already exist in the database.
 
         Args:
             minutes_until_stale: only prices older then given minutes are regarding as stale and will be updated. Will use default (60) if not specified.
@@ -941,15 +1046,16 @@
                 },
             )
 
     @classmethod
     def _fetch_sde_data_cached(cls) -> dict:
         type_material_data_all = cache.get(cls.SDE_CACHE_KEY)
         if not type_material_data_all:
-            r = requests.get(urljoin(SDE_ZZEVE_URL, cls.SDE_ZZEVE_ROUTE))
+            url = EVEUNIVERSE_ZZEVE_SDE_URL.rstrip("/") + "/" + cls.SDE_ZZEVE_ROUTE
+            r = requests.get(url, timeout=EVEUNIVERSE_REQUESTS_DEFAULT_TIMEOUT)
             r.raise_for_status()
             type_material_data_all = dict()
             for row in r.json():
                 type_id = row["typeID"]
                 if type_id not in type_material_data_all:
                     type_material_data_all[type_id] = list()
                 type_material_data_all[type_id].append(row)
```

### Comparing `django-eveuniverse-0.9.0/eveuniverse/migrations/0001_initial.py` & `django_eveuniverse-1.0.0a1/eveuniverse/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 2.2.13 on 2020-07-22 19:11
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="EveCategory",
```

### Comparing `django-eveuniverse-0.9.0/eveuniverse/migrations/0002_load_eveunit.py` & `django_eveuniverse-1.0.0a1/eveuniverse/migrations/0002_load_eveunit.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
                 "description": row["description"] if row["description"] else "",
             },
         }
         EveUnit.objects.update_or_create(**args)
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("eveuniverse", "0001_initial"),
     ]
 
     operations = [
         migrations.RunPython(migrate_forward),
     ]
```

### Comparing `django-eveuniverse-0.9.0/eveuniverse/migrations/0003_evemarketprice.py` & `django_eveuniverse-1.0.0a1/eveuniverse/migrations/0003_evemarketprice.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.1.1 on 2020-10-23 13:13
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("eveuniverse", "0002_load_eveunit"),
     ]
 
     operations = [
         migrations.CreateModel(
             name="EveMarketPrice",
```

### Comparing `django-eveuniverse-0.9.0/eveuniverse/migrations/0005_type_materials_and_sections.py` & `django_eveuniverse-1.0.0a1/eveuniverse/migrations/0005_type_materials_and_sections.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # Generated by Django 3.1.6 on 2021-02-25 18:10
 
 import bitfield.models
-
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("eveuniverse", "0004_effect_longer_name"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="eveplanet",
```

### Comparing `django-eveuniverse-0.9.0/eveuniverse/migrations/eve_unit.json` & `django_eveuniverse-1.0.0a1/eveuniverse/migrations/eve_unit.json`

 * *Files identical despite different names*

### Comparing `django-eveuniverse-0.9.0/eveuniverse/models.py` & `django_eveuniverse-1.0.0a1/eveuniverse/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import math
 import sys
 from collections import namedtuple
 from typing import Any, Dict, Iterable, List, Optional, Set, Tuple
 
 from bitfield import BitField
 from bravado.exception import HTTPNotFound
-
 from django.contrib.staticfiles.storage import staticfiles_storage
 from django.db import models
 
 from .app_settings import (
     EVEUNIVERSE_LOAD_ASTEROID_BELTS,
     EVEUNIVERSE_LOAD_DOGMAS,
     EVEUNIVERSE_LOAD_GRAPHICS,
@@ -21,15 +20,15 @@
     EVEUNIVERSE_LOAD_STARGATES,
     EVEUNIVERSE_LOAD_STARS,
     EVEUNIVERSE_LOAD_STATIONS,
     EVEUNIVERSE_LOAD_TYPE_MATERIALS,
     EVEUNIVERSE_USE_EVESKINSERVER,
 )
 from .constants import EveCategoryId, EveGroupId
-from .core import eveimageserver, evemicros, eveskinserver
+from .core import dotlan, eveimageserver, eveitems, evesdeapi, eveskinserver, evewho
 from .managers import (
     EveAsteroidBeltManager,
     EveEntityManager,
     EveMarketPriceManager,
     EveMoonManager,
     EvePlanetManager,
     EveStargateManager,
@@ -141,15 +140,15 @@
             x[0]: x[1]
             for x in inspect.getmembers(sys.modules[__name__], inspect.isclass)
             if issubclass(x[1], (EveUniverseBaseModel, EveUniverseInlineModel))
         }
         try:
             return classes[model_name]
         except KeyError:
-            raise ValueError("Unknown model_name: %s" % model_name)
+            raise ValueError("Unknown model_name: %s" % model_name) from None
 
     @classmethod
     def _esi_mapping(cls, enabled_sections: Set[str] = None) -> dict:
         field_mappings = cls._eve_universe_meta_attr("field_mappings")
         functional_pk = cls._eve_universe_meta_attr("functional_pk")
         parent_fk = cls._eve_universe_meta_attr("parent_fk")
         dont_create_related = cls._eve_universe_meta_attr("dont_create_related")
@@ -220,15 +219,15 @@
             value = getattr(cls.EveUniverseMeta, attr_name)
         except AttributeError:
             value = None
             if is_mandatory:
                 raise ValueError(
                     "Mandatory attribute EveUniverseMeta.%s not defined "
                     "for class %s" % (attr_name, cls.__name__)
-                )
+                ) from None
 
         return value
 
 
 class EveUniverseEntityModel(EveUniverseBaseModel):
     """Base class for Eve Universe Entity models
 
@@ -262,40 +261,40 @@
 
     class Meta:
         abstract = True
 
     def __str__(self) -> str:
         return self.name
 
-    @classmethod
-    def _enabled_sections_union(cls, enabled_sections: Iterable[str] = None) -> set:
-        """returns union of global and given enabled sections.
-        Needs to be overloaded by sub class using sections
-        """
+    @staticmethod
+    def determine_effective_sections(
+        enabled_sections: Iterable[str] = None,
+    ) -> Set[str]:
+        """Determine currently effective sections."""
         enabled_sections = set(enabled_sections) if enabled_sections else set()
         if EVEUNIVERSE_LOAD_ASTEROID_BELTS:
-            enabled_sections.add(EvePlanet.Section.ASTEROID_BELTS)
+            enabled_sections.add(EvePlanet.Section.ASTEROID_BELTS.value)
         if EVEUNIVERSE_LOAD_DOGMAS:
-            enabled_sections.add(EveType.Section.DOGMAS)
+            enabled_sections.add(EveType.Section.DOGMAS.value)
         if EVEUNIVERSE_LOAD_GRAPHICS:
-            enabled_sections.add(EveType.Section.GRAPHICS)
+            enabled_sections.add(EveType.Section.GRAPHICS.value)
         if EVEUNIVERSE_LOAD_MARKET_GROUPS:
-            enabled_sections.add(EveType.Section.MARKET_GROUPS)
+            enabled_sections.add(EveType.Section.MARKET_GROUPS.value)
         if EVEUNIVERSE_LOAD_MOONS:
-            enabled_sections.add(EvePlanet.Section.MOONS)
+            enabled_sections.add(EvePlanet.Section.MOONS.value)
         if EVEUNIVERSE_LOAD_PLANETS:
-            enabled_sections.add(EveSolarSystem.Section.PLANETS)
+            enabled_sections.add(EveSolarSystem.Section.PLANETS.value)
         if EVEUNIVERSE_LOAD_STARGATES:
-            enabled_sections.add(EveSolarSystem.Section.STARGATES)
+            enabled_sections.add(EveSolarSystem.Section.STARGATES.value)
         if EVEUNIVERSE_LOAD_STARS:
-            enabled_sections.add(EveSolarSystem.Section.STARS)
+            enabled_sections.add(EveSolarSystem.Section.STARS.value)
         if EVEUNIVERSE_LOAD_STATIONS:
-            enabled_sections.add(EveSolarSystem.Section.STATIONS)
+            enabled_sections.add(EveSolarSystem.Section.STATIONS.value)
         if EVEUNIVERSE_LOAD_TYPE_MATERIALS:
-            enabled_sections.add(EveType.Section.TYPE_MATERIALS)
+            enabled_sections.add(EveType.Section.TYPE_MATERIALS.value)
         return enabled_sections
 
     @classmethod
     def eve_entity_category(cls) -> str:
         """returns the EveEntity category of this model if one exists
         else and empty string
         """
@@ -370,14 +369,16 @@
 
     # NPC IDs
     NPC_CORPORATION_ID_BEGIN = 1_000_000
     NPC_CORPORATION_ID_END = 2_000_000
     NPC_CHARACTER_ID_BEGIN = 3_000_000
     NPC_CHARACTER_ID_END = 4_000_000
 
+    ESI_INVALID_IDS = {1}  # Will never try to resolve these invalid IDs from ESI
+
     # categories
     CATEGORY_ALLIANCE = "alliance"
     CATEGORY_CHARACTER = "character"
     CATEGORY_CONSTELLATION = "constellation"
     CATEGORY_CORPORATION = "corporation"
     CATEGORY_FACTION = "faction"
     CATEGORY_INVENTORY_TYPE = "inventory_type"
@@ -406,21 +407,20 @@
     class EveUniverseMeta:
         esi_pk = "ids"
         esi_path_object = "Universe.post_universe_names"
         load_order = 110
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
-        self._CATEGORIES = {x[0] for x in self.CATEGORY_CHOICES}
+        self._CATEGORIES = self.categories()
 
     def __str__(self) -> str:
         if self.name:
             return self.name
-        else:
-            return f"ID:{self.id}"
+        return f"ID:{self.id}"
 
     @property
     def is_alliance(self) -> bool:
         """returns True if entity is an alliance, else False"""
         return self.is_category(self.CATEGORY_ALLIANCE)
 
     @property
@@ -461,31 +461,71 @@
     @property
     def is_station(self) -> bool:
         """returns True if entity is a station, else False"""
         return self.is_category(self.CATEGORY_STATION)
 
     @property
     def is_npc(self) -> bool:
-        """returns True if this entity is an NPC character or NPC corporation,
-        else False
-        """
+        """True if this entity is an NPC character or NPC corporation, else False."""
         if (
             self.is_corporation
             and self.NPC_CORPORATION_ID_BEGIN <= self.id < self.NPC_CORPORATION_ID_END
         ):
             return True
-
         if (
             self.is_character
             and self.NPC_CHARACTER_ID_BEGIN <= self.id < self.NPC_CHARACTER_ID_END
         ):
             return True
-
         return False
 
+    @property
+    def is_npc_starter_corporation(self) -> bool:
+        """True if this entity is an NPC starter corporation else False."""
+        starter_corporation_ids = {
+            1000165,  # Amarr - Hedion University
+            1000166,  # Amarr - Imperial Academy
+            1000077,  # Amarr - Royal Amarr Institute
+            1000044,  # Caldari - School of Applied Knowledge
+            1000045,  # Caldari - Science and Trade Institute
+            1000167,  # Caldari - State War Academy
+            1000169,  # Gallente - Center for Advanced Studies
+            1000168,  # Gallente - Federal Navy Academy
+            1000115,  # Gallente - University of Caille
+            1000172,  # Minmatar - Pator Tech School
+            1000170,  # Minmatar - Republic Military School
+            1000171,  # Minmatar - Republic University
+        }
+        return self.is_corporation and self.id in starter_corporation_ids
+
+    @property
+    def profile_url(self) -> str:
+        """URL to default third party website with profile info about this entity.
+
+        Supported for:
+        alliance, character, corporation, faction, region, solar system, station, type
+        """
+        if self.is_alliance:
+            return dotlan.alliance_url(self.name)
+        elif self.is_character:
+            return evewho.character_url(self.id)
+        elif self.is_corporation:
+            return dotlan.corporation_url(self.name)
+        elif self.is_faction:
+            return dotlan.faction_url(self.name)
+        elif self.is_region:
+            return dotlan.region_url(self.name)
+        elif self.is_solar_system:
+            return dotlan.solar_system_url(self.name)
+        elif self.is_station:
+            return dotlan.station_url(self.name)
+        elif self.is_type:
+            return eveitems.type_url(self.id)
+        return ""
+
     def is_category(self, category: str) -> bool:
         """returns True if this entity has the given category, else False"""
         return category in self._CATEGORIES and self.category == category
 
     def update_from_esi(self) -> "EveEntity":
         """Update the current object from ESI
 
@@ -513,14 +553,24 @@
         }
         if self.category not in map_category_2_other:
             return ""
         else:
             func = map_category_2_other[self.category]
             return getattr(eveimageserver, func)(self.id, size=size)
 
+    @classmethod
+    def categories(cls) -> Set[str]:
+        """Set of valid categories."""
+        return {x[0] for x in cls.CATEGORY_CHOICES}
+
+    @classmethod
+    def is_valid_category(cls, category: str) -> bool:
+        """Wether given category is valid."""
+        return category in cls.categories()
+
 
 class EveAncestry(EveUniverseEntityModel):
     """An ancestry in Eve Online"""
 
     eve_bloodline = models.ForeignKey(
         "EveBloodline", on_delete=models.CASCADE, related_name="eve_bloodlines"
     )
@@ -771,15 +821,15 @@
         "EveDogmaEffect",
         on_delete=models.SET_DEFAULT,
         null=True,
         default=None,
         blank=True,
         related_name="modifying_effect_modifiers",
     )
-    operator = models.PositiveIntegerField(default=None, null=True)
+    operator = models.IntegerField(default=None, null=True)
 
     class Meta:
         constraints = [
             models.UniqueConstraint(
                 fields=["eve_dogma_effect", "func"],
                 name="fpk_evedogmaeffectmodifier",
             )
@@ -822,14 +872,19 @@
     class EveUniverseMeta:
         esi_pk = "faction_id"
         esi_path_list = "Universe.get_universe_factions"
         esi_path_object = "Universe.get_universe_factions"
         field_mappings = {"eve_solar_system": "solar_system_id"}
         load_order = 210
 
+    @property
+    def profile_url(self) -> str:
+        """URL to default third party website with profile info about this entity."""
+        return dotlan.faction_url(self.name)
+
     def logo_url(self, size=EveUniverseEntityModel.DEFAULT_ICON_SIZE) -> str:
         """returns an image URL for this faction
 
         Args:
             size: optional size of the image
         """
         return eveimageserver.faction_logo_url(self.id, size=size)
@@ -1001,15 +1056,15 @@
             "position_z": ("position", "z"),
         }
         children = {"moons": "EveMoon", "asteroid_belts": "EveAsteroidBelt"}
         load_order = 205
 
     @classmethod
     def _children(cls, enabled_sections: Iterable[str] = None) -> dict:
-        enabled_sections = cls._enabled_sections_union(enabled_sections)
+        enabled_sections = cls.determine_effective_sections(enabled_sections)
         children = dict()
         if cls.Section.ASTEROID_BELTS in enabled_sections:
             children["asteroid_belts"] = "EveAsteroidBelt"
         if cls.Section.MOONS in enabled_sections:
             children["moons"] = "EveMoon"
         return children
 
@@ -1035,28 +1090,33 @@
     class EveUniverseMeta:
         esi_pk = "region_id"
         esi_path_list = "Universe.get_universe_regions"
         esi_path_object = "Universe.get_universe_regions_region_id"
         children = {"constellations": "EveConstellation"}
         load_order = 190
 
+    @property
+    def profile_url(self) -> str:
+        """URL to default third party website with profile info about this entity."""
+        return dotlan.region_url(self.name)
+
     @classmethod
     def eve_entity_category(cls) -> str:
         return EveEntity.CATEGORY_REGION
 
 
 class EveSolarSystem(EveUniverseEntityModel):
     """A solar system in Eve Online"""
 
     class Section(_SectionBase):
         """Sections that can be optionally loaded with each instance"""
 
         PLANETS = "planets"  #:
         STARGATES = "stargates"  #:
-        STARS = "stars"  #
+        STARS = "stars"  #:
         STATIONS = "stations"  #:
 
     eve_constellation = models.ForeignKey(
         "EveConstellation", on_delete=models.CASCADE, related_name="eve_solarsystems"
     )
     eve_star = models.OneToOneField(
         "EveStar",
@@ -1098,14 +1158,19 @@
 
     NearestCelestial = namedtuple(
         "NearestCelestial", ["eve_type", "eve_object", "distance"]
     )
     NearestCelestial.__doc__ = "Container for a nearest celestial"
 
     @property
+    def profile_url(self) -> str:
+        """URL to default third party website with profile info about this entity."""
+        return dotlan.solar_system_url(self.name)
+
+    @property
     def is_high_sec(self) -> bool:
         """returns True if this solar system is in high sec, else False"""
         return round(self.security_status, 1) >= 0.5
 
     @property
     def is_low_sec(self) -> bool:
         """returns True if this solar system is in low sec, else False"""
@@ -1206,52 +1271,52 @@
 
         Raises:
             HTTPError: If an HTTP error is encountered
 
         Returns:
             Eve item or None if none is found
         """
-        item = evemicros.nearest_celestial(
+        item = evesdeapi.nearest_celestial(
             solar_system_id=self.id, x=x, y=y, z=z, group_id=group_id
         )
         if not item:
             return None
         eve_type, _ = EveType.objects.get_or_create_esi(id=item.type_id)
-        if eve_type.eve_group_id == EveGroupId.ASTEROID_BELT:
-            MyClass = EveAsteroidBelt
-        elif eve_type.eve_group_id == EveGroupId.MOON:
-            MyClass = EveMoon
-        elif eve_type.eve_group_id == EveGroupId.PLANET:
-            MyClass = EvePlanet
-        elif eve_type.eve_group_id == EveGroupId.STARGATE:
-            MyClass = EveStargate
-        elif eve_type.eve_group_id == EveGroupId.STATION:
-            MyClass = EveStation
-        else:
+        class_mapping = {
+            EveGroupId.ASTEROID_BELT: EveAsteroidBelt,
+            EveGroupId.MOON: EveMoon,
+            EveGroupId.PLANET: EvePlanet,
+            EveGroupId.STAR: EveStar,
+            EveGroupId.STARGATE: EveStargate,
+            EveGroupId.STATION: EveStation,
+        }
+        try:
+            MyClass = class_mapping[eve_type.eve_group_id]
+        except KeyError:
             return None
         obj, _ = MyClass.objects.get_or_create_esi(id=item.id)
         return self.NearestCelestial(
             eve_type=eve_type, eve_object=obj, distance=item.distance
         )
 
     @classmethod
     def _children(cls, enabled_sections: Iterable[str] = None) -> dict:
-        enabled_sections = cls._enabled_sections_union(enabled_sections)
+        enabled_sections = cls.determine_effective_sections(enabled_sections)
         children = dict()
         if cls.Section.PLANETS in enabled_sections:
             children["planets"] = "EvePlanet"
         if cls.Section.STARGATES in enabled_sections:
             children["stargates"] = "EveStargate"
         if cls.Section.STATIONS in enabled_sections:
             children["stations"] = "EveStation"
         return children
 
     @classmethod
     def _disabled_fields(cls, enabled_sections: Set[str] = None) -> set:
-        enabled_sections = cls._enabled_sections_union(enabled_sections)
+        enabled_sections = cls.determine_effective_sections(enabled_sections)
         if cls.Section.STARS not in enabled_sections:
             return {"eve_star"}
         return {}
 
     @classmethod
     def _inline_objects(cls, enabled_sections: Set[str] = None) -> dict:
         if enabled_sections and cls.Section.PLANETS in enabled_sections:
@@ -1401,18 +1466,19 @@
     """An inventory type in Eve Online"""
 
     class Section(_SectionBase):
         """Sections that can be optionally loaded with each instance"""
 
         DOGMAS = "dogmas"  #:
         GRAPHICS = "graphics"  #:
-        MARKET_GROUPS = "market_groups"  #
+        MARKET_GROUPS = "market_groups"  #:
         TYPE_MATERIALS = "type_materials"  #:
 
     capacity = models.FloatField(default=None, null=True)
+    description = models.TextField(default="")
     eve_group = models.ForeignKey(
         "EveGroup",
         on_delete=models.CASCADE,
         related_name="eve_types",
     )
     eve_graphic = models.ForeignKey(
         "EveGraphic",
@@ -1429,15 +1495,15 @@
         null=True,
         related_name="eve_types",
     )
     mass = models.FloatField(default=None, null=True)
     packaged_volume = models.FloatField(default=None, null=True)
     portion_size = models.PositiveIntegerField(default=None, null=True)
     radius = models.FloatField(default=None, null=True)
-    published = models.BooleanField()  # TODO: Add index
+    published = models.BooleanField()
     volume = models.FloatField(default=None, null=True)
     enabled_sections = BitField(
         flags=tuple(Section.values()),
         help_text=(
             "Flags for loadable sections. True if instance was loaded with section."
         ),  # no index, because MySQL does not support it for bitwise operations
     )
@@ -1455,14 +1521,19 @@
         }
         inline_objects = {
             "dogma_attributes": "EveTypeDogmaAttribute",
             "dogma_effects": "EveTypeDogmaEffect",
         }
         load_order = 134
 
+    @property
+    def profile_url(self) -> str:
+        """URL to display this type on the default third party webpage."""
+        return eveitems.type_url(self.id)
+
     class IconVariant(enum.Enum):
         """Variant of icon to produce with `icon_url()`"""
 
         REGULAR = enum.auto()
         """anything, except blueprint or skin"""
 
         BPO = enum.auto()
@@ -1527,15 +1598,15 @@
 
     def render_url(self, size=EveUniverseEntityModel.DEFAULT_ICON_SIZE) -> str:
         """return an image URL to this type as render"""
         return eveimageserver.type_render_url(self.id, size=size)
 
     @classmethod
     def _disabled_fields(cls, enabled_sections: Set[str] = None) -> set:
-        enabled_sections = cls._enabled_sections_union(enabled_sections)
+        enabled_sections = cls.determine_effective_sections(enabled_sections)
         disabled_fields = set()
         if cls.Section.GRAPHICS not in enabled_sections:
             disabled_fields.add("eve_graphic")
         if cls.Section.MARKET_GROUPS not in enabled_sections:
             disabled_fields.add("eve_market_group")
         return disabled_fields
```

### Comparing `django-eveuniverse-0.9.0/eveuniverse/static/eveuniverse/skin_generic_128.png` & `django_eveuniverse-1.0.0a1/eveuniverse/static/eveuniverse/skin_generic_128.png`

 * *Files identical despite different names*

### Comparing `django-eveuniverse-0.9.0/eveuniverse/static/eveuniverse/skin_generic_32.png` & `django_eveuniverse-1.0.0a1/eveuniverse/static/eveuniverse/skin_generic_32.png`

 * *Files identical despite different names*

### Comparing `django-eveuniverse-0.9.0/eveuniverse/static/eveuniverse/skin_generic_64.png` & `django_eveuniverse-1.0.0a1/eveuniverse/static/eveuniverse/skin_generic_64.png`

 * *Files identical despite different names*

### Comparing `django-eveuniverse-0.9.0/eveuniverse/tasks.py` & `django_eveuniverse-1.0.0a1/eveuniverse/tasks.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,92 +1,95 @@
 import logging
 from typing import Iterable, List
 
-from bravado.exception import HTTPBadGateway, HTTPGatewayTimeout, HTTPServiceUnavailable
 from celery import shared_task
+from celery_once import QueueOnce as BaseQueueOnce
+from django.db.utils import OperationalError
 
 from . import __title__, models
-from .app_settings import (
-    EVEUNIVERSE_LOAD_ASTEROID_BELTS,
-    EVEUNIVERSE_LOAD_DOGMAS,
-    EVEUNIVERSE_LOAD_GRAPHICS,
-    EVEUNIVERSE_LOAD_MARKET_GROUPS,
-    EVEUNIVERSE_LOAD_MOONS,
-    EVEUNIVERSE_LOAD_PLANETS,
-    EVEUNIVERSE_LOAD_STARGATES,
-    EVEUNIVERSE_LOAD_STARS,
-    EVEUNIVERSE_LOAD_STATIONS,
-    EVEUNIVERSE_TASKS_TIME_LIMIT,
-)
-from .constants import EVE_CATEGORY_ID_SHIP, EveCategoryId
-from .models import EveEntity, EveMarketPrice, EveUniverseEntityModel
+from .app_settings import EVEUNIVERSE_LOAD_TASKS_PRIORITY, EVEUNIVERSE_TASKS_TIME_LIMIT
+from .constants import POST_UNIVERSE_NAMES_MAX_ITEMS, EveCategoryId
+from .models import EveEntity, EveMarketPrice, EveType, EveUniverseEntityModel
 from .providers import esi
-from .utils import LoggerAddTag
+from .utils import LoggerAddTag, chunks
 
 logger = LoggerAddTag(logging.getLogger(__name__), __title__)
 # logging.getLogger("esi").setLevel(logging.INFO)
 
 
+class QueueOnce(BaseQueueOnce):
+    """Make sure all redundant tasks will abort gracefully."""
+
+    once = BaseQueueOnce.once
+    once["graceful"] = True
+
+
 # params for all tasks
-TASK_DEFAULT_KWARGS = {
-    "time_limit": EVEUNIVERSE_TASKS_TIME_LIMIT,
-}
+TASK_DEFAULTS = {"time_limit": EVEUNIVERSE_TASKS_TIME_LIMIT}
 
 # params for tasks that make ESI calls
-TASK_ESI_KWARGS = {
-    **TASK_DEFAULT_KWARGS,
+TASK_ESI_DEFAULTS = {
+    **TASK_DEFAULTS,
     **{
-        "autoretry_for": (
-            OSError,
-            HTTPBadGateway,
-            HTTPGatewayTimeout,
-            HTTPServiceUnavailable,
-        ),
+        "autoretry_for": [OperationalError],
         "retry_kwargs": {"max_retries": 3},
-        "retry_backoff": 30,
+        "retry_backoff": True,
     },
 }
+TASK_ESI_DEFAULTS_ONCE = {**TASK_ESI_DEFAULTS, **{"base": QueueOnce}}
+
 
 # Eve Universe objects
 
 
-@shared_task(**TASK_ESI_KWARGS)
+@shared_task(**TASK_ESI_DEFAULTS_ONCE)
 def load_eve_object(
     model_name: str, id: int, include_children=False, wait_for_children=True
 ) -> None:
     """Task for loading an eve object.
     Will only be created from ESI if it does not exist
     """
     logger.info("Loading %s with ID %s", model_name, id)
     ModelClass = EveUniverseEntityModel.get_model_class(model_name)
     ModelClass.objects.get_or_create_esi(
         id=id, include_children=include_children, wait_for_children=wait_for_children
     )
 
 
-@shared_task(**TASK_ESI_KWARGS)
+@shared_task(**TASK_ESI_DEFAULTS_ONCE)
 def update_or_create_eve_object(
     model_name: str,
     id: int,
     include_children=False,
     wait_for_children=True,
     enabled_sections: List[str] = None,
+    task_priority: int = None,
 ) -> None:
-    """Task for updating or creating an eve object from ESI"""
+    """Update or create an eve object from ESI.
+
+    Args:
+        model_name: Name of the respective Django model, e.g. ``"EveType"``
+        id: Eve Online ID of object
+        include_children: if child objects should be updated/created as well (only when a new object is created)
+        wait_for_children: when true child objects will be updated/created blocking (if any), else async (only when a new object is created)
+        enabled_sections: Sections to load regardless of current settings, e.g. `[EveType.Section.DOGMAS]` will always load dogmas for EveTypes
+        task_priority: priority of started tasks
+    """
     logger.info("Updating/Creating %s with ID %s", model_name, id)
     ModelClass = EveUniverseEntityModel.get_model_class(model_name)
     ModelClass.objects.update_or_create_esi(
         id=id,
         include_children=include_children,
         wait_for_children=wait_for_children,
         enabled_sections=enabled_sections,
+        task_priority=task_priority,
     )
 
 
-@shared_task(**TASK_ESI_KWARGS)
+@shared_task(**TASK_ESI_DEFAULTS_ONCE)
 def update_or_create_inline_object(
     parent_obj_id: int,
     parent_fk: str,
     eve_data_obj: dict,
     other_pk_info: dict,
     parent2_model_name: str,
     inline_model_name: str,
@@ -111,127 +114,166 @@
         enabled_sections=enabled_sections,
     )
 
 
 # EveEntity objects
 
 
-@shared_task(**TASK_ESI_KWARGS)
+@shared_task(**TASK_ESI_DEFAULTS)
 def create_eve_entities(ids: Iterable[int]) -> None:
     """Task for bulk creating and resolving multiple entities from ESI."""
     EveEntity.objects.bulk_create_esi(ids)
 
 
-@shared_task(**TASK_ESI_KWARGS)
+@shared_task(**TASK_ESI_DEFAULTS_ONCE)
 def update_unresolved_eve_entities() -> None:
-    """Task for bulk updating all unresolved EveEntity objects in the database from ESI."""
-    EveEntity.objects.bulk_update_new_esi()
+    """Update all unresolved EveEntity objects from ESI.
+
+    Will resolve entities in parallel to speed up resolving large sets.
+    """
+    ids = list(EveEntity.objects.filter(name="").valid_ids())
+    logger.info("Updating %d unresolved entities from ESI", len(ids))
+    for chunk_ids in chunks(ids, POST_UNIVERSE_NAMES_MAX_ITEMS):
+        _update_unresolved_eve_entities_for_page.delay(chunk_ids)
+
+
+@shared_task(**TASK_ESI_DEFAULTS)
+def _update_unresolved_eve_entities_for_page(ids: Iterable[int]) -> None:
+    """Update unresolved EveEntity objects for given ids from ESI."""
+    EveEntity.objects.update_from_esi_by_id(ids)
 
 
 # Object loaders
 
 
-def _eve_object_names_to_be_loaded() -> list:
-    """returns a list of eve object that are loaded"""
-    config_map = [
-        (EVEUNIVERSE_LOAD_DOGMAS, "dogmas"),
-        (EVEUNIVERSE_LOAD_MARKET_GROUPS, "market groups"),
-        (EVEUNIVERSE_LOAD_ASTEROID_BELTS, "asteroid belts"),
-        (EVEUNIVERSE_LOAD_GRAPHICS, "graphics"),
-        (EVEUNIVERSE_LOAD_MOONS, "moons"),
-        (EVEUNIVERSE_LOAD_PLANETS, "planets"),
-        (EVEUNIVERSE_LOAD_STARGATES, "stargates"),
-        (EVEUNIVERSE_LOAD_STARS, "stars"),
-        (EVEUNIVERSE_LOAD_STATIONS, "stations"),
-    ]
-    names_to_be_loaded = []
-    for setting, entity_name in config_map:
-        if setting:
-            names_to_be_loaded.append(entity_name)
-    return sorted(names_to_be_loaded)
-
-
-@shared_task(**TASK_ESI_KWARGS)
-def load_map() -> None:
-    """loads the complete Eve map with all regions, constellation and solarsystems
-    and additional related entities if they are enabled
+@shared_task(**TASK_ESI_DEFAULTS_ONCE)
+def load_map(enabled_sections: List[str] = None) -> None:
+    """Load the complete Eve map with all regions, constellation and solar systems
+    and additional related entities if they are enabled.
+
+    Args:
+        enabled_sections: Sections to load regardless of current settings
     """
     logger.info(
-        "Loading complete map with all regions, constellations, solarsystems "
+        "Loading complete map with all regions, constellations, solar systems "
         "and the following additional entities if related to the map: %s",
-        ", ".join(_eve_object_names_to_be_loaded()),
+        ", ".join(
+            EveUniverseEntityModel.determine_effective_sections(enabled_sections)
+        ),
     )
     category, method = models.EveRegion._esi_path_list()
     all_ids = getattr(getattr(esi.client, category), method)().results()
     for id in all_ids:
         update_or_create_eve_object.delay(
             model_name="EveRegion",
             id=id,
             include_children=True,
             wait_for_children=False,
+            enabled_sections=enabled_sections,
+            task_priority=EVEUNIVERSE_LOAD_TASKS_PRIORITY,
         )
 
 
-def _load_category(category_id: int, force_loading_dogma: bool = False) -> None:
-    """Starts a task for loading a category incl. all it's children from ESI via"""
-    enabled_sections = (
-        [EveUniverseEntityModel.LOAD_DOGMAS] if force_loading_dogma else None
+@shared_task(**TASK_ESI_DEFAULTS_ONCE)
+def load_all_types(enabled_sections: List[str] = None) -> None:
+    """Load all eve types.
+
+    Args:
+        enabled_sections: Sections to load regardless of current settings
+    """
+    logger.info(
+        "Loading all eve types from ESI including these sections: %s",
+        ", ".join(
+            EveUniverseEntityModel.determine_effective_sections(enabled_sections)
+        ),
     )
+    category, method = models.EveCategory._esi_path_list()
+    result = getattr(getattr(esi.client, category), method)().results()
+    if not result:
+        raise ValueError("Did not receive category IDs from ESI.")
+    category_ids = sorted(result)
+    logger.debug("Fetching categories for IDs: %s", category_ids)
+    for category_id in category_ids:
+        _load_category_with_children(
+            category_id=category_id, enabled_sections=enabled_sections
+        )
+
+
+def _load_category_with_children(
+    category_id: int,
+    force_loading_dogma: bool = False,
+    enabled_sections: List[str] = None,
+) -> None:
+    """Start loading a category async incl. all it's children from ESI."""
+    enabled_sections = enabled_sections or []
+    if force_loading_dogma:
+        enabled_sections.append(EveType.Section.DOGMAS.value)
     update_or_create_eve_object.delay(
         model_name="EveCategory",
         id=category_id,
         include_children=True,
         wait_for_children=False,
         enabled_sections=enabled_sections,
+        task_priority=EVEUNIVERSE_LOAD_TASKS_PRIORITY,
     )
 
 
-def _load_group(group_id: int, force_loading_dogma: bool = False) -> None:
+def _load_group_with_children(group_id: int, force_loading_dogma: bool = False) -> None:
     """Starts a task for loading a group incl. all it's children from ESI"""
-    enabled_sections = (
-        [EveUniverseEntityModel.LOAD_DOGMAS] if force_loading_dogma else None
-    )
+    enabled_sections = [EveType.Section.DOGMAS.value] if force_loading_dogma else None
     update_or_create_eve_object.delay(
         model_name="EveGroup",
         id=group_id,
         include_children=True,
         wait_for_children=False,
         enabled_sections=enabled_sections,
+        task_priority=EVEUNIVERSE_LOAD_TASKS_PRIORITY,
     )
 
 
-def _load_type(type_id: int, force_loading_dogma: bool = False) -> None:
+def _load_type_with_children(type_id: int, force_loading_dogma: bool = False) -> None:
     """Starts a task for loading a type incl. all it's children from ESI"""
-    enabled_sections = (
-        [EveUniverseEntityModel.LOAD_DOGMAS] if force_loading_dogma else None
-    )
+    enabled_sections = [EveType.Section.DOGMAS.value] if force_loading_dogma else None
     update_or_create_eve_object.delay(
         model_name="EveType",
         id=type_id,
         include_children=False,
         wait_for_children=False,
         enabled_sections=enabled_sections,
+        task_priority=EVEUNIVERSE_LOAD_TASKS_PRIORITY,
     )
 
 
-@shared_task(**TASK_DEFAULT_KWARGS)
-def load_ship_types() -> None:
-    """Loads all ship types"""
+@shared_task(**TASK_ESI_DEFAULTS_ONCE)
+def load_ship_types(enabled_sections: List[str] = None) -> None:
+    """Load all ship types.
+
+    Args:
+        enabled_sections: Sections to load regardless of current settings
+    """
     logger.info("Started loading all ship types into eveuniverse")
-    _load_category(EVE_CATEGORY_ID_SHIP)
+    _load_category_with_children(
+        category_id=EveCategoryId.SHIP.value, enabled_sections=enabled_sections
+    )
 
 
-@shared_task(**TASK_DEFAULT_KWARGS)
-def load_structure_types() -> None:
-    """Loads all structure types"""
+@shared_task(**TASK_ESI_DEFAULTS_ONCE)
+def load_structure_types(enabled_sections: List[str] = None) -> None:
+    """Load all structure types.
+
+    Args:
+        enabled_sections: Sections to load regardless of current settings
+    """
     logger.info("Started loading all structure types into eveuniverse")
-    _load_category(EveCategoryId.STRUCTURE)
+    _load_category_with_children(
+        category_id=EveCategoryId.STRUCTURE.value, enabled_sections=enabled_sections
+    )
 
 
-@shared_task(**TASK_DEFAULT_KWARGS)
+@shared_task(**TASK_ESI_DEFAULTS_ONCE)
 def load_eve_types(
     category_ids: List[int] = None,
     group_ids: List[int] = None,
     type_ids: List[int] = None,
     force_loading_dogma: bool = False,
 ) -> None:
     """Load specified eve types from ESI. Will always load all children except for EveType
@@ -241,23 +283,23 @@
     - group_ids: EveGroup IDs
     - type_ids: EveType IDs
     - load_dogma: When True will load dogma for all types
     """
     logger.info("Started loading several eve types into eveuniverse")
     if category_ids:
         for category_id in category_ids:
-            _load_category(category_id, force_loading_dogma)
+            _load_category_with_children(category_id, force_loading_dogma)
 
     if group_ids:
         for group_id in group_ids:
-            _load_group(group_id, force_loading_dogma)
+            _load_group_with_children(group_id, force_loading_dogma)
 
     if type_ids:
         for type_id in type_ids:
-            _load_type(type_id, force_loading_dogma)
+            _load_type_with_children(type_id, force_loading_dogma)
 
 
-@shared_task(**TASK_ESI_KWARGS)
+@shared_task(**TASK_ESI_DEFAULTS_ONCE)
 def update_market_prices(minutes_until_stale: int = None):
     """Updates market prices from ESI.
     see EveMarketPrice.objects.update_from_esi() for details"""
     EveMarketPrice.objects.update_from_esi(minutes_until_stale)
```

### Comparing `django-eveuniverse-0.9.0/eveuniverse/tests/pilot.py` & `django_eveuniverse-1.0.0a1/eveuniverse/tests/pilot.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -30,23 +30,23 @@
 
 django.setup()
 
 # normal imports
 import logging
 
 from django.core.cache import cache
+
 from eveuniverse.models import *
 from eveuniverse.providers import esi
 
 cache.clear()
 logger = logging.getLogger("__name__")
 
 
 def main():
-
     # EveType.objects.update_or_create_esi(603)
     # EveType.objects.update_or_create_esi(608)
     EveStation.objects.update_or_create(id=60015068)
 
     # EveBloodline.objects.load_esi()
```

### Comparing `django-eveuniverse-0.9.0/eveuniverse/tests/test_helpers.py` & `django_eveuniverse-1.0.0a1/eveuniverse/tests/test_helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..helpers import EveEntityNameResolver, meters_to_au, meters_to_ly
+from ..helpers import EveEntityNameResolver, dict_hash, meters_to_au, meters_to_ly
 from ..utils import NoSocketsTestCase
 
 
 class TestHelpers(NoSocketsTestCase):
     def test_meters_to_ly(self):
         self.assertEqual(meters_to_ly(9_460_730_472_580_800), 1)
         self.assertEqual(meters_to_ly(0), 0)
@@ -17,7 +17,22 @@
 
 
 class TestEveEntityNameResolver(NoSocketsTestCase):
     def test_to_name(self):
         resolver = EveEntityNameResolver({1: "alpha", 2: "bravo", 3: "charlie"})
         self.assertEqual(resolver.to_name(2), "bravo")
         self.assertEqual(resolver.to_name(4), "")
+
+
+class TestDictHash(NoSocketsTestCase):
+    def test_should_create_string(self):
+        # given
+        d1 = {"a": 1, "b": 2, "c": 3}
+        d2 = {"a": 1, "b": 2, "c": 4}
+        # when
+        hash_1a = dict_hash(d1)
+        hash_1b = dict_hash(d1)
+        hash_2 = dict_hash(d2)
+        # then
+        self.assertIsInstance(hash_1a, str)
+        self.assertEqual(hash_1a, hash_1b)
+        self.assertNotEqual(hash_1a, hash_2)
```

### Comparing `django-eveuniverse-0.9.0/eveuniverse/tests/test_models_1.py` & `django_eveuniverse-1.0.0a1/eveuniverse/tests/test_models_1.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime as dt
 import unittest
 from unittest.mock import Mock, patch
 
 from bravado.exception import HTTPNotFound
-
+from django.test.utils import override_settings
 from django.utils.timezone import now
 
 from ..helpers import meters_to_ly
 from ..models import (
     EveAncestry,
     EveAsteroidBelt,
     EveBloodline,
@@ -146,14 +146,18 @@
         self.assertEqual(obj.position_z, 219234300596.24887)
         self.assertEqual(obj.eve_planet, EvePlanet.objects.get(id=40349471))
 
 
 @patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_DOGMAS", True)
 @patch(MANAGERS_PATH + ".esi")
 class TestEveCategory(NoSocketsTestCase):
+    """These tests also cover the manager functionality shared among
+    all entity models. (1/2)
+    """
+
     def test_when_not_exists_load_object_from_esi(self, mock_esi):
         mock_esi.client = EsiClientStub()
 
         obj, created = EveCategory.objects.get_or_create_esi(id=6)
         self.assertTrue(created)
         self.assertEqual(obj.id, 6)
         self.assertEqual(obj.name, "Ship")
@@ -217,14 +221,178 @@
         )
         self.assertSetEqual(
             set(eve_type.dogma_effects.values_list("eve_dogma_effect_id", flat=True)),
             {1816, 1817},
         )
 
 
+@override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
+@patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_GRAPHICS", False)
+@patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_DOGMAS", False)
+@patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_MARKET_GROUPS", False)
+@patch(MANAGERS_PATH + ".esi")
+class TestEveCategoryUpdateAll(NoSocketsTestCase):
+    """These tests also cover the manager functionality shared among
+    all entity models. (2/2)
+    """
+
+    def test_should_update_without_children_and_sync(self, mock_esi):
+        # given
+        mock_esi.client = EsiClientStub()
+        # when
+        EveCategory.objects.update_or_create_all_esi(
+            include_children=False, wait_for_children=True
+        )
+        # then
+        self.assertSetEqual(
+            set(EveCategory.objects.values_list("id", flat=True)),
+            {1, 2, 3, 4, 6, 9, 17, 65, 91},
+        )
+        self.assertEqual(EveGroup.objects.count(), 0)
+        self.assertEqual(EveType.objects.count(), 0)
+
+    def test_should_update_without_children_and_sync_task_priority(self, mock_esi):
+        # given
+        mock_esi.client = EsiClientStub()
+        # when
+        EveCategory.objects.update_or_create_all_esi(
+            include_children=False, wait_for_children=True, task_priority=7
+        )
+        # then
+        self.assertSetEqual(
+            set(EveCategory.objects.values_list("id", flat=True)),
+            {1, 2, 3, 4, 6, 9, 17, 65, 91},
+        )
+        self.assertEqual(EveGroup.objects.count(), 0)
+        self.assertEqual(EveType.objects.count(), 0)
+
+    def test_should_raise_exception_on_error(self, mock_esi):
+        # given
+        mock_esi.client.Universe.get_universe_categories.side_effect = OSError
+        # when/then
+        with self.assertRaises(OSError):
+            EveCategory.objects.update_or_create_all_esi(
+                include_children=False, wait_for_children=True
+            )
+
+    def test_should_update_with_children_and_sync(self, mock_esi):
+        # given
+        mock_esi.client = EsiClientStub()
+        # when
+        EveCategory.objects.update_or_create_all_esi(
+            include_children=True, wait_for_children=True
+        )
+        # then
+        self.assertSetEqual(
+            set(EveCategory.objects.values_list("id", flat=True)),
+            {1, 2, 3, 4, 6, 9, 17, 65, 91},
+        )
+        self.assertSetEqual(
+            set(EveGroup.objects.values_list("id", flat=True)),
+            {1, 5, 6, 7, 8, 9, 10, 105, 15, 18, 536, 25, 26, 1404, 1950},
+        )
+        self.assertSetEqual(
+            set(EveType.objects.values_list("id", flat=True)),
+            {
+                13,
+                14,
+                15,
+                16,
+                34,
+                35,
+                36,
+                37,
+                38,
+                39,
+                40,
+                34599,
+                950,
+                21947,
+                29627,
+                21949,
+                21951,
+                21953,
+                21955,
+                21957,
+                21959,
+                21961,
+                21967,
+                3800,
+                603,
+                608,
+                2016,
+                621,
+                45038,
+                35825,
+                626,
+                1529,
+                1376,
+                5,
+                52678,
+            },
+        )
+
+    def test_should_update_with_children_and_async(self, mock_esi):
+        # given
+        mock_esi.client = EsiClientStub()
+        # when
+        EveCategory.objects.update_or_create_all_esi(
+            include_children=True, wait_for_children=False, task_priority=7
+        )
+        # then
+        self.assertSetEqual(
+            set(EveCategory.objects.values_list("id", flat=True)),
+            {1, 2, 3, 4, 6, 9, 17, 65, 91},
+        )
+        self.assertSetEqual(
+            set(EveGroup.objects.values_list("id", flat=True)),
+            {1, 5, 6, 7, 8, 9, 10, 105, 15, 18, 536, 25, 26, 1404, 1950},
+        )
+        self.assertSetEqual(
+            set(EveType.objects.values_list("id", flat=True)),
+            {
+                5,
+                13,
+                14,
+                15,
+                16,
+                34,
+                35,
+                36,
+                37,
+                38,
+                39,
+                40,
+                950,
+                1376,
+                34599,
+                21947,
+                29627,
+                21949,
+                21951,
+                21953,
+                21955,
+                21957,
+                21959,
+                21961,
+                21967,
+                3800,
+                603,
+                608,
+                2016,
+                621,
+                45038,
+                35825,
+                626,
+                1529,
+                52678,
+            },
+        )
+
+
 @patch(MANAGERS_PATH + ".esi")
 class TestBulkGetOrCreateEsi(NoSocketsTestCase):
     def test_can_load_all_from_esi(self, mock_esi):
         mock_esi.client = EsiClientStub()
 
         result = EveCategory.objects.bulk_get_or_create_esi(ids=[2, 3])
         self.assertEqual({x.id for x in result}, {2, 3})
```

### Comparing `django-eveuniverse-0.9.0/eveuniverse/tests/test_models_3.py` & `django_eveuniverse-1.0.0a1/eveuniverse/tests/test_models_3.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 from unittest.mock import patch
 
 import requests_mock
 
-from django.test.utils import override_settings
-
 from ..constants import EveGroupId
-from ..core import evemicros
+from ..core import evesdeapi
 from ..models import (
     EveAsteroidBelt,
-    EveCategory,
-    EveGroup,
     EveMoon,
     EvePlanet,
     EveSolarSystem,
+    EveStar,
     EveStargate,
     EveStation,
     EveType,
     EveTypeMaterial,
 )
 from ..utils import NoSocketsTestCase
 from .testdata.esi import EsiClientStub
 from .testdata.sde import sde_data, type_materials_cache_content
 
 MODELS_PATH = "eveuniverse.models"
 MANAGERS_PATH = "eveuniverse.managers"
 
 
+@patch(MANAGERS_PATH + ".EVEUNIVERSE_ZZEVE_SDE_URL", "https://sde.eve-o.tech/latest")
 @patch(MANAGERS_PATH + ".cache")
 @patch(MANAGERS_PATH + ".esi")
 @requests_mock.Mocker()
 class TestEveTypeMaterial(NoSocketsTestCase):
     def test_should_create_new_instance(self, mock_esi, mock_cache, requests_mocker):
         # given
         mock_esi.client = EsiClientStub()
         mock_cache.get.return_value = None
         mock_cache.set.return_value = None
         requests_mocker.register_uri(
             "GET",
-            url="https://sde.zzeve.com/invTypeMaterials.json",
+            url="https://sde.eve-o.tech/latest/invTypeMaterials.json",
             json=sde_data["type_materials"],
         )
         with patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_TYPE_MATERIALS", False):
             eve_type, _ = EveType.objects.get_or_create_esi(id=603)
         # when
         EveTypeMaterial.objects.update_or_create_api(eve_type=eve_type)
         # then
@@ -73,15 +71,15 @@
     def test_should_use_cache_if_available(self, mock_esi, mock_cache, requests_mocker):
         # given
         mock_esi.client = EsiClientStub()
         mock_cache.get.return_value = type_materials_cache_content()
         mock_cache.set.return_value = None
         requests_mocker.register_uri(
             "GET",
-            url="https://sde.zzeve.com/invTypeMaterials.json",
+            url="https://sde.eve-o.tech/latest/invTypeMaterials.json",
             json=sde_data["type_materials"],
         )
         with patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_TYPE_MATERIALS", False):
             eve_type, _ = EveType.objects.get_or_create_esi(id=603)
         # when
         EveTypeMaterial.objects.update_or_create_api(eve_type=eve_type)
         # then
@@ -101,15 +99,15 @@
     ):
         # given
         mock_esi.client = EsiClientStub()
         mock_cache.get.return_value = None
         mock_cache.set.return_value = None
         requests_mocker.register_uri(
             "GET",
-            url="https://sde.zzeve.com/invTypeMaterials.json",
+            url="https://sde.eve-o.tech/latest/invTypeMaterials.json",
             json=sde_data["type_materials"],
         )
         with patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_TYPE_MATERIALS", False):
             eve_type, _ = EveType.objects.get_or_create_esi(id=34)
         # when
         EveTypeMaterial.objects.update_or_create_api(eve_type=eve_type)
         # then
@@ -129,15 +127,15 @@
     ):
         # given
         mock_esi.client = EsiClientStub()
         mock_cache.get.return_value = None
         mock_cache.set.return_value = None
         requests_mocker.register_uri(
             "GET",
-            url="https://sde.zzeve.com/invTypeMaterials.json",
+            url="https://sde.eve-o.tech/latest/invTypeMaterials.json",
             json=sde_data["type_materials"],
         )
         # when
         with patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_TYPE_MATERIALS", True):
             eve_type, _ = EveType.objects.update_or_create_esi(id=603)
         # then
         self.assertTrue(requests_mocker.called)
@@ -156,15 +154,15 @@
     ):
         # given
         mock_esi.client = EsiClientStub()
         mock_cache.get.return_value = None
         mock_cache.set.return_value = None
         requests_mocker.register_uri(
             "GET",
-            url="https://sde.zzeve.com/invTypeMaterials.json",
+            url="https://sde.eve-o.tech/latest/invTypeMaterials.json",
             json=sde_data["type_materials"],
         )
         # when
         with patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_TYPE_MATERIALS", False):
             eve_type, _ = EveType.objects.update_or_create_esi(id=603)
         # then
         self.assertFalse(requests_mocker.called)
@@ -406,15 +404,15 @@
             {34, 35, 36, 37, 38, 39, 40},
         )
         self.assertEqual(obj.eve_graphic_id, 314)
         self.assertTrue(obj.enabled_sections.graphics)
         self.assertTrue(obj.enabled_sections.type_materials)
 
 
-class EveTypeSection(NoSocketsTestCase):
+class TestEveTypeSection(NoSocketsTestCase):
     def test_should_return_value_as_str(self):
         self.assertEqual(str(EveType.Section.DOGMAS), "dogmas")
 
     def test_should_return_values(self):
         self.assertEqual(
             list(EveType.Section),
             ["dogmas", "graphics", "market_groups", "type_materials"],
@@ -906,53 +904,79 @@
         self.assertEqual(
             set(obj.eve_moons.values_list("id", flat=True)), {40349472, 40349473}
         )
         self.assertFalse(obj.enabled_sections.asteroid_belts)
         self.assertTrue(obj.enabled_sections.moons)
 
 
-@patch(MODELS_PATH + ".evemicros")
+@patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_ASTEROID_BELTS", False)
+@patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_DOGMAS", False)
+@patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_GRAPHICS", False)
+@patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_MARKET_GROUPS", False)
+@patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_MOONS", False)
+@patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_PLANETS", False)
+@patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_STARGATES", False)
+@patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_STARS", False)
+@patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_STATIONS", False)
+@patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_TYPE_MATERIALS", False)
+@patch(MODELS_PATH + ".evesdeapi")
 @patch(MANAGERS_PATH + ".esi")
 class TestEveSolarSystemNearestCelestial(NoSocketsTestCase):
-    def test_should_return_stargate(self, mock_esi, mock_evemicros):
+    def test_should_return_stargate(self, mock_esi, mock_evesdeapi):
         # given
         mock_esi.client = EsiClientStub()
-        mock_evemicros.nearest_celestial.return_value = evemicros.EveItem(
+        mock_evesdeapi.nearest_celestial.return_value = evesdeapi.EveItem(
             id=50016284, name="Stargate (Akidagi)", type_id=16, distance=1000
         )
         enaluri, _ = EveSolarSystem.objects.get_or_create_esi(id=30045339)
         # when
         result = enaluri.nearest_celestial(x=-1, y=-2, z=3)
         # then
         self.assertEqual(result.eve_type, EveType.objects.get_or_create_esi(id=16)[0])
         self.assertEqual(
             result.eve_object, EveStargate.objects.get_or_create_esi(id=50016284)[0]
         )
         self.assertEqual(result.distance, 1000)
 
-    def test_should_return_planet(self, mock_esi, mock_evemicros):
+    def test_should_return_star(self, mock_esi, mock_evesdeapi):
+        # given
+        mock_esi.client = EsiClientStub()
+        mock_evesdeapi.nearest_celestial.return_value = evesdeapi.EveItem(
+            id=40349466, name="StaEnaluri - Star", type_id=3800, distance=0
+        )
+        enaluri, _ = EveSolarSystem.objects.get_or_create_esi(id=30045339)
+        # when
+        result = enaluri.nearest_celestial(x=0, y=0, z=0)
+        # then
+        self.assertEqual(result.eve_type, EveType.objects.get_or_create_esi(id=3800)[0])
+        self.assertEqual(
+            result.eve_object, EveStar.objects.get_or_create_esi(id=40349466)[0]
+        )
+        self.assertEqual(result.distance, 0)
+
+    def test_should_return_planet(self, mock_esi, mock_evesdeapi):
         # given
         mock_esi.client = EsiClientStub()
-        mock_evemicros.nearest_celestial.return_value = evemicros.EveItem(
+        mock_evesdeapi.nearest_celestial.return_value = evesdeapi.EveItem(
             id=40349471, name="Enaluri III", type_id=13, distance=1000
         )
         enaluri, _ = EveSolarSystem.objects.get_or_create_esi(id=30045339)
         # when
         result = enaluri.nearest_celestial(x=-1, y=-2, z=3)
         # then
         self.assertEqual(result.eve_type, EveType.objects.get_or_create_esi(id=13)[0])
         self.assertEqual(
             result.eve_object, EvePlanet.objects.get_or_create_esi(id=40349471)[0]
         )
         self.assertEqual(result.distance, 1000)
 
-    def test_should_return_station(self, mock_esi, mock_evemicros):
+    def test_should_return_station(self, mock_esi, mock_evesdeapi):
         # given
         mock_esi.client = EsiClientStub()
-        mock_evemicros.nearest_celestial.return_value = evemicros.EveItem(
+        mock_evesdeapi.nearest_celestial.return_value = evesdeapi.EveItem(
             id=60015068,
             name="Enaluri V - State Protectorate Assembly Plant",
             type_id=1529,
             distance=1000,
         )
         enaluri, _ = EveSolarSystem.objects.get_or_create_esi(id=30045339)
         # when
@@ -960,18 +984,18 @@
         # then
         self.assertEqual(result.eve_type, EveType.objects.get_or_create_esi(id=1529)[0])
         self.assertEqual(
             result.eve_object, EveStation.objects.get_or_create_esi(id=60015068)[0]
         )
         self.assertEqual(result.distance, 1000)
 
-    def test_should_return_asteroid_belt(self, mock_esi, mock_evemicros):
+    def test_should_return_asteroid_belt(self, mock_esi, mock_evesdeapi):
         # given
         mock_esi.client = EsiClientStub()
-        mock_evemicros.nearest_celestial.return_value = evemicros.EveItem(
+        mock_evesdeapi.nearest_celestial.return_value = evesdeapi.EveItem(
             id=40349487, name="Enaluri III - Asteroid Belt 1", type_id=15, distance=1000
         )
         enaluri, _ = EveSolarSystem.objects.get_or_create_esi(id=30045339)
         # when
         result = enaluri.nearest_celestial(x=-1, y=-2, z=3)
         # then
         self.assertEqual(
@@ -979,190 +1003,60 @@
             EveType.objects.get_or_create_esi(id=15)[0],
         )
         self.assertEqual(
             result.eve_object, EveAsteroidBelt.objects.get_or_create_esi(id=40349487)[0]
         )
         self.assertEqual(result.distance, 1000)
 
-    def test_should_return_moon(self, mock_esi, mock_evemicros):
+    def test_should_return_moon(self, mock_esi, mock_evesdeapi):
         # given
         mock_esi.client = EsiClientStub()
-        mock_evemicros.nearest_celestial.return_value = evemicros.EveItem(
+        mock_evesdeapi.nearest_celestial.return_value = evesdeapi.EveItem(
             id=40349472, name="Enaluri III - Moon 1", type_id=14, distance=1000
         )
         enaluri, _ = EveSolarSystem.objects.get_or_create_esi(id=30045339)
         # when
         result = enaluri.nearest_celestial(x=-1, y=-2, z=3)
         # then
         self.assertEqual(result.eve_type, EveType.objects.get_or_create_esi(id=14)[0])
         self.assertEqual(
             result.eve_object, EveMoon.objects.get_or_create_esi(id=40349472)[0]
         )
         self.assertEqual(result.distance, 1000)
 
-    def test_should_return_none_if_unknown_type(self, mock_esi, mock_evemicros):
+    def test_should_return_none_if_unknown_type(self, mock_esi, mock_evesdeapi):
         # given
         mock_esi.client = EsiClientStub()
-        mock_evemicros.nearest_celestial.return_value = evemicros.EveItem(
+        mock_evesdeapi.nearest_celestial.return_value = evesdeapi.EveItem(
             id=99, name="Merlin", type_id=603, distance=1000
         )
         enaluri, _ = EveSolarSystem.objects.get_or_create_esi(id=30045339)
         # when
         result = enaluri.nearest_celestial(x=-1, y=-2, z=3)
         # then
         self.assertIsNone(result)
 
-    def test_should_return_none_if_not_found(self, mock_esi, mock_evemicros):
+    def test_should_return_none_if_not_found(self, mock_esi, mock_evesdeapi):
         # given
         mock_esi.client = EsiClientStub()
-        mock_evemicros.nearest_celestial.return_value = None
+        mock_evesdeapi.nearest_celestial.return_value = None
         enaluri, _ = EveSolarSystem.objects.get_or_create_esi(id=30045339)
         # when
         result = enaluri.nearest_celestial(x=-1, y=-2, z=3)
         # then
         self.assertIsNone(result)
 
-    def test_should_return_moon_by_group(self, mock_esi, mock_evemicros):
+    def test_should_return_moon_by_group(self, mock_esi, mock_evesdeapi):
         # given
         mock_esi.client = EsiClientStub()
-        mock_evemicros.nearest_celestial.return_value = evemicros.EveItem(
+        mock_evesdeapi.nearest_celestial.return_value = evesdeapi.EveItem(
             id=40349472, name="Enaluri III - Moon 1", type_id=14, distance=1000
         )
         enaluri, _ = EveSolarSystem.objects.get_or_create_esi(id=30045339)
         # when
         result = enaluri.nearest_celestial(x=-1, y=-2, z=3, group_id=EveGroupId.MOON)
         # then
         self.assertEqual(result.eve_type, EveType.objects.get_or_create_esi(id=14)[0])
         self.assertEqual(
             result.eve_object, EveMoon.objects.get_or_create_esi(id=40349472)[0]
         )
         self.assertEqual(result.distance, 1000)
-
-
-@override_settings(CELERY_ALWAYS_EAGER=True)
-@patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_GRAPHICS", False)
-@patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_DOGMAS", False)
-@patch(MODELS_PATH + ".EVEUNIVERSE_LOAD_MARKET_GROUPS", False)
-@patch(MANAGERS_PATH + ".esi")
-class EveCategoryUpdateAll(NoSocketsTestCase):
-    def test_should_update_without_children_and_sync(self, mock_esi):
-        # given
-        mock_esi.client = EsiClientStub()
-        # when
-        EveCategory.objects.update_or_create_all_esi(
-            include_children=False, wait_for_children=True
-        )
-        # then
-        self.assertSetEqual(
-            set(EveCategory.objects.values_list("id", flat=True)),
-            {2, 3, 4, 6, 9, 17, 65, 91},
-        )
-        self.assertEqual(EveGroup.objects.count(), 0)
-        self.assertEqual(EveType.objects.count(), 0)
-
-    def test_should_update_with_children_and_sync(self, mock_esi):
-        # given
-        mock_esi.client = EsiClientStub()
-        # when
-        EveCategory.objects.update_or_create_all_esi(
-            include_children=True, wait_for_children=True
-        )
-        # then
-        self.assertSetEqual(
-            set(EveCategory.objects.values_list("id", flat=True)),
-            {2, 3, 4, 6, 9, 17, 65, 91},
-        )
-        self.assertSetEqual(
-            set(EveGroup.objects.values_list("id", flat=True)),
-            {6, 7, 8, 9, 10, 105, 15, 18, 536, 25, 26, 1404, 1950},
-        )
-        self.assertSetEqual(
-            set(EveType.objects.values_list("id", flat=True)),
-            {
-                13,
-                14,
-                15,
-                16,
-                34,
-                35,
-                36,
-                37,
-                38,
-                39,
-                40,
-                34599,
-                950,
-                21947,
-                29627,
-                21949,
-                21951,
-                21953,
-                21955,
-                21957,
-                21959,
-                21961,
-                21967,
-                3800,
-                603,
-                608,
-                2016,
-                621,
-                45038,
-                35825,
-                626,
-                1529,
-            },
-        )
-
-    def test_should_update_with_children_and_async(self, mock_esi):
-        # given
-        mock_esi.client = EsiClientStub()
-        # when
-        EveCategory.objects.update_or_create_all_esi(
-            include_children=True, wait_for_children=False
-        )
-        # then
-        self.assertSetEqual(
-            set(EveCategory.objects.values_list("id", flat=True)),
-            {2, 3, 4, 6, 9, 17, 65, 91},
-        )
-        self.assertSetEqual(
-            set(EveGroup.objects.values_list("id", flat=True)),
-            {6, 7, 8, 9, 10, 105, 15, 18, 536, 25, 26, 1404, 1950},
-        )
-        self.assertSetEqual(
-            set(EveType.objects.values_list("id", flat=True)),
-            {
-                13,
-                14,
-                15,
-                16,
-                34,
-                35,
-                36,
-                37,
-                38,
-                39,
-                40,
-                34599,
-                950,
-                21947,
-                29627,
-                21949,
-                21951,
-                21953,
-                21955,
-                21957,
-                21959,
-                21961,
-                21967,
-                3800,
-                603,
-                608,
-                2016,
-                621,
-                45038,
-                35825,
-                626,
-                1529,
-            },
-        )
```

### Comparing `django-eveuniverse-0.9.0/eveuniverse/tests/test_tasks.py` & `django_eveuniverse-1.0.0a1/eveuniverse/tests/test_tasks.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,68 @@
 from unittest.mock import patch
 
 from django.test import TestCase
 from django.test.utils import override_settings
 
-from ..models import (
+from eveuniverse.models import (
     EveCategory,
     EveConstellation,
     EveDogmaAttribute,
+    EveEntity,
     EveGroup,
     EveRegion,
     EveSolarSystem,
     EveType,
 )
-from ..tasks import (
+from eveuniverse.tasks import (
     create_eve_entities,
+    load_all_types,
     load_eve_object,
     load_map,
     load_ship_types,
     load_structure_types,
     update_market_prices,
     update_or_create_eve_object,
     update_or_create_inline_object,
     update_unresolved_eve_entities,
 )
-from ..utils import NoSocketsTestCase
-from .testdata.esi import EsiClientStub
+from eveuniverse.utils import NoSocketsTestCase
 
-MODULE_PATH = "eveuniverse.tasks"
+from .testdata.esi import BravadoOperationStub, EsiClientStub
+
+TASKS_PATH = "eveuniverse.tasks"
+MANAGERS_PATH = "eveuniverse.managers"
 
 
 class TestTasks(NoSocketsTestCase):
-    @patch("eveuniverse.managers.esi")
+    @patch(MANAGERS_PATH + ".esi")
     def test_load_eve_object(self, mock_esi):
         mock_esi.client = EsiClientStub()
 
         load_eve_object(
             "EveRegion", 10000002, include_children=False, wait_for_children=False
         )
 
         self.assertTrue(EveRegion.objects.filter(id=10000002).exists())
 
-    @patch("eveuniverse.managers.esi")
+    @patch(MANAGERS_PATH + ".esi")
     def test_update_or_create_eve_object(self, mock_esi):
         mock_esi.client = EsiClientStub()
         obj, _ = EveRegion.objects.update_or_create_esi(id=10000002)
         obj.name = "Dummy"
         obj.save()
 
         update_or_create_eve_object(
             "EveRegion", 10000002, include_children=False, wait_for_children=False
         )
 
         obj.refresh_from_db()
         self.assertNotEqual(obj.name, "Dummy")
 
-    @patch("eveuniverse.managers.esi")
+    @patch(MANAGERS_PATH + ".esi")
     def test_update_or_create_inline_object(self, mock_esi):
         mock_esi.client = EsiClientStub()
         eve_type, _ = EveType.objects.update_or_create_esi(id=603)
 
         update_or_create_inline_object(
             parent_obj_id=eve_type.id,
             parent_fk="eve_type",
@@ -73,35 +77,50 @@
             parent_model_name=type(eve_type).__name__,
         )
         dogma_attribute_1 = eve_type.dogma_attributes.filter(
             eve_dogma_attribute=EveDogmaAttribute.objects.get(id=588)
         ).first()
         self.assertEqual(dogma_attribute_1.value, 5)
 
-    @patch(MODULE_PATH + ".EveEntity.objects.bulk_create_esi")
+    @patch(TASKS_PATH + ".EveEntity.objects.bulk_create_esi")
     def test_create_eve_entities(self, mock_bulk_create_esi):
         create_eve_entities([1, 2, 3])
         self.assertTrue(mock_bulk_create_esi.called)
         args, _ = mock_bulk_create_esi.call_args
         self.assertListEqual(args[0], [1, 2, 3])
 
-    @patch(MODULE_PATH + ".EveEntity.objects.bulk_update_new_esi")
-    def test_update_unresolved_eve_entities(self, mock_bulk_update_new_esi):
-        update_unresolved_eve_entities()
-        self.assertTrue(mock_bulk_update_new_esi.called)
-
-    @patch(MODULE_PATH + ".EveMarketPrice.objects.update_from_esi")
+    @patch(TASKS_PATH + ".EveMarketPrice.objects.update_from_esi")
     def test_update_market_prices(self, mock_update_from_esi):
         update_market_prices()
         self.assertTrue(mock_update_from_esi.called)
 
 
-@override_settings(CELERY_ALWAYS_EAGER=True)
-@patch(MODULE_PATH + ".esi")
-@patch("eveuniverse.managers.esi")
+@override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
+@patch(MANAGERS_PATH + ".esi")
+class TestTasks2(TestCase):
+    def test_update_unresolved_eve_entities(self, mock_esi):
+        # given
+        mock_esi.client = EsiClientStub()
+        obj_1 = EveEntity.objects.create(id=1001)
+        obj_2 = EveEntity.objects.create(id=1002)
+        obj_3 = EveEntity.objects.create(id=2001)
+        # when
+        update_unresolved_eve_entities.delay()
+        # then
+        obj_1.refresh_from_db()
+        self.assertEqual(obj_1.category, EveEntity.CATEGORY_CHARACTER)
+        obj_2.refresh_from_db()
+        self.assertEqual(obj_2.category, EveEntity.CATEGORY_CHARACTER)
+        obj_3.refresh_from_db()
+        self.assertEqual(obj_3.category, EveEntity.CATEGORY_CORPORATION)
+
+
+@override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
+@patch(TASKS_PATH + ".esi")
+@patch(MANAGERS_PATH + ".esi")
 class TestLoadData(TestCase):
     def test_load_map(self, mock_esi_1, mock_esi_2):
         mock_esi_1.client = EsiClientStub()
         mock_esi_2.client = EsiClientStub()
         load_map()
 
         for id in [10000002, 10000014, 10000069, 11000031]:
@@ -132,7 +151,45 @@
 
         self.assertTrue(EveCategory.objects.filter(id=65).exists())
         for id in [1404]:
             self.assertTrue(EveGroup.objects.filter(id=id).exists())
 
         for id in [35825]:
             self.assertTrue(EveType.objects.filter(id=id).exists())
+
+
+@patch(TASKS_PATH + ".update_or_create_eve_object")
+@patch(TASKS_PATH + ".esi")
+class TestLoadAllTypes(NoSocketsTestCase):
+    def test_should_load_all_types(self, mock_esi, mock_update_or_create_eve_object):
+        # given
+        mock_esi.client.Universe.get_universe_categories.return_value = (
+            BravadoOperationStub([1, 2])
+        )
+        # when
+        load_all_types()
+        # then
+        self.assertEqual(mock_update_or_create_eve_object.delay.call_count, 2)
+
+    def test_should_abort_when_esi_returns_no_data(
+        self, mock_esi, mock_update_or_create_eve_object
+    ):
+        # given
+        mock_esi.client.Universe.get_universe_categories.return_value = (
+            BravadoOperationStub(None)
+        )
+        # when/then
+        with self.assertRaises(ValueError):
+            load_all_types()
+
+    def test_should_load_all_types_with_enabled_sections(
+        self, mock_esi, mock_update_or_create_eve_object
+    ):
+        # given
+        mock_esi.client.Universe.get_universe_categories.return_value = (
+            BravadoOperationStub([1])
+        )
+        # when
+        load_all_types(["alpha", "bravo"])
+        # then
+        _, kwargs = mock_update_or_create_eve_object.delay.call_args
+        self.assertEqual(kwargs["enabled_sections"], ["alpha", "bravo"])
```

### Comparing `django-eveuniverse-0.9.0/eveuniverse/tests/test_tools_testdata.py` & `django_eveuniverse-1.0.0a1/eveuniverse/tests/test_tools_testdata.py`

 * *Files identical despite different names*

### Comparing `django-eveuniverse-0.9.0/eveuniverse/tests/test_utils.py` & `django_eveuniverse-1.0.0a1/eveuniverse/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from unittest.mock import Mock, patch
 
 import requests
-
 from django.test import TestCase
 
 from ..utils import NoSocketsTestCase, SocketAccessError, chunks, clean_setting
 
 MODULE_PATH = "eveuniverse.utils"
 
 
@@ -98,10 +97,9 @@
             "TEST_SETTING_DUMMY", default_value="alpha", choices=["alpha", "bravo"]
         )
         self.assertEqual(result, "alpha")
 
 
 class TestNoSocketsTestCase(NoSocketsTestCase):
     def test_raises_exception_on_attempted_network_access(self):
-
         with self.assertRaises(SocketAccessError):
             requests.get("https://www.google.com")
```

### Comparing `django-eveuniverse-0.9.0/eveuniverse/tests/testdata/esi.py` & `django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata/esi.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,14 +64,31 @@
                 result = []
                 for id in kwargs["ids"]:
                     if str(id) in esi_data[self._category][self._method]:
                         result.append(esi_data[self._category][self._method][str(id)])
                     else:
                         raise HTTPNotFound(Mock(**{"status_code": 404}))
 
+            elif self._category == "Universe" and self._method == "post_universe_ids":
+                result = {
+                    "agents": None,
+                    "alliances": None,
+                    "characters": None,
+                    "constellations": None,
+                    "corporations": None,
+                    "factions": None,
+                    "inventory_types": None,
+                    "regions": None,
+                    "stations": None,
+                    "systems": None,
+                }
+                for name in kwargs["names"]:
+                    if name in esi_data[self._category][self._method]:
+                        result.update(esi_data[self._category][self._method][name])
+
             else:
                 if len(kwargs) > 0:
                     raise ValueError(
                         f"{self._method} does not have parameter {kwargs.popitem()[0]}"
                     )
                 result = esi_data[self._category][self._method]
 
@@ -129,14 +146,15 @@
             EsiEndpoint("Universe", "get_universe_stars_star_id", "star_id"),
             EsiEndpoint("Universe", "get_universe_stations_station_id", "station_id"),
             EsiEndpoint("Universe", "get_universe_systems", None),
             EsiEndpoint("Universe", "get_universe_systems_system_id", "system_id"),
             EsiEndpoint("Universe", "get_universe_types_type_id", "type_id"),
             EsiEndpoint("Universe", "get_universe_types", None),
             EsiEndpoint("Universe", "post_universe_names", None),
+            EsiEndpoint("Universe", "post_universe_ids", None),
         ]
         for endpoint in esi_endpoints:
             if not hasattr(cls, endpoint.category):
                 setattr(
                     cls, endpoint.category, type(endpoint.category, (object,), dict())
                 )
             my_category = getattr(cls, endpoint.category)
```

### Comparing `django-eveuniverse-0.9.0/eveuniverse/tests/testdata/factories.py` & `django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata/factories.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-items = {
+from ...models import EveEntity
+
+_items = {
     40170698: {
         "itemID": 40170698,
         "itemName": "Colelie VI - Asteroid Belt 1",
         "typeID": 15,
         "typeName": "Asteroid Belt",
         "groupID": 9,
         "groupName": "Asteroid Belt",
@@ -100,16 +102,44 @@
         "security": 0.51238882808862296069918329521897248923778533935546875,
         "distance": 4.70300000000000029132252166164107620716094970703125,
         "distanceKm": 703551499,
     },
 }
 
 
-def create_evemicros_item(item_id):
-    return items[item_id]
+def _create_evemicros_item(item_id):
+    return _items[item_id]
 
 
-def create_evemicros_request(*item_ids, ok=True):
+def create_evemicros_response(*item_ids, ok=True):
     return {
         "ok": ok,
-        "result": [create_evemicros_item(item_id) for item_id in item_ids],
+        "result": [_create_evemicros_item(item_id) for item_id in item_ids],
+    }
+
+
+def create_eve_entity(**kwargs):
+    if "category" not in kwargs:
+        kwargs["category"] = EveEntity.CATEGORY_CHARACTER
+    return EveEntity.objects.create(**kwargs)
+
+
+def create_evesdeapi_response(*item_ids):
+    return [_create_evesdeapi_item(item_id) for item_id in item_ids]
+
+
+def _create_evesdeapi_item(item_id):
+    item = _items[item_id]
+    return {
+        "distance": item["distanceKm"],
+        "group_id": item["groupID"],
+        "group_name": item["groupName"],
+        "item_id": item["itemID"],
+        "name": item["itemName"],
+        "position": {
+            "x": item["x"],
+            "y": item["y"],
+            "z": item["z"],
+        },
+        "type_id": item["typeID"],
+        "type_name": item["typeName"],
     }
```

### Comparing `django-eveuniverse-0.9.0/eveuniverse/tests/testdata/fetch_esi_raw_data.py` & `django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata/fetch_esi_raw_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import json
 from pathlib import Path
 
 import requests
 
+from eveuniverse.app_settings import EVEUNIVERSE_REQUESTS_DEFAULT_TIMEOUT
+
 TYPE_IDS = [
     34,
     35,
     36,
     37,
     38,
     39,
@@ -26,32 +28,39 @@
 
 # fetching types from ESI
 esi_data = {"categories": dict(), "groups": dict(), "types": dict()}
 category_ids = set()
 group_ids = set()
 print("Fetching types...")
 for type_id in TYPE_IDS:
-    r = requests.get(f"https://esi.evetech.net/latest/universe/types/{type_id}/")
+    r = requests.get(
+        f"https://esi.evetech.net/latest/universe/types/{type_id}/",
+        timeout=EVEUNIVERSE_REQUESTS_DEFAULT_TIMEOUT,
+    )
     r.raise_for_status()
     info = r.json()
     esi_data["types"][type_id] = info
     group_ids.add(info["group_id"])
 
 print("Fetching groups...")
 for group_id in group_ids:
-    r = requests.get(f"https://esi.evetech.net/latest/universe/groups/{group_id}/")
+    r = requests.get(
+        f"https://esi.evetech.net/latest/universe/groups/{group_id}/",
+        timeout=EVEUNIVERSE_REQUESTS_DEFAULT_TIMEOUT,
+    )
     r.raise_for_status()
     info = r.json()
     esi_data["groups"][group_id] = info
     category_ids.add(info["category_id"])
 
 print("Fetching categories...")
 for category_id in category_ids:
     r = requests.get(
-        f"https://esi.evetech.net/latest/universe/categories/{category_id}/"
+        f"https://esi.evetech.net/latest/universe/categories/{category_id}/",
+        timeout=EVEUNIVERSE_REQUESTS_DEFAULT_TIMEOUT,
     )
     r.raise_for_status()
     info = r.json()
     esi_data["categories"][category_id] = info
 
 # writing raw data
 esi_data_path = Path(__file__).parent / "esi_raw_data.json"
```

### Comparing `django-eveuniverse-0.9.0/eveuniverse/tests/testdata/generate_sde.py` & `django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata/generate_sde.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 import requests
 
 print("Generating SDE data...")
 
 # fetch type materials from SDE bridge
-r = requests.get("https://sde.zzeve.com/invTypeMaterials.json")
+r = requests.get("https://sde.eve-o.tech/latest/invTypeMaterials.json")
 r.raise_for_status()
 data_all = r.json()
 
 # fetch type IDs from current test data
 esi_data_path = Path(__file__).parent / "esi_data.json"
 with esi_data_path.open("r", encoding="utf-8") as fp:
     esi_data = json.load(fp)
```

### Comparing `django-eveuniverse-0.9.0/eveuniverse/tests/testdata/sde.py` & `django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata/sde.py`

 * *Files identical despite different names*

### Comparing `django-eveuniverse-0.9.0/eveuniverse/tools/drop_tables.sql` & `django_eveuniverse-1.0.0a1/eveuniverse/tools/drop_tables.sql`

 * *Files identical despite different names*

### Comparing `django-eveuniverse-0.9.0/eveuniverse/tools/testdata.py` & `django_eveuniverse-1.0.0a1/eveuniverse/tools/testdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import logging
 from collections import OrderedDict, namedtuple
 from copy import deepcopy
 from typing import Iterable, List
 
 from django.core.serializers.json import DjangoJSONEncoder
+
 from eveuniverse.models import EveSolarSystem, EveStargate, EveUniverseBaseModel
 
 from .. import __title__
 from ..core.esitools import is_esi_online
 from ..utils import LoggerAddTag
 
 logger = LoggerAddTag(logging.getLogger(__name__), __title__)
@@ -61,26 +62,30 @@
     if not is_esi_online():
         raise RuntimeError("ESI not online")
 
     # load data per spec
     num = 0
     for model_spec in spec:
         num += 1
+        ids = set(model_spec.ids)
         print(
             f"Loading {num}/{len(spec)}: {model_spec.model_name} with "
-            f"{len(model_spec.ids)} objects... "
+            f"{len(ids)} objects",
+            end="",
         )
         MyModel = EveUniverseBaseModel.get_model_class(model_spec.model_name)
-        for id in model_spec.ids:
+        for id in ids:
+            print(".", end="")
             MyModel.objects.get_or_create_esi(
                 id=id,
                 include_children=model_spec.include_children,
                 wait_for_children=True,
                 enabled_sections=model_spec.enabled_sections,
             )
+        print()
 
     # dump all data into file
     data = OrderedDict()
     for MyModel in EveUniverseBaseModel.all_models():
         if MyModel.objects.count() > 0 and MyModel.__name__ != "EveUnit":
             logger.info(
                 "Collecting %d rows for %s", MyModel.objects.count(), MyModel.__name__
```

### Comparing `django-eveuniverse-0.9.0/eveuniverse/utils.py` & `django_eveuniverse-1.0.0a1/eveuniverse/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,19 +18,14 @@
     def process(self, msg, kwargs):
         return "[%s] %s" % (self.prefix, msg), kwargs
 
 
 logger = LoggerAddTag(logging.getLogger(__name__), __package__)
 
 
-def make_logger_prefix(tag: str):
-    """creates a function to add logger prefix, which returns tag when used empty"""
-    return lambda text="": "{}{}".format(tag, (": " + text) if text else "")
-
-
 def chunks(lst, size):
     """Yield successive sized chunks from lst."""
     for i in range(0, len(lst), size):
         yield lst[i : i + size]
 
 
 def clean_setting(
```

