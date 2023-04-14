# Comparing `tmp/cumulusci-3.9.0.tar.gz` & `tmp/cumulusci-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cumulusci-3.9.0.tar", last modified: Mon Mar 16 21:14:09 2020, max compression
+gzip compressed data, was "dist/cumulusci-3.9.1.tar", last modified: Wed Mar 25 20:17:53 2020, max compression
```

## Comparing `cumulusci-3.9.0.tar` & `cumulusci-3.9.1.tar`

### file list

```diff
@@ -1,457 +1,457 @@
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.126217 cumulusci-3.9.0/
--rw-r--r--   0 runner    (1001) docker     (115)      567 2020-03-16 21:13:58.000000 cumulusci-3.9.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (115)     4438 2020-03-16 21:13:58.000000 cumulusci-3.9.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (115)   120479 2020-03-16 21:13:58.000000 cumulusci-3.9.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (115)     1598 2020-03-16 21:13:58.000000 cumulusci-3.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (115)      452 2020-03-16 21:13:58.000000 cumulusci-3.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (115)   142154 2020-03-16 21:14:09.130217 cumulusci-3.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     1895 2020-03-16 21:13:58.000000 cumulusci-3.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.054218 cumulusci-3.9.0/cumulusci/
--rw-r--r--   0 runner    (1001) docker     (115)      342 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)       43 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.054218 cumulusci-3.9.0/cumulusci/cli/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)    50079 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/cli/cci.py
--rw-r--r--   0 runner    (1001) docker     (115)     1760 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/cli/logger.py
--rw-r--r--   0 runner    (1001) docker     (115)     6100 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/cli/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.058218 cumulusci-3.9.0/cumulusci/cli/tests/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/cli/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)    57805 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/cli/tests/test_cci.py
--rw-r--r--   0 runner    (1001) docker     (115)     1358 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/cli/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (115)     7296 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/cli/tests/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (115)    11771 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/cli/tests/test_ui.py
--rw-r--r--   0 runner    (1001) docker     (115)     4904 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/cli/ui.py
--rw-r--r--   0 runner    (1001) docker     (115)     1079 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.058218 cumulusci-3.9.0/cumulusci/core/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.058218 cumulusci-3.9.0/cumulusci/core/config/
--rw-r--r--   0 runner    (1001) docker     (115)     1298 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/config/BaseConfig.py
--rw-r--r--   0 runner    (1001) docker     (115)     2039 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/config/BaseGlobalConfig.py
--rw-r--r--   0 runner    (1001) docker     (115)     2115 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/config/BaseTaskFlowConfig.py
--rw-r--r--   0 runner    (1001) docker     (115)     6072 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/config/OrgConfig.py
--rw-r--r--   0 runner    (1001) docker     (115)    11868 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/config/ScratchOrgConfig.py
--rw-r--r--   0 runner    (1001) docker     (115)     1239 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)    29059 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/config/project_config.py
--rw-r--r--   0 runner    (1001) docker     (115)     5514 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (115)    26478 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/flowrunner.py
--rw-r--r--   0 runner    (1001) docker     (115)     5827 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/github.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.062218 cumulusci-3.9.0/cumulusci/core/keychain/
--rw-r--r--   0 runner    (1001) docker     (115)     3690 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/keychain/BaseEncryptedProjectKeychain.py
--rw-r--r--   0 runner    (1001) docker     (115)     9101 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/keychain/BaseProjectKeychain.py
--rw-r--r--   0 runner    (1001) docker     (115)     4202 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/keychain/EncryptedFileProjectKeychain.py
--rw-r--r--   0 runner    (1001) docker     (115)     1847 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/keychain/EnvironmentProjectKeychain.py
--rw-r--r--   0 runner    (1001) docker     (115)      591 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/keychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     3051 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/runtime.py
--rw-r--r--   0 runner    (1001) docker     (115)     1868 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/sfdx.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.062218 cumulusci-3.9.0/cumulusci/core/source/
--rw-r--r--   0 runner    (1001) docker     (115)      239 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     4586 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/source/github.py
--rw-r--r--   0 runner    (1001) docker     (115)      785 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/source/local_folder.py
--rw-r--r--   0 runner    (1001) docker     (115)     7444 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/tasks.py
--rw-r--r--   0 runner    (1001) docker     (115)     1455 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/template_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.066218 cumulusci-3.9.0/cumulusci/core/tests/
--rw-r--r--   0 runner    (1001) docker     (115)      479 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/tests/BarTestPage.py
--rw-r--r--   0 runner    (1001) docker     (115)      324 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/tests/FooTestPage.py
--rw-r--r--   0 runner    (1001) docker     (115)       56 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)    42173 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (115)    25741 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/tests/test_config_expensive.py
--rw-r--r--   0 runner    (1001) docker     (115)      558 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (115)    19750 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/tests/test_flowrunner.py
--rw-r--r--   0 runner    (1001) docker     (115)     9611 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (115)    19646 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/tests/test_keychain.py
--rw-r--r--   0 runner    (1001) docker     (115)     4646 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/tests/test_pageobjects.py
--rw-r--r--   0 runner    (1001) docker     (115)     3483 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/tests/test_salesforce.py
--rw-r--r--   0 runner    (1001) docker     (115)     2826 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/tests/test_salesforce_locators.py
--rw-r--r--   0 runner    (1001) docker     (115)     1136 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/tests/test_sfdx.py
--rw-r--r--   0 runner    (1001) docker     (115)    16216 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/tests/test_source.py
--rw-r--r--   0 runner    (1001) docker     (115)     7180 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (115)     3759 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (115)     3036 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (115)     5715 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (115)    37971 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/cumulusci.yml
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.066218 cumulusci-3.9.0/cumulusci/files/
--rw-r--r--   0 runner    (1001) docker     (115)      457 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/files/admin_profile.xml
--rw-r--r--   0 runner    (1001) docker     (115)     9909 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/files/metadata_whitelist.txt
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.046218 cumulusci-3.9.0/cumulusci/files/templates/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.066218 cumulusci-3.9.0/cumulusci/files/templates/project/
--rw-r--r--   0 runner    (1001) docker     (115)      343 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/files/templates/project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (115)      424 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/files/templates/project/README.md
--rw-r--r--   0 runner    (1001) docker     (115)     1699 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/files/templates/project/cumulusci.yml
--rw-r--r--   0 runner    (1001) docker     (115)     1126 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/files/templates/project/mapping.yml
--rw-r--r--   0 runner    (1001) docker     (115)      567 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/files/templates/project/scratch_def.json
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.066218 cumulusci-3.9.0/cumulusci/oauth/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/oauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)      116 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/oauth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (115)     6847 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/oauth/salesforce.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.066218 cumulusci-3.9.0/cumulusci/oauth/tests/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/oauth/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     6150 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/oauth/tests/test_salesforce.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.070218 cumulusci-3.9.0/cumulusci/robotframework/
--rw-r--r--   0 runner    (1001) docker     (115)     9370 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/CumulusCI.py
--rw-r--r--   0 runner    (1001) docker     (115)      123 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/CumulusCI.robot
--rw-r--r--   0 runner    (1001) docker     (115)    42214 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/Salesforce.py
--rw-r--r--   0 runner    (1001) docker     (115)     4870 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/Salesforce.robot
--rw-r--r--   0 runner    (1001) docker     (115)      111 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     5142 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/locator_manager.py
--rw-r--r--   0 runner    (1001) docker     (115)     3957 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/locators_45.py
--rw-r--r--   0 runner    (1001) docker     (115)      717 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/locators_46.py
--rw-r--r--   0 runner    (1001) docker     (115)      486 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/locators_47.py
--rw-r--r--   0 runner    (1001) docker     (115)     1714 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/locators_48.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.070218 cumulusci-3.9.0/cumulusci/robotframework/pageobjects/
--rw-r--r--   0 runner    (1001) docker     (115)     9938 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/pageobjects/BasePageObjects.py
--rw-r--r--   0 runner    (1001) docker     (115)     1418 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/pageobjects/PageObjectLibrary.py
--rw-r--r--   0 runner    (1001) docker     (115)    13060 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/pageobjects/PageObjects.py
--rw-r--r--   0 runner    (1001) docker     (115)      336 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/pageobjects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     4011 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/pageobjects/baseobjects.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.046218 cumulusci-3.9.0/cumulusci/robotframework/perftests/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.070218 cumulusci-3.9.0/cumulusci/robotframework/perftests/short/
--rw-r--r--   0 runner    (1001) docker     (115)     4066 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/perftests/short/collection_perf.robot
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.070218 cumulusci-3.9.0/cumulusci/robotframework/tests/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.074218 cumulusci-3.9.0/cumulusci/robotframework/tests/cumulusci/
--rw-r--r--   0 runner    (1001) docker     (115)      995 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/tests/cumulusci/base.robot
--rw-r--r--   0 runner    (1001) docker     (115)     1160 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/tests/cumulusci/bulkdata.robot
--rw-r--r--   0 runner    (1001) docker     (115)     2301 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/tests/cumulusci/communities.robot
--rw-r--r--   0 runner    (1001) docker     (115)     3306 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/tests/cumulusci/datagen.robot
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.074218 cumulusci-3.9.0/cumulusci/robotframework/tests/salesforce/
--rw-r--r--   0 runner    (1001) docker     (115)      539 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/tests/salesforce/TestLibraryA.py
--rw-r--r--   0 runner    (1001) docker     (115)      487 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/tests/salesforce/TestLibraryB.py
--rw-r--r--   0 runner    (1001) docker     (115)     3499 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/tests/salesforce/TestListener.py
--rw-r--r--   0 runner    (1001) docker     (115)     4920 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/tests/salesforce/api.robot
--rw-r--r--   0 runner    (1001) docker     (115)     4199 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/tests/salesforce/browsers.robot
--rw-r--r--   0 runner    (1001) docker     (115)     1821 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/tests/salesforce/create_contact.robot
--rw-r--r--   0 runner    (1001) docker     (115)     1900 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/tests/salesforce/locators.robot
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.074218 cumulusci-3.9.0/cumulusci/robotframework/tests/salesforce/pageobjects/
--rw-r--r--   0 runner    (1001) docker     (115)     3635 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/tests/salesforce/pageobjects/base_pageobjects.robot
--rw-r--r--   0 runner    (1001) docker     (115)      761 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/tests/salesforce/pageobjects/example_page_object.py
--rw-r--r--   0 runner    (1001) docker     (115)     6149 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/tests/salesforce/pageobjects/pageobjects.robot
--rw-r--r--   0 runner    (1001) docker     (115)     3621 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/tests/salesforce/populate.robot
--rw-r--r--   0 runner    (1001) docker     (115)     1423 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/tests/salesforce/test_testlistener.py
--rw-r--r--   0 runner    (1001) docker     (115)     7955 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/tests/salesforce/ui.robot
--rw-r--r--   0 runner    (1001) docker     (115)     5254 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/tests/test_locator_manager.py
--rw-r--r--   0 runner    (1001) docker     (115)     1872 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/tests/test_template_util.py
--rw-r--r--   0 runner    (1001) docker     (115)     1055 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (115)     7675 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/robotframework/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.078218 cumulusci-3.9.0/cumulusci/salesforce_api/
--rw-r--r--   0 runner    (1001) docker     (115)       56 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/salesforce_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)      525 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/salesforce_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (115)    24173 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/salesforce_api/metadata.py
--rw-r--r--   0 runner    (1001) docker     (115)     4473 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/salesforce_api/package_zip.py
--rw-r--r--   0 runner    (1001) docker     (115)     5769 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/salesforce_api/soap_envelopes.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.078218 cumulusci-3.9.0/cumulusci/salesforce_api/tests/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/salesforce_api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     4748 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/salesforce_api/tests/metadata_test_strings.py
--rw-r--r--   0 runner    (1001) docker     (115)    37472 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/salesforce_api/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (115)     2517 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/salesforce_api/tests/test_package_zip.py
--rw-r--r--   0 runner    (1001) docker     (115)     3184 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/salesforce_api/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (115)     1151 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/salesforce_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.078218 cumulusci-3.9.0/cumulusci/tasks/
--rw-r--r--   0 runner    (1001) docker     (115)       56 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.078218 cumulusci-3.9.0/cumulusci/tasks/apex/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/apex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     5289 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/apex/anon.py
--rw-r--r--   0 runner    (1001) docker     (115)     6001 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/apex/batch.py
--rw-r--r--   0 runner    (1001) docker     (115)    23999 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/apex/testrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.078218 cumulusci-3.9.0/cumulusci/tasks/apex/tests/
--rw-r--r--   0 runner    (1001) docker     (115)    39096 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/apex/tests/test_apex_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.082218 cumulusci-3.9.0/cumulusci/tasks/bulkdata/
--rw-r--r--   0 runner    (1001) docker     (115)      485 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     3329 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/base_generate_data_task.py
--rw-r--r--   0 runner    (1001) docker     (115)     4364 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/delete.py
--rw-r--r--   0 runner    (1001) docker     (115)    11631 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/extract.py
--rw-r--r--   0 runner    (1001) docker     (115)     4021 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/factory_utils.py
--rw-r--r--   0 runner    (1001) docker     (115)      107 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/generate.py
--rw-r--r--   0 runner    (1001) docker     (115)     8286 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/generate_and_load_data.py
--rw-r--r--   0 runner    (1001) docker     (115)      706 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/generate_and_load_data_from_yaml.py
--rw-r--r--   0 runner    (1001) docker     (115)     7068 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/generate_from_yaml.py
--rw-r--r--   0 runner    (1001) docker     (115)    15262 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/generate_mapping.py
--rw-r--r--   0 runner    (1001) docker     (115)    18556 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/load.py
--rw-r--r--   0 runner    (1001) docker     (115)     1780 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/mapping_parser.py
--rw-r--r--   0 runner    (1001) docker     (115)    11200 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/step.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.086217 cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     1333 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/dummy_data_factory.py
--rw-r--r--   0 runner    (1001) docker     (115)     1723 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/mapping-oid.yml
--rw-r--r--   0 runner    (1001) docker     (115)      685 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/mapping_after.yml
--rw-r--r--   0 runner    (1001) docker     (115)      547 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/mapping_v1.yml
--rw-r--r--   0 runner    (1001) docker     (115)      421 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/mapping_v2.yml
--rw-r--r--   0 runner    (1001) docker     (115)     1561 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/mapping_vanilla_sf.yml
--rw-r--r--   0 runner    (1001) docker     (115)      353 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/mock_data_factory_without_mapping.py
--rw-r--r--   0 runner    (1001) docker     (115)      143 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/recordtypes.yml
--rw-r--r--   0 runner    (1001) docker     (115)       83 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/simple_snowfakery.yml
--rw-r--r--   0 runner    (1001) docker     (115)     2173 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/test_base_generate_data_tasks.py
--rw-r--r--   0 runner    (1001) docker     (115)    12123 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (115)    21612 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (115)     1514 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/test_factory_utils.py
--rw-r--r--   0 runner    (1001) docker     (115)     8045 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/test_generate_and_load.py
--rw-r--r--   0 runner    (1001) docker     (115)    21868 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/test_generatemapping.py
--rw-r--r--   0 runner    (1001) docker     (115)    35577 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (115)     1976 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/test_mapping_parser.py
--rw-r--r--   0 runner    (1001) docker     (115)    18552 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/test_step.py
--rw-r--r--   0 runner    (1001) docker     (115)     6389 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.086217 cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/tests/
--rw-r--r--   0 runner    (1001) docker     (115)     9348 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/tests/test_generate_from_snowfakery_task.py
--rw-r--r--   0 runner    (1001) docker     (115)      670 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (115)     6157 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/bulkdata/utils.py
--rw-r--r--   0 runner    (1001) docker     (115)     6801 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/command.py
--rw-r--r--   0 runner    (1001) docker     (115)     7025 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/connectedapp.py
--rw-r--r--   0 runner    (1001) docker     (115)    11541 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/datadictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.090217 cumulusci-3.9.0/cumulusci/tasks/github/
--rw-r--r--   0 runner    (1001) docker     (115)      373 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)      574 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/github/base.py
--rw-r--r--   0 runner    (1001) docker     (115)     8662 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/github/merge.py
--rw-r--r--   0 runner    (1001) docker     (115)      269 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/github/pull_request.py
--rw-r--r--   0 runner    (1001) docker     (115)     3462 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/github/release.py
--rw-r--r--   0 runner    (1001) docker     (115)     4106 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/github/release_report.py
--rw-r--r--   0 runner    (1001) docker     (115)     1505 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/github/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.090217 cumulusci-3.9.0/cumulusci/tasks/github/tests/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/github/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)    17647 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/github/tests/test_merge.py
--rw-r--r--   0 runner    (1001) docker     (115)     1022 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/github/tests/test_pull_request.py
--rw-r--r--   0 runner    (1001) docker     (115)     4996 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/github/tests/test_release.py
--rw-r--r--   0 runner    (1001) docker     (115)     3589 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/github/tests/test_release_report.py
--rw-r--r--   0 runner    (1001) docker     (115)     3206 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/github/tests/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (115)     5777 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/github/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (115)    21440 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/github/tests/util_github_api.py
--rw-r--r--   0 runner    (1001) docker     (115)     9030 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/github/util.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.090217 cumulusci-3.9.0/cumulusci/tasks/metadata/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     3191 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/metadata/ee_src.py
--rw-r--r--   0 runner    (1001) docker     (115)     3312 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/metadata/managed_src.py
--rw-r--r--   0 runner    (1001) docker     (115)    16147 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/metadata/metadata_map.yml
--rw-r--r--   0 runner    (1001) docker     (115)     4147 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/metadata/modify.py
--rw-r--r--   0 runner    (1001) docker     (115)    12998 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/metadata/package.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.090217 cumulusci-3.9.0/cumulusci/tasks/metadata/tests/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/metadata/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.046218 cumulusci-3.9.0/cumulusci/tasks/metadata/tests/package_metadata/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.090217 cumulusci-3.9.0/cumulusci/tasks/metadata/tests/package_metadata/namespaced_report_folder/
--rw-r--r--   0 runner    (1001) docker     (115)      287 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/metadata/tests/package_metadata/namespaced_report_folder/destructiveChanges.xml
--rw-r--r--   0 runner    (1001) docker     (115)      286 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/metadata/tests/package_metadata/namespaced_report_folder/package.xml
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.046218 cumulusci-3.9.0/cumulusci/tasks/metadata/tests/package_metadata/namespaced_report_folder/reports/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.090217 cumulusci-3.9.0/cumulusci/tasks/metadata/tests/package_metadata/namespaced_report_folder/reports/namespace__TestFolder/
--rw-r--r--   0 runner    (1001) docker     (115)      106 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/metadata/tests/package_metadata/namespaced_report_folder/reports/namespace__TestFolder/TestReport.report
--rw-r--r--   0 runner    (1001) docker     (115)      287 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/metadata/tests/sample_package.xml
--rw-r--r--   0 runner    (1001) docker     (115)     3366 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/metadata/tests/test_ee_src.py
--rw-r--r--   0 runner    (1001) docker     (115)     3280 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/metadata/tests/test_managed_src.py
--rw-r--r--   0 runner    (1001) docker     (115)     4842 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/metadata/tests/test_modify.py
--rw-r--r--   0 runner    (1001) docker     (115)    12611 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/metadata/tests/test_package.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.090217 cumulusci-3.9.0/cumulusci/tasks/metadata_etl/
--rw-r--r--   0 runner    (1001) docker     (115)      749 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/metadata_etl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)    10869 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/metadata_etl/base.py
--rw-r--r--   0 runner    (1001) docker     (115)     2321 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/metadata_etl/layouts.py
--rw-r--r--   0 runner    (1001) docker     (115)     4361 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/metadata_etl/permissions.py
--rw-r--r--   0 runner    (1001) docker     (115)     5127 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/metadata_etl/sharing.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.094217 cumulusci-3.9.0/cumulusci/tasks/metadata_etl/tests/
--rw-r--r--   0 runner    (1001) docker     (115)    12677 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/metadata_etl/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (115)     5796 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/metadata_etl/tests/test_layouts.py
--rw-r--r--   0 runner    (1001) docker     (115)     7059 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/metadata_etl/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (115)     8716 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/metadata_etl/tests/test_sharing.py
--rw-r--r--   0 runner    (1001) docker     (115)     8728 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/metadata_etl/tests/test_value_sets.py
--rw-r--r--   0 runner    (1001) docker     (115)     2922 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/metadata_etl/value_sets.py
--rw-r--r--   0 runner    (1001) docker     (115)     9440 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/metadeploy.py
--rw-r--r--   0 runner    (1001) docker     (115)     3426 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/metaxml.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.094217 cumulusci-3.9.0/cumulusci/tasks/push/
--rw-r--r--   0 runner    (1001) docker     (115)     3759 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/push/README.md
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/push/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)    25003 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/push/push_api.py
--rw-r--r--   0 runner    (1001) docker     (115)     5447 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/push/pushfails.py
--rw-r--r--   0 runner    (1001) docker     (115)    15651 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/push/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.094217 cumulusci-3.9.0/cumulusci/tasks/push/tests/
--rw-r--r--   0 runner    (1001) docker     (115)     4888 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/push/tests/test_push_api.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.094217 cumulusci-3.9.0/cumulusci/tasks/release_notes/
--rw-r--r--   0 runner    (1001) docker     (115)     2132 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/release_notes/README.md
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/release_notes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)      179 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/release_notes/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (115)    10962 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/release_notes/generator.py
--rw-r--r--   0 runner    (1001) docker     (115)     9581 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/release_notes/parser.py
--rw-r--r--   0 runner    (1001) docker     (115)     6885 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/release_notes/provider.py
--rw-r--r--   0 runner    (1001) docker     (115)     8831 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/release_notes/task.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.094217 cumulusci-3.9.0/cumulusci/tasks/release_notes/tests/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/release_notes/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.050218 cumulusci-3.9.0/cumulusci/tasks/release_notes/tests/change_notes/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.094217 cumulusci-3.9.0/cumulusci/tasks/release_notes/tests/change_notes/full/
--rw-r--r--   0 runner    (1001) docker     (115)      330 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/release_notes/tests/change_notes/full/example1.md
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.098217 cumulusci-3.9.0/cumulusci/tasks/release_notes/tests/change_notes/multi/
--rw-r--r--   0 runner    (1001) docker     (115)        2 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/release_notes/tests/change_notes/multi/1.txt
--rw-r--r--   0 runner    (1001) docker     (115)        2 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/release_notes/tests/change_notes/multi/2.txt
--rw-r--r--   0 runner    (1001) docker     (115)        6 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/release_notes/tests/change_notes/multi/3.txt
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.098217 cumulusci-3.9.0/cumulusci/tasks/release_notes/tests/change_notes/single/
--rw-r--r--   0 runner    (1001) docker     (115)        2 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/release_notes/tests/change_notes/single/1.txt
--rw-r--r--   0 runner    (1001) docker     (115)    20823 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/release_notes/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (115)    21934 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/release_notes/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (115)    18788 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/release_notes/tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (115)    15036 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/release_notes/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (115)     4763 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/release_notes/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.098217 cumulusci-3.9.0/cumulusci/tasks/robotframework/
--rw-r--r--   0 runner    (1001) docker     (115)      311 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/robotframework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.098217 cumulusci-3.9.0/cumulusci/tasks/robotframework/debugger/
--rw-r--r--   0 runner    (1001) docker     (115)     3120 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/robotframework/debugger/DebugListener.py
--rw-r--r--   0 runner    (1001) docker     (115)      314 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/robotframework/debugger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     2764 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/robotframework/debugger/model.py
--rw-r--r--   0 runner    (1001) docker     (115)     7824 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/robotframework/debugger/ui.py
--rw-r--r--   0 runner    (1001) docker     (115)     6842 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/robotframework/libdoc.py
--rw-r--r--   0 runner    (1001) docker     (115)     7768 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/robotframework/lint.py
--rw-r--r--   0 runner    (1001) docker     (115)     5791 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/robotframework/robotframework.py
--rw-r--r--   0 runner    (1001) docker     (115)     2087 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/robotframework/stylesheet.css
--rw-r--r--   0 runner    (1001) docker     (115)     3254 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/robotframework/template.html
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.098217 cumulusci-3.9.0/cumulusci/tasks/robotframework/tests/
--rw-r--r--   0 runner    (1001) docker     (115)      669 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/robotframework/tests/TestLibrary.py
--rw-r--r--   0 runner    (1001) docker     (115)      647 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/robotframework/tests/TestPageObjects.py
--rw-r--r--   0 runner    (1001) docker     (115)      254 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/robotframework/tests/TestResource.robot
--rw-r--r--   0 runner    (1001) docker     (115)    17229 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/robotframework/tests/test_debugger.py
--rw-r--r--   0 runner    (1001) docker     (115)     8170 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/robotframework/tests/test_robot_lint.py
--rw-r--r--   0 runner    (1001) docker     (115)    15638 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/robotframework/tests/test_robotframework.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.106217 cumulusci-3.9.0/cumulusci/tasks/salesforce/
--rw-r--r--   0 runner    (1001) docker     (115)     3189 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/BaseRetrieveMetadata.py
--rw-r--r--   0 runner    (1001) docker     (115)     1164 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/BaseSalesforceApiTask.py
--rw-r--r--   0 runner    (1001) docker     (115)      425 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/BaseSalesforceMetadataApiTask.py
--rw-r--r--   0 runner    (1001) docker     (115)      975 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/BaseSalesforceTask.py
--rw-r--r--   0 runner    (1001) docker     (115)     1119 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/BaseUninstallMetadata.py
--rw-r--r--   0 runner    (1001) docker     (115)     3257 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/CreateCommunity.py
--rw-r--r--   0 runner    (1001) docker     (115)     1076 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/CreatePackage.py
--rw-r--r--   0 runner    (1001) docker     (115)    11188 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/Deploy.py
--rw-r--r--   0 runner    (1001) docker     (115)     2887 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/DeployBundles.py
--rw-r--r--   0 runner    (1001) docker     (115)     6630 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/EnsureRecordTypes.py
--rw-r--r--   0 runner    (1001) docker     (115)      284 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/GetInstalledPackages.py
--rw-r--r--   0 runner    (1001) docker     (115)     4400 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/InstallPackageVersion.py
--rw-r--r--   0 runner    (1001) docker     (115)     1513 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/ListCommunities.py
--rw-r--r--   0 runner    (1001) docker     (115)      608 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/ListCommunityTemplates.py
--rw-r--r--   0 runner    (1001) docker     (115)     2326 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/PublishCommunity.py
--rw-r--r--   0 runner    (1001) docker     (115)     1316 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/RetrievePackaged.py
--rw-r--r--   0 runner    (1001) docker     (115)     3335 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/RetrieveReportsAndDashboards.py
--rw-r--r--   0 runner    (1001) docker     (115)     1239 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/RetrieveUnpackaged.py
--rw-r--r--   0 runner    (1001) docker     (115)     1401 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/SOQLQuery.py
--rw-r--r--   0 runner    (1001) docker     (115)      492 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/UninstallLocal.py
--rw-r--r--   0 runner    (1001) docker     (115)      759 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/UninstallLocalBundles.py
--rw-r--r--   0 runner    (1001) docker     (115)     2220 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/UninstallLocalNamespacedBundles.py
--rw-r--r--   0 runner    (1001) docker     (115)     1240 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/UninstallPackage.py
--rw-r--r--   0 runner    (1001) docker     (115)     2176 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/UninstallPackaged.py
--rw-r--r--   0 runner    (1001) docker     (115)     5197 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/UninstallPackagedIncremental.py
--rw-r--r--   0 runner    (1001) docker     (115)    15763 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/UpdateDependencies.py
--rw-r--r--   0 runner    (1001) docker     (115)     3883 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     2406 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/activate_flow.py
--rw-r--r--   0 runner    (1001) docker     (115)     6352 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/custom_settings.py
--rw-r--r--   0 runner    (1001) docker     (115)     1356 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/insert_record.py
--rw-r--r--   0 runner    (1001) docker     (115)     2829 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/org_settings.py
--rw-r--r--   0 runner    (1001) docker     (115)     8664 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/package_upload.py
--rw-r--r--   0 runner    (1001) docker     (115)    15555 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/sourcetracking.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.110217 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/
--rw-r--r--   0 runner    (1001) docker     (115)       30 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     9156 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_CreateCommunity.py
--rw-r--r--   0 runner    (1001) docker     (115)      755 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_CreatePackage.py
--rw-r--r--   0 runner    (1001) docker     (115)    18835 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_Deploy.py
--rw-r--r--   0 runner    (1001) docker     (115)     2754 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_DeployBundles.py
--rw-r--r--   0 runner    (1001) docker     (115)     9801 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_EnsureRecordTypes.py
--rw-r--r--   0 runner    (1001) docker     (115)     1658 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_InstallPackageVersion.py
--rw-r--r--   0 runner    (1001) docker     (115)     3757 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_ListCommunities.py
--rw-r--r--   0 runner    (1001) docker     (115)     1912 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_ListCommunityTemplates.py
--rw-r--r--   0 runner    (1001) docker     (115)    11830 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_PackageUpload.py
--rw-r--r--   0 runner    (1001) docker     (115)    13591 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_ProfileGrantAllAccess.py
--rw-r--r--   0 runner    (1001) docker     (115)     7128 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_PublishCommunity.py
--rw-r--r--   0 runner    (1001) docker     (115)      874 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_RetrievePackaged.py
--rw-r--r--   0 runner    (1001) docker     (115)     1762 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_RetrieveReportsAndDashboards.py
--rw-r--r--   0 runner    (1001) docker     (115)      711 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_RetrieveUnpackaged.py
--rw-r--r--   0 runner    (1001) docker     (115)      989 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_SOQLQuery.py
--rw-r--r--   0 runner    (1001) docker     (115)      625 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_UninstallLocal.py
--rw-r--r--   0 runner    (1001) docker     (115)      591 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_UninstallLocalBundles.py
--rw-r--r--   0 runner    (1001) docker     (115)      950 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_UninstallLocalNamespacedBundles.py
--rw-r--r--   0 runner    (1001) docker     (115)      714 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_UninstallPackage.py
--rw-r--r--   0 runner    (1001) docker     (115)     1265 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_UninstallPackaged.py
--rw-r--r--   0 runner    (1001) docker     (115)     2874 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_UninstallPackagedIncremental.py
--rw-r--r--   0 runner    (1001) docker     (115)    12395 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_UpdateDependencies.py
--rw-r--r--   0 runner    (1001) docker     (115)     3971 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_activate_flow.py
--rw-r--r--   0 runner    (1001) docker     (115)     3760 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_base_tasks.py
--rw-r--r--   0 runner    (1001) docker     (115)     8539 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_custom_settings.py
--rw-r--r--   0 runner    (1001) docker     (115)     2994 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_insert_record.py
--rw-r--r--   0 runner    (1001) docker     (115)     2563 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_org_settings.py
--rw-r--r--   0 runner    (1001) docker     (115)     9312 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_sourcetracking.py
--rw-r--r--   0 runner    (1001) docker     (115)    10361 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_trigger_handlers.py
--rw-r--r--   0 runner    (1001) docker     (115)     1018 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (115)     3953 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/trigger_handlers.py
--rw-r--r--   0 runner    (1001) docker     (115)    10931 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/salesforce/update_profile.py
--rw-r--r--   0 runner    (1001) docker     (115)     3171 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/sfdx.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.114217 cumulusci-3.9.0/cumulusci/tasks/tests/
--rw-r--r--   0 runner    (1001) docker     (115)       24 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     4851 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (115)    11555 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/tests/test_connectedapp.py
--rw-r--r--   0 runner    (1001) docker     (115)    21288 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/tests/test_datadictionary.py
--rw-r--r--   0 runner    (1001) docker     (115)    13592 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/tests/test_metadeploy.py
--rw-r--r--   0 runner    (1001) docker     (115)     3399 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/tests/test_metaxml.py
--rw-r--r--   0 runner    (1001) docker     (115)     3236 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/tests/test_pushfails.py
--rw-r--r--   0 runner    (1001) docker     (115)     2781 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/tests/test_salesforce.py
--rw-r--r--   0 runner    (1001) docker     (115)     3725 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/tests/test_sfdx.py
--rw-r--r--   0 runner    (1001) docker     (115)     5701 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (115)     7576 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tasks/util.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.114217 cumulusci-3.9.0/cumulusci/tests/
--rw-r--r--   0 runner    (1001) docker     (115)       24 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)      185 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (115)    20150 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (115)     2003 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/tests/util.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.114217 cumulusci-3.9.0/cumulusci/utils/
--rw-r--r--   0 runner    (1001) docker     (115)    22155 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     2769 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/utils/fileutils.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.114217 cumulusci-3.9.0/cumulusci/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (115)     1861 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/utils/tests/test_fileutils.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.114217 cumulusci-3.9.0/cumulusci/utils/xml/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/utils/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)    10125 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/utils/xml/metadata_tree.py
--rw-r--r--   0 runner    (1001) docker     (115)     1697 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/utils/xml/salesforce_encoding.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.114217 cumulusci-3.9.0/cumulusci/utils/xml/test/
--rw-r--r--   0 runner    (1001) docker     (115)     6685 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/utils/xml/test/test_metadata_tree.py
--rw-r--r--   0 runner    (1001) docker     (115)     2638 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/utils/xml/test/test_salesforce_encoding.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.114217 cumulusci-3.9.0/cumulusci/utils/yaml/
--rw-r--r--   0 runner    (1001) docker     (115)     1038 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/utils/yaml/cumulusci_yml.py
--rw-r--r--   0 runner    (1001) docker     (115)     4711 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/utils/yaml/model_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.114217 cumulusci-3.9.0/cumulusci/utils/yaml/tests/
--rw-r--r--   0 runner    (1001) docker     (115)     1081 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/utils/yaml/tests/test_cumulusci_yml.py
--rw-r--r--   0 runner    (1001) docker     (115)     4932 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/utils/yaml/tests/test_model_parser.py
--rw-r--r--   0 runner    (1001) docker     (115)        5 2020-03-16 21:13:58.000000 cumulusci-3.9.0/cumulusci/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.054218 cumulusci-3.9.0/cumulusci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (115)   142154 2020-03-16 21:14:08.000000 cumulusci-3.9.0/cumulusci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)    16400 2020-03-16 21:14:08.000000 cumulusci-3.9.0/cumulusci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2020-03-16 21:14:08.000000 cumulusci-3.9.0/cumulusci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (115)       48 2020-03-16 21:14:08.000000 cumulusci-3.9.0/cumulusci.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2020-03-16 21:14:08.000000 cumulusci-3.9.0/cumulusci.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (115)      706 2020-03-16 21:14:08.000000 cumulusci-3.9.0/cumulusci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (115)       10 2020-03-16 21:14:08.000000 cumulusci-3.9.0/cumulusci.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.122217 cumulusci-3.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (115)     6774 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (115)      150 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/api_reference.rst
--rw-r--r--   0 runner    (1001) docker     (115)       28 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (115)    14626 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/bulk_data.rst
--rwxr-xr-x   0 runner    (1001) docker     (115)     9290 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (115)       33 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (115)    19775 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/cookbook.rst
--rw-r--r--   0 runner    (1001) docker     (115)   183748 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/cumulus_ci_workflow.png
--rw-r--r--   0 runner    (1001) docker     (115)    12754 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/cumulusci_flow.rst
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.050218 cumulusci-3.9.0/docs/diagram/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.122217 cumulusci-3.9.0/docs/diagram/img/
--rw-r--r--   0 runner    (1001) docker     (115)     4409 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/diagram/img/image1.png
--rw-r--r--   0 runner    (1001) docker     (115)   108243 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/diagram/img/image12.png
--rw-r--r--   0 runner    (1001) docker     (115)    26963 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/diagram/img/image15.png
--rw-r--r--   0 runner    (1001) docker     (115)    68821 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/diagram/img/image17.png
--rw-r--r--   0 runner    (1001) docker     (115)    78349 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/diagram/img/image3.png
--rw-r--r--   0 runner    (1001) docker     (115)    38018 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/features.rst
--rw-r--r--   0 runner    (1001) docker     (115)    53215 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/github-commit_status_error.png
--rw-r--r--   0 runner    (1001) docker     (115)    51940 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/github-commit_status_pass.png
--rw-r--r--   0 runner    (1001) docker     (115)    51527 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/github-creating_a_uat_release.png
--rw-r--r--   0 runner    (1001) docker     (115)       28 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/history.rst
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-16 21:14:09.126217 cumulusci-3.9.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (115)     7203 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/images/env-var.png
--rw-r--r--   0 runner    (1001) docker     (115)    67314 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/images/locate_elements_screenshot.png
--rw-r--r--   0 runner    (1001) docker     (115)    15048 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/images/pipx.png
--rw-r--r--   0 runner    (1001) docker     (115)   251244 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/images/salesforce-org-process.png
--rw-r--r--   0 runner    (1001) docker     (115)   417827 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/images/windows_python.png
--rw-r--r--   0 runner    (1001) docker     (115)      702 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (115)     3944 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (115)     6465 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (115)     9244 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/robotframework-debugger.rst
--rw-r--r--   0 runner    (1001) docker     (115)    15403 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/robotframework-tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (115)    33005 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/robotframework.rst
--rw-r--r--   0 runner    (1001) docker     (115)    91997 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/tasks.rst
--rw-r--r--   0 runner    (1001) docker     (115)    37639 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (115)     1608 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (115)    12793 2020-03-16 21:13:58.000000 cumulusci-3.9.0/docs/why_cumulusci.rst
--rw-r--r--   0 runner    (1001) docker     (115)      709 2020-03-16 21:13:58.000000 cumulusci-3.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (115)      230 2020-03-16 21:13:58.000000 cumulusci-3.9.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (115)      122 2020-03-16 21:14:09.130217 cumulusci-3.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (115)     2154 2020-03-16 21:13:58.000000 cumulusci-3.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:53.002115 cumulusci-3.9.1/
+-rw-r--r--   0 runner    (1001) docker     (115)      567 2020-03-25 20:17:40.000000 cumulusci-3.9.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (115)     4438 2020-03-25 20:17:40.000000 cumulusci-3.9.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (115)   121237 2020-03-25 20:17:40.000000 cumulusci-3.9.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (115)     1598 2020-03-25 20:17:40.000000 cumulusci-3.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (115)      452 2020-03-25 20:17:40.000000 cumulusci-3.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (115)   143072 2020-03-25 20:17:53.006115 cumulusci-3.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)     1895 2020-03-25 20:17:40.000000 cumulusci-3.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.946115 cumulusci-3.9.1/cumulusci/
+-rw-r--r--   0 runner    (1001) docker     (115)      342 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)       43 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.950115 cumulusci-3.9.1/cumulusci/cli/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)    50079 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/cli/cci.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1760 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/cli/logger.py
+-rw-r--r--   0 runner    (1001) docker     (115)     6100 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/cli/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.950115 cumulusci-3.9.1/cumulusci/cli/tests/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/cli/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)    57805 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/cli/tests/test_cci.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1358 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/cli/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (115)     7296 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/cli/tests/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (115)    11771 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/cli/tests/test_ui.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4904 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/cli/ui.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1079 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.950115 cumulusci-3.9.1/cumulusci/core/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.950115 cumulusci-3.9.1/cumulusci/core/config/
+-rw-r--r--   0 runner    (1001) docker     (115)     1298 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/config/BaseConfig.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2039 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/config/BaseGlobalConfig.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2115 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/config/BaseTaskFlowConfig.py
+-rw-r--r--   0 runner    (1001) docker     (115)     6072 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/config/OrgConfig.py
+-rw-r--r--   0 runner    (1001) docker     (115)    11868 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/config/ScratchOrgConfig.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1239 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)    29735 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/config/project_config.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5514 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (115)    26480 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/flowrunner.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5827 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/github.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.954115 cumulusci-3.9.1/cumulusci/core/keychain/
+-rw-r--r--   0 runner    (1001) docker     (115)     3690 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/keychain/BaseEncryptedProjectKeychain.py
+-rw-r--r--   0 runner    (1001) docker     (115)     9101 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/keychain/BaseProjectKeychain.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4202 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/keychain/EncryptedFileProjectKeychain.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1847 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/keychain/EnvironmentProjectKeychain.py
+-rw-r--r--   0 runner    (1001) docker     (115)      591 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/keychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3051 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1868 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/sfdx.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.954115 cumulusci-3.9.1/cumulusci/core/source/
+-rw-r--r--   0 runner    (1001) docker     (115)      239 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4586 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/source/github.py
+-rw-r--r--   0 runner    (1001) docker     (115)      785 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/source/local_folder.py
+-rw-r--r--   0 runner    (1001) docker     (115)     8430 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1455 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/template_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.954115 cumulusci-3.9.1/cumulusci/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (115)      479 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/tests/BarTestPage.py
+-rw-r--r--   0 runner    (1001) docker     (115)      324 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/tests/FooTestPage.py
+-rw-r--r--   0 runner    (1001) docker     (115)       56 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)    43877 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (115)    25741 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/tests/test_config_expensive.py
+-rw-r--r--   0 runner    (1001) docker     (115)      558 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (115)    19750 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/tests/test_flowrunner.py
+-rw-r--r--   0 runner    (1001) docker     (115)     9611 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (115)    19646 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/tests/test_keychain.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4646 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/tests/test_pageobjects.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3483 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/tests/test_salesforce.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2826 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/tests/test_salesforce_locators.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1136 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/tests/test_sfdx.py
+-rw-r--r--   0 runner    (1001) docker     (115)    16216 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/tests/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (115)     7180 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3759 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3036 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5715 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (115)    37971 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/cumulusci.yml
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.954115 cumulusci-3.9.1/cumulusci/files/
+-rw-r--r--   0 runner    (1001) docker     (115)      457 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/files/admin_profile.xml
+-rw-r--r--   0 runner    (1001) docker     (115)     9909 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/files/metadata_whitelist.txt
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.942115 cumulusci-3.9.1/cumulusci/files/templates/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.958115 cumulusci-3.9.1/cumulusci/files/templates/project/
+-rw-r--r--   0 runner    (1001) docker     (115)      343 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/files/templates/project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (115)      424 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/files/templates/project/README.md
+-rw-r--r--   0 runner    (1001) docker     (115)     1699 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/files/templates/project/cumulusci.yml
+-rw-r--r--   0 runner    (1001) docker     (115)     1126 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/files/templates/project/mapping.yml
+-rw-r--r--   0 runner    (1001) docker     (115)      567 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/files/templates/project/scratch_def.json
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.958115 cumulusci-3.9.1/cumulusci/oauth/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/oauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)      116 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/oauth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (115)     6847 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/oauth/salesforce.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.958115 cumulusci-3.9.1/cumulusci/oauth/tests/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/oauth/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     6150 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/oauth/tests/test_salesforce.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.958115 cumulusci-3.9.1/cumulusci/robotframework/
+-rw-r--r--   0 runner    (1001) docker     (115)     9370 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/CumulusCI.py
+-rw-r--r--   0 runner    (1001) docker     (115)      123 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/CumulusCI.robot
+-rw-r--r--   0 runner    (1001) docker     (115)    42214 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/Salesforce.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4870 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/Salesforce.robot
+-rw-r--r--   0 runner    (1001) docker     (115)      111 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5142 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/locator_manager.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3957 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/locators_45.py
+-rw-r--r--   0 runner    (1001) docker     (115)      717 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/locators_46.py
+-rw-r--r--   0 runner    (1001) docker     (115)      486 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/locators_47.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1714 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/locators_48.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.958115 cumulusci-3.9.1/cumulusci/robotframework/pageobjects/
+-rw-r--r--   0 runner    (1001) docker     (115)     9938 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/pageobjects/BasePageObjects.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1418 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/pageobjects/PageObjectLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (115)    13060 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/pageobjects/PageObjects.py
+-rw-r--r--   0 runner    (1001) docker     (115)      336 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/pageobjects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4011 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/pageobjects/baseobjects.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.942115 cumulusci-3.9.1/cumulusci/robotframework/perftests/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.958115 cumulusci-3.9.1/cumulusci/robotframework/perftests/short/
+-rw-r--r--   0 runner    (1001) docker     (115)     4066 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/perftests/short/collection_perf.robot
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.958115 cumulusci-3.9.1/cumulusci/robotframework/tests/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.962115 cumulusci-3.9.1/cumulusci/robotframework/tests/cumulusci/
+-rw-r--r--   0 runner    (1001) docker     (115)      995 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/tests/cumulusci/base.robot
+-rw-r--r--   0 runner    (1001) docker     (115)     1160 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/tests/cumulusci/bulkdata.robot
+-rw-r--r--   0 runner    (1001) docker     (115)     2301 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/tests/cumulusci/communities.robot
+-rw-r--r--   0 runner    (1001) docker     (115)     3306 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/tests/cumulusci/datagen.robot
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.962115 cumulusci-3.9.1/cumulusci/robotframework/tests/salesforce/
+-rw-r--r--   0 runner    (1001) docker     (115)      539 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/tests/salesforce/TestLibraryA.py
+-rw-r--r--   0 runner    (1001) docker     (115)      487 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/tests/salesforce/TestLibraryB.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3499 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/tests/salesforce/TestListener.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4920 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/tests/salesforce/api.robot
+-rw-r--r--   0 runner    (1001) docker     (115)     4199 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/tests/salesforce/browsers.robot
+-rw-r--r--   0 runner    (1001) docker     (115)     1821 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/tests/salesforce/create_contact.robot
+-rw-r--r--   0 runner    (1001) docker     (115)     1900 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/tests/salesforce/locators.robot
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.962115 cumulusci-3.9.1/cumulusci/robotframework/tests/salesforce/pageobjects/
+-rw-r--r--   0 runner    (1001) docker     (115)     3635 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/tests/salesforce/pageobjects/base_pageobjects.robot
+-rw-r--r--   0 runner    (1001) docker     (115)      761 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/tests/salesforce/pageobjects/example_page_object.py
+-rw-r--r--   0 runner    (1001) docker     (115)     6149 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/tests/salesforce/pageobjects/pageobjects.robot
+-rw-r--r--   0 runner    (1001) docker     (115)     3621 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/tests/salesforce/populate.robot
+-rw-r--r--   0 runner    (1001) docker     (115)     1423 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/tests/salesforce/test_testlistener.py
+-rw-r--r--   0 runner    (1001) docker     (115)     7955 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/tests/salesforce/ui.robot
+-rw-r--r--   0 runner    (1001) docker     (115)     5254 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/tests/test_locator_manager.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1872 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/tests/test_template_util.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1055 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (115)     7675 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/robotframework/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.962115 cumulusci-3.9.1/cumulusci/salesforce_api/
+-rw-r--r--   0 runner    (1001) docker     (115)       56 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/salesforce_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)      525 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/salesforce_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (115)    24343 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/salesforce_api/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4473 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/salesforce_api/package_zip.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5769 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/salesforce_api/soap_envelopes.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.962115 cumulusci-3.9.1/cumulusci/salesforce_api/tests/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/salesforce_api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4748 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/salesforce_api/tests/metadata_test_strings.py
+-rw-r--r--   0 runner    (1001) docker     (115)    37472 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/salesforce_api/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2517 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/salesforce_api/tests/test_package_zip.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3184 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/salesforce_api/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1151 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/salesforce_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.966115 cumulusci-3.9.1/cumulusci/tasks/
+-rw-r--r--   0 runner    (1001) docker     (115)       56 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.966115 cumulusci-3.9.1/cumulusci/tasks/apex/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/apex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5289 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/apex/anon.py
+-rw-r--r--   0 runner    (1001) docker     (115)     6739 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/apex/batch.py
+-rw-r--r--   0 runner    (1001) docker     (115)    23999 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/apex/testrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.966115 cumulusci-3.9.1/cumulusci/tasks/apex/tests/
+-rw-r--r--   0 runner    (1001) docker     (115)    40133 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/apex/tests/test_apex_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.966115 cumulusci-3.9.1/cumulusci/tasks/bulkdata/
+-rw-r--r--   0 runner    (1001) docker     (115)      485 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3329 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/base_generate_data_task.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4364 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/delete.py
+-rw-r--r--   0 runner    (1001) docker     (115)    11631 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/extract.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4021 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/factory_utils.py
+-rw-r--r--   0 runner    (1001) docker     (115)      107 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/generate.py
+-rw-r--r--   0 runner    (1001) docker     (115)     8286 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/generate_and_load_data.py
+-rw-r--r--   0 runner    (1001) docker     (115)      706 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/generate_and_load_data_from_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (115)     7068 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/generate_from_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (115)    15262 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/generate_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (115)    18730 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/load.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1876 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/mapping_parser.py
+-rw-r--r--   0 runner    (1001) docker     (115)    11200 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/step.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.970115 cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1333 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/dummy_data_factory.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1723 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/mapping-oid.yml
+-rw-r--r--   0 runner    (1001) docker     (115)      685 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/mapping_after.yml
+-rw-r--r--   0 runner    (1001) docker     (115)      547 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/mapping_v1.yml
+-rw-r--r--   0 runner    (1001) docker     (115)      421 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/mapping_v2.yml
+-rw-r--r--   0 runner    (1001) docker     (115)     1561 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/mapping_vanilla_sf.yml
+-rw-r--r--   0 runner    (1001) docker     (115)      353 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/mock_data_factory_without_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (115)      143 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/recordtypes.yml
+-rw-r--r--   0 runner    (1001) docker     (115)       83 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/simple_snowfakery.yml
+-rw-r--r--   0 runner    (1001) docker     (115)     2173 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/test_base_generate_data_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (115)    12123 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (115)    21612 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1514 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/test_factory_utils.py
+-rw-r--r--   0 runner    (1001) docker     (115)     8045 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/test_generate_and_load.py
+-rw-r--r--   0 runner    (1001) docker     (115)    21868 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/test_generatemapping.py
+-rw-r--r--   0 runner    (1001) docker     (115)    35067 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1976 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/test_mapping_parser.py
+-rw-r--r--   0 runner    (1001) docker     (115)    18552 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/test_step.py
+-rw-r--r--   0 runner    (1001) docker     (115)     6389 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.970115 cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/tests/
+-rw-r--r--   0 runner    (1001) docker     (115)     9348 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/tests/test_generate_from_snowfakery_task.py
+-rw-r--r--   0 runner    (1001) docker     (115)      670 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (115)     6157 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/bulkdata/utils.py
+-rw-r--r--   0 runner    (1001) docker     (115)     6801 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/command.py
+-rw-r--r--   0 runner    (1001) docker     (115)     7025 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/connectedapp.py
+-rw-r--r--   0 runner    (1001) docker     (115)    11541 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/datadictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.970115 cumulusci-3.9.1/cumulusci/tasks/github/
+-rw-r--r--   0 runner    (1001) docker     (115)      373 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)      574 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/github/base.py
+-rw-r--r--   0 runner    (1001) docker     (115)     8662 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/github/merge.py
+-rw-r--r--   0 runner    (1001) docker     (115)      269 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/github/pull_request.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3462 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/github/release.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4106 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/github/release_report.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1505 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/github/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.970115 cumulusci-3.9.1/cumulusci/tasks/github/tests/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/github/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)    17647 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/github/tests/test_merge.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1022 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/github/tests/test_pull_request.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5029 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/github/tests/test_release.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3589 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/github/tests/test_release_report.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3206 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/github/tests/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5777 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/github/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (115)    21440 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/github/tests/util_github_api.py
+-rw-r--r--   0 runner    (1001) docker     (115)     9030 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/github/util.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.974115 cumulusci-3.9.1/cumulusci/tasks/metadata/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3191 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/metadata/ee_src.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3312 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/metadata/managed_src.py
+-rw-r--r--   0 runner    (1001) docker     (115)    16147 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/metadata/metadata_map.yml
+-rw-r--r--   0 runner    (1001) docker     (115)     4147 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/metadata/modify.py
+-rw-r--r--   0 runner    (1001) docker     (115)    12998 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/metadata/package.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.974115 cumulusci-3.9.1/cumulusci/tasks/metadata/tests/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/metadata/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.942115 cumulusci-3.9.1/cumulusci/tasks/metadata/tests/package_metadata/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.974115 cumulusci-3.9.1/cumulusci/tasks/metadata/tests/package_metadata/namespaced_report_folder/
+-rw-r--r--   0 runner    (1001) docker     (115)      287 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/metadata/tests/package_metadata/namespaced_report_folder/destructiveChanges.xml
+-rw-r--r--   0 runner    (1001) docker     (115)      286 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/metadata/tests/package_metadata/namespaced_report_folder/package.xml
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.942115 cumulusci-3.9.1/cumulusci/tasks/metadata/tests/package_metadata/namespaced_report_folder/reports/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.974115 cumulusci-3.9.1/cumulusci/tasks/metadata/tests/package_metadata/namespaced_report_folder/reports/namespace__TestFolder/
+-rw-r--r--   0 runner    (1001) docker     (115)      106 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/metadata/tests/package_metadata/namespaced_report_folder/reports/namespace__TestFolder/TestReport.report
+-rw-r--r--   0 runner    (1001) docker     (115)      287 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/metadata/tests/sample_package.xml
+-rw-r--r--   0 runner    (1001) docker     (115)     3366 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/metadata/tests/test_ee_src.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3280 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/metadata/tests/test_managed_src.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4842 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/metadata/tests/test_modify.py
+-rw-r--r--   0 runner    (1001) docker     (115)    12611 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/metadata/tests/test_package.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.974115 cumulusci-3.9.1/cumulusci/tasks/metadata_etl/
+-rw-r--r--   0 runner    (1001) docker     (115)      749 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/metadata_etl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)    10954 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/metadata_etl/base.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2321 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/metadata_etl/layouts.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4361 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/metadata_etl/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5695 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/metadata_etl/sharing.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.978115 cumulusci-3.9.1/cumulusci/tasks/metadata_etl/tests/
+-rw-r--r--   0 runner    (1001) docker     (115)    12670 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/metadata_etl/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5796 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/metadata_etl/tests/test_layouts.py
+-rw-r--r--   0 runner    (1001) docker     (115)     7059 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/metadata_etl/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (115)    10891 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/metadata_etl/tests/test_sharing.py
+-rw-r--r--   0 runner    (1001) docker     (115)     8728 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/metadata_etl/tests/test_value_sets.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2922 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/metadata_etl/value_sets.py
+-rw-r--r--   0 runner    (1001) docker     (115)     9440 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/metadeploy.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3426 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/metaxml.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.978115 cumulusci-3.9.1/cumulusci/tasks/push/
+-rw-r--r--   0 runner    (1001) docker     (115)     3759 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/push/README.md
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/push/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)    25003 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/push/push_api.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5447 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/push/pushfails.py
+-rw-r--r--   0 runner    (1001) docker     (115)    15651 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/push/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.978115 cumulusci-3.9.1/cumulusci/tasks/push/tests/
+-rw-r--r--   0 runner    (1001) docker     (115)     4888 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/push/tests/test_push_api.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.978115 cumulusci-3.9.1/cumulusci/tasks/release_notes/
+-rw-r--r--   0 runner    (1001) docker     (115)     2132 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/release_notes/README.md
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/release_notes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)      179 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/release_notes/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (115)    10962 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/release_notes/generator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     9581 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/release_notes/parser.py
+-rw-r--r--   0 runner    (1001) docker     (115)     6885 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/release_notes/provider.py
+-rw-r--r--   0 runner    (1001) docker     (115)     8831 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/release_notes/task.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.978115 cumulusci-3.9.1/cumulusci/tasks/release_notes/tests/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/release_notes/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.942115 cumulusci-3.9.1/cumulusci/tasks/release_notes/tests/change_notes/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.978115 cumulusci-3.9.1/cumulusci/tasks/release_notes/tests/change_notes/full/
+-rw-r--r--   0 runner    (1001) docker     (115)      330 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/release_notes/tests/change_notes/full/example1.md
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.978115 cumulusci-3.9.1/cumulusci/tasks/release_notes/tests/change_notes/multi/
+-rw-r--r--   0 runner    (1001) docker     (115)        2 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/release_notes/tests/change_notes/multi/1.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        2 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/release_notes/tests/change_notes/multi/2.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        6 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/release_notes/tests/change_notes/multi/3.txt
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.978115 cumulusci-3.9.1/cumulusci/tasks/release_notes/tests/change_notes/single/
+-rw-r--r--   0 runner    (1001) docker     (115)        2 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/release_notes/tests/change_notes/single/1.txt
+-rw-r--r--   0 runner    (1001) docker     (115)    20823 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/release_notes/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (115)    21934 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/release_notes/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (115)    18788 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/release_notes/tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (115)    15036 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/release_notes/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4763 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/release_notes/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.982115 cumulusci-3.9.1/cumulusci/tasks/robotframework/
+-rw-r--r--   0 runner    (1001) docker     (115)      311 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/robotframework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.982115 cumulusci-3.9.1/cumulusci/tasks/robotframework/debugger/
+-rw-r--r--   0 runner    (1001) docker     (115)     3120 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/robotframework/debugger/DebugListener.py
+-rw-r--r--   0 runner    (1001) docker     (115)      314 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/robotframework/debugger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2764 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/robotframework/debugger/model.py
+-rw-r--r--   0 runner    (1001) docker     (115)     7824 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/robotframework/debugger/ui.py
+-rw-r--r--   0 runner    (1001) docker     (115)     6842 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/robotframework/libdoc.py
+-rw-r--r--   0 runner    (1001) docker     (115)     7768 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/robotframework/lint.py
+-rw-r--r--   0 runner    (1001) docker     (115)     6535 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/robotframework/robotframework.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2087 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/robotframework/stylesheet.css
+-rw-r--r--   0 runner    (1001) docker     (115)     3254 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/robotframework/template.html
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.982115 cumulusci-3.9.1/cumulusci/tasks/robotframework/tests/
+-rw-r--r--   0 runner    (1001) docker     (115)      669 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/robotframework/tests/TestLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (115)      647 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/robotframework/tests/TestPageObjects.py
+-rw-r--r--   0 runner    (1001) docker     (115)      254 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/robotframework/tests/TestResource.robot
+-rw-r--r--   0 runner    (1001) docker     (115)    17229 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/robotframework/tests/test_debugger.py
+-rw-r--r--   0 runner    (1001) docker     (115)     8170 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/robotframework/tests/test_robot_lint.py
+-rw-r--r--   0 runner    (1001) docker     (115)    16559 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/robotframework/tests/test_robotframework.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.986115 cumulusci-3.9.1/cumulusci/tasks/salesforce/
+-rw-r--r--   0 runner    (1001) docker     (115)     3189 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/BaseRetrieveMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1164 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/BaseSalesforceApiTask.py
+-rw-r--r--   0 runner    (1001) docker     (115)      425 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/BaseSalesforceMetadataApiTask.py
+-rw-r--r--   0 runner    (1001) docker     (115)      128 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/BaseSalesforceTask.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1119 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/BaseUninstallMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3257 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/CreateCommunity.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1076 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/CreatePackage.py
+-rw-r--r--   0 runner    (1001) docker     (115)    11188 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/Deploy.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2887 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/DeployBundles.py
+-rw-r--r--   0 runner    (1001) docker     (115)     6630 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/EnsureRecordTypes.py
+-rw-r--r--   0 runner    (1001) docker     (115)      284 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/GetInstalledPackages.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4400 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/InstallPackageVersion.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1513 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/ListCommunities.py
+-rw-r--r--   0 runner    (1001) docker     (115)      608 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/ListCommunityTemplates.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2326 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/PublishCommunity.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1316 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/RetrievePackaged.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3335 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/RetrieveReportsAndDashboards.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1239 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/RetrieveUnpackaged.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1401 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/SOQLQuery.py
+-rw-r--r--   0 runner    (1001) docker     (115)      492 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/UninstallLocal.py
+-rw-r--r--   0 runner    (1001) docker     (115)      759 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/UninstallLocalBundles.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2220 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/UninstallLocalNamespacedBundles.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1240 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/UninstallPackage.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2176 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/UninstallPackaged.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5197 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/UninstallPackagedIncremental.py
+-rw-r--r--   0 runner    (1001) docker     (115)    15763 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/UpdateDependencies.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3883 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2408 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/activate_flow.py
+-rw-r--r--   0 runner    (1001) docker     (115)     6352 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/custom_settings.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1356 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/insert_record.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2829 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/org_settings.py
+-rw-r--r--   0 runner    (1001) docker     (115)     8664 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/package_upload.py
+-rw-r--r--   0 runner    (1001) docker     (115)    15555 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/sourcetracking.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.990115 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/
+-rw-r--r--   0 runner    (1001) docker     (115)       30 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     9156 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_CreateCommunity.py
+-rw-r--r--   0 runner    (1001) docker     (115)      755 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_CreatePackage.py
+-rw-r--r--   0 runner    (1001) docker     (115)    18835 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_Deploy.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2754 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_DeployBundles.py
+-rw-r--r--   0 runner    (1001) docker     (115)     9801 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_EnsureRecordTypes.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1658 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_InstallPackageVersion.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3757 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_ListCommunities.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1912 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_ListCommunityTemplates.py
+-rw-r--r--   0 runner    (1001) docker     (115)    11830 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_PackageUpload.py
+-rw-r--r--   0 runner    (1001) docker     (115)    14164 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_ProfileGrantAllAccess.py
+-rw-r--r--   0 runner    (1001) docker     (115)     7128 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_PublishCommunity.py
+-rw-r--r--   0 runner    (1001) docker     (115)      874 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_RetrievePackaged.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1762 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_RetrieveReportsAndDashboards.py
+-rw-r--r--   0 runner    (1001) docker     (115)      711 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_RetrieveUnpackaged.py
+-rw-r--r--   0 runner    (1001) docker     (115)      989 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_SOQLQuery.py
+-rw-r--r--   0 runner    (1001) docker     (115)      625 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_UninstallLocal.py
+-rw-r--r--   0 runner    (1001) docker     (115)      591 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_UninstallLocalBundles.py
+-rw-r--r--   0 runner    (1001) docker     (115)      950 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_UninstallLocalNamespacedBundles.py
+-rw-r--r--   0 runner    (1001) docker     (115)      714 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_UninstallPackage.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1265 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_UninstallPackaged.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2874 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_UninstallPackagedIncremental.py
+-rw-r--r--   0 runner    (1001) docker     (115)    12395 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_UpdateDependencies.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3971 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_activate_flow.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3760 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_base_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (115)     8539 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_custom_settings.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2994 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_insert_record.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2563 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_org_settings.py
+-rw-r--r--   0 runner    (1001) docker     (115)     9312 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_sourcetracking.py
+-rw-r--r--   0 runner    (1001) docker     (115)    10361 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_trigger_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1018 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3953 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/trigger_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (115)    11581 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/salesforce/update_profile.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3171 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/sfdx.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.994115 cumulusci-3.9.1/cumulusci/tasks/tests/
+-rw-r--r--   0 runner    (1001) docker     (115)       24 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4851 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (115)    11555 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/tests/test_connectedapp.py
+-rw-r--r--   0 runner    (1001) docker     (115)    21288 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/tests/test_datadictionary.py
+-rw-r--r--   0 runner    (1001) docker     (115)    13592 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/tests/test_metadeploy.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3399 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/tests/test_metaxml.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3236 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/tests/test_pushfails.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2781 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/tests/test_salesforce.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3725 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/tests/test_sfdx.py
+-rw-r--r--   0 runner    (1001) docker     (115)     5701 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (115)     7576 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tasks/util.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.994115 cumulusci-3.9.1/cumulusci/tests/
+-rw-r--r--   0 runner    (1001) docker     (115)       24 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)      185 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (115)    20150 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1870 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.994115 cumulusci-3.9.1/cumulusci/utils/
+-rw-r--r--   0 runner    (1001) docker     (115)    22155 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2770 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/utils/fileutils.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.994115 cumulusci-3.9.1/cumulusci/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (115)     2148 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/utils/tests/test_fileutils.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.994115 cumulusci-3.9.1/cumulusci/utils/xml/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/utils/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)    10125 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/utils/xml/metadata_tree.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1697 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/utils/xml/salesforce_encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.994115 cumulusci-3.9.1/cumulusci/utils/xml/test/
+-rw-r--r--   0 runner    (1001) docker     (115)     6685 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/utils/xml/test/test_metadata_tree.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2638 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/utils/xml/test/test_salesforce_encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.994115 cumulusci-3.9.1/cumulusci/utils/yaml/
+-rw-r--r--   0 runner    (1001) docker     (115)     1041 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/utils/yaml/cumulusci_yml.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4711 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/utils/yaml/model_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.994115 cumulusci-3.9.1/cumulusci/utils/yaml/tests/
+-rw-r--r--   0 runner    (1001) docker     (115)     1081 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/utils/yaml/tests/test_cumulusci_yml.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4932 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/utils/yaml/tests/test_model_parser.py
+-rw-r--r--   0 runner    (1001) docker     (115)        5 2020-03-25 20:17:40.000000 cumulusci-3.9.1/cumulusci/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.950115 cumulusci-3.9.1/cumulusci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (115)   143072 2020-03-25 20:17:52.000000 cumulusci-3.9.1/cumulusci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)    16400 2020-03-25 20:17:52.000000 cumulusci-3.9.1/cumulusci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        1 2020-03-25 20:17:52.000000 cumulusci-3.9.1/cumulusci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       48 2020-03-25 20:17:52.000000 cumulusci-3.9.1/cumulusci.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        1 2020-03-25 20:17:52.000000 cumulusci-3.9.1/cumulusci.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (115)      724 2020-03-25 20:17:52.000000 cumulusci-3.9.1/cumulusci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       10 2020-03-25 20:17:52.000000 cumulusci-3.9.1/cumulusci.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.998115 cumulusci-3.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (115)     6774 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (115)      150 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/api_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (115)       28 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (115)    14626 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/bulk_data.rst
+-rwxr-xr-x   0 runner    (1001) docker     (115)     9290 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (115)       33 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (115)    19775 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/cookbook.rst
+-rw-r--r--   0 runner    (1001) docker     (115)   183748 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/cumulus_ci_workflow.png
+-rw-r--r--   0 runner    (1001) docker     (115)    12754 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/cumulusci_flow.rst
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:52.946115 cumulusci-3.9.1/docs/diagram/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:53.002115 cumulusci-3.9.1/docs/diagram/img/
+-rw-r--r--   0 runner    (1001) docker     (115)     4409 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/diagram/img/image1.png
+-rw-r--r--   0 runner    (1001) docker     (115)   108243 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/diagram/img/image12.png
+-rw-r--r--   0 runner    (1001) docker     (115)    26963 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/diagram/img/image15.png
+-rw-r--r--   0 runner    (1001) docker     (115)    68821 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/diagram/img/image17.png
+-rw-r--r--   0 runner    (1001) docker     (115)    78349 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/diagram/img/image3.png
+-rw-r--r--   0 runner    (1001) docker     (115)    38018 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/features.rst
+-rw-r--r--   0 runner    (1001) docker     (115)    53215 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/github-commit_status_error.png
+-rw-r--r--   0 runner    (1001) docker     (115)    51940 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/github-commit_status_pass.png
+-rw-r--r--   0 runner    (1001) docker     (115)    51527 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/github-creating_a_uat_release.png
+-rw-r--r--   0 runner    (1001) docker     (115)       28 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/history.rst
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-03-25 20:17:53.002115 cumulusci-3.9.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (115)     7203 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/images/env-var.png
+-rw-r--r--   0 runner    (1001) docker     (115)    67314 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/images/locate_elements_screenshot.png
+-rw-r--r--   0 runner    (1001) docker     (115)    15048 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/images/pipx.png
+-rw-r--r--   0 runner    (1001) docker     (115)   251244 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/images/salesforce-org-process.png
+-rw-r--r--   0 runner    (1001) docker     (115)   417827 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/images/windows_python.png
+-rw-r--r--   0 runner    (1001) docker     (115)      702 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (115)     3944 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (115)     6465 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (115)     9244 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/robotframework-debugger.rst
+-rw-r--r--   0 runner    (1001) docker     (115)    15403 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/robotframework-tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (115)    33005 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/robotframework.rst
+-rw-r--r--   0 runner    (1001) docker     (115)    91997 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/tasks.rst
+-rw-r--r--   0 runner    (1001) docker     (115)    37639 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (115)     1608 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (115)    12793 2020-03-25 20:17:40.000000 cumulusci-3.9.1/docs/why_cumulusci.rst
+-rw-r--r--   0 runner    (1001) docker     (115)      727 2020-03-25 20:17:40.000000 cumulusci-3.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (115)      230 2020-03-25 20:17:40.000000 cumulusci-3.9.1/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (115)      122 2020-03-25 20:17:53.006115 cumulusci-3.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (115)     2154 2020-03-25 20:17:40.000000 cumulusci-3.9.1/setup.py
```

### Comparing `cumulusci-3.9.0/AUTHORS.rst` & `cumulusci-3.9.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/CONTRIBUTING.rst` & `cumulusci-3.9.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/HISTORY.rst` & `cumulusci-3.9.1/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,31 @@
 =======
 History
 =======
 
+3.9.1 (2020-03-25)
+------------------
+
+Issues closed:
+
+* The ``batch_apex_wait`` task will now detect aborted and failed jobs instead of waiting indefinitely.
+
+* Fixed reporting of errors from Robot Framework when it exits with a return code > 250.
+
+* Fixed an ImportError that could happen when importing the new metadata ETL tasks.
+
+* Fixed bugs in how the ``set_organization_wide_defaults`` and ``update_admin_profile`` tasks operated in namespaced scratch orgs.
+
+* Show a more helpful error message if CumulusCI can't find a project's repository or release on GitHub. (#1281)
+
+* Fixed the message shown for skipped steps in ``cci flow info``.
+
+* Fixed a regression which accidentally removed support for the ``bulk_mode`` option in bulk data mappings.
+
+
 3.9.0 (2020-03-16)
 ------------------
 
 Critical changes:
 
 * The ``update_admin_profile`` task can now add field-level permissions for all packaged objects.
   This behavior is the default for projects with ``minimum_cumulusci_version`` >= 3.9.0 that are
```

### Comparing `cumulusci-3.9.0/LICENSE` & `cumulusci-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/PKG-INFO` & `cumulusci-3.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cumulusci
-Version: 3.9.0
+Version: 3.9.1
 Summary: Build and release tools for Salesforce developers
 Home-page: https://github.com/SFDO-Tooling/CumulusCI
 Author: Salesforce.org
 Author-email: jlantz@salesforce.com
 License: BSD license
 Description: ===============================
         CumulusCI
@@ -44,14 +44,34 @@
         The master branch now contains CumulusCI 2 which is not backwards compatible with the previous CumulusCI that was based on Ant. If you are using the Ant targets, please switch to using the `legacy-1.0` branch of the repository which contains the Ant based version. Or, consider upgrading to CumulusCI 2.
         
         
         =======
         History
         =======
         
+        3.9.1 (2020-03-25)
+        ------------------
+        
+        Issues closed:
+        
+        * The ``batch_apex_wait`` task will now detect aborted and failed jobs instead of waiting indefinitely.
+        
+        * Fixed reporting of errors from Robot Framework when it exits with a return code > 250.
+        
+        * Fixed an ImportError that could happen when importing the new metadata ETL tasks.
+        
+        * Fixed bugs in how the ``set_organization_wide_defaults`` and ``update_admin_profile`` tasks operated in namespaced scratch orgs.
+        
+        * Show a more helpful error message if CumulusCI can't find a project's repository or release on GitHub. (#1281)
+        
+        * Fixed the message shown for skipped steps in ``cci flow info``.
+        
+        * Fixed a regression which accidentally removed support for the ``bulk_mode`` option in bulk data mappings.
+        
+        
         3.9.0 (2020-03-16)
         ------------------
         
         Critical changes:
         
         * The ``update_admin_profile`` task can now add field-level permissions for all packaged objects.
           This behavior is the default for projects with ``minimum_cumulusci_version`` >= 3.9.0 that are
```

### Comparing `cumulusci-3.9.0/README.rst` & `cumulusci-3.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/cli/cci.py` & `cumulusci-3.9.1/cumulusci/cli/cci.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/cli/logger.py` & `cumulusci-3.9.1/cumulusci/cli/logger.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/cli/runtime.py` & `cumulusci-3.9.1/cumulusci/cli/runtime.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/cli/tests/test_cci.py` & `cumulusci-3.9.1/cumulusci/cli/tests/test_cci.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/cli/tests/test_logger.py` & `cumulusci-3.9.1/cumulusci/cli/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/cli/tests/test_runtime.py` & `cumulusci-3.9.1/cumulusci/cli/tests/test_runtime.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/cli/tests/test_ui.py` & `cumulusci-3.9.1/cumulusci/cli/tests/test_ui.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/cli/ui.py` & `cumulusci-3.9.1/cumulusci/cli/ui.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/conftest.py` & `cumulusci-3.9.1/cumulusci/conftest.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/config/BaseConfig.py` & `cumulusci-3.9.1/cumulusci/core/config/BaseConfig.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/config/BaseGlobalConfig.py` & `cumulusci-3.9.1/cumulusci/core/config/BaseGlobalConfig.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/config/BaseTaskFlowConfig.py` & `cumulusci-3.9.1/cumulusci/core/config/BaseTaskFlowConfig.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/config/OrgConfig.py` & `cumulusci-3.9.1/cumulusci/core/config/OrgConfig.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/config/ScratchOrgConfig.py` & `cumulusci-3.9.1/cumulusci/core/config/ScratchOrgConfig.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/config/__init__.py` & `cumulusci-3.9.1/cumulusci/core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/config/project_config.py` & `cumulusci-3.9.1/cumulusci/core/config/project_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from distutils.version import LooseVersion
 import os
 import re
 
 API_VERSION_RE = re.compile(r"^\d\d+\.0$")
 
+import github3
 import yaml
 
 from cumulusci.core.utils import merge_config
 from cumulusci.core.config import BaseTaskFlowConfig
 from cumulusci.core.exceptions import (
     ConfigError,
     DependencyResolutionError,
+    GithubException,
     KeychainNotFound,
     NamespaceNotFoundError,
     NotInProject,
     ProjectConfigNotFound,
 )
 from cumulusci.core.github import get_github_api_for_repo
 from cumulusci.core.github import find_latest_release
@@ -225,15 +227,15 @@
         keys = list(info.keys())
         keys.sort()
         for key in keys:
             self.logger.warning(f"  {key}: {info[key]}")
         self.logger.info("")
 
     def _split_repo_url(self, url):
-        url_parts = url.split("/")
+        url_parts = url.rstrip("/").split("/")
         name = url_parts[-1]
         owner = url_parts[-2]
         if name.endswith(".git"):
             name = name[:-4]
         git_info = {"url": url, "owner": owner, "name": name}
         return git_info
 
@@ -363,44 +365,57 @@
         return commit_sha
 
     def get_github_api(self, owner=None, repo=None):
         return get_github_api_for_repo(
             self.keychain, owner or self.repo_owner, repo or self.repo_name
         )
 
-    def get_latest_tag(self, beta=False):
-        """ Query Github Releases to find the latest production or beta tag """
+    def _get_repo(self):
         gh = self.get_github_api()
         repo = gh.repository(self.repo_owner, self.repo_name)
+        if repo is None:
+            raise GithubException(
+                f"Github repository not found or not authorized. ({self.repo_url})"
+            )
+        return repo
+
+    def get_latest_tag(self, beta=False):
+        """ Query Github Releases to find the latest production or beta tag """
+        repo = self._get_repo()
         if not beta:
-            release = repo.latest_release()
+            try:
+                release = repo.latest_release()
+            except github3.exceptions.NotFoundError:
+                raise GithubException(f"No release found for repo {self.repo_url}")
             prefix = self.project__git__prefix_release
             if not release.tag_name.startswith(prefix):
                 return self._get_latest_tag_for_prefix(repo, prefix)
             return release.tag_name
         else:
             return self._get_latest_tag_for_prefix(repo, self.project__git__prefix_beta)
 
     def _get_latest_tag_for_prefix(self, repo, prefix):
         for release in repo.releases():
             if not release.tag_name.startswith(prefix):
                 continue
             return release.tag_name
+        raise GithubException(
+            f"No release found for {self.repo_url} with tag prefix {prefix}"
+        )
 
     def get_latest_version(self, beta=False):
         """ Query Github Releases to find the latest production or beta release """
         tag = self.get_latest_tag(beta)
         version = self.get_version_for_tag(tag)
         if version is not None:
             return LooseVersion(version)
 
     def get_previous_version(self):
         """Query GitHub releases to find the previous production release"""
-        gh = self.get_github_api()
-        repo = gh.repository(self.repo_owner, self.repo_name)
+        repo = self._get_repo()
         release = find_previous_release(repo, self.project__git__prefix_release)
         if release is not None:
             return LooseVersion(self.get_version_for_tag(release.tag_name))
 
     @property
     def config_project_path(self):
         if not self.repo_root:
@@ -528,14 +543,18 @@
 
         # Initialize github3.py API against repo
         repo_owner, repo_name = dependency["github"].split("/")[3:5]
         if repo_name.endswith(".git"):
             repo_name = repo_name[:-4]
         gh = self.get_github_api(repo_owner, repo_name)
         repo = gh.repository(repo_owner, repo_name)
+        if repo is None:
+            raise DependencyResolutionError(
+                f"{indent}Github repository {dependency['github']} not found or not authorized."
+            )
 
         # Determine the commit
         release = None
         if "ref" in dependency:
             ref = dependency["ref"]
         else:
             if "tag" in dependency:
```

### Comparing `cumulusci-3.9.0/cumulusci/core/exceptions.py` & `cumulusci-3.9.1/cumulusci/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/flowrunner.py` & `cumulusci-3.9.1/cumulusci/core/flowrunner.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,15 +360,15 @@
                         "project_config": step.project_config,
                         "org_config": self.org_config,
                     }
                     expr = jinja2_env.compile_expression(step.when)
                     value = expr(**jinja2_context)
                     if not value:
                         self.logger.info(
-                            f"Skipping task {step.task_name} (skipped when {step.when})"
+                            f"Skipping task {step.task_name} (skipped unless {step.when})"
                         )
                         continue
 
                 self._rule(fill="-")
                 self.logger.info(f"Running task: {step.task_name}")
                 self._rule(fill="-", new_line=True)
```

### Comparing `cumulusci-3.9.0/cumulusci/core/github.py` & `cumulusci-3.9.1/cumulusci/core/github.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/keychain/BaseEncryptedProjectKeychain.py` & `cumulusci-3.9.1/cumulusci/core/keychain/BaseEncryptedProjectKeychain.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/keychain/BaseProjectKeychain.py` & `cumulusci-3.9.1/cumulusci/core/keychain/BaseProjectKeychain.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/keychain/EncryptedFileProjectKeychain.py` & `cumulusci-3.9.1/cumulusci/core/keychain/EncryptedFileProjectKeychain.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/keychain/EnvironmentProjectKeychain.py` & `cumulusci-3.9.1/cumulusci/core/keychain/EnvironmentProjectKeychain.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/keychain/__init__.py` & `cumulusci-3.9.1/cumulusci/core/keychain/__init__.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/runtime.py` & `cumulusci-3.9.1/cumulusci/core/runtime.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/sfdx.py` & `cumulusci-3.9.1/cumulusci/core/sfdx.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/source/github.py` & `cumulusci-3.9.1/cumulusci/core/source/github.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/source/local_folder.py` & `cumulusci-3.9.1/cumulusci/core/source/local_folder.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/tasks.py` & `cumulusci-3.9.1/cumulusci/core/tasks.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 """
 import contextlib
 import logging
 import os
 import time
 import threading
 
+from cumulusci import __version__
 from cumulusci.utils import cd
+from cumulusci.core.exceptions import ServiceNotValid, ServiceNotConfigured
 from cumulusci.core.exceptions import TaskRequiresSalesforceOrg
 from cumulusci.core.exceptions import TaskOptionsError
 
 CURRENT_TASK = threading.local()
 CURRENT_TASK.stack = []
 
 
@@ -219,7 +221,31 @@
                 "step_num": str(step.step_num),
                 "task_class": self.task_config.class_path,
                 "task_config": task_config,
                 "source": step.project_config.source.frozenspec,
             }
         )
         return [ui_step]
+
+
+class BaseSalesforceTask(BaseTask):
+    """Base for tasks that need a Salesforce org"""
+
+    name = "BaseSalesforceTask"
+    salesforce_task = True
+
+    def _get_client_name(self):
+        try:
+            app = self.project_config.keychain.get_service("connectedapp")
+            return app.client_id
+        except (ServiceNotValid, ServiceNotConfigured):
+            return "CumulusCI/{}".format(__version__)
+
+    def _run_task(self):
+        raise NotImplementedError("Subclasses should provide their own implementation")
+
+    def _update_credentials(self):
+        orig_config = self.org_config.config.copy()
+        self.org_config.refresh_oauth_token(self.project_config.keychain)
+        if self.org_config.config != orig_config:
+            self.logger.info("Org info updated, writing to keychain")
+            self.project_config.keychain.set_org(self.org_config)
```

### Comparing `cumulusci-3.9.0/cumulusci/core/template_utils.py` & `cumulusci-3.9.1/cumulusci/core/template_utils.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/tests/test_config.py` & `cumulusci-3.9.1/cumulusci/core/tests/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from cumulusci.core.config import BaseConfig
 from cumulusci.core.config import BaseGlobalConfig
 from cumulusci.core.config import BaseProjectConfig
 from cumulusci.core.config import BaseTaskFlowConfig
 from cumulusci.core.config import OrgConfig
 from cumulusci.core.exceptions import ConfigError
 from cumulusci.core.exceptions import DependencyResolutionError
+from cumulusci.core.exceptions import GithubException
 from cumulusci.core.exceptions import KeychainNotFound
 from cumulusci.core.exceptions import FlowNotFoundError
 from cumulusci.core.exceptions import NamespaceNotFoundError
 from cumulusci.core.exceptions import SalesforceCredentialsException
 from cumulusci.core.exceptions import TaskNotFoundError
 from cumulusci.core.source import LocalFolderSource
 from cumulusci.utils import temporary_dir
@@ -129,14 +130,15 @@
     def releases(self):
         return iter(self._releases)
 
     def latest_release(self):
         for release in self._releases:
             if release.tag_name.startswith("release/"):
                 return release
+        raise NotFoundError(DummyResponse("", 404))
 
     def release_from_tag(self, tag_name):
         for release in self._releases:
             if release.tag_name == tag_name:
                 return release
         raise NotFoundError(DummyResponse("", 404))
 
@@ -428,14 +430,38 @@
                 }
             },
         )
         config.get_github_api = mock.Mock(return_value=self._make_github())
         result = config.get_latest_tag(beta=True)
         self.assertEqual("beta/1.0-Beta_2", result)
 
+    def test_get_latest_tag__beta_not_found(self):
+        config = BaseProjectConfig(BaseGlobalConfig())
+        github = self._make_github()
+        github.repositories["CumulusCI"]._releases = []
+        config.get_github_api = mock.Mock(return_value=github)
+        with pytest.raises(GithubException):
+            config.get_latest_tag(beta=True)
+
+    def test_get_latest_tag__repo_not_found(self):
+        config = BaseProjectConfig(BaseGlobalConfig())
+        github = self._make_github()
+        github.repositories["CumulusCI"] = None
+        config.get_github_api = mock.Mock(return_value=github)
+        with pytest.raises(GithubException):
+            config.get_latest_tag()
+
+    def test_get_latest_tag__release_not_found(self):
+        config = BaseProjectConfig(BaseGlobalConfig())
+        github = self._make_github()
+        github.repositories["CumulusCI"]._releases = []
+        config.get_github_api = mock.Mock(return_value=github)
+        with pytest.raises(GithubException):
+            config.get_latest_tag()
+
     def test_get_latest_version(self):
         config = BaseProjectConfig(
             BaseGlobalConfig(),
             {
                 "project": {
                     "git": {"prefix_beta": "beta/", "prefix_release": "release/"}
                 }
@@ -784,14 +810,27 @@
                     "namespace_inject": "ccitest",
                     "namespace_strip": None,
                     "namespace_tokenize": None,
                 },
             ],
         )
 
+    def test_process_github_dependency__cannot_find_repo(self):
+        global_config = BaseGlobalConfig()
+        config = BaseProjectConfig(global_config)
+        config.keychain = DummyKeychain()
+        github = self._make_github()
+        github.repositories["CumulusCI-Test-Dep"] = None
+        config.get_github_api = mock.Mock(return_value=github)
+
+        with self.assertRaises(DependencyResolutionError):
+            config.process_github_dependency(
+                {"github": "https://github.com/SFDO-Tooling/CumulusCI-Test-Dep.git"}
+            )
+
     def test_process_github_dependency_cannot_find_latest(self):
         global_config = BaseGlobalConfig()
         config = BaseProjectConfig(global_config)
         config.keychain = DummyKeychain()
         github = self._make_github()
         github.repositories["CumulusCI-Test-Dep"]._releases = []
         config.get_github_api = mock.Mock(return_value=github)
```

### Comparing `cumulusci-3.9.0/cumulusci/core/tests/test_config_expensive.py` & `cumulusci-3.9.1/cumulusci/core/tests/test_config_expensive.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/tests/test_exceptions.py` & `cumulusci-3.9.1/cumulusci/core/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/tests/test_flowrunner.py` & `cumulusci-3.9.1/cumulusci/core/tests/test_flowrunner.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/tests/test_github.py` & `cumulusci-3.9.1/cumulusci/core/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/tests/test_keychain.py` & `cumulusci-3.9.1/cumulusci/core/tests/test_keychain.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/tests/test_pageobjects.py` & `cumulusci-3.9.1/cumulusci/core/tests/test_pageobjects.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/tests/test_salesforce.py` & `cumulusci-3.9.1/cumulusci/core/tests/test_salesforce.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/tests/test_salesforce_locators.py` & `cumulusci-3.9.1/cumulusci/core/tests/test_salesforce_locators.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/tests/test_sfdx.py` & `cumulusci-3.9.1/cumulusci/core/tests/test_sfdx.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/tests/test_source.py` & `cumulusci-3.9.1/cumulusci/core/tests/test_source.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/tests/test_tasks.py` & `cumulusci-3.9.1/cumulusci/core/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/tests/test_utils.py` & `cumulusci-3.9.1/cumulusci/core/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/tests/utils.py` & `cumulusci-3.9.1/cumulusci/core/tests/utils.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/core/utils.py` & `cumulusci-3.9.1/cumulusci/core/utils.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/cumulusci.yml` & `cumulusci-3.9.1/cumulusci/cumulusci.yml`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/files/metadata_whitelist.txt` & `cumulusci-3.9.1/cumulusci/files/metadata_whitelist.txt`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/files/templates/project/cumulusci.yml` & `cumulusci-3.9.1/cumulusci/files/templates/project/cumulusci.yml`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/files/templates/project/mapping.yml` & `cumulusci-3.9.1/cumulusci/files/templates/project/mapping.yml`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/files/templates/project/scratch_def.json` & `cumulusci-3.9.1/cumulusci/files/templates/project/scratch_def.json`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/oauth/salesforce.py` & `cumulusci-3.9.1/cumulusci/oauth/salesforce.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/oauth/tests/test_salesforce.py` & `cumulusci-3.9.1/cumulusci/oauth/tests/test_salesforce.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/CumulusCI.py` & `cumulusci-3.9.1/cumulusci/robotframework/CumulusCI.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/Salesforce.py` & `cumulusci-3.9.1/cumulusci/robotframework/Salesforce.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/Salesforce.robot` & `cumulusci-3.9.1/cumulusci/robotframework/Salesforce.robot`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/locator_manager.py` & `cumulusci-3.9.1/cumulusci/robotframework/locator_manager.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/locators_45.py` & `cumulusci-3.9.1/cumulusci/robotframework/locators_45.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/locators_46.py` & `cumulusci-3.9.1/cumulusci/robotframework/locators_46.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/locators_48.py` & `cumulusci-3.9.1/cumulusci/robotframework/locators_48.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/pageobjects/BasePageObjects.py` & `cumulusci-3.9.1/cumulusci/robotframework/pageobjects/BasePageObjects.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/pageobjects/PageObjectLibrary.py` & `cumulusci-3.9.1/cumulusci/robotframework/pageobjects/PageObjectLibrary.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/pageobjects/PageObjects.py` & `cumulusci-3.9.1/cumulusci/robotframework/pageobjects/PageObjects.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/pageobjects/baseobjects.py` & `cumulusci-3.9.1/cumulusci/robotframework/pageobjects/baseobjects.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/perftests/short/collection_perf.robot` & `cumulusci-3.9.1/cumulusci/robotframework/perftests/short/collection_perf.robot`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/tests/cumulusci/base.robot` & `cumulusci-3.9.1/cumulusci/robotframework/tests/cumulusci/base.robot`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/tests/cumulusci/bulkdata.robot` & `cumulusci-3.9.1/cumulusci/robotframework/tests/cumulusci/bulkdata.robot`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/tests/cumulusci/communities.robot` & `cumulusci-3.9.1/cumulusci/robotframework/tests/cumulusci/communities.robot`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/tests/cumulusci/datagen.robot` & `cumulusci-3.9.1/cumulusci/robotframework/tests/cumulusci/datagen.robot`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/tests/salesforce/TestLibraryA.py` & `cumulusci-3.9.1/cumulusci/robotframework/tests/salesforce/TestLibraryA.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/tests/salesforce/TestListener.py` & `cumulusci-3.9.1/cumulusci/robotframework/tests/salesforce/TestListener.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/tests/salesforce/api.robot` & `cumulusci-3.9.1/cumulusci/robotframework/tests/salesforce/api.robot`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/tests/salesforce/browsers.robot` & `cumulusci-3.9.1/cumulusci/robotframework/tests/salesforce/browsers.robot`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/tests/salesforce/create_contact.robot` & `cumulusci-3.9.1/cumulusci/robotframework/tests/salesforce/create_contact.robot`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/tests/salesforce/locators.robot` & `cumulusci-3.9.1/cumulusci/robotframework/tests/salesforce/locators.robot`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/tests/salesforce/pageobjects/base_pageobjects.robot` & `cumulusci-3.9.1/cumulusci/robotframework/tests/salesforce/pageobjects/base_pageobjects.robot`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/tests/salesforce/pageobjects/example_page_object.py` & `cumulusci-3.9.1/cumulusci/robotframework/tests/salesforce/pageobjects/example_page_object.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/tests/salesforce/pageobjects/pageobjects.robot` & `cumulusci-3.9.1/cumulusci/robotframework/tests/salesforce/pageobjects/pageobjects.robot`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/tests/salesforce/populate.robot` & `cumulusci-3.9.1/cumulusci/robotframework/tests/salesforce/populate.robot`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/tests/salesforce/test_testlistener.py` & `cumulusci-3.9.1/cumulusci/robotframework/tests/salesforce/test_testlistener.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/tests/salesforce/ui.robot` & `cumulusci-3.9.1/cumulusci/robotframework/tests/salesforce/ui.robot`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/tests/test_locator_manager.py` & `cumulusci-3.9.1/cumulusci/robotframework/tests/test_locator_manager.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/tests/test_template_util.py` & `cumulusci-3.9.1/cumulusci/robotframework/tests/test_template_util.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/tests/test_utils.py` & `cumulusci-3.9.1/cumulusci/robotframework/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/robotframework/utils.py` & `cumulusci-3.9.1/cumulusci/robotframework/utils.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/salesforce_api/exceptions.py` & `cumulusci-3.9.1/cumulusci/salesforce_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/salesforce_api/metadata.py` & `cumulusci-3.9.1/cumulusci/salesforce_api/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,22 @@
 from cumulusci.salesforce_api import soap_envelopes
 from cumulusci.core.exceptions import ApexTestException
 from cumulusci.utils import zip_subfolder, parse_api_datetime
 from cumulusci.salesforce_api.exceptions import MetadataComponentFailure
 from cumulusci.salesforce_api.exceptions import MetadataParseError
 from cumulusci.salesforce_api.exceptions import MetadataApiError
 
-from urllib3.contrib import pyopenssl
-
-pyopenssl.extract_from_urllib3()
+# If pyOpenSSL is installed, make sure it's not used for requests
+# (it's not needed in the verisons of Python we support)
+try:
+    from urllib3.contrib import pyopenssl
+except ImportError:
+    pass
+else:
+    pyopenssl.extract_from_urllib3()
 
 retry_policy = Retry(backoff_factor=0.3)
 
 
 class BaseMetadataApiCall(object):
     check_interval = 1
     soap_envelope_start = None
```

### Comparing `cumulusci-3.9.0/cumulusci/salesforce_api/package_zip.py` & `cumulusci-3.9.1/cumulusci/salesforce_api/package_zip.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/salesforce_api/soap_envelopes.py` & `cumulusci-3.9.1/cumulusci/salesforce_api/soap_envelopes.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/salesforce_api/tests/metadata_test_strings.py` & `cumulusci-3.9.1/cumulusci/salesforce_api/tests/metadata_test_strings.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/salesforce_api/tests/test_metadata.py` & `cumulusci-3.9.1/cumulusci/salesforce_api/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/salesforce_api/tests/test_package_zip.py` & `cumulusci-3.9.1/cumulusci/salesforce_api/tests/test_package_zip.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/salesforce_api/tests/test_utils.py` & `cumulusci-3.9.1/cumulusci/salesforce_api/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/salesforce_api/utils.py` & `cumulusci-3.9.1/cumulusci/salesforce_api/utils.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/apex/anon.py` & `cumulusci-3.9.1/cumulusci/tasks/apex/anon.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/apex/batch.py` & `cumulusci-3.9.1/cumulusci/tasks/apex/batch.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from datetime import datetime
 from typing import Sequence, Optional
 
 from cumulusci.utils import parse_api_datetime
 from cumulusci.tasks.salesforce import BaseSalesforceApiTask
 from cumulusci.core.exceptions import SalesforceException
 
-COMPLETED_STATUSES = ["Completed"]
+COMPLETED_STATUSES = ["Completed", "Aborted", "Failed"]
+STOPPED_STATUSES = ["Aborted"]
+FAILED_STATUSES = ["Failed"]
 
 
 class BatchApexWait(BaseSalesforceApiTask):
     """ BatchApexWait polls an org until the latest batch job
         for an apex class completes or fails."""
 
     name = "BatchApexWait"
@@ -32,16 +34,25 @@
 
         self._poll()  # will block until poll_complete
 
         self.logger.info("Job is complete.")
 
         summary = self.summarize_subjobs(self.subjobs)
         failed_batches = self.failed_batches(self.subjobs)
-
-        if failed_batches:
+        job_aborted = summary["AnyAborted"]
+        job_failed = summary[
+            "AnyFailed"
+        ]  # note that a failed sub-job is different than a failed batch
+
+        # per https://help.salesforce.com/articleView?id=code_apex_job.htm&type=5
+        if job_aborted:
+            raise SalesforceException("Job was aborted by a user.")
+        elif job_failed:
+            raise SalesforceException("Job experienced a system failure.")
+        elif failed_batches:
             self.logger.info("There have been some batch failures.")
             raise SalesforceException(
                 f"There were batch errors: {repr(failed_batches)}"
             )
         elif not summary["CountsAddUp"]:
             self.logger.info("The final record counts do not add up.")
             self.logger.info("This is probably related to W-1132237")
@@ -118,14 +129,18 @@
         rc = {
             "JobItemsProcessed": reduce_key("JobItemsProcessed", sum),
             "TotalJobItems": reduce_key("TotalJobItems", sum),
             "NumberOfErrors": reduce_key("NumberOfErrors", sum),
             "Completed": all(
                 subjob["Status"] in COMPLETED_STATUSES for subjob in subjobs
             ),
+            "AnyAborted": any(
+                subjob["Status"] in STOPPED_STATUSES for subjob in subjobs
+            ),
+            "AnyFailed": any(subjob["Status"] in FAILED_STATUSES for subjob in subjobs),
         }
         rc["Success"] = rc["NumberOfErrors"] == 0
         rc["ElapsedTime"] = self.elapsed_time(subjobs)
         rc["CountsAddUp"] = rc["JobItemsProcessed"] == rc["TotalJobItems"]
         return rc
 
     def elapsed_time(self, subjobs: Sequence[dict]):
```

### Comparing `cumulusci-3.9.0/cumulusci/tasks/apex/testrunner.py` & `cumulusci-3.9.1/cumulusci/tasks/apex/testrunner.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/apex/tests/test_apex_tasks.py` & `cumulusci-3.9.1/cumulusci/tasks/apex/tests/test_apex_tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -859,14 +859,39 @@
         task, url = self._get_url_and_task()
         response = self._get_query_resp()
         responses.add(responses.GET, url, json=response)
         task()
         self.assertEqual(task.elapsed_time(task.subjobs), 61)
 
     @responses.activate
+    def test_run_batch_apex_status_aborted(self):
+        task, url = self._get_url_and_task()
+        response = self._get_query_resp()
+        response["records"][0]["Status"] = "Aborted"
+        response["records"][0]["JobItemsProcessed"] = 1
+        response["records"][0]["TotalJobItems"] = 3
+        responses.add(responses.GET, url, json=response)
+        with self.assertRaises(SalesforceException) as e:
+            task()
+        assert "aborted" in str(e.exception)
+
+    @responses.activate
+    def test_run_batch_apex_status_failed(self):
+        task, url = self._get_url_and_task()
+        response = self._get_query_resp()
+        response["records"][0]["Status"] = "Failed"
+        response["records"][0]["JobItemsProcessed"] = 1
+        response["records"][0]["TotalJobItems"] = 3
+        responses.add(responses.GET, url, json=response)
+        self.task_log["info"] = []
+        with self.assertRaises(SalesforceException) as e:
+            task()
+        assert "failure" in str(e.exception)
+
+    @responses.activate
     def test_chained_subjobs(self):
         "Test subjobs that kick off a successor before they complete"
         task, url = self._get_url_and_task()
         url2 = (
             url.split("?")[0]
             + "?q=SELECT+Id%2C+ApexClass.Name%2C+Status%2C+ExtendedStatus%2C+TotalJobItems%2C+JobItemsProcessed%2C+NumberOfErrors%2C+CreatedDate%2C+CompletedDate+FROM+AsyncApexJob+WHERE+JobType%3D%27BatchApex%27+AND+ApexClass.Name%3D%27ADDR_Seasonal_BATCH%27++AND+CreatedDate+%3E%3D+2018-08-07T16%3A00%3A00Z++ORDER+BY+CreatedDate+DESC++"
         )
```

### Comparing `cumulusci-3.9.0/cumulusci/tasks/bulkdata/base_generate_data_task.py` & `cumulusci-3.9.1/cumulusci/tasks/bulkdata/base_generate_data_task.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/bulkdata/delete.py` & `cumulusci-3.9.1/cumulusci/tasks/bulkdata/delete.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/bulkdata/extract.py` & `cumulusci-3.9.1/cumulusci/tasks/bulkdata/extract.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/bulkdata/factory_utils.py` & `cumulusci-3.9.1/cumulusci/tasks/bulkdata/factory_utils.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/bulkdata/generate_and_load_data.py` & `cumulusci-3.9.1/cumulusci/tasks/bulkdata/generate_and_load_data.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/bulkdata/generate_and_load_data_from_yaml.py` & `cumulusci-3.9.1/cumulusci/tasks/bulkdata/generate_and_load_data_from_yaml.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/bulkdata/generate_from_yaml.py` & `cumulusci-3.9.1/cumulusci/tasks/bulkdata/generate_from_yaml.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/bulkdata/generate_mapping.py` & `cumulusci-3.9.1/cumulusci/tasks/bulkdata/generate_mapping.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/bulkdata/load.py` & `cumulusci-3.9.1/cumulusci/tasks/bulkdata/load.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from collections import defaultdict
 import datetime
+from unittest.mock import MagicMock
+from typing import Union
+
 from sqlalchemy import Column, MetaData, Table, Unicode, create_engine, text
 from sqlalchemy.orm import aliased, Session
 from sqlalchemy.ext.automap import automap_base
 
 from cumulusci.core.exceptions import BulkDataException, TaskOptionsError
 from cumulusci.core.utils import process_bool_arg
 from cumulusci.tasks.bulkdata.utils import (
@@ -11,19 +14,20 @@
     SqlAlchemyMixin,
     RowErrorChecker,
 )
 from cumulusci.tasks.bulkdata.step import (
     BulkApiDmlOperation,
     DataOperationStatus,
     DataOperationType,
+    DataOperationJobResult,
 )
 from cumulusci.tasks.salesforce import BaseSalesforceApiTask
 from cumulusci.utils import os_friendly_path
 
-from cumulusci.tasks.bulkdata.mapping_parser import parse_from_yaml
+from cumulusci.tasks.bulkdata.mapping_parser import parse_from_yaml, MappingStep
 
 
 class LoadData(BaseSalesforceApiTask, SqlAlchemyMixin):
     """Perform Bulk API operations to load data defined by a mapping from a local store into an org."""
 
     task_options = {
         "database_url": {
@@ -88,30 +92,32 @@
             if not started and start_step and name != start_step:
                 self.logger.info(f"Skipping step: {name}")
                 continue
 
             started = True
 
             self.logger.info(f"Running step: {name}")
-            result = self._load_mapping(mapping)
+            result = self._execute_step(mapping)
             if result.status is DataOperationStatus.JOB_FAILURE:
                 raise BulkDataException(
                     f"Step {name} did not complete successfully: {','.join(result.job_errors)}"
                 )
 
             if name in self.after_steps:
                 for after_name, after_step in self.after_steps[name].items():
                     self.logger.info(f"Running post-load step: {after_name}")
-                    result = self._load_mapping(after_step)
+                    result = self._execute_step(after_step)
                     if result.status is DataOperationStatus.JOB_FAILURE:
                         raise BulkDataException(
                             f"Step {after_name} did not complete successfully: {','.join(result.job_errors)}"
                         )
 
-    def _load_mapping(self, mapping):
+    def _execute_step(
+        self, mapping: MappingStep
+    ) -> Union[DataOperationJobResult, MagicMock]:
         """Load data for a single step."""
 
         if mapping.get("fields", {}).get("RecordTypeId"):
             conn = self.session.connection()
             self._load_record_types([mapping["sf_object"]], conn)
             self.session.commit()
```

### Comparing `cumulusci-3.9.0/cumulusci/tasks/bulkdata/mapping_parser.py` & `cumulusci-3.9.1/cumulusci/tasks/bulkdata/mapping_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Dict, List, Union, IO
 from logging import getLogger
 from pathlib import Path
 
 from pydantic import Field, validator, ValidationError
 
 from cumulusci.utils.yaml.model_parser import CCIDictModel
+from typing_extensions import Literal
 
 LOGGER_NAME = "MAPPING_LOADER"
 logger = getLogger(LOGGER_NAME)
 
 
 class MappingLookup(CCIDictModel):
     "Lookup relationship between two tables."
@@ -27,14 +28,15 @@
     fields_: Dict[str, str] = Field(..., alias="fields")
     lookups: Dict[str, MappingLookup] = {}
     static: Dict[str, str] = {}
     filters: List[str] = []
     action: str = "insert"
     oid_as_pk: bool = False  # this one should be discussed and probably deprecated
     record_type: str = None  # should be discussed and probably deprecated
+    bulk_mode: Literal["Serial", "Parallel"] = "Parallel"
 
     @validator("record_type")
     def record_type_is_deprecated(cls, v):
         logger.warning(
             "record_type is deprecated. Just supply a RecordTypeId column declaration and it will be inferred"
         )
         return v
```

### Comparing `cumulusci-3.9.0/cumulusci/tasks/bulkdata/step.py` & `cumulusci-3.9.1/cumulusci/tasks/bulkdata/step.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/dummy_data_factory.py` & `cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/dummy_data_factory.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/mapping-oid.yml` & `cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/mapping-oid.yml`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/mapping_after.yml` & `cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/mapping_after.yml`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/mapping_v1.yml` & `cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/mapping_v1.yml`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/mapping_vanilla_sf.yml` & `cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/mapping_vanilla_sf.yml`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/test_base_generate_data_tasks.py` & `cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/test_base_generate_data_tasks.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/test_delete.py` & `cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/test_extract.py` & `cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/test_factory_utils.py` & `cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/test_factory_utils.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/test_generate_and_load.py` & `cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/test_generate_and_load.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/test_generatemapping.py` & `cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/test_generatemapping.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/test_load.py` & `cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/test_load.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     DataOperationJobResult,
     DataOperationType,
     DataOperationStatus,
     BaseDmlOperation,
 )
 from cumulusci.tasks.bulkdata.tests.utils import _make_task
 from cumulusci.utils import temporary_dir
-from cumulusci.tasks.bulkdata.mapping_parser import MappingLookup
+from cumulusci.tasks.bulkdata.mapping_parser import MappingLookup, MappingStep
 
 
 MAPPING_FILE = """Insert Households:
     sf_object: Account
     table: households
     fields:
         Id: sf_id
@@ -47,15 +47,17 @@
             table: households
             join_field: household_id
             value_field: sf_id
 """
 
 
 class MockBulkApiDmlOperation(BaseDmlOperation):
-    def __init__(self, *, sobject, operation, api_options, context, fields):
+    def __init__(
+        self, *, context, sobject=None, operation=None, api_options=None, fields=None,
+    ):
         super().__init__(
             sobject=sobject,
             operation=operation,
             api_options=api_options,
             context=context,
             fields=fields,
         )
@@ -162,22 +164,24 @@
                     "start_step": "Insert Contacts",
                 }
             },
         )
         task._init_db = mock.Mock()
         task._init_mapping = mock.Mock()
         task.mapping = {}
-        task.mapping["Insert Households"] = {"one": 1}
-        task.mapping["Insert Contacts"] = {"two": 2}
+        task.mapping["Insert Households"] = MappingStep(sf_object="one", fields={})
+        task.mapping["Insert Contacts"] = MappingStep(sf_object="two", fields={})
         task.after_steps = {}
-        task._load_mapping = mock.Mock(
+        task._execute_step = mock.Mock(
             return_value=DataOperationJobResult(DataOperationStatus.SUCCESS, [], 0, 0)
         )
         task()
-        task._load_mapping.assert_called_once_with({"two": 2, "action": "insert"})
+        task._execute_step.assert_called_once_with(
+            MappingStep(sf_object="two", fields={})
+        )
 
     def test_run_task__after_steps(self):
         task = _make_task(
             LoadData,
             {"options": {"database_url": "sqlite://", "mapping": "mapping.yml"}},
         )
         task._init_db = mock.Mock()
@@ -189,19 +193,19 @@
         households_steps = {}
         households_steps["four"] = 4
         households_steps["five"] = 5
         task.after_steps = {
             "Insert Contacts": {"three": 3},
             "Insert Households": households_steps,
         }
-        task._load_mapping = mock.Mock(
+        task._execute_step = mock.Mock(
             return_value=DataOperationJobResult(DataOperationStatus.SUCCESS, [], 0, 0)
         )
         task()
-        task._load_mapping.assert_has_calls(
+        task._execute_step.assert_has_calls(
             [mock.call(1), mock.call(4), mock.call(5), mock.call(2), mock.call(3)]
         )
 
     def test_run_task__after_steps_failure(self):
         task = _make_task(
             LoadData,
             {"options": {"database_url": "sqlite://", "mapping": "mapping.yml"}},
@@ -215,15 +219,15 @@
         households_steps = {}
         households_steps["four"] = 4
         households_steps["five"] = 5
         task.after_steps = {
             "Insert Contacts": {"three": 3},
             "Insert Households": households_steps,
         }
-        task._load_mapping = mock.Mock(
+        task._execute_step = mock.Mock(
             side_effect=[
                 DataOperationJobResult(DataOperationStatus.SUCCESS, [], 0, 0),
                 DataOperationJobResult(DataOperationStatus.JOB_FAILURE, [], 0, 0),
             ]
         )
         with self.assertRaises(BulkDataException):
             task()
@@ -298,40 +302,14 @@
 
         assert t.bulk_mode is None
 
     def test_init_options__bulk_mode_wrong(self):
         with self.assertRaises(TaskOptionsError):
             _make_task(LoadData, {"options": {"bulk_mode": "Test"}})
 
-    @mock.patch("cumulusci.tasks.bulkdata.load.BulkApiDmlOperation")
-    def test_bulk_mode_override(self, stepmock):
-        task = _make_task(
-            LoadData,
-            {
-                "options": {
-                    "database_url": "file:///test.db",
-                    "mapping": "mapping.yml",
-                    "bulk_mode": "Serial",
-                }
-            },
-        )
-        task.session = mock.Mock()
-        task._load_record_types = mock.Mock()
-        task._process_job_results = mock.Mock()
-
-        task._load_mapping(
-            {
-                "sf_object": "Account",
-                "action": "insert",
-                "fields": {"Name": "Name"},
-                "bulk_mode": "XYZZY",
-            }
-        )
-        assert stepmock.mock_calls[0][2]["api_options"]["bulk_mode"] == "XYZZY"
-
     def test_init_options__database_url(self):
         t = _make_task(
             LoadData,
             {"options": {"database_url": "file:///test.db", "mapping": "mapping.yml"}},
         )
 
         assert t.options["database_url"] == "file:///test.db"
@@ -603,15 +581,15 @@
     def test_run_task__exception_failure(self):
         task = _make_task(
             LoadData,
             {"options": {"database_url": "sqlite://", "mapping": "mapping.yml"}},
         )
         task._init_db = mock.Mock()
         task._init_mapping = mock.Mock()
-        task._load_mapping = mock.Mock(
+        task._execute_step = mock.Mock(
             return_value=DataOperationJobResult(
                 DataOperationStatus.JOB_FAILURE, [], 0, 0
             )
         )
         task.mapping = {"Test": {"test": "test"}}
 
         with self.assertRaises(BulkDataException):
@@ -850,36 +828,44 @@
 
         assert list(generator) == [
             ("001000000000009", "001000000000000"),
             ("001000000000011", "001000000000002"),
         ]
 
     @mock.patch("cumulusci.tasks.bulkdata.load.BulkApiDmlOperation")
-    def test_load_mapping__record_type_mapping(self, step_mock):
+    def test_execute_step__record_type_mapping(self, step_mock):
         task = _make_task(
             LoadData,
             {"options": {"database_url": "sqlite://", "mapping": "mapping.yml"}},
         )
 
         task.session = mock.Mock()
         task._load_record_types = mock.Mock()
         task._process_job_results = mock.Mock()
 
-        task._load_mapping(
-            {"sf_object": "Account", "action": "insert", "fields": {"Name": "Name"}}
+        task._execute_step(
+            MappingStep(
+                **{
+                    "sf_object": "Account",
+                    "action": "insert",
+                    "fields": {"Name": "Name"},
+                }
+            )
         )
 
         task._load_record_types.assert_not_called()
 
-        task._load_mapping(
-            {
-                "sf_object": "Account",
-                "action": "insert",
-                "fields": {"Name": "Name", "RecordTypeId": "RecordTypeId"},
-            }
+        task._execute_step(
+            MappingStep(
+                **{
+                    "sf_object": "Account",
+                    "action": "insert",
+                    "fields": {"Name": "Name", "RecordTypeId": "RecordTypeId"},
+                }
+            )
         )
         task._load_record_types.assert_called_once_with(
             ["Account"], task.session.connection.return_value
         )
 
     def test_query_db__record_type_mapping(self):
         task = _make_task(
```

### Comparing `cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/test_mapping_parser.py` & `cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/test_mapping_parser.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/test_step.py` & `cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/test_step.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/test_utils.py` & `cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/tests/test_generate_from_snowfakery_task.py` & `cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/tests/test_generate_from_snowfakery_task.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/bulkdata/tests/utils.py` & `cumulusci-3.9.1/cumulusci/tasks/bulkdata/tests/utils.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/bulkdata/utils.py` & `cumulusci-3.9.1/cumulusci/tasks/bulkdata/utils.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/command.py` & `cumulusci-3.9.1/cumulusci/tasks/command.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/connectedapp.py` & `cumulusci-3.9.1/cumulusci/tasks/connectedapp.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/datadictionary.py` & `cumulusci-3.9.1/cumulusci/tasks/datadictionary.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/github/base.py` & `cumulusci-3.9.1/cumulusci/tasks/github/base.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/github/merge.py` & `cumulusci-3.9.1/cumulusci/tasks/github/merge.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/github/release.py` & `cumulusci-3.9.1/cumulusci/tasks/github/release.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/github/release_report.py` & `cumulusci-3.9.1/cumulusci/tasks/github/release_report.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/github/tag.py` & `cumulusci-3.9.1/cumulusci/tasks/github/tag.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/github/tests/test_merge.py` & `cumulusci-3.9.1/cumulusci/tasks/github/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/github/tests/test_pull_request.py` & `cumulusci-3.9.1/cumulusci/tasks/github/tests/test_pull_request.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/github/tests/test_release.py` & `cumulusci-3.9.1/cumulusci/tasks/github/tests/test_release.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,19 @@
 class TestCreateRelease(unittest.TestCase, GithubApiTestMixin):
     def setUp(self):
         self.repo_owner = "TestOwner"
         self.repo_name = "TestRepo"
         self.repo_api_url = "https://api.github.com/repos/{}/{}".format(
             self.repo_owner, self.repo_name
         )
-        self.project_config = create_project_config(self.repo_name, self.repo_owner)
-        self.project_config._repo_commit = "21e04cfe480f5293e2f7103eee8a5cbdb94f7982"
+        self.project_config = create_project_config(
+            self.repo_name,
+            self.repo_owner,
+            repo_commit="21e04cfe480f5293e2f7103eee8a5cbdb94f7982",
+        )
         self.project_config.keychain.set_service(
             "github",
             ServiceConfig(
                 {
                     "username": "TestUser",
                     "password": "TestPass",
                     "email": "testuser@testdomain.com",
@@ -119,15 +122,15 @@
             json=self._get_expected_repo(owner=self.repo_owner, name=self.repo_name),
         )
         responses.add(
             method=responses.GET,
             url=self.repo_api_url + "/releases/tags/release/1.0",
             status=404,
         )
-        del self.project_config._repo_commit
+        del self.project_config._repo_info["commit"]
 
         with self.assertRaises(GithubException):
             CreateRelease(
                 self.project_config,
                 TaskConfig({"options": {"version": "1.0", "commit": None}}),
             )
 
@@ -139,13 +142,13 @@
             json=self._get_expected_repo(owner=self.repo_owner, name=self.repo_name),
         )
         responses.add(
             method=responses.GET,
             url=self.repo_api_url + "/releases/tags/release/1.0",
             status=404,
         )
-        self.project_config._repo_commit = "too_short"
+        self.project_config._repo_info["commit"] = "too_short"
 
         with self.assertRaises(TaskOptionsError):
             CreateRelease(
                 self.project_config, TaskConfig({"options": {"version": "1.0"}})
             )
```

### Comparing `cumulusci-3.9.0/cumulusci/tasks/github/tests/test_release_report.py` & `cumulusci-3.9.1/cumulusci/tasks/github/tests/test_release_report.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/github/tests/test_tag.py` & `cumulusci-3.9.1/cumulusci/tasks/github/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/github/tests/test_util.py` & `cumulusci-3.9.1/cumulusci/tasks/github/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/github/tests/util_github_api.py` & `cumulusci-3.9.1/cumulusci/tasks/github/tests/util_github_api.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/github/util.py` & `cumulusci-3.9.1/cumulusci/tasks/github/util.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/metadata/ee_src.py` & `cumulusci-3.9.1/cumulusci/tasks/metadata/ee_src.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/metadata/managed_src.py` & `cumulusci-3.9.1/cumulusci/tasks/metadata/managed_src.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/metadata/metadata_map.yml` & `cumulusci-3.9.1/cumulusci/tasks/metadata/metadata_map.yml`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/metadata/modify.py` & `cumulusci-3.9.1/cumulusci/tasks/metadata/modify.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/metadata/package.py` & `cumulusci-3.9.1/cumulusci/tasks/metadata/package.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/metadata/tests/test_ee_src.py` & `cumulusci-3.9.1/cumulusci/tasks/metadata/tests/test_ee_src.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/metadata/tests/test_managed_src.py` & `cumulusci-3.9.1/cumulusci/tasks/metadata/tests/test_managed_src.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/metadata/tests/test_modify.py` & `cumulusci-3.9.1/cumulusci/tasks/metadata/tests/test_modify.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/metadata/tests/test_package.py` & `cumulusci-3.9.1/cumulusci/tasks/metadata/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/metadata_etl/__init__.py` & `cumulusci-3.9.1/cumulusci/tasks/metadata_etl/__init__.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/metadata_etl/base.py` & `cumulusci-3.9.1/cumulusci/tasks/metadata_etl/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from abc import ABCMeta, abstractmethod
 import enum
 from pathlib import Path
 import tempfile
 from urllib.parse import quote, unquote
 
 from cumulusci.core.exceptions import CumulusCIException
-from cumulusci.tasks.salesforce import BaseSalesforceApiTask, Deploy
+from cumulusci.core.tasks import BaseSalesforceTask
 from cumulusci.salesforce_api.metadata import ApiRetrieveUnpackaged
 from cumulusci.tasks.metadata.package import PackageXmlGenerator
 from cumulusci.core.utils import process_bool_arg, process_list_arg
 from cumulusci.utils import inject_namespace
 from cumulusci.core.config import TaskConfig
 from cumulusci.utils.xml import metadata_tree
 
 
 class MetadataOperation(enum.Enum):
     DEPLOY = "deploy"
     RETRIEVE = "retrieve"
 
 
-class BaseMetadataETLTask(BaseSalesforceApiTask, metaclass=ABCMeta):
+class BaseMetadataETLTask(BaseSalesforceTask, metaclass=ABCMeta):
     """Abstract base class for all Metadata ETL tasks. Concrete tasks should
     generally subclass BaseMetadataSynthesisTask, BaseMetadataTransformTask,
     or MetadataSingleEntityTransformTask."""
 
     deploy = False
     retrieve = False
 
@@ -92,14 +92,17 @@
         """Deploy metadata from self.deploy_dir"""
         self.logger.info("Loading transformed metadata...")
         target_profile_xml = Path(self.deploy_dir, "package.xml")
         target_profile_xml.write_text(
             self._generate_package_xml(MetadataOperation.DEPLOY)
         )
 
+        # import is here to avoid an import cycle
+        from cumulusci.tasks.salesforce import Deploy
+
         api = Deploy(
             self.project_config,
             TaskConfig(
                 {
                     "options": {
                         "path": self.deploy_dir,
                         "namespace_inject": self.options.get("namespace_inject"),
```

### Comparing `cumulusci-3.9.0/cumulusci/tasks/metadata_etl/layouts.py` & `cumulusci-3.9.1/cumulusci/tasks/metadata_etl/layouts.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/metadata_etl/permissions.py` & `cumulusci-3.9.1/cumulusci/tasks/metadata_etl/permissions.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/metadata_etl/sharing.py` & `cumulusci-3.9.1/cumulusci/tasks/metadata_etl/sharing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from datetime import datetime
 
 from cumulusci.core.exceptions import CumulusCIException, TaskOptionsError
 from cumulusci.tasks.metadata_etl import MetadataSingleEntityTransformTask
+from cumulusci.tasks.salesforce import BaseSalesforceApiTask
 from cumulusci.utils.xml.metadata_tree import MetadataElement
 
 
-class SetOrgWideDefaults(MetadataSingleEntityTransformTask):
+class SetOrgWideDefaults(MetadataSingleEntityTransformTask, BaseSalesforceApiTask):
     entity = "CustomObject"
     task_options = {
         "org_wide_defaults": {
             "description": "The target Organization-Wide Defaults, "
             "organized as a list with each element containing the keys api_name, "
             "internal_sharing_model, and external_sharing_model. NOTE: you must have "
             "External Sharing Model turned on in Sharing Settings to use the latter feature.",
@@ -100,18 +101,27 @@
         elapsed = datetime.now() - self.time_start
         if elapsed.total_seconds() > self.options["timeout"]:
             raise CumulusCIException(
                 f'Sharing enablement not completed after {self.options["timeout"]} seconds'
             )
 
         for sobject in self.owds:
+            # The Tooling API requires that we use fully-qualified sObject names in namespaced scratch orgs.
+            # However, the Metadata API requires no namespaces in that context.
+            # Dynamically inject the namespace if required.
+            real_api_name = (
+                f"{self.project_config.project__package__namespace}__{sobject}"
+                if self.org_config.namespaced and sobject.count("__") == 1
+                else sobject
+            )
+
             result = self.sf.query(
                 f"SELECT ExternalSharingModel, InternalSharingModel "
                 f"FROM EntityDefinition "
-                f"WHERE QualifiedApiName = '{sobject}'"
+                f"WHERE QualifiedApiName = '{real_api_name}'"
             )
             if result["totalSize"] == 1:
                 record = result["records"][0]
                 if (
                     self.owds[sobject]["internal_sharing_model"]
                     and record["InternalSharingModel"]
                     != self.owds[sobject]["internal_sharing_model"]
```

### Comparing `cumulusci-3.9.0/cumulusci/tasks/metadata_etl/tests/test_base.py` & `cumulusci-3.9.1/cumulusci/tasks/metadata_etl/tests/test_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             task, task._generate_package_xml(False), "47.0"
         )
         api_mock.return_value.assert_called_once_with()
         api_mock.return_value.return_value.extractall.assert_called_once_with(
             task.retrieve_dir
         )
 
-    @mock.patch("cumulusci.tasks.metadata_etl.base.Deploy")
+    @mock.patch("cumulusci.tasks.salesforce.Deploy")
     def test_deploy(self, deploy_mock):
         with tempfile.TemporaryDirectory() as tmpdir:
             task = create_task(
                 MetadataETLTask,
                 {"managed": False, "namespace_inject": "test", "api_version": "47.0"},
             )
             task.deploy_dir = Path(tmpdir)
```

### Comparing `cumulusci-3.9.0/cumulusci/tasks/metadata_etl/tests/test_layouts.py` & `cumulusci-3.9.1/cumulusci/tasks/metadata_etl/tests/test_layouts.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/metadata_etl/tests/test_permissions.py` & `cumulusci-3.9.1/cumulusci/tasks/metadata_etl/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/metadata_etl/tests/test_sharing.py` & `cumulusci-3.9.1/cumulusci/tasks/metadata_etl/tests/test_sharing.py`

 * *Files 10% similar despite different names*

```diff
@@ -172,14 +172,82 @@
                 mock.call(query.format("Account")),
                 mock.call(query.format("Test__c")),
             ]
         )
 
         assert task.poll_complete
 
+    def test_post_deploy_waits_for_enablement__namespaced_org(self):
+        task = create_task(
+            SetOrgWideDefaults,
+            {
+                "managed": False,
+                "api_version": "47.0",
+                "api_names": "bar,foo",
+                "org_wide_defaults": [
+                    {
+                        "api_name": "Account",
+                        "internal_sharing_model": "Private",
+                        "external_sharing_model": "Private",
+                    },
+                    {
+                        "api_name": "Test__c",
+                        "internal_sharing_model": "ReadWrite",
+                        "external_sharing_model": "Read",
+                    },
+                ],
+            },
+        )
+        task.org_config.namespaced = True
+        task.project_config.project__package__namespace = "test"
+        task.sf = mock.Mock()
+        task.sf.query.side_effect = [
+            {
+                "totalSize": 1,
+                "records": [
+                    {"ExternalSharingModel": "Read", "InternalSharingModel": "Read"}
+                ],
+            },
+            {
+                "totalSize": 1,
+                "records": [
+                    {
+                        "ExternalSharingModel": "Private",
+                        "InternalSharingModel": "Private",
+                    }
+                ],
+            },
+            {
+                "totalSize": 1,
+                "records": [
+                    {
+                        "ExternalSharingModel": "Read",
+                        "InternalSharingModel": "ReadWrite",
+                    }
+                ],
+            },
+        ]
+        task._post_deploy("Success")
+
+        query = (
+            "SELECT ExternalSharingModel, InternalSharingModel "
+            "FROM EntityDefinition "
+            "WHERE QualifiedApiName = '{}'"
+        )
+
+        task.sf.query.assert_has_calls(
+            [
+                mock.call(query.format("Account")),
+                mock.call(query.format("Account")),
+                mock.call(query.format("test__Test__c")),
+            ]
+        )
+
+        assert task.poll_complete
+
     def test_post_deploy_exception_not_found(self):
         task = create_task(
             SetOrgWideDefaults,
             {
                 "managed": True,
                 "api_version": "47.0",
                 "api_names": "bar,foo",
```

### Comparing `cumulusci-3.9.0/cumulusci/tasks/metadata_etl/tests/test_value_sets.py` & `cumulusci-3.9.1/cumulusci/tasks/metadata_etl/tests/test_value_sets.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/metadata_etl/value_sets.py` & `cumulusci-3.9.1/cumulusci/tasks/metadata_etl/value_sets.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/metadeploy.py` & `cumulusci-3.9.1/cumulusci/tasks/metadeploy.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/metaxml.py` & `cumulusci-3.9.1/cumulusci/tasks/metaxml.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/push/README.md` & `cumulusci-3.9.1/cumulusci/tasks/push/README.md`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/push/push_api.py` & `cumulusci-3.9.1/cumulusci/tasks/push/push_api.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/push/pushfails.py` & `cumulusci-3.9.1/cumulusci/tasks/push/pushfails.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/push/tasks.py` & `cumulusci-3.9.1/cumulusci/tasks/push/tasks.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/push/tests/test_push_api.py` & `cumulusci-3.9.1/cumulusci/tasks/push/tests/test_push_api.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/release_notes/README.md` & `cumulusci-3.9.1/cumulusci/tasks/release_notes/README.md`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/release_notes/generator.py` & `cumulusci-3.9.1/cumulusci/tasks/release_notes/generator.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/release_notes/parser.py` & `cumulusci-3.9.1/cumulusci/tasks/release_notes/parser.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/release_notes/provider.py` & `cumulusci-3.9.1/cumulusci/tasks/release_notes/provider.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/release_notes/task.py` & `cumulusci-3.9.1/cumulusci/tasks/release_notes/task.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/release_notes/tests/test_generator.py` & `cumulusci-3.9.1/cumulusci/tasks/release_notes/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/release_notes/tests/test_parser.py` & `cumulusci-3.9.1/cumulusci/tasks/release_notes/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/release_notes/tests/test_provider.py` & `cumulusci-3.9.1/cumulusci/tasks/release_notes/tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/release_notes/tests/test_task.py` & `cumulusci-3.9.1/cumulusci/tasks/release_notes/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/release_notes/tests/utils.py` & `cumulusci-3.9.1/cumulusci/tasks/release_notes/tests/utils.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/robotframework/debugger/DebugListener.py` & `cumulusci-3.9.1/cumulusci/tasks/robotframework/debugger/DebugListener.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/robotframework/debugger/model.py` & `cumulusci-3.9.1/cumulusci/tasks/robotframework/debugger/model.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/robotframework/debugger/ui.py` & `cumulusci-3.9.1/cumulusci/tasks/robotframework/debugger/ui.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/robotframework/libdoc.py` & `cumulusci-3.9.1/cumulusci/tasks/robotframework/libdoc.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/robotframework/lint.py` & `cumulusci-3.9.1/cumulusci/tasks/robotframework/lint.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/robotframework/robotframework.py` & `cumulusci-3.9.1/cumulusci/tasks/robotframework/robotframework.py`

 * *Files 10% similar despite different names*

```diff
@@ -80,16 +80,31 @@
                 options[option] = self.options[option]
         options["variable"] = self.options.get("vars") or []
         options["outputdir"] = os.path.relpath(
             os.path.join(self.working_path, options.get("outputdir", ".")), os.getcwd()
         )
 
         num_failed = robot_run(self.options["suites"], **options)
-        if num_failed:
-            raise RobotTestFailure("{} tests failed".format(num_failed))
+
+        # These numbers are from the robot framework user guide:
+        # http://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#return-codes
+        if 0 < num_failed < 250:
+            raise RobotTestFailure(
+                f"{num_failed} test{'' if num_failed == 1 else 's'} failed."
+            )
+        elif num_failed == 250:
+            raise RobotTestFailure("250 or more tests failed.")
+        elif num_failed == 251:
+            raise RobotTestFailure("Help or version information printed.")
+        elif num_failed == 252:
+            raise RobotTestFailure("Invalid test data or command line options.")
+        elif num_failed == 253:
+            raise RobotTestFailure("Test execution stopped by user.")
+        elif num_failed >= 255:
+            raise RobotTestFailure("Unexpected internal error")
 
 
 class RobotTestDoc(BaseTask):
     task_options = {
         "path": {
             "description": "The path containing .robot test files",
             "required": True,
```

### Comparing `cumulusci-3.9.0/cumulusci/tasks/robotframework/stylesheet.css` & `cumulusci-3.9.1/cumulusci/tasks/robotframework/stylesheet.css`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/robotframework/template.html` & `cumulusci-3.9.1/cumulusci/tasks/robotframework/template.html`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/robotframework/tests/TestLibrary.py` & `cumulusci-3.9.1/cumulusci/tasks/robotframework/tests/TestLibrary.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/robotframework/tests/TestPageObjects.py` & `cumulusci-3.9.1/cumulusci/tasks/robotframework/tests/TestPageObjects.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/robotframework/tests/test_debugger.py` & `cumulusci-3.9.1/cumulusci/tasks/robotframework/tests/test_debugger.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/robotframework/tests/test_robot_lint.py` & `cumulusci-3.9.1/cumulusci/tasks/robotframework/tests/test_robot_lint.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/robotframework/tests/test_robotframework.py` & `cumulusci-3.9.1/cumulusci/tasks/robotframework/tests/test_robotframework.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,20 +19,39 @@
 from cumulusci.utils import touch
 
 from cumulusci.tasks.robotframework.libdoc import KeywordFile
 
 
 class TestRobot(unittest.TestCase):
     @mock.patch("cumulusci.tasks.robotframework.robotframework.robot_run")
-    def test_run_task(self, robot_run):
+    def test_run_task_with_failure(self, robot_run):
         robot_run.return_value = 1
         task = create_task(Robot, {"suites": "tests", "pdb": True})
         with self.assertRaises(RobotTestFailure):
             task()
 
+    @mock.patch("cumulusci.tasks.robotframework.robotframework.robot_run")
+    def test_run_task_error_message(self, robot_run):
+        expected = {
+            1: "1 test failed.",  # singular; pet peeve of my to see "1 tests"
+            2: "2 tests failed.",  # plural
+            249: "249 tests failed.",
+            250: "250 or more tests failed.",
+            251: "Help or version information printed.",
+            252: "Invalid test data or command line options.",
+            253: "Test execution stopped by user.",
+            255: "Unexpected internal error",
+        }
+        for error_code in expected.keys():
+            robot_run.return_value = error_code
+            task = create_task(Robot, {"suites": "tests", "pdb": True})
+            with self.assertRaises(RobotTestFailure) as error:
+                task()
+            self.assertEqual(str(error.exception), expected[error_code])
+
     @mock.patch("cumulusci.tasks.robotframework.robotframework.patch_statusreporter")
     def test_pdb_arg(self, patch_statusreporter):
         create_task(
             Robot,
             {
                 "suites": "test",  # required, or the task will raise an exception
                 "pdb": "False",
```

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/BaseRetrieveMetadata.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/BaseRetrieveMetadata.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/BaseSalesforceApiTask.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/BaseSalesforceApiTask.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/BaseUninstallMetadata.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/BaseUninstallMetadata.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/CreateCommunity.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/CreateCommunity.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/CreatePackage.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/CreatePackage.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/Deploy.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/Deploy.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/DeployBundles.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/DeployBundles.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/EnsureRecordTypes.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/EnsureRecordTypes.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/InstallPackageVersion.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/InstallPackageVersion.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/ListCommunities.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/ListCommunities.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/ListCommunityTemplates.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/ListCommunityTemplates.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/PublishCommunity.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/PublishCommunity.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/RetrievePackaged.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/RetrievePackaged.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/RetrieveReportsAndDashboards.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/RetrieveReportsAndDashboards.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/RetrieveUnpackaged.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/RetrieveUnpackaged.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/SOQLQuery.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/SOQLQuery.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/UninstallLocalBundles.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/UninstallLocalBundles.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/UninstallLocalNamespacedBundles.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/UninstallLocalNamespacedBundles.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/UninstallPackage.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/UninstallPackage.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/UninstallPackaged.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/UninstallPackaged.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/UninstallPackagedIncremental.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/UninstallPackagedIncremental.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/UpdateDependencies.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/UpdateDependencies.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/__init__.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/__init__.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/activate_flow.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/activate_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Activate the Flows with the supplied Developer Names
     """
 
     task_options = {
         "developer_names": {
             "description": "List of DeveloperNames to query in SOQL",
             "required": True,
-        },
+        }
     }
 
     def _init_options(self, kwargs):
         super(ActivateFlow, self)._init_options(kwargs)
         self.options["developer_names"] = process_list_arg(
             self.options.get("developer_names")
         )
@@ -50,10 +50,10 @@
             response = self.tooling._call_salesforce("PATCH", urlpath, json=data)
             self.logger.info(response)
         excluded = []
         for i in self.options["developer_names"]:
             if i not in results:
                 excluded.append(i)
         if len(excluded) > 0:
-            self.logger.warn(
+            self.logger.warning(
                 f"The following developer names were not found: {excluded}"
             )
```

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/custom_settings.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/custom_settings.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/insert_record.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/insert_record.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/org_settings.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/org_settings.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/package_upload.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/package_upload.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/sourcetracking.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/sourcetracking.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_CreateCommunity.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_CreateCommunity.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_CreatePackage.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_CreatePackage.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_Deploy.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_Deploy.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_DeployBundles.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_DeployBundles.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_EnsureRecordTypes.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_EnsureRecordTypes.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_InstallPackageVersion.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_InstallPackageVersion.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_ListCommunities.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_ListCommunities.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_ListCommunityTemplates.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_ListCommunityTemplates.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_PackageUpload.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_PackageUpload.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_ProfileGrantAllAccess.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_ProfileGrantAllAccess.py`

 * *Files 3% similar despite different names*

```diff
@@ -238,14 +238,34 @@
     types = package_xml.find("types", name="Profile")
     assert {elem.text for elem in types.findall("members")} == {
         "Admin",
         "ns__Continuous Integration",
     }
 
 
+def test_expand_profile_members__namespaced_org():
+    task = create_task(
+        ProfileGrantAllAccess,
+        {
+            "api_names": ["Admin", "%%%NAMESPACE%%%Continuous Integration"],
+            "namespace_inject": "ns",
+            "namespaced_org": True,
+        },
+    )
+    package_xml = metadata_tree.fromstring(PACKAGE_XML_BEFORE)
+
+    task._expand_profile_members(package_xml)
+
+    types = package_xml.find("types", name="Profile")
+    assert {elem.text for elem in types.findall("members")} == {
+        "Admin",
+        "Continuous Integration",
+    }
+
+
 def test_expand_profile_members__broken_package():
     task = create_task(ProfileGrantAllAccess, {"api_names": ["Admin"]})
     task.tooling = mock.Mock()
     task.tooling.query.return_value = {
         "totalSize": 2,
         "records": [
             {"DeveloperName": "Test", "NamespacePrefix": "ns"},
```

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_PublishCommunity.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_PublishCommunity.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_RetrievePackaged.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_RetrievePackaged.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_RetrieveReportsAndDashboards.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_RetrieveReportsAndDashboards.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_RetrieveUnpackaged.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_RetrieveUnpackaged.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_SOQLQuery.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_SOQLQuery.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_UninstallLocal.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_UninstallLocal.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_UninstallLocalBundles.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_UninstallLocalBundles.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_UninstallLocalNamespacedBundles.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_UninstallLocalNamespacedBundles.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_UninstallPackage.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_UninstallPackage.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_UninstallPackaged.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_UninstallPackaged.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_UninstallPackagedIncremental.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_UninstallPackagedIncremental.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_UpdateDependencies.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_UpdateDependencies.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_activate_flow.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_activate_flow.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_base_tasks.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_base_tasks.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_custom_settings.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_custom_settings.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_insert_record.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_insert_record.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_org_settings.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_org_settings.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_sourcetracking.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_sourcetracking.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/test_trigger_handlers.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/test_trigger_handlers.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/tests/util.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/tests/util.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/trigger_handlers.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/trigger_handlers.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/salesforce/update_profile.py` & `cumulusci-3.9.1/cumulusci/tasks/salesforce/update_profile.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 from cumulusci.tasks.metadata_etl import (
     MetadataOperation,
     MetadataSingleEntityTransformTask,
 )
 
 from cumulusci.core.exceptions import TaskOptionsError, CumulusCIException
 from cumulusci.core.utils import process_bool_arg, process_list_arg
+from cumulusci.tasks.salesforce import BaseSalesforceApiTask
 from cumulusci.utils import CUMULUSCI_PATH
 from cumulusci.utils.xml import metadata_tree
 
 
-class ProfileGrantAllAccess(MetadataSingleEntityTransformTask):
+class ProfileGrantAllAccess(MetadataSingleEntityTransformTask, BaseSalesforceApiTask):
     name = "ProfileGrantAllAccess"
     entity = "Profile"
 
     task_options = {
         "package_xml": {
             "description": "Override the default package.xml file for retrieving the Admin.profile and all objects and classes "
             "that need to be included by providing a path to your custom package.xml"
@@ -112,15 +113,24 @@
         else:
             if "profile_name" in self.options:
                 self.api_names.add(self.options["profile_name"])
 
             if not self.api_names:
                 self.api_names.add("Admin")
 
+            if self.options["namespaced_org"]:
+                # Namespaced orgs don't use the explicit namespace references in `package.xml`.
+                # Preserving historic behavior but guarding here
+                self.options["managed"] = False
+
             self.api_names = {self._inject_namespace(x) for x in self.api_names}
+
+            if self.options["namespaced_org"]:
+                self.options["managed"] = True
+
             self.package_xml_path = os.path.join(
                 CUMULUSCI_PATH, "cumulusci", "files", "admin_profile.xml"
             )
 
     def freeze(self, step):
         # Preserve behavior from when we subclassed Deploy.
 
@@ -141,15 +151,20 @@
                 self.options["include_packaged_objects"]
                 or "package_xml" not in self.options
             ):
                 # We need to rewrite the package.xml for one or two reasons.
                 # Either we are using packaged-object expansion, or we're using
                 # the built-in admin_profile.xml and need to substitute in
                 # profile API names.
-                package_xml = metadata_tree.fromstring(package_xml_content)
+
+                # Convert to bytes because stored `package.xml`s typically have an encoding declaration,
+                # which `fromstring()` doesn't like.
+                package_xml = metadata_tree.fromstring(
+                    package_xml_content.encode("utf-8")
+                )
 
                 if self.options["include_packaged_objects"]:
                     self._expand_package_xml(package_xml)
                 if "package_xml" not in self.options:
                     self._expand_profile_members(package_xml)
 
                 package_xml_content = package_xml.tostring(xml_declaration=True)
```

### Comparing `cumulusci-3.9.0/cumulusci/tasks/sfdx.py` & `cumulusci-3.9.1/cumulusci/tasks/sfdx.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/tests/test_command.py` & `cumulusci-3.9.1/cumulusci/tasks/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/tests/test_connectedapp.py` & `cumulusci-3.9.1/cumulusci/tasks/tests/test_connectedapp.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/tests/test_datadictionary.py` & `cumulusci-3.9.1/cumulusci/tasks/tests/test_datadictionary.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/tests/test_metadeploy.py` & `cumulusci-3.9.1/cumulusci/tasks/tests/test_metadeploy.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/tests/test_metaxml.py` & `cumulusci-3.9.1/cumulusci/tasks/tests/test_metaxml.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/tests/test_pushfails.py` & `cumulusci-3.9.1/cumulusci/tasks/tests/test_pushfails.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/tests/test_salesforce.py` & `cumulusci-3.9.1/cumulusci/tasks/tests/test_salesforce.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/tests/test_sfdx.py` & `cumulusci-3.9.1/cumulusci/tasks/tests/test_sfdx.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/tests/test_util.py` & `cumulusci-3.9.1/cumulusci/tasks/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tasks/util.py` & `cumulusci-3.9.1/cumulusci/tasks/util.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tests/test_utils.py` & `cumulusci-3.9.1/cumulusci/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/tests/util.py` & `cumulusci-3.9.1/cumulusci/tests/util.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,50 +8,43 @@
 
 
 def random_sha():
     hash = random.getrandbits(128)
     return "%032x" % hash
 
 
-def create_project_config(repo_name="TestRepo", repo_owner="TestOwner"):
+def create_project_config(
+    repo_name="TestRepo", repo_owner="TestOwner", repo_commit=None
+):
     global_config = BaseGlobalConfig()
     project_config = DummyProjectConfig(
         global_config=global_config,
         repo_name=repo_name,
         repo_owner=repo_owner,
+        repo_commit=repo_commit,
         config=copy.deepcopy(global_config.config),
     )
     keychain = BaseProjectKeychain(project_config, None)
     project_config.set_keychain(keychain)
     return project_config
 
 
 class DummyProjectConfig(BaseProjectConfig):
     def __init__(
         self, global_config, repo_name, repo_owner, repo_commit=None, config=None
     ):
-        self._repo_name = repo_name
-        self._repo_owner = repo_owner
-        self._repo_commit = repo_commit
-        self._init_config = config
-        super(DummyProjectConfig, self).__init__(global_config, config)
-
-    @property
-    def repo_name(self):
-        return self._repo_name
-
-    @property
-    def repo_owner(self):
-        return self._repo_owner
-
-    @property
-    def repo_commit(self):
-        if not self._repo_commit:
-            self._repo_commit = random_sha()
-        return self._repo_commit
+        repo_info = {
+            "owner": repo_owner,
+            "name": repo_name,
+            "url": f"https://github.com/{repo_owner}/{repo_name}",
+            "commit": repo_commit or random_sha(),
+        }
+        super(DummyProjectConfig, self).__init__(
+            global_config, config, repo_info=repo_info
+        )
 
 
 class DummyOrgConfig(OrgConfig):
     def __init__(self, config=None, name=None):
         if not name:
             name = "test"
         super(DummyOrgConfig, self).__init__(config, name)
```

### Comparing `cumulusci-3.9.0/cumulusci/utils/__init__.py` & `cumulusci-3.9.1/cumulusci/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/utils/fileutils.py` & `cumulusci-3.9.1/cumulusci/utils/fileutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     ...     print(path)
     ...     print(file.read(10).strip())
     ...
     http://www.salesforce.com
     <!DOCTYPE
 
     >>> from urllib.request import urlopen
-    >>> with urlopen("http://www.salesforce.com") as f:
+    >>> with urlopen("https://www.salesforce.com") as f:
     ...     with load_from_source(f) as (path, file):
     ...         print(path)
     ...         print(file.read(10).strip())  #doctest: +ELLIPSIS
     ...
     https://www.salesforce.com/...
     <!DOCTYPE...
```

### Comparing `cumulusci-3.9.0/cumulusci/utils/tests/test_fileutils.py` & `cumulusci-3.9.1/cumulusci/utils/tests/test_fileutils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 import doctest
 from io import BytesIO, UnsupportedOperation
 from pathlib import Path
+from unittest import mock
 
 import pytest
 import responses
 
 from cumulusci.utils import fileutils, temporary_dir
 from cumulusci.utils.fileutils import load_from_source
 
 
 class TestFileutils:
     @responses.activate
-    def test_docstrings(self):
-        responses.add("GET", "http://www.salesforce.com", body="<!DOCTYPE HTML ...")
+    @mock.patch("urllib.request.urlopen")
+    def test_docstrings(self, urlopen):
+        pretend_html = b"<!DOCTYPE HTML ...blah blah blah"
+        responses.add("GET", "http://www.salesforce.com/", body=pretend_html)
+        fake_http_stream = BytesIO(pretend_html)
+        fake_http_stream.url = "https://www.salesforce.com/"
+        urlopen.return_value = fake_http_stream
         try:
             doctest.testmod(fileutils, raise_on_error=True, verbose=True)
         except doctest.DocTestFailure as e:
             print("Got")
             print(str(e.got))
             raise
```

### Comparing `cumulusci-3.9.0/cumulusci/utils/xml/metadata_tree.py` & `cumulusci-3.9.1/cumulusci/utils/xml/metadata_tree.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/utils/xml/salesforce_encoding.py` & `cumulusci-3.9.1/cumulusci/utils/xml/salesforce_encoding.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/utils/xml/test/test_metadata_tree.py` & `cumulusci-3.9.1/cumulusci/utils/xml/test/test_metadata_tree.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/utils/xml/test/test_salesforce_encoding.py` & `cumulusci-3.9.1/cumulusci/utils/xml/test/test_salesforce_encoding.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/utils/yaml/cumulusci_yml.py` & `cumulusci-3.9.1/cumulusci/utils/yaml/cumulusci_yml.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         rc = string.replace(NBSP, " ")
         return rc
 
     data = pattern.sub(_replacer_func, origdata)
 
     if counter:
         plural = "s were" if counter > 1 else " was"
-        logger.warn(
+        logger.warning(
             f"Note: {counter} lines with non-breaking space character{plural} detected in cumulusci.yml.\n"
             "Perhaps you cut and pasted from a Web page?\n"
             "Future versions of CumulusCI may disallow these characters.\n"
         )
     return data
```

### Comparing `cumulusci-3.9.0/cumulusci/utils/yaml/model_parser.py` & `cumulusci-3.9.1/cumulusci/utils/yaml/model_parser.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/utils/yaml/tests/test_cumulusci_yml.py` & `cumulusci-3.9.1/cumulusci/utils/yaml/tests/test_cumulusci_yml.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci/utils/yaml/tests/test_model_parser.py` & `cumulusci-3.9.1/cumulusci/utils/yaml/tests/test_model_parser.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci.egg-info/PKG-INFO` & `cumulusci-3.9.1/cumulusci.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cumulusci
-Version: 3.9.0
+Version: 3.9.1
 Summary: Build and release tools for Salesforce developers
 Home-page: https://github.com/SFDO-Tooling/CumulusCI
 Author: Salesforce.org
 Author-email: jlantz@salesforce.com
 License: BSD license
 Description: ===============================
         CumulusCI
@@ -44,14 +44,34 @@
         The master branch now contains CumulusCI 2 which is not backwards compatible with the previous CumulusCI that was based on Ant. If you are using the Ant targets, please switch to using the `legacy-1.0` branch of the repository which contains the Ant based version. Or, consider upgrading to CumulusCI 2.
         
         
         =======
         History
         =======
         
+        3.9.1 (2020-03-25)
+        ------------------
+        
+        Issues closed:
+        
+        * The ``batch_apex_wait`` task will now detect aborted and failed jobs instead of waiting indefinitely.
+        
+        * Fixed reporting of errors from Robot Framework when it exits with a return code > 250.
+        
+        * Fixed an ImportError that could happen when importing the new metadata ETL tasks.
+        
+        * Fixed bugs in how the ``set_organization_wide_defaults`` and ``update_admin_profile`` tasks operated in namespaced scratch orgs.
+        
+        * Show a more helpful error message if CumulusCI can't find a project's repository or release on GitHub. (#1281)
+        
+        * Fixed the message shown for skipped steps in ``cci flow info``.
+        
+        * Fixed a regression which accidentally removed support for the ``bulk_mode`` option in bulk data mappings.
+        
+        
         3.9.0 (2020-03-16)
         ------------------
         
         Critical changes:
         
         * The ``update_admin_profile`` task can now add field-level permissions for all packaged objects.
           This behavior is the default for projects with ``minimum_cumulusci_version`` >= 3.9.0 that are
```

### Comparing `cumulusci-3.9.0/cumulusci.egg-info/SOURCES.txt` & `cumulusci-3.9.1/cumulusci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/cumulusci.egg-info/requires.txt` & `cumulusci-3.9.1/requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 asn1crypto==1.3.0
 certifi==2019.11.28
 cffi==1.14.0
 chardet==3.0.4
 click==7.1.1
-coloredlogs==14.0
+coloredlogs==14.0   
 cryptography==2.8
 docutils==0.16
 github3.py==1.3.0
 humanfriendly==8.1
 jinja2==2.11.1
 jwcrypto==0.7
 keyring==21.2.0
 lxml==4.5.0
 MarkupSafe==1.1.1
 pycparser==2.20
 pydantic==1.4
 PyJWT==1.7.1
 python-dateutil==2.8.1
 pytz==2019.3
-PyYAML==5.3
+PyYAML==5.3.1
 raven==6.10.0
-requests[security]==2.23.0
+requests==2.23.0
 robotframework==3.1.2
 robotframework-seleniumlibrary==4.3.0
 rst2ansi==0.1.5
 salesforce-bulk==2.1.0
 sarge==0.1.5.post0
 selenium==3.141.0
-simple-salesforce==0.75.3
+simple-salesforce==1.0.0
 six==1.14.0
 SQLAlchemy==1.3.15
 terminaltables==3.1.0
+typing-extensions==3.7.4.1
 unicodecsv==0.14.1
 uritemplate==3.0.1
 urllib3==1.25.8
 xmltodict==0.12.0
 robotframework-lint==1.0
 factory-boy==2.12.0
```

### Comparing `cumulusci-3.9.0/docs/Makefile` & `cumulusci-3.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/docs/bulk_data.rst` & `cumulusci-3.9.1/docs/bulk_data.rst`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/docs/conf.py` & `cumulusci-3.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/docs/cookbook.rst` & `cumulusci-3.9.1/docs/cookbook.rst`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/docs/cumulus_ci_workflow.png` & `cumulusci-3.9.1/docs/cumulus_ci_workflow.png`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/docs/cumulusci_flow.rst` & `cumulusci-3.9.1/docs/cumulusci_flow.rst`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/docs/diagram/img/image1.png` & `cumulusci-3.9.1/docs/diagram/img/image1.png`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/docs/diagram/img/image12.png` & `cumulusci-3.9.1/docs/diagram/img/image12.png`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/docs/diagram/img/image15.png` & `cumulusci-3.9.1/docs/diagram/img/image15.png`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/docs/diagram/img/image17.png` & `cumulusci-3.9.1/docs/diagram/img/image17.png`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/docs/diagram/img/image3.png` & `cumulusci-3.9.1/docs/diagram/img/image3.png`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/docs/features.rst` & `cumulusci-3.9.1/docs/features.rst`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/docs/github-commit_status_error.png` & `cumulusci-3.9.1/docs/github-commit_status_error.png`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/docs/github-commit_status_pass.png` & `cumulusci-3.9.1/docs/github-commit_status_pass.png`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/docs/github-creating_a_uat_release.png` & `cumulusci-3.9.1/docs/github-creating_a_uat_release.png`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/docs/images/env-var.png` & `cumulusci-3.9.1/docs/images/env-var.png`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/docs/images/locate_elements_screenshot.png` & `cumulusci-3.9.1/docs/images/locate_elements_screenshot.png`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/docs/images/pipx.png` & `cumulusci-3.9.1/docs/images/pipx.png`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/docs/images/salesforce-org-process.png` & `cumulusci-3.9.1/docs/images/salesforce-org-process.png`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/docs/images/windows_python.png` & `cumulusci-3.9.1/docs/images/windows_python.png`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/docs/index.rst` & `cumulusci-3.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/docs/install.rst` & `cumulusci-3.9.1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/docs/make.bat` & `cumulusci-3.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/docs/robotframework-debugger.rst` & `cumulusci-3.9.1/docs/robotframework-debugger.rst`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/docs/robotframework-tutorial.rst` & `cumulusci-3.9.1/docs/robotframework-tutorial.rst`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/docs/robotframework.rst` & `cumulusci-3.9.1/docs/robotframework.rst`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/docs/tasks.rst` & `cumulusci-3.9.1/docs/tasks.rst`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/docs/tutorial.rst` & `cumulusci-3.9.1/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/docs/usage.rst` & `cumulusci-3.9.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/docs/why_cumulusci.rst` & `cumulusci-3.9.1/docs/why_cumulusci.rst`

 * *Files identical despite different names*

### Comparing `cumulusci-3.9.0/requirements.txt` & `cumulusci-3.9.1/cumulusci.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 asn1crypto==1.3.0
 certifi==2019.11.28
 cffi==1.14.0
 chardet==3.0.4
 click==7.1.1
-coloredlogs==14.0   
+coloredlogs==14.0
 cryptography==2.8
 docutils==0.16
 github3.py==1.3.0
 humanfriendly==8.1
 jinja2==2.11.1
 jwcrypto==0.7
 keyring==21.2.0
 lxml==4.5.0
 MarkupSafe==1.1.1
 pycparser==2.20
 pydantic==1.4
 PyJWT==1.7.1
 python-dateutil==2.8.1
 pytz==2019.3
-PyYAML==5.3
+PyYAML==5.3.1
 raven==6.10.0
-requests[security]==2.23.0
+requests==2.23.0
 robotframework==3.1.2
 robotframework-seleniumlibrary==4.3.0
 rst2ansi==0.1.5
 salesforce-bulk==2.1.0
 sarge==0.1.5.post0
 selenium==3.141.0
-simple-salesforce==0.75.3
+simple-salesforce==1.0.0
 six==1.14.0
 SQLAlchemy==1.3.15
 terminaltables==3.1.0
+typing-extensions==3.7.4.1
 unicodecsv==0.14.1
 uritemplate==3.0.1
 urllib3==1.25.8
 xmltodict==0.12.0
 robotframework-lint==1.0
 factory-boy==2.12.0
```

### Comparing `cumulusci-3.9.0/setup.py` & `cumulusci-3.9.1/setup.py`

 * *Files identical despite different names*

