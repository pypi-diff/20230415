# Comparing `tmp/starlette_web-0.1.2.tar.gz` & `tmp/starlette_web-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlette_web-0.1.2.tar", last modified: Thu Apr 13 19:30:56 2023, max compression
+gzip compressed data, was "starlette_web-0.1.3.tar", last modified: Sat Apr 15 08:29:36 2023, max compression
```

## Comparing `starlette_web-0.1.2.tar` & `starlette_web-0.1.3.tar`

### file list

```diff
@@ -1,260 +1,260 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.476963 starlette_web-0.1.2/
--rw-rw-rw-   0        0        0     1092 2022-04-25 19:06:18.000000 starlette_web-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       75 2023-04-13 19:30:53.000000 starlette_web-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3245 2023-04-13 19:30:56.476963 starlette_web-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2329 2023-03-26 13:41:03.000000 starlette_web-0.1.2/README.md
--rw-rw-rw-   0        0        0     1870 2023-04-13 19:30:56.476963 starlette_web-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0       75 2022-04-25 19:06:18.000000 starlette_web-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.317238 starlette_web-0.1.2/starlette_web/
--rw-rw-rw-   0        0        0       23 2022-12-29 14:13:54.000000 starlette_web-0.1.2/starlette_web/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.317238 starlette_web-0.1.2/starlette_web/common/
--rw-rw-rw-   0        0        0       52 2022-04-25 19:06:18.000000 starlette_web-0.1.2/starlette_web/common/__init__.py
--rw-rw-rw-   0        0        0     5348 2023-03-30 21:26:53.000000 starlette_web-0.1.2/starlette_web/common/app.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.317238 starlette_web-0.1.2/starlette_web/common/authorization/
--rw-rw-rw-   0        0        0        0 2022-12-31 10:33:26.000000 starlette_web-0.1.2/starlette_web/common/authorization/__init__.py
--rw-rw-rw-   0        0        0      856 2023-03-25 08:05:20.000000 starlette_web-0.1.2/starlette_web/common/authorization/backends.py
--rw-rw-rw-   0        0        0      329 2023-03-25 08:05:20.000000 starlette_web-0.1.2/starlette_web/common/authorization/base_user.py
--rw-rw-rw-   0        0        0     3025 2023-03-25 08:05:20.000000 starlette_web-0.1.2/starlette_web/common/authorization/permissions.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.327060 starlette_web-0.1.2/starlette_web/common/caches/
--rw-rw-rw-   0        0        0       80 2023-03-16 18:44:56.000000 starlette_web-0.1.2/starlette_web/common/caches/__init__.py
--rw-rw-rw-   0        0        0     2162 2023-03-25 08:05:20.000000 starlette_web-0.1.2/starlette_web/common/caches/base.py
--rw-rw-rw-   0        0        0     3342 2023-04-01 08:01:57.000000 starlette_web-0.1.2/starlette_web/common/caches/base_lock.py
--rw-rw-rw-   0        0        0     1112 2023-03-16 18:44:56.000000 starlette_web-0.1.2/starlette_web/common/caches/cache_handler.py
--rw-rw-rw-   0        0        0     5241 2023-03-24 16:47:56.000000 starlette_web-0.1.2/starlette_web/common/caches/local_memory.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.337279 starlette_web-0.1.2/starlette_web/common/channels/
--rw-rw-rw-   0        0        0       54 2023-03-12 16:44:21.000000 starlette_web-0.1.2/starlette_web/common/channels/__init__.py
--rw-rw-rw-   0        0        0     4253 2023-04-01 19:06:23.000000 starlette_web-0.1.2/starlette_web/common/channels/base.py
--rw-rw-rw-   0        0        0      447 2023-03-12 16:44:21.000000 starlette_web-0.1.2/starlette_web/common/channels/event.py
--rw-rw-rw-   0        0        0      181 2023-03-22 16:38:31.000000 starlette_web-0.1.2/starlette_web/common/channels/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.337279 starlette_web-0.1.2/starlette_web/common/channels/layers/
--rw-rw-rw-   0        0        0        0 2023-03-12 16:44:21.000000 starlette_web-0.1.2/starlette_web/common/channels/layers/__init__.py
--rw-rw-rw-   0        0        0      753 2023-03-12 16:44:21.000000 starlette_web-0.1.2/starlette_web/common/channels/layers/base.py
--rw-rw-rw-   0        0        0     1694 2023-03-12 19:30:41.000000 starlette_web-0.1.2/starlette_web/common/channels/layers/local_memory.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.337279 starlette_web-0.1.2/starlette_web/common/conf/
--rw-rw-rw-   0        0        0     2285 2023-03-30 21:26:53.000000 starlette_web-0.1.2/starlette_web/common/conf/__init__.py
--rw-rw-rw-   0        0        0     3314 2023-04-13 17:27:54.000000 starlette_web-0.1.2/starlette_web/common/conf/app_manager.py
--rw-rw-rw-   0        0        0      198 2023-03-03 17:32:15.000000 starlette_web-0.1.2/starlette_web/common/conf/base_app_config.py
--rw-rw-rw-   0        0        0     1752 2023-04-06 19:27:41.000000 starlette_web-0.1.2/starlette_web/common/conf/global_settings.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.337279 starlette_web-0.1.2/starlette_web/common/database/
--rw-rw-rw-   0        0        0      359 2022-05-09 11:25:06.000000 starlette_web-0.1.2/starlette_web/common/database/__init__.py
--rw-rw-rw-   0        0        0     1362 2023-02-26 15:17:29.000000 starlette_web-0.1.2/starlette_web/common/database/columns.py
--rw-rw-rw-   0        0        0       81 2022-05-09 11:25:06.000000 starlette_web-0.1.2/starlette_web/common/database/model_base.py
--rw-rw-rw-   0        0        0     9279 2023-04-09 22:15:24.000000 starlette_web-0.1.2/starlette_web/common/database/model_mixin.py
--rw-rw-rw-   0        0        0     1550 2023-02-17 20:43:07.000000 starlette_web-0.1.2/starlette_web/common/database/session_maker.py
--rw-rw-rw-   0        0        0     2059 2023-02-18 12:47:03.000000 starlette_web-0.1.2/starlette_web/common/database/types.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.347097 starlette_web-0.1.2/starlette_web/common/email/
--rw-rw-rw-   0        0        0      169 2022-05-22 18:14:32.000000 starlette_web-0.1.2/starlette_web/common/email/__init__.py
--rw-rw-rw-   0        0        0     1604 2023-03-28 17:00:26.000000 starlette_web-0.1.2/starlette_web/common/email/base_sender.py
--rw-rw-rw-   0        0        0     1770 2023-03-27 20:27:55.000000 starlette_web-0.1.2/starlette_web/common/email/email_manager.py
--rw-rw-rw-   0        0        0     1728 2023-03-30 21:26:53.000000 starlette_web-0.1.2/starlette_web/common/email/smtp.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.347097 starlette_web-0.1.2/starlette_web/common/files/
--rw-rw-rw-   0        0        0        0 2023-03-22 16:53:00.000000 starlette_web-0.1.2/starlette_web/common/files/__init__.py
--rw-rw-rw-   0        0        0     7085 2023-03-30 21:26:53.000000 starlette_web-0.1.2/starlette_web/common/files/cache.py
--rw-rw-rw-   0        0        0     3837 2023-04-01 08:06:20.000000 starlette_web-0.1.2/starlette_web/common/files/filelock.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.347097 starlette_web-0.1.2/starlette_web/common/files/storages/
--rw-rw-rw-   0        0        0      136 2023-03-30 20:24:14.000000 starlette_web-0.1.2/starlette_web/common/files/storages/__init__.py
--rw-rw-rw-   0        0        0     6332 2023-03-31 18:48:34.000000 starlette_web-0.1.2/starlette_web/common/files/storages/base.py
--rw-rw-rw-   0        0        0     4532 2023-04-01 16:31:26.000000 starlette_web-0.1.2/starlette_web/common/files/storages/filesystem.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.357993 starlette_web-0.1.2/starlette_web/common/http/
--rw-rw-rw-   0        0        0        0 2022-05-03 08:01:50.000000 starlette_web-0.1.2/starlette_web/common/http/__init__.py
--rw-rw-rw-   0        0        0     6474 2023-03-26 10:02:27.000000 starlette_web-0.1.2/starlette_web/common/http/base_endpoint.py
--rw-rw-rw-   0        0        0     4338 2023-02-26 15:17:29.000000 starlette_web-0.1.2/starlette_web/common/http/exception_handlers.py
--rw-rw-rw-   0        0        0     4287 2023-03-30 21:26:53.000000 starlette_web-0.1.2/starlette_web/common/http/exceptions.py
--rw-rw-rw-   0        0        0     1075 2022-05-09 11:25:06.000000 starlette_web-0.1.2/starlette_web/common/http/renderers.py
--rw-rw-rw-   0        0        0      336 2022-10-03 19:19:24.000000 starlette_web-0.1.2/starlette_web/common/http/responses.py
--rw-rw-rw-   0        0        0      829 2022-10-03 19:19:24.000000 starlette_web-0.1.2/starlette_web/common/http/schemas.py
--rw-rw-rw-   0        0        0      942 2023-03-14 17:15:47.000000 starlette_web-0.1.2/starlette_web/common/http/statuses.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.357993 starlette_web-0.1.2/starlette_web/common/i18n/
--rw-rw-rw-   0        0        0      163 2022-09-03 15:11:31.000000 starlette_web-0.1.2/starlette_web/common/i18n/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.357993 starlette_web-0.1.2/starlette_web/common/management/
--rw-rw-rw-   0        0        0        0 2022-12-31 10:33:26.000000 starlette_web-0.1.2/starlette_web/common/management/__init__.py
--rw-rw-rw-   0        0        0     1489 2023-03-30 21:26:53.000000 starlette_web-0.1.2/starlette_web/common/management/admin_util.py
--rw-rw-rw-   0        0        0     1080 2023-04-06 12:18:07.000000 starlette_web-0.1.2/starlette_web/common/management/alembic_mixin.py
--rw-rw-rw-   0        0        0     6023 2023-04-13 17:02:30.000000 starlette_web-0.1.2/starlette_web/common/management/base.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.367331 starlette_web-0.1.2/starlette_web/common/management/commands/
--rw-rw-rw-   0        0        0        0 2023-03-21 19:56:59.000000 starlette_web-0.1.2/starlette_web/common/management/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.367331 starlette_web-0.1.2/starlette_web/common/management/commands/_app_defaults/
--rw-rw-rw-   0        0        0        0 2023-03-26 18:53:46.000000 starlette_web-0.1.2/starlette_web/common/management/commands/_app_defaults/__init__.py
--rw-rw-rw-   0        0        0      376 2023-03-26 18:59:14.000000 starlette_web-0.1.2/starlette_web/common/management/commands/_app_defaults/admin.py
--rw-rw-rw-   0        0        0      224 2023-03-26 18:55:02.000000 starlette_web-0.1.2/starlette_web/common/management/commands/_app_defaults/apps.py
--rw-rw-rw-   0        0        0      297 2023-03-26 18:59:20.000000 starlette_web-0.1.2/starlette_web/common/management/commands/_app_defaults/models.py
--rw-rw-rw-   0        0        0       95 2023-03-26 19:00:40.000000 starlette_web-0.1.2/starlette_web/common/management/commands/_app_defaults/routes.py
--rw-rw-rw-   0        0        0      154 2023-03-26 19:00:00.000000 starlette_web-0.1.2/starlette_web/common/management/commands/_app_defaults/views.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.377349 starlette_web-0.1.2/starlette_web/common/management/commands/_project_defaults/
--rw-rw-rw-   0        0        0        0 2023-03-26 17:54:43.000000 starlette_web-0.1.2/starlette_web/common/management/commands/_project_defaults/__init__.py
--rw-rw-rw-   0        0        0      466 2023-04-03 20:19:20.000000 starlette_web-0.1.2/starlette_web/common/management/commands/_project_defaults/asgi.py
--rw-rw-rw-   0        0        0      896 2023-03-26 17:36:41.000000 starlette_web-0.1.2/starlette_web/common/management/commands/_project_defaults/command.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.377349 starlette_web-0.1.2/starlette_web/common/management/commands/_project_defaults/core/
--rw-rw-rw-   0        0        0        0 2022-04-25 19:06:18.000000 starlette_web-0.1.2/starlette_web/common/management/commands/_project_defaults/core/__init__.py
--rw-rw-rw-   0        0        0      885 2023-04-13 18:30:43.000000 starlette_web-0.1.2/starlette_web/common/management/commands/_project_defaults/core/routes.py
--rw-rw-rw-   0        0        0     3441 2023-04-06 18:51:17.000000 starlette_web-0.1.2/starlette_web/common/management/commands/_project_defaults/core/settings.py
--rw-rw-rw-   0        0        0     1552 2023-04-06 16:46:50.000000 starlette_web-0.1.2/starlette_web/common/management/commands/makemigrations.py
--rw-rw-rw-   0        0        0     1294 2023-04-06 16:46:56.000000 starlette_web-0.1.2/starlette_web/common/management/commands/migrate.py
--rw-rw-rw-   0        0        0     2171 2023-03-30 21:26:53.000000 starlette_web-0.1.2/starlette_web/common/management/commands/startapp.py
--rw-rw-rw-   0        0        0     3800 2023-04-06 16:47:27.000000 starlette_web-0.1.2/starlette_web/common/management/commands/startproject.py
--rw-rw-rw-   0        0        0     2019 2023-04-08 06:35:50.000000 starlette_web-0.1.2/starlette_web/common/management/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.386994 starlette_web-0.1.2/starlette_web/common/utils/
--rw-rw-rw-   0        0        0      506 2023-04-01 19:36:50.000000 starlette_web-0.1.2/starlette_web/common/utils/__init__.py
--rw-rw-rw-   0        0        0     2578 2022-09-03 15:11:31.000000 starlette_web-0.1.2/starlette_web/common/utils/choices.py
--rw-rw-rw-   0        0        0     1265 2023-03-18 14:43:23.000000 starlette_web-0.1.2/starlette_web/common/utils/crypto.py
--rw-rw-rw-   0        0        0      187 2023-04-01 19:33:59.000000 starlette_web-0.1.2/starlette_web/common/utils/encoding.py
--rw-rw-rw-   0        0        0      633 2023-02-17 20:46:29.000000 starlette_web-0.1.2/starlette_web/common/utils/importing.py
--rw-rw-rw-   0        0        0      546 2023-03-30 21:26:53.000000 starlette_web-0.1.2/starlette_web/common/utils/inspect.py
--rw-rw-rw-   0        0        0     2324 2022-05-09 11:25:06.000000 starlette_web-0.1.2/starlette_web/common/utils/json.py
--rw-rw-rw-   0        0        0     2273 2023-03-30 21:26:53.000000 starlette_web-0.1.2/starlette_web/common/utils/regex.py
--rw-rw-rw-   0        0        0     1828 2023-03-25 08:05:10.000000 starlette_web-0.1.2/starlette_web/common/utils/serializers.py
--rw-rw-rw-   0        0        0      246 2022-05-09 11:25:06.000000 starlette_web-0.1.2/starlette_web/common/utils/singleton.py
--rw-rw-rw-   0        0        0      217 2022-10-03 19:19:24.000000 starlette_web-0.1.2/starlette_web/common/utils/urls.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.386994 starlette_web-0.1.2/starlette_web/common/ws/
--rw-rw-rw-   0        0        0        0 2022-12-29 14:13:54.000000 starlette_web-0.1.2/starlette_web/common/ws/__init__.py
--rw-rw-rw-   0        0        0     6919 2023-03-14 17:15:47.000000 starlette_web-0.1.2/starlette_web/common/ws/base_endpoint.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.386994 starlette_web-0.1.2/starlette_web/contrib/
--rw-rw-rw-   0        0        0        0 2022-05-09 11:25:06.000000 starlette_web-0.1.2/starlette_web/contrib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.396939 starlette_web-0.1.2/starlette_web/contrib/admin/
--rw-rw-rw-   0        0        0      185 2023-02-26 15:17:29.000000 starlette_web-0.1.2/starlette_web/contrib/admin/__init__.py
--rw-rw-rw-   0        0        0     3705 2023-03-24 18:55:03.000000 starlette_web-0.1.2/starlette_web/contrib/admin/admin.py
--rw-rw-rw-   0        0        0      564 2023-03-03 17:32:15.000000 starlette_web-0.1.2/starlette_web/contrib/admin/apps.py
--rw-rw-rw-   0        0        0     2780 2023-02-26 15:17:29.000000 starlette_web-0.1.2/starlette_web/contrib/admin/auth_provider.py
--rw-rw-rw-   0        0        0     5122 2023-03-18 20:17:51.000000 starlette_web-0.1.2/starlette_web/contrib/admin/middleware.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.396939 starlette_web-0.1.2/starlette_web/contrib/apispec/
--rw-rw-rw-   0        0        0        0 2022-10-03 19:19:24.000000 starlette_web-0.1.2/starlette_web/contrib/apispec/__init__.py
--rw-rw-rw-   0        0        0     2017 2023-04-03 20:01:29.000000 starlette_web-0.1.2/starlette_web/contrib/apispec/apps.py
--rw-rw-rw-   0        0        0     5451 2023-03-03 17:32:15.000000 starlette_web-0.1.2/starlette_web/contrib/apispec/introspection.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.396939 starlette_web-0.1.2/starlette_web/contrib/apispec/marshmallow/
--rw-rw-rw-   0        0        0      352 2022-10-03 19:19:24.000000 starlette_web-0.1.2/starlette_web/contrib/apispec/marshmallow/__init__.py
--rw-rw-rw-   0        0        0     1545 2022-10-03 19:19:24.000000 starlette_web-0.1.2/starlette_web/contrib/apispec/marshmallow/converters.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.287172 starlette_web-0.1.2/starlette_web/contrib/apispec/static/
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.396939 starlette_web-0.1.2/starlette_web/contrib/apispec/static/apispec/
--rw-rw-rw-   0        0        0   879592 2022-10-03 19:19:24.000000 starlette_web-0.1.2/starlette_web/contrib/apispec/static/apispec/redoc.js
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.297397 starlette_web-0.1.2/starlette_web/contrib/apispec/templates/
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.396939 starlette_web-0.1.2/starlette_web/contrib/apispec/templates/apispec/
--rw-rw-rw-   0        0        0      539 2022-10-03 19:19:24.000000 starlette_web-0.1.2/starlette_web/contrib/apispec/templates/apispec/redoc.html
--rw-rw-rw-   0        0        0     1889 2023-04-13 18:25:49.000000 starlette_web-0.1.2/starlette_web/contrib/apispec/views.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.407376 starlette_web-0.1.2/starlette_web/contrib/auth/
--rw-rw-rw-   0        0        0        0 2023-04-13 17:15:05.000000 starlette_web-0.1.2/starlette_web/contrib/auth/__init__.py
--rw-rw-rw-   0        0        0     3484 2023-02-26 16:10:52.000000 starlette_web-0.1.2/starlette_web/contrib/auth/admin.py
--rw-rw-rw-   0        0        0      261 2023-03-17 18:16:19.000000 starlette_web-0.1.2/starlette_web/contrib/auth/apps.py
--rw-rw-rw-   0        0        0     4299 2023-02-26 15:17:29.000000 starlette_web-0.1.2/starlette_web/contrib/auth/backend.py
--rw-rw-rw-   0        0        0     3981 2023-03-25 08:05:10.000000 starlette_web-0.1.2/starlette_web/contrib/auth/hashers.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.417272 starlette_web-0.1.2/starlette_web/contrib/auth/management/
--rw-rw-rw-   0        0        0        0 2023-02-26 15:17:29.000000 starlette_web-0.1.2/starlette_web/contrib/auth/management/__init__.py
--rw-rw-rw-   0        0        0     1308 2023-04-01 16:41:19.000000 starlette_web-0.1.2/starlette_web/contrib/auth/management/auth_command_mixin.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.417272 starlette_web-0.1.2/starlette_web/contrib/auth/management/commands/
--rw-rw-rw-   0        0        0        0 2023-02-26 15:17:29.000000 starlette_web-0.1.2/starlette_web/contrib/auth/management/commands/__init__.py
--rw-rw-rw-   0        0        0     1428 2023-04-01 16:41:42.000000 starlette_web-0.1.2/starlette_web/contrib/auth/management/commands/changepassword.py
--rw-rw-rw-   0        0        0     1459 2023-04-01 16:41:42.000000 starlette_web-0.1.2/starlette_web/contrib/auth/management/commands/createsuperuser.py
--rw-rw-rw-   0        0        0     3192 2023-02-26 15:17:30.000000 starlette_web-0.1.2/starlette_web/contrib/auth/models.py
--rw-rw-rw-   0        0        0     3057 2023-03-18 20:17:51.000000 starlette_web-0.1.2/starlette_web/contrib/auth/password_validation.py
--rw-rw-rw-   0        0        0      624 2023-02-26 15:17:30.000000 starlette_web-0.1.2/starlette_web/contrib/auth/permissions.py
--rw-rw-rw-   0        0        0      654 2022-05-09 11:25:06.000000 starlette_web-0.1.2/starlette_web/contrib/auth/routes.py
--rw-rw-rw-   0        0        0     2724 2022-10-01 11:03:47.000000 starlette_web-0.1.2/starlette_web/contrib/auth/schemas.py
--rw-rw-rw-   0        0        0     1414 2023-03-18 20:17:51.000000 starlette_web-0.1.2/starlette_web/contrib/auth/utils.py
--rw-rw-rw-   0        0        0    18290 2023-03-30 21:26:53.000000 starlette_web-0.1.2/starlette_web/contrib/auth/views.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.417272 starlette_web-0.1.2/starlette_web/contrib/camel_case/
--rw-rw-rw-   0        0        0      249 2022-05-03 14:50:29.000000 starlette_web-0.1.2/starlette_web/contrib/camel_case/__init__.py
--rw-rw-rw-   0        0        0      389 2023-04-09 20:47:08.000000 starlette_web-0.1.2/starlette_web/contrib/camel_case/parser.py
--rw-rw-rw-   0        0        0      262 2022-05-03 14:50:29.000000 starlette_web-0.1.2/starlette_web/contrib/camel_case/renderer.py
--rw-rw-rw-   0        0        0     4103 2022-10-03 19:19:24.000000 starlette_web-0.1.2/starlette_web/contrib/camel_case/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.417272 starlette_web-0.1.2/starlette_web/contrib/constance/
--rw-rw-rw-   0        0        0     3754 2023-04-06 19:52:27.000000 starlette_web-0.1.2/starlette_web/contrib/constance/__init__.py
--rw-rw-rw-   0        0        0     1144 2023-04-06 20:13:04.000000 starlette_web-0.1.2/starlette_web/contrib/constance/apps.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.417272 starlette_web-0.1.2/starlette_web/contrib/constance/backends/
--rw-rw-rw-   0        0        0        0 2023-02-20 07:01:30.000000 starlette_web-0.1.2/starlette_web/contrib/constance/backends/__init__.py
--rw-rw-rw-   0        0        0     1410 2023-04-06 19:49:34.000000 starlette_web-0.1.2/starlette_web/contrib/constance/backends/base.py
--rw-rw-rw-   0        0        0     1656 2023-04-06 20:18:43.000000 starlette_web-0.1.2/starlette_web/contrib/constance/backends/caching_mixin.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.427173 starlette_web-0.1.2/starlette_web/contrib/constance/backends/database/
--rw-rw-rw-   0        0        0     1717 2023-03-12 16:44:01.000000 starlette_web-0.1.2/starlette_web/contrib/constance/backends/database/__init__.py
--rw-rw-rw-   0        0        0      152 2023-03-03 17:32:15.000000 starlette_web-0.1.2/starlette_web/contrib/constance/backends/database/apps.py
--rw-rw-rw-   0        0        0      368 2023-03-12 16:44:01.000000 starlette_web-0.1.2/starlette_web/contrib/constance/backends/database/models.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.427173 starlette_web-0.1.2/starlette_web/contrib/postgres/
--rw-rw-rw-   0        0        0        0 2023-03-12 16:44:21.000000 starlette_web-0.1.2/starlette_web/contrib/postgres/__init__.py
--rw-rw-rw-   0        0        0     3535 2023-04-02 10:14:34.000000 starlette_web-0.1.2/starlette_web/contrib/postgres/channel_layers.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.427173 starlette_web-0.1.2/starlette_web/contrib/redis/
--rw-rw-rw-   0        0        0      137 2022-05-14 13:30:44.000000 starlette_web-0.1.2/starlette_web/contrib/redis/__init__.py
--rw-rw-rw-   0        0        0     4616 2023-04-01 19:37:06.000000 starlette_web-0.1.2/starlette_web/contrib/redis/cache.py
--rw-rw-rw-   0        0        0     2261 2023-04-01 19:42:16.000000 starlette_web-0.1.2/starlette_web/contrib/redis/channel_layers.py
--rw-rw-rw-   0        0        0     1196 2023-03-27 18:37:04.000000 starlette_web-0.1.2/starlette_web/contrib/redis/redislock.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.427173 starlette_web-0.1.2/starlette_web/contrib/scheduler/
--rw-rw-rw-   0        0        0      133 2023-03-04 19:50:46.000000 starlette_web-0.1.2/starlette_web/contrib/scheduler/__init__.py
--rw-rw-rw-   0        0        0     2217 2023-03-04 19:50:46.000000 starlette_web-0.1.2/starlette_web/contrib/scheduler/app_settings.py
--rw-rw-rw-   0        0        0     2084 2023-04-03 20:00:17.000000 starlette_web-0.1.2/starlette_web/contrib/scheduler/apps.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.437099 starlette_web-0.1.2/starlette_web/contrib/scheduler/backends/
--rw-rw-rw-   0        0        0      843 2023-03-31 19:10:23.000000 starlette_web-0.1.2/starlette_web/contrib/scheduler/backends/__init__.py
--rw-rw-rw-   0        0        0     3867 2023-04-09 17:22:30.000000 starlette_web-0.1.2/starlette_web/contrib/scheduler/backends/base.py
--rw-rw-rw-   0        0        0     2629 2023-03-31 19:15:23.000000 starlette_web-0.1.2/starlette_web/contrib/scheduler/backends/posix.py
--rw-rw-rw-   0        0        0     7287 2023-03-31 19:15:38.000000 starlette_web-0.1.2/starlette_web/contrib/scheduler/backends/win32.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.437099 starlette_web-0.1.2/starlette_web/contrib/scheduler/management/
--rw-rw-rw-   0        0        0        0 2023-03-04 19:50:46.000000 starlette_web-0.1.2/starlette_web/contrib/scheduler/management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.437099 starlette_web-0.1.2/starlette_web/contrib/scheduler/management/commands/
--rw-rw-rw-   0        0        0        0 2023-03-04 19:50:46.000000 starlette_web-0.1.2/starlette_web/contrib/scheduler/management/commands/__init__.py
--rw-rw-rw-   0        0        0     1432 2023-03-31 19:14:46.000000 starlette_web-0.1.2/starlette_web/contrib/scheduler/management/commands/scheduler.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.437099 starlette_web-0.1.2/starlette_web/contrib/staticfiles/
--rw-rw-rw-   0        0        0        0 2023-03-03 17:32:15.000000 starlette_web-0.1.2/starlette_web/contrib/staticfiles/__init__.py
--rw-rw-rw-   0        0        0      136 2023-03-03 17:32:15.000000 starlette_web-0.1.2/starlette_web/contrib/staticfiles/apps.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.437099 starlette_web-0.1.2/starlette_web/contrib/staticfiles/management/
--rw-rw-rw-   0        0        0        0 2023-03-03 17:32:15.000000 starlette_web-0.1.2/starlette_web/contrib/staticfiles/management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.437099 starlette_web-0.1.2/starlette_web/contrib/staticfiles/management/commands/
--rw-rw-rw-   0        0        0        0 2023-03-03 17:32:15.000000 starlette_web-0.1.2/starlette_web/contrib/staticfiles/management/commands/__init__.py
--rw-rw-rw-   0        0        0     4229 2023-03-03 17:32:15.000000 starlette_web-0.1.2/starlette_web/contrib/staticfiles/management/commands/collectstatic.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.447104 starlette_web-0.1.2/starlette_web/tests/
--rw-rw-rw-   0        0        0        0 2022-04-25 19:06:18.000000 starlette_web-0.1.2/starlette_web/tests/__init__.py
--rw-rw-rw-   0        0        0      202 2023-03-03 17:32:15.000000 starlette_web-0.1.2/starlette_web/tests/apps.py
--rw-rw-rw-   0        0        0     5474 2023-04-06 20:04:06.000000 starlette_web-0.1.2/starlette_web/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.457963 starlette_web-0.1.2/starlette_web/tests/contrib/
--rw-rw-rw-   0        0        0        0 2022-05-03 14:50:29.000000 starlette_web-0.1.2/starlette_web/tests/contrib/__init__.py
--rw-rw-rw-   0        0        0    16572 2023-04-13 18:40:01.000000 starlette_web-0.1.2/starlette_web/tests/contrib/test_apispec.py
--rw-rw-rw-   0        0        0    27613 2023-03-30 19:24:14.000000 starlette_web-0.1.2/starlette_web/tests/contrib/test_auth.py
--rw-rw-rw-   0        0        0     1966 2022-05-03 14:50:29.000000 starlette_web-0.1.2/starlette_web/tests/contrib/test_camel_case.py
--rw-rw-rw-   0        0        0     7677 2023-04-05 19:51:46.000000 starlette_web-0.1.2/starlette_web/tests/contrib/test_channels.py
--rw-rw-rw-   0        0        0     1141 2023-04-06 19:30:04.000000 starlette_web-0.1.2/starlette_web/tests/contrib/test_constance.py
--rw-rw-rw-   0        0        0      994 2023-03-17 18:16:19.000000 starlette_web-0.1.2/starlette_web/tests/contrib/test_password_validators.py
--rw-rw-rw-   0        0        0     1410 2023-03-27 19:00:45.000000 starlette_web-0.1.2/starlette_web/tests/contrib/test_redis_cache.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.457963 starlette_web-0.1.2/starlette_web/tests/core/
--rw-rw-rw-   0        0        0        0 2022-04-25 19:06:18.000000 starlette_web-0.1.2/starlette_web/tests/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.457963 starlette_web-0.1.2/starlette_web/tests/core/helpers/
--rw-rw-rw-   0        0        0        0 2023-03-22 16:53:00.000000 starlette_web-0.1.2/starlette_web/tests/core/helpers/__init__.py
--rw-rw-rw-   0        0        0     4350 2023-03-30 21:26:53.000000 starlette_web-0.1.2/starlette_web/tests/core/helpers/base_cache_tester.py
--rw-rw-rw-   0        0        0     5553 2023-02-26 15:17:30.000000 starlette_web-0.1.2/starlette_web/tests/core/test_auth_backends.py
--rw-rw-rw-   0        0        0     4741 2022-12-29 14:13:54.000000 starlette_web-0.1.2/starlette_web/tests/core/test_base.py
--rw-rw-rw-   0        0        0     1434 2023-03-27 18:28:47.000000 starlette_web-0.1.2/starlette_web/tests/core/test_base_caches.py
--rw-rw-rw-   0        0        0      867 2023-03-30 19:24:14.000000 starlette_web-0.1.2/starlette_web/tests/core/test_service.py
--rw-rw-rw-   0        0        0      528 2023-03-23 18:13:37.000000 starlette_web-0.1.2/starlette_web/tests/core/test_settings.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.457963 starlette_web-0.1.2/starlette_web/tests/database/
--rw-rw-rw-   0        0        0        0 2022-05-03 15:41:46.000000 starlette_web-0.1.2/starlette_web/tests/database/__init__.py
--rw-rw-rw-   0        0        0     4712 2022-05-09 11:25:06.000000 starlette_web-0.1.2/starlette_web/tests/database/test_model_mixin.py
--rw-rw-rw-   0        0        0     1786 2023-02-26 15:17:30.000000 starlette_web-0.1.2/starlette_web/tests/database/test_nested_transaction.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.467066 starlette_web-0.1.2/starlette_web/tests/files/
--rw-rw-rw-   0        0        0        0 2023-03-29 21:09:33.000000 starlette_web-0.1.2/starlette_web/tests/files/__init__.py
--rw-rw-rw-   0        0        0     4532 2023-03-31 18:52:29.000000 starlette_web-0.1.2/starlette_web/tests/files/test_filesystem_storage.py
--rw-rw-rw-   0        0        0      911 2023-03-30 20:24:14.000000 starlette_web-0.1.2/starlette_web/tests/files/test_media_storage.py
--rw-rw-rw-   0        0        0     3432 2023-02-26 14:23:54.000000 starlette_web-0.1.2/starlette_web/tests/helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.307223 starlette_web-0.1.2/starlette_web/tests/management/
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.467066 starlette_web-0.1.2/starlette_web/tests/management/commands/
--rw-rw-rw-   0        0        0      287 2022-05-03 14:50:29.000000 starlette_web-0.1.2/starlette_web/tests/management/commands/test_call_command.py
--rw-rw-rw-   0        0        0     1229 2023-03-12 16:44:21.000000 starlette_web-0.1.2/starlette_web/tests/management/commands/test_channels_publisher.py
--rw-rw-rw-   0        0        0     1326 2023-03-12 16:44:21.000000 starlette_web-0.1.2/starlette_web/tests/management/commands/test_channels_subscriber.py
--rw-rw-rw-   0        0        0      672 2023-01-28 08:02:03.000000 starlette_web-0.1.2/starlette_web/tests/management/commands/test_db.py
--rw-rw-rw-   0        0        0      722 2023-03-26 10:31:10.000000 starlette_web-0.1.2/starlette_web/tests/management/commands/test_parser.py
--rw-rw-rw-   0        0        0     1089 2022-05-14 13:30:44.000000 starlette_web-0.1.2/starlette_web/tests/mocks.py
--rw-rw-rw-   0        0        0     1641 2023-04-13 18:29:48.000000 starlette_web-0.1.2/starlette_web/tests/routes.py
--rw-rw-rw-   0        0        0     4689 2023-04-06 19:58:52.000000 starlette_web-0.1.2/starlette_web/tests/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.476963 starlette_web-0.1.2/starlette_web/tests/utils/
--rw-rw-rw-   0        0        0        0 2022-04-25 19:06:18.000000 starlette_web-0.1.2/starlette_web/tests/utils/__init__.py
--rw-rw-rw-   0        0        0     2960 2023-03-18 20:17:51.000000 starlette_web-0.1.2/starlette_web/tests/utils/test_auth_hasher.py
--rw-rw-rw-   0        0        0      768 2022-05-09 11:25:06.000000 starlette_web-0.1.2/starlette_web/tests/utils/test_json.py
--rw-rw-rw-   0        0        0     1447 2023-03-22 16:53:00.000000 starlette_web-0.1.2/starlette_web/tests/utils/test_redis_pattern_matcher.py
--rw-rw-rw-   0        0        0     1023 2022-05-09 11:25:06.000000 starlette_web-0.1.2/starlette_web/tests/utils/test_serializers.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.476963 starlette_web-0.1.2/starlette_web/tests/views/
--rw-rw-rw-   0        0        0      375 2023-03-23 18:10:52.000000 starlette_web-0.1.2/starlette_web/tests/views/__init__.py
--rw-rw-rw-   0        0        0     2098 2023-03-23 18:10:52.000000 starlette_web-0.1.2/starlette_web/tests/views/http.py
--rw-rw-rw-   0        0        0     6815 2023-03-26 09:54:37.000000 starlette_web-0.1.2/starlette_web/tests/views/websocket.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.476963 starlette_web-0.1.2/starlette_web/tests/websockets/
--rw-rw-rw-   0        0        0     2027 2023-03-12 16:44:21.000000 starlette_web-0.1.2/starlette_web/tests/websockets/test_websocket_chat.py
--rw-rw-rw-   0        0        0     7314 2023-03-15 20:43:06.000000 starlette_web-0.1.2/starlette_web/tests/websockets/test_websocket_endpoint.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:30:56.317238 starlette_web-0.1.2/starlette_web.egg-info/
--rw-rw-rw-   0        0        0     3245 2023-04-13 19:30:56.000000 starlette_web-0.1.2/starlette_web.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9087 2023-04-13 19:30:56.000000 starlette_web-0.1.2/starlette_web.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 19:30:56.000000 starlette_web-0.1.2/starlette_web.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-04-13 19:30:56.000000 starlette_web-0.1.2/starlette_web.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      817 2023-04-13 19:30:56.000000 starlette_web-0.1.2/starlette_web.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-13 19:30:56.000000 starlette_web-0.1.2/starlette_web.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.318779 starlette_web-0.1.3/
+-rw-rw-rw-   0        0        0     1108 2023-04-15 07:48:43.000000 starlette_web-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0       75 2023-04-13 19:30:53.000000 starlette_web-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3430 2023-04-15 08:29:36.318779 starlette_web-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2329 2023-03-26 13:41:03.000000 starlette_web-0.1.3/README.md
+-rw-rw-rw-   0        0        0     2382 2023-04-15 08:29:19.000000 starlette_web-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-15 08:29:36.318779 starlette_web-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.177866 starlette_web-0.1.3/starlette_web/
+-rw-rw-rw-   0        0        0       23 2022-12-29 14:13:54.000000 starlette_web-0.1.3/starlette_web/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.187874 starlette_web-0.1.3/starlette_web/common/
+-rw-rw-rw-   0        0        0       52 2022-04-25 19:06:18.000000 starlette_web-0.1.3/starlette_web/common/__init__.py
+-rw-rw-rw-   0        0        0     5348 2023-03-30 21:26:53.000000 starlette_web-0.1.3/starlette_web/common/app.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.190724 starlette_web-0.1.3/starlette_web/common/authorization/
+-rw-rw-rw-   0        0        0        0 2022-12-31 10:33:26.000000 starlette_web-0.1.3/starlette_web/common/authorization/__init__.py
+-rw-rw-rw-   0        0        0      856 2023-03-25 08:05:20.000000 starlette_web-0.1.3/starlette_web/common/authorization/backends.py
+-rw-rw-rw-   0        0        0      329 2023-03-25 08:05:20.000000 starlette_web-0.1.3/starlette_web/common/authorization/base_user.py
+-rw-rw-rw-   0        0        0     3025 2023-03-25 08:05:20.000000 starlette_web-0.1.3/starlette_web/common/authorization/permissions.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.193718 starlette_web-0.1.3/starlette_web/common/caches/
+-rw-rw-rw-   0        0        0       80 2023-03-16 18:44:56.000000 starlette_web-0.1.3/starlette_web/common/caches/__init__.py
+-rw-rw-rw-   0        0        0     2162 2023-03-25 08:05:20.000000 starlette_web-0.1.3/starlette_web/common/caches/base.py
+-rw-rw-rw-   0        0        0     3342 2023-04-01 08:01:57.000000 starlette_web-0.1.3/starlette_web/common/caches/base_lock.py
+-rw-rw-rw-   0        0        0     1112 2023-03-16 18:44:56.000000 starlette_web-0.1.3/starlette_web/common/caches/cache_handler.py
+-rw-rw-rw-   0        0        0     5241 2023-03-24 16:47:56.000000 starlette_web-0.1.3/starlette_web/common/caches/local_memory.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.195712 starlette_web-0.1.3/starlette_web/common/channels/
+-rw-rw-rw-   0        0        0       54 2023-03-12 16:44:21.000000 starlette_web-0.1.3/starlette_web/common/channels/__init__.py
+-rw-rw-rw-   0        0        0     4253 2023-04-01 19:06:23.000000 starlette_web-0.1.3/starlette_web/common/channels/base.py
+-rw-rw-rw-   0        0        0      447 2023-03-12 16:44:21.000000 starlette_web-0.1.3/starlette_web/common/channels/event.py
+-rw-rw-rw-   0        0        0      181 2023-03-22 16:38:31.000000 starlette_web-0.1.3/starlette_web/common/channels/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.199702 starlette_web-0.1.3/starlette_web/common/channels/layers/
+-rw-rw-rw-   0        0        0        0 2023-03-12 16:44:21.000000 starlette_web-0.1.3/starlette_web/common/channels/layers/__init__.py
+-rw-rw-rw-   0        0        0      753 2023-03-12 16:44:21.000000 starlette_web-0.1.3/starlette_web/common/channels/layers/base.py
+-rw-rw-rw-   0        0        0     1694 2023-03-12 19:30:41.000000 starlette_web-0.1.3/starlette_web/common/channels/layers/local_memory.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.203153 starlette_web-0.1.3/starlette_web/common/conf/
+-rw-rw-rw-   0        0        0     2285 2023-03-30 21:26:53.000000 starlette_web-0.1.3/starlette_web/common/conf/__init__.py
+-rw-rw-rw-   0        0        0     3314 2023-04-13 17:27:54.000000 starlette_web-0.1.3/starlette_web/common/conf/app_manager.py
+-rw-rw-rw-   0        0        0      198 2023-03-03 17:32:15.000000 starlette_web-0.1.3/starlette_web/common/conf/base_app_config.py
+-rw-rw-rw-   0        0        0     1994 2023-04-15 07:17:45.000000 starlette_web-0.1.3/starlette_web/common/conf/global_settings.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.206147 starlette_web-0.1.3/starlette_web/common/database/
+-rw-rw-rw-   0        0        0      359 2022-05-09 11:25:06.000000 starlette_web-0.1.3/starlette_web/common/database/__init__.py
+-rw-rw-rw-   0        0        0     1362 2023-02-26 15:17:29.000000 starlette_web-0.1.3/starlette_web/common/database/columns.py
+-rw-rw-rw-   0        0        0       81 2022-05-09 11:25:06.000000 starlette_web-0.1.3/starlette_web/common/database/model_base.py
+-rw-rw-rw-   0        0        0     9279 2023-04-09 22:15:24.000000 starlette_web-0.1.3/starlette_web/common/database/model_mixin.py
+-rw-rw-rw-   0        0        0     1550 2023-02-17 20:43:07.000000 starlette_web-0.1.3/starlette_web/common/database/session_maker.py
+-rw-rw-rw-   0        0        0     2059 2023-02-18 12:47:03.000000 starlette_web-0.1.3/starlette_web/common/database/types.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.209138 starlette_web-0.1.3/starlette_web/common/email/
+-rw-rw-rw-   0        0        0      169 2022-05-22 18:14:32.000000 starlette_web-0.1.3/starlette_web/common/email/__init__.py
+-rw-rw-rw-   0        0        0     1604 2023-03-28 17:00:26.000000 starlette_web-0.1.3/starlette_web/common/email/base_sender.py
+-rw-rw-rw-   0        0        0     1770 2023-03-27 20:27:55.000000 starlette_web-0.1.3/starlette_web/common/email/email_manager.py
+-rw-rw-rw-   0        0        0     1728 2023-03-30 21:26:53.000000 starlette_web-0.1.3/starlette_web/common/email/smtp.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.210800 starlette_web-0.1.3/starlette_web/common/files/
+-rw-rw-rw-   0        0        0        0 2023-03-22 16:53:00.000000 starlette_web-0.1.3/starlette_web/common/files/__init__.py
+-rw-rw-rw-   0        0        0     7085 2023-03-30 21:26:53.000000 starlette_web-0.1.3/starlette_web/common/files/cache.py
+-rw-rw-rw-   0        0        0     3837 2023-04-01 08:06:20.000000 starlette_web-0.1.3/starlette_web/common/files/filelock.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.212416 starlette_web-0.1.3/starlette_web/common/files/storages/
+-rw-rw-rw-   0        0        0      136 2023-03-30 20:24:14.000000 starlette_web-0.1.3/starlette_web/common/files/storages/__init__.py
+-rw-rw-rw-   0        0        0     6332 2023-03-31 18:48:34.000000 starlette_web-0.1.3/starlette_web/common/files/storages/base.py
+-rw-rw-rw-   0        0        0     4532 2023-04-01 16:31:26.000000 starlette_web-0.1.3/starlette_web/common/files/storages/filesystem.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.219803 starlette_web-0.1.3/starlette_web/common/http/
+-rw-rw-rw-   0        0        0        0 2022-05-03 08:01:50.000000 starlette_web-0.1.3/starlette_web/common/http/__init__.py
+-rw-rw-rw-   0        0        0     6650 2023-04-15 07:20:59.000000 starlette_web-0.1.3/starlette_web/common/http/base_endpoint.py
+-rw-rw-rw-   0        0        0     4338 2023-02-26 15:17:29.000000 starlette_web-0.1.3/starlette_web/common/http/exception_handlers.py
+-rw-rw-rw-   0        0        0     4287 2023-03-30 21:26:53.000000 starlette_web-0.1.3/starlette_web/common/http/exceptions.py
+-rw-rw-rw-   0        0        0     1075 2022-05-09 11:25:06.000000 starlette_web-0.1.3/starlette_web/common/http/renderers.py
+-rw-rw-rw-   0        0        0      336 2022-10-03 19:19:24.000000 starlette_web-0.1.3/starlette_web/common/http/responses.py
+-rw-rw-rw-   0        0        0     1174 2023-04-14 17:38:43.000000 starlette_web-0.1.3/starlette_web/common/http/schemas.py
+-rw-rw-rw-   0        0        0      942 2023-03-14 17:15:47.000000 starlette_web-0.1.3/starlette_web/common/http/statuses.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.220388 starlette_web-0.1.3/starlette_web/common/i18n/
+-rw-rw-rw-   0        0        0      163 2022-09-03 15:11:31.000000 starlette_web-0.1.3/starlette_web/common/i18n/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.223045 starlette_web-0.1.3/starlette_web/common/management/
+-rw-rw-rw-   0        0        0        0 2022-12-31 10:33:26.000000 starlette_web-0.1.3/starlette_web/common/management/__init__.py
+-rw-rw-rw-   0        0        0     1489 2023-04-15 07:46:58.000000 starlette_web-0.1.3/starlette_web/common/management/admin_util.py
+-rw-rw-rw-   0        0        0     1080 2023-04-06 12:18:07.000000 starlette_web-0.1.3/starlette_web/common/management/alembic_mixin.py
+-rw-rw-rw-   0        0        0     6023 2023-04-13 17:02:30.000000 starlette_web-0.1.3/starlette_web/common/management/base.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.226010 starlette_web-0.1.3/starlette_web/common/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-03-21 19:56:59.000000 starlette_web-0.1.3/starlette_web/common/management/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.233019 starlette_web-0.1.3/starlette_web/common/management/commands/_app_defaults/
+-rw-rw-rw-   0        0        0        0 2023-03-26 18:53:46.000000 starlette_web-0.1.3/starlette_web/common/management/commands/_app_defaults/__init__.py
+-rw-rw-rw-   0        0        0      376 2023-03-26 18:59:14.000000 starlette_web-0.1.3/starlette_web/common/management/commands/_app_defaults/admin.py
+-rw-rw-rw-   0        0        0      224 2023-03-26 18:55:02.000000 starlette_web-0.1.3/starlette_web/common/management/commands/_app_defaults/apps.py
+-rw-rw-rw-   0        0        0      297 2023-03-26 18:59:20.000000 starlette_web-0.1.3/starlette_web/common/management/commands/_app_defaults/models.py
+-rw-rw-rw-   0        0        0       95 2023-03-26 19:00:40.000000 starlette_web-0.1.3/starlette_web/common/management/commands/_app_defaults/routes.py
+-rw-rw-rw-   0        0        0      154 2023-03-26 19:00:00.000000 starlette_web-0.1.3/starlette_web/common/management/commands/_app_defaults/views.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.235016 starlette_web-0.1.3/starlette_web/common/management/commands/_project_defaults/
+-rw-rw-rw-   0        0        0        0 2023-03-26 17:54:43.000000 starlette_web-0.1.3/starlette_web/common/management/commands/_project_defaults/__init__.py
+-rw-rw-rw-   0        0        0      466 2023-04-03 20:19:20.000000 starlette_web-0.1.3/starlette_web/common/management/commands/_project_defaults/asgi.py
+-rw-rw-rw-   0        0        0      896 2023-03-26 17:36:41.000000 starlette_web-0.1.3/starlette_web/common/management/commands/_project_defaults/command.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.237035 starlette_web-0.1.3/starlette_web/common/management/commands/_project_defaults/core/
+-rw-rw-rw-   0        0        0        0 2022-04-25 19:06:18.000000 starlette_web-0.1.3/starlette_web/common/management/commands/_project_defaults/core/__init__.py
+-rw-rw-rw-   0        0        0      885 2023-04-13 18:30:43.000000 starlette_web-0.1.3/starlette_web/common/management/commands/_project_defaults/core/routes.py
+-rw-rw-rw-   0        0        0     3354 2023-04-14 17:40:54.000000 starlette_web-0.1.3/starlette_web/common/management/commands/_project_defaults/core/settings.py
+-rw-rw-rw-   0        0        0     1552 2023-04-06 16:46:50.000000 starlette_web-0.1.3/starlette_web/common/management/commands/makemigrations.py
+-rw-rw-rw-   0        0        0     1294 2023-04-06 16:46:56.000000 starlette_web-0.1.3/starlette_web/common/management/commands/migrate.py
+-rw-rw-rw-   0        0        0     2171 2023-03-30 21:26:53.000000 starlette_web-0.1.3/starlette_web/common/management/commands/startapp.py
+-rw-rw-rw-   0        0        0     3800 2023-04-06 16:47:27.000000 starlette_web-0.1.3/starlette_web/common/management/commands/startproject.py
+-rw-rw-rw-   0        0        0     2019 2023-04-08 06:35:50.000000 starlette_web-0.1.3/starlette_web/common/management/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.242995 starlette_web-0.1.3/starlette_web/common/utils/
+-rw-rw-rw-   0        0        0      506 2023-04-01 19:36:50.000000 starlette_web-0.1.3/starlette_web/common/utils/__init__.py
+-rw-rw-rw-   0        0        0     2578 2022-09-03 15:11:31.000000 starlette_web-0.1.3/starlette_web/common/utils/choices.py
+-rw-rw-rw-   0        0        0     1265 2023-03-18 14:43:23.000000 starlette_web-0.1.3/starlette_web/common/utils/crypto.py
+-rw-rw-rw-   0        0        0      187 2023-04-01 19:33:59.000000 starlette_web-0.1.3/starlette_web/common/utils/encoding.py
+-rw-rw-rw-   0        0        0      633 2023-02-17 20:46:29.000000 starlette_web-0.1.3/starlette_web/common/utils/importing.py
+-rw-rw-rw-   0        0        0      546 2023-03-30 21:26:53.000000 starlette_web-0.1.3/starlette_web/common/utils/inspect.py
+-rw-rw-rw-   0        0        0     2324 2022-05-09 11:25:06.000000 starlette_web-0.1.3/starlette_web/common/utils/json.py
+-rw-rw-rw-   0        0        0     2273 2023-03-30 21:26:53.000000 starlette_web-0.1.3/starlette_web/common/utils/regex.py
+-rw-rw-rw-   0        0        0     1828 2023-03-25 08:05:10.000000 starlette_web-0.1.3/starlette_web/common/utils/serializers.py
+-rw-rw-rw-   0        0        0      246 2022-05-09 11:25:06.000000 starlette_web-0.1.3/starlette_web/common/utils/singleton.py
+-rw-rw-rw-   0        0        0      217 2022-10-03 19:19:24.000000 starlette_web-0.1.3/starlette_web/common/utils/urls.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.243992 starlette_web-0.1.3/starlette_web/common/ws/
+-rw-rw-rw-   0        0        0        0 2022-12-29 14:13:54.000000 starlette_web-0.1.3/starlette_web/common/ws/__init__.py
+-rw-rw-rw-   0        0        0     6919 2023-03-14 17:15:47.000000 starlette_web-0.1.3/starlette_web/common/ws/base_endpoint.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.247013 starlette_web-0.1.3/starlette_web/contrib/
+-rw-rw-rw-   0        0        0        0 2022-05-09 11:25:06.000000 starlette_web-0.1.3/starlette_web/contrib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.249976 starlette_web-0.1.3/starlette_web/contrib/admin/
+-rw-rw-rw-   0        0        0      185 2023-02-26 15:17:29.000000 starlette_web-0.1.3/starlette_web/contrib/admin/__init__.py
+-rw-rw-rw-   0        0        0     3705 2023-03-24 18:55:03.000000 starlette_web-0.1.3/starlette_web/contrib/admin/admin.py
+-rw-rw-rw-   0        0        0      564 2023-03-03 17:32:15.000000 starlette_web-0.1.3/starlette_web/contrib/admin/apps.py
+-rw-rw-rw-   0        0        0     2780 2023-02-26 15:17:29.000000 starlette_web-0.1.3/starlette_web/contrib/admin/auth_provider.py
+-rw-rw-rw-   0        0        0     5122 2023-03-18 20:17:51.000000 starlette_web-0.1.3/starlette_web/contrib/admin/middleware.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.252973 starlette_web-0.1.3/starlette_web/contrib/apispec/
+-rw-rw-rw-   0        0        0        0 2022-10-03 19:19:24.000000 starlette_web-0.1.3/starlette_web/contrib/apispec/__init__.py
+-rw-rw-rw-   0        0        0     2017 2023-04-03 20:01:29.000000 starlette_web-0.1.3/starlette_web/contrib/apispec/apps.py
+-rw-rw-rw-   0        0        0     5451 2023-03-03 17:32:15.000000 starlette_web-0.1.3/starlette_web/contrib/apispec/introspection.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.254001 starlette_web-0.1.3/starlette_web/contrib/apispec/marshmallow/
+-rw-rw-rw-   0        0        0      352 2022-10-03 19:19:24.000000 starlette_web-0.1.3/starlette_web/contrib/apispec/marshmallow/__init__.py
+-rw-rw-rw-   0        0        0     1545 2022-10-03 19:19:24.000000 starlette_web-0.1.3/starlette_web/contrib/apispec/marshmallow/converters.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.169232 starlette_web-0.1.3/starlette_web/contrib/apispec/static/
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.254001 starlette_web-0.1.3/starlette_web/contrib/apispec/static/apispec/
+-rw-rw-rw-   0        0        0   879592 2022-10-03 19:19:24.000000 starlette_web-0.1.3/starlette_web/contrib/apispec/static/apispec/redoc.js
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.169232 starlette_web-0.1.3/starlette_web/contrib/apispec/templates/
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.255891 starlette_web-0.1.3/starlette_web/contrib/apispec/templates/apispec/
+-rw-rw-rw-   0        0        0      539 2022-10-03 19:19:24.000000 starlette_web-0.1.3/starlette_web/contrib/apispec/templates/apispec/redoc.html
+-rw-rw-rw-   0        0        0     1889 2023-04-13 18:25:49.000000 starlette_web-0.1.3/starlette_web/contrib/apispec/views.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.264264 starlette_web-0.1.3/starlette_web/contrib/auth/
+-rw-rw-rw-   0        0        0        0 2023-04-13 17:15:05.000000 starlette_web-0.1.3/starlette_web/contrib/auth/__init__.py
+-rw-rw-rw-   0        0        0     3484 2023-02-26 16:10:52.000000 starlette_web-0.1.3/starlette_web/contrib/auth/admin.py
+-rw-rw-rw-   0        0        0      261 2023-03-17 18:16:19.000000 starlette_web-0.1.3/starlette_web/contrib/auth/apps.py
+-rw-rw-rw-   0        0        0     4299 2023-02-26 15:17:29.000000 starlette_web-0.1.3/starlette_web/contrib/auth/backend.py
+-rw-rw-rw-   0        0        0     3981 2023-03-25 08:05:10.000000 starlette_web-0.1.3/starlette_web/contrib/auth/hashers.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.266226 starlette_web-0.1.3/starlette_web/contrib/auth/management/
+-rw-rw-rw-   0        0        0        0 2023-02-26 15:17:29.000000 starlette_web-0.1.3/starlette_web/contrib/auth/management/__init__.py
+-rw-rw-rw-   0        0        0     1308 2023-04-01 16:41:19.000000 starlette_web-0.1.3/starlette_web/contrib/auth/management/auth_command_mixin.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.267291 starlette_web-0.1.3/starlette_web/contrib/auth/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-02-26 15:17:29.000000 starlette_web-0.1.3/starlette_web/contrib/auth/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     1428 2023-04-01 16:41:42.000000 starlette_web-0.1.3/starlette_web/contrib/auth/management/commands/changepassword.py
+-rw-rw-rw-   0        0        0     1459 2023-04-01 16:41:42.000000 starlette_web-0.1.3/starlette_web/contrib/auth/management/commands/createsuperuser.py
+-rw-rw-rw-   0        0        0     3192 2023-02-26 15:17:30.000000 starlette_web-0.1.3/starlette_web/contrib/auth/models.py
+-rw-rw-rw-   0        0        0     3057 2023-03-18 20:17:51.000000 starlette_web-0.1.3/starlette_web/contrib/auth/password_validation.py
+-rw-rw-rw-   0        0        0      624 2023-02-26 15:17:30.000000 starlette_web-0.1.3/starlette_web/contrib/auth/permissions.py
+-rw-rw-rw-   0        0        0      654 2022-05-09 11:25:06.000000 starlette_web-0.1.3/starlette_web/contrib/auth/routes.py
+-rw-rw-rw-   0        0        0     2724 2022-10-01 11:03:47.000000 starlette_web-0.1.3/starlette_web/contrib/auth/schemas.py
+-rw-rw-rw-   0        0        0     1414 2023-03-18 20:17:51.000000 starlette_web-0.1.3/starlette_web/contrib/auth/utils.py
+-rw-rw-rw-   0        0        0    18290 2023-03-30 21:26:53.000000 starlette_web-0.1.3/starlette_web/contrib/auth/views.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.267291 starlette_web-0.1.3/starlette_web/contrib/camel_case/
+-rw-rw-rw-   0        0        0      249 2022-05-03 14:50:29.000000 starlette_web-0.1.3/starlette_web/contrib/camel_case/__init__.py
+-rw-rw-rw-   0        0        0      389 2023-04-09 20:47:08.000000 starlette_web-0.1.3/starlette_web/contrib/camel_case/parser.py
+-rw-rw-rw-   0        0        0      262 2022-05-03 14:50:29.000000 starlette_web-0.1.3/starlette_web/contrib/camel_case/renderer.py
+-rw-rw-rw-   0        0        0     4103 2022-10-03 19:19:24.000000 starlette_web-0.1.3/starlette_web/contrib/camel_case/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.271291 starlette_web-0.1.3/starlette_web/contrib/constance/
+-rw-rw-rw-   0        0        0     3754 2023-04-06 19:52:27.000000 starlette_web-0.1.3/starlette_web/contrib/constance/__init__.py
+-rw-rw-rw-   0        0        0     1144 2023-04-06 20:13:04.000000 starlette_web-0.1.3/starlette_web/contrib/constance/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.271291 starlette_web-0.1.3/starlette_web/contrib/constance/backends/
+-rw-rw-rw-   0        0        0        0 2023-02-20 07:01:30.000000 starlette_web-0.1.3/starlette_web/contrib/constance/backends/__init__.py
+-rw-rw-rw-   0        0        0     1410 2023-04-06 19:49:34.000000 starlette_web-0.1.3/starlette_web/contrib/constance/backends/base.py
+-rw-rw-rw-   0        0        0     1656 2023-04-06 20:18:43.000000 starlette_web-0.1.3/starlette_web/contrib/constance/backends/caching_mixin.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.271291 starlette_web-0.1.3/starlette_web/contrib/constance/backends/database/
+-rw-rw-rw-   0        0        0     1717 2023-03-12 16:44:01.000000 starlette_web-0.1.3/starlette_web/contrib/constance/backends/database/__init__.py
+-rw-rw-rw-   0        0        0      152 2023-03-03 17:32:15.000000 starlette_web-0.1.3/starlette_web/contrib/constance/backends/database/apps.py
+-rw-rw-rw-   0        0        0      368 2023-03-12 16:44:01.000000 starlette_web-0.1.3/starlette_web/contrib/constance/backends/database/models.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.275292 starlette_web-0.1.3/starlette_web/contrib/postgres/
+-rw-rw-rw-   0        0        0        0 2023-03-12 16:44:21.000000 starlette_web-0.1.3/starlette_web/contrib/postgres/__init__.py
+-rw-rw-rw-   0        0        0     3535 2023-04-02 10:14:34.000000 starlette_web-0.1.3/starlette_web/contrib/postgres/channel_layers.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.275292 starlette_web-0.1.3/starlette_web/contrib/redis/
+-rw-rw-rw-   0        0        0      137 2022-05-14 13:30:44.000000 starlette_web-0.1.3/starlette_web/contrib/redis/__init__.py
+-rw-rw-rw-   0        0        0     4616 2023-04-01 19:37:06.000000 starlette_web-0.1.3/starlette_web/contrib/redis/cache.py
+-rw-rw-rw-   0        0        0     2261 2023-04-01 19:42:16.000000 starlette_web-0.1.3/starlette_web/contrib/redis/channel_layers.py
+-rw-rw-rw-   0        0        0     1196 2023-03-27 18:37:04.000000 starlette_web-0.1.3/starlette_web/contrib/redis/redislock.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.279315 starlette_web-0.1.3/starlette_web/contrib/scheduler/
+-rw-rw-rw-   0        0        0      133 2023-03-04 19:50:46.000000 starlette_web-0.1.3/starlette_web/contrib/scheduler/__init__.py
+-rw-rw-rw-   0        0        0     2217 2023-03-04 19:50:46.000000 starlette_web-0.1.3/starlette_web/contrib/scheduler/app_settings.py
+-rw-rw-rw-   0        0        0     2084 2023-04-03 20:00:17.000000 starlette_web-0.1.3/starlette_web/contrib/scheduler/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.283292 starlette_web-0.1.3/starlette_web/contrib/scheduler/backends/
+-rw-rw-rw-   0        0        0      843 2023-03-31 19:10:23.000000 starlette_web-0.1.3/starlette_web/contrib/scheduler/backends/__init__.py
+-rw-rw-rw-   0        0        0     3867 2023-04-09 17:22:30.000000 starlette_web-0.1.3/starlette_web/contrib/scheduler/backends/base.py
+-rw-rw-rw-   0        0        0     2629 2023-03-31 19:15:23.000000 starlette_web-0.1.3/starlette_web/contrib/scheduler/backends/posix.py
+-rw-rw-rw-   0        0        0     7287 2023-03-31 19:15:38.000000 starlette_web-0.1.3/starlette_web/contrib/scheduler/backends/win32.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.283292 starlette_web-0.1.3/starlette_web/contrib/scheduler/management/
+-rw-rw-rw-   0        0        0        0 2023-03-04 19:50:46.000000 starlette_web-0.1.3/starlette_web/contrib/scheduler/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.283292 starlette_web-0.1.3/starlette_web/contrib/scheduler/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-03-04 19:50:46.000000 starlette_web-0.1.3/starlette_web/contrib/scheduler/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     1432 2023-03-31 19:14:46.000000 starlette_web-0.1.3/starlette_web/contrib/scheduler/management/commands/scheduler.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.287316 starlette_web-0.1.3/starlette_web/contrib/staticfiles/
+-rw-rw-rw-   0        0        0        0 2023-03-03 17:32:15.000000 starlette_web-0.1.3/starlette_web/contrib/staticfiles/__init__.py
+-rw-rw-rw-   0        0        0      136 2023-03-03 17:32:15.000000 starlette_web-0.1.3/starlette_web/contrib/staticfiles/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.287316 starlette_web-0.1.3/starlette_web/contrib/staticfiles/management/
+-rw-rw-rw-   0        0        0        0 2023-03-03 17:32:15.000000 starlette_web-0.1.3/starlette_web/contrib/staticfiles/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.287316 starlette_web-0.1.3/starlette_web/contrib/staticfiles/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-03-03 17:32:15.000000 starlette_web-0.1.3/starlette_web/contrib/staticfiles/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     4229 2023-03-03 17:32:15.000000 starlette_web-0.1.3/starlette_web/contrib/staticfiles/management/commands/collectstatic.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.291318 starlette_web-0.1.3/starlette_web/tests/
+-rw-rw-rw-   0        0        0        0 2022-04-25 19:06:18.000000 starlette_web-0.1.3/starlette_web/tests/__init__.py
+-rw-rw-rw-   0        0        0      202 2023-03-03 17:32:15.000000 starlette_web-0.1.3/starlette_web/tests/apps.py
+-rw-rw-rw-   0        0        0     5474 2023-04-06 20:04:06.000000 starlette_web-0.1.3/starlette_web/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.298777 starlette_web-0.1.3/starlette_web/tests/contrib/
+-rw-rw-rw-   0        0        0        0 2022-05-03 14:50:29.000000 starlette_web-0.1.3/starlette_web/tests/contrib/__init__.py
+-rw-rw-rw-   0        0        0    16572 2023-04-13 18:40:01.000000 starlette_web-0.1.3/starlette_web/tests/contrib/test_apispec.py
+-rw-rw-rw-   0        0        0    27613 2023-03-30 19:24:14.000000 starlette_web-0.1.3/starlette_web/tests/contrib/test_auth.py
+-rw-rw-rw-   0        0        0     1966 2022-05-03 14:50:29.000000 starlette_web-0.1.3/starlette_web/tests/contrib/test_camel_case.py
+-rw-rw-rw-   0        0        0     7677 2023-04-05 19:51:46.000000 starlette_web-0.1.3/starlette_web/tests/contrib/test_channels.py
+-rw-rw-rw-   0        0        0     1141 2023-04-06 19:30:04.000000 starlette_web-0.1.3/starlette_web/tests/contrib/test_constance.py
+-rw-rw-rw-   0        0        0      994 2023-03-17 18:16:19.000000 starlette_web-0.1.3/starlette_web/tests/contrib/test_password_validators.py
+-rw-rw-rw-   0        0        0     1410 2023-03-27 19:00:45.000000 starlette_web-0.1.3/starlette_web/tests/contrib/test_redis_cache.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.302780 starlette_web-0.1.3/starlette_web/tests/core/
+-rw-rw-rw-   0        0        0        0 2022-04-25 19:06:18.000000 starlette_web-0.1.3/starlette_web/tests/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.302780 starlette_web-0.1.3/starlette_web/tests/core/helpers/
+-rw-rw-rw-   0        0        0        0 2023-03-22 16:53:00.000000 starlette_web-0.1.3/starlette_web/tests/core/helpers/__init__.py
+-rw-rw-rw-   0        0        0     4350 2023-03-30 21:26:53.000000 starlette_web-0.1.3/starlette_web/tests/core/helpers/base_cache_tester.py
+-rw-rw-rw-   0        0        0     5553 2023-02-26 15:17:30.000000 starlette_web-0.1.3/starlette_web/tests/core/test_auth_backends.py
+-rw-rw-rw-   0        0        0     4741 2022-12-29 14:13:54.000000 starlette_web-0.1.3/starlette_web/tests/core/test_base.py
+-rw-rw-rw-   0        0        0     1434 2023-03-27 18:28:47.000000 starlette_web-0.1.3/starlette_web/tests/core/test_base_caches.py
+-rw-rw-rw-   0        0        0      867 2023-03-30 19:24:14.000000 starlette_web-0.1.3/starlette_web/tests/core/test_service.py
+-rw-rw-rw-   0        0        0      528 2023-03-23 18:13:37.000000 starlette_web-0.1.3/starlette_web/tests/core/test_settings.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.302780 starlette_web-0.1.3/starlette_web/tests/database/
+-rw-rw-rw-   0        0        0        0 2022-05-03 15:41:46.000000 starlette_web-0.1.3/starlette_web/tests/database/__init__.py
+-rw-rw-rw-   0        0        0     4712 2022-05-09 11:25:06.000000 starlette_web-0.1.3/starlette_web/tests/database/test_model_mixin.py
+-rw-rw-rw-   0        0        0     1786 2023-02-26 15:17:30.000000 starlette_web-0.1.3/starlette_web/tests/database/test_nested_transaction.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.306780 starlette_web-0.1.3/starlette_web/tests/files/
+-rw-rw-rw-   0        0        0        0 2023-03-29 21:09:33.000000 starlette_web-0.1.3/starlette_web/tests/files/__init__.py
+-rw-rw-rw-   0        0        0     4532 2023-03-31 18:52:29.000000 starlette_web-0.1.3/starlette_web/tests/files/test_filesystem_storage.py
+-rw-rw-rw-   0        0        0      911 2023-03-30 20:24:14.000000 starlette_web-0.1.3/starlette_web/tests/files/test_media_storage.py
+-rw-rw-rw-   0        0        0     3432 2023-02-26 14:23:54.000000 starlette_web-0.1.3/starlette_web/tests/helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.175212 starlette_web-0.1.3/starlette_web/tests/management/
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.306780 starlette_web-0.1.3/starlette_web/tests/management/commands/
+-rw-rw-rw-   0        0        0      287 2022-05-03 14:50:29.000000 starlette_web-0.1.3/starlette_web/tests/management/commands/test_call_command.py
+-rw-rw-rw-   0        0        0     1229 2023-03-12 16:44:21.000000 starlette_web-0.1.3/starlette_web/tests/management/commands/test_channels_publisher.py
+-rw-rw-rw-   0        0        0     1326 2023-03-12 16:44:21.000000 starlette_web-0.1.3/starlette_web/tests/management/commands/test_channels_subscriber.py
+-rw-rw-rw-   0        0        0      672 2023-01-28 08:02:03.000000 starlette_web-0.1.3/starlette_web/tests/management/commands/test_db.py
+-rw-rw-rw-   0        0        0      722 2023-03-26 10:31:10.000000 starlette_web-0.1.3/starlette_web/tests/management/commands/test_parser.py
+-rw-rw-rw-   0        0        0     1089 2022-05-14 13:30:44.000000 starlette_web-0.1.3/starlette_web/tests/mocks.py
+-rw-rw-rw-   0        0        0     1641 2023-04-13 18:29:48.000000 starlette_web-0.1.3/starlette_web/tests/routes.py
+-rw-rw-rw-   0        0        0     4602 2023-04-14 17:40:22.000000 starlette_web-0.1.3/starlette_web/tests/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.314780 starlette_web-0.1.3/starlette_web/tests/utils/
+-rw-rw-rw-   0        0        0        0 2022-04-25 19:06:18.000000 starlette_web-0.1.3/starlette_web/tests/utils/__init__.py
+-rw-rw-rw-   0        0        0     2960 2023-03-18 20:17:51.000000 starlette_web-0.1.3/starlette_web/tests/utils/test_auth_hasher.py
+-rw-rw-rw-   0        0        0      768 2022-05-09 11:25:06.000000 starlette_web-0.1.3/starlette_web/tests/utils/test_json.py
+-rw-rw-rw-   0        0        0     1447 2023-03-22 16:53:00.000000 starlette_web-0.1.3/starlette_web/tests/utils/test_redis_pattern_matcher.py
+-rw-rw-rw-   0        0        0     1023 2022-05-09 11:25:06.000000 starlette_web-0.1.3/starlette_web/tests/utils/test_serializers.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.314780 starlette_web-0.1.3/starlette_web/tests/views/
+-rw-rw-rw-   0        0        0      375 2023-03-23 18:10:52.000000 starlette_web-0.1.3/starlette_web/tests/views/__init__.py
+-rw-rw-rw-   0        0        0     2098 2023-03-23 18:10:52.000000 starlette_web-0.1.3/starlette_web/tests/views/http.py
+-rw-rw-rw-   0        0        0     6847 2023-04-14 17:57:54.000000 starlette_web-0.1.3/starlette_web/tests/views/websocket.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.318779 starlette_web-0.1.3/starlette_web/tests/websockets/
+-rw-rw-rw-   0        0        0     2027 2023-03-12 16:44:21.000000 starlette_web-0.1.3/starlette_web/tests/websockets/test_websocket_chat.py
+-rw-rw-rw-   0        0        0     7314 2023-03-15 20:43:06.000000 starlette_web-0.1.3/starlette_web/tests/websockets/test_websocket_endpoint.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.187313 starlette_web-0.1.3/starlette_web.egg-info/
+-rw-rw-rw-   0        0        0     3430 2023-04-15 08:29:36.000000 starlette_web-0.1.3/starlette_web.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9083 2023-04-15 08:29:36.000000 starlette_web-0.1.3/starlette_web.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 08:29:36.000000 starlette_web-0.1.3/starlette_web.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-04-15 08:29:36.000000 starlette_web-0.1.3/starlette_web.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      933 2023-04-15 08:29:36.000000 starlette_web-0.1.3/starlette_web.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       73 2023-04-15 08:29:36.000000 starlette_web-0.1.3/starlette_web.egg-info/top_level.txt
```

### Comparing `starlette_web-0.1.2/LICENSE` & `starlette_web-0.1.3/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Dmitry Burnaev
+Copyright (c) 2022 Sergey Sayamov, Dmitry Burnaev
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `starlette_web-0.1.2/PKG-INFO` & `starlette_web-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 Metadata-Version: 2.1
 Name: starlette_web
-Version: 0.1.2
+Version: 0.1.3
 Summary: Asynchronous web framework, based on Starlette and inspired by Django
-Home-page: https://github.com/dolamroth/starlette-web
-Author: Sergey Sayamov
-Author-email: dolamroth@mail.ru
-License: MIT License
-Download-URL: https://github.com/dolamroth/starlette-web/archive/refs/tags/0.1.2.tar.gz
-Platform: UNKNOWN
+Author-email: Sergey Sayamov <dolamroth@mail.ru>, Dmitry Burnaev <dmitry.burnaev@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/dolamroth/starlette-web
+Project-URL: Issues, https://github.com/dolamroth/starlette-web/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.9
+Description-Content-Type: text/markdown
 Provides-Extra: apispec
 Provides-Extra: admin
 Provides-Extra: auth
 Provides-Extra: postgres
 Provides-Extra: redis
 Provides-Extra: scheduler
 Provides-Extra: deploy
 Provides-Extra: develop
 Provides-Extra: testing
+Provides-Extra: all
+Provides-Extra: full
 License-File: LICENSE
 
 ## starlette_web
 
 `starlette_web` is a native-asynchronous web-framework, based on [Starlette](https://www.starlette.io/) 
 and inspired by [Django](https://www.djangoproject.com/) and its ecosystem.
 It aims to provide most of the relevant features of Django in async-all-the-way setting.
@@ -61,9 +64,7 @@
 
 See tests for more examples of usage.
 
 ## Code borrowing
 
 starlette-web borrows/adopts a lot of code from other open-source Python libraries. 
 List of libraries is given in the [docs](./docs/borrowing.md), with links to repositories and licences.
-
-
```

### Comparing `starlette_web-0.1.2/README.md` & `starlette_web-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/app.py` & `starlette_web-0.1.3/starlette_web/common/app.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/authorization/backends.py` & `starlette_web-0.1.3/starlette_web/common/authorization/backends.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/authorization/permissions.py` & `starlette_web-0.1.3/starlette_web/common/authorization/permissions.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/caches/base.py` & `starlette_web-0.1.3/starlette_web/common/caches/base.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/caches/base_lock.py` & `starlette_web-0.1.3/starlette_web/common/caches/base_lock.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/caches/cache_handler.py` & `starlette_web-0.1.3/starlette_web/common/caches/cache_handler.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/caches/local_memory.py` & `starlette_web-0.1.3/starlette_web/common/caches/local_memory.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/channels/base.py` & `starlette_web-0.1.3/starlette_web/common/channels/base.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/channels/layers/base.py` & `starlette_web-0.1.3/starlette_web/common/channels/layers/base.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/channels/layers/local_memory.py` & `starlette_web-0.1.3/starlette_web/common/channels/layers/local_memory.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/conf/__init__.py` & `starlette_web-0.1.3/starlette_web/common/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/conf/app_manager.py` & `starlette_web-0.1.3/starlette_web/common/conf/app_manager.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/database/columns.py` & `starlette_web-0.1.3/starlette_web/common/database/columns.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/database/model_mixin.py` & `starlette_web-0.1.3/starlette_web/common/database/model_mixin.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/database/session_maker.py` & `starlette_web-0.1.3/starlette_web/common/database/session_maker.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/database/types.py` & `starlette_web-0.1.3/starlette_web/common/database/types.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/email/base_sender.py` & `starlette_web-0.1.3/starlette_web/common/email/base_sender.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/email/email_manager.py` & `starlette_web-0.1.3/starlette_web/common/email/email_manager.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/email/smtp.py` & `starlette_web-0.1.3/starlette_web/common/email/smtp.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/files/cache.py` & `starlette_web-0.1.3/starlette_web/common/files/cache.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/files/filelock.py` & `starlette_web-0.1.3/starlette_web/common/files/filelock.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/files/storages/base.py` & `starlette_web-0.1.3/starlette_web/common/files/storages/base.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/files/storages/filesystem.py` & `starlette_web-0.1.3/starlette_web/common/files/storages/filesystem.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/http/base_endpoint.py` & `starlette_web-0.1.3/starlette_web/common/http/base_endpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,23 +14,25 @@
 from starlette_web.common.app import WebApp
 from starlette_web.common.authorization.backends import (
     BaseAuthenticationBackend,
     NoAuthenticationBackend,
 )
 from starlette_web.common.authorization.permissions import PermissionType
 from starlette_web.common.authorization.base_user import AnonymousUser
+from starlette_web.common.conf import settings
 from starlette_web.common.http.exceptions import (
     UnexpectedError,
     BaseApplicationError,
     InvalidParameterError,
     PermissionDeniedError,
 )
-from starlette_web.common.http.renderers import BaseRenderer, JSONRenderer
+from starlette_web.common.http.renderers import BaseRenderer
 from starlette_web.common.http.statuses import ResponseStatus
 from starlette_web.common.database import DBModel
+from starlette_web.common.utils import import_string
 
 
 logger = logging.getLogger(__name__)
 
 
 class BaseHTTPEndpoint(HTTPEndpoint):
     """
@@ -40,21 +42,23 @@
     app = None
     request: Request
     db_session: AsyncSession
     request_schema: ClassVar[Type[Schema]]
     response_schema: ClassVar[Type[Schema]]
     auth_backend: ClassVar[Type[BaseAuthenticationBackend]] = NoAuthenticationBackend
     permission_classes: ClassVar[List[PermissionType]] = []
-    request_parser: ClassVar[Type[StarletteParser]] = StarletteParser
-    response_renderer: ClassVar[Type[BaseRenderer]] = JSONRenderer
+    request_parser: ClassVar[Type[StarletteParser]] = \
+        import_string(settings.DEFAULT_REQUEST_PARSER)
+    response_renderer: ClassVar[Type[BaseRenderer]] = \
+        import_string(settings.DEFAULT_RESPONSE_RENDERER)
 
     async def dispatch(self) -> None:
         """
-        This method is calling in every request.
-        So, we can use this one for customs authenticate and catch all exceptions
+        This method is called in every request.
+        So, we can use this one for custom authentication and exception handling
         """
 
         self.request = Request(self.scope, receive=self.receive)
         self.app: WebApp = self.scope.get("app")
 
         handler_name = "get" if self.request.method == "HEAD" else self.request.method.lower()
         handler = getattr(self, handler_name, self.method_not_allowed)
```

### Comparing `starlette_web-0.1.2/starlette_web/common/http/exception_handlers.py` & `starlette_web-0.1.3/starlette_web/common/http/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/http/exceptions.py` & `starlette_web-0.1.3/starlette_web/common/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/http/renderers.py` & `starlette_web-0.1.3/starlette_web/common/http/renderers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/http/statuses.py` & `starlette_web-0.1.3/starlette_web/common/http/statuses.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/management/admin_util.py` & `starlette_web-0.1.3/starlette_web/common/management/admin_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         for arg in sys_argv.copy():
             if arg.startswith("--settings="):
                 settings_module = arg[11:]
                 sys_argv.remove(arg)
 
         os.environ.setdefault("STARLETTE_SETTINGS_MODULE", settings_module)
 
-        if len(sys_argv) < 1:
+        if len(sys_argv) < 2:
             raise Exception(
                 'Missing command name. Correct syntax is: '
                 '"starlette-web-admin command_name ..."'
             )
 
         from starlette_web.common.conf import settings
         from starlette_web.common.app import get_app
```

### Comparing `starlette_web-0.1.2/starlette_web/common/management/alembic_mixin.py` & `starlette_web-0.1.3/starlette_web/common/management/alembic_mixin.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/management/base.py` & `starlette_web-0.1.3/starlette_web/common/management/base.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/management/commands/_project_defaults/command.py` & `starlette_web-0.1.3/starlette_web/common/management/commands/_project_defaults/command.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/management/commands/_project_defaults/core/routes.py` & `starlette_web-0.1.3/starlette_web/common/management/commands/_project_defaults/core/routes.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/management/commands/_project_defaults/core/settings.py` & `starlette_web-0.1.3/starlette_web/common/management/commands/_project_defaults/core/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,10 +110,9 @@
 APISPEC = {
     "CONFIG": dict(
         title="Project documentation",
         version="0.0.1",
         openapi_version="3.0.2",
         info=dict(description="My custom project."),
     ),
-    "ERROR_RESPONSE_SCHEMA": "starlette_web.common.http.schemas.ErrorResponseSchema",
     "CONVERT_TO_CAMEL_CASE": False,
 }
```

### Comparing `starlette_web-0.1.2/starlette_web/common/management/commands/makemigrations.py` & `starlette_web-0.1.3/starlette_web/common/management/commands/makemigrations.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/management/commands/migrate.py` & `starlette_web-0.1.3/starlette_web/common/management/commands/migrate.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/management/commands/startapp.py` & `starlette_web-0.1.3/starlette_web/common/management/commands/startapp.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/management/commands/startproject.py` & `starlette_web-0.1.3/starlette_web/common/management/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/management/utils.py` & `starlette_web-0.1.3/starlette_web/common/management/utils.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/utils/choices.py` & `starlette_web-0.1.3/starlette_web/common/utils/choices.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/utils/crypto.py` & `starlette_web-0.1.3/starlette_web/common/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/utils/importing.py` & `starlette_web-0.1.3/starlette_web/common/utils/importing.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/utils/inspect.py` & `starlette_web-0.1.3/starlette_web/common/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/utils/json.py` & `starlette_web-0.1.3/starlette_web/common/utils/json.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/utils/regex.py` & `starlette_web-0.1.3/starlette_web/common/utils/regex.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/utils/serializers.py` & `starlette_web-0.1.3/starlette_web/common/utils/serializers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/common/ws/base_endpoint.py` & `starlette_web-0.1.3/starlette_web/common/ws/base_endpoint.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/admin/admin.py` & `starlette_web-0.1.3/starlette_web/contrib/admin/admin.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/admin/apps.py` & `starlette_web-0.1.3/starlette_web/contrib/admin/apps.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/admin/auth_provider.py` & `starlette_web-0.1.3/starlette_web/contrib/admin/auth_provider.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/admin/middleware.py` & `starlette_web-0.1.3/starlette_web/contrib/admin/middleware.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/apispec/apps.py` & `starlette_web-0.1.3/starlette_web/contrib/apispec/apps.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/apispec/introspection.py` & `starlette_web-0.1.3/starlette_web/contrib/apispec/introspection.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/apispec/marshmallow/converters.py` & `starlette_web-0.1.3/starlette_web/contrib/apispec/marshmallow/converters.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/apispec/static/apispec/redoc.js` & `starlette_web-0.1.3/starlette_web/contrib/apispec/static/apispec/redoc.js`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/apispec/templates/apispec/redoc.html` & `starlette_web-0.1.3/starlette_web/contrib/apispec/templates/apispec/redoc.html`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/apispec/views.py` & `starlette_web-0.1.3/starlette_web/contrib/apispec/views.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/auth/admin.py` & `starlette_web-0.1.3/starlette_web/contrib/auth/admin.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/auth/backend.py` & `starlette_web-0.1.3/starlette_web/contrib/auth/backend.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/auth/hashers.py` & `starlette_web-0.1.3/starlette_web/contrib/auth/hashers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/auth/management/auth_command_mixin.py` & `starlette_web-0.1.3/starlette_web/contrib/auth/management/auth_command_mixin.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/auth/management/commands/changepassword.py` & `starlette_web-0.1.3/starlette_web/contrib/auth/management/commands/changepassword.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/auth/management/commands/createsuperuser.py` & `starlette_web-0.1.3/starlette_web/contrib/auth/management/commands/createsuperuser.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/auth/models.py` & `starlette_web-0.1.3/starlette_web/contrib/auth/models.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/auth/password_validation.py` & `starlette_web-0.1.3/starlette_web/contrib/auth/password_validation.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/auth/permissions.py` & `starlette_web-0.1.3/starlette_web/contrib/auth/permissions.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/auth/routes.py` & `starlette_web-0.1.3/starlette_web/contrib/auth/routes.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/auth/schemas.py` & `starlette_web-0.1.3/starlette_web/contrib/auth/schemas.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/auth/utils.py` & `starlette_web-0.1.3/starlette_web/contrib/auth/utils.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/auth/views.py` & `starlette_web-0.1.3/starlette_web/contrib/auth/views.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/camel_case/utils.py` & `starlette_web-0.1.3/starlette_web/contrib/camel_case/utils.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/constance/__init__.py` & `starlette_web-0.1.3/starlette_web/contrib/constance/__init__.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/constance/apps.py` & `starlette_web-0.1.3/starlette_web/contrib/constance/apps.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/constance/backends/base.py` & `starlette_web-0.1.3/starlette_web/contrib/constance/backends/base.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/constance/backends/caching_mixin.py` & `starlette_web-0.1.3/starlette_web/contrib/constance/backends/caching_mixin.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/constance/backends/database/__init__.py` & `starlette_web-0.1.3/starlette_web/contrib/constance/backends/database/__init__.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/postgres/channel_layers.py` & `starlette_web-0.1.3/starlette_web/contrib/postgres/channel_layers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/redis/cache.py` & `starlette_web-0.1.3/starlette_web/contrib/redis/cache.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/redis/channel_layers.py` & `starlette_web-0.1.3/starlette_web/contrib/redis/channel_layers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/redis/redislock.py` & `starlette_web-0.1.3/starlette_web/contrib/redis/redislock.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/scheduler/app_settings.py` & `starlette_web-0.1.3/starlette_web/contrib/scheduler/app_settings.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/scheduler/apps.py` & `starlette_web-0.1.3/starlette_web/contrib/scheduler/apps.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/scheduler/backends/__init__.py` & `starlette_web-0.1.3/starlette_web/contrib/scheduler/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/scheduler/backends/base.py` & `starlette_web-0.1.3/starlette_web/contrib/scheduler/backends/base.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/scheduler/backends/posix.py` & `starlette_web-0.1.3/starlette_web/contrib/scheduler/backends/posix.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/scheduler/backends/win32.py` & `starlette_web-0.1.3/starlette_web/contrib/scheduler/backends/win32.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/scheduler/management/commands/scheduler.py` & `starlette_web-0.1.3/starlette_web/contrib/scheduler/management/commands/scheduler.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/contrib/staticfiles/management/commands/collectstatic.py` & `starlette_web-0.1.3/starlette_web/contrib/staticfiles/management/commands/collectstatic.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/conftest.py` & `starlette_web-0.1.3/starlette_web/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/contrib/test_apispec.py` & `starlette_web-0.1.3/starlette_web/tests/contrib/test_apispec.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/contrib/test_auth.py` & `starlette_web-0.1.3/starlette_web/tests/contrib/test_auth.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/contrib/test_camel_case.py` & `starlette_web-0.1.3/starlette_web/tests/contrib/test_camel_case.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/contrib/test_channels.py` & `starlette_web-0.1.3/starlette_web/tests/contrib/test_channels.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/contrib/test_constance.py` & `starlette_web-0.1.3/starlette_web/tests/contrib/test_constance.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/contrib/test_password_validators.py` & `starlette_web-0.1.3/starlette_web/tests/contrib/test_password_validators.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/contrib/test_redis_cache.py` & `starlette_web-0.1.3/starlette_web/tests/contrib/test_redis_cache.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/core/helpers/base_cache_tester.py` & `starlette_web-0.1.3/starlette_web/tests/core/helpers/base_cache_tester.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/core/test_auth_backends.py` & `starlette_web-0.1.3/starlette_web/tests/core/test_auth_backends.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/core/test_base.py` & `starlette_web-0.1.3/starlette_web/tests/core/test_base.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/core/test_base_caches.py` & `starlette_web-0.1.3/starlette_web/tests/core/test_base_caches.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/core/test_service.py` & `starlette_web-0.1.3/starlette_web/tests/core/test_service.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/core/test_settings.py` & `starlette_web-0.1.3/starlette_web/tests/core/test_settings.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/database/test_model_mixin.py` & `starlette_web-0.1.3/starlette_web/tests/database/test_model_mixin.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/database/test_nested_transaction.py` & `starlette_web-0.1.3/starlette_web/tests/database/test_nested_transaction.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/files/test_filesystem_storage.py` & `starlette_web-0.1.3/starlette_web/tests/files/test_filesystem_storage.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/files/test_media_storage.py` & `starlette_web-0.1.3/starlette_web/tests/files/test_media_storage.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/helpers.py` & `starlette_web-0.1.3/starlette_web/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/management/commands/test_channels_publisher.py` & `starlette_web-0.1.3/starlette_web/tests/management/commands/test_channels_publisher.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/management/commands/test_channels_subscriber.py` & `starlette_web-0.1.3/starlette_web/tests/management/commands/test_channels_subscriber.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/management/commands/test_db.py` & `starlette_web-0.1.3/starlette_web/tests/management/commands/test_db.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/management/commands/test_parser.py` & `starlette_web-0.1.3/starlette_web/tests/management/commands/test_parser.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/mocks.py` & `starlette_web-0.1.3/starlette_web/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/routes.py` & `starlette_web-0.1.3/starlette_web/tests/routes.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/settings.py` & `starlette_web-0.1.3/starlette_web/tests/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,10 +137,9 @@
 APISPEC = {
     "CONFIG": dict(
         title="Project documentation",
         version="0.0.1",
         openapi_version="3.0.2",
         info=dict(description="My custom project."),
     ),
-    "ERROR_RESPONSE_SCHEMA": "starlette_web.common.http.schemas.ErrorResponseSchema",
     "CONVERT_TO_CAMEL_CASE": False,
 }
```

### Comparing `starlette_web-0.1.2/starlette_web/tests/utils/test_auth_hasher.py` & `starlette_web-0.1.3/starlette_web/tests/utils/test_auth_hasher.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/utils/test_json.py` & `starlette_web-0.1.3/starlette_web/tests/utils/test_json.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/utils/test_redis_pattern_matcher.py` & `starlette_web-0.1.3/starlette_web/tests/utils/test_redis_pattern_matcher.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/utils/test_serializers.py` & `starlette_web-0.1.3/starlette_web/tests/utils/test_serializers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/views/http.py` & `starlette_web-0.1.3/starlette_web/tests/views/http.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/views/websocket.py` & `starlette_web-0.1.3/starlette_web/tests/views/websocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,17 +136,18 @@
 
         room = "chatroom"
 
         if data["request_type"] == "publish":
             await self._channels.publish(room, data["message"])
 
         elif data["request_type"] == "connect":
-            # In test endpoint, unregister checks that there are any tasks left,
-            # before closing the channel. Since this parent task will close
-            # as soon it spawns dialogue task, we need to register the latter.
+            # In test endpoint, _unregister_background_task checks that
+            # there are any tasks left, before closing the channel.
+            # Since this parent task will close as soon
+            # it spawns dialogue task, we need to register the latter.
             dialogue_task_id = get_random_string(50)
             self._tasks.add(dialogue_task_id)
             self.task_group.start_soon(self._run_dialogue, websocket, room, dialogue_task_id)
 
         else:
             raise WebSocketDisconnect(code=1005, reason="Invalid request type")
```

### Comparing `starlette_web-0.1.2/starlette_web/tests/websockets/test_websocket_chat.py` & `starlette_web-0.1.3/starlette_web/tests/websockets/test_websocket_chat.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web/tests/websockets/test_websocket_endpoint.py` & `starlette_web-0.1.3/starlette_web/tests/websockets/test_websocket_endpoint.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.2/starlette_web.egg-info/PKG-INFO` & `starlette_web-0.1.3/starlette_web.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 Metadata-Version: 2.1
 Name: starlette-web
-Version: 0.1.2
+Version: 0.1.3
 Summary: Asynchronous web framework, based on Starlette and inspired by Django
-Home-page: https://github.com/dolamroth/starlette-web
-Author: Sergey Sayamov
-Author-email: dolamroth@mail.ru
-License: MIT License
-Download-URL: https://github.com/dolamroth/starlette-web/archive/refs/tags/0.1.2.tar.gz
-Platform: UNKNOWN
+Author-email: Sergey Sayamov <dolamroth@mail.ru>, Dmitry Burnaev <dmitry.burnaev@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/dolamroth/starlette-web
+Project-URL: Issues, https://github.com/dolamroth/starlette-web/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.9
+Description-Content-Type: text/markdown
 Provides-Extra: apispec
 Provides-Extra: admin
 Provides-Extra: auth
 Provides-Extra: postgres
 Provides-Extra: redis
 Provides-Extra: scheduler
 Provides-Extra: deploy
 Provides-Extra: develop
 Provides-Extra: testing
+Provides-Extra: all
+Provides-Extra: full
 License-File: LICENSE
 
 ## starlette_web
 
 `starlette_web` is a native-asynchronous web-framework, based on [Starlette](https://www.starlette.io/) 
 and inspired by [Django](https://www.djangoproject.com/) and its ecosystem.
 It aims to provide most of the relevant features of Django in async-all-the-way setting.
@@ -61,9 +64,7 @@
 
 See tests for more examples of usage.
 
 ## Code borrowing
 
 starlette-web borrows/adopts a lot of code from other open-source Python libraries. 
 List of libraries is given in the [docs](./docs/borrowing.md), with links to repositories and licences.
-
-
```

### Comparing `starlette_web-0.1.2/starlette_web.egg-info/SOURCES.txt` & `starlette_web-0.1.3/starlette_web.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
-setup.cfg
-setup.py
+pyproject.toml
 starlette_web/__init__.py
 starlette_web.egg-info/PKG-INFO
 starlette_web.egg-info/SOURCES.txt
 starlette_web.egg-info/dependency_links.txt
 starlette_web.egg-info/entry_points.txt
 starlette_web.egg-info/requires.txt
 starlette_web.egg-info/top_level.txt
```

