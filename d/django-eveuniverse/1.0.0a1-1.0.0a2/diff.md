# Comparing `tmp/django_eveuniverse-1.0.0a1.tar.gz` & `tmp/django_eveuniverse-1.0.0a2.tar.gz`

## Comparing `django_eveuniverse-1.0.0a1.tar` & `django_eveuniverse-1.0.0a2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/__init__.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/admin.py
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/app_settings.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/apps.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/backends.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/constants.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/helpers.py
--rw-r--r--   0        0        0    41499 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/managers.py
--rw-r--r--   0        0        0    58930 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/models.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/providers.py
--rw-r--r--   0        0        0   887006 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/swagger.json
--rw-r--r--   0        0        0    10500 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tasks.py
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/core/__init__.py
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/core/dotlan.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/core/esitools.py
--rw-r--r--   0        0        0     5036 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/core/eveimageserver.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/core/eveitems.py
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/core/evemicros.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/core/evesdeapi.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/core/eveskinserver.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/core/evewho.py
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/core/evexml.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/core/zkillboard.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/management/commands/__init__.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/management/commands/eveuniverse_load_data.py
--rw-r--r--   0        0        0     5348 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/management/commands/eveuniverse_load_types.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/management/commands/eveuniverse_purge_data.py
--rw-r--r--   0        0        0    51659 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/migrations/0001_initial.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/migrations/0002_load_eveunit.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/migrations/0003_evemarketprice.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/migrations/0004_effect_longer_name.py
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/migrations/0005_type_materials_and_sections.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/migrations/0006_alter_evedogmaeffectmodifier_operator.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/migrations/0007_evetype_description.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/migrations/__init__.py
--rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/migrations/eve_unit.json
--rw-r--r--   0        0        0    14542 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/static/eveuniverse/skin_generic_128.png
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/static/eveuniverse/skin_generic_32.png
--rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/static/eveuniverse/skin_generic_64.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/__init__.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/pilot.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/test_backends.py
--rw-r--r--   0        0        0    10286 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/test_commands.py
--rw-r--r--   0        0        0    22388 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/test_core.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/test_helpers.py
--rw-r--r--   0        0        0    42399 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/test_models_1.py
--rw-r--r--   0        0        0    28631 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/test_models_2.py
--rw-r--r--   0        0        0    43206 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/test_models_3.py
--rw-r--r--   0        0        0    30849 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/test_models_4.py
--rw-r--r--   0        0        0     6759 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/test_tasks.py
--rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/test_tools_testdata.py
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/test_utils.py
--rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata_example.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata/__init__.py
--rw-r--r--   0        0        0     7725 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata/esi.py
--rw-r--r--   0        0        0    78321 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata/esi_data.json
--rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata/factories.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata/fetch_esi_raw_data.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata/generate_sde.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata/sde.py
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata/sde_data.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/tools/__init__.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tests/tools/clear_celery_once_locks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tools/__init__.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tools/drop_tables.sql
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/eveuniverse/tools/testdata.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/LICENSE
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/README.md
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/__init__.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/admin.py
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/app_settings.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/apps.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/backends.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/constants.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/helpers.py
+-rw-r--r--   0        0        0    41499 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/managers.py
+-rw-r--r--   0        0        0    58930 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/models.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/providers.py
+-rw-r--r--   0        0        0   887006 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/swagger.json
+-rw-r--r--   0        0        0    10500 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tasks.py
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/core/__init__.py
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/core/dotlan.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/core/esitools.py
+-rw-r--r--   0        0        0     5036 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/core/eveimageserver.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/core/eveitems.py
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/core/evemicros.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/core/evesdeapi.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/core/eveskinserver.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/core/evewho.py
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/core/evexml.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/core/zkillboard.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/management/commands/__init__.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/management/commands/eveuniverse_load_data.py
+-rw-r--r--   0        0        0     5348 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/management/commands/eveuniverse_load_types.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/management/commands/eveuniverse_purge_data.py
+-rw-r--r--   0        0        0    51659 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/migrations/0001_initial.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/migrations/0002_load_eveunit.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/migrations/0003_evemarketprice.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/migrations/0004_effect_longer_name.py
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/migrations/0005_type_materials_and_sections.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/migrations/0006_alter_evedogmaeffectmodifier_operator.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/migrations/0007_evetype_description.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/migrations/__init__.py
+-rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/migrations/eve_unit.json
+-rw-r--r--   0        0        0    14542 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/static/eveuniverse/skin_generic_128.png
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/static/eveuniverse/skin_generic_32.png
+-rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/static/eveuniverse/skin_generic_64.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/__init__.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/pilot.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/test_backends.py
+-rw-r--r--   0        0        0    10286 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/test_commands.py
+-rw-r--r--   0        0        0    22388 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/test_core.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/test_helpers.py
+-rw-r--r--   0        0        0    42399 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/test_models_1.py
+-rw-r--r--   0        0        0    28631 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/test_models_2.py
+-rw-r--r--   0        0        0    43206 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/test_models_3.py
+-rw-r--r--   0        0        0    30849 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/test_models_4.py
+-rw-r--r--   0        0        0     6759 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/test_tasks.py
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/test_tools_testdata.py
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/test_utils.py
+-rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata_example.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/__init__.py
+-rw-r--r--   0        0        0     7725 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/esi.py
+-rw-r--r--   0        0        0    78321 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/esi_data.json
+-rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/factories.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/fetch_esi_raw_data.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/generate_sde.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/sde.py
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/sde_data.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/tools/__init__.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tests/tools/clear_celery_once_locks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tools/__init__.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tools/drop_tables.sql
+-rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/eveuniverse/tools/testdata.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/LICENSE
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/README.md
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 django_eveuniverse-1.0.0a2/PKG-INFO
```

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/admin.py` & `django_eveuniverse-1.0.0a2/eveuniverse/admin.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/app_settings.py` & `django_eveuniverse-1.0.0a2/eveuniverse/app_settings.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/backends.py` & `django_eveuniverse-1.0.0a2/eveuniverse/backends.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/helpers.py` & `django_eveuniverse-1.0.0a2/eveuniverse/helpers.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/managers.py` & `django_eveuniverse-1.0.0a2/eveuniverse/managers.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/models.py` & `django_eveuniverse-1.0.0a2/eveuniverse/models.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/swagger.json` & `django_eveuniverse-1.0.0a2/eveuniverse/swagger.json`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/tasks.py` & `django_eveuniverse-1.0.0a2/eveuniverse/tasks.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/utils.py` & `django_eveuniverse-1.0.0a2/eveuniverse/utils.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/core/dotlan.py` & `django_eveuniverse-1.0.0a2/eveuniverse/core/dotlan.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/core/eveimageserver.py` & `django_eveuniverse-1.0.0a2/eveuniverse/core/eveimageserver.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/core/evemicros.py` & `django_eveuniverse-1.0.0a2/eveuniverse/core/evemicros.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/core/evesdeapi.py` & `django_eveuniverse-1.0.0a2/eveuniverse/core/evesdeapi.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/core/evewho.py` & `django_eveuniverse-1.0.0a2/eveuniverse/core/evewho.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/core/evexml.py` & `django_eveuniverse-1.0.0a2/eveuniverse/core/evexml.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/core/zkillboard.py` & `django_eveuniverse-1.0.0a2/eveuniverse/core/zkillboard.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/management/commands/eveuniverse_load_data.py` & `django_eveuniverse-1.0.0a2/eveuniverse/management/commands/eveuniverse_load_data.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/management/commands/eveuniverse_load_types.py` & `django_eveuniverse-1.0.0a2/eveuniverse/management/commands/eveuniverse_load_types.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/management/commands/eveuniverse_purge_data.py` & `django_eveuniverse-1.0.0a2/eveuniverse/management/commands/eveuniverse_purge_data.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/migrations/0001_initial.py` & `django_eveuniverse-1.0.0a2/eveuniverse/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/migrations/0002_load_eveunit.py` & `django_eveuniverse-1.0.0a2/eveuniverse/migrations/0002_load_eveunit.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/migrations/0003_evemarketprice.py` & `django_eveuniverse-1.0.0a2/eveuniverse/migrations/0003_evemarketprice.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/migrations/0005_type_materials_and_sections.py` & `django_eveuniverse-1.0.0a2/eveuniverse/migrations/0005_type_materials_and_sections.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/migrations/eve_unit.json` & `django_eveuniverse-1.0.0a2/eveuniverse/migrations/eve_unit.json`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/static/eveuniverse/skin_generic_128.png` & `django_eveuniverse-1.0.0a2/eveuniverse/static/eveuniverse/skin_generic_128.png`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/static/eveuniverse/skin_generic_32.png` & `django_eveuniverse-1.0.0a2/eveuniverse/static/eveuniverse/skin_generic_32.png`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/static/eveuniverse/skin_generic_64.png` & `django_eveuniverse-1.0.0a2/eveuniverse/static/eveuniverse/skin_generic_64.png`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/tests/pilot.py` & `django_eveuniverse-1.0.0a2/eveuniverse/tests/pilot.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/tests/test_backends.py` & `django_eveuniverse-1.0.0a2/eveuniverse/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/tests/test_commands.py` & `django_eveuniverse-1.0.0a2/eveuniverse/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/tests/test_core.py` & `django_eveuniverse-1.0.0a2/eveuniverse/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/tests/test_helpers.py` & `django_eveuniverse-1.0.0a2/eveuniverse/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/tests/test_models_1.py` & `django_eveuniverse-1.0.0a2/eveuniverse/tests/test_models_1.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/tests/test_models_2.py` & `django_eveuniverse-1.0.0a2/eveuniverse/tests/test_models_2.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/tests/test_models_3.py` & `django_eveuniverse-1.0.0a2/eveuniverse/tests/test_models_3.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/tests/test_models_4.py` & `django_eveuniverse-1.0.0a2/eveuniverse/tests/test_models_4.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/tests/test_tasks.py` & `django_eveuniverse-1.0.0a2/eveuniverse/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/tests/test_tools_testdata.py` & `django_eveuniverse-1.0.0a2/eveuniverse/tests/test_tools_testdata.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/tests/test_utils.py` & `django_eveuniverse-1.0.0a2/eveuniverse/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata_example.json` & `django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata_example.json`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata/esi.py` & `django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/esi.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata/esi_data.json` & `django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/esi_data.json`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata/factories.py` & `django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/factories.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata/fetch_esi_raw_data.py` & `django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/fetch_esi_raw_data.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata/generate_sde.py` & `django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/generate_sde.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata/sde.py` & `django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/sde.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/tests/testdata/sde_data.json` & `django_eveuniverse-1.0.0a2/eveuniverse/tests/testdata/sde_data.json`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/tests/tools/clear_celery_once_locks.py` & `django_eveuniverse-1.0.0a2/eveuniverse/tests/tools/clear_celery_once_locks.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/tools/drop_tables.sql` & `django_eveuniverse-1.0.0a2/eveuniverse/tools/drop_tables.sql`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/eveuniverse/tools/testdata.py` & `django_eveuniverse-1.0.0a2/eveuniverse/tools/testdata.py`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/LICENSE` & `django_eveuniverse-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/README.md` & `django_eveuniverse-1.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `django_eveuniverse-1.0.0a1/pyproject.toml` & `django_eveuniverse-1.0.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 [project.urls]
 Homepage = "https://gitlab.com/ErikKalkoken/django-eveuniverse"
 
 [tool.hatch.version]
 path = "eveuniverse/__init__.py"
 
-[tool.hatch.build.targets.sdist]
+[tool.hatch.build]
 include = [
     "/eveuniverse",
 ]
 
 [tool.isort]
 profile = "black"
```

### Comparing `django_eveuniverse-1.0.0a1/PKG-INFO` & `django_eveuniverse-1.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-eveuniverse
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Complete set of Eve Universe models with on-demand loading from ESI
 Project-URL: Homepage, https://gitlab.com/ErikKalkoken/django-eveuniverse
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

