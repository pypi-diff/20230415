# Comparing `tmp/jupyterhub-tmpnativeauthenticator-1.0.1.tar.gz` & `tmp/jupyterhub-tmpnativeauthenticator-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-tmpnativeauthenticator-1.0.1.tar", last modified: Wed Apr 12 12:10:00 2023, max compression
+gzip compressed data, was "jupyterhub-tmpnativeauthenticator-1.0.2.tar", last modified: Sat Apr 15 17:27:23 2023, max compression
```

## Comparing `jupyterhub-tmpnativeauthenticator-1.0.1.tar` & `jupyterhub-tmpnativeauthenticator-1.0.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 12:10:00.568853 jupyterhub-tmpnativeauthenticator-1.0.1/
--rw-rw-rw-   0        0        0     1539 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      179 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2947 2023-04-12 12:10:00.567844 jupyterhub-tmpnativeauthenticator-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2607 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/README.md
--rw-rw-rw-   0        0        0       98 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/dev-requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 12:10:00.520829 jupyterhub-tmpnativeauthenticator-1.0.1/docs/
--rw-rw-rw-   0        0        0     1353 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/docs/Makefile
--rwxrwxrwx   0        0        0     1108 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/docs/make.bat
--rw-rw-rw-   0        0        0      321 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 12:10:00.526830 jupyterhub-tmpnativeauthenticator-1.0.1/docs/source/
-drwxrwxrwx   0        0        0        0 2023-04-12 12:10:00.539845 jupyterhub-tmpnativeauthenticator-1.0.1/docs/source/_static/
--rw-rw-rw-   0        0        0    62232 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/docs/source/_static/authorization_area.png
--rw-rw-rw-   0        0        0  2487640 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/docs/source/_static/block_user_failed_logins.png
--rw-rw-rw-   0        0        0    59939 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/docs/source/_static/change_password_self.png
--rw-rw-rw-   0        0        0    52206 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/docs/source/_static/change_password_user.png
--rw-rw-rw-   0        0        0    85574 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/docs/source/_static/login-two-factor-auth.png
--rw-rw-rw-   0        0        0  1355938 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/docs/source/_static/native_auth_flow.png
--rw-rw-rw-   0        0        0    91790 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/docs/source/_static/signup-two-factor-auth.png
--rw-rw-rw-   0        0        0    78767 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/docs/source/_static/wrong_signup.png
--rw-rw-rw-   0        0        0     1939 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/docs/source/conf.py
--rw-rw-rw-   0        0        0     1127 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/docs/source/index.md
--rw-rw-rw-   0        0        0    10165 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/docs/source/options.md
--rw-rw-rw-   0        0        0     4435 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/docs/source/quickstart.md
--rw-rw-rw-   0        0        0     2033 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/docs/source/troubleshooting.md
-drwxrwxrwx   0        0        0        0 2023-04-12 12:10:00.547852 jupyterhub-tmpnativeauthenticator-1.0.1/jupyterhub_tmpnativeauthenticator.egg-info/
--rw-rw-rw-   0        0        0     2947 2023-04-12 12:10:00.000000 jupyterhub-tmpnativeauthenticator-1.0.1/jupyterhub_tmpnativeauthenticator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1659 2023-04-12 12:10:00.000000 jupyterhub-tmpnativeauthenticator-1.0.1/jupyterhub_tmpnativeauthenticator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 12:10:00.000000 jupyterhub-tmpnativeauthenticator-1.0.1/jupyterhub_tmpnativeauthenticator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-12 12:10:00.000000 jupyterhub-tmpnativeauthenticator-1.0.1/jupyterhub_tmpnativeauthenticator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-12 12:10:00.000000 jupyterhub-tmpnativeauthenticator-1.0.1/jupyterhub_tmpnativeauthenticator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 12:10:00.552832 jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/
--rw-rw-rw-   0        0        0      123 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/__init__.py
--rw-rw-rw-   0        0        0    86508 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/common-credentials.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 12:10:00.556829 jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/crypto/
--rw-rw-rw-   0        0        0        0 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/crypto/__init__.py
--rw-rw-rw-   0        0        0     2584 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/crypto/crypto.py
--rw-rw-rw-   0        0        0     6660 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/crypto/encoding.py
--rw-rw-rw-   0        0        0     7948 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/crypto/signing.py
--rw-rw-rw-   0        0        0    21875 2023-04-12 11:16:29.000000 jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/handlers.py
--rw-rw-rw-   0        0        0    16034 2023-04-12 11:56:46.000000 jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/nativeauthenticator.py
--rw-rw-rw-   0        0        0     4470 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/orm.py
-drwxrwxrwx   0        0        0        0 2023-04-12 12:10:00.564831 jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/templates/
--rw-rw-rw-   0        0        0     1915 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/templates/authorization-area.html
--rw-rw-rw-   0        0        0     2333 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/templates/change-password-admin.html
--rw-rw-rw-   0        0        0     2944 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/templates/change-password.html
--rw-rw-rw-   0        0        0      256 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/templates/my_message.html
--rw-rw-rw-   0        0        0     3207 2023-04-12 11:55:33.000000 jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/templates/native-login.html
--rw-rw-rw-   0        0        0      290 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/templates/page.html
--rw-rw-rw-   0        0        0     5008 2023-04-12 11:19:31.000000 jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/templates/signup.html
-drwxrwxrwx   0        0        0        0 2023-04-12 12:10:00.566829 jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/tests/
--rw-rw-rw-   0        0        0        0 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/tests/__init__.py
--rw-rw-rw-   0        0        0    12828 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/tests/test_authenticator.py
--rw-rw-rw-   0        0        0     1291 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/tests/test_orm.py
--rw-rw-rw-   0        0        0       42 2023-04-12 12:10:00.568853 jupyterhub-tmpnativeauthenticator-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      662 2023-04-12 12:09:49.000000 jupyterhub-tmpnativeauthenticator-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 17:27:22.999607 jupyterhub-tmpnativeauthenticator-1.0.2/
+-rw-rw-rw-   0        0        0     1539 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      179 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2947 2023-04-15 17:27:22.998609 jupyterhub-tmpnativeauthenticator-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2607 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/README.md
+-rw-rw-rw-   0        0        0       98 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/dev-requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 17:27:22.953606 jupyterhub-tmpnativeauthenticator-1.0.2/docs/
+-rw-rw-rw-   0        0        0     1353 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/docs/Makefile
+-rwxrwxrwx   0        0        0     1108 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/docs/make.bat
+-rw-rw-rw-   0        0        0      321 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 17:27:22.958626 jupyterhub-tmpnativeauthenticator-1.0.2/docs/source/
+drwxrwxrwx   0        0        0        0 2023-04-15 17:27:22.970605 jupyterhub-tmpnativeauthenticator-1.0.2/docs/source/_static/
+-rw-rw-rw-   0        0        0    62232 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/docs/source/_static/authorization_area.png
+-rw-rw-rw-   0        0        0  2487640 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/docs/source/_static/block_user_failed_logins.png
+-rw-rw-rw-   0        0        0    59939 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/docs/source/_static/change_password_self.png
+-rw-rw-rw-   0        0        0    52206 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/docs/source/_static/change_password_user.png
+-rw-rw-rw-   0        0        0    85574 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/docs/source/_static/login-two-factor-auth.png
+-rw-rw-rw-   0        0        0  1355938 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/docs/source/_static/native_auth_flow.png
+-rw-rw-rw-   0        0        0    91790 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/docs/source/_static/signup-two-factor-auth.png
+-rw-rw-rw-   0        0        0    78767 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/docs/source/_static/wrong_signup.png
+-rw-rw-rw-   0        0        0     1939 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/docs/source/conf.py
+-rw-rw-rw-   0        0        0     1127 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/docs/source/index.md
+-rw-rw-rw-   0        0        0    10165 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/docs/source/options.md
+-rw-rw-rw-   0        0        0     4435 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/docs/source/quickstart.md
+-rw-rw-rw-   0        0        0     2033 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/docs/source/troubleshooting.md
+drwxrwxrwx   0        0        0        0 2023-04-15 17:27:22.976619 jupyterhub-tmpnativeauthenticator-1.0.2/jupyterhub_tmpnativeauthenticator.egg-info/
+-rw-rw-rw-   0        0        0     2947 2023-04-15 17:27:22.000000 jupyterhub-tmpnativeauthenticator-1.0.2/jupyterhub_tmpnativeauthenticator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1659 2023-04-15 17:27:22.000000 jupyterhub-tmpnativeauthenticator-1.0.2/jupyterhub_tmpnativeauthenticator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 17:27:22.000000 jupyterhub-tmpnativeauthenticator-1.0.2/jupyterhub_tmpnativeauthenticator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-04-15 17:27:22.000000 jupyterhub-tmpnativeauthenticator-1.0.2/jupyterhub_tmpnativeauthenticator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-15 17:27:22.000000 jupyterhub-tmpnativeauthenticator-1.0.2/jupyterhub_tmpnativeauthenticator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 17:27:22.983606 jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/
+-rw-rw-rw-   0        0        0      123 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/__init__.py
+-rw-rw-rw-   0        0        0    86508 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/common-credentials.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 17:27:22.987607 jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/crypto/
+-rw-rw-rw-   0        0        0        0 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/crypto/__init__.py
+-rw-rw-rw-   0        0        0     2584 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/crypto/crypto.py
+-rw-rw-rw-   0        0        0     6660 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/crypto/encoding.py
+-rw-rw-rw-   0        0        0     7948 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/crypto/signing.py
+-rw-rw-rw-   0        0        0    22092 2023-04-15 17:26:54.000000 jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/handlers.py
+-rw-rw-rw-   0        0        0    16264 2023-04-15 17:26:54.000000 jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/nativeauthenticator.py
+-rw-rw-rw-   0        0        0     4470 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/orm.py
+drwxrwxrwx   0        0        0        0 2023-04-15 17:27:22.995608 jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/templates/
+-rw-rw-rw-   0        0        0     1915 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/templates/authorization-area.html
+-rw-rw-rw-   0        0        0     2333 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/templates/change-password-admin.html
+-rw-rw-rw-   0        0        0     2944 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/templates/change-password.html
+-rw-rw-rw-   0        0        0      256 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/templates/my_message.html
+-rw-rw-rw-   0        0        0     3207 2023-04-12 11:55:33.000000 jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/templates/native-login.html
+-rw-rw-rw-   0        0        0      290 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/templates/page.html
+-rw-rw-rw-   0        0        0     5008 2023-04-12 12:53:22.000000 jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/templates/signup.html
+drwxrwxrwx   0        0        0        0 2023-04-15 17:27:22.998609 jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/tests/__init__.py
+-rw-rw-rw-   0        0        0    12828 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/tests/test_authenticator.py
+-rw-rw-rw-   0        0        0     1291 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/tests/test_orm.py
+-rw-rw-rw-   0        0        0       42 2023-04-15 17:27:22.999607 jupyterhub-tmpnativeauthenticator-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      662 2023-04-15 17:27:20.000000 jupyterhub-tmpnativeauthenticator-1.0.2/setup.py
```

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/LICENSE` & `jupyterhub-tmpnativeauthenticator-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/PKG-INFO` & `jupyterhub-tmpnativeauthenticator-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterhub-tmpnativeauthenticator
-Version: 1.0.1
+Version: 1.0.2
 Summary: JupyterHub Native Authenticator with tmp login
 Home-page: https://github.com/Gorbacheb/tmpnativeauthenticator
 Author: Vladimir Nedugov
 Author-email: MegaRs1@yandex.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/README.md` & `jupyterhub-tmpnativeauthenticator-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/docs/Makefile` & `jupyterhub-tmpnativeauthenticator-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/docs/make.bat` & `jupyterhub-tmpnativeauthenticator-1.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/docs/source/_static/authorization_area.png` & `jupyterhub-tmpnativeauthenticator-1.0.2/docs/source/_static/authorization_area.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/docs/source/_static/block_user_failed_logins.png` & `jupyterhub-tmpnativeauthenticator-1.0.2/docs/source/_static/block_user_failed_logins.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/docs/source/_static/change_password_self.png` & `jupyterhub-tmpnativeauthenticator-1.0.2/docs/source/_static/change_password_self.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/docs/source/_static/change_password_user.png` & `jupyterhub-tmpnativeauthenticator-1.0.2/docs/source/_static/change_password_user.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/docs/source/_static/login-two-factor-auth.png` & `jupyterhub-tmpnativeauthenticator-1.0.2/docs/source/_static/login-two-factor-auth.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/docs/source/_static/native_auth_flow.png` & `jupyterhub-tmpnativeauthenticator-1.0.2/docs/source/_static/native_auth_flow.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/docs/source/_static/signup-two-factor-auth.png` & `jupyterhub-tmpnativeauthenticator-1.0.2/docs/source/_static/signup-two-factor-auth.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/docs/source/_static/wrong_signup.png` & `jupyterhub-tmpnativeauthenticator-1.0.2/docs/source/_static/wrong_signup.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/docs/source/conf.py` & `jupyterhub-tmpnativeauthenticator-1.0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/docs/source/index.md` & `jupyterhub-tmpnativeauthenticator-1.0.2/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/docs/source/options.md` & `jupyterhub-tmpnativeauthenticator-1.0.2/docs/source/options.md`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/docs/source/quickstart.md` & `jupyterhub-tmpnativeauthenticator-1.0.2/docs/source/quickstart.md`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/docs/source/troubleshooting.md` & `jupyterhub-tmpnativeauthenticator-1.0.2/docs/source/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/jupyterhub_tmpnativeauthenticator.egg-info/PKG-INFO` & `jupyterhub-tmpnativeauthenticator-1.0.2/jupyterhub_tmpnativeauthenticator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterhub-tmpnativeauthenticator
-Version: 1.0.1
+Version: 1.0.2
 Summary: JupyterHub Native Authenticator with tmp login
 Home-page: https://github.com/Gorbacheb/tmpnativeauthenticator
 Author: Vladimir Nedugov
 Author-email: MegaRs1@yandex.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/jupyterhub_tmpnativeauthenticator.egg-info/SOURCES.txt` & `jupyterhub-tmpnativeauthenticator-1.0.2/jupyterhub_tmpnativeauthenticator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/common-credentials.txt` & `jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/common-credentials.txt`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/crypto/crypto.py` & `jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/crypto/encoding.py` & `jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/crypto/encoding.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/crypto/signing.py` & `jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/crypto/signing.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/handlers.py` & `jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-import os
+import os, uuid
 from datetime import date
 from datetime import datetime
 from datetime import timezone as tz
 
 from jinja2 import ChoiceLoader
 from jinja2 import FileSystemLoader
 from jupyterhub.handlers import BaseHandler
 from jupyterhub.handlers.login import LoginHandler
 
-import uuid
-
-from traitlets import Bool
 from tornado import gen
 
 try:
     from jupyterhub.scopes import needs_scope
 
     admin_users_scope = needs_scope("admin:users")
 except ImportError:
@@ -541,22 +538,28 @@
 
 
 class NoPassAuthenticateHandler(BaseHandler):
     """
     Responsible for /nopasslogin
     Creates a new user with a random UUID, and auto starts their server
     """
-    def initialize(self, force_new_server, process_user):
+    def initialize(self, tmp_user_lifetime, force_new_server, process_user):
         super().initialize()
+        self.tmp_user_lifetime = tmp_user_lifetime
         self.force_new_server = force_new_server
         self.process_user = process_user
 
     @gen.coroutine
     def get(self):
         raw_user = yield self.get_current_user()
+
+        for user_name, user in self.users:
+            if (datetime.utcnow() - user.last_activity).days >= self.tmp_user_lifetime:
+                self.users.delete(user_name)
+
         if raw_user:
             if self.force_new_server and raw_user.running:
                 # Stop user's current server if it is running
                 # so we get a new one.
                 status = yield raw_user.spawner.poll_and_notify()
                 if status is None:
                     yield self.stop_single_user(raw_user)
```

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/nativeauthenticator.py` & `jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/nativeauthenticator.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,18 +177,26 @@
         When set to True, users going to /hub/nopasslogin will *always* get a
         new single-user server. When set to False, they'll be
         redirected to their current session if one exists.
         """,
         config=True
     )
 
+    tmp_user_lifetime = Integer(
+        1,
+        help="""
+        number of hours when temporary user will alive.
+        """,
+        config=True
+    )
+
     def process_user(self, user, handler):
         """
         Do additional arbitrary things to the created user before spawn.
-        user is a user object, and handler is a TmpAuthenticateHandler object
+        user is a user object, and handler is a NoPassAuthenticateHandler object
         Should return the new user object.
         This method can be a @tornado.gen.coroutine.
         Note: This is primarily for overriding in subclasses
         """
         return user
 
     def __init__(self, add_new_table=True, *args, **kwargs):
@@ -425,14 +433,15 @@
             (r"/authorize", AuthorizationAreaHandler),
             (r"/authorize/([^/]*)", ToggleAuthorizationHandler),
             # the following /confirm/ must be like in generate_approval_url()
             (r"/confirm/([^/]*)", EmailAuthorizationHandler),
             (r"/change-password", ChangePasswordHandler),
             (r"/change-password/([^/]+)", ChangePasswordAdminHandler),
             (r"/nopass-auth", NoPassAuthenticateHandler, {
+                'tmp_user_lifetime': self.tmp_user_lifetime,
                 'force_new_server': self.force_new_server,
                 'process_user': self.process_user
             }),
         ]
         return native_handlers
 
     def delete_user(self, user):
```

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/orm.py` & `jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/orm.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/templates/authorization-area.html` & `jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/templates/authorization-area.html`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/templates/change-password-admin.html` & `jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/templates/change-password-admin.html`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/templates/change-password.html` & `jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/templates/change-password.html`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/templates/native-login.html` & `jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/templates/native-login.html`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/templates/signup.html` & `jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/templates/signup.html`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/tests/test_authenticator.py` & `jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/tests/test_authenticator.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/nativeauthenticator/tests/test_orm.py` & `jupyterhub-tmpnativeauthenticator-1.0.2/nativeauthenticator/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.1/setup.py` & `jupyterhub-tmpnativeauthenticator-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setup(
     name="jupyterhub-tmpnativeauthenticator",
-    version="1.0.1",
+    version="1.0.2",
     description="JupyterHub Native Authenticator with tmp login",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Gorbacheb/tmpnativeauthenticator",
     author="Vladimir Nedugov",
     author_email="MegaRs1@yandex.ru",
     license="MIT",
```

