# Comparing `tmp/plone.app.contentrules-5.0.1.tar.gz` & `tmp/plone.app.contentrules-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.contentrules-5.0.1.tar", last modified: Thu Apr  6 10:30:51 2023, max compression
+gzip compressed data, was "plone.app.contentrules-5.0.2.tar", last modified: Sat Apr 15 08:06:07 2023, max compression
```

## Comparing `plone.app.contentrules-5.0.1.tar` & `plone.app.contentrules-5.0.2.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:30:51.045786 plone.app.contentrules-5.0.1/
--rw-r--r--   0 maurits    (501) staff       (20)    20132 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      148 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    21633 2023-04-06 10:30:51.045964 plone.app.contentrules-5.0.1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      527 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:30:51.016489 plone.app.contentrules-5.0.1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      684 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:30:51.016800 plone.app.contentrules-5.0.1/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:30:51.019476 plone.app.contentrules-5.0.1/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:30:51.021894 plone.app.contentrules-5.0.1/plone/app/contentrules/
--rw-r--r--   0 maurits    (501) staff       (20)      162 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:30:51.024976 plone.app.contentrules-5.0.1/plone/app/contentrules/actions/
--rw-r--r--   0 maurits    (501) staff       (20)     1923 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/actions/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     6880 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/actions/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4835 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/actions/copy.py
--rw-r--r--   0 maurits    (501) staff       (20)     2197 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/actions/delete.py
--rw-r--r--   0 maurits    (501) staff       (20)     4143 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/actions/logger.py
--rw-r--r--   0 maurits    (501) staff       (20)     7188 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/actions/mail.py
--rw-r--r--   0 maurits    (501) staff       (20)     5694 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/actions/move.py
--rw-r--r--   0 maurits    (501) staff       (20)     2887 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/actions/notify.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:30:51.025279 plone.app.contentrules-5.0.1/plone/app/contentrules/actions/templates/
--rw-r--r--   0 maurits    (501) staff       (20)     1172 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/actions/templates/mail.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2850 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/actions/versioning.py
--rw-r--r--   0 maurits    (501) staff       (20)     3558 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/actions/workflow.py
--rw-r--r--   0 maurits    (501) staff       (20)     2391 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/api.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:30:51.028904 plone.app.contentrules-5.0.1/plone/app/contentrules/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        2 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3799 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/browser/adding.py
--rw-r--r--   0 maurits    (501) staff       (20)     7174 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/browser/assignments.py
--rw-r--r--   0 maurits    (501) staff       (20)     5827 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5294 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/browser/controlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)     8506 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/browser/elements.py
--rw-r--r--   0 maurits    (501) staff       (20)     5139 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/browser/formhelper.py
--rw-r--r--   0 maurits    (501) staff       (20)      842 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/browser/info.py
--rw-r--r--   0 maurits    (501) staff       (20)      990 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/browser/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      827 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/browser/navigation.py
--rw-r--r--   0 maurits    (501) staff       (20)     1895 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/browser/rule.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:30:51.030122 plone.app.contentrules-5.0.1/plone/app/contentrules/browser/templates/
--rw-r--r--   0 maurits    (501) staff       (20)      968 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/browser/templates/contentrules-pageform.pt
--rw-r--r--   0 maurits    (501) staff       (20)    14016 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/browser/templates/controlpanel.pt
--rw-r--r--   0 maurits    (501) staff       (20)    14486 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/browser/templates/manage-assignments.pt
--rw-r--r--   0 maurits    (501) staff       (20)    15756 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/browser/templates/manage-elements.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2166 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/browser/traversal.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:30:51.033037 plone.app.contentrules-5.0.1/plone/app/contentrules/conditions/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/conditions/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     7283 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/conditions/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3435 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/conditions/fileextension.py
--rw-r--r--   0 maurits    (501) staff       (20)     3313 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/conditions/group.py
--rw-r--r--   0 maurits    (501) staff       (20)     3773 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/conditions/portaltype.py
--rw-r--r--   0 maurits    (501) staff       (20)     3170 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/conditions/role.py
--rw-r--r--   0 maurits    (501) staff       (20)     3439 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/conditions/talesexpression.py
--rw-r--r--   0 maurits    (501) staff       (20)     3201 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/conditions/wfstate.py
--rw-r--r--   0 maurits    (501) staff       (20)     3148 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/conditions/wftransition.py
--rw-r--r--   0 maurits    (501) staff       (20)     5009 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:30:51.034212 plone.app.contentrules-5.0.1/plone/app/contentrules/exportimport/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/exportimport/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      891 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/exportimport/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      745 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/exportimport/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)    13594 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/exportimport/rules.py
--rw-r--r--   0 maurits    (501) staff       (20)     6057 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/handlers.py
--rw-r--r--   0 maurits    (501) staff       (20)      704 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/namechooser.py
--rw-r--r--   0 maurits    (501) staff       (20)     3137 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/rule.py
--rw-r--r--   0 maurits    (501) staff       (20)      962 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:30:51.044383 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     4025 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/assignment.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1403 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/base.py
--rw-r--r--   0 maurits    (501) staff       (20)      761 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/dummy.py
--rw-r--r--   0 maurits    (501) staff       (20)     4021 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/multipublish.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:30:51.013674 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:30:51.045495 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/profiles/testing/
--rw-r--r--   0 maurits    (501) staff       (20)     3556 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/profiles/testing/contentrules.xml
--rw-r--r--   0 maurits    (501) staff       (20)      264 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/profiles/testing/export_steps.xml
--rw-r--r--   0 maurits    (501) staff       (20)      346 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/profiles/testing/import_steps.xml
--rw-r--r--   0 maurits    (501) staff       (20)     3447 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/simplepublish.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4683 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_action_copy.py
--rw-r--r--   0 maurits    (501) staff       (20)     1821 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_action_delete.py
--rw-r--r--   0 maurits    (501) staff       (20)     3481 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_action_logger.py
--rw-r--r--   0 maurits    (501) staff       (20)     9521 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_action_mail.py
--rw-r--r--   0 maurits    (501) staff       (20)     1079 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_action_modify.py
--rw-r--r--   0 maurits    (501) staff       (20)     5419 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_action_move.py
--rw-r--r--   0 maurits    (501) staff       (20)     2686 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_action_notify.py
--rw-r--r--   0 maurits    (501) staff       (20)     2757 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_action_versioning.py
--rw-r--r--   0 maurits    (501) staff       (20)     3068 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_action_workflow.py
--rw-r--r--   0 maurits    (501) staff       (20)      663 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_browser.py
--rw-r--r--   0 maurits    (501) staff       (20)     1653 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_cascading_rule.py
--rw-r--r--   0 maurits    (501) staff       (20)     2588 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_condition_group.py
--rw-r--r--   0 maurits    (501) staff       (20)     2809 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_condition_portal_type.py
--rw-r--r--   0 maurits    (501) staff       (20)     2479 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_condition_role.py
--rw-r--r--   0 maurits    (501) staff       (20)     3086 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_condition_tales_expression.py
--rw-r--r--   0 maurits    (501) staff       (20)     2749 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_condition_wfstate.py
--rw-r--r--   0 maurits    (501) staff       (20)     3441 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_condition_wftransition.py
--rw-r--r--   0 maurits    (501) staff       (20)     8131 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_configuration.py
--rw-r--r--   0 maurits    (501) staff       (20)      288 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_events.py
--rw-r--r--   0 maurits    (501) staff       (20)     1652 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_handlers.py
--rw-r--r--   0 maurits    (501) staff       (20)     5713 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_rule_assignment_mapping.py
--rw-r--r--   0 maurits    (501) staff       (20)     6123 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_rule_management_views.py
--rw-r--r--   0 maurits    (501) staff       (20)      857 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_setup.py
--rw-r--r--   0 maurits    (501) staff       (20)     1926 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_traversal.py
--rw-r--r--   0 maurits    (501) staff       (20)     2743 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_ui.txt
--rw-r--r--   0 maurits    (501) staff       (20)      482 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/testing.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      155 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone/app/contentrules/tests/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-06 10:30:51.019145 plone.app.contentrules-5.0.1/plone.app.contentrules.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    21633 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone.app.contentrules.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     4398 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone.app.contentrules.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone.app.contentrules.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone.app.contentrules.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone.app.contentrules.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      485 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone.app.contentrules.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/plone.app.contentrules.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1643 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      217 2023-04-06 10:30:51.046532 plone.app.contentrules-5.0.1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2204 2023-04-06 10:30:50.000000 plone.app.contentrules-5.0.1/setup.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:06:07.052976 plone.app.contentrules-5.0.2/
+-rw-r--r--   0 gil       (1000) gil       (1000)    20241 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/CHANGES.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)       70 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 gil       (1000) gil       (1000)      148 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/MANIFEST.in
+-rw-r--r--   0 gil       (1000) gil       (1000)    21742 2023-04-15 08:06:07.053975 plone.app.contentrules-5.0.2/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)      527 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/README.rst
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:06:07.043975 plone.app.contentrules-5.0.2/docs/
+-rw-r--r--   0 gil       (1000) gil       (1000)    15220 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/docs/LICENSE.GPL
+-rw-r--r--   0 gil       (1000) gil       (1000)      684 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/docs/LICENSE.txt
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:06:07.043975 plone.app.contentrules-5.0.2/plone/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:06:07.044975 plone.app.contentrules-5.0.2/plone/app/
+-rw-r--r--   0 gil       (1000) gil       (1000)       56 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:06:07.044975 plone.app.contentrules-5.0.2/plone/app/contentrules/
+-rw-r--r--   0 gil       (1000) gil       (1000)      162 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/__init__.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:06:07.045975 plone.app.contentrules-5.0.2/plone/app/contentrules/actions/
+-rw-r--r--   0 gil       (1000) gil       (1000)     1923 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/actions/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6880 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/actions/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     4835 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/actions/copy.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2197 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/actions/delete.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     4143 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/actions/logger.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     7188 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/actions/mail.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     5694 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/actions/move.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2887 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/actions/notify.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:06:07.045975 plone.app.contentrules-5.0.2/plone/app/contentrules/actions/templates/
+-rw-r--r--   0 gil       (1000) gil       (1000)     1172 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/actions/templates/mail.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     2850 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/actions/versioning.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3558 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/actions/workflow.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2391 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/api.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:06:07.047975 plone.app.contentrules-5.0.2/plone/app/contentrules/browser/
+-rw-r--r--   0 gil       (1000) gil       (1000)        2 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/browser/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3799 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/browser/adding.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     7174 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/browser/assignments.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     5827 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/browser/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     5294 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/browser/controlpanel.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     8506 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/browser/elements.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     5139 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/browser/formhelper.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      842 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/browser/info.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      990 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/browser/interfaces.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      827 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/browser/navigation.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1895 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/browser/rule.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:06:07.047975 plone.app.contentrules-5.0.2/plone/app/contentrules/browser/templates/
+-rw-r--r--   0 gil       (1000) gil       (1000)      968 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/browser/templates/contentrules-pageform.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)    14016 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/browser/templates/controlpanel.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)    14486 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/browser/templates/manage-assignments.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)    15756 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/browser/templates/manage-elements.pt
+-rw-r--r--   0 gil       (1000) gil       (1000)     2166 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/browser/traversal.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:06:07.048975 plone.app.contentrules-5.0.2/plone/app/contentrules/conditions/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/conditions/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     7283 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/conditions/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)     3435 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/conditions/fileextension.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3313 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/conditions/group.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3773 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/conditions/portaltype.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3170 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/conditions/role.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3439 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/conditions/talesexpression.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3201 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/conditions/wfstate.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3148 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/conditions/wftransition.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     5009 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/configure.zcml
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:06:07.049975 plone.app.contentrules-5.0.2/plone/app/contentrules/exportimport/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/exportimport/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      891 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/exportimport/configure.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)      745 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/exportimport/interfaces.py
+-rw-r--r--   0 gil       (1000) gil       (1000)    13594 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/exportimport/rules.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6057 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/handlers.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      704 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/namechooser.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3137 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/rule.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      962 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/testing.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:06:07.052976 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/
+-rw-r--r--   0 gil       (1000) gil       (1000)        0 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/__init__.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     4025 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/assignment.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     1403 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/base.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      761 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/dummy.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     4021 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/multipublish.txt
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:06:07.042975 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/profiles/
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:06:07.052976 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/profiles/testing/
+-rw-r--r--   0 gil       (1000) gil       (1000)     3556 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/profiles/testing/contentrules.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)      264 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/profiles/testing/export_steps.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)      346 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/profiles/testing/import_steps.xml
+-rw-r--r--   0 gil       (1000) gil       (1000)     3447 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/simplepublish.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     4683 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_action_copy.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1821 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_action_delete.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3481 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_action_logger.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     9521 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_action_mail.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1079 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_action_modify.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     5419 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_action_move.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2686 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_action_notify.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2757 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_action_versioning.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3068 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_action_workflow.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      663 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_browser.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1653 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_cascading_rule.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2588 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_condition_group.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2809 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_condition_portal_type.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2479 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_condition_role.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3086 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_condition_tales_expression.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2749 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_condition_wfstate.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     3441 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_condition_wftransition.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     8131 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_configuration.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      288 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_events.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1652 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_handlers.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     5713 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_rule_assignment_mapping.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     6123 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_rule_management_views.py
+-rw-r--r--   0 gil       (1000) gil       (1000)      857 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_setup.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     1926 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_traversal.py
+-rw-r--r--   0 gil       (1000) gil       (1000)     2743 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_ui.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)      482 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/testing.zcml
+-rw-r--r--   0 gil       (1000) gil       (1000)      155 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone/app/contentrules/tests/utils.py
+drwxr-xr-x   0 gil       (1000) gil       (1000)        0 2023-04-15 08:06:07.043975 plone.app.contentrules-5.0.2/plone.app.contentrules.egg-info/
+-rw-r--r--   0 gil       (1000) gil       (1000)    21742 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone.app.contentrules.egg-info/PKG-INFO
+-rw-r--r--   0 gil       (1000) gil       (1000)     4398 2023-04-15 08:06:07.000000 plone.app.contentrules-5.0.2/plone.app.contentrules.egg-info/SOURCES.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone.app.contentrules.egg-info/dependency_links.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)       16 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone.app.contentrules.egg-info/namespace_packages.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        1 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone.app.contentrules.egg-info/not-zip-safe
+-rw-r--r--   0 gil       (1000) gil       (1000)      331 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone.app.contentrules.egg-info/requires.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)        6 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/plone.app.contentrules.egg-info/top_level.txt
+-rw-r--r--   0 gil       (1000) gil       (1000)     2782 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/pyproject.toml
+-rw-r--r--   0 gil       (1000) gil       (1000)      217 2023-04-15 08:06:07.053975 plone.app.contentrules-5.0.2/setup.cfg
+-rw-r--r--   0 gil       (1000) gil       (1000)     1938 2023-04-15 08:06:06.000000 plone.app.contentrules-5.0.2/setup.py
```

### Comparing `plone.app.contentrules-5.0.1/CHANGES.rst` & `plone.app.contentrules-5.0.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.2 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (0b0246aa)
+
+
 5.0.1 (2023-04-06)
 ------------------
 
 Bug fixes:
 
 
 - Explicitly mark exclude_actor as not-required
```

### Comparing `plone.app.contentrules-5.0.1/PKG-INFO` & `plone.app.contentrules-5.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.contentrules
-Version: 5.0.1
+Version: 5.0.2
 Summary: Plone integration for plone.contentrules
 Home-page: https://pypi.org/project/plone.app.contentrules
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone automatic content rules
 Classifier: Development Status :: 5 - Production/Stable
@@ -46,14 +46,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.2 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (0b0246aa)
+
+
 5.0.1 (2023-04-06)
 ------------------
 
 Bug fixes:
 
 
 - Explicitly mark exclude_actor as not-required
```

### Comparing `plone.app.contentrules-5.0.1/README.rst` & `plone.app.contentrules-5.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/docs/LICENSE.GPL` & `plone.app.contentrules-5.0.2/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/docs/LICENSE.txt` & `plone.app.contentrules-5.0.2/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/actions/__init__.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/actions/configure.zcml` & `plone.app.contentrules-5.0.2/plone/app/contentrules/actions/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/actions/copy.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/actions/copy.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/actions/delete.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/actions/delete.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/actions/logger.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/actions/logger.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/actions/mail.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/actions/mail.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/actions/move.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/actions/move.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/actions/notify.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/actions/notify.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/actions/templates/mail.pt` & `plone.app.contentrules-5.0.2/plone/app/contentrules/actions/templates/mail.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/actions/versioning.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/actions/versioning.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/actions/workflow.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/actions/workflow.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/api.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/api.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/browser/adding.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/browser/adding.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/browser/assignments.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/browser/assignments.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/browser/configure.zcml` & `plone.app.contentrules-5.0.2/plone/app/contentrules/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/browser/controlpanel.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/browser/elements.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/browser/elements.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/browser/formhelper.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/browser/formhelper.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/browser/info.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/browser/info.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/browser/interfaces.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/browser/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/browser/navigation.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/browser/navigation.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/browser/rule.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/browser/rule.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/browser/templates/contentrules-pageform.pt` & `plone.app.contentrules-5.0.2/plone/app/contentrules/browser/templates/contentrules-pageform.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/browser/templates/controlpanel.pt` & `plone.app.contentrules-5.0.2/plone/app/contentrules/browser/templates/controlpanel.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/browser/templates/manage-assignments.pt` & `plone.app.contentrules-5.0.2/plone/app/contentrules/browser/templates/manage-assignments.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/browser/templates/manage-elements.pt` & `plone.app.contentrules-5.0.2/plone/app/contentrules/browser/templates/manage-elements.pt`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/browser/traversal.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/browser/traversal.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/conditions/configure.zcml` & `plone.app.contentrules-5.0.2/plone/app/contentrules/conditions/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/conditions/fileextension.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/conditions/fileextension.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/conditions/group.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/conditions/group.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/conditions/portaltype.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/conditions/portaltype.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/conditions/role.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/conditions/role.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/conditions/talesexpression.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/conditions/talesexpression.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/conditions/wfstate.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/conditions/wfstate.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/conditions/wftransition.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/conditions/wftransition.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/configure.zcml` & `plone.app.contentrules-5.0.2/plone/app/contentrules/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/exportimport/configure.zcml` & `plone.app.contentrules-5.0.2/plone/app/contentrules/exportimport/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/exportimport/interfaces.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/exportimport/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/exportimport/rules.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/exportimport/rules.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/handlers.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/handlers.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/namechooser.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/namechooser.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/rule.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/rule.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/testing.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/assignment.txt` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/assignment.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/base.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/base.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/dummy.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/dummy.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/multipublish.txt` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/multipublish.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/profiles/testing/contentrules.xml` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/profiles/testing/contentrules.xml`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/simplepublish.txt` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/simplepublish.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_action_copy.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_action_copy.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_action_delete.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_action_delete.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_action_logger.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_action_logger.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_action_mail.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_action_mail.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_action_modify.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_action_modify.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_action_move.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_action_move.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_action_notify.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_action_notify.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_action_versioning.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_action_versioning.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_action_workflow.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_action_workflow.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_browser.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_browser.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_cascading_rule.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_cascading_rule.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_condition_group.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_condition_group.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_condition_portal_type.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_condition_portal_type.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_condition_role.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_condition_role.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_condition_tales_expression.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_condition_tales_expression.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_condition_wfstate.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_condition_wfstate.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_condition_wftransition.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_condition_wftransition.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_configuration.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_handlers.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_rule_assignment_mapping.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_rule_assignment_mapping.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_rule_management_views.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_rule_management_views.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_setup.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_traversal.py` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_traversal.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone/app/contentrules/tests/test_ui.txt` & `plone.app.contentrules-5.0.2/plone/app/contentrules/tests/test_ui.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/plone.app.contentrules.egg-info/PKG-INFO` & `plone.app.contentrules-5.0.2/plone.app.contentrules.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.contentrules
-Version: 5.0.1
+Version: 5.0.2
 Summary: Plone integration for plone.contentrules
 Home-page: https://pypi.org/project/plone.app.contentrules
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone automatic content rules
 Classifier: Development Status :: 5 - Production/Stable
@@ -46,14 +46,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+5.0.2 (2023-04-15)
+------------------
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (0b0246aa)
+
+
 5.0.1 (2023-04-06)
 ------------------
 
 Bug fixes:
 
 
 - Explicitly mark exclude_actor as not-required
```

### Comparing `plone.app.contentrules-5.0.1/plone.app.contentrules.egg-info/SOURCES.txt` & `plone.app.contentrules-5.0.2/plone.app.contentrules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contentrules-5.0.1/setup.py` & `plone.app.contentrules-5.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "5.0.1"
+version = "5.0.2"
 
 setup(
     name="plone.app.contentrules",
     version=version,
     description="Plone integration for plone.contentrules",
     long_description=(open("README.rst").read() + "\n\n" + open("CHANGES.rst").read()),
     classifiers=[
@@ -39,34 +39,24 @@
             "plone.app.testing",
             "plone.app.contenttypes[test]",
             "plone.dexterity",
             "plone.testing",
         ]
     },
     install_requires=[
-        "BTrees",
-        "Products.MailHost",
-        "Products.PluggableAuthService",
         "lxml",
         "plone.app.contenttypes",
-        "plone.app.discussion",
         "plone.app.uuid",
-        "plone.registry",
-        "plone.supermodel",
-        "plone.z3cform",
-        "z3c.form",
-        "setuptools",
+        "plone.app.vocabularies",
+        "plone.autoform",
         "plone.base",
         "plone.contentrules",
         "plone.memoize",
         "plone.stringinterp",
+        "plone.supermodel",
         "plone.uuid",
-        "plone.autoform",
-        "plone.app.vocabularies",
-        "zope.annotation",
-        "zope.browser",
-        "Products.CMFPlone",
-        "Products.GenericSetup >= 2.0",
+        "Products.PluggableAuthService",
         "Products.statusmessages",
-        "Zope",
+        "setuptools",
+        "z3c.form",
     ],
 )
```

