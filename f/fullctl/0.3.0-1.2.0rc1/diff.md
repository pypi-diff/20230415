# Comparing `tmp/fullctl-0.3.0.tar.gz` & `tmp/fullctl-1.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fullctl-0.3.0.tar", max compression
+gzip compressed data, was "fullctl-1.2.0rc1.tar", max compression
```

## Comparing `fullctl-0.3.0.tar` & `fullctl-1.2.0rc1.tar`

### file list

```diff
@@ -1,121 +1,291 @@
--rw-r--r--   0        0        0    11357 2021-03-23 11:15:22.694151 fullctl-0.3.0/LICENSE
--rw-r--r--   0        0        0     1430 2021-03-24 13:24:06.081757 fullctl-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-03-23 11:15:22.694151 fullctl-0.3.0/src/fullctl/__init__.py
--rwxr-xr-x   0        0        0        0 2021-03-23 11:15:22.694151 fullctl-0.3.0/src/fullctl/django/__init__.py
--rw-r--r--   0        0        0      613 2021-03-23 11:15:22.694151 fullctl-0.3.0/src/fullctl/django/admin.py
--rw-r--r--   0        0        0      205 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/apps.py
--rw-r--r--   0        0        0      980 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/auth.py
--rw-r--r--   0        0        0        0 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/autocomplete/__init__.py
--rw-r--r--   0        0        0     1332 2021-03-23 16:15:13.824761 fullctl-0.3.0/src/fullctl/django/autocomplete/views.py
--rw-r--r--   0        0        0     1293 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/context_processors.py
--rw-r--r--   0        0        0     1911 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/decorators.py
--rw-r--r--   0        0        0       57 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/enum.py
--rw-r--r--   0        0        0       79 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/forms.py
--rw-r--r--   0        0        0        0 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/inet/__init__.py
--rw-r--r--   0        0        0      325 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/inet/const.py
--rw-r--r--   0        0        0      186 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/inet/exceptions.py
--rw-r--r--   0        0        0      761 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/inet/fields.py
--rw-r--r--   0        0        0      290 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/inet/util.py
--rw-r--r--   0        0        0     3738 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/inet/validators.py
--rw-r--r--   0        0        0        0 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/management/__init__.py
--rw-r--r--   0        0        0        0 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/management/commands/__init__.py
--rw-r--r--   0        0        0     1195 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/management/commands/fullctl_peeringdb_sync.py
--rw-r--r--   0        0        0     1652 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/middleware.py
--rw-r--r--   0        0        0     8662 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/migrations/__init__.py
--rw-r--r--   0        0        0       73 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/models/__init__.py
--rw-r--r--   0        0        0       70 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/models/abstract/__init__.py
--rw-r--r--   0        0        0     3204 2021-03-23 16:15:13.824761 fullctl-0.3.0/src/fullctl/django/models/abstract/alert.py
--rw-r--r--   0        0        0     2211 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/models/abstract/base.py
--rw-r--r--   0        0        0     4674 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/models/abstract/task_interface.py
--rw-r--r--   0        0        0       73 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/models/concrete/__init__.py
--rw-r--r--   0        0        0     6723 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/models/concrete/account.py
--rw-r--r--   0        0        0        0 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/rest/__init__.py
--rw-r--r--   0        0        0     4027 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/rest/api_schema.py
--rw-r--r--   0        0        0      876 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/rest/authentication.py
--rw-r--r--   0        0        0     1831 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/rest/core.py
--rw-r--r--   0        0        0     5351 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/rest/decorators.py
--rw-r--r--   0        0        0     1220 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/rest/filters.py
--rw-r--r--   0        0        0      585 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/rest/mixins.py
--rw-r--r--   0        0        0     2162 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/rest/renderers.py
--rw-r--r--   0        0        0        0 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/rest/route/__init__.py
--rw-r--r--   0        0        0      279 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/rest/route/account.py
--rw-r--r--   0        0        0      344 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/rest/route/usage.py
--rw-r--r--   0        0        0     1441 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/rest/serializers/__init__.py
--rw-r--r--   0        0        0     1300 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/rest/serializers/account.py
--rw-r--r--   0        0        0      806 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/rest/serializers/org.py
--rw-r--r--   0        0        0      440 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/rest/serializers/usage.py
--rw-r--r--   0        0        0        0 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/rest/urls/__init__.py
--rw-r--r--   0        0        0      210 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/rest/urls/account.py
--rw-r--r--   0        0        0     1910 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/rest/urls/service_bridge.py
--rw-r--r--   0        0        0      204 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/rest/urls/usage.py
--rw-r--r--   0        0        0      419 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/rest/usage.py
--rw-r--r--   0        0        0        0 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/rest/views/__init__.py
--rw-r--r--   0        0        0     1305 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/rest/views/account.py
--rw-r--r--   0        0        0     1474 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/rest/views/usage.py
--rw-r--r--   0        0        0       96 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/signals.py
--rw-r--r--   0        0        0        0 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/social/__init__.py
--rw-r--r--   0        0        0        0 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/social/backends/__init__.py
--rw-r--r--   0        0        0     1206 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/social/backends/peeringdb.py
--rw-r--r--   0        0        0     1482 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/social/backends/twentyc.py
--rw-r--r--   0        0        0     1149 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/social/pipelines/__init__.py
--rw-r--r--   0        0        0     4237 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/static/common/20c/twentyc.core.min.js
--rw-r--r--   0        0        0    18751 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/static/common/20c/twentyc.rest.js
--rw-r--r--   0        0        0     9475 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/static/common/20c-logo-filled.svg
--rw-r--r--   0        0        0    13772 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/static/common/app.css
--rw-r--r--   0        0        0    11315 2021-03-23 11:15:22.697485 fullctl-0.3.0/src/fullctl/django/static/common/app.js
--rw-r--r--   0        0        0     3380 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/static/common/icons/Indicator/Check-Ind/Check.svg
--rw-r--r--   0        0        0     3657 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/static/common/icons/Indicator/X-Ind/X.svg
--rw-r--r--   0        0        0     3430 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/static/common/icons/icon/add.svg
--rw-r--r--   0        0        0     3819 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/static/common/icons/icon/alerts.svg
--rw-r--r--   0        0        0     1303 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/static/common/icons/icon/dark-mode.svg
--rw-r--r--   0        0        0     2681 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/static/common/icons/icon/delete.svg
--rw-r--r--   0        0        0     5490 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/static/common/icons/icon/edit.svg
--rw-r--r--   0        0        0     1601 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/static/common/icons/icon/light-mode.svg
--rw-r--r--   0        0        0     3357 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/static/common/icons/icon/list.svg
--rw-r--r--   0        0        0     2617 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/static/common/icons/icon/logout.svg
--rw-r--r--   0        0        0     2761 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/static/common/icons/icon/org.svg
--rw-r--r--   0        0        0     8263 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/static/common/icons/icon/settings.svg
--rw-r--r--   0        0        0     4138 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/static/common/icons/icon/user.svg
--rw-r--r--   0        0        0     3689 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/static/common/icons/ixctl-logo-darkbg.svg
--rw-r--r--   0        0        0      169 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/static/common/icons/md-add.svg
--rw-r--r--   0        0        0      275 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/static/common/icons/md-create.svg
--rw-r--r--   0        0        0      272 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/static/common/icons/md-list-box.svg
--rw-r--r--   0        0        0      240 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/static/common/icons/md-trash.svg
--rw-r--r--   0        0        0     5957 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/static/common/icons/prefixctl-logo-darkbg.svg
--rw-r--r--   0        0        0      954 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/static/common/icons/ui-caret-caret/down.svg
--rw-r--r--   0        0        0      818 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/static/common/icons/ui-close.svg
--rw-r--r--   0        0        0     9475 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/static/common/oauth/20c.svg
--rw-r--r--   0        0        0      689 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/static/common/oauth/google.svg
--rw-r--r--   0        0        0     9186 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/static/common/oauth/peeringdb.png
--rw-r--r--   0        0        0     4336 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/static/common/service_bridge.js
--rw-r--r--   0        0        0     5709 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/static/common/themes/dark.css
--rw-r--r--   0        0        0        0 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/static/common/themes/light.css
--rw-r--r--   0        0        0      740 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/tasks.py
--rw-r--r--   0        0        0      668 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/templates/common/apidocs/redoc.html
--rw-r--r--   0        0        0      866 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/templates/common/apidocs/swagger.html
--rw-r--r--   0        0        0     7102 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/templates/common/app/base.html
--rw-r--r--   0        0        0      211 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/templates/common/app/checkbox.html
--rw-r--r--   0        0        0     1935 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/templates/common/app/forms/alert-prefs.html
--rw-r--r--   0        0        0      726 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/templates/common/app/forms/import-org.html
--rw-r--r--   0        0        0      494 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/templates/common/app/forms/invite.html
--rw-r--r--   0        0        0      792 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/templates/common/app/forms/org-create.html
--rw-r--r--   0        0        0     3826 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/templates/common/app/forms/org-prefs.html
--rw-r--r--   0        0        0      355 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/templates/common/app/index.html
--rw-r--r--   0        0        0     1974 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/templates/common/app/manage/permissions.html
--rw-r--r--   0        0        0     3275 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/templates/common/app/modal.html
--rw-r--r--   0        0        0     2668 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/templates/common/app/navbar.html
--rw-r--r--   0        0        0      356 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/templates/common/app/templates.html
--rw-r--r--   0        0        0     3101 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/templates/common/auth/login.html
--rw-r--r--   0        0        0      880 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/templates/common/auth/oauth-badge.html
--rw-r--r--   0        0        0     1110 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/templates/common/auth/oauth.html
--rw-r--r--   0        0        0     2823 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/templates/common/base.html
--rw-r--r--   0        0        0      234 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/templates/common/tool_base.html
--rw-r--r--   0        0        0     1561 2021-03-24 13:23:32.498536 fullctl-0.3.0/src/fullctl/django/urls.py
--rw-r--r--   0        0        0      483 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/util.py
--rw-r--r--   0        0        0      878 2021-03-23 16:15:13.824761 fullctl-0.3.0/src/fullctl/django/validators.py
--rw-r--r--   0        0        0      263 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/django/views.py
--rw-r--r--   0        0        0        0 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/service_bridge/__init__.py
--rw-r--r--   0        0        0     1928 2021-03-23 11:15:22.700818 fullctl-0.3.0/src/fullctl/service_bridge/client.py
--rw-r--r--   0        0        0     2391 2021-03-24 13:24:07.131287 fullctl-0.3.0/setup.py
--rw-r--r--   0        0        0     1269 2021-03-24 13:24:07.131866 fullctl-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2021-04-22 13:27:52.952758 fullctl-1.2.0rc1/LICENSE
+-rw-r--r--   0        0        0     2197 2023-04-15 17:38:24.097273 fullctl-1.2.0rc1/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.953758 fullctl-1.2.0rc1/src/fullctl/__init__.py
+-rwxr-xr-x   0        0        0        0 2021-04-22 13:27:52.953758 fullctl-1.2.0rc1/src/fullctl/django/__init__.py
+-rw-r--r--   0        0        0     5587 2023-04-15 16:24:16.029446 fullctl-1.2.0rc1/src/fullctl/django/admin.py
+-rw-r--r--   0        0        0      259 2021-10-21 03:49:59.920722 fullctl-1.2.0rc1/src/fullctl/django/apps.py
+-rw-r--r--   0        0        0     7188 2023-02-27 05:27:02.246818 fullctl-1.2.0rc1/src/fullctl/django/auditlog.py
+-rw-r--r--   0        0        0     4863 2023-04-15 16:24:16.030446 fullctl-1.2.0rc1/src/fullctl/django/auth.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.954758 fullctl-1.2.0rc1/src/fullctl/django/autocomplete/__init__.py
+-rw-r--r--   0        0        0      954 2023-02-27 05:27:02.247818 fullctl-1.2.0rc1/src/fullctl/django/autocomplete/pdb.py
+-rw-r--r--   0        0        0     2518 2023-04-15 16:24:16.030446 fullctl-1.2.0rc1/src/fullctl/django/context.py
+-rw-r--r--   0        0        0     3402 2023-04-15 16:24:16.030446 fullctl-1.2.0rc1/src/fullctl/django/context_processors.py
+-rw-r--r--   0        0        0     3102 2023-04-15 17:32:55.630524 fullctl-1.2.0rc1/src/fullctl/django/decorators.py
+-rw-r--r--   0        0        0      233 2023-04-15 17:32:55.630524 fullctl-1.2.0rc1/src/fullctl/django/enum.py
+-rw-r--r--   0        0        0      283 2022-10-14 13:57:25.205745 fullctl-1.2.0rc1/src/fullctl/django/exceptions.py
+-rw-r--r--   0        0        0      650 2022-10-14 13:57:25.205745 fullctl-1.2.0rc1/src/fullctl/django/fields/__init__.py
+-rw-r--r--   0        0        0     4351 2023-02-27 05:27:02.248818 fullctl-1.2.0rc1/src/fullctl/django/fields/service_bridge/__init__.py
+-rw-r--r--   0        0        0      317 2023-02-27 05:27:02.248818 fullctl-1.2.0rc1/src/fullctl/django/fields/service_bridge/prefixctl.py
+-rw-r--r--   0        0        0       79 2021-06-15 13:03:05.246145 fullctl-1.2.0rc1/src/fullctl/django/forms.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.954758 fullctl-1.2.0rc1/src/fullctl/django/inet/__init__.py
+-rw-r--r--   0        0        0      325 2021-04-22 13:27:52.954758 fullctl-1.2.0rc1/src/fullctl/django/inet/const.py
+-rw-r--r--   0        0        0      186 2021-04-22 13:27:52.955758 fullctl-1.2.0rc1/src/fullctl/django/inet/exceptions.py
+-rw-r--r--   0        0        0      761 2021-06-15 13:03:05.246145 fullctl-1.2.0rc1/src/fullctl/django/inet/fields.py
+-rw-r--r--   0        0        0      519 2021-06-15 13:03:05.246145 fullctl-1.2.0rc1/src/fullctl/django/inet/util.py
+-rw-r--r--   0        0        0     3738 2021-06-15 13:03:05.246145 fullctl-1.2.0rc1/src/fullctl/django/inet/validators.py
+-rw-r--r--   0        0        0      307 2023-02-27 05:27:02.248818 fullctl-1.2.0rc1/src/fullctl/django/mail.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.955758 fullctl-1.2.0rc1/src/fullctl/django/management/__init__.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.955758 fullctl-1.2.0rc1/src/fullctl/django/management/commands/__init__.py
+-rw-r--r--   0        0        0     4128 2021-10-29 12:45:46.921418 fullctl-1.2.0rc1/src/fullctl/django/management/commands/base.py
+-rw-r--r--   0        0        0     1867 2023-02-27 05:27:02.248818 fullctl-1.2.0rc1/src/fullctl/django/management/commands/fullctl_peeringdb_sync.py
+-rw-r--r--   0        0        0     4750 2023-02-27 05:27:02.249818 fullctl-1.2.0rc1/src/fullctl/django/management/commands/fullctl_poll_tasks.py
+-rw-r--r--   0        0        0      620 2023-02-27 05:27:02.249818 fullctl-1.2.0rc1/src/fullctl/django/management/commands/fullctl_promote_user.py
+-rw-r--r--   0        0        0      763 2023-02-27 05:27:02.249818 fullctl-1.2.0rc1/src/fullctl/django/management/commands/fullctl_work_task.py
+-rw-r--r--   0        0        0     3040 2023-04-15 16:24:16.030446 fullctl-1.2.0rc1/src/fullctl/django/middleware.py
+-rw-r--r--   0        0        0     8661 2023-02-27 05:27:02.250818 fullctl-1.2.0rc1/src/fullctl/django/migrations/0001_initial.py
+-rw-r--r--   0        0        0      291 2023-02-27 05:27:02.250818 fullctl-1.2.0rc1/src/fullctl/django/migrations/0002_delete_apikey.py
+-rw-r--r--   0        0        0     2216 2023-02-27 05:27:02.250818 fullctl-1.2.0rc1/src/fullctl/django/migrations/0003_auditlog.py
+-rw-r--r--   0        0        0     1081 2023-02-27 05:27:02.250818 fullctl-1.2.0rc1/src/fullctl/django/migrations/0004_auto_20210528_1247.py
+-rw-r--r--   0        0        0      625 2023-02-27 05:27:02.250818 fullctl-1.2.0rc1/src/fullctl/django/migrations/0005_auto_20210528_1252.py
+-rw-r--r--   0        0        0     1374 2023-02-27 05:27:02.251818 fullctl-1.2.0rc1/src/fullctl/django/migrations/0006_auto_20210603_0542.py
+-rw-r--r--   0        0        0      485 2023-02-27 05:27:02.251818 fullctl-1.2.0rc1/src/fullctl/django/migrations/0007_auditlog_ip_address.py
+-rw-r--r--   0        0        0     4435 2023-02-27 05:27:02.251818 fullctl-1.2.0rc1/src/fullctl/django/migrations/0008_managementtask.py
+-rw-r--r--   0        0        0     2341 2023-02-27 05:27:02.251818 fullctl-1.2.0rc1/src/fullctl/django/migrations/0009_taskclaim.py
+-rw-r--r--   0        0        0      557 2023-02-27 05:27:02.251818 fullctl-1.2.0rc1/src/fullctl/django/migrations/0010_alter_managementtask_queue_id.py
+-rw-r--r--   0        0        0      749 2023-02-27 05:27:02.252818 fullctl-1.2.0rc1/src/fullctl/django/migrations/0011_alter_managementtask_status.py
+-rw-r--r--   0        0        0     5399 2023-02-27 05:27:02.252818 fullctl-1.2.0rc1/src/fullctl/django/migrations/0012_auto_20210805_1153.py
+-rw-r--r--   0        0        0      723 2023-02-27 05:27:02.252818 fullctl-1.2.0rc1/src/fullctl/django/migrations/0013_auto_20210805_1200.py
+-rw-r--r--   0        0        0      516 2023-02-27 05:27:02.252818 fullctl-1.2.0rc1/src/fullctl/django/migrations/0014_alter_taskclaim_task.py
+-rw-r--r--   0        0        0      625 2023-02-27 05:27:02.252818 fullctl-1.2.0rc1/src/fullctl/django/migrations/0015_alter_task_parent.py
+-rw-r--r--   0        0        0      414 2023-02-27 05:27:02.253818 fullctl-1.2.0rc1/src/fullctl/django/migrations/0016_task_limit_id.py
+-rw-r--r--   0        0        0      463 2023-02-27 05:27:02.253818 fullctl-1.2.0rc1/src/fullctl/django/migrations/0017_alter_organizationuser_options.py
+-rw-r--r--   0        0        0     4271 2023-02-27 05:27:02.253818 fullctl-1.2.0rc1/src/fullctl/django/migrations/0018_task_schedule.py
+-rw-r--r--   0        0        0      402 2023-02-27 05:27:02.253818 fullctl-1.2.0rc1/src/fullctl/django/migrations/0019_default_org.py
+-rw-r--r--   0        0        0      389 2023-02-27 05:27:02.254818 fullctl-1.2.0rc1/src/fullctl/django/migrations/0020_auditlog_action_length.py
+-rw-r--r--   0        0        0     3330 2023-02-27 05:27:02.254818 fullctl-1.2.0rc1/src/fullctl/django/migrations/0021_servicebridgeaction.py
+-rw-r--r--   0        0        0     1077 2023-02-27 05:27:02.254818 fullctl-1.2.0rc1/src/fullctl/django/migrations/0022_auto_20220907_1253.py
+-rw-r--r--   0        0        0     1050 2023-02-27 05:27:02.254818 fullctl-1.2.0rc1/src/fullctl/django/migrations/0023_auto_20220907_1354.py
+-rw-r--r--   0        0        0     2539 2023-02-27 05:27:02.254818 fullctl-1.2.0rc1/src/fullctl/django/migrations/0024_auto_20221012_1227.py
+-rw-r--r--   0        0        0      900 2023-02-27 05:27:02.254818 fullctl-1.2.0rc1/src/fullctl/django/migrations/0025_auto_20221025_1215.py
+-rw-r--r--   0        0        0      837 2023-02-27 05:27:02.255818 fullctl-1.2.0rc1/src/fullctl/django/migrations/0026_auto_20230131_1405.py
+-rw-r--r--   0        0        0     4518 2023-04-15 16:24:16.030446 fullctl-1.2.0rc1/src/fullctl/django/migrations/0027_request_response.py
+-rw-r--r--   0        0        0      457 2023-04-15 16:24:16.030446 fullctl-1.2.0rc1/src/fullctl/django/migrations/0028_request_identifier.py
+-rw-r--r--   0        0        0      427 2023-04-15 16:24:16.030446 fullctl-1.2.0rc1/src/fullctl/django/migrations/0029_response_content.py
+-rw-r--r--   0        0        0      550 2023-04-15 16:24:16.030446 fullctl-1.2.0rc1/src/fullctl/django/migrations/0030_alter_response_content.py
+-rw-r--r--   0        0        0     2496 2023-04-15 16:24:16.030446 fullctl-1.2.0rc1/src/fullctl/django/migrations/0031_auto_20230310_2152.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.956758 fullctl-1.2.0rc1/src/fullctl/django/migrations/__init__.py
+-rw-r--r--   0        0        0      218 2021-10-21 03:49:59.989723 fullctl-1.2.0rc1/src/fullctl/django/models/__init__.py
+-rw-r--r--   0        0        0      150 2022-10-14 13:57:25.208745 fullctl-1.2.0rc1/src/fullctl/django/models/abstract/__init__.py
+-rw-r--r--   0        0        0     3282 2022-06-14 21:13:57.268730 fullctl-1.2.0rc1/src/fullctl/django/models/abstract/alert.py
+-rw-r--r--   0        0        0     3337 2022-10-14 13:57:25.209745 fullctl-1.2.0rc1/src/fullctl/django/models/abstract/base.py
+-rw-r--r--   0        0        0    13540 2023-04-15 16:24:16.030446 fullctl-1.2.0rc1/src/fullctl/django/models/abstract/meta.py
+-rw-r--r--   0        0        0     7822 2023-02-27 05:27:02.255818 fullctl-1.2.0rc1/src/fullctl/django/models/abstract/service_bridge.py
+-rw-r--r--   0        0        0     2682 2023-02-27 05:27:02.256818 fullctl-1.2.0rc1/src/fullctl/django/models/abstract/template.py
+-rw-r--r--   0        0        0      288 2023-04-15 16:24:16.030446 fullctl-1.2.0rc1/src/fullctl/django/models/concrete/__init__.py
+-rw-r--r--   0        0        0     7437 2023-02-27 05:27:02.256818 fullctl-1.2.0rc1/src/fullctl/django/models/concrete/account.py
+-rw-r--r--   0        0        0     1884 2023-02-27 05:27:02.256818 fullctl-1.2.0rc1/src/fullctl/django/models/concrete/auditlog.py
+-rw-r--r--   0        0        0     1808 2023-04-15 16:24:16.030446 fullctl-1.2.0rc1/src/fullctl/django/models/concrete/meta.py
+-rw-r--r--   0        0        0     7811 2023-02-27 05:27:02.257818 fullctl-1.2.0rc1/src/fullctl/django/models/concrete/service_bridge.py
+-rw-r--r--   0        0        0    16238 2023-04-15 16:24:16.031446 fullctl-1.2.0rc1/src/fullctl/django/models/concrete/tasks.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.956758 fullctl-1.2.0rc1/src/fullctl/django/rest/__init__.py
+-rw-r--r--   0        0        0     8217 2023-02-27 05:27:02.257818 fullctl-1.2.0rc1/src/fullctl/django/rest/api_schema.py
+-rw-r--r--   0        0        0     1143 2021-10-29 12:45:46.966419 fullctl-1.2.0rc1/src/fullctl/django/rest/authentication.py
+-rw-r--r--   0        0        0     1831 2021-06-15 13:03:05.250145 fullctl-1.2.0rc1/src/fullctl/django/rest/core.py
+-rw-r--r--   0        0        0     8517 2023-02-27 05:27:02.258818 fullctl-1.2.0rc1/src/fullctl/django/rest/decorators.py
+-rw-r--r--   0        0        0      328 2023-02-27 05:27:02.258818 fullctl-1.2.0rc1/src/fullctl/django/rest/fields.py
+-rw-r--r--   0        0        0     1074 2021-10-21 03:50:00.023724 fullctl-1.2.0rc1/src/fullctl/django/rest/filters.py
+-rw-r--r--   0        0        0     1486 2022-10-14 13:57:25.257745 fullctl-1.2.0rc1/src/fullctl/django/rest/mixins.py
+-rw-r--r--   0        0        0     2148 2021-10-29 12:45:46.983419 fullctl-1.2.0rc1/src/fullctl/django/rest/renderers.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.957758 fullctl-1.2.0rc1/src/fullctl/django/rest/route/__init__.py
+-rw-r--r--   0        0        0      352 2023-02-27 05:27:02.258818 fullctl-1.2.0rc1/src/fullctl/django/rest/route/aaactl_sync.py
+-rw-r--r--   0        0        0      298 2021-10-21 03:50:00.070725 fullctl-1.2.0rc1/src/fullctl/django/rest/route/account.py
+-rw-r--r--   0        0        0      426 2023-02-27 05:27:02.258818 fullctl-1.2.0rc1/src/fullctl/django/rest/route/service_bridge.py
+-rw-r--r--   0        0        0      342 2023-02-27 05:27:02.259818 fullctl-1.2.0rc1/src/fullctl/django/rest/route/usage.py
+-rw-r--r--   0        0        0     1558 2023-02-27 05:27:02.259818 fullctl-1.2.0rc1/src/fullctl/django/rest/serializers/__init__.py
+-rw-r--r--   0        0        0     2136 2023-04-15 16:24:16.031446 fullctl-1.2.0rc1/src/fullctl/django/rest/serializers/aaactl_sync.py
+-rw-r--r--   0        0        0     2523 2023-04-15 17:32:55.630524 fullctl-1.2.0rc1/src/fullctl/django/rest/serializers/account.py
+-rw-r--r--   0        0        0      518 2023-04-15 16:24:16.032446 fullctl-1.2.0rc1/src/fullctl/django/rest/serializers/meta.py
+-rw-r--r--   0        0        0      807 2022-10-14 13:57:25.258745 fullctl-1.2.0rc1/src/fullctl/django/rest/serializers/org.py
+-rw-r--r--   0        0        0      233 2023-02-27 05:27:02.260818 fullctl-1.2.0rc1/src/fullctl/django/rest/serializers/service_bridge.py
+-rw-r--r--   0        0        0      688 2022-10-14 13:57:25.258745 fullctl-1.2.0rc1/src/fullctl/django/rest/serializers/template.py
+-rw-r--r--   0        0        0      440 2023-02-27 05:27:02.260818 fullctl-1.2.0rc1/src/fullctl/django/rest/serializers/usage.py
+-rw-r--r--   0        0        0      395 2023-04-15 17:32:55.630524 fullctl-1.2.0rc1/src/fullctl/django/rest/throttle.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.958758 fullctl-1.2.0rc1/src/fullctl/django/rest/urls/__init__.py
+-rw-r--r--   0        0        0      222 2021-10-21 03:50:00.135727 fullctl-1.2.0rc1/src/fullctl/django/rest/urls/aaactl_sync.py
+-rw-r--r--   0        0        0      210 2021-06-15 13:03:05.251145 fullctl-1.2.0rc1/src/fullctl/django/rest/urls/account.py
+-rw-r--r--   0        0        0      491 2021-10-29 12:45:46.983419 fullctl-1.2.0rc1/src/fullctl/django/rest/urls/service_bridge.py
+-rw-r--r--   0        0        0     2084 2023-02-27 05:27:02.260818 fullctl-1.2.0rc1/src/fullctl/django/rest/urls/service_bridge_proxy.py
+-rw-r--r--   0        0        0      204 2021-06-15 13:03:05.251145 fullctl-1.2.0rc1/src/fullctl/django/rest/urls/usage.py
+-rw-r--r--   0        0        0      419 2021-06-15 13:03:05.251145 fullctl-1.2.0rc1/src/fullctl/django/rest/usage.py
+-rw-r--r--   0        0        0        0 2021-06-15 13:03:05.251145 fullctl-1.2.0rc1/src/fullctl/django/rest/views/__init__.py
+-rw-r--r--   0        0        0     3258 2022-10-14 13:57:25.258745 fullctl-1.2.0rc1/src/fullctl/django/rest/views/aaactl_sync.py
+-rw-r--r--   0        0        0     2576 2023-04-15 17:32:55.630524 fullctl-1.2.0rc1/src/fullctl/django/rest/views/account.py
+-rw-r--r--   0        0        0     7159 2023-04-15 17:32:55.630524 fullctl-1.2.0rc1/src/fullctl/django/rest/views/service_bridge.py
+-rw-r--r--   0        0        0      994 2023-02-27 05:27:02.261818 fullctl-1.2.0rc1/src/fullctl/django/rest/views/template.py
+-rw-r--r--   0        0        0     1410 2023-02-27 05:27:02.261818 fullctl-1.2.0rc1/src/fullctl/django/rest/views/usage.py
+-rw-r--r--   0        0        0    16282 2023-04-15 17:32:55.631524 fullctl-1.2.0rc1/src/fullctl/django/settings/__init__.py
+-rw-r--r--   0        0        0     2655 2023-02-27 05:27:02.262818 fullctl-1.2.0rc1/src/fullctl/django/settings/default.py
+-rw-r--r--   0        0        0     1215 2023-02-27 05:27:02.262818 fullctl-1.2.0rc1/src/fullctl/django/signals.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.958758 fullctl-1.2.0rc1/src/fullctl/django/social/__init__.py
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.958758 fullctl-1.2.0rc1/src/fullctl/django/social/backends/__init__.py
+-rw-r--r--   0        0        0     1206 2021-06-15 13:03:05.252145 fullctl-1.2.0rc1/src/fullctl/django/social/backends/peeringdb.py
+-rw-r--r--   0        0        0     1589 2021-10-21 03:50:00.137727 fullctl-1.2.0rc1/src/fullctl/django/social/backends/twentyc.py
+-rw-r--r--   0        0        0      388 2021-06-15 13:03:05.252145 fullctl-1.2.0rc1/src/fullctl/django/social/pipelines/__init__.py
+-rw-r--r--   0        0        0     4237 2021-04-22 13:27:52.959758 fullctl-1.2.0rc1/src/fullctl/django/static/common/20c/twentyc.core.min.js
+-rw-r--r--   0        0        0    56503 2023-04-15 17:32:55.631524 fullctl-1.2.0rc1/src/fullctl/django/static/common/20c/twentyc.rest.js
+-rw-r--r--   0        0        0     9475 2021-04-22 13:27:52.959758 fullctl-1.2.0rc1/src/fullctl/django/static/common/20c-logo-filled.svg
+-rw-r--r--   0        0        0    21299 2023-02-27 05:27:02.264818 fullctl-1.2.0rc1/src/fullctl/django/static/common/app.css
+-rw-r--r--   0        0        0    19449 2023-02-27 05:27:02.265818 fullctl-1.2.0rc1/src/fullctl/django/static/common/app.js
+-rwxr-xr-x   0        0        0   372526 2021-10-29 12:45:47.007420 fullctl-1.2.0rc1/src/fullctl/django/static/common/favicon.ico
+-rw-r--r--   0        0        0     3380 2021-04-22 13:27:52.960758 fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/Indicator/Check-Ind/Check.svg
+-rw-r--r--   0        0        0     3657 2021-04-22 13:27:52.960758 fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/Indicator/X-Ind/X.svg
+-rw-r--r--   0        0        0     3430 2021-04-22 13:27:52.960758 fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/icon/add.svg
+-rw-r--r--   0        0        0     3819 2021-04-22 13:27:52.961758 fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/icon/alerts.svg
+-rw-r--r--   0        0        0     2838 2022-06-14 21:13:57.362731 fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/icon/api.svg
+-rw-r--r--   0        0        0     1303 2021-04-22 13:27:52.961758 fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/icon/dark-mode.svg
+-rw-r--r--   0        0        0     2681 2021-04-22 13:27:52.961758 fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/icon/delete.svg
+-rw-r--r--   0        0        0     5490 2021-04-22 13:27:52.961758 fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/icon/edit.svg
+-rwxr-xr-x   0        0        0     1172 2021-10-29 12:45:47.024420 fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/icon/launch.svg
+-rw-r--r--   0        0        0     1601 2021-04-22 13:27:52.961758 fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/icon/light-mode.svg
+-rw-r--r--   0        0        0     3357 2021-04-22 13:27:52.961758 fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/icon/list.svg
+-rwxr-xr-x   0        0        0     1721 2022-06-14 21:13:57.362731 fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/icon/location.svg
+-rw-r--r--   0        0        0     2617 2021-04-22 13:27:52.961758 fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/icon/logout.svg
+-rwxr-xr-x   0        0        0      726 2021-10-29 12:45:47.026420 fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/icon/mail.svg
+-rw-r--r--   0        0        0     2761 2021-04-22 13:27:52.961758 fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/icon/org.svg
+-rw-r--r--   0        0        0     1597 2022-06-14 21:13:57.599734 fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/icon/refresh.svg
+-rw-r--r--   0        0        0     1515 2022-06-14 21:13:57.623735 fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/icon/report.svg
+-rw-r--r--   0        0        0     8263 2021-04-22 13:27:52.961758 fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/icon/settings.svg
+-rw-r--r--   0        0        0     4138 2021-04-22 13:27:52.961758 fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/icon/user.svg
+-rwxr-xr-x   0        0        0     2782 2021-10-29 12:45:47.035421 fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/icon/view.svg
+-rw-r--r--   0        0        0     3689 2021-04-22 13:27:52.962758 fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/ixctl-logo-darkbg.svg
+-rw-r--r--   0        0        0      169 2021-04-22 13:27:52.962758 fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/md-add.svg
+-rw-r--r--   0        0        0      275 2021-04-22 13:27:52.962758 fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/md-create.svg
+-rw-r--r--   0        0        0      272 2021-04-22 13:27:52.962758 fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/md-list-box.svg
+-rw-r--r--   0        0        0      240 2021-04-22 13:27:52.962758 fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/md-trash.svg
+-rw-r--r--   0        0        0     5957 2021-04-22 13:27:52.962758 fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/prefixctl-logo-darkbg.svg
+-rw-r--r--   0        0        0      954 2021-04-22 13:27:52.962758 fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/ui-caret-caret/down.svg
+-rw-r--r--   0        0        0      818 2021-04-22 13:27:52.962758 fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/ui-close.svg
+-rwxr-xr-x   0        0        0     2427 2023-02-27 05:27:02.266818 fullctl-1.2.0rc1/src/fullctl/django/static/common/logos/aclctl-dark.svg
+-rwxr-xr-x   0        0        0    36084 2023-04-15 16:24:16.033446 fullctl-1.2.0rc1/src/fullctl/django/static/common/logos/ctl-mark-dark.png
+-rwxr-xr-x   0        0        0    36307 2023-04-15 16:24:16.033446 fullctl-1.2.0rc1/src/fullctl/django/static/common/logos/ctl-mark-light.png
+-rwxr-xr-x   0        0        0     4680 2022-10-14 13:57:25.295745 fullctl-1.2.0rc1/src/fullctl/django/static/common/logos/devicectl-dark.svg
+-rwxr-xr-x   0        0        0     2579 2021-10-29 12:45:47.035421 fullctl-1.2.0rc1/src/fullctl/django/static/common/logos/ixctl-dark.svg
+-rwxr-xr-x   0        0        0     3857 2021-10-29 12:45:47.035421 fullctl-1.2.0rc1/src/fullctl/django/static/common/logos/pdbctl-dark.svg
+-rwxr-xr-x   0        0        0     4166 2021-10-29 12:45:47.036420 fullctl-1.2.0rc1/src/fullctl/django/static/common/logos/peerctl-dark.svg
+-rwxr-xr-x   0        0        0     4336 2022-06-14 21:13:57.623735 fullctl-1.2.0rc1/src/fullctl/django/static/common/logos/prefixctl-dark.svg
+-rw-r--r--   0        0        0     9475 2021-04-22 13:27:52.962758 fullctl-1.2.0rc1/src/fullctl/django/static/common/oauth/20c.svg
+-rw-r--r--   0        0        0      689 2021-04-22 13:27:52.963758 fullctl-1.2.0rc1/src/fullctl/django/static/common/oauth/google.svg
+-rw-r--r--   0        0        0     5222 2023-04-15 16:24:16.033446 fullctl-1.2.0rc1/src/fullctl/django/static/common/oauth/peeringdb-dark.png
+-rw-r--r--   0        0        0     9186 2021-04-22 13:27:52.963758 fullctl-1.2.0rc1/src/fullctl/django/static/common/oauth/peeringdb.png
+-rw-r--r--   0        0        0     4323 2021-10-21 03:50:00.180728 fullctl-1.2.0rc1/src/fullctl/django/static/common/service_bridge.js
+-rw-r--r--   0        0        0    11545 2023-02-27 05:27:02.266818 fullctl-1.2.0rc1/src/fullctl/django/static/common/themes/dark.css
+-rw-r--r--   0        0        0        0 2021-04-22 13:27:52.963758 fullctl-1.2.0rc1/src/fullctl/django/static/common/themes/light.css
+-rw-r--r--   0        0        0    25412 2023-04-15 17:32:55.632524 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/app.css
+-rw-r--r--   0        0        0    32037 2023-04-15 17:32:55.632524 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/app.js
+-rw-r--r--   0        0        0      644 2023-02-27 05:27:02.268818 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/icons/add.svg
+-rw-r--r--   0        0        0     4812 2023-02-27 05:27:02.268818 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/icons/api.svg
+-rw-r--r--   0        0        0      352 2023-02-27 05:27:02.269818 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/icons/arrow-clockwise.svg
+-rw-r--r--   0        0        0      232 2023-02-27 05:27:02.269818 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/icons/arrow.svg
+-rw-r--r--   0        0        0      532 2023-02-27 05:27:02.269818 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/icons/box-arrow-up-right.svg
+-rw-r--r--   0        0        0      423 2023-02-27 05:27:02.269818 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/icons/cancel.svg
+-rw-r--r--   0        0        0      274 2023-02-27 05:27:02.269818 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/icons/close.svg
+-rw-r--r--   0        0        0     1229 2023-04-15 16:24:16.034446 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/icons/database.svg
+-rw-r--r--   0        0        0      427 2023-02-27 05:27:02.269818 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/icons/download.svg
+-rw-r--r--   0        0        0      438 2023-02-27 05:27:02.269818 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/icons/envelope.svg
+-rw-r--r--   0        0        0      569 2023-02-27 05:27:02.270818 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/icons/eye.svg
+-rw-r--r--   0        0        0      483 2023-02-27 05:27:02.270818 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/icons/file-earmark-text.svg
+-rw-r--r--   0        0        0     1530 2023-02-27 05:27:02.270818 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/icons/gear.svg
+-rw-r--r--   0        0        0      483 2023-02-27 05:27:02.270818 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/icons/geo-alt.svg
+-rw-r--r--   0        0        0     1975 2023-02-27 05:27:02.270818 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/icons/help.svg
+-rw-r--r--   0        0        0      582 2023-02-27 05:27:02.271818 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/icons/list/delete.svg
+-rw-r--r--   0        0        0      438 2023-02-27 05:27:02.271818 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/icons/list/edit.svg
+-rw-r--r--   0        0        0      818 2023-02-27 05:27:02.271818 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/icons/list/options.svg
+-rw-r--r--   0        0        0      447 2023-02-27 05:27:02.270818 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/icons/list-ul.svg
+-rw-r--r--   0        0        0      553 2023-02-27 05:27:02.271818 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/icons/logout.svg
+-rw-r--r--   0        0        0      749 2023-02-27 05:27:02.271818 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/icons/org.svg
+-rw-r--r--   0        0        0      331 2023-02-27 05:27:02.271818 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/icons/search.svg
+-rw-r--r--   0        0        0     1465 2023-02-27 05:27:02.272818 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/icons/theme-switcher.svg
+-rw-r--r--   0        0        0      465 2023-02-27 05:27:02.272818 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/icons/ui-caret/dbl-select.svg
+-rw-r--r--   0        0        0      190 2023-02-27 05:27:02.272818 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/icons/ui-caret/down.svg
+-rw-r--r--   0        0        0     4138 2023-02-27 05:27:02.272818 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/icons/user.svg
+-rw-r--r--   0        0        0     3986 2023-02-27 05:27:02.272818 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/icons/view-settings.svg
+-rw-r--r--   0        0        0    61189 2023-02-27 05:27:02.273818 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/imgs/help.png
+-rw-r--r--   0        0        0   426086 2023-04-15 16:24:16.037446 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/imgs/loading-shim.png
+-rw-r--r--   0        0        0    14637 2023-04-15 16:24:16.037446 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/themes/dark.css
+-rw-r--r--   0        0        0        0 2023-02-27 05:27:02.273818 fullctl-1.2.0rc1/src/fullctl/django/static/common/v2/themes/light.css
+-rw-r--r--   0        0        0      921 2023-02-27 05:27:02.274818 fullctl-1.2.0rc1/src/fullctl/django/tasks/__init__.py
+-rw-r--r--   0        0        0      740 2021-10-21 03:50:00.186728 fullctl-1.2.0rc1/src/fullctl/django/tasks/celery.py
+-rw-r--r--   0        0        0     2351 2023-04-15 16:24:16.037446 fullctl-1.2.0rc1/src/fullctl/django/tasks/orm.py
+-rw-r--r--   0        0        0     2220 2023-04-15 16:24:16.037446 fullctl-1.2.0rc1/src/fullctl/django/tasks/qualifiers.py
+-rw-r--r--   0        0        0      374 2023-02-27 05:27:02.274818 fullctl-1.2.0rc1/src/fullctl/django/tasks/util.py
+-rw-r--r--   0        0        0      658 2022-10-14 13:57:25.296744 fullctl-1.2.0rc1/src/fullctl/django/templates/common/apidocs/redoc.html
+-rw-r--r--   0        0        0      856 2022-10-14 13:57:25.296744 fullctl-1.2.0rc1/src/fullctl/django/templates/common/apidocs/swagger.html
+-rw-r--r--   0        0        0     8871 2022-10-14 13:57:25.296744 fullctl-1.2.0rc1/src/fullctl/django/templates/common/app/base.html
+-rw-r--r--   0        0        0      211 2021-04-22 13:27:52.964758 fullctl-1.2.0rc1/src/fullctl/django/templates/common/app/checkbox.html
+-rw-r--r--   0        0        0     1935 2021-04-22 13:27:52.964758 fullctl-1.2.0rc1/src/fullctl/django/templates/common/app/forms/alert-prefs.html
+-rw-r--r--   0        0        0      726 2021-04-22 13:27:52.964758 fullctl-1.2.0rc1/src/fullctl/django/templates/common/app/forms/import-org.html
+-rw-r--r--   0        0        0      494 2021-04-22 13:27:52.964758 fullctl-1.2.0rc1/src/fullctl/django/templates/common/app/forms/invite.html
+-rw-r--r--   0        0        0      792 2021-04-22 13:27:52.964758 fullctl-1.2.0rc1/src/fullctl/django/templates/common/app/forms/org-create.html
+-rw-r--r--   0        0        0     3826 2021-04-22 13:27:52.964758 fullctl-1.2.0rc1/src/fullctl/django/templates/common/app/forms/org-prefs.html
+-rw-r--r--   0        0        0      355 2021-06-15 13:03:05.254145 fullctl-1.2.0rc1/src/fullctl/django/templates/common/app/index.html
+-rw-r--r--   0        0        0     1974 2021-04-22 13:27:52.964758 fullctl-1.2.0rc1/src/fullctl/django/templates/common/app/manage/permissions.html
+-rw-r--r--   0        0        0     4752 2022-10-14 13:57:25.297744 fullctl-1.2.0rc1/src/fullctl/django/templates/common/app/modal.html
+-rw-r--r--   0        0        0     2668 2021-04-22 13:27:52.965758 fullctl-1.2.0rc1/src/fullctl/django/templates/common/app/navbar.html
+-rw-r--r--   0        0        0      371 2023-02-27 05:27:02.275818 fullctl-1.2.0rc1/src/fullctl/django/templates/common/app/templates.html
+-rw-r--r--   0        0        0     3101 2022-10-14 13:57:25.297744 fullctl-1.2.0rc1/src/fullctl/django/templates/common/auth/login.html
+-rw-r--r--   0        0        0      880 2021-04-22 13:27:52.965758 fullctl-1.2.0rc1/src/fullctl/django/templates/common/auth/oauth-badge.html
+-rw-r--r--   0        0        0     1110 2021-04-22 13:27:52.965758 fullctl-1.2.0rc1/src/fullctl/django/templates/common/auth/oauth.html
+-rw-r--r--   0        0        0     1996 2023-04-15 16:24:16.038446 fullctl-1.2.0rc1/src/fullctl/django/templates/common/base.html
+-rw-r--r--   0        0        0      333 2021-06-15 13:03:05.255145 fullctl-1.2.0rc1/src/fullctl/django/templates/common/errors/400.html
+-rw-r--r--   0        0        0      367 2021-06-15 13:03:05.255145 fullctl-1.2.0rc1/src/fullctl/django/templates/common/errors/401.html
+-rw-r--r--   0        0        0      375 2021-06-15 13:03:05.255145 fullctl-1.2.0rc1/src/fullctl/django/templates/common/errors/403.html
+-rw-r--r--   0        0        0      377 2021-06-15 13:03:05.255145 fullctl-1.2.0rc1/src/fullctl/django/templates/common/errors/404.html
+-rw-r--r--   0        0        0      456 2021-06-15 13:03:05.255145 fullctl-1.2.0rc1/src/fullctl/django/templates/common/errors/500.html
+-rw-r--r--   0        0        0      565 2021-06-15 13:03:05.255145 fullctl-1.2.0rc1/src/fullctl/django/templates/common/errors/base.html
+-rw-r--r--   0        0        0      351 2021-06-15 13:03:05.255145 fullctl-1.2.0rc1/src/fullctl/django/templates/common/errors/details.html
+-rw-r--r--   0        0        0     1229 2022-06-14 21:13:57.992740 fullctl-1.2.0rc1/src/fullctl/django/templates/common/snippets.html
+-rw-r--r--   0        0        0      234 2021-04-22 13:27:52.965758 fullctl-1.2.0rc1/src/fullctl/django/templates/common/tool_base.html
+-rw-r--r--   0        0        0      658 2023-02-27 05:27:02.276818 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/apidocs/redoc.html
+-rw-r--r--   0        0        0      856 2023-02-27 05:27:02.276818 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/apidocs/swagger.html
+-rw-r--r--   0        0        0    12217 2023-04-15 17:32:55.632524 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/app/base.html
+-rw-r--r--   0        0        0      211 2023-02-27 05:27:02.277818 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/app/checkbox.html
+-rw-r--r--   0        0        0     2092 2023-04-15 17:32:55.632524 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/app/cross-promote-trials.html
+-rw-r--r--   0        0        0      357 2023-02-27 05:27:02.277818 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/app/delete_selected.html
+-rw-r--r--   0        0        0     1775 2023-04-15 17:32:55.632524 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/app/footer.html
+-rw-r--r--   0        0        0     1935 2023-02-27 05:27:02.278818 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/app/forms/alert-prefs.html
+-rw-r--r--   0        0        0      430 2023-04-15 17:32:55.632524 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/app/forms/feature-request.html
+-rw-r--r--   0        0        0      726 2023-02-27 05:27:02.278818 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/app/forms/import-org.html
+-rw-r--r--   0        0        0      494 2023-02-27 05:27:02.278818 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/app/forms/invite.html
+-rw-r--r--   0        0        0      792 2023-02-27 05:27:02.278818 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/app/forms/org-create.html
+-rw-r--r--   0        0        0     3826 2023-02-27 05:27:02.278818 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/app/forms/org-prefs.html
+-rw-r--r--   0        0        0      358 2023-02-27 05:27:02.279818 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/app/index.html
+-rw-r--r--   0        0        0     1974 2023-02-27 05:27:02.279818 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/app/manage/permissions.html
+-rw-r--r--   0        0        0     6317 2023-04-15 16:24:16.038446 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/app/modal.html
+-rw-r--r--   0        0        0     2668 2023-02-27 05:27:02.280818 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/app/navbar.html
+-rw-r--r--   0        0        0      413 2023-02-27 05:27:02.280818 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/app/templates.html
+-rw-r--r--   0        0        0     3048 2023-02-27 05:27:02.280818 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/auth/login.html
+-rw-r--r--   0        0        0     1109 2023-04-15 16:24:16.038446 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/auth/oauth-badge.html
+-rw-r--r--   0        0        0     1339 2023-04-15 16:24:16.038446 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/auth/oauth.html
+-rw-r--r--   0        0        0     1977 2023-04-15 16:24:16.038446 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/base.html
+-rw-r--r--   0        0        0      339 2023-02-27 05:27:02.281818 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/errors/400.html
+-rw-r--r--   0        0        0      373 2023-02-27 05:27:02.281818 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/errors/401.html
+-rw-r--r--   0        0        0      381 2023-02-27 05:27:02.281818 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/errors/403.html
+-rw-r--r--   0        0        0      383 2023-02-27 05:27:02.281818 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/errors/404.html
+-rw-r--r--   0        0        0      462 2023-02-27 05:27:02.281818 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/errors/500.html
+-rw-r--r--   0        0        0      568 2023-02-27 05:27:02.282818 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/errors/base.html
+-rw-r--r--   0        0        0      351 2023-02-27 05:27:02.282818 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/errors/details.html
+-rw-r--r--   0        0        0     1661 2023-04-15 16:24:16.039446 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/snippets.html
+-rw-r--r--   0        0        0      234 2023-02-27 05:27:02.282818 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/tool_base.html
+-rw-r--r--   0        0        0      249 2023-02-27 05:27:02.282818 fullctl-1.2.0rc1/src/fullctl/django/templates/common/v2/tool_base_sidebar.html
+-rw-r--r--   0        0        0        0 2022-06-14 21:13:57.992740 fullctl-1.2.0rc1/src/fullctl/django/templatetags/__init__.py
+-rw-r--r--   0        0        0     3398 2023-04-15 16:24:16.039446 fullctl-1.2.0rc1/src/fullctl/django/templatetags/fullctl_util.py
+-rw-r--r--   0        0        0     3152 2023-02-27 05:27:02.283818 fullctl-1.2.0rc1/src/fullctl/django/testutil.py
+-rw-r--r--   0        0        0     3266 2023-04-15 17:32:55.633525 fullctl-1.2.0rc1/src/fullctl/django/urls.py
+-rw-r--r--   0        0        0     1171 2023-02-27 05:27:02.283818 fullctl-1.2.0rc1/src/fullctl/django/util.py
+-rw-r--r--   0        0        0     1193 2022-10-14 13:57:25.299744 fullctl-1.2.0rc1/src/fullctl/django/validators.py
+-rw-r--r--   0        0        0     2304 2023-02-27 05:27:02.284818 fullctl-1.2.0rc1/src/fullctl/django/views/__init__.py
+-rw-r--r--   0        0        0      199 2022-10-14 13:57:25.300744 fullctl-1.2.0rc1/src/fullctl/django/views/api_schema.py
+-rw-r--r--   0        0        0      927 2023-04-15 17:32:55.633525 fullctl-1.2.0rc1/src/fullctl/django/views/template.py
+-rw-r--r--   0        0        0        0 2021-06-15 13:03:05.256145 fullctl-1.2.0rc1/src/fullctl/service_bridge/__init__.py
+-rw-r--r--   0        0        0     2604 2023-04-15 17:32:55.633525 fullctl-1.2.0rc1/src/fullctl/service_bridge/aaactl.py
+-rw-r--r--   0        0        0     8510 2023-04-15 16:24:16.052446 fullctl-1.2.0rc1/src/fullctl/service_bridge/client.py
+-rw-r--r--   0        0        0     3419 2023-02-27 05:27:02.285818 fullctl-1.2.0rc1/src/fullctl/service_bridge/data.py
+-rw-r--r--   0        0        0     2180 2023-04-15 16:24:16.053446 fullctl-1.2.0rc1/src/fullctl/service_bridge/devicectl.py
+-rw-r--r--   0        0        0     2577 2023-04-15 16:24:16.053446 fullctl-1.2.0rc1/src/fullctl/service_bridge/ixctl.py
+-rw-r--r--   0        0        0     2651 2023-02-27 05:27:02.286818 fullctl-1.2.0rc1/src/fullctl/service_bridge/nautobot.py
+-rw-r--r--   0        0        0     1699 2023-04-15 16:24:16.054446 fullctl-1.2.0rc1/src/fullctl/service_bridge/pdbctl.py
+-rw-r--r--   0        0        0     1037 2023-04-15 16:24:16.063447 fullctl-1.2.0rc1/src/fullctl/service_bridge/peerctl.py
+-rw-r--r--   0        0        0     1076 2023-04-15 16:24:16.097447 fullctl-1.2.0rc1/src/fullctl/service_bridge/prefixctl.py
+-rw-r--r--   0        0        0     6952 2023-04-15 16:24:16.097447 fullctl-1.2.0rc1/src/fullctl/service_bridge/sot.py
+-rw-r--r--   0        0        0      323 2022-10-14 13:57:25.408743 fullctl-1.2.0rc1/src/fullctl/utils/__init__.py
+-rw-r--r--   0        0        0     1868 1970-01-01 00:00:00.000000 fullctl-1.2.0rc1/PKG-INFO
```

### Comparing `fullctl-0.3.0/LICENSE` & `fullctl-1.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/decorators.py` & `fullctl-1.2.0rc1/src/fullctl/django/decorators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,31 @@
+from functools import wraps
+
 import django.http
+from django.http import JsonResponse
 from django.shortcuts import redirect
 from django.urls import reverse
 
+import fullctl.django.context as context
 from fullctl.django.models import Instance, Organization
 
 
 class require_auth:
 
     """
     decorate a view to require auth
     """
 
     def __call__(self, fn):
         def wrapped(request, *args, **kwargs):
             if not request.user.is_authenticated:
-
-                # return redirect(
-                #     reverse("social:begin", args=("twentyc",))
-                #     + f"?next={request.get_full_path()}"
-                # )
-                return redirect(reverse("login") + f"?next={request.get_full_path()}")
+                return redirect(
+                    reverse("social:begin", args=("twentyc",))
+                    + f"?next={request.get_full_path()}"
+                )
 
             return fn(request, *args, **kwargs)
 
         wrapped.__name__ = fn.__name__
         return wrapped
 
 
@@ -49,26 +51,66 @@
         self.public = public
 
     def __call__(self, fn):
         model = self.model
         public = self.public
 
         def wrapped(request, *args, **kwargs):
-
             org = request.org
-            print("ORG", org)
             if not public and org not in Organization.accessible(request.user):
-                raise django.http.Http404()
+                if request.user.is_authenticated and not getattr(
+                    request, "impersonating", None
+                ):
+                    raise django.http.Http404()
+                else:
+                    return redirect(
+                        reverse("login") + f"?next={request.get_full_path()}"
+                    )
 
             try:
                 instance, _ = model.objects.get_or_create(org=org)
             except model.DoesNotExist:
                 raise django.http.Http404()
 
             request.app_id = instance.app_id
 
             return fn(request, instance, *args, **kwargs)
 
         wrapped.__name__ = fn.__name__
         wrapped.public = public
 
         return wrapped
+
+
+class service_bridge_sync:
+    def __init__(self, **kwargs):
+        self.ctx_args = kwargs
+
+    def __call__(self, fn):
+        ctx_args = self.ctx_args
+
+        def wrapped(*args, **kwargs):
+            with context.service_bridge_sync(**ctx_args):
+                return fn(*args, **kwargs)
+
+        wrapped.__name__ = fn.__name__
+        return wrapped
+
+
+def origin_allowed(origins):
+    """
+    Origin white listing for CORS enabled views.
+    """
+
+    def decorator(view_func):
+        @wraps(view_func)
+        def _wrapped_view(request, *args, **kwargs):
+            origin = request.META.get("HTTP_ORIGIN")
+            if origin not in origins:
+                response_data = {"status": "error", "message": "Origin not allowed"}
+                return JsonResponse(response_data, status=403)
+
+            return view_func(request, *args, **kwargs)
+
+        return _wrapped_view
+
+    return decorator
```

### Comparing `fullctl-0.3.0/src/fullctl/django/inet/fields.py` & `fullctl-1.2.0rc1/src/fullctl/django/inet/fields.py`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/inet/validators.py` & `fullctl-1.2.0rc1/src/fullctl/django/inet/validators.py`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/middleware.py` & `fullctl-1.2.0rc1/src/fullctl/django/middleware.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,31 @@
+from django.contrib.auth import get_user_model
 from django.http import Http404
 
 from fullctl.django.auth import permissions
+from fullctl.django.context import current_request
 from fullctl.django.models import Organization
 
 
+class CurrentRequestContext:
+
+    """
+    Middleware that sets the current request context
+
+    This allows us to access the current request from anywhere we need to
+    """
+
+    def __init__(self, get_response):
+        self.get_response = get_response
+
+    def __call__(self, request):
+        with current_request(request):
+            return self.get_response(request)
+
+
 class RequestAugmentation:
 
     """
     Augments the request by selecting org from `org_tag`
     passed in the URL
 
     When fullctl is not managed by oauth it also makes sure
@@ -19,33 +37,60 @@
 
     def __call__(self, request):
         response = self.get_response(request)
         return response
 
     def process_view(self, request, view_func, view_args, view_kwargs):
         kwargs = request.resolver_match.kwargs
+
         request.perms = permissions(request.user)
+        request.perms.load()
+
+        if "impersonating" in request.session:
+            # impersonation is enabled, set the impersonated user
+            # as the current user on the request
+
+            impersonate_user = get_user_model().objects.get(
+                id=request.session["impersonating"]
+            )
+
+            request.impersonating = {
+                "superuser": request.user,
+                "user": impersonate_user,
+            }
+            request.user = impersonate_user
+
+            # fetch permissions for the impersonated user
+
+            request.perms = permissions(request.user)
+            request.perms.load()
+
         if (
             not hasattr(request.user, "org_set") or not request.user.org_set.exists()
         ) and "org_tag" not in kwargs:
-
             if not request.user.is_authenticated:
-
                 # user is not authenticated, return
                 # Guest org
 
                 request.org = Organization(name="Guest")
                 return
 
         try:
             if "org_tag" in kwargs:
                 request.org = Organization.objects.get(slug=kwargs["org_tag"])
 
             elif request.user.org_set.exists():
-                request.org = request.user.org_set.first().org
+                default_org = request.user.org_set.filter(is_default=True).first()
+
+                if default_org:
+                    request.org = default_org.org
+                else:
+                    request.org = (
+                        request.user.org_set.filter(user=request.user).first().org
+                    )
 
             if hasattr(request.user, "org_set"):
                 request.orgs = request.user.org_set.all()
             else:
                 request.orgs = []
         except Organization.DoesNotExist:
             raise Http404
```

### Comparing `fullctl-0.3.0/src/fullctl/django/migrations/0001_initial.py` & `fullctl-1.2.0rc1/src/fullctl/django/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from django.conf import settings
 from django.db import migrations, models
 
 import fullctl.django.models.concrete.account
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
     ]
 
     operations = [
```

### Comparing `fullctl-0.3.0/src/fullctl/django/models/abstract/alert.py` & `fullctl-1.2.0rc1/src/fullctl/django/models/abstract/alert.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+from django.conf import settings
 from django.db import models
-
 from django.utils.translation import gettext_lazy as _
 
+from fullctl.django.mail import send_plain
 from fullctl.django.models.abstract.base import HandleRefModel
-from fullctl.django.models.abstract.task_interface import TaskContainer
-
 
 ALERT_RECIPIENT_TYPE = (("email", _("Email")),)
 
-class AlertGroup(TaskContainer):
+# XXX this needs to be adapted to the new task system
+
+
+class AlertGroup(HandleRefModel):
 
     """
     Describes a group of recipients for alert notifications
     """
 
     name = models.CharField(max_length=255, help_text=_("Group name"))
 
@@ -50,15 +52,16 @@
 
         log = self.create_log(subject, message)
 
         for recipient in self.recipients:
             recipient.notify(subject, message)
             log.alertlogrcp_set.add(
                 self.log_recipient_class(
-                    typ=recipient.typ, recipient=recipient.recipient,
+                    typ=recipient.typ,
+                    recipient=recipient.recipient,
                 ),
                 bulk=False,
             )
         return log
 
 
 class AlertRecipient(HandleRefModel):
@@ -119,8 +122,7 @@
 
     class HandleRef:
         tag = "alertlog"
 
     @property
     def recipients(self):
         raise NotImplementedError("Should return recipient set")
-
```

### Comparing `fullctl-0.3.0/src/fullctl/django/models/concrete/account.py` & `fullctl-1.2.0rc1/src/fullctl/django/models/concrete/account.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,22 +2,64 @@
 
 import reversion
 from django.contrib.auth import get_user_model
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 from django_grainy.decorators import grainy_model
 
-from fullctl.django.auth import permissions
+import fullctl.django.auth as auth
 from fullctl.django.models.abstract import HandleRefModel
 
+__all__ = [
+    "generate_secret",
+    "Organization",
+    "Instance",
+    "OrganizationUser",
+    "UserSettings",
+]
+
 
 def generate_secret():
     return token_urlsafe()
 
 
+COLOR_SCHEMES = (
+    ("dark", _("Dark")),
+    ("light", _("Light")),
+)
+
+
+@reversion.register()
+@grainy_model(namespace="user")
+class UserSettings(HandleRefModel):
+    user = models.OneToOneField(
+        get_user_model(), on_delete=models.CASCADE, related_name="settings"
+    )
+    theme = models.CharField(
+        max_length=255,
+        null=True,
+        blank=True,
+        help_text=_("override layout theme for this user"),
+    )
+    color_scheme = models.CharField(
+        max_length=255,
+        choices=COLOR_SCHEMES,
+        default="dark",
+        help_text=_("user's color scheme selection"),
+    )
+
+    class HandleRef:
+        tag = "user_settings"
+
+    class Meta:
+        db_table = "fullctl_user_settings"
+        verbose_name = _("User settings")
+        verbose_name_plural = _("User settings")
+
+
 @reversion.register()
 @grainy_model(namespace="org", namespace_instance="org.{instance.permission_id}")
 class Organization(HandleRefModel):
 
     """
     Describes an organization
     """
@@ -62,15 +104,14 @@
     def permission_id(self):
         if self.remote_id:
             return self.remote_id
         return self.id
 
     @classmethod
     def accessible(cls, user):
-
         """
         Returns a list of organizations that are accessible by the
         user.
 
         Accessible here means they either have direct read permissions
         to the organization or to an object inside the organization
 
@@ -79,30 +120,29 @@
         - user (`User`)
 
         **Returns**
 
         - `list`
         """
 
-        perms = permissions(user)
+        perms = auth.permissions(user)
 
         # user is a member of these orgs
         if hasattr(user, "org_set"):
             related_orgs = [o.org for o in user.org_set.all()]
         else:
             related_orgs = []
 
         # user has permissions to these orgs (customer of)
         permissioned_orgs = []
 
         perms.load()
         org_namespaces = perms.pset.expand("?.?", exact=True)
 
         for ns in org_namespaces:
-
             try:
                 int(ns[1])
             except (ValueError, IndexError):
                 continue
 
             try:
                 org = cls.objects.get(remote_id=ns[1])
@@ -136,40 +176,51 @@
                 changed = True
             if data["name"] != org.name:
                 org.name = data["name"]
                 changed = True
             if data["personal"] != org.personal:
                 org.personal = data["personal"]
                 changed = True
+
             if changed:
                 org.save()
         except cls.DoesNotExist:
             org = cls.objects.create(
                 remote_id=data["id"],
                 backend=backend,
                 name=data["name"],
                 slug=data["slug"],
                 personal=data["personal"],
             )
 
+        is_default = data.get("is_default", False)
+
         if not user.org_set.filter(org=org).exists():
-            OrganizationUser.objects.create(org=org, user=user)
+            OrganizationUser.objects.create(org=org, user=user, is_default=is_default)
+        else:
+            user.org_set.filter(org=org).update(is_default=is_default)
 
         return org
 
     @property
     def tag(self):
         return self.slug
 
     @property
     def display_name(self):
         if self.personal:
             return _("Personal")
         return self.name
 
+    @property
+    def display_name_verbose(self):
+        if self.personal:
+            return _("your personal organization")
+        return self.name
+
     def __str__(self):
         return f"{self.name} ({self.slug})"
 
 
 @grainy_model(namespace="org")
 class Instance(HandleRefModel):
 
@@ -221,42 +272,19 @@
     org = models.ForeignKey(
         Organization, on_delete=models.CASCADE, related_name="user_set"
     )
     user = models.ForeignKey(
         get_user_model(), on_delete=models.CASCADE, related_name="org_set"
     )
 
+    is_default = models.BooleanField(default=False)
+
     class HandleRef:
-        tag = "orguser"
+        tag = "org_user"
 
     class Meta:
         db_table = "fullctl_org_user"
         verbose_name = _("Organization User")
-        verbose_name = _("Organization Users")
+        verbose_name_plural = _("Organization Users")
 
     def __str__(self):
         return f"{self.user.username} <{self.user.email}>"
-
-
-@reversion.register
-@grainy_model(namespace="org")
-class APIKey(HandleRefModel):
-    """
-    Describes an APIKey
-
-    These are managed in account.20c.com, but will also be cached here
-
-    Creation should always happen at account.20c.com
-    """
-
-    key = models.CharField(max_length=255, unique=True)
-    user = models.ForeignKey(
-        get_user_model(), on_delete=models.CASCADE, related_name="key_set"
-    )
-
-    class Meta:
-        db_table = "fullctl_apikey"
-        verbose_name = _("API Key")
-        verbose_name_plural = _("API Keys")
-
-    class HandleRef:
-        tag = "key"
```

### Comparing `fullctl-0.3.0/src/fullctl/django/rest/core.py` & `fullctl-1.2.0rc1/src/fullctl/django/rest/core.py`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/rest/decorators.py` & `fullctl-1.2.0rc1/src/fullctl/django/rest/decorators.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,35 @@
+from functools import wraps
+
 import reversion
 from django.conf import settings
+from django.contrib.auth import get_user_model
 from django_grainy.decorators import grainy_rest_viewset_response
 from rest_framework import exceptions
 from rest_framework.response import Response
 
-from fullctl.service_bridge.client import AaaCtl
 from fullctl.django.auth import Permissions, RemotePermissions
-from fullctl.django.models import Organization
+from fullctl.django.models import Instance, Organization
+from fullctl.django.rest.authentication import APIKey
 from fullctl.django.rest.core import HANDLEREF_FIELDS
+from fullctl.service_bridge.client import AaaCtl
+
+
+class base:
+    def load_org_instance(self, request, data):
+        data.update(org=request.org)
 
+        if isinstance(data.get("instance"), self.instance_class):
+            return
 
-class load_object:
+        instance, _ = self.instance_class.objects.get_or_create(org=request.org)
+        data.update(instance=instance, org=request.org)
+
+
+class load_object(base):
 
     """
     Will load an object and pass it to the view handler
     for `model` Model as argument `argname`
 
     **Arguments**
 
@@ -23,119 +38,200 @@
 
     **Keyword Arguments**
 
     Any keyword argument will be passed as a filter to the
     `get` query
     """
 
-    def __init__(self, argname, model, **filters):
+    def __init__(self, argname, model, instance_class=Instance, **filters):
         self.argname = argname
         self.model = model
         self.filters = filters
+        self.instance_class = instance_class
 
     def __call__(self, fn):
-
         decorator = self
 
         def wrapped(self, request, *args, **kwargs):
             filters = {}
+
+            decorator.load_org_instance(request, kwargs)
+
             for field, key in decorator.filters.items():
                 filters[field] = kwargs.get(key)
 
             try:
                 kwargs[decorator.argname] = decorator.model.objects.get(**filters)
             except decorator.model.DoesNotExist:
                 return Response(status=404)
+
             return fn(self, request, *args, **kwargs)
 
         wrapped.__name__ = fn.__name__
         return wrapped
 
 
-class grainy_endpoint:
+class grainy_endpoint_response(grainy_rest_viewset_response):
+
+    """
+    Override of grainy_rest_viewset_response so we can
+    toggle permission application to responses on or off
+    through our grainy_endpoint decorator
+    """
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+
+        self.enable_apply_perms = kwargs.pop("enable_apply_perms", True)
+
+    def apply_perms(self, request, response, view_function, view):
+        if self.enable_apply_perms:
+            return super().apply_perms(request, response, view_function, view)
+        return response
+
+
+class grainy_endpoint(base):
     def __init__(
         self,
         namespace=None,
         require_auth=True,
-        explicit=True,
+        explicit=False,
         instance_class=None,
         **kwargs,
     ):
         self.namespace = namespace or ["org", "{request.org.permission_id}"]
         self.require_auth = require_auth
         self.explicit = explicit
         self.instance_class = instance_class
+        self.enable_apply_perms = kwargs.pop("enable_apply_perms", True)
         self.kwargs = kwargs
 
     def __call__(self, fn):
         decorator = self
 
         if getattr(settings, "USE_LOCAL_PERMISSIONS", False):
             permissions_cls = Permissions
         else:
             permissions_cls = RemotePermissions
 
-        @grainy_rest_viewset_response(
+        @grainy_endpoint_response(
             namespace=decorator.namespace,
             namespace_instance=decorator.namespace,
             explicit=decorator.explicit,
             ignore_grant_all=True,
             permissions_cls=permissions_cls,
+            enable_apply_perms=decorator.enable_apply_perms,
             **decorator.kwargs,
         )
-        def wrapped(self, request, *args, **kwargs):
+        def inner(self, request, *args, **kwargs):
+            """
+            inner wrapper, called after grainy permissioning logic ran
+
+            handles auth requirement, loading of organization instance
+            and opening of reversion context
+            """
 
             if decorator.require_auth and not request.user.is_authenticated:
                 return Response(status=401)
 
             if decorator.instance_class:
-                instance, _ = decorator.instance_class.objects.get_or_create(
-                    org=request.org
-                )
-                kwargs.update(instance=instance)
+                decorator.load_org_instance(request, kwargs)
+
+            # if an api key is set, that should become the permission
+            # holder
+
+            if hasattr(request, "api_key"):
+                request.perms = permissions_cls(APIKey(request.api_key))
+
+            # check if the request is permissioned to access
+            # the fullctl service
+
+            if not request.perms.check(
+                f"service.{settings.SERVICE_TAG}.{request.org.permission_id}",
+                "r",
+                ignore_grant_all=True,
+            ):
+                return Response(status=403)
 
             with reversion.create_revision():
-                reversion.set_user(request.user)
-                return fn(self, request, org=request.org, *args, **kwargs)
+                if isinstance(request.user, get_user_model()):
+                    reversion.set_user(request.user)
+                else:
+                    reversion.set_comment(f"{request.user}")
 
-        wrapped.__name__ = fn.__name__
+                return fn(self, request, *args, **kwargs)
 
-        return wrapped
+        inner.__name__ = fn.__name__
+
+        @wraps(fn)
+        def outer(self, request, *args, **kwargs):
+            """
+            outer wrapper, called before grainy permissioning logic runs
+
+            handles superuser imitation for sufficiently provisioned api keys
+            """
+
+            as_user = request.headers.get("X-User")
+            if as_user and hasattr(request, "api_key"):
+                if permissions_cls(APIKey(request.api_key)).check(
+                    f"superuser.{as_user}", "c"
+                ):
+                    request.user = get_user_model().objects.get(
+                        social_auth__uid=as_user
+                    )
 
+            return inner(self, request, *args, **kwargs)
 
-class billable:
+        outer.__name__ = fn.__name__
+
+        return outer
+
+
+class _aaactl:
+    @property
+    def connected(self):
+        return getattr(settings, "AAACTL_URL", None) is not None
+
+    def bridge(self, org_slug):
+        return AaaCtl(settings.AAACTL_URL, settings.SERVICE_KEY, org_slug)
+
+
+class billable(_aaactl):
 
     """
     Will use the aaactl service bridge to determine
     if the specified product/service has accumulated
-    costs during the current subscription cycle and
+    costs during the current subscription subscription_cycle and
     return an error response if the there are costs
     but the organization has not yet set up billing
     """
 
     def __init__(self, product):
         self.product = product
 
     def __call__(self, fn):
-
         product = self.product
 
+        # if billing integration is disabled we just
+        # return the undecorated function
+
+        if not settings.BILLING_INTEGRATION:
+            return fn
+
         def wrapped(viewset, request, *args, **kwargs):
+            if not self.connected:
+                return fn(viewset, request, *args, **kwargs)
 
-            # TODO: use org keys once they are in
-            # for now grab the first api key of the requesting
-            # user
-            api_key = request.user.key_set.first().key
-            aaactl = AaaCtl(settings.AAACTL_HOST, api_key, request.org.slug)
+            aaactl = self.bridge(request.org.slug)
 
             if aaactl.requires_billing(product):
                 return Response(
                     {
                         "non_field_errors": [
-                            f"Billing setup required to continue using {product}. Please set up billing for your organization at {settings.AAACTL_HOST}/billing/setup?org={request.org.slug}"
+                            f"Billing setup required to continue using {product}. Please set up billing for your organization at {settings.AAACTL_URL}/billing/setup?org={request.org.slug}"
                         ]
                     },
                     status=403,
                 )
             return fn(viewset, request, *args, **kwargs)
 
         return wrapped
@@ -145,15 +241,17 @@
     class Serializers:
         pass
 
     def register(cls):
         if not hasattr(cls, "ref_tag"):
             cls.ref_tag = cls.Meta.model.HandleRef.tag
             cls.Meta.fields += ["grainy"] + HANDLEREF_FIELDS
-        setattr(Serializers, cls.ref_tag, cls)
+
+        ref_tag = cls.ref_tag.replace(".", "__")
+        setattr(Serializers, ref_tag, cls)
         return cls
 
     return (Serializers, register)
 
 
 def set_org(fn):
     def wrapped(self, request, pk, *args, **kwargs):
```

### Comparing `fullctl-0.3.0/src/fullctl/django/rest/renderers.py` & `fullctl-1.2.0rc1/src/fullctl/django/rest/renderers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime
 import json
 
-import django_countries
+import django_countries.fields
 from django.db import connection
 from django.utils.encoding import smart_text
 from rest_framework import renderers
 from rest_framework.utils import encoders
 
 
 class JSONEncoder(encoders.JSONEncoder):
@@ -39,16 +39,15 @@
     def render(self, data, media_type=None, renderer_context=None):
         status = renderer_context.get("response").status_code
 
         container = {"data": [], "errors": {}}
 
         # FIXME: should be a config value to disable/enable profile
         # info in the response data
-        if True:
-            container["profiling"] = {"queries": len(connection.queries)}
+        container["profiling"] = {"queries": len(connection.queries)}
 
         if status >= 400:
             container["errors"] = data
         else:
             if isinstance(data, dict):
                 container["data"].append(data)
             elif isinstance(data, list):
```

### Comparing `fullctl-0.3.0/src/fullctl/django/rest/serializers/__init__.py` & `fullctl-1.2.0rc1/src/fullctl/django/rest/serializers/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,24 +27,25 @@
         }
         valid = len(self.fields) != len(missing.keys())
         if not valid:
             raise ValidationError(missing)
 
 
 class ModelSerializer(serializers.ModelSerializer):
-    grainy = serializers.SerializerMethodField()
+    grainy = serializers.SerializerMethodField(help_text="Grainy permission namespace")
+
+    status = serializers.CharField(help_text="Object status", read_only=True)
 
     def get_grainy(self, obj):
         if hasattr(obj, "Grainy"):
             return obj.Grainy.namespace(obj)
         return None
 
 
 class RequireContext:
-
     required_context = []
 
     def validate(self, data):
         data = super().validate(data)
 
         for key in self.required_context:
             if key not in self.context:
```

### Comparing `fullctl-0.3.0/src/fullctl/django/rest/serializers/account.py` & `fullctl-1.2.0rc1/src/fullctl/django/rest/serializers/org.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,47 +4,26 @@
 from fullctl.django.rest.decorators import serializer_registry
 from fullctl.django.rest.serializers import ModelSerializer
 
 Serializers, register = serializer_registry()
 
 
 @register
-class Organization(ModelSerializer):
-    selected = serializers.SerializerMethodField()
+class OrganizationUser(ModelSerializer):
+    ref_tag = "org_user"
+
     name = serializers.SerializerMethodField()
-    access_type = serializers.SerializerMethodField()
+    email = serializers.SerializerMethodField()
+    you = serializers.SerializerMethodField()
 
     class Meta:
-        model = models.Organization
-        fields = ["slug", "name", "selected", "personal", "access_type"]
-
-    def get_access_type(self, obj):
-        user = self.context.get("user")
-        if user and not user.org_set.filter(org_id=obj.id).exists():
-            return "customer"
-        return "member"
-
-    def get_selected(self, obj):
-        org = self.context.get("org")
-        return obj == org
+        model = models.OrganizationUser
+        fields = ["id", "name", "email", "you"]
 
     def get_name(self, obj):
-        if obj.personal:
-            return "Personal"
-        return obj.name
-
-
-@register
-class ASN(serializers.Serializer):
+        return f"{obj.user.first_name} {obj.user.last_name}"
 
-    asn = serializers.IntegerField()
-    name = serializers.SerializerMethodField()
-
-    ref_tag = "asn"
+    def get_email(self, obj):
+        return obj.user.email
 
-    class Meta:
-        fields = ["asn", "name"]
-
-    def get_name(self, obj):
-        if obj["pdb_net"]:
-            return obj["pdb_net"].name
-        return ""
+    def get_you(self, obj):
+        return obj.user == self.context.get("user")
```

### Comparing `fullctl-0.3.0/src/fullctl/django/rest/serializers/org.py` & `fullctl-1.2.0rc1/src/fullctl/django/rest/serializers/meta.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 from rest_framework import serializers
 
-import fullctl.django.models as models
-from fullctl.django.rest.decorators import serializer_registry
 from fullctl.django.rest.serializers import ModelSerializer
 
-Serializers, register = serializer_registry()
 
+class Data(ModelSerializer):
+    ref_tag = "meta_data"
+    meta_source = None
 
-@register
-class OrganizationUser(ModelSerializer):
-    ref_tag = "orguser"
-
-    name = serializers.SerializerMethodField()
-    email = serializers.SerializerMethodField()
-    you = serializers.SerializerMethodField()
+    data = serializers.SerializerMethodField()
 
     class Meta:
-        model = models.OrganizationUser
-        fields = ["id", "name", "email", "you"]
+        fields = ["id", "data"]
+
+    def meta_data(self, obj, name, delete=True):
+        data = obj.data
+        val = data.get(name)
 
-    def get_name(self, obj):
-        return f"{obj.user.first_name} {obj.user.last_name}"
+        if delete and name in data:
+            data.pop(name)
 
-    def get_email(self, obj):
-        return obj.user.email
+        return val
 
-    def get_you(self, obj):
-        return obj.user == self.context.get("user")
+    def get_data(self, obj):
+        return obj.data
```

### Comparing `fullctl-0.3.0/src/fullctl/django/rest/urls/service_bridge.py` & `fullctl-1.2.0rc1/src/fullctl/django/rest/urls/service_bridge_proxy.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,71 +1,77 @@
 import json
+
 import requests
+from django.conf import settings
 from django.http import JsonResponse
 from django.urls import include, path
 
 PROXIED = {}
 
 
 def proxy_api(service, host, endpoints):
-
     """
     proxies a fullctl service's api with it's endpoints
     exposed to the local service's api 1:1
     """
 
     paths = [
-        proxy_api_endpoint(service, host, {"remote": remote, "local": local})
-        for remote, local in endpoints
+        proxy_api_endpoint(
+            service, host, {"remote": remote, "local": local, "name": name}
+        )
+        for remote, local, name in endpoints
     ]
 
     return include(paths)
 
 
 def proxy_api_endpoint(service, host, endpoint):
     def view_proxy(request, org_tag, *args, **kwargs):
-        api_key = request.user.key_set.first()
+        api_key = settings.SERVICE_KEY
         method = request.method.lower()
         request_fn = getattr(requests, method)
 
         # drf_request = Request(request, parsers=[JSONParser])
         _kwargs = {}
 
         if method in ["post", "put", "patch"]:
             _kwargs.update(json=json.loads(request.body))
 
-        print(_kwargs)
-
         endpoint_remote = endpoint["remote"].format(org_tag=org_tag, **kwargs)
 
         url = f"{host}/api/{endpoint_remote}"
 
-        response = request_fn(url, params={"key": api_key.key}, **_kwargs)
+        headers = {
+            "Authorization": f"Bearer {api_key}",
+            "X-User": request.user.social_auth.first().uid,
+        }
+
+        response = request_fn(url, headers=headers, **_kwargs)
         print("proxied response in", response.elapsed.total_seconds())
 
         json_dumps_params = {}
 
         if "pretty" in request.GET:
             json_dumps_params.update(indent=2)
 
         return JsonResponse(
             response.json(),
             status=response.status_code,
             json_dumps_params=json_dumps_params,
         )
 
     return path(
-        endpoint["local"], view_proxy, name=f"proxies-api-{service}-{endpoint['local']}"
+        endpoint["local"], view_proxy, name=f"proxies-api-{service}-{endpoint['name']}"
     )
 
 
 def setup(service, patterns):
-
     if service in PROXIED:
-        raise ValueError(f"Proxied api for service {service} already setup")
+        print(f"Proxied api for service {service} already setup")
+        return
 
     PROXIED[service] = patterns
 
 
 def urlpatterns(supported_services):
     urlpatterns = []
```

### Comparing `fullctl-0.3.0/src/fullctl/django/rest/views/account.py` & `fullctl-1.2.0rc1/src/fullctl/django/models/concrete/meta.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,84 @@
-from rest_framework import viewsets
-from rest_framework.decorators import action
-from rest_framework.response import Response
+"""
+Implements request and response models for universal non-specific
+requests and responses using the meta-data request caching system
+"""
+
+from django.db import models
+from django.utils.translation import gettext_lazy as _
+
+from fullctl.django.models.abstract.meta import Attachment as BaseAttachment
+from fullctl.django.models.abstract.meta import Request as BaseRequest
+from fullctl.django.models.abstract.meta import Response as BaseResponse
+
+__all__ = [
+    "Request",
+    "Response",
+    "Attachment",
+]
 
-import fullctl.django.models as models
-from fullctl.django.rest.decorators import grainy_endpoint
-from fullctl.django.rest.route.account import route
-from fullctl.django.rest.serializers.account import Serializers
-from fullctl.django.util import verified_asns
 
+class Request(BaseRequest):
+    """
+    request model
+    """
+
+    identifier = models.CharField(max_length=255, db_index=True)
+
+    class Meta:
+        db_table = "request"
+        verbose_name = _("Request")
+        verbose_name_plural = _("Requests")
+
+    class HandleRef:
+        tag = "request"
 
-@route
-class Organization(viewsets.GenericViewSet):
+    class Config:
+        source_name = "generic"
+        cache_expiry = 86400
+        target_field = "identifier"
 
+
+class Response(BaseResponse):
     """
-    Manage user's organizations
+    response model
     """
 
-    serializer_class = Serializers.org
-    queryset = models.Organization.objects.all()
+    request = models.OneToOneField(
+        Request,
+        on_delete=models.CASCADE,
+        related_name="response",
+    )
+
+    class Meta:
+        db_table = "meta_response"
+        verbose_name = _("Response")
+        verbose_name_plural = _("Responses")
+
+    class HandleRef:
+        tag = "response"
+
+    class Config:
+        meta_data_cls = None
+        attachment_cls = None
+
 
-    def list(self, request, *args, **kwargs):
+class Attachment(BaseAttachment):
 
-        """
-        list the organizations that the user belongs
-        to or has permissions to
-        """
+    """
+    file attachment model
+    """
 
-        serializer = Serializers.org(
-            instance=models.Organization.accessible(request.user),
-            many=True,
-            context={"user": request.user},
-        )
-        return Response(serializer.data)
+    response = models.ForeignKey(
+        Response, on_delete=models.CASCADE, related_name="attachments"
+    )
 
+    class Meta:
+        db_table = "meta_attachment"
+        verbose_name = _("Attachment")
+        verbose_name_plural = _("Attachments")
 
-@route
-class User(viewsets.GenericViewSet):
+    class HandleRef:
+        tag = "attachment"
 
-    ref_tag = "user"
-    serializer_class = Serializers.asn
 
-    @action(detail=False, methods=["GET"])
-    @grainy_endpoint()
-    def asns(self, request, org, *args, **kwargs):
-        serializer = Serializers.asn(verified_asns(request.perms), many=True)
-        return Response(serializer.data)
+Response.Config.attachment_cls = Attachment
```

### Comparing `fullctl-0.3.0/src/fullctl/django/rest/views/usage.py` & `fullctl-1.2.0rc1/src/fullctl/django/rest/views/usage.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,41 @@
 import datetime
 
 from rest_framework import viewsets
 from rest_framework.response import Response
 
 import fullctl.django.models as models
-from fullctl.django.rest.serializers.usage import Serializers
-from fullctl.django.rest.route.usage import route
 from fullctl.django.rest.decorators import grainy_endpoint
-from fullctl.django.rest.mixins import OrgQuerysetMixin, CachedObjectMixin
+from fullctl.django.rest.mixins import CachedObjectMixin, OrgQuerysetMixin
+from fullctl.django.rest.route.usage import route
+from fullctl.django.rest.serializers.usage import Serializers
 from fullctl.django.rest.usage import REGISTERED
 
 
 @route
 class Usage(CachedObjectMixin, OrgQuerysetMixin, viewsets.GenericViewSet):
-
-    """
-    Manage user's organizations
-    """
-
     serializer_class = Serializers.usage
     queryset = models.Organization.objects.all()
 
     ref_tag = "usage"
 
     @grainy_endpoint("billing.{request.org.permission_id}")
-    def list(self, request, org, *args, **kwargs):
-
+    def list(self, request, *args, **kwargs):
         """
-        list the organizations that the user belongs
-        to or has permissions to
+        List organization's usage for metered apis
         """
 
         data = []
 
         # TODO: support ranges eventually
         start = datetime.datetime.now()
         end = datetime.datetime.now()
 
+        org = request.org
+
         for metric_cls in REGISTERED.values():
             metric = metric_cls(org)
             data.append(
                 {
                     "name": metric.Meta.name,
                     "units": metric.calc(start, end),
                     "start": start,
```

### Comparing `fullctl-0.3.0/src/fullctl/django/social/backends/peeringdb.py` & `fullctl-1.2.0rc1/src/fullctl/django/social/backends/peeringdb.py`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/social/backends/twentyc.py` & `fullctl-1.2.0rc1/src/fullctl/django/social/backends/twentyc.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,18 +18,20 @@
 
     def get_user_details(self, response):
         """Return user details."""
         if response.get("verified_user") is not True:
             raise AuthFailed(self, "User is not verified")
 
         return {
-            "username": response.get("given_name"),
+            "username": response.get("user_name"),
             "email": response.get("email") or "",
             "first_name": response.get("given_name"),
             "last_name": response.get("family_name"),
+            "is_superuser": response.get("is_superuser"),
+            "is_staff": response.get("is_staff"),
         }
 
     def user_data(self, access_token, *args, **kwargs):
         """Load user data from service."""
         headers = {"Authorization": "Bearer %s" % access_token}
         data = self.get_json(self.PROFILE_URL, headers=headers)
         return data
```

### Comparing `fullctl-0.3.0/src/fullctl/django/static/common/20c/twentyc.core.min.js` & `fullctl-1.2.0rc1/src/fullctl/django/static/common/20c/twentyc.core.min.js`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/static/common/20c-logo-filled.svg` & `fullctl-1.2.0rc1/src/fullctl/django/static/common/20c-logo-filled.svg`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/static/common/app.css` & `fullctl-1.2.0rc1/src/fullctl/django/static/common/app.css`

 * *Files 26% similar despite different names*

```diff
@@ -9,46 +9,117 @@
 a[data-action],
 .action {
   cursor: pointer;
 }
 
 a[data-action]:hover,
 .action:hover {
+}
+
+body {
+  overflow: scroll;
+}
+
+button {
+  border: none;
+  font-family: "Archivo Narrow";
+  font-size: 16px;
+  letter-spacing: 0;
+  line-height: 16px;
+  text-transform: capitalize;
   text-decoration: none;
+  text-align: left;
+}
+
+button span.label {
+  text-decoration: underline;
+}
+
+
+[data-api-submit] {
+  position: relative;
 }
 
+button:focus {
+  outline: none;
+}
 
 .loading-shim {
   position: absolute;
   top: 0px;
   left: 0px;
   bottom: 0px;
   right: 0px;
   z-index: 10;
 }
 
 .nowrap {
   white-space: nowrap;
 }
 
+.center {
+  text-align: center;
+}
+
 .right {
   text-align: right;
 }
 
 .bold {
   font-weight: bold;
 }
 
 .sortable-button {
   cursor: pointer;
 }
-a{
+
+.rounded-button {
+  border-radius: 50px;
+  padding: 12px 16px;
+}
+
+.small-info {
+  font-size: 12px;
+}
+
+.m-info {
+  font-size: 14px;
+}
+
+.ux-keep-list-open {
+  margin-right: 4px;
+}
+
+a,
+a:hover {
+  text-decoration: underline;
+}
+
+a.a-button {
+  text-decoration: none;
+}
+
+a.a-button:hover {
+  text-decoration: none;
+}
+
+
+a.button span.label{
+  text-decoration: underline;
+}
+
+a.button span.label.no-text-deco{
+  text-decoration: none;
+}
+
+a.button span.label:hover {
   text-decoration: underline;
 }
 
+
 button {
   cursor: pointer;
 }
 
 @media (min-width: 1900px) {
   .container {
       max-width: 1400px;
@@ -78,27 +149,52 @@
 }
 
 div.validation-error p {
   font-size: 14px;
   margin: 0px;
 }
 
+div.loading-anim {
+  text-align: center;
+  padding: 8px;
+}
+
 .marg-top-lg {
-  margin-top: 30px;
+  margin-top: 24px;
 }
 
 .marg-bot-sm {
   margin-bottom: 5px;
 }
 
 .marg-sm {
   margin-top: 5px;
   margin-bottom: 5px;
 }
 
+.pad-top-lg {
+  padding-top: 24px;
+}
+
+.pad-top-9 {
+  padding-top: 9px;
+}
+
+.tool-spacing-left {
+  margin-left: 8px;
+}
+
+.indent {
+  padding-left: 20px;
+}
+
+.indent-on .indent-toggled {
+  padding-left: 20px;
+}
+
 /**
  * page
  */
 
 body {
   font-family: "Archivo Narrow";
   letter-spacing: 0;
@@ -106,15 +202,15 @@
 
 /**
  * header
  */
 
 
 div.header {
-
+  min-height: 69px;
 }
 
 div.header-left {
 }
 
 div.header-left a {
   line-height: 24px;
@@ -194,14 +290,21 @@
   height: 28px;
   border-radius: 25px;
   position: absolute;
   left: 2px;
   top: 2px;
 }
 
+div.header span.header-control span.icon > span.inner-icon {
+  top: 8px;
+  left: -2px;
+  position: relative;
+}
+
+div.header span.header-control span.icon > span.inner-icon,
 div.header span.header-control span.icon > img {
   display: inline-block;
   padding: 7px;
 }
 
 
 div.header span.header-control .dropdown-item {
@@ -251,14 +354,20 @@
   font-family: "Archivo Narrow";
   font-size: 16px;
   letter-spacing: 0;
   line-height: 24px;
   padding-left: 10px;
 }
 
+div.dropdown-meny.show,
+span.header-control.show,
+span.dropdown.show {
+  display: inline-block !important;
+}
+
 div.header span.header-control .dropdown-item:hover {
   text-decoration: underline;
 }
 
 div.header span.header-control .dropdown-item span.icon {
   height: 16px;
   width: 16px;
@@ -302,15 +411,15 @@
 }
 
 div.header .app-switcher .selected {
   padding-top: 18px;
   padding-bottom: 9px;
   padding-left: 15px;
   padding-right: 28px;
-  width: 210px;
+  width: 220px;
   display: inline-block;
   cursor: pointer;
   position: relative;
 }
 
 div.header .app-switcher .selected .icon-caret-down {
   display: inline-block;
@@ -343,57 +452,171 @@
 div.toolbar {
   padding-top: 24px;
   padding-bottom: 24px;
   font-size: 20px;
   line-height: 24px;
 }
 
+input.slim {
+  width: 75px;
+}
+
+.list-body .secondary div.row:first-child {
+  margin-top: 0px;
+}
+
+.list-body .secondary div.row:not(:first-child) {
+  margin-top: 3px;
+}
+
+.list-body label {
+  font-size: 11px;
+  margin:0px;
+}
+
+
+.list-body + .list-no-data {
+  display: none;
+}
+
+.list-body:empty + .list-no-data {
+  display: block;
+  text-align: center;
+  padding: 8px;
+}
+
+tbody.list-body:empty + tbody.list-no-data {
+  display: table-row-group;
+  text-align: center;
+}
+
+
+.list-body td input.slim,
+.list-body div.secondary input[type="text"],
+div.toolbar-field input[type="text"] {
+  border: 1px solid;
+  font-family: "Archivo Narrow";
+  font-size: 16px;
+  letter-spacing: 0;
+  line-height: 20px;
+  padding: 2px 2px 2px 8px;
+}
+
+.list-body .secondary select,
+div.toolbar-field select,
+div.toolbar input[type=text],
+.select2-container--default .select2-selection--single,
 div.toolbar select {
   border: none;
+  border-radius: 0px;
+}
+.select2-container--default .select2-selection--single,
+div.toolbar select {
   font-size: 20px;
   font-weight: bold;
-  border-radius: 0px;
   line-height: 24px;
   padding: 8px 48px 8px 8px;
   -webkit-appearance: none;
   -moz-appearance: none;
   appearance: none;
   margin-left: 16px;
 }
 
+
+div.toolbar .select2-container .select2-selection--single {
+  height: 35px;
+}
+
+div.toolbar input[type=text] {
+  margin: 7px;
+}
+
+div.toolbar div.toolbar-control-group {
+  display: inline-block;
+  padding-left: 8px;
+}
+
 div.toolbar span.toolbar-control {
   position: relative;
   display: inline-block;
 }
 
 div.toolbar span.toolbar-control > img.caret {
   position: absolute;
   right: 18px;
   top: 19px;
 }
 
+div.toolbar-field {
+  position: relative;
+  font-family: "Archivo Narrow";
+  font-size: 16px;
+  letter-spacing: 0;
+  line-height: 20px;
+  display: inline;
+  margin-left: 1px;
+  padding: 8px;
+}
+
+div.toolbar-field > span.icon {
+  background-color: #fff;
+  position: absolute;
+  z-index: 1;
+  right: 14px;
+  top: 10px;
+}
+
+div.toolbar-field > span.value {
+  font-family: "Archivo Narrow";
+  font-size: 16px;
+  font-weight: bold;
+  letter-spacing: 0;
+  line-height: 20px;
+}
+
+
 
 div.menu .button {
   display: block;
-  margin-bottom: 5px;
   width: 100%;
-  text-align: center;
+  border: none;
+  font-family: "Archivo Narrow";
+  font-size: 16px;
+  letter-spacing: 0;
+  line-height: 16px;
+  text-transform: capitalize;
   text-decoration: none;
+  text-align: left;
+  margin: 4px 0px;
+}
+
+div.menu .button:hover {
+  text-decoration: none;
+}
+
+div.menu .button span.label {
+  text-decoration: underline;
+}
+
+.shift-down .menu-deco-border {
+  margin-top: 55px;
+}
+
+.shift-down .menu .section {
+  padding-top: 55px;
 }
 
-div.menu .button,
 div.toolbar .button {
   border: none;
   border-radius: 25px;
-  padding: 12px 18px 12px 18px;
   font-size: 16px;
   line-height: 16px;
   border: none;
-  :0
   outline: none;
+  text-align: left;
 }
 
 div.menu .button .icon,
 div.toolbar .button .icon {
   width: 16px;
   height: 16px;
   vertical-align: bottom;
@@ -404,28 +627,50 @@
 }
 
 div.menu div.section.tabs h5.active {
   cursor: default;
   text-decoration: underline;
 }
 
+div.tool-custom {
+  padding-left: 15px;
+}
+
+
+div.tool-custom > h4.tool-title {
+  font-family: "Archivo Narrow";
+  font-size: 30px;
+  letter-spacing: 0;
+  line-height: 30px;
+  margin-top: 24px;
+  font-weight: 400;
+  border-bottom: 2px solid transparent;
+}
+
 /**
  * icons
  */
 
+span.inner-icon,
 span.icon {
   display: inline-block;
   height: 16px;
   width: 16px;
   vertical-align: bottom;
   margin-right: 3px;
+  mask-position: center;
+  -webkit-mask-position: center;
   mask-repeat: no-repeat;
   -webkit-mask-repeat: no-repeat;
 }
 
+span.icon-right {
+  margin-left: 3px;
+}
+
 .inner-list span.icon {
 }
 
 span.icon-add {
   -webkit-mask-image: url(icons/icon/add.svg);
   mask-image: url(icons/icon/add.svg);
 }
@@ -438,38 +683,79 @@
   -webkit-mask-image: url(icons/icon/edit.svg);
   mask-image: url(icons/icon/edit.svg);
 }
 span.icon-logout {
   -webkit-mask-image: url(icons/icon/logout.svg);
   mask-image: url(icons/icon/logout.svg);
 }
+span.icon-location {
+  -webkit-mask-image: url(icons/icon/location.svg);
+  mask-image: url(icons/icon/location.svg);
+}
 span.icon-settings {
   -webkit-mask-image: url(icons/icon/settings.svg);
   mask-image: url(icons/icon/settings.svg);
 }
 
 span.icon-list {
   -webkit-mask-image: url(icons/icon/list.svg);
   mask-image: url(icons/icon/list.svg);
 }
 
+span.icon-api {
+  -webkit-mask-image: url(icons/icon/api.svg);
+  mask-image: url(icons/icon/api.svg);
+}
+
+span.icon-report {
+  -webkit-mask-image: url(icons/icon/report.svg);
+  mask-image: url(icons/icon/report.svg);
+}
+
+span.icon-refresh {
+  -webkit-mask-image: url(icons/icon/refresh.svg);
+  mask-image: url(icons/icon/refresh.svg);
+}
+
 span.icon-download {
   -webkit-mask-image: url(icons/icon/logout.svg);
   mask-image: url(icons/icon/logout.svg);
   transform: rotate(-90deg);
 }
 span.icon-org {
   -webkit-mask-image: url(icons/icon/org.svg);
   mask-image: url(icons/icon/org.svg);
 }
+
+span.icon-launch {
+  -webkit-mask-image: url(icons/icon/launch.svg);
+  mask-image: url(icons/icon/launch.svg);
+}
+span.icon-mail {
+  -webkit-mask-image: url(icons/icon/mail.svg);
+  mask-image: url(icons/icon/mail.svg);
+}
+span.icon-view {
+  -webkit-mask-image: url(icons/icon/view.svg);
+  mask-image: url(icons/icon/view.svg);
+}
+
+
+
 span.icon-caret-down {
   -webkit-mask-image: url(icons/ui-caret-caret/down.svg);
   mask-image: url(icons/ui-caret-caret/down.svg);
 }
 
+span.icon-caret-left {
+  -webkit-mask-image: url(icons/ui-caret-caret/down.svg);
+  mask-image: url(icons/ui-caret-caret/down.svg);
+  transform: rotate(-90deg);
+}
+
 
 img.icon.filled {
   border-radius: 25px;
   padding: 2px;
 }
 
 img.icon {
@@ -485,19 +771,37 @@
 }
 
 .checked [data-true] {
   display: inline;
 }
 
 /**
+ * nav
+ */
+
+a.nav-link {
+  font-family: "Archivo Narrow";
+  font-size: 20px;
+  font-weight: 500;
+  letter-spacing: 0;
+  line-height: 24px;
+  text-decoration: none;
+  padding: 12px 0px;
+  margin: 0px 12px -20px 12px;
+}
+
+a.nav-link.active {
+  border-bottom: 2px solid;
+}
+
+/**
  * menu
  */
 
 div.menu {
-  margin-top: 54px;
   position: relative;
 }
 
 
 div.menu h4 {
   font-family: "Archivo Narrow";
   font-size: 30px;
@@ -507,37 +811,58 @@
   font-weight: 400;
 }
 
 div.menu div.menu-deco-border {
   position: absolute;
   height: 2px;
   left: 15px;
-  right: -15px;
+  right: -12px;
   z-index: 10;
   top: 0px;
 }
 
 div.menu .button {
   margin-bottom: 8px;
 }
 
 /**
  * content
  */
 
+.main[data-component="main"] {
+  margin-top: 54px;
+}
+
+div.list-th,
+table thead tr th {
+  opacity: 0.4;
+}
+
+div.list-th,
+.table.list-table  {
+  border-top: 2px solid #9da2a7;
+}
+
+div.list-th,
 .table th {
   font-size: 15px;
   letter-spacing: 3px;
   line-height: 30px;
   text-transform: uppercase;
 }
 
 .table td,
 .table th {
   border-top: none;
+  padding: 12px;
+}
+
+.table th {
+  vertical-align: bottom;
+  border-bottom: 2px solid #dee2e6;
 }
 
 .tool {
   position: relative;
 }
 
 .table td.highlight {
@@ -545,14 +870,15 @@
 }
 
 .table td {
   font-size: 16px;
   line-height: 16px;
 }
 
+.list-body div.secondary,
 .table tr.secondary {
   border-bottom: 1px transparent solid;
 }
 
 .table td[data-field="controls"] a {
   white-space: nowrap;
 }
@@ -567,29 +893,61 @@
 }
 
 @media (min-width: 767.98px) {
 .table tr.secondary td.property div.field {
   --margin-top: -12px;
   --margin-bottom: -12px;
 }
+
+.marg-top-xl {
+  margin-top: 55px;
+}
+
 td.property {
   padding: 0px 15px;
 }
 }
 
 .secondary .property .field,
 .secondary .property .field-empty,
 .table tr.secondary td.property div.field {
   padding-top: 12px;
   padding-bottom: 11px;
   border-left: 1px transparent solid;
 }
 
+div.list-body .secondary .property {
+  margin-left: calc(var(--bs-gutter-x) * -0.5);
+}
+
+div.list-body .secondary .property .transparent-field,
+div.list-body .secondary .property .field {
+  padding: 8px;
+  min-height: 42px;
+  display: inline-block;
+}
+
+div.list-body .secondary .property [data-field] {
+  margin-left: 4px;
+}
+
+div.list-body .secondary button {
+}
+
+.row-gap button {
+  font-family: "Archivo Narrow";
+  font-size: 16px;
+  font-weight: bold;
+  letter-spacing: 0;
+  line-height: 20px;
+  text-decoration: none;
+}
+
 tr.secondary > td {
-  padding: 0px 15px;
+  padding: 0px calc(var(--bs-gutter-x) * .5);
 }
 
 .row.double-row > div.field > span {
   display: block;
 }
 
 .row.double-row > div.field > span:nth-child(2) {
@@ -612,23 +970,36 @@
   padding-right: .75rem;
 }
 
 div.list-body > div.row {
   margin-top: 5px;
 }
 
+div.list-body div.secondary {
+  margin-left: 0px;
+}
+
+div.list-body .primary-row-name {
+  font-family: "Archivo Narrow";
+  font-size: 20px;
+  font-weight: bold;
+  letter-spacing: 0;
+  line-height: 24px;
+  margin: 16px 0px 16px 8px;
+}
+
 tbody.list-footer {
   border-top: 1px solid transparent !important;
 }
 
 tbody.list-footer td {
   text-align: center;
 }
 
-tbody.list-footer button {
+tbody.list-footer button:not(.rounded-button)1 {
   text-decoration: underline;
 }
 
 div.column-list-3 {
   column-count: 3;
 }
 
@@ -637,14 +1008,15 @@
 }
 
 
 td.inner-list-container {
   padding-left: 0px;
   padding-right: 0px;
   padding-bottom: 0px;
+  padding-top: 0px;
 }
 
 
 div.inner-list-head {
   margin-top: -1rem;
   padding: 8px;
 }
@@ -656,65 +1028,102 @@
   text-transform: uppercase;
 }
 
 div.inner-list > div {
   padding: 3px 0px;
 }
 
+.inner-list-2 {
+  border-top: 1px solid;
+}
+
+
+.prelist {
+  border-bottom: none !important;
+  border-left: 16px solid;
+}
+
+.prelist div.prefix-container {
+  padding: 4px 8px;
+  margin: 0 32px;
+}
+
+.prefix-container {
+  background: #0F1317;
+  position: relative;
+}
+
+.prefix-container a,
+.prefix-container span {
+  display: inline-block;
+}
+
+.prefix {
+  text-decoration: underline;
+}
+
 td div.controls div.alert {
   margin: 0px;
 }
 
 td div.controls  {
   padding: 5px;
 }
 
+td div.controls .label {
+  padding: 5px;
+}
+
+.underline {
+  text-decoration: underline;
+}
+
 div.flags > span {
   margin: 5px;
   display: inline-block;
 }
 
 
 /**
  * Table headings (ordering)
  */
 
 .selected-order-header-asc {
-  color: #0099FF;
-  opacity: 1;
 }
 .selected-order-header-asc::after {
   content: " \2191";
 }
 
 .selected-order-header-desc {
-  color: #0099FF;
-  opacity: 1;
 }
 
 .selected-order-header-desc::after {
   content: " \2193";
 }
 
 /**
  * modal
  */
 
+@media (min-width: 1100px) {
+  .modal-xl {
+    max-width: 1200px;
+  }
+}
+
 h5.modal-title {
   font-family: "Archivo Narrow";
   font-size: 24px;
   font-weight: 500;
   letter-spacing: 0;
   line-height: 26px;
 }
 
-button.close {
+button.btn-close {
   text-shadow: none;
-  position: relative;
-  top: -40px;
   opacity: 1;
 }
 
 div.controls button.generic,
 div.controls button.submit,
 div.modal button.submit {
   border-radius: 20px;
@@ -769,15 +1178,17 @@
 div.controls input[type="password"]:disabled,
 div.controls select:disabled {
   padding: 0px;
 }
 
 
 div.controls input[type="text"],
-div.controls input[type="password"] {
+div.controls input[type="text"]:disabled,
+div.controls input[type="password"],
+div.controls input[type="password"]:disabled {
   padding: 6px 8px;
   height: auto;
 }
 
 div.controls textarea {
   padding: 6px 8px;
 }
@@ -814,20 +1225,22 @@
 div.controls input[type="checkbox"] ~ label {
   font-family: "Archivo Narrow";
   font-size: 20px;
   letter-spacing: 0;
   line-height: 24px;
 }
 
-div.modal span.modal-control {
+span.modal-control {
   position: relative;
   display: block;
 }
 
-div.modal span.modal-control > img.caret {
+
+
+span.modal-control > img.caret {
   position: absolute;
   right: 18px;
   top: 19px;
 }
 
 
 
@@ -838,57 +1251,124 @@
 
 .input-group .select2-selection__rendered {
   padding-left: 10px !important;
   line-height: 25px !important;
 }
 
 /*
+ * status badge
+ */
+
+span.status-badge {
+  padding: 0px 5px;
+  border: 1px solid;
+  border-radius: 3px;
+  font-size: 13px;
+  text-transform: capitalize;
+}
+
+span.status-badge div.spinner {
+  padding-top: 2px;
+}
+
+.prefix-rep,
+.rep-status {
+  text-transform: uppercase;
+}
+
+.inline-addon-control,
+.prefix-rep {
+  padding: 4px;
+  border-radius: 5px;
+  display: inline-block;
+}
+
+
+.capitalize {
+  text-transform: capitalize;
+}
+
+/*
  * oauth
  */
 
 .btn-oauth {
   width: 210px;
 }
 
-div.oauth-backend.twentyc > a.btn {
-  background-color: #191919;
-  border-color: #0f1419;
-}
-
 img.login-twentyc,
 img.login-peeringdb {
   height: 40px;
 }
 
 img.login-google {
   width: 40px;
 }
 
 
-
+textarea.template-editor {
+  height: 300px;
+}
 
 
 /**
  * footer
  */
 
 div.app-footer {
+  margin-top: 100px;
   text-align: center;
 }
 
 
-/**
- * login
+/*
+ * error page
  */
 
-div.login button {
-  color: #0099ff;
-  background-color: #000;
+div.page_error {
+  text-align: center;
+  margin: 50px;
 }
 
-div.login input {
-  background-color: #3C4650;
-  color: #fff;
+
+
+div.create .edit-toggled {
+  display: none;
 }
 
 
+/*
+ * wizard
+ */
+
+
+div.wizard .wiz-step {
+  display: none;
+}
 
+div.wizard.wiz-step-6 .wiz-step.wiz-step-6,
+div.wizard.wiz-step-5 .wiz-step.wiz-step-5,
+div.wizard.wiz-step-4 .wiz-step.wiz-step-4,
+div.wizard.wiz-step-3 .wiz-step.wiz-step-3,
+div.wizard.wiz-step-2 .wiz-step.wiz-step-2,
+div.wizard.wiz-step-1 .wiz-step.wiz-step-1{
+  display: block;
+}
+
+/*
+ * tags
+ */
+
+span.tag {
+  padding: 3px 5px;
+  margin-right: 10px;
+  border-radius: 5px;
+  font-size: 12px;
+}
+
+span.tag-name {
+  font-weight: 600;
+}
+
+span.tag-value {
+  margin-left: 10px;
+}
```

### Comparing `fullctl-0.3.0/src/fullctl/django/static/common/icons/Indicator/Check-Ind/Check.svg` & `fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/Indicator/Check-Ind/Check.svg`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/static/common/icons/Indicator/X-Ind/X.svg` & `fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/Indicator/X-Ind/X.svg`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/static/common/icons/icon/add.svg` & `fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/icon/add.svg`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/static/common/icons/icon/alerts.svg` & `fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/icon/alerts.svg`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/static/common/icons/icon/dark-mode.svg` & `fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/icon/dark-mode.svg`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/static/common/icons/icon/delete.svg` & `fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/icon/delete.svg`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/static/common/icons/icon/edit.svg` & `fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/icon/edit.svg`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/static/common/icons/icon/light-mode.svg` & `fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/icon/light-mode.svg`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/static/common/icons/icon/list.svg` & `fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/icon/list.svg`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/static/common/icons/icon/logout.svg` & `fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/icon/logout.svg`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/static/common/icons/icon/org.svg` & `fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/icon/org.svg`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/static/common/icons/icon/settings.svg` & `fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/icon/settings.svg`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/static/common/icons/icon/user.svg` & `fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/icon/user.svg`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/static/common/icons/ixctl-logo-darkbg.svg` & `fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/ixctl-logo-darkbg.svg`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/static/common/icons/prefixctl-logo-darkbg.svg` & `fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/prefixctl-logo-darkbg.svg`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/static/common/icons/ui-caret-caret/down.svg` & `fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/ui-caret-caret/down.svg`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/static/common/icons/ui-close.svg` & `fullctl-1.2.0rc1/src/fullctl/django/static/common/icons/ui-close.svg`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/static/common/oauth/20c.svg` & `fullctl-1.2.0rc1/src/fullctl/django/static/common/oauth/20c.svg`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/static/common/oauth/google.svg` & `fullctl-1.2.0rc1/src/fullctl/django/static/common/oauth/google.svg`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/static/common/oauth/peeringdb.png` & `fullctl-1.2.0rc1/src/fullctl/django/static/common/oauth/peeringdb.png`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/static/common/service_bridge.js` & `fullctl-1.2.0rc1/src/fullctl/django/static/common/service_bridge.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -133,16 +133,15 @@
              * determine if the org has costs in a products current
              * subscription cycle
              *
              * `callback` will be called if yes
              */
 
             has_service_costs: function(product, callback) {
-                var j, item, org = this.org(),
-                    status = {};
+                var j, item, org = this.org();
 
                 return this.get(`billing/${org}/services/`).then((response) => {
                     response.rows((row, i) => {
                         for (j = 0; j < row.items.length; j++) {
                             item = row.items[j];
                             if (item.name.toLowerCase() == product.toLowerCase()) {
                                 return callback(item.cost > 0, item, row);
```

### Comparing `fullctl-0.3.0/src/fullctl/django/tasks.py` & `fullctl-1.2.0rc1/src/fullctl/django/tasks/celery.py`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/templates/common/apidocs/redoc.html` & `fullctl-1.2.0rc1/src/fullctl/django/templates/common/apidocs/redoc.html`

 * *Files 27% similar despite different names*

```diff
@@ -12,11 +12,11 @@
       body {
         margin: 0;
         padding: 0;
       }
     </style>
   </head>
   <body>
-    <redoc spec-url='{% static "docs/openapi.yaml" %}'></redoc>
+    <redoc spec-url='{% url "api_schema" %}'></redoc>
     <script src="https://cdn.jsdelivr.net/npm/redoc@next/bundles/redoc.standalone.js"> </script>
   </body>
 </html>
```

### Comparing `fullctl-0.3.0/src/fullctl/django/templates/common/apidocs/swagger.html` & `fullctl-1.2.0rc1/src/fullctl/django/templates/common/apidocs/swagger.html`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     <link rel="stylesheet" type="text/css" href="//unpkg.com/swagger-ui-dist@3/swagger-ui.css" />
   </head>
   <body>
     <div id="swagger-ui"></div>
     <script src="//unpkg.com/swagger-ui-dist@3/swagger-ui-bundle.js"></script>
     <script>
     const ui = SwaggerUIBundle({
-        url: "{% static "docs/openapi.yaml" %}",
+        url: "{% url "api_schema" %}",
         dom_id: '#swagger-ui',
         presets: [
           SwaggerUIBundle.presets.apis,
           SwaggerUIBundle.SwaggerUIStandalonePreset
         ],
         layout: "BaseLayout",
         requestInterceptor: (request) => {
```

### Comparing `fullctl-0.3.0/src/fullctl/django/templates/common/app/base.html` & `fullctl-1.2.0rc1/src/fullctl/django/templates/common/app/base.html`

 * *Files 12% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 <script src="{% static "autocomplete_light/jquery.post-setup.js" %}" type="text/javascript"></script>
 <script src="{% static "common/app.js" %}" type="text/javascript"></script>
 <script src="{% static "common/service_bridge.js" %}" type="text/javascript"></script>
 {% endblock %}
 
 {% block "css" %}
 {{ block.super }}
-<link rel="stylesheet" type="text/css" href="{% static "common/app.css" %}" />
-<link rel="stylesheet" type="text/css" href="{% static "common/themes/dark.css" %}" />
+<link rel="stylesheet" type="text/css" href="{% static "common/app.css" %}?v=041208" />
+<link rel="stylesheet" type="text/css" href="{% static "common/themes/dark.css" %}?v=030802" />
 <link rel="stylesheet" type="text/css" href="{% static "admin/css/vendor/select2/select2.css" %}" />
 <link rel="stylesheet" type="text/css" href="{% static "admin/css/autocomplete.css" %}" />
 <link rel="stylesheet" type="text/css" href="{% static "autocomplete_light/select2.css" %}" />
 <link href="https://fonts.googleapis.com/css2?family=Archivo+Narrow:wght@400;500;600;700&display=swap" rel="stylesheet">
 
 {% endblock %}
 
@@ -31,50 +31,99 @@
 fullctl.user = {
   id : {{ request.user.id }},
   email : "{{ request.user.email }}",
   username : "{{ request.user.username }}"
 }
 
 fullctl.org = {
+  id : {{ request.org.permission_id }},
   slug : "{{ request.org.slug }}",
   name : "{{ request.org.name }}"
 }
 
 fullctl.aaactl_urls = {{ account_service.urls|safe }}
 
 var True = true, False = false;
 
 fullctl.permissions = {{ permissions|safe }}
 </script>
 
 {% block "header" %}
+
 <div class="container-fluid header-outer">
   <div class="top-border {{ request.app_id }} app_bg"></div>
+
+  {% if request.impersonating %}
+  <div class="row">
+    <div class="col-12 col-sm-2"></div>
+    <div class="col-12 col-sm-8">
+      <div class="alert alert-info center">
+      {% blocktrans with user=request.user logged_in_user=request.impersonating.superuser %}
+      You are currently impersonating <b>{{ user }}</b> - logged in as <b>{{ logged_in_user }}</b>
+      {% endblocktrans %}
+      </div>
+    </div>
+    <div class="col-12 col-sm-2"></div>
+  </div>
+  {% endif %}
+
+
   <div class="row header" data-component="header">
-    <div class="col-12 col-sm-6  header-left">
+
+    <!-- logo and app switcher -->
+
+    <div class="col-12 col-sm-4 header-left">
+      {% block "header_left" %}
       <div class="app-switcher" data-element="app_switcher">
         <div class="selected {{ request.app_id }}">
           <img class="app-logo" src="{% static service_logo_dark %}" alt="{{ service_tag }}">
         <span class="icon {{ request.app_id }} icon-caret-down"></span>
         <div class="others" style="display:none">
+          {% for service_app in service_applications %}
+          {%   if service_app.slug != service_tag %}
+          {%     with "common/logos/"|add:service_app.slug|add:"-dark.svg" as other_app_logo %}
+            <a data-grainy-remove="{{ service_app.grainy }}.{{ request.org.remote_id}}" href="{{ service_app.org_redirect }}">
+              {% if not service_app.logo %}
+                <img class="app-logo" src="{% static other_app_logo %}" alt="{{ service_app.slug }}">
+              {% else %}
+                <img class="app-logo" src="{{ service_app.logo }}" alt="{{ service_app.slug }}">
+              {% endif %}
+            </a>
+          {%     endwith %}
+          {%   endif %}
+          {% endfor %}
+
         </div>
         </div>
       </div>
+      {% endblock "header_left" %}
+    </div>
+
+    <!-- /logo and app switcher -->
+
+    <!-- pages -->
+
+    <div class="col-12 col-sm-4 header-middle">
+    {% block "header_middle" %}
+    {% endblock "header_middle" %}
     </div>
-    <div class="col-12 col-sm-6 header-right">
+
+    <!-- /pages -->
+
+    <div class="col-12 col-sm-4 header-right">
     {% block "header_right" %}
       {% block "header_account_panel" %}
 
       <!-- org switcher -->
       <span class="header-control">
         <span class="icon">
           <img src="{% static "common/icons/icon/org.svg" %}">
         </span>
 
-        <button data-element="button_select_org" class="button" type="button"  id="org-menu" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
+        <button data-element="button_select_org" class="button" type="button"  id="org-menu" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
         {{ request.org.display_name }}
         </button>
         <div class="dropdown-menu dropdown-menu-right" aria-labelledby="org-menu">
 
           <!-- current org options / actions -->
           <!-- switch org options -->
           <div
@@ -103,27 +152,27 @@
             <span class="icon icon-settings"></span>
             {% trans "Manage Organization" %}
           </a>
           {% endif %}
 
           {% if oauth_manages_org %}
 
-          <a class="dropdown-item" href="{{ account_service.urls.create_org }}?service={{ app_id }}">
+          <a class="dropdown-item" href="{{ account_service.urls.create_org }}">
             <span class="icon icon-add"></span>{% trans "Create Organization" %}</a>
           {% endif %}
         </div>
         <img class="caret" src="{% static "common/icons/ui-caret-caret/down.svg" %}">
       </span>
 
       <!-- user menu -->
       <span class="header-control">
         <span class="icon">
           <img src="{% static "common/icons/icon/user.svg" %}">
         </span>
-        <button data-element="button_account" class="button" type="button"  id="user-menu" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
+        <button data-element="button_account" class="button" type="button"  id="user-menu" data-bs-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
         {{ request.user.username }}
         </button>
         <div class="dropdown-menu dropdown-menu-right" aria-labelledby="user-menu">
           <h4>{{ request.user.first_name }} {{ request.user.last_name }}</h4>
           <span class="email">{{ request.user.email }}</span>
           <div class="horizontal-line"></div>
           <a class="dropdown-item" href="/logout/">
@@ -134,15 +183,17 @@
       {% endblock %}
     {% endblock %}
     </div>
   </div>
 </div>
 {% endblock %}
 
-{% if not permissions.read_instance %}
+{% block "error_content" %}{% endblock %}
+
+{% if not permissions.read_instance and request.org %}
 <div class="row">
   <div class="col-4"></div>
   <div class="col-4">
     <div class="alert alert-danger marg-top-lg">
 {% blocktrans trimmed with app_id=request.app_id org_name=request.org.name %}
 You do not have the permissions to view the {{ app_id }} workspace for the {{ org_name }} organization.
 {% endblocktrans %}
@@ -186,10 +237,16 @@
 {% include "common/app/modal.html" %}
 </div>
 {% if not permissions.read_instance %}</div>{% endif %}
 
 <div class="center app-footer">
 {% block "footer" %}
 version {{ version }}
+<p>
+<a class="button" href="mailto:{{ support_email }}">
+  <span class="icon icon-mail fullctl"></span>
+  <span class="label">Contact Support</span>
+</a>
+</p>
 {% endblock %}
 </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -5,22 +5,37 @@
 utocomplete.init.js" %}" type="text/javascript">
 orward.js" %}" type="text/javascript">
 elect2.js" %}" type="text/javascript">
 query.post-setup.js" %}" type="text/javascript">
 pp.js" %}" type="text/javascript">
 ervice_bridge.js" %}" type="text/javascript">
 {% endblock %} {% block "css" %} {{ block.super }}
-pp.css" %}" />
-hemes/dark.css" %}" />
+pp.css" %}?v=041208" />
+hemes/dark.css" %}?v=030802" />
 ss/vendor/select2/select2.css" %}" />
 ss/autocomplete.css" %}" />
 elect2.css" %}" />
  {% endblock %} {% block "content" %}
  {% block "header" %}
+{% if request.impersonating %}
+{% blocktrans with user=request.user
+logged_in_user=request.impersonating.superuser %} You are currently
+impersonating {{ user }} - logged in as {{ logged_in_user }} {% endblocktrans
+%}
+{% endif %}
+{% block "header_left" %}
 [{{ service_tag }}]
+{% for service_app in service_applications %} {% if service_app.slug !=
+service_tag %} {% with "common/logos/"|add:service_app.slug|add:"-dark.svg" as
+other_app_logo %} {%_if_not_service_app.logo_%}_[{{_service_app.slug_}}]_{%
+else_%}_[{{_service_app.slug_}}]_{%_endif_%} {% endwith %} {% endif %} {%
+endfor %}
+{% endblock "header_left" %}
+
+{% block "header_middle" %} {% endblock "header_middle" %}
 {% block "header_right" %} {% block "header_account_panel" %}
 cons/icon/org.svg" %}">   {{ request.org.display_name }}
 
  %}" data-org="{{ request.org.slug }}" data-element="select_org">
  cons/icon/org.svg" %}">   {% if permissions.update_instance and
 oauth_manages_org %}  {% endif %}
  {% if permissions.update_instance and oauth_manages_org %} _{%_trans_"Manage
@@ -28,24 +43,27 @@
 Organization"_%} {% endif %}
 cons/ui-caret-caret/down.svg" %}">
 cons/icon/user.svg" %}">   {{ request.user.username }}
 *** {{ request.user.first_name }} {{ request.user.last_name }} ***
 {{ request.user.email }}
 {%_trans_"Logout"_%}
 cons/ui-caret-caret/down.svg" %}">  {% endblock %} {% endblock %}
-{% endblock %} {% if not permissions.read_instance %}
+{% endblock %} {% block "error_content" %}{% endblock %} {% if not
+permissions.read_instance and request.org %}
 {% blocktrans trimmed with app_id=request.app_id org_name=request.org.name %}
 You do not have the permissions to view the {{ app_id }} workspace for the {
 { org_name }} organization. {% endblocktrans %}
 {% endif %} {% block "app_content" %}
 {% block "app_content_toolbar_outer" %}
 {% block "app_content_toolbar" %}{% endblock %}
 {% endblock %}
 {% block "app_content_main" %}{% endblock %}
 {% endblock %}
 {% include "common/app/templates.html" %} {% block "templates" %} {% endblock
 %}
 {% include "common/app/modal.html" %}
 {% if not permissions.read_instance %}
 {% endif %}
-{% block "footer" %} version {{ version }} {% endblock %}
+{% block "footer" %} version {{ version }}
+_Contact_Support
+{% endblock %}
 {% endblock %}
```

### Comparing `fullctl-0.3.0/src/fullctl/django/templates/common/app/forms/alert-prefs.html` & `fullctl-1.2.0rc1/src/fullctl/django/templates/common/app/forms/alert-prefs.html`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/templates/common/app/forms/import-org.html` & `fullctl-1.2.0rc1/src/fullctl/django/templates/common/app/forms/import-org.html`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/templates/common/app/forms/org-create.html` & `fullctl-1.2.0rc1/src/fullctl/django/templates/common/app/forms/org-create.html`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/templates/common/app/forms/org-prefs.html` & `fullctl-1.2.0rc1/src/fullctl/django/templates/common/app/forms/org-prefs.html`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/templates/common/app/manage/permissions.html` & `fullctl-1.2.0rc1/src/fullctl/django/templates/common/app/manage/permissions.html`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/templates/common/app/navbar.html` & `fullctl-1.2.0rc1/src/fullctl/django/templates/common/app/navbar.html`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/templates/common/auth/login.html` & `fullctl-1.2.0rc1/src/fullctl/django/templates/common/auth/login.html`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     <link rel="stylesheet" type="text/css" href="{% static "{{ sertvice_tag }}/{{ sertvice_tag }}.css" %}" />
     {% endblock %}
 
     {% block "header_middle" %}
     <div class="container-fluid header-outer">
         <div class="top-border {{ sertvice_tag }} app_bg"></div>
         <div class="row header">
-            <div class="col-12 col-sm-6 header-left mt-3 mb-2 ml-3 app-switcher">
+            <div class="col-12 col-sm-6 header-left mt-3 mb-2 ms-3 app-switcher">
                 <img class="app-logo" src="{% static service_logo_dark %}" alt="{{ sertvice_tag }}">
             </div>
         </div>
     </div>
     {% endblock %}
 
     {% if form.errors %}
```

### Comparing `fullctl-0.3.0/src/fullctl/django/templates/common/auth/oauth-badge.html` & `fullctl-1.2.0rc1/src/fullctl/django/templates/common/auth/oauth-badge.html`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/templates/common/auth/oauth.html` & `fullctl-1.2.0rc1/src/fullctl/django/templates/common/auth/oauth.html`

 * *Files identical despite different names*

### Comparing `fullctl-0.3.0/src/fullctl/django/templates/common/base.html` & `fullctl-1.2.0rc1/src/fullctl/django/templates/common/base.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 {% load static %}
-<!DOCYTYPE html>
+<!DOCTYPE html>
 <html>
   <head>
     <title>{% block "title" %}fullctl{% endblock %}</title>
     <meta charset="utf-8">
     <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
-    <link rel="shortcut icon" type="image/ico" href="{% static "website/favicon.ico" %}">
+    <link rel="shortcut icon" type="image/ico" href="{% static "common/favicon.ico" %}">
 
     {% block "js" %}
-    <script
-      src="https://code.jquery.com/jquery-3.3.1.min.js"
-      integrity="sha256-FgpCb/KJQlLNfOu91ta32o/NMZxltwRo8QtmkMRdAu8="
-      crossorigin="anonymous"></script>
-    <script src="https://cdnjs.cloudflare.com/ajax/libs/tether/1.4.0/js/tether.min.js" integrity="sha384-DztdAPBWPRXSA/3eYEEUWrWCy7G5KFbe8fFjk5JAIxUYHKkDx6Qin1DkWx51bBrb" crossorigin="anonymous"></script>
-    <script src="https://unpkg.com/popper.js/dist/umd/popper.min.js" crossorigin="anonymous"></script>
-    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js" integrity="sha384-ChfqqxuZUCnJSK3+MXmPNIyE6ZbWh2IMqE241rYiqJxyMiZ6OW/JmZQ5stwEULTy" crossorigin="anonymous"></script>
+    <script src="https://code.jquery.com/jquery-3.6.0.min.js" integrity="sha256-/xUj+3OJU5yExlq6GSYGSHk7tPXikynS7ogEvDej/m4=" crossorigin="anonymous"></script>
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/tether/1.4.7/js/tether.min.js" integrity="sha512-X7kCKQJMwapt5FCOl2+ilyuHJp+6ISxFTVrx+nkrhgplZozodT9taV2GuGHxBgKKpOJZ4je77OuPooJg9FJLvw==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-kenU1KFdBIe4zVF0s0G1M5b4hcpxyD9F7jL+jjXkk+Q2h455rYXK/7HAuoJl+0I4" crossorigin="anonymous"></script>
     <script src="{% static "common/20c/twentyc.core.min.js" %}"></script>
     <script src="{% static "common/20c/twentyc.rest.js" %}"></script>
     <script src="{% static "grainy/grainy.js" %}"></script>
     <script>
     $(document).ready(function() {
       twentyc.rest.config.csrf = "{{ csrf_token }}";
 
@@ -28,46 +24,19 @@
       {% endfor %}
       })
     });
     </script>
     {% endblock %}
     {% block "css" %}
     <link href="https://fonts.googleapis.com/css?family=Archivo+Narrow" rel="stylesheet">
-    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css" integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO" crossorigin="anonymous">
+    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-rbsA2VBKQhggwzxH7pPCaAqO46MgnOM80zW1RWuH61DGLwZJEdK2Kadq2F9CUG65" crossorigin="anonymous">
     {% endblock %}
   </head>
   <body>
   {% block "content" %}
 
   {% endblock "content" %}
 
-{% if env == "prod" %}
-<!-- Global site tag (gtag.js) - Google Analytics -->
-<script async src="https://www.googletagmanager.com/gtag/js?id=UA-20466829-3"></script>
-<script>
-  window.dataLayer = window.dataLayer || [];
-  function gtag(){dataLayer.push(arguments);}
-  gtag('js', new Date());
-
-  gtag('config', 'UA-20466829-3');
-</script>
-{% endif %}
-
-
-<link rel="stylesheet" type="text/css" href="//cdnjs.cloudflare.com/ajax/libs/cookieconsent2/3.1.0/cookieconsent.min.css" />
-<script src="//cdnjs.cloudflare.com/ajax/libs/cookieconsent2/3.1.0/cookieconsent.min.js"></script>
-<script>
-window.addEventListener("load", function(){
-window.cookieconsent.initialise({
-  "palette": {
-    "popup": {
-      "background": "#252e39"
-    },
-    "button": {
-      "background": "#14a7d0"
-    }
-  }
-})});
-</script>
+  {% include "common/snippets.html" %}
 
   </body>
 </html>
```

### Comparing `fullctl-0.3.0/src/fullctl/django/validators.py` & `fullctl-1.2.0rc1/src/fullctl/django/validators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import ipaddress
 import re
 
 from django.core.exceptions import ValidationError
 
 
 def validate_alphanumeric(value):
     """
@@ -37,7 +38,21 @@
     """
 
     if not isinstance(value, list):
         value = value.split(",")
 
     for item in value:
         validate_alphanumeric(item)
+
+
+def ip_address_string(value):
+    """
+    Takes an ip address string and returns a validated normalized
+    ip address string.
+
+    This will strep the net mask if it is provided
+    """
+
+    if not value:
+        return value
+    value = str(value)
+    return str(ipaddress.ip_interface(value))
```

### Comparing `fullctl-0.3.0/PKG-INFO` & `fullctl-1.2.0rc1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,45 @@
 Metadata-Version: 2.1
 Name: fullctl
-Version: 0.3.0
+Version: 1.2.0rc1
 Summary: Core classes and functions for service applications
 Home-page: https://github.com/fullctl/fullctl
 License: Apache-2.0
 Author: 20C
 Author-email: code@20c.com
-Requires-Python: >=3.6,<4.0
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
-Requires-Dist: Django (>=2.2,<3)
-Requires-Dist: celery (>=5,<6)
-Requires-Dist: django-autocomplete-light (>=3,<=4)
-Requires-Dist: django-grainy (>=1.9.0,<2)
-Requires-Dist: django-handleref (>=0.5)
-Requires-Dist: django-inet
-Requires-Dist: django-peeringdb
-Requires-Dist: django-reversion (<4)
-Requires-Dist: djangorestframework (>=3.11,<4)
-Requires-Dist: grainy (>=1.6.0,<2)
-Requires-Dist: peeringdb (<2)
-Requires-Dist: pip
-Requires-Dist: pyyaml
-Requires-Dist: social-auth-app-django (<4)
+Requires-Dist: Django (>=3.2,<3.3)
+Requires-Dist: confu (>=1.5,<2.0)
+Requires-Dist: django-autocomplete-light (==3.5.1)
+Requires-Dist: django-crispy-forms (>=1.8,<2.0)
+Requires-Dist: django-grainy (>=1.9,<2.0)
+Requires-Dist: django-handleref (>=1,<2)
+Requires-Dist: django-inet (>=1,<2)
+Requires-Dist: django-netfields (<2)
+Requires-Dist: django-peeringdb (>=2.8,<3.0)
+Requires-Dist: django-recaptcha (>=2,<3)
+Requires-Dist: django-reversion (>=5,<6)
+Requires-Dist: django-structlog (>=2.1.3,<3.0.0)
+Requires-Dist: djangorestframework (>=3,<4)
+Requires-Dist: grainy (>=1.8.1,<2.0.0)
+Requires-Dist: psycopg2-binary (>=2.8,<3.0)
+Requires-Dist: pyuwsgi (>=2.0.19,<3.0.0)
+Requires-Dist: pyyaml (>=5)
+Requires-Dist: setuptools
+Requires-Dist: social-auth-app-django (>=5.2)
+Requires-Dist: whitenoise (>=6,<7)
 Project-URL: Repository, https://github.com/fullctl/fullctl
```

