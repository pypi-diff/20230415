# Comparing `tmp/telegram_django_bot-1.0.1.tar.gz` & `tmp/telegram_django_bot-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_django_bot-1.0.1.tar", last modified: Sun Apr  9 07:46:20 2023, max compression
+gzip compressed data, was "telegram_django_bot-1.0.2.tar", last modified: Sat Apr 15 18:53:52 2023, max compression
```

## Comparing `telegram_django_bot-1.0.1.tar` & `telegram_django_bot-1.0.2.tar`

### file list

```diff
@@ -1,46 +1,53 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 07:46:20.765903 telegram_django_bot-1.0.1/
--rw-r--r--   0 alex       (501) staff       (20)     1073 2022-09-07 14:16:11.000000 telegram_django_bot-1.0.1/LICENSE
--rw-r--r--   0 alex       (501) staff       (20)      169 2023-01-17 13:23:14.000000 telegram_django_bot-1.0.1/MANIFEST.in
--rw-r--r--   0 alex       (501) staff       (20)    40224 2023-04-09 07:46:20.766386 telegram_django_bot-1.0.1/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)    38984 2023-04-09 07:32:50.000000 telegram_django_bot-1.0.1/README.rst
--rw-r--r--   0 alex       (501) staff       (20)     1302 2023-04-09 07:46:20.767911 telegram_django_bot-1.0.1/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)       39 2022-09-07 14:16:11.000000 telegram_django_bot-1.0.1/setup.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 07:46:20.753732 telegram_django_bot-1.0.1/telegram_django_bot/
--rw-r--r--   0 alex       (501) staff       (20)       72 2023-04-09 07:32:50.000000 telegram_django_bot-1.0.1/telegram_django_bot/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     4332 2023-04-09 07:45:25.000000 telegram_django_bot-1.0.1/telegram_django_bot/admin.py
--rw-r--r--   0 alex       (501) staff       (20)     1000 2023-04-09 07:21:01.000000 telegram_django_bot-1.0.1/telegram_django_bot/admin_utils.py
--rw-r--r--   0 alex       (501) staff       (20)      111 2023-01-17 12:17:05.000000 telegram_django_bot-1.0.1/telegram_django_bot/apps.py
--rw-r--r--   0 alex       (501) staff       (20)     6909 2023-04-09 07:32:50.000000 telegram_django_bot-1.0.1/telegram_django_bot/forms.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 07:46:20.743149 telegram_django_bot-1.0.1/telegram_django_bot/locale/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 07:46:20.743257 telegram_django_bot-1.0.1/telegram_django_bot/locale/ru/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 07:46:20.758104 telegram_django_bot-1.0.1/telegram_django_bot/locale/ru/LC_MESSAGES/
--rw-r--r--   0 alex       (501) staff       (20)     6042 2023-04-09 07:45:25.000000 telegram_django_bot-1.0.1/telegram_django_bot/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 alex       (501) staff       (20)     7478 2023-04-09 07:45:25.000000 telegram_django_bot-1.0.1/telegram_django_bot/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 07:46:20.764993 telegram_django_bot-1.0.1/telegram_django_bot/migrations/
--rw-r--r--   0 alex       (501) staff       (20)     9252 2022-09-07 14:16:11.000000 telegram_django_bot-1.0.1/telegram_django_bot/migrations/0001_initial.py
--rw-r--r--   0 alex       (501) staff       (20)      292 2022-09-07 14:16:11.000000 telegram_django_bot-1.0.1/telegram_django_bot/migrations/0002_delete_user.py
--rw-r--r--   0 alex       (501) staff       (20)      604 2022-09-07 14:16:11.000000 telegram_django_bot-1.0.1/telegram_django_bot/migrations/0003_botmenuelem_message_format.py
--rw-r--r--   0 alex       (501) staff       (20)     4613 2022-09-16 18:03:58.000000 telegram_django_bot-1.0.1/telegram_django_bot/migrations/0004_auto_20220915_0448.py
--rw-r--r--   0 alex       (501) staff       (20)      397 2022-10-10 18:30:54.000000 telegram_django_bot-1.0.1/telegram_django_bot/migrations/0005_auto_20221010_1330.py
--rw-r--r--   0 alex       (501) staff       (20)      478 2022-10-23 06:57:02.000000 telegram_django_bot-1.0.1/telegram_django_bot/migrations/0006_auto_20221023_0157.py
--rw-r--r--   0 alex       (501) staff       (20)      636 2022-12-02 09:05:36.000000 telegram_django_bot-1.0.1/telegram_django_bot/migrations/0007_auto_20221202_0305.py
--rw-r--r--   0 alex       (501) staff       (20)     1626 2023-01-17 12:17:05.000000 telegram_django_bot-1.0.1/telegram_django_bot/migrations/0008_auto_20221225_1050.py
--rw-r--r--   0 alex       (501) staff       (20)        0 2022-09-07 14:16:11.000000 telegram_django_bot-1.0.1/telegram_django_bot/migrations/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)    14827 2023-04-09 07:45:25.000000 telegram_django_bot-1.0.1/telegram_django_bot/models.py
--rw-r--r--   0 alex       (501) staff       (20)      277 2023-04-09 07:32:50.000000 telegram_django_bot-1.0.1/telegram_django_bot/permissions.py
--rw-r--r--   0 alex       (501) staff       (20)     5375 2023-04-09 07:32:50.000000 telegram_django_bot-1.0.1/telegram_django_bot/routing.py
--rw-r--r--   0 alex       (501) staff       (20)     5232 2022-10-23 21:06:50.000000 telegram_django_bot-1.0.1/telegram_django_bot/tasks.py
--rw-r--r--   0 alex       (501) staff       (20)    30066 2023-04-09 07:32:50.000000 telegram_django_bot-1.0.1/telegram_django_bot/td_viewset.py
--rw-r--r--   0 alex       (501) staff       (20)     1498 2023-04-09 07:32:50.000000 telegram_django_bot-1.0.1/telegram_django_bot/telegram_lib_redefinition.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 07:46:20.765420 telegram_django_bot-1.0.1/telegram_django_bot/templates/
--rw-r--r--   0 alex       (501) staff       (20)     1598 2022-09-07 14:16:11.000000 telegram_django_bot-1.0.1/telegram_django_bot/templates/dropdown_filter1.html
--rw-r--r--   0 alex       (501) staff       (20)     3300 2023-04-09 07:32:50.000000 telegram_django_bot-1.0.1/telegram_django_bot/test.py
--rw-r--r--   0 alex       (501) staff       (20)    12071 2023-04-09 07:32:50.000000 telegram_django_bot-1.0.1/telegram_django_bot/tg_dj_bot.py
--rw-r--r--   0 alex       (501) staff       (20)     2293 2023-04-09 07:32:50.000000 telegram_django_bot-1.0.1/telegram_django_bot/user_viewset.py
--rw-r--r--   0 alex       (501) staff       (20)    12164 2023-04-09 07:32:50.000000 telegram_django_bot-1.0.1/telegram_django_bot/utils.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-09 07:46:20.756791 telegram_django_bot-1.0.1/telegram_django_bot.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)    40224 2023-04-09 07:46:20.000000 telegram_django_bot-1.0.1/telegram_django_bot.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     1403 2023-04-09 07:46:20.000000 telegram_django_bot-1.0.1/telegram_django_bot.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2023-04-09 07:46:20.000000 telegram_django_bot-1.0.1/telegram_django_bot.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)      106 2023-04-09 07:46:20.000000 telegram_django_bot-1.0.1/telegram_django_bot.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       20 2023-04-09 07:46:20.000000 telegram_django_bot-1.0.1/telegram_django_bot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:53:52.743677 telegram_django_bot-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    40864 2023-04-15 18:53:52.743677 telegram_django_bot-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39644 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-15 18:53:52.747677 telegram_django_bot-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:53:52.739677 telegram_django_bot-1.0.2/telegram_django_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/admin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:53:52.735677 telegram_django_bot-1.0.2/telegram_django_bot/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:53:52.735677 telegram_django_bot-1.0.2/telegram_django_bot/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:53:52.743677 telegram_django_bot-1.0.2/telegram_django_bot/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:53:52.743677 telegram_django_bot-1.0.2/telegram_django_bot/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/migrations/0002_delete_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/migrations/0003_botmenuelem_message_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/migrations/0004_auto_20220915_0448.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/migrations/0005_auto_20221010_1330.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/migrations/0006_auto_20221023_0157.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/migrations/0007_auto_20221202_0305.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/migrations/0008_auto_20221225_1050.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30066 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/td_viewset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/telegram_lib_redefinition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:53:52.743677 telegram_django_bot-1.0.2/telegram_django_bot/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/templates/dropdown_filter1.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12334 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/tg_dj_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/user_viewset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/telegram_django_bot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:53:52.739677 telegram_django_bot-1.0.2/telegram_django_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40864 2023-04-15 18:53:52.000000 telegram_django_bot-1.0.2/telegram_django_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-15 18:53:52.000000 telegram_django_bot-1.0.2/telegram_django_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 18:53:52.000000 telegram_django_bot-1.0.2/telegram_django_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-15 18:53:52.000000 telegram_django_bot-1.0.2/telegram_django_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-15 18:53:52.000000 telegram_django_bot-1.0.2/telegram_django_bot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:53:52.743677 telegram_django_bot-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/tests/test_bme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/tests/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/tests/test_td_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31352 2023-04-15 18:53:33.000000 telegram_django_bot-1.0.2/tests/test_viewset.py
```

### Comparing `telegram_django_bot-1.0.1/LICENSE` & `telegram_django_bot-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.1/PKG-INFO` & `telegram_django_bot-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: telegram_django_bot
-Version: 1.0.1
+Version: 1.0.2
 Summary: Telegram Django Bot Bridge
 Home-page: https://github.com/alexanderaleskin/telegram_django_bot_bridge
 Author: Alexander Aleskin
 Author-email: alexanderaleskin@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
@@ -29,72 +28,46 @@
 Classifier: Topic :: Internet
 Requires-Python: >=3.8
 License-File: LICENSE
 
 Telegram Django Bot Bridge
 ============================
 
-This library provides a Python interface for creating Telegram Bots. It standardizes coding approach in the best
-practice of the web development. The library combines `Django <https://www.djangoproject.com/>`_ and `Python-Telegram-Bot <https://python-telegram-bot.org/>`_.
-and provides extra powerful utilities based on these libraries.
-
-
-Normally, Python-Telegram-Bot gives next opportunities for bot creating:
-
-* Python Interface for communication with Telegram API;
-* Web-service to get updates from telegram;
-
-and Django:
-
-* Django ORM  (communication with Database);
-* Administration panel for management.
-
-
-Telegram Django Bot Bridge provides next special opportunities:
-
-* using Django Forms;
-* using Viewsets (typical action with model (create, update, list, delete));
-* using Django localization.
-* using function routing like urls routing in Django.
-
-And some extra useful staff:
-
-* using function routing like urls routing in Django;
-* creating tests;
-* creating general menu items with no-coding (through Django Admin Panel);
-* extra high-level Bot functions, such as wrapper for sending delayed (or scheduled) messages;
-* collecting stats from user actions in the bot;
-* creating user triggers;
-* commonly used utilities.
-
+This library provides a Python high-level interface for creating Telegram Bots. It standardizes the coding in the best
+practice of the web development. The library is based on `Django <https://www.djangoproject.com/>`_ and `Python-Telegram-Bot <https://python-telegram-bot.org/>`_.
+and provides viewset interface for managing data with.
 
+If you start a new project, you could use `Telegram django bot template <https://github.com/alexanderaleskin/telergam_django_bot_template>`_ with preconfigured settings.
 
 Install
 ------------
 
 You can install via ``pip``:
 
 .. code-block:: shell
 
     $ pip install telegram_django_bot
 
 
-Then you can configurate it in your app:
+Then you can configure it in your app:
 
 
 1. Add "telegram_django_bot" to your INSTALLED_APPS setting like this:
 
 .. code-block:: python
 
     INSTALLED_APPS = [
         ...
         'telegram_django_bot',
+        'django_json_widget', # needed for django admin site
     ]
 
 
+If you are planning to use Django in asynchronous mode, then you need to set ``DJANGO_ALLOW_ASYNC_UNSAFE = True`` (otherwise DB writings will be failed).
+
 
 2. Run ``python manage.py migrate`` to create the telegram_django_bot models (checked that the ``AUTH_USER_MODEL`` selected
 in settings).
 
 
 3. Set up constants in Django settings file:
 
@@ -110,34 +83,68 @@
 4. This step connects ``Telegram Django Bot Bridge`` with ``Python-Telegram-Bot``. Add ``RouterCallbackMessageCommandHandler`` in handlers for using TELEGRAM_ROOT_UTRLCONF :
 
 .. code-block:: python
 
     updater = Updater(bot=TG_DJ_Bot(settings.TELEGRAM_TOKEN))
     updater.dispatcher.add_handler(RouterCallbackMessageCommandHandler())
 
+or in 20.x version :
+
+.. code-block:: python
+
+    bot = TG_DJ_Bot(settings.TELEGRAM_TOKEN)
+    application = ApplicationBuilder().bot(bot).build()
+    application.add_handler(RouterCallbackMessageCommandHandler())
+
+    
 
-If you start a new project, you could use `Telegram django bot template <https://github.com/alexanderaleskin/telergam_django_bot_template>`_ with preconfigured settings.
 
 
 Quick start
 ------------
 
 
+Normally, Python-Telegram-Bot gives the next opportunities for bot creation:
+
+* Python Interface for communication with Telegram API;
+* Web service to get updates from telegram;
+
+and Django:
+
+* Django ORM  (communication with Database);
+* Administration panel for management.
 
-The key feature of the lib is ``TelegaViewSet`` - class for manage Django ORM model. It is designed in the
+
+Telegram Django Bot Bridge provides next special opportunities:
+
+* using Viewsets (typical action with model (create, update, list, delete));
+* using Django localization.
+* using function routing like urls routing in Django.
+
+And some extra useful staff:
+
+* creating general menu items with no-coding (through Django Admin Panel);
+* extra high-level Bot functions, such as a wrapper for sending delayed (or scheduled) messages;
+* creating tests;
+* collecting stats from user actions in the bot;
+* commonly used utilities.
+
+
+
+The key feature of the lib is ``TelegramViewSet`` - a class for managing Django ORM model. It is designed in a
 similar way as `Django rest framework Viewset <https://www.django-rest-framework.org/api-guide/viewsets/>`_ , but has
-a significant difference: while DRF Viewset provides response in serializable format (usually in json format) to frontend app, TelegaViewSet
-provides response to user in telegram interface in message format with buttons. So, you will manage data and receive
-response in human format by executing TelegaViewSet method. The methods use some kind of templates for generating human
-response (it is possible to overwrite these templates). By default, TelegaViewSet has 5 methods:
+a significant difference: while DRF Viewset provides a response in serializable format (usually in json format) to frontend app, TelegaViewSet
+provides a response to the user in telegram interface in message format with buttons. So, you will manage data and receive
+responses in human format by executing TelegaViewSet method. The methods use some kind of templates for generating human
+responses (it is possible to overwrite these templates). By default, TelegaViewSet has 5 methods:
 
-* ``create`` - create a new instance of specified ORM model;
+* ``create`` - create a new instance of the specified ORM model;
 * ``change`` - update instance fields of specified ORM model;
-* ``show_elem`` - show fields of the instance and buttons with actions of this instance;
-* ``show_list`` - show list of model instance (with pagination);
+* ``show_elem`` - show fields of the element and buttons with actions of this instance;
+* ``show_list`` - show list of model elements (with pagination);
 * ``delete`` - delete the instance
 
 
 So, if, for example, you have a model of some *request* in your project:
 
 .. code-block:: python
 
@@ -146,39 +153,39 @@
     class Request(models.Model):
         text = models.TextField()
         importance_level = models.PositiveSmallIntegerField()  # for example it will be integer field
         project = models.ForeignKey('Project', on_delete=models.CASCADE)
         tags = models.ManyToManyField('Tags')
 
 
-The next piece of code gives opportunity for full managing (create, update, show, delete) of this model from Telegram:
+The next piece of code gives the opportunity for full managing (create, update, show, delete) of this model from Telegram:
 
 .. code-block:: python
 
     from telegram_django_bot import forms as td_forms
-    from telegram_django_bot.td_viewset import TelegaViewSet
+    from telegram_django_bot.td_viewset import TelegramViewSet
 
 
     class RequestForm(td_forms.TelegaModelForm):
         class Meta:
             model = Request
             fields = ['text', 'importance_level', 'project', 'tags']
 
 
-    class RequestViewSet(TelegaViewSet):
+    class RequestViewSet(TelegramViewSet):
         telega_form = RequestForm
         queryset = Request.objects.all()
         viewset_name = 'Request'
 
 
-If you need, you can add extra actions to RequestViewSet for managing (see details information below) or change existed functions.
+If you need, you can add extra actions to RequestViewSet for managing (see details information below) or change existing functions.
 There are several parameters and secondary functions in TelegaViewSet for customizing logic if it is necessary.
 
 In this example, ``TelegaModelForm`` was used. TelegaModelForm is a descendant of Django ModelForm. So, you could use
-labels, clean and other parameters and functions for managing logic and displaying.
+labels, clean functions and other parameters and functions for managing logic and displaying.
 
 
 TelegaViewSet is designed to answer next user actions: clicking buttons and sometimes sending messages. The library imposes
 `Django URL notation <https://docs.djangoproject.com/en/4.1/topics/http/urls/>`_ for mapping user actions to TelegaViewSet methods (or usual handlers).
 Usually, for correct mapping you just need to set ``TELEGRAM_ROOT_UTRLCONF`` and use ``RouterCallbackMessageCommandHandler`` in
 dispatcher as it is mentioned above in the *Install paragraph*.
 
@@ -207,28 +214,30 @@
 
 
 Deep in details
 ------------------
 
 In this chapter, we will analyze how everything works. The main task of the library is to unify the code and
 provide frequently used functions for developing a bot, that is why a lot of logic is based on resources and paradigms
-Django <https://www.djangoproject.com/>`_ and `Python-Telegram-Bot <https://python-telegram-bot.org/>`_ . Let's analyze
+of Django <https://www.djangoproject.com/>`_ and `Python-Telegram-Bot <https://python-telegram-bot.org/>`_ . Let's analyze
 key features of the library on the example of `Telegram django bot template <https://github.com/alexanderaleskin/telergam_django_bot_template>`_ .
 
+.. important::
+
+    The template is based on 13.x Python-Telegram-Bot version (synchronous version). So, the next examples is suitable for that version. For use with 20.x versions you need to do some modification.
+
 
 Since Telegram bots are designed as a tool for responding to user requests, writing a bot begins
 from the user request handler. For this, the standard tools of the Python-Telegram-Bot library are used ﹣
 ``telegram.ext.Update``:
 
 .. code-block:: python
 
      from telegram.ext import Updater
 
-     ...
-
      def main():
          ...
 
          updater = Updater(bot=TG_DJ_Bot(TELEGRAM_TOKEN))
          add_handlers(updater)
          updater.start_polling()
          updater.idle()
@@ -239,15 +248,14 @@
 
 As indicated in the example, to run the bot (Update) you need to specify a few things (the ``Python-Telegram-Bot`` library standard):
 
 1. an instance of the ``telegram.Bot`` model with the specified API token. In this case, a descendant ``telegram_django_bot.tg_dj_bot.TG_DJ_Bot``
 of the ``telegram.Bot`` class is used. It has additional functionality for convenience (we will return to it later);
 2. Handlers that will be called in response to user requests.
 
-
 In the example, the list of handlers is specified in the ``add_handlers`` function:
 
 
 
 .. code-block:: python
 
      from telegram_django_bot.routing import RouterCallbackMessageCommandHandler
@@ -296,16 +304,16 @@
 There is following code in the specified included file ``base.utrls.py`` :
 
 
 .. code-block:: python
 
     from django.urls import re_path
     from django.conf import settings
-
-    from .views import start, BotMenuElemViewSet, UserViewSet, some_debug_func
+    from telegram_django_bot.user_viewset import UserViewSet
+    from .views import start, BotMenuElemViewSet, some_debug_func
 
 
     urlpatterns = [
         re_path('start', start, name='start'),
         re_path('main_menu', start, name='start'),
 
         re_path('sb/', BotMenuElemViewSet, name='BotMenuElemViewSet'),
@@ -342,43 +350,43 @@
 change     up       Change model attributes
 delete     de       Deleting a model
 show_elem  se       Display a model
 show_list  sl       Display a list of models
 ========= ======== ===========================
 
 Thus, if we want to call the ``BotMenuElemViewSet.create`` method to create an element, we need to use
-path 'sb/cr', where by the first part of path 'sb/'  the router ``RouterCallbackMessageCommandHandler`` will execute
+path 'sb/cr', whereby the first part of the path 'sb/'  the router ``RouterCallbackMessageCommandHandler`` will execute
 the ``BotMenuElemViewSet`` class, namely the ``TelegaViewSet.dispatch`` method, which in turn will call  the ``create`` method by analyzing the second part of the path
 ``cr``.
 
 To sum up the scheme of handlers routing, there are following key points:
 
 1. ``telegram.ext.Update`` is used as a receiver of messages from Telegram;
 2. Standard handlers of the ``Python-Telegram-Bot`` library can be used as handlers. For convenient use Django's path scheme and ``TelegaViewSet`` you need to use ``RouterCallbackMessageCommandHandler``.
 3. ``TelegaViewSet`` aggregates a set of standard functions for managing data, what is made possible to group code associated with one type of data type in one class (place).
 
 
 
-TelegaViewSet features
+TelegramViewSet features
 ~~~~~~~~~~~~~~~~~~~~~~~~
 
 As described above, TelegaViewSet contains standard functions for data manipulation.
 Due to such standard data processing methods, it turns out in the example to describe the logic of ``BotMenuElemViewSet`` in 40
-lines of code, also using some customization for a beautiful data displaying.
+lines of code, also using some customization for beautiful data displaying.
 
 
 To use all the features of the TelegaViewSet in your class, it should be inherited from it, as, for example, this is done
 in the ``BotMenuElemViewSet``:
 
 
 .. code-block:: python
 
-    from telegram_django_bot.td_viewset import TelegaViewSet
+    from telegram_django_bot.td_viewset import TelegramViewSet
 
-    class BotMenuElemViewSet(TelegaViewSet):
+    class BotMenuElemViewSet(TelegramViewSet):
 
 
 In order to customize the ViewSet, you must specify 3 required attributes:
 
 1. ``viewset_name`` - class name, used to display to telegram users
 2. ``telega_form`` - data form, used to specify which fields of the ORM database model to use in the viewset;
 3. ``queryset`` - basic query for getting model elements.
@@ -433,24 +441,24 @@
 1. The clean function and other `form validation process functions <https://docs.djangoproject.com/en/4.1/ref/forms/validation/>`_ ;
 2. ``labels`` - field names;
 3. ``forms.HiddenInput`` - designation of hidden fields (hiding fields allows them not to be shown to the user, while using and configuring in forms or in ``TelegaViewSet``).
 
 
 
 ``TelegaViewSet`` is designed to interact with descendants of the ``TelegaModelForm`` class and allows you to use
-generate forms with different fields, such as ``CharField, IntegerField`` or ``ForeignKey, ManyToManyField``. Also, it is good idea
+generate forms with different fields, such as ``CharField, IntegerField`` or ``ForeignKey, ManyToManyField``. Also, it is a good idea
 to use the ``prechoice_fields_values`` dictionary in ``TelegaViewSet`` descendants for improving the convenience of filling out forms for users.
 It is possible to store a list of frequently used values of form fields in the ``prechoice_fields_values``.
 This allows users to select the desired values by clicking buttons rather than
 writing text manually. The template has an example of using this field:
 
 
 .. code-block:: python
 
-    class BotMenuElemViewSet(TelegaViewSet):
+    class BotMenuElemViewSet(TelegramViewSet):
         ...
 
         prechoice_fields_values = {
             'is_visable': (
                 (True, '👁 Visable'),
                 (False, '🚫 Disabled'),
             )
@@ -458,18 +466,18 @@
 
 In this case, 2 values are specified for choosing true or false for the boolean field ``is_visable``. You can also use
 ``prechoice_fields_values`` for ``CharField, IntegerField`` or any other fields.
 Sometimes the list of values needs to be generated dynamically, in which case you can override
 ``prechoice_fields_values`` as a ``@property`` function.
 
 
-Key logic of TelegaViewSet
+Key logic of TelegramViewSet
 ************************************************
 
-The main function of the class, which is selected the function for managing data by the request of the user,  is ``TelegaViewSet.dispatch``.
+The main function of the class, which is selected the function for managing data by the request of the user,  is ``TelegramViewSet.dispatch``.
 Let's analyze its logic in more detail:
 
 .. code-block:: python
 
     def dispatch(self, bot, update, user):
 
         self.bot = bot
@@ -503,40 +511,40 @@
 
 
 Like a regular handler, the function takes 3 arguments as input: bot, update, user. After saving these arguments in class,
 the determination of the current routing path is occurred. It is determined either by pressing a button in the bot (the ``callback_data`` value of the button), or
 can be stored in the user attribute ``user.current_utrl``. The second option is possible if the user manually enters
 some information (for example, filled in a text field of form). After that, the arguments are extracted from the path
 to call a specific function. Storing and interacting with arguments in a path is similar to how ``sys.argv`` works. So,
-for example, the string ``"sl&1&20"`` will be converted to the list ``['sl', '1', '20']``. Separator character between attributes
+for example, the string ``"sl&1&20"`` will be converted to the list ``['sl', '1', '20']``. The separator character between attributes
 is ``&`` by default and can be changed via the ``TelegaViewSet.ARGS_SEPARATOR_SYMBOL`` variable.
 
 When using ``TelegaViewSet`` you most likely won't have to interact with the argument string directly, since
-how ``dispatch`` converts a string into arguments, and to create a string for a ``callback_data`` button for calling another method by user, you should use
+``dispatch`` converts a string into arguments. And for creating a ``callback_data`` button string, that the user can call another method from Telegram interface, you should use
 ``TelegaViewSet.gm_callback_data`` function. In case you need more low-level interaction with function arguments, then
 you can use the ``construct_utrl`` and ``get_utrl_params`` functions.
 
 After receiving the utrl_args arguments and checking access rights, the managing method (action) is directly selected and called.
 The first argument, which is the short name for the function, is popped from the utrl_args. All other arguments are passed as parameters
-into a function. Inside the function, the necessary business logic and the data formating for displaying to the user as a response take place.
+into a function. Inside the function, the necessary business logic and the data formatting for displaying to the user as a response take place.
 Any such managing function in the ``TelegaViewSet`` class must return the action type ``chat_action`` and the parameters to that action ``chat_action_args``.
-By default, the  class has only 1 action ﹣ ``CHAT_ACTION_MESSAGE``, which means that the user will receive
-a text message (possibly with buttons) as an answer for his/her action. The arguments to this action are the text of the message and a list of buttons (can be None).
+By default, the class has only 1 action ﹣ ``CHAT_ACTION_MESSAGE``, which means that the user will receive
+a text message (possibly with buttons) as an answer for his/her action. The arguments for this action are the text of the message and a list of buttons (can be None).
 
 
-After the function is processed, a response is sent to the user  by ``send_answer`` function and the user's action is logged.
+After the function is processed, a response is sent to the user by ``send_answer`` function and the user's action is logged.
 
 
 The methods to call in ``viewset_routing`` are the ``create, update, delete, show_elem, show_list`` methods.
 You can also add your own methods. Suppose we want to add a ``def super_method(self, *args)`` method, then
 you need to add the following lines in the class:
 
 .. code-block:: python
 
-    class SomeViewSetClass(TelegaViewSet):
+    class SomeViewSetClass(TelegramViewSet):
         ...
 
         actions = ['create', 'change', 'delete', 'show_elem', 'show_list', 'super_method']
 
         command_routing_super_method = 'sm'
 
 
@@ -547,45 +555,45 @@
 Where ``actions`` defines the list of available methods and ``command_routing_<method>`` defines the path (url; short name) of the method.
 
 As noted above, the ``dispatch`` method performs a permissions check by calling the ``has_permissions`` method.
 The check is performed by the classes specified in ``permission_classes`` and the default class is ``AllowAny``:
 
 .. code-block:: python
 
-    class TelegaViewSet:
+    class TelegramViewSet:
         permission_classes = [AllowAny]
 
 
 
-Additional TelegaViewSet Tools
+Additional TelegramViewSet Tools
 ************************************************
 
 This section describes the following class functionality that makes it easier to write code:
 
 1. External filters;
 2. Data display setting options;
 3. Helper functions for displaying data;
 4. Helper functions of business logic;
 
 
 External filters
 +++++++++++++++++++++
 
-Quite often, there is situation when you need to work not with all the elements of a database table, but with some
+Quite often, there is a situation when you need to work not with all the elements of a database table, but with some
 group (for example, a group of elements with a specific foreign key). For such purposes, you should use the ``foreign_filters`` list,
 which stores the values for filtering when the method is called. How exactly to use these filters is up to you, but
-usually it is good idea to use it in the ``get_queryset`` function. Thus, it is possible to pass to functions
+usually it is a good idea to use it in the ``get_queryset`` function. Thus, it is possible to pass to functions
 additional arguments that do not break the key logic of standard functions. Using the template example, you can modify
 ``BotMenuElemViewSet`` so that if an additional parameter is specified, then the BotMenuElem list displays
 only those elements that contain the specified parameter in their ``command`` attribute. To do this, you need to make the following changes to the code:
 
 
 .. code-block:: python
 
-    class BotMenuElemViewSet(TelegaViewSet):
+    class BotMenuElemViewSet(TelegramViewSet):
         ...
 
         foreign_filter_amount = 1
 
         def get_queryset(self):
             queryset = super().get_queryset()
             if self.foreign_filters[0]:
@@ -604,15 +612,15 @@
 This allows you to change the value of filters when generating paths.
 
 A more detailed use of external filters can be seen in the example of `Drive Bot <https://github.com/alexanderaleskin/drive_bot>`_ .
 
 Data display options
 ++++++++++++++++++++++++++++++++++++++++++
 
-The ``TelegaViewSet`` has the following options for displaying model elements:
+The ``TelegramViewSet`` has the following options for displaying model elements:
 
 * ``updating_fields: list`` - list of fields that can be changed (displayed when showing the element (``show_elem``);
 * ``show_cancel_updating_button: bool = True`` - shows a cancel button when changing fields, which leads back to the displaying element (``show_elem``);
 * ``deleting_with_confirm: bool = True`` - ask the user for confirmation when deleting an element;
 * ``cancel_adding_button: InlineKeyboardButtonDJ = None`` - cancel button when creating an element (``create`` method);
 * ``use_name_and_id_in_elem_showing: bool = True`` - enables the use of the name and ID of the element when displaying this element (methods ``show_list`` and ``show_elem``);
 * ``meta_texts_dict: dict`` - a dictionary that stores standard texts for display (texts are used in all methods).
@@ -642,17 +650,17 @@
 
 Depending on the need for customization, it is necessary to redefine these functions.
 
 
 Helper functions of business logic
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
-The ``TelegaViewSet`` class uses the following helper functions:
+The ``TelegramViewSet`` class uses the following helper functions:
 
-* ``def get_queryset`` - allows you to modify Model queries to database (most often used to filter elements, as in the example above);
+* ``def get_queryset`` - allows you to modify Model queries to the database (most often used to filter elements, as in the example above);
 * ``def create_or_update_helper`` - main logic for ``create`` and ``update`` methods;
 * ``def show_list_get_queryset`` - allows you to customize the selection of items to display in show_list;
 
 
 handler_decor
 ~~~~~~~~~~~~~~~~
 
@@ -674,46 +682,45 @@
 To support the use of different languages, the main elements of the Python-Telegram-Bot library are redefined in ``telegram_django_bot.telegram_lib_redefinition``:
 
 
 1. ``telegram.Bot`` -> ``telegram_django_bot.BotDJ`` ;
 2. ``telegram.ReplyMarkup`` -> ``telegram_django_bot.ReplyMarkupDJ`` ;
 3. ``telegram.KeyboardButton`` -> ``telegram_django_bot.KeyboardButtonDJ`` ;
 4. ``telegram.InlineKeyboardButton`` -> ``telegram_django_bot.InlineKeyboardButtonDJ`` ;
-5. ``telegram.InlineKeyboardMarkup`` -> ``telegram_django_bot.InlineKeyboardMarkupDJ``;
-
+5. ``telegram.InlineKeyboardMarkup`` -> ``telegram_django_bot.InlineKeyboardMarkupDJ``.
 
 
 When using these classes in code, multilingual support comes down to the following steps:
 
 1. Specifying the necessary settings in the settings.py file: ``LANGUAGES`` - list of languages, ``LANGUAGE_CODE`` - default language;
 1. Necessary texts for translation are wrapped in ``gettext`` and ``gettext_lazy`` from ``django.utils.translation`` (how it works in Django `read here <https://docs.djangoproject.com/en /4.1/topics/i18n/translation/#standard-translation>`_ )
 2. Run command ``$ django-admin makemessages -a`` to generate texts for translation (created in locale folder)
 3. Generation of translation files ``$ django-admin compilemessages``.
 
-Only a part of the functions uses localization in the template. It is made for easy understanding. Usage of localization can be seen in the example
+Only a part of the functions uses localization in the template. It is made for easy understanding. The usage of localization can be seen in the example
 functions ``some_debug_func``.
 
 
 Extra lib features
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 The library provides some additional tools for the convenience of developing and managing the bot.
 
 Модели библиотеки
 ************************************
 
 
-For the correct work of ``TelegaViewSet`` and other components the Django ORM model representing the user in the Telegram must be inherited
+For the correct work of ``TelegaViewSet`` and other components the Django ORM model representing the user in Telegram must be inherited
 from ``telegram_django_bot.models.TelegramUser``, as these components use its fields. ``TelegramUser`` inherited from
 ``django.contrib.auth.models.AbstractUser`` (which allows you to authorize users on the site if necessary) and has
 the following additional fields:
 
 * ``id`` - redefined to use user ID from telegrams;
 * ``seed_code`` - arbitrary value from 1 to 100 to randomly group users for tests and analysis;
-* ``telegram_username`` - username of the user in the telegram;
+* ``telegram_username`` - username of the user in telegram;
 * ``telegram_language_code`` - telegram language code (some languages have dialects and as a result the code designation is more than 2 symbols);
 * ``timezone`` - the user's time zone (for determining the time);
 * ``current_utrl`` - path (utrl) of the last user action (used in ``TelegaViewSet``);
 * ``current_utrl_code_dttm`` - time of the last action, when saving the path;
 * ``current_utrl_context_db`` - path context (utrl);
 * ``current_utrl_form_db`` - intermediate data for the form. Acts as a temporary data store when filling out a form;
 
@@ -724,15 +731,15 @@
 * ``current_utrl_context`` (property) - returns the current path context (utrl);
 * ``save_form_in_db`` - saves the form in the ``current_utrl_form_db`` field;
 * ``save_context_in_db`` - saves the context in the field ``current_utrl_context_db``;
 * ``clear_status`` - clears the data associated with the used path (fields ``current_utrl_<suffix>``) ;
 * ``language_code`` (property) - returns the language code in which messages should be generated for the user;
 
 
-Actually, if you want, you can create your self Django ORM model representing the user, you just need to copy
+If you want, you can create your self Django ORM model representing the user, you just need to copy
 ``id, telegram_username, telegram_language_code, current_utrl, current_utrl_code_dttm, current_utrl_context_db, current_utrl_form_db``
 and corresponding functions.
 
 
 The library also describes additional models to improve the usability of the bot:
 
 * ``ActionLog`` - stores user actions. Records help to collect analytics and make triggers that work on certain actions;
@@ -744,15 +751,15 @@
 
 
 Additional functions of TG_DJ_Bot
 *********************************************
 
 To improve convenience, ``TG_DJ_Bot`` has several high-level functions:
 
-* ``send_format_message`` - Allows you to send a message of an arbitrary type (internally, depending on the ``message_format`` selects the appropriate method of the ``Python-Telegram-Bot`` library). An important feature of this function is that if the user clicks on the button, then the previous message of the bot is changed, rather than a new one is sent. If, nevertheless, in this case you need to send a new message to the user, then you need to set the parameter ``only_send=True`` ;
+* ``send_format_message`` - Allows you to send a message of an arbitrary type (internally, depending on the ``message_format`` selects the appropriate method of the ``Python-Telegram-Bot`` library). An important feature of this function is that if the user clicks on the button, then the previous message of the bot is changed, rather than a new one being sent. If, nevertheless you need to send a new message to the user, then you need to set the parameter ``only_send=True`` ;
 * ``edit_or_send`` - wrapper of the ``send_format_message`` method for sending text messages with buttons;
 * ``send_botmenuelem`` - Sends a ``BotMenuElem`` to the user. The ``update`` argument can be empty;
 * ``task_send_message_handler`` - created for sending messages to many users. Handles situations where the user blocked the bot, deleted or when the limit for sending messages to users is reached;
 
 
 Utils
 **********
@@ -774,33 +781,31 @@
 Django. Also ``RouterCallbackMessageCommandHandler`` provides the ability to handle calls to ``BotMenuElem`` as
 through commands, and through callback. This is achieved by using the functions ``all_command_bme_handler`` and
 ``all_callback_bme_handler``. By default, ``BotMenuElem`` call handling is enabled and handled after
 no suitable path was found in the description of utrls (paths in Django notation). If there is no ``BotMenuElem`` element
 match is found, the ``BotMenuElem`` is considered to be configured incorrectly and an error message is returned to the user.
 You can create a class with the ``only_utrl=True`` attribute, what is disable calls to ``BotMenuElem``.
 
-The example template contains the use of the ``telega_reverse`` function, the essence of which is to generate a path (string) to
+The example template contains the use of the ``telega_reverse`` function, the essence of which is to generate a path (string) to the
 handler specified in the function argument. The function is analogous to the `reverse <https://docs.djangoproject.com/en/4.1/ref/urlresolvers/#reverse>`_ Django function
 and avoids errors when changing paths.
 
 
 
 Tests
 **********************
 
 The library also extends the ``django.test.TestCase`` capabilities for use with Telegram through the ``TD_TestCase`` class.
 
 The simplest approach for testing the bot is to generate messages that the bot expects from Telegram and
-sending a response to Telegram (to check that the bot's response messages are in the correct format). Class ``TD_TestCase``
+send a response to Telegram (to check that the bot's response messages are in the correct format). Class ``TD_TestCase``
 has a function ``create_update`` for easy and fast creation of ``Telegram.Update`` which generates the request
 telegram user. So the overall design looks like this:
 
 1. A ``Telegram.Update`` is created for emitting a user request;
-2. The ``handle_update`` lambda function, which uses ``RouterCallbackMessageCommandHandler``,  is called with created update. It does its staff and as a result sends a real message to the test user. Due to this, the correctness of the responsing data format  is checked by Telegram;
+2. The ``handle_update`` lambda function, which uses ``RouterCallbackMessageCommandHandler``,  is called with created update. It does its staff and as a result sends a real message to the test user. Due to this, the correctness of the response data format  is checked by Telegram;
 3. The correctness of the sent data and changes in the database is checked using the standard tools ``django.test.TestCase``.
 
 You need to specify at least one test user ID in the ``TELEGRAM_TEST_USER_IDS`` settings section for correct tests work.
 Messages will be sent to that user, so the bot needs to have permission to write to that user.
 
 In the ``tests`` folder you could find test examples.
-
-
```

### Comparing `telegram_django_bot-1.0.1/README.rst` & `telegram_django_bot-1.0.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,68 +1,42 @@
 Telegram Django Bot Bridge
 ============================
 
-This library provides a Python interface for creating Telegram Bots. It standardizes coding approach in the best
-practice of the web development. The library combines `Django <https://www.djangoproject.com/>`_ and `Python-Telegram-Bot <https://python-telegram-bot.org/>`_.
-and provides extra powerful utilities based on these libraries.
-
-
-Normally, Python-Telegram-Bot gives next opportunities for bot creating:
-
-* Python Interface for communication with Telegram API;
-* Web-service to get updates from telegram;
-
-and Django:
-
-* Django ORM  (communication with Database);
-* Administration panel for management.
-
-
-Telegram Django Bot Bridge provides next special opportunities:
-
-* using Django Forms;
-* using Viewsets (typical action with model (create, update, list, delete));
-* using Django localization.
-* using function routing like urls routing in Django.
-
-And some extra useful staff:
-
-* using function routing like urls routing in Django;
-* creating tests;
-* creating general menu items with no-coding (through Django Admin Panel);
-* extra high-level Bot functions, such as wrapper for sending delayed (or scheduled) messages;
-* collecting stats from user actions in the bot;
-* creating user triggers;
-* commonly used utilities.
-
+This library provides a Python high-level interface for creating Telegram Bots. It standardizes the coding in the best
+practice of the web development. The library is based on `Django <https://www.djangoproject.com/>`_ and `Python-Telegram-Bot <https://python-telegram-bot.org/>`_.
+and provides viewset interface for managing data with.
 
+If you start a new project, you could use `Telegram django bot template <https://github.com/alexanderaleskin/telergam_django_bot_template>`_ with preconfigured settings.
 
 Install
 ------------
 
 You can install via ``pip``:
 
 .. code-block:: shell
 
     $ pip install telegram_django_bot
 
 
-Then you can configurate it in your app:
+Then you can configure it in your app:
 
 
 1. Add "telegram_django_bot" to your INSTALLED_APPS setting like this:
 
 .. code-block:: python
 
     INSTALLED_APPS = [
         ...
         'telegram_django_bot',
+        'django_json_widget', # needed for django admin site
     ]
 
 
+If you are planning to use Django in asynchronous mode, then you need to set ``DJANGO_ALLOW_ASYNC_UNSAFE = True`` (otherwise DB writings will be failed).
+
 
 2. Run ``python manage.py migrate`` to create the telegram_django_bot models (checked that the ``AUTH_USER_MODEL`` selected
 in settings).
 
 
 3. Set up constants in Django settings file:
 
@@ -78,34 +52,68 @@
 4. This step connects ``Telegram Django Bot Bridge`` with ``Python-Telegram-Bot``. Add ``RouterCallbackMessageCommandHandler`` in handlers for using TELEGRAM_ROOT_UTRLCONF :
 
 .. code-block:: python
 
     updater = Updater(bot=TG_DJ_Bot(settings.TELEGRAM_TOKEN))
     updater.dispatcher.add_handler(RouterCallbackMessageCommandHandler())
 
+or in 20.x version :
+
+.. code-block:: python
+
+    bot = TG_DJ_Bot(settings.TELEGRAM_TOKEN)
+    application = ApplicationBuilder().bot(bot).build()
+    application.add_handler(RouterCallbackMessageCommandHandler())
+
+    
 
-If you start a new project, you could use `Telegram django bot template <https://github.com/alexanderaleskin/telergam_django_bot_template>`_ with preconfigured settings.
 
 
 Quick start
 ------------
 
 
+Normally, Python-Telegram-Bot gives the next opportunities for bot creation:
+
+* Python Interface for communication with Telegram API;
+* Web service to get updates from telegram;
+
+and Django:
+
+* Django ORM  (communication with Database);
+* Administration panel for management.
+
+
+Telegram Django Bot Bridge provides next special opportunities:
+
+* using Viewsets (typical action with model (create, update, list, delete));
+* using Django localization.
+* using function routing like urls routing in Django.
+
+And some extra useful staff:
+
+* creating general menu items with no-coding (through Django Admin Panel);
+* extra high-level Bot functions, such as a wrapper for sending delayed (or scheduled) messages;
+* creating tests;
+* collecting stats from user actions in the bot;
+* commonly used utilities.
 
-The key feature of the lib is ``TelegaViewSet`` - class for manage Django ORM model. It is designed in the
+
+
+The key feature of the lib is ``TelegramViewSet`` - a class for managing Django ORM model. It is designed in a
 similar way as `Django rest framework Viewset <https://www.django-rest-framework.org/api-guide/viewsets/>`_ , but has
-a significant difference: while DRF Viewset provides response in serializable format (usually in json format) to frontend app, TelegaViewSet
-provides response to user in telegram interface in message format with buttons. So, you will manage data and receive
-response in human format by executing TelegaViewSet method. The methods use some kind of templates for generating human
-response (it is possible to overwrite these templates). By default, TelegaViewSet has 5 methods:
+a significant difference: while DRF Viewset provides a response in serializable format (usually in json format) to frontend app, TelegaViewSet
+provides a response to the user in telegram interface in message format with buttons. So, you will manage data and receive
+responses in human format by executing TelegaViewSet method. The methods use some kind of templates for generating human
+responses (it is possible to overwrite these templates). By default, TelegaViewSet has 5 methods:
 
-* ``create`` - create a new instance of specified ORM model;
+* ``create`` - create a new instance of the specified ORM model;
 * ``change`` - update instance fields of specified ORM model;
-* ``show_elem`` - show fields of the instance and buttons with actions of this instance;
-* ``show_list`` - show list of model instance (with pagination);
+* ``show_elem`` - show fields of the element and buttons with actions of this instance;
+* ``show_list`` - show list of model elements (with pagination);
 * ``delete`` - delete the instance
 
 
 So, if, for example, you have a model of some *request* in your project:
 
 .. code-block:: python
 
@@ -114,39 +122,39 @@
     class Request(models.Model):
         text = models.TextField()
         importance_level = models.PositiveSmallIntegerField()  # for example it will be integer field
         project = models.ForeignKey('Project', on_delete=models.CASCADE)
         tags = models.ManyToManyField('Tags')
 
 
-The next piece of code gives opportunity for full managing (create, update, show, delete) of this model from Telegram:
+The next piece of code gives the opportunity for full managing (create, update, show, delete) of this model from Telegram:
 
 .. code-block:: python
 
     from telegram_django_bot import forms as td_forms
-    from telegram_django_bot.td_viewset import TelegaViewSet
+    from telegram_django_bot.td_viewset import TelegramViewSet
 
 
     class RequestForm(td_forms.TelegaModelForm):
         class Meta:
             model = Request
             fields = ['text', 'importance_level', 'project', 'tags']
 
 
-    class RequestViewSet(TelegaViewSet):
+    class RequestViewSet(TelegramViewSet):
         telega_form = RequestForm
         queryset = Request.objects.all()
         viewset_name = 'Request'
 
 
-If you need, you can add extra actions to RequestViewSet for managing (see details information below) or change existed functions.
+If you need, you can add extra actions to RequestViewSet for managing (see details information below) or change existing functions.
 There are several parameters and secondary functions in TelegaViewSet for customizing logic if it is necessary.
 
 In this example, ``TelegaModelForm`` was used. TelegaModelForm is a descendant of Django ModelForm. So, you could use
-labels, clean and other parameters and functions for managing logic and displaying.
+labels, clean functions and other parameters and functions for managing logic and displaying.
 
 
 TelegaViewSet is designed to answer next user actions: clicking buttons and sometimes sending messages. The library imposes
 `Django URL notation <https://docs.djangoproject.com/en/4.1/topics/http/urls/>`_ for mapping user actions to TelegaViewSet methods (or usual handlers).
 Usually, for correct mapping you just need to set ``TELEGRAM_ROOT_UTRLCONF`` and use ``RouterCallbackMessageCommandHandler`` in
 dispatcher as it is mentioned above in the *Install paragraph*.
 
@@ -175,28 +183,30 @@
 
 
 Deep in details
 ------------------
 
 In this chapter, we will analyze how everything works. The main task of the library is to unify the code and
 provide frequently used functions for developing a bot, that is why a lot of logic is based on resources and paradigms
-Django <https://www.djangoproject.com/>`_ and `Python-Telegram-Bot <https://python-telegram-bot.org/>`_ . Let's analyze
+of Django <https://www.djangoproject.com/>`_ and `Python-Telegram-Bot <https://python-telegram-bot.org/>`_ . Let's analyze
 key features of the library on the example of `Telegram django bot template <https://github.com/alexanderaleskin/telergam_django_bot_template>`_ .
 
+.. important::
+
+    The template is based on 13.x Python-Telegram-Bot version (synchronous version). So, the next examples is suitable for that version. For use with 20.x versions you need to do some modification.
+
 
 Since Telegram bots are designed as a tool for responding to user requests, writing a bot begins
 from the user request handler. For this, the standard tools of the Python-Telegram-Bot library are used ﹣
 ``telegram.ext.Update``:
 
 .. code-block:: python
 
      from telegram.ext import Updater
 
-     ...
-
      def main():
          ...
 
          updater = Updater(bot=TG_DJ_Bot(TELEGRAM_TOKEN))
          add_handlers(updater)
          updater.start_polling()
          updater.idle()
@@ -207,15 +217,14 @@
 
 As indicated in the example, to run the bot (Update) you need to specify a few things (the ``Python-Telegram-Bot`` library standard):
 
 1. an instance of the ``telegram.Bot`` model with the specified API token. In this case, a descendant ``telegram_django_bot.tg_dj_bot.TG_DJ_Bot``
 of the ``telegram.Bot`` class is used. It has additional functionality for convenience (we will return to it later);
 2. Handlers that will be called in response to user requests.
 
-
 In the example, the list of handlers is specified in the ``add_handlers`` function:
 
 
 
 .. code-block:: python
 
      from telegram_django_bot.routing import RouterCallbackMessageCommandHandler
@@ -264,16 +273,16 @@
 There is following code in the specified included file ``base.utrls.py`` :
 
 
 .. code-block:: python
 
     from django.urls import re_path
     from django.conf import settings
-
-    from .views import start, BotMenuElemViewSet, UserViewSet, some_debug_func
+    from telegram_django_bot.user_viewset import UserViewSet
+    from .views import start, BotMenuElemViewSet, some_debug_func
 
 
     urlpatterns = [
         re_path('start', start, name='start'),
         re_path('main_menu', start, name='start'),
 
         re_path('sb/', BotMenuElemViewSet, name='BotMenuElemViewSet'),
@@ -310,43 +319,43 @@
 change     up       Change model attributes
 delete     de       Deleting a model
 show_elem  se       Display a model
 show_list  sl       Display a list of models
 ========= ======== ===========================
 
 Thus, if we want to call the ``BotMenuElemViewSet.create`` method to create an element, we need to use
-path 'sb/cr', where by the first part of path 'sb/'  the router ``RouterCallbackMessageCommandHandler`` will execute
+path 'sb/cr', whereby the first part of the path 'sb/'  the router ``RouterCallbackMessageCommandHandler`` will execute
 the ``BotMenuElemViewSet`` class, namely the ``TelegaViewSet.dispatch`` method, which in turn will call  the ``create`` method by analyzing the second part of the path
 ``cr``.
 
 To sum up the scheme of handlers routing, there are following key points:
 
 1. ``telegram.ext.Update`` is used as a receiver of messages from Telegram;
 2. Standard handlers of the ``Python-Telegram-Bot`` library can be used as handlers. For convenient use Django's path scheme and ``TelegaViewSet`` you need to use ``RouterCallbackMessageCommandHandler``.
 3. ``TelegaViewSet`` aggregates a set of standard functions for managing data, what is made possible to group code associated with one type of data type in one class (place).
 
 
 
-TelegaViewSet features
+TelegramViewSet features
 ~~~~~~~~~~~~~~~~~~~~~~~~
 
 As described above, TelegaViewSet contains standard functions for data manipulation.
 Due to such standard data processing methods, it turns out in the example to describe the logic of ``BotMenuElemViewSet`` in 40
-lines of code, also using some customization for a beautiful data displaying.
+lines of code, also using some customization for beautiful data displaying.
 
 
 To use all the features of the TelegaViewSet in your class, it should be inherited from it, as, for example, this is done
 in the ``BotMenuElemViewSet``:
 
 
 .. code-block:: python
 
-    from telegram_django_bot.td_viewset import TelegaViewSet
+    from telegram_django_bot.td_viewset import TelegramViewSet
 
-    class BotMenuElemViewSet(TelegaViewSet):
+    class BotMenuElemViewSet(TelegramViewSet):
 
 
 In order to customize the ViewSet, you must specify 3 required attributes:
 
 1. ``viewset_name`` - class name, used to display to telegram users
 2. ``telega_form`` - data form, used to specify which fields of the ORM database model to use in the viewset;
 3. ``queryset`` - basic query for getting model elements.
@@ -401,24 +410,24 @@
 1. The clean function and other `form validation process functions <https://docs.djangoproject.com/en/4.1/ref/forms/validation/>`_ ;
 2. ``labels`` - field names;
 3. ``forms.HiddenInput`` - designation of hidden fields (hiding fields allows them not to be shown to the user, while using and configuring in forms or in ``TelegaViewSet``).
 
 
 
 ``TelegaViewSet`` is designed to interact with descendants of the ``TelegaModelForm`` class and allows you to use
-generate forms with different fields, such as ``CharField, IntegerField`` or ``ForeignKey, ManyToManyField``. Also, it is good idea
+generate forms with different fields, such as ``CharField, IntegerField`` or ``ForeignKey, ManyToManyField``. Also, it is a good idea
 to use the ``prechoice_fields_values`` dictionary in ``TelegaViewSet`` descendants for improving the convenience of filling out forms for users.
 It is possible to store a list of frequently used values of form fields in the ``prechoice_fields_values``.
 This allows users to select the desired values by clicking buttons rather than
 writing text manually. The template has an example of using this field:
 
 
 .. code-block:: python
 
-    class BotMenuElemViewSet(TelegaViewSet):
+    class BotMenuElemViewSet(TelegramViewSet):
         ...
 
         prechoice_fields_values = {
             'is_visable': (
                 (True, '👁 Visable'),
                 (False, '🚫 Disabled'),
             )
@@ -426,18 +435,18 @@
 
 In this case, 2 values are specified for choosing true or false for the boolean field ``is_visable``. You can also use
 ``prechoice_fields_values`` for ``CharField, IntegerField`` or any other fields.
 Sometimes the list of values needs to be generated dynamically, in which case you can override
 ``prechoice_fields_values`` as a ``@property`` function.
 
 
-Key logic of TelegaViewSet
+Key logic of TelegramViewSet
 ************************************************
 
-The main function of the class, which is selected the function for managing data by the request of the user,  is ``TelegaViewSet.dispatch``.
+The main function of the class, which is selected the function for managing data by the request of the user,  is ``TelegramViewSet.dispatch``.
 Let's analyze its logic in more detail:
 
 .. code-block:: python
 
     def dispatch(self, bot, update, user):
 
         self.bot = bot
@@ -471,40 +480,40 @@
 
 
 Like a regular handler, the function takes 3 arguments as input: bot, update, user. After saving these arguments in class,
 the determination of the current routing path is occurred. It is determined either by pressing a button in the bot (the ``callback_data`` value of the button), or
 can be stored in the user attribute ``user.current_utrl``. The second option is possible if the user manually enters
 some information (for example, filled in a text field of form). After that, the arguments are extracted from the path
 to call a specific function. Storing and interacting with arguments in a path is similar to how ``sys.argv`` works. So,
-for example, the string ``"sl&1&20"`` will be converted to the list ``['sl', '1', '20']``. Separator character between attributes
+for example, the string ``"sl&1&20"`` will be converted to the list ``['sl', '1', '20']``. The separator character between attributes
 is ``&`` by default and can be changed via the ``TelegaViewSet.ARGS_SEPARATOR_SYMBOL`` variable.
 
 When using ``TelegaViewSet`` you most likely won't have to interact with the argument string directly, since
-how ``dispatch`` converts a string into arguments, and to create a string for a ``callback_data`` button for calling another method by user, you should use
+``dispatch`` converts a string into arguments. And for creating a ``callback_data`` button string, that the user can call another method from Telegram interface, you should use
 ``TelegaViewSet.gm_callback_data`` function. In case you need more low-level interaction with function arguments, then
 you can use the ``construct_utrl`` and ``get_utrl_params`` functions.
 
 After receiving the utrl_args arguments and checking access rights, the managing method (action) is directly selected and called.
 The first argument, which is the short name for the function, is popped from the utrl_args. All other arguments are passed as parameters
-into a function. Inside the function, the necessary business logic and the data formating for displaying to the user as a response take place.
+into a function. Inside the function, the necessary business logic and the data formatting for displaying to the user as a response take place.
 Any such managing function in the ``TelegaViewSet`` class must return the action type ``chat_action`` and the parameters to that action ``chat_action_args``.
-By default, the  class has only 1 action ﹣ ``CHAT_ACTION_MESSAGE``, which means that the user will receive
-a text message (possibly with buttons) as an answer for his/her action. The arguments to this action are the text of the message and a list of buttons (can be None).
+By default, the class has only 1 action ﹣ ``CHAT_ACTION_MESSAGE``, which means that the user will receive
+a text message (possibly with buttons) as an answer for his/her action. The arguments for this action are the text of the message and a list of buttons (can be None).
 
 
-After the function is processed, a response is sent to the user  by ``send_answer`` function and the user's action is logged.
+After the function is processed, a response is sent to the user by ``send_answer`` function and the user's action is logged.
 
 
 The methods to call in ``viewset_routing`` are the ``create, update, delete, show_elem, show_list`` methods.
 You can also add your own methods. Suppose we want to add a ``def super_method(self, *args)`` method, then
 you need to add the following lines in the class:
 
 .. code-block:: python
 
-    class SomeViewSetClass(TelegaViewSet):
+    class SomeViewSetClass(TelegramViewSet):
         ...
 
         actions = ['create', 'change', 'delete', 'show_elem', 'show_list', 'super_method']
 
         command_routing_super_method = 'sm'
 
 
@@ -515,45 +524,45 @@
 Where ``actions`` defines the list of available methods and ``command_routing_<method>`` defines the path (url; short name) of the method.
 
 As noted above, the ``dispatch`` method performs a permissions check by calling the ``has_permissions`` method.
 The check is performed by the classes specified in ``permission_classes`` and the default class is ``AllowAny``:
 
 .. code-block:: python
 
-    class TelegaViewSet:
+    class TelegramViewSet:
         permission_classes = [AllowAny]
 
 
 
-Additional TelegaViewSet Tools
+Additional TelegramViewSet Tools
 ************************************************
 
 This section describes the following class functionality that makes it easier to write code:
 
 1. External filters;
 2. Data display setting options;
 3. Helper functions for displaying data;
 4. Helper functions of business logic;
 
 
 External filters
 +++++++++++++++++++++
 
-Quite often, there is situation when you need to work not with all the elements of a database table, but with some
+Quite often, there is a situation when you need to work not with all the elements of a database table, but with some
 group (for example, a group of elements with a specific foreign key). For such purposes, you should use the ``foreign_filters`` list,
 which stores the values for filtering when the method is called. How exactly to use these filters is up to you, but
-usually it is good idea to use it in the ``get_queryset`` function. Thus, it is possible to pass to functions
+usually it is a good idea to use it in the ``get_queryset`` function. Thus, it is possible to pass to functions
 additional arguments that do not break the key logic of standard functions. Using the template example, you can modify
 ``BotMenuElemViewSet`` so that if an additional parameter is specified, then the BotMenuElem list displays
 only those elements that contain the specified parameter in their ``command`` attribute. To do this, you need to make the following changes to the code:
 
 
 .. code-block:: python
 
-    class BotMenuElemViewSet(TelegaViewSet):
+    class BotMenuElemViewSet(TelegramViewSet):
         ...
 
         foreign_filter_amount = 1
 
         def get_queryset(self):
             queryset = super().get_queryset()
             if self.foreign_filters[0]:
@@ -572,15 +581,15 @@
 This allows you to change the value of filters when generating paths.
 
 A more detailed use of external filters can be seen in the example of `Drive Bot <https://github.com/alexanderaleskin/drive_bot>`_ .
 
 Data display options
 ++++++++++++++++++++++++++++++++++++++++++
 
-The ``TelegaViewSet`` has the following options for displaying model elements:
+The ``TelegramViewSet`` has the following options for displaying model elements:
 
 * ``updating_fields: list`` - list of fields that can be changed (displayed when showing the element (``show_elem``);
 * ``show_cancel_updating_button: bool = True`` - shows a cancel button when changing fields, which leads back to the displaying element (``show_elem``);
 * ``deleting_with_confirm: bool = True`` - ask the user for confirmation when deleting an element;
 * ``cancel_adding_button: InlineKeyboardButtonDJ = None`` - cancel button when creating an element (``create`` method);
 * ``use_name_and_id_in_elem_showing: bool = True`` - enables the use of the name and ID of the element when displaying this element (methods ``show_list`` and ``show_elem``);
 * ``meta_texts_dict: dict`` - a dictionary that stores standard texts for display (texts are used in all methods).
@@ -610,17 +619,17 @@
 
 Depending on the need for customization, it is necessary to redefine these functions.
 
 
 Helper functions of business logic
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
-The ``TelegaViewSet`` class uses the following helper functions:
+The ``TelegramViewSet`` class uses the following helper functions:
 
-* ``def get_queryset`` - allows you to modify Model queries to database (most often used to filter elements, as in the example above);
+* ``def get_queryset`` - allows you to modify Model queries to the database (most often used to filter elements, as in the example above);
 * ``def create_or_update_helper`` - main logic for ``create`` and ``update`` methods;
 * ``def show_list_get_queryset`` - allows you to customize the selection of items to display in show_list;
 
 
 handler_decor
 ~~~~~~~~~~~~~~~~
 
@@ -642,46 +651,45 @@
 To support the use of different languages, the main elements of the Python-Telegram-Bot library are redefined in ``telegram_django_bot.telegram_lib_redefinition``:
 
 
 1. ``telegram.Bot`` -> ``telegram_django_bot.BotDJ`` ;
 2. ``telegram.ReplyMarkup`` -> ``telegram_django_bot.ReplyMarkupDJ`` ;
 3. ``telegram.KeyboardButton`` -> ``telegram_django_bot.KeyboardButtonDJ`` ;
 4. ``telegram.InlineKeyboardButton`` -> ``telegram_django_bot.InlineKeyboardButtonDJ`` ;
-5. ``telegram.InlineKeyboardMarkup`` -> ``telegram_django_bot.InlineKeyboardMarkupDJ``;
-
+5. ``telegram.InlineKeyboardMarkup`` -> ``telegram_django_bot.InlineKeyboardMarkupDJ``.
 
 
 When using these classes in code, multilingual support comes down to the following steps:
 
 1. Specifying the necessary settings in the settings.py file: ``LANGUAGES`` - list of languages, ``LANGUAGE_CODE`` - default language;
 1. Necessary texts for translation are wrapped in ``gettext`` and ``gettext_lazy`` from ``django.utils.translation`` (how it works in Django `read here <https://docs.djangoproject.com/en /4.1/topics/i18n/translation/#standard-translation>`_ )
 2. Run command ``$ django-admin makemessages -a`` to generate texts for translation (created in locale folder)
 3. Generation of translation files ``$ django-admin compilemessages``.
 
-Only a part of the functions uses localization in the template. It is made for easy understanding. Usage of localization can be seen in the example
+Only a part of the functions uses localization in the template. It is made for easy understanding. The usage of localization can be seen in the example
 functions ``some_debug_func``.
 
 
 Extra lib features
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 The library provides some additional tools for the convenience of developing and managing the bot.
 
 Модели библиотеки
 ************************************
 
 
-For the correct work of ``TelegaViewSet`` and other components the Django ORM model representing the user in the Telegram must be inherited
+For the correct work of ``TelegaViewSet`` and other components the Django ORM model representing the user in Telegram must be inherited
 from ``telegram_django_bot.models.TelegramUser``, as these components use its fields. ``TelegramUser`` inherited from
 ``django.contrib.auth.models.AbstractUser`` (which allows you to authorize users on the site if necessary) and has
 the following additional fields:
 
 * ``id`` - redefined to use user ID from telegrams;
 * ``seed_code`` - arbitrary value from 1 to 100 to randomly group users for tests and analysis;
-* ``telegram_username`` - username of the user in the telegram;
+* ``telegram_username`` - username of the user in telegram;
 * ``telegram_language_code`` - telegram language code (some languages have dialects and as a result the code designation is more than 2 symbols);
 * ``timezone`` - the user's time zone (for determining the time);
 * ``current_utrl`` - path (utrl) of the last user action (used in ``TelegaViewSet``);
 * ``current_utrl_code_dttm`` - time of the last action, when saving the path;
 * ``current_utrl_context_db`` - path context (utrl);
 * ``current_utrl_form_db`` - intermediate data for the form. Acts as a temporary data store when filling out a form;
 
@@ -692,15 +700,15 @@
 * ``current_utrl_context`` (property) - returns the current path context (utrl);
 * ``save_form_in_db`` - saves the form in the ``current_utrl_form_db`` field;
 * ``save_context_in_db`` - saves the context in the field ``current_utrl_context_db``;
 * ``clear_status`` - clears the data associated with the used path (fields ``current_utrl_<suffix>``) ;
 * ``language_code`` (property) - returns the language code in which messages should be generated for the user;
 
 
-Actually, if you want, you can create your self Django ORM model representing the user, you just need to copy
+If you want, you can create your self Django ORM model representing the user, you just need to copy
 ``id, telegram_username, telegram_language_code, current_utrl, current_utrl_code_dttm, current_utrl_context_db, current_utrl_form_db``
 and corresponding functions.
 
 
 The library also describes additional models to improve the usability of the bot:
 
 * ``ActionLog`` - stores user actions. Records help to collect analytics and make triggers that work on certain actions;
@@ -712,15 +720,15 @@
 
 
 Additional functions of TG_DJ_Bot
 *********************************************
 
 To improve convenience, ``TG_DJ_Bot`` has several high-level functions:
 
-* ``send_format_message`` - Allows you to send a message of an arbitrary type (internally, depending on the ``message_format`` selects the appropriate method of the ``Python-Telegram-Bot`` library). An important feature of this function is that if the user clicks on the button, then the previous message of the bot is changed, rather than a new one is sent. If, nevertheless, in this case you need to send a new message to the user, then you need to set the parameter ``only_send=True`` ;
+* ``send_format_message`` - Allows you to send a message of an arbitrary type (internally, depending on the ``message_format`` selects the appropriate method of the ``Python-Telegram-Bot`` library). An important feature of this function is that if the user clicks on the button, then the previous message of the bot is changed, rather than a new one being sent. If, nevertheless you need to send a new message to the user, then you need to set the parameter ``only_send=True`` ;
 * ``edit_or_send`` - wrapper of the ``send_format_message`` method for sending text messages with buttons;
 * ``send_botmenuelem`` - Sends a ``BotMenuElem`` to the user. The ``update`` argument can be empty;
 * ``task_send_message_handler`` - created for sending messages to many users. Handles situations where the user blocked the bot, deleted or when the limit for sending messages to users is reached;
 
 
 Utils
 **********
@@ -742,31 +750,31 @@
 Django. Also ``RouterCallbackMessageCommandHandler`` provides the ability to handle calls to ``BotMenuElem`` as
 through commands, and through callback. This is achieved by using the functions ``all_command_bme_handler`` and
 ``all_callback_bme_handler``. By default, ``BotMenuElem`` call handling is enabled and handled after
 no suitable path was found in the description of utrls (paths in Django notation). If there is no ``BotMenuElem`` element
 match is found, the ``BotMenuElem`` is considered to be configured incorrectly and an error message is returned to the user.
 You can create a class with the ``only_utrl=True`` attribute, what is disable calls to ``BotMenuElem``.
 
-The example template contains the use of the ``telega_reverse`` function, the essence of which is to generate a path (string) to
+The example template contains the use of the ``telega_reverse`` function, the essence of which is to generate a path (string) to the
 handler specified in the function argument. The function is analogous to the `reverse <https://docs.djangoproject.com/en/4.1/ref/urlresolvers/#reverse>`_ Django function
 and avoids errors when changing paths.
 
 
 
 Tests
 **********************
 
 The library also extends the ``django.test.TestCase`` capabilities for use with Telegram through the ``TD_TestCase`` class.
 
 The simplest approach for testing the bot is to generate messages that the bot expects from Telegram and
-sending a response to Telegram (to check that the bot's response messages are in the correct format). Class ``TD_TestCase``
+send a response to Telegram (to check that the bot's response messages are in the correct format). Class ``TD_TestCase``
 has a function ``create_update`` for easy and fast creation of ``Telegram.Update`` which generates the request
 telegram user. So the overall design looks like this:
 
 1. A ``Telegram.Update`` is created for emitting a user request;
-2. The ``handle_update`` lambda function, which uses ``RouterCallbackMessageCommandHandler``,  is called with created update. It does its staff and as a result sends a real message to the test user. Due to this, the correctness of the responsing data format  is checked by Telegram;
+2. The ``handle_update`` lambda function, which uses ``RouterCallbackMessageCommandHandler``,  is called with created update. It does its staff and as a result sends a real message to the test user. Due to this, the correctness of the response data format  is checked by Telegram;
 3. The correctness of the sent data and changes in the database is checked using the standard tools ``django.test.TestCase``.
 
 You need to specify at least one test user ID in the ``TELEGRAM_TEST_USER_IDS`` settings section for correct tests work.
 Messages will be sent to that user, so the bot needs to have permission to write to that user.
 
 In the ``tests`` folder you could find test examples.
```

### Comparing `telegram_django_bot-1.0.1/setup.cfg` & `telegram_django_bot-1.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = telegram_django_bot
-version = 1.0.1
+version = 1.0.2
 description = Telegram Django Bot Bridge
 long_description = file: README.rst
 url = https://github.com/alexanderaleskin/telegram_django_bot_bridge
 author = Alexander Aleskin
 author_email = alexanderaleskin@gmail.com
 license = MIT
 classifiers =
```

### Comparing `telegram_django_bot-1.0.1/telegram_django_bot/admin.py` & `telegram_django_bot-1.0.2/telegram_django_bot/admin.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.1/telegram_django_bot/admin_utils.py` & `telegram_django_bot-1.0.2/telegram_django_bot/admin_utils.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.1/telegram_django_bot/forms.py` & `telegram_django_bot-1.0.2/telegram_django_bot/forms.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.1/telegram_django_bot/locale/ru/LC_MESSAGES/django.mo` & `telegram_django_bot-1.0.2/telegram_django_bot/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.1/telegram_django_bot/locale/ru/LC_MESSAGES/django.po` & `telegram_django_bot-1.0.2/telegram_django_bot/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.1/telegram_django_bot/migrations/0001_initial.py` & `telegram_django_bot-1.0.2/telegram_django_bot/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.1/telegram_django_bot/migrations/0003_botmenuelem_message_format.py` & `telegram_django_bot-1.0.2/telegram_django_bot/migrations/0003_botmenuelem_message_format.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.1/telegram_django_bot/migrations/0004_auto_20220915_0448.py` & `telegram_django_bot-1.0.2/telegram_django_bot/migrations/0004_auto_20220915_0448.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.1/telegram_django_bot/migrations/0007_auto_20221202_0305.py` & `telegram_django_bot-1.0.2/telegram_django_bot/migrations/0007_auto_20221202_0305.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.1/telegram_django_bot/migrations/0008_auto_20221225_1050.py` & `telegram_django_bot-1.0.2/telegram_django_bot/migrations/0008_auto_20221225_1050.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.1/telegram_django_bot/models.py` & `telegram_django_bot-1.0.2/telegram_django_bot/models.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.1/telegram_django_bot/routing.py` & `telegram_django_bot-1.0.2/telegram_django_bot/routing.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,26 @@
 from .models import BotMenuElem
 from .utils import handler_decor
 from .td_viewset import TelegaViewSet
 from django.urls import resolve, Resolver404, reverse
 from django.conf import settings
 from django.contrib.auth import get_user_model
 
-import telegram
+from telegram import (
+    Update,
+)
 import inspect
 
-from telegram.ext import Handler
+
+try:
+    # version 20.x +
+    from telegram.ext import BaseHandler as Handler
+except ImportError:
+    # old version
+    from telegram.ext import Handler
 
 
 def telega_resolve(path, utrl_conf=None):
     if path[0] != '/':
         path = f'/{path}'
 
     if '?' in path:
@@ -103,15 +111,15 @@
 
     def check_update(self, update: object):
         """
         check if callback or message (command actually is message)
         :param update:
         :return:
         """
-        if isinstance(update, telegram.Update) and (update.effective_message or update.callback_query):
+        if isinstance(update, Update) and (update.effective_message or update.callback_query):
             callback = self.get_callback_utrl(update)
             if callback:
                 return True
             elif not self.only_utrl:
                 if update.message and update.message.text and update.message.text[0] == '/':
                     # if it is a command then it should be  early in handlers
                     # or in BME (then return True
```

### Comparing `telegram_django_bot-1.0.1/telegram_django_bot/tasks.py` & `telegram_django_bot-1.0.2/telegram_django_bot/tasks.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.1/telegram_django_bot/td_viewset.py` & `telegram_django_bot-1.0.2/telegram_django_bot/td_viewset.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.1/telegram_django_bot/templates/dropdown_filter1.html` & `telegram_django_bot-1.0.2/telegram_django_bot/templates/dropdown_filter1.html`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.1/telegram_django_bot/test.py` & `telegram_django_bot-1.0.2/telegram_django_bot/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,27 @@
 from telegram import Update, Message, Chat, User as TelegramAPIUser, CallbackQuery
 from telegram_django_bot.routing import RouterCallbackMessageCommandHandler
 # from telegram.utils.types import JSONDict, ODVInput
 # from telegram.utils.helpers import DEFAULT_NONE
 # from typing import Union
 
 from .tg_dj_bot import TG_DJ_Bot
+# import asyncio
 
 
 test_bot = TG_DJ_Bot(token=settings.TELEGRAM_TOKEN)
 if hasattr(settings, 'TELEGRAM_TEST_USER_IDS'):
     TELEGRAM_TEST_USER_IDS = settings.TELEGRAM_TEST_USER_IDS
     for user_id in TELEGRAM_TEST_USER_IDS:
         try:
-            test_bot.send_message(user_id, 'ping')
+            res = test_bot.send_message(user_id, 'ping')
+
+            # if asyncio.iscoroutine(res):
+            #     asyncio.run(res)
+
         except Exception as error:
             logging.error(
                 f'the error {error} occurred while sending test message to TELEGRAM_TEST_USER_ID={user_id} '
                 f'by bot {test_bot.id}. Please, check details'
             )
 else:
     TELEGRAM_TEST_USER_IDS = []
@@ -45,15 +50,15 @@
 
         self.test_callback_context = TestCallbackContext()
         self.rc_mch = RouterCallbackMessageCommandHandler()
         self.handle_update = lambda update: self.rc_mch.handle_update(
             update, 'some_str', 'some_str', self.test_callback_context
         )
 
-    def create_update(self, message_kwargs:dict=None, callback_kwargs:dict=None, user_id=None,):
+    def create_update(self, message_kwargs: dict = None, callback_kwargs: dict = None, user_id=None,):
         if user_id is None and len(TELEGRAM_TEST_USER_IDS):
             user_id = TELEGRAM_TEST_USER_IDS[0]
 
         if user_id is None:
             raise ValueError('the user_id (or TELEGRAM_TEST_USER_IDS) should be set for creating Update model')
 
         chat = Chat(id=user_id, type='private')
```

### Comparing `telegram_django_bot-1.0.1/telegram_django_bot/tg_dj_bot.py` & `telegram_django_bot-1.0.2/telegram_django_bot/tg_dj_bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,25 @@
 
         if menu_elem is None:
             if settings.USE_I18N:
                 translation.activate(user.language_code)
 
             message_format = MESSAGE_FORMAT.TEXT
             mess = str(ERROR_MESSAGE)
-            logging.warning('Try to find BME, but there is no such models, so the error message shown for the client')
+
+            utrl = ''
+            if update:
+                if update.message:
+                    utrl = update.message.text
+                elif update.callback_query:
+                    utrl = update.callback_query.data
+
+            logging.warning(
+                f'Try to find BME {utrl}, but there is no such models, so the error message shown for the client'
+            )
         else:
             language_code = settings.LANGUAGE_CODE
             if settings.USE_I18N and user.language_code != settings.LANGUAGE_CODE:
                 language_code = user.language_code
 
             message_format = menu_elem.message_format
             mess = menu_elem.get_message(language_code)
@@ -89,15 +99,15 @@
 
             **extra_kwargs,
         )
 
         if menu_elem and menu_elem.telegram_file_code is None and menu_elem.media and len(media_codes) > 0:
             menu_elem.telegram_file_code = media_codes[0]
             menu_elem.save()
-        return [response]
+        return response
 
     def send_format_message(
             bot,
             message_format: str = MESSAGE_FORMAT.TEXT,
             text: str = None,
             media_files_list: list = None,
             update: Update = None,
```

### Comparing `telegram_django_bot-1.0.1/telegram_django_bot/user_viewset.py` & `telegram_django_bot-1.0.2/telegram_django_bot/user_viewset.py`

 * *Files identical despite different names*

### Comparing `telegram_django_bot-1.0.1/telegram_django_bot/utils.py` & `telegram_django_bot-1.0.2/telegram_django_bot/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,20 +99,20 @@
             raise_error = None
             try:
                 res = func(bot, update, user)
             except telegram.error.BadRequest as error:
                 if 'Message is not modified:' in error.message:
                     res = None
                 else:
-                    res = [bot.send_message(user.id, str(ERROR_MESSAGE))]  # should be bot.send_format_message
+                    res = bot.send_message(user.id, str(ERROR_MESSAGE))  # should be bot.send_format_message
                     tb = sys.exc_info()[2]
                     raise_error = error.with_traceback(tb)
             except Exception as error:
 
-                res = [bot.send_message(user.id, str(ERROR_MESSAGE))]  # should be bot.send_format_message
+                res = bot.send_message(user.id, str(ERROR_MESSAGE))  # should be bot.send_format_message
                 tb = sys.exc_info()[2]
                 raise_error = error.with_traceback(tb)
 
             # log actions
 
             if log_type != 'N':
                 if log_type == 'C':
```

### Comparing `telegram_django_bot-1.0.1/telegram_django_bot.egg-info/PKG-INFO` & `telegram_django_bot-1.0.2/telegram_django_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: telegram-django-bot
-Version: 1.0.1
+Version: 1.0.2
 Summary: Telegram Django Bot Bridge
 Home-page: https://github.com/alexanderaleskin/telegram_django_bot_bridge
 Author: Alexander Aleskin
 Author-email: alexanderaleskin@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
@@ -29,72 +28,46 @@
 Classifier: Topic :: Internet
 Requires-Python: >=3.8
 License-File: LICENSE
 
 Telegram Django Bot Bridge
 ============================
 
-This library provides a Python interface for creating Telegram Bots. It standardizes coding approach in the best
-practice of the web development. The library combines `Django <https://www.djangoproject.com/>`_ and `Python-Telegram-Bot <https://python-telegram-bot.org/>`_.
-and provides extra powerful utilities based on these libraries.
-
-
-Normally, Python-Telegram-Bot gives next opportunities for bot creating:
-
-* Python Interface for communication with Telegram API;
-* Web-service to get updates from telegram;
-
-and Django:
-
-* Django ORM  (communication with Database);
-* Administration panel for management.
-
-
-Telegram Django Bot Bridge provides next special opportunities:
-
-* using Django Forms;
-* using Viewsets (typical action with model (create, update, list, delete));
-* using Django localization.
-* using function routing like urls routing in Django.
-
-And some extra useful staff:
-
-* using function routing like urls routing in Django;
-* creating tests;
-* creating general menu items with no-coding (through Django Admin Panel);
-* extra high-level Bot functions, such as wrapper for sending delayed (or scheduled) messages;
-* collecting stats from user actions in the bot;
-* creating user triggers;
-* commonly used utilities.
-
+This library provides a Python high-level interface for creating Telegram Bots. It standardizes the coding in the best
+practice of the web development. The library is based on `Django <https://www.djangoproject.com/>`_ and `Python-Telegram-Bot <https://python-telegram-bot.org/>`_.
+and provides viewset interface for managing data with.
 
+If you start a new project, you could use `Telegram django bot template <https://github.com/alexanderaleskin/telergam_django_bot_template>`_ with preconfigured settings.
 
 Install
 ------------
 
 You can install via ``pip``:
 
 .. code-block:: shell
 
     $ pip install telegram_django_bot
 
 
-Then you can configurate it in your app:
+Then you can configure it in your app:
 
 
 1. Add "telegram_django_bot" to your INSTALLED_APPS setting like this:
 
 .. code-block:: python
 
     INSTALLED_APPS = [
         ...
         'telegram_django_bot',
+        'django_json_widget', # needed for django admin site
     ]
 
 
+If you are planning to use Django in asynchronous mode, then you need to set ``DJANGO_ALLOW_ASYNC_UNSAFE = True`` (otherwise DB writings will be failed).
+
 
 2. Run ``python manage.py migrate`` to create the telegram_django_bot models (checked that the ``AUTH_USER_MODEL`` selected
 in settings).
 
 
 3. Set up constants in Django settings file:
 
@@ -110,34 +83,68 @@
 4. This step connects ``Telegram Django Bot Bridge`` with ``Python-Telegram-Bot``. Add ``RouterCallbackMessageCommandHandler`` in handlers for using TELEGRAM_ROOT_UTRLCONF :
 
 .. code-block:: python
 
     updater = Updater(bot=TG_DJ_Bot(settings.TELEGRAM_TOKEN))
     updater.dispatcher.add_handler(RouterCallbackMessageCommandHandler())
 
+or in 20.x version :
+
+.. code-block:: python
+
+    bot = TG_DJ_Bot(settings.TELEGRAM_TOKEN)
+    application = ApplicationBuilder().bot(bot).build()
+    application.add_handler(RouterCallbackMessageCommandHandler())
+
+    
 
-If you start a new project, you could use `Telegram django bot template <https://github.com/alexanderaleskin/telergam_django_bot_template>`_ with preconfigured settings.
 
 
 Quick start
 ------------
 
 
+Normally, Python-Telegram-Bot gives the next opportunities for bot creation:
+
+* Python Interface for communication with Telegram API;
+* Web service to get updates from telegram;
+
+and Django:
+
+* Django ORM  (communication with Database);
+* Administration panel for management.
 
-The key feature of the lib is ``TelegaViewSet`` - class for manage Django ORM model. It is designed in the
+
+Telegram Django Bot Bridge provides next special opportunities:
+
+* using Viewsets (typical action with model (create, update, list, delete));
+* using Django localization.
+* using function routing like urls routing in Django.
+
+And some extra useful staff:
+
+* creating general menu items with no-coding (through Django Admin Panel);
+* extra high-level Bot functions, such as a wrapper for sending delayed (or scheduled) messages;
+* creating tests;
+* collecting stats from user actions in the bot;
+* commonly used utilities.
+
+
+
+The key feature of the lib is ``TelegramViewSet`` - a class for managing Django ORM model. It is designed in a
 similar way as `Django rest framework Viewset <https://www.django-rest-framework.org/api-guide/viewsets/>`_ , but has
-a significant difference: while DRF Viewset provides response in serializable format (usually in json format) to frontend app, TelegaViewSet
-provides response to user in telegram interface in message format with buttons. So, you will manage data and receive
-response in human format by executing TelegaViewSet method. The methods use some kind of templates for generating human
-response (it is possible to overwrite these templates). By default, TelegaViewSet has 5 methods:
+a significant difference: while DRF Viewset provides a response in serializable format (usually in json format) to frontend app, TelegaViewSet
+provides a response to the user in telegram interface in message format with buttons. So, you will manage data and receive
+responses in human format by executing TelegaViewSet method. The methods use some kind of templates for generating human
+responses (it is possible to overwrite these templates). By default, TelegaViewSet has 5 methods:
 
-* ``create`` - create a new instance of specified ORM model;
+* ``create`` - create a new instance of the specified ORM model;
 * ``change`` - update instance fields of specified ORM model;
-* ``show_elem`` - show fields of the instance and buttons with actions of this instance;
-* ``show_list`` - show list of model instance (with pagination);
+* ``show_elem`` - show fields of the element and buttons with actions of this instance;
+* ``show_list`` - show list of model elements (with pagination);
 * ``delete`` - delete the instance
 
 
 So, if, for example, you have a model of some *request* in your project:
 
 .. code-block:: python
 
@@ -146,39 +153,39 @@
     class Request(models.Model):
         text = models.TextField()
         importance_level = models.PositiveSmallIntegerField()  # for example it will be integer field
         project = models.ForeignKey('Project', on_delete=models.CASCADE)
         tags = models.ManyToManyField('Tags')
 
 
-The next piece of code gives opportunity for full managing (create, update, show, delete) of this model from Telegram:
+The next piece of code gives the opportunity for full managing (create, update, show, delete) of this model from Telegram:
 
 .. code-block:: python
 
     from telegram_django_bot import forms as td_forms
-    from telegram_django_bot.td_viewset import TelegaViewSet
+    from telegram_django_bot.td_viewset import TelegramViewSet
 
 
     class RequestForm(td_forms.TelegaModelForm):
         class Meta:
             model = Request
             fields = ['text', 'importance_level', 'project', 'tags']
 
 
-    class RequestViewSet(TelegaViewSet):
+    class RequestViewSet(TelegramViewSet):
         telega_form = RequestForm
         queryset = Request.objects.all()
         viewset_name = 'Request'
 
 
-If you need, you can add extra actions to RequestViewSet for managing (see details information below) or change existed functions.
+If you need, you can add extra actions to RequestViewSet for managing (see details information below) or change existing functions.
 There are several parameters and secondary functions in TelegaViewSet for customizing logic if it is necessary.
 
 In this example, ``TelegaModelForm`` was used. TelegaModelForm is a descendant of Django ModelForm. So, you could use
-labels, clean and other parameters and functions for managing logic and displaying.
+labels, clean functions and other parameters and functions for managing logic and displaying.
 
 
 TelegaViewSet is designed to answer next user actions: clicking buttons and sometimes sending messages. The library imposes
 `Django URL notation <https://docs.djangoproject.com/en/4.1/topics/http/urls/>`_ for mapping user actions to TelegaViewSet methods (or usual handlers).
 Usually, for correct mapping you just need to set ``TELEGRAM_ROOT_UTRLCONF`` and use ``RouterCallbackMessageCommandHandler`` in
 dispatcher as it is mentioned above in the *Install paragraph*.
 
@@ -207,28 +214,30 @@
 
 
 Deep in details
 ------------------
 
 In this chapter, we will analyze how everything works. The main task of the library is to unify the code and
 provide frequently used functions for developing a bot, that is why a lot of logic is based on resources and paradigms
-Django <https://www.djangoproject.com/>`_ and `Python-Telegram-Bot <https://python-telegram-bot.org/>`_ . Let's analyze
+of Django <https://www.djangoproject.com/>`_ and `Python-Telegram-Bot <https://python-telegram-bot.org/>`_ . Let's analyze
 key features of the library on the example of `Telegram django bot template <https://github.com/alexanderaleskin/telergam_django_bot_template>`_ .
 
+.. important::
+
+    The template is based on 13.x Python-Telegram-Bot version (synchronous version). So, the next examples is suitable for that version. For use with 20.x versions you need to do some modification.
+
 
 Since Telegram bots are designed as a tool for responding to user requests, writing a bot begins
 from the user request handler. For this, the standard tools of the Python-Telegram-Bot library are used ﹣
 ``telegram.ext.Update``:
 
 .. code-block:: python
 
      from telegram.ext import Updater
 
-     ...
-
      def main():
          ...
 
          updater = Updater(bot=TG_DJ_Bot(TELEGRAM_TOKEN))
          add_handlers(updater)
          updater.start_polling()
          updater.idle()
@@ -239,15 +248,14 @@
 
 As indicated in the example, to run the bot (Update) you need to specify a few things (the ``Python-Telegram-Bot`` library standard):
 
 1. an instance of the ``telegram.Bot`` model with the specified API token. In this case, a descendant ``telegram_django_bot.tg_dj_bot.TG_DJ_Bot``
 of the ``telegram.Bot`` class is used. It has additional functionality for convenience (we will return to it later);
 2. Handlers that will be called in response to user requests.
 
-
 In the example, the list of handlers is specified in the ``add_handlers`` function:
 
 
 
 .. code-block:: python
 
      from telegram_django_bot.routing import RouterCallbackMessageCommandHandler
@@ -296,16 +304,16 @@
 There is following code in the specified included file ``base.utrls.py`` :
 
 
 .. code-block:: python
 
     from django.urls import re_path
     from django.conf import settings
-
-    from .views import start, BotMenuElemViewSet, UserViewSet, some_debug_func
+    from telegram_django_bot.user_viewset import UserViewSet
+    from .views import start, BotMenuElemViewSet, some_debug_func
 
 
     urlpatterns = [
         re_path('start', start, name='start'),
         re_path('main_menu', start, name='start'),
 
         re_path('sb/', BotMenuElemViewSet, name='BotMenuElemViewSet'),
@@ -342,43 +350,43 @@
 change     up       Change model attributes
 delete     de       Deleting a model
 show_elem  se       Display a model
 show_list  sl       Display a list of models
 ========= ======== ===========================
 
 Thus, if we want to call the ``BotMenuElemViewSet.create`` method to create an element, we need to use
-path 'sb/cr', where by the first part of path 'sb/'  the router ``RouterCallbackMessageCommandHandler`` will execute
+path 'sb/cr', whereby the first part of the path 'sb/'  the router ``RouterCallbackMessageCommandHandler`` will execute
 the ``BotMenuElemViewSet`` class, namely the ``TelegaViewSet.dispatch`` method, which in turn will call  the ``create`` method by analyzing the second part of the path
 ``cr``.
 
 To sum up the scheme of handlers routing, there are following key points:
 
 1. ``telegram.ext.Update`` is used as a receiver of messages from Telegram;
 2. Standard handlers of the ``Python-Telegram-Bot`` library can be used as handlers. For convenient use Django's path scheme and ``TelegaViewSet`` you need to use ``RouterCallbackMessageCommandHandler``.
 3. ``TelegaViewSet`` aggregates a set of standard functions for managing data, what is made possible to group code associated with one type of data type in one class (place).
 
 
 
-TelegaViewSet features
+TelegramViewSet features
 ~~~~~~~~~~~~~~~~~~~~~~~~
 
 As described above, TelegaViewSet contains standard functions for data manipulation.
 Due to such standard data processing methods, it turns out in the example to describe the logic of ``BotMenuElemViewSet`` in 40
-lines of code, also using some customization for a beautiful data displaying.
+lines of code, also using some customization for beautiful data displaying.
 
 
 To use all the features of the TelegaViewSet in your class, it should be inherited from it, as, for example, this is done
 in the ``BotMenuElemViewSet``:
 
 
 .. code-block:: python
 
-    from telegram_django_bot.td_viewset import TelegaViewSet
+    from telegram_django_bot.td_viewset import TelegramViewSet
 
-    class BotMenuElemViewSet(TelegaViewSet):
+    class BotMenuElemViewSet(TelegramViewSet):
 
 
 In order to customize the ViewSet, you must specify 3 required attributes:
 
 1. ``viewset_name`` - class name, used to display to telegram users
 2. ``telega_form`` - data form, used to specify which fields of the ORM database model to use in the viewset;
 3. ``queryset`` - basic query for getting model elements.
@@ -433,24 +441,24 @@
 1. The clean function and other `form validation process functions <https://docs.djangoproject.com/en/4.1/ref/forms/validation/>`_ ;
 2. ``labels`` - field names;
 3. ``forms.HiddenInput`` - designation of hidden fields (hiding fields allows them not to be shown to the user, while using and configuring in forms or in ``TelegaViewSet``).
 
 
 
 ``TelegaViewSet`` is designed to interact with descendants of the ``TelegaModelForm`` class and allows you to use
-generate forms with different fields, such as ``CharField, IntegerField`` or ``ForeignKey, ManyToManyField``. Also, it is good idea
+generate forms with different fields, such as ``CharField, IntegerField`` or ``ForeignKey, ManyToManyField``. Also, it is a good idea
 to use the ``prechoice_fields_values`` dictionary in ``TelegaViewSet`` descendants for improving the convenience of filling out forms for users.
 It is possible to store a list of frequently used values of form fields in the ``prechoice_fields_values``.
 This allows users to select the desired values by clicking buttons rather than
 writing text manually. The template has an example of using this field:
 
 
 .. code-block:: python
 
-    class BotMenuElemViewSet(TelegaViewSet):
+    class BotMenuElemViewSet(TelegramViewSet):
         ...
 
         prechoice_fields_values = {
             'is_visable': (
                 (True, '👁 Visable'),
                 (False, '🚫 Disabled'),
             )
@@ -458,18 +466,18 @@
 
 In this case, 2 values are specified for choosing true or false for the boolean field ``is_visable``. You can also use
 ``prechoice_fields_values`` for ``CharField, IntegerField`` or any other fields.
 Sometimes the list of values needs to be generated dynamically, in which case you can override
 ``prechoice_fields_values`` as a ``@property`` function.
 
 
-Key logic of TelegaViewSet
+Key logic of TelegramViewSet
 ************************************************
 
-The main function of the class, which is selected the function for managing data by the request of the user,  is ``TelegaViewSet.dispatch``.
+The main function of the class, which is selected the function for managing data by the request of the user,  is ``TelegramViewSet.dispatch``.
 Let's analyze its logic in more detail:
 
 .. code-block:: python
 
     def dispatch(self, bot, update, user):
 
         self.bot = bot
@@ -503,40 +511,40 @@
 
 
 Like a regular handler, the function takes 3 arguments as input: bot, update, user. After saving these arguments in class,
 the determination of the current routing path is occurred. It is determined either by pressing a button in the bot (the ``callback_data`` value of the button), or
 can be stored in the user attribute ``user.current_utrl``. The second option is possible if the user manually enters
 some information (for example, filled in a text field of form). After that, the arguments are extracted from the path
 to call a specific function. Storing and interacting with arguments in a path is similar to how ``sys.argv`` works. So,
-for example, the string ``"sl&1&20"`` will be converted to the list ``['sl', '1', '20']``. Separator character between attributes
+for example, the string ``"sl&1&20"`` will be converted to the list ``['sl', '1', '20']``. The separator character between attributes
 is ``&`` by default and can be changed via the ``TelegaViewSet.ARGS_SEPARATOR_SYMBOL`` variable.
 
 When using ``TelegaViewSet`` you most likely won't have to interact with the argument string directly, since
-how ``dispatch`` converts a string into arguments, and to create a string for a ``callback_data`` button for calling another method by user, you should use
+``dispatch`` converts a string into arguments. And for creating a ``callback_data`` button string, that the user can call another method from Telegram interface, you should use
 ``TelegaViewSet.gm_callback_data`` function. In case you need more low-level interaction with function arguments, then
 you can use the ``construct_utrl`` and ``get_utrl_params`` functions.
 
 After receiving the utrl_args arguments and checking access rights, the managing method (action) is directly selected and called.
 The first argument, which is the short name for the function, is popped from the utrl_args. All other arguments are passed as parameters
-into a function. Inside the function, the necessary business logic and the data formating for displaying to the user as a response take place.
+into a function. Inside the function, the necessary business logic and the data formatting for displaying to the user as a response take place.
 Any such managing function in the ``TelegaViewSet`` class must return the action type ``chat_action`` and the parameters to that action ``chat_action_args``.
-By default, the  class has only 1 action ﹣ ``CHAT_ACTION_MESSAGE``, which means that the user will receive
-a text message (possibly with buttons) as an answer for his/her action. The arguments to this action are the text of the message and a list of buttons (can be None).
+By default, the class has only 1 action ﹣ ``CHAT_ACTION_MESSAGE``, which means that the user will receive
+a text message (possibly with buttons) as an answer for his/her action. The arguments for this action are the text of the message and a list of buttons (can be None).
 
 
-After the function is processed, a response is sent to the user  by ``send_answer`` function and the user's action is logged.
+After the function is processed, a response is sent to the user by ``send_answer`` function and the user's action is logged.
 
 
 The methods to call in ``viewset_routing`` are the ``create, update, delete, show_elem, show_list`` methods.
 You can also add your own methods. Suppose we want to add a ``def super_method(self, *args)`` method, then
 you need to add the following lines in the class:
 
 .. code-block:: python
 
-    class SomeViewSetClass(TelegaViewSet):
+    class SomeViewSetClass(TelegramViewSet):
         ...
 
         actions = ['create', 'change', 'delete', 'show_elem', 'show_list', 'super_method']
 
         command_routing_super_method = 'sm'
 
 
@@ -547,45 +555,45 @@
 Where ``actions`` defines the list of available methods and ``command_routing_<method>`` defines the path (url; short name) of the method.
 
 As noted above, the ``dispatch`` method performs a permissions check by calling the ``has_permissions`` method.
 The check is performed by the classes specified in ``permission_classes`` and the default class is ``AllowAny``:
 
 .. code-block:: python
 
-    class TelegaViewSet:
+    class TelegramViewSet:
         permission_classes = [AllowAny]
 
 
 
-Additional TelegaViewSet Tools
+Additional TelegramViewSet Tools
 ************************************************
 
 This section describes the following class functionality that makes it easier to write code:
 
 1. External filters;
 2. Data display setting options;
 3. Helper functions for displaying data;
 4. Helper functions of business logic;
 
 
 External filters
 +++++++++++++++++++++
 
-Quite often, there is situation when you need to work not with all the elements of a database table, but with some
+Quite often, there is a situation when you need to work not with all the elements of a database table, but with some
 group (for example, a group of elements with a specific foreign key). For such purposes, you should use the ``foreign_filters`` list,
 which stores the values for filtering when the method is called. How exactly to use these filters is up to you, but
-usually it is good idea to use it in the ``get_queryset`` function. Thus, it is possible to pass to functions
+usually it is a good idea to use it in the ``get_queryset`` function. Thus, it is possible to pass to functions
 additional arguments that do not break the key logic of standard functions. Using the template example, you can modify
 ``BotMenuElemViewSet`` so that if an additional parameter is specified, then the BotMenuElem list displays
 only those elements that contain the specified parameter in their ``command`` attribute. To do this, you need to make the following changes to the code:
 
 
 .. code-block:: python
 
-    class BotMenuElemViewSet(TelegaViewSet):
+    class BotMenuElemViewSet(TelegramViewSet):
         ...
 
         foreign_filter_amount = 1
 
         def get_queryset(self):
             queryset = super().get_queryset()
             if self.foreign_filters[0]:
@@ -604,15 +612,15 @@
 This allows you to change the value of filters when generating paths.
 
 A more detailed use of external filters can be seen in the example of `Drive Bot <https://github.com/alexanderaleskin/drive_bot>`_ .
 
 Data display options
 ++++++++++++++++++++++++++++++++++++++++++
 
-The ``TelegaViewSet`` has the following options for displaying model elements:
+The ``TelegramViewSet`` has the following options for displaying model elements:
 
 * ``updating_fields: list`` - list of fields that can be changed (displayed when showing the element (``show_elem``);
 * ``show_cancel_updating_button: bool = True`` - shows a cancel button when changing fields, which leads back to the displaying element (``show_elem``);
 * ``deleting_with_confirm: bool = True`` - ask the user for confirmation when deleting an element;
 * ``cancel_adding_button: InlineKeyboardButtonDJ = None`` - cancel button when creating an element (``create`` method);
 * ``use_name_and_id_in_elem_showing: bool = True`` - enables the use of the name and ID of the element when displaying this element (methods ``show_list`` and ``show_elem``);
 * ``meta_texts_dict: dict`` - a dictionary that stores standard texts for display (texts are used in all methods).
@@ -642,17 +650,17 @@
 
 Depending on the need for customization, it is necessary to redefine these functions.
 
 
 Helper functions of business logic
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
-The ``TelegaViewSet`` class uses the following helper functions:
+The ``TelegramViewSet`` class uses the following helper functions:
 
-* ``def get_queryset`` - allows you to modify Model queries to database (most often used to filter elements, as in the example above);
+* ``def get_queryset`` - allows you to modify Model queries to the database (most often used to filter elements, as in the example above);
 * ``def create_or_update_helper`` - main logic for ``create`` and ``update`` methods;
 * ``def show_list_get_queryset`` - allows you to customize the selection of items to display in show_list;
 
 
 handler_decor
 ~~~~~~~~~~~~~~~~
 
@@ -674,46 +682,45 @@
 To support the use of different languages, the main elements of the Python-Telegram-Bot library are redefined in ``telegram_django_bot.telegram_lib_redefinition``:
 
 
 1. ``telegram.Bot`` -> ``telegram_django_bot.BotDJ`` ;
 2. ``telegram.ReplyMarkup`` -> ``telegram_django_bot.ReplyMarkupDJ`` ;
 3. ``telegram.KeyboardButton`` -> ``telegram_django_bot.KeyboardButtonDJ`` ;
 4. ``telegram.InlineKeyboardButton`` -> ``telegram_django_bot.InlineKeyboardButtonDJ`` ;
-5. ``telegram.InlineKeyboardMarkup`` -> ``telegram_django_bot.InlineKeyboardMarkupDJ``;
-
+5. ``telegram.InlineKeyboardMarkup`` -> ``telegram_django_bot.InlineKeyboardMarkupDJ``.
 
 
 When using these classes in code, multilingual support comes down to the following steps:
 
 1. Specifying the necessary settings in the settings.py file: ``LANGUAGES`` - list of languages, ``LANGUAGE_CODE`` - default language;
 1. Necessary texts for translation are wrapped in ``gettext`` and ``gettext_lazy`` from ``django.utils.translation`` (how it works in Django `read here <https://docs.djangoproject.com/en /4.1/topics/i18n/translation/#standard-translation>`_ )
 2. Run command ``$ django-admin makemessages -a`` to generate texts for translation (created in locale folder)
 3. Generation of translation files ``$ django-admin compilemessages``.
 
-Only a part of the functions uses localization in the template. It is made for easy understanding. Usage of localization can be seen in the example
+Only a part of the functions uses localization in the template. It is made for easy understanding. The usage of localization can be seen in the example
 functions ``some_debug_func``.
 
 
 Extra lib features
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 The library provides some additional tools for the convenience of developing and managing the bot.
 
 Модели библиотеки
 ************************************
 
 
-For the correct work of ``TelegaViewSet`` and other components the Django ORM model representing the user in the Telegram must be inherited
+For the correct work of ``TelegaViewSet`` and other components the Django ORM model representing the user in Telegram must be inherited
 from ``telegram_django_bot.models.TelegramUser``, as these components use its fields. ``TelegramUser`` inherited from
 ``django.contrib.auth.models.AbstractUser`` (which allows you to authorize users on the site if necessary) and has
 the following additional fields:
 
 * ``id`` - redefined to use user ID from telegrams;
 * ``seed_code`` - arbitrary value from 1 to 100 to randomly group users for tests and analysis;
-* ``telegram_username`` - username of the user in the telegram;
+* ``telegram_username`` - username of the user in telegram;
 * ``telegram_language_code`` - telegram language code (some languages have dialects and as a result the code designation is more than 2 symbols);
 * ``timezone`` - the user's time zone (for determining the time);
 * ``current_utrl`` - path (utrl) of the last user action (used in ``TelegaViewSet``);
 * ``current_utrl_code_dttm`` - time of the last action, when saving the path;
 * ``current_utrl_context_db`` - path context (utrl);
 * ``current_utrl_form_db`` - intermediate data for the form. Acts as a temporary data store when filling out a form;
 
@@ -724,15 +731,15 @@
 * ``current_utrl_context`` (property) - returns the current path context (utrl);
 * ``save_form_in_db`` - saves the form in the ``current_utrl_form_db`` field;
 * ``save_context_in_db`` - saves the context in the field ``current_utrl_context_db``;
 * ``clear_status`` - clears the data associated with the used path (fields ``current_utrl_<suffix>``) ;
 * ``language_code`` (property) - returns the language code in which messages should be generated for the user;
 
 
-Actually, if you want, you can create your self Django ORM model representing the user, you just need to copy
+If you want, you can create your self Django ORM model representing the user, you just need to copy
 ``id, telegram_username, telegram_language_code, current_utrl, current_utrl_code_dttm, current_utrl_context_db, current_utrl_form_db``
 and corresponding functions.
 
 
 The library also describes additional models to improve the usability of the bot:
 
 * ``ActionLog`` - stores user actions. Records help to collect analytics and make triggers that work on certain actions;
@@ -744,15 +751,15 @@
 
 
 Additional functions of TG_DJ_Bot
 *********************************************
 
 To improve convenience, ``TG_DJ_Bot`` has several high-level functions:
 
-* ``send_format_message`` - Allows you to send a message of an arbitrary type (internally, depending on the ``message_format`` selects the appropriate method of the ``Python-Telegram-Bot`` library). An important feature of this function is that if the user clicks on the button, then the previous message of the bot is changed, rather than a new one is sent. If, nevertheless, in this case you need to send a new message to the user, then you need to set the parameter ``only_send=True`` ;
+* ``send_format_message`` - Allows you to send a message of an arbitrary type (internally, depending on the ``message_format`` selects the appropriate method of the ``Python-Telegram-Bot`` library). An important feature of this function is that if the user clicks on the button, then the previous message of the bot is changed, rather than a new one being sent. If, nevertheless you need to send a new message to the user, then you need to set the parameter ``only_send=True`` ;
 * ``edit_or_send`` - wrapper of the ``send_format_message`` method for sending text messages with buttons;
 * ``send_botmenuelem`` - Sends a ``BotMenuElem`` to the user. The ``update`` argument can be empty;
 * ``task_send_message_handler`` - created for sending messages to many users. Handles situations where the user blocked the bot, deleted or when the limit for sending messages to users is reached;
 
 
 Utils
 **********
@@ -774,33 +781,31 @@
 Django. Also ``RouterCallbackMessageCommandHandler`` provides the ability to handle calls to ``BotMenuElem`` as
 through commands, and through callback. This is achieved by using the functions ``all_command_bme_handler`` and
 ``all_callback_bme_handler``. By default, ``BotMenuElem`` call handling is enabled and handled after
 no suitable path was found in the description of utrls (paths in Django notation). If there is no ``BotMenuElem`` element
 match is found, the ``BotMenuElem`` is considered to be configured incorrectly and an error message is returned to the user.
 You can create a class with the ``only_utrl=True`` attribute, what is disable calls to ``BotMenuElem``.
 
-The example template contains the use of the ``telega_reverse`` function, the essence of which is to generate a path (string) to
+The example template contains the use of the ``telega_reverse`` function, the essence of which is to generate a path (string) to the
 handler specified in the function argument. The function is analogous to the `reverse <https://docs.djangoproject.com/en/4.1/ref/urlresolvers/#reverse>`_ Django function
 and avoids errors when changing paths.
 
 
 
 Tests
 **********************
 
 The library also extends the ``django.test.TestCase`` capabilities for use with Telegram through the ``TD_TestCase`` class.
 
 The simplest approach for testing the bot is to generate messages that the bot expects from Telegram and
-sending a response to Telegram (to check that the bot's response messages are in the correct format). Class ``TD_TestCase``
+send a response to Telegram (to check that the bot's response messages are in the correct format). Class ``TD_TestCase``
 has a function ``create_update`` for easy and fast creation of ``Telegram.Update`` which generates the request
 telegram user. So the overall design looks like this:
 
 1. A ``Telegram.Update`` is created for emitting a user request;
-2. The ``handle_update`` lambda function, which uses ``RouterCallbackMessageCommandHandler``,  is called with created update. It does its staff and as a result sends a real message to the test user. Due to this, the correctness of the responsing data format  is checked by Telegram;
+2. The ``handle_update`` lambda function, which uses ``RouterCallbackMessageCommandHandler``,  is called with created update. It does its staff and as a result sends a real message to the test user. Due to this, the correctness of the response data format  is checked by Telegram;
 3. The correctness of the sent data and changes in the database is checked using the standard tools ``django.test.TestCase``.
 
 You need to specify at least one test user ID in the ``TELEGRAM_TEST_USER_IDS`` settings section for correct tests work.
 Messages will be sent to that user, so the bot needs to have permission to write to that user.
 
 In the ``tests`` folder you could find test examples.
-
-
```

### Comparing `telegram_django_bot-1.0.1/telegram_django_bot.egg-info/SOURCES.txt` & `telegram_django_bot-1.0.2/telegram_django_bot.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -30,8 +30,14 @@
 telegram_django_bot/migrations/0003_botmenuelem_message_format.py
 telegram_django_bot/migrations/0004_auto_20220915_0448.py
 telegram_django_bot/migrations/0005_auto_20221010_1330.py
 telegram_django_bot/migrations/0006_auto_20221023_0157.py
 telegram_django_bot/migrations/0007_auto_20221202_0305.py
 telegram_django_bot/migrations/0008_auto_20221225_1050.py
 telegram_django_bot/migrations/__init__.py
-telegram_django_bot/templates/dropdown_filter1.html
+telegram_django_bot/templates/dropdown_filter1.html
+tests/test_bme.py
+tests/test_routing.py
+tests/test_td_bot.py
+tests/test_user.py
+tests/test_utils.py
+tests/test_viewset.py
```

