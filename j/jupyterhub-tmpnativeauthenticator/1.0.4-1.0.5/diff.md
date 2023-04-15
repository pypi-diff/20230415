# Comparing `tmp/jupyterhub-tmpnativeauthenticator-1.0.4.tar.gz` & `tmp/jupyterhub-tmpnativeauthenticator-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-tmpnativeauthenticator-1.0.4.tar", last modified: Sat Apr 15 17:39:19 2023, max compression
+gzip compressed data, was "jupyterhub-tmpnativeauthenticator-1.0.5.tar", last modified: Sat Apr 15 17:43:16 2023, max compression
```

## Comparing `jupyterhub-tmpnativeauthenticator-1.0.4.tar` & `jupyterhub-tmpnativeauthenticator-1.0.5.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 17:39:19.327595 jupyterhub-tmpnativeauthenticator-1.0.4/
--rw-rw-rw-   0        0        0     1539 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      179 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2947 2023-04-15 17:39:19.326562 jupyterhub-tmpnativeauthenticator-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2607 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/README.md
--rw-rw-rw-   0        0        0       98 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/dev-requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 17:39:19.276568 jupyterhub-tmpnativeauthenticator-1.0.4/docs/
--rw-rw-rw-   0        0        0     1353 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/docs/Makefile
--rwxrwxrwx   0        0        0     1108 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/docs/make.bat
--rw-rw-rw-   0        0        0      321 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 17:39:19.282577 jupyterhub-tmpnativeauthenticator-1.0.4/docs/source/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:39:19.296586 jupyterhub-tmpnativeauthenticator-1.0.4/docs/source/_static/
--rw-rw-rw-   0        0        0    62232 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/docs/source/_static/authorization_area.png
--rw-rw-rw-   0        0        0  2487640 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/docs/source/_static/block_user_failed_logins.png
--rw-rw-rw-   0        0        0    59939 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/docs/source/_static/change_password_self.png
--rw-rw-rw-   0        0        0    52206 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/docs/source/_static/change_password_user.png
--rw-rw-rw-   0        0        0    85574 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/docs/source/_static/login-two-factor-auth.png
--rw-rw-rw-   0        0        0  1355938 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/docs/source/_static/native_auth_flow.png
--rw-rw-rw-   0        0        0    91790 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/docs/source/_static/signup-two-factor-auth.png
--rw-rw-rw-   0        0        0    78767 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/docs/source/_static/wrong_signup.png
--rw-rw-rw-   0        0        0     1939 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/docs/source/conf.py
--rw-rw-rw-   0        0        0     1127 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/docs/source/index.md
--rw-rw-rw-   0        0        0    10165 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/docs/source/options.md
--rw-rw-rw-   0        0        0     4435 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/docs/source/quickstart.md
--rw-rw-rw-   0        0        0     2033 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/docs/source/troubleshooting.md
-drwxrwxrwx   0        0        0        0 2023-04-15 17:39:19.302583 jupyterhub-tmpnativeauthenticator-1.0.4/jupyterhub_tmpnativeauthenticator.egg-info/
--rw-rw-rw-   0        0        0     2947 2023-04-15 17:39:19.000000 jupyterhub-tmpnativeauthenticator-1.0.4/jupyterhub_tmpnativeauthenticator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1659 2023-04-15 17:39:19.000000 jupyterhub-tmpnativeauthenticator-1.0.4/jupyterhub_tmpnativeauthenticator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 17:39:19.000000 jupyterhub-tmpnativeauthenticator-1.0.4/jupyterhub_tmpnativeauthenticator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-15 17:39:19.000000 jupyterhub-tmpnativeauthenticator-1.0.4/jupyterhub_tmpnativeauthenticator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-15 17:39:19.000000 jupyterhub-tmpnativeauthenticator-1.0.4/jupyterhub_tmpnativeauthenticator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 17:39:19.308562 jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/
--rw-rw-rw-   0        0        0      123 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/__init__.py
--rw-rw-rw-   0        0        0    86508 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/common-credentials.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 17:39:19.314562 jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/crypto/
--rw-rw-rw-   0        0        0        0 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/crypto/__init__.py
--rw-rw-rw-   0        0        0     2584 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/crypto/crypto.py
--rw-rw-rw-   0        0        0     6660 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/crypto/encoding.py
--rw-rw-rw-   0        0        0     7948 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/crypto/signing.py
--rw-rw-rw-   0        0        0    22111 2023-04-15 17:38:41.000000 jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/handlers.py
--rw-rw-rw-   0        0        0    16265 2023-04-15 17:38:41.000000 jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/nativeauthenticator.py
--rw-rw-rw-   0        0        0     4470 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/orm.py
-drwxrwxrwx   0        0        0        0 2023-04-15 17:39:19.321582 jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/templates/
--rw-rw-rw-   0        0        0     1915 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/templates/authorization-area.html
--rw-rw-rw-   0        0        0     2333 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/templates/change-password-admin.html
--rw-rw-rw-   0        0        0     2944 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/templates/change-password.html
--rw-rw-rw-   0        0        0      256 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/templates/my_message.html
--rw-rw-rw-   0        0        0     3207 2023-04-12 11:55:33.000000 jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/templates/native-login.html
--rw-rw-rw-   0        0        0      290 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/templates/page.html
--rw-rw-rw-   0        0        0     5008 2023-04-12 12:53:22.000000 jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/templates/signup.html
-drwxrwxrwx   0        0        0        0 2023-04-15 17:39:19.325562 jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/tests/
--rw-rw-rw-   0        0        0        0 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/tests/__init__.py
--rw-rw-rw-   0        0        0    12828 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/tests/test_authenticator.py
--rw-rw-rw-   0        0        0     1291 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/tests/test_orm.py
--rw-rw-rw-   0        0        0       42 2023-04-15 17:39:19.327595 jupyterhub-tmpnativeauthenticator-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      662 2023-04-15 17:39:16.000000 jupyterhub-tmpnativeauthenticator-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 17:43:16.752424 jupyterhub-tmpnativeauthenticator-1.0.5/
+-rw-rw-rw-   0        0        0     1539 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0      179 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2947 2023-04-15 17:43:16.752424 jupyterhub-tmpnativeauthenticator-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2607 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/README.md
+-rw-rw-rw-   0        0        0       98 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/dev-requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 17:43:16.701489 jupyterhub-tmpnativeauthenticator-1.0.5/docs/
+-rw-rw-rw-   0        0        0     1353 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/docs/Makefile
+-rwxrwxrwx   0        0        0     1108 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/docs/make.bat
+-rw-rw-rw-   0        0        0      321 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 17:43:16.706461 jupyterhub-tmpnativeauthenticator-1.0.5/docs/source/
+drwxrwxrwx   0        0        0        0 2023-04-15 17:43:16.721138 jupyterhub-tmpnativeauthenticator-1.0.5/docs/source/_static/
+-rw-rw-rw-   0        0        0    62232 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/docs/source/_static/authorization_area.png
+-rw-rw-rw-   0        0        0  2487640 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/docs/source/_static/block_user_failed_logins.png
+-rw-rw-rw-   0        0        0    59939 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/docs/source/_static/change_password_self.png
+-rw-rw-rw-   0        0        0    52206 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/docs/source/_static/change_password_user.png
+-rw-rw-rw-   0        0        0    85574 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/docs/source/_static/login-two-factor-auth.png
+-rw-rw-rw-   0        0        0  1355938 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/docs/source/_static/native_auth_flow.png
+-rw-rw-rw-   0        0        0    91790 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/docs/source/_static/signup-two-factor-auth.png
+-rw-rw-rw-   0        0        0    78767 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/docs/source/_static/wrong_signup.png
+-rw-rw-rw-   0        0        0     1939 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/docs/source/conf.py
+-rw-rw-rw-   0        0        0     1127 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/docs/source/index.md
+-rw-rw-rw-   0        0        0    10165 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/docs/source/options.md
+-rw-rw-rw-   0        0        0     4435 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/docs/source/quickstart.md
+-rw-rw-rw-   0        0        0     2033 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/docs/source/troubleshooting.md
+drwxrwxrwx   0        0        0        0 2023-04-15 17:43:16.728161 jupyterhub-tmpnativeauthenticator-1.0.5/jupyterhub_tmpnativeauthenticator.egg-info/
+-rw-rw-rw-   0        0        0     2947 2023-04-15 17:43:16.000000 jupyterhub-tmpnativeauthenticator-1.0.5/jupyterhub_tmpnativeauthenticator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1659 2023-04-15 17:43:16.000000 jupyterhub-tmpnativeauthenticator-1.0.5/jupyterhub_tmpnativeauthenticator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 17:43:16.000000 jupyterhub-tmpnativeauthenticator-1.0.5/jupyterhub_tmpnativeauthenticator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-04-15 17:43:16.000000 jupyterhub-tmpnativeauthenticator-1.0.5/jupyterhub_tmpnativeauthenticator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-15 17:43:16.000000 jupyterhub-tmpnativeauthenticator-1.0.5/jupyterhub_tmpnativeauthenticator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 17:43:16.735162 jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/
+-rw-rw-rw-   0        0        0      123 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/__init__.py
+-rw-rw-rw-   0        0        0    86508 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/common-credentials.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 17:43:16.739162 jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/crypto/
+-rw-rw-rw-   0        0        0        0 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/crypto/__init__.py
+-rw-rw-rw-   0        0        0     2584 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/crypto/crypto.py
+-rw-rw-rw-   0        0        0     6660 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/crypto/encoding.py
+-rw-rw-rw-   0        0        0     7948 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/crypto/signing.py
+-rw-rw-rw-   0        0        0    22125 2023-04-15 17:43:04.000000 jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/handlers.py
+-rw-rw-rw-   0        0        0    16265 2023-04-15 17:38:41.000000 jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/nativeauthenticator.py
+-rw-rw-rw-   0        0        0     4470 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/orm.py
+drwxrwxrwx   0        0        0        0 2023-04-15 17:43:16.748417 jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/templates/
+-rw-rw-rw-   0        0        0     1915 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/templates/authorization-area.html
+-rw-rw-rw-   0        0        0     2333 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/templates/change-password-admin.html
+-rw-rw-rw-   0        0        0     2944 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/templates/change-password.html
+-rw-rw-rw-   0        0        0      256 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/templates/my_message.html
+-rw-rw-rw-   0        0        0     3207 2023-04-12 11:55:33.000000 jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/templates/native-login.html
+-rw-rw-rw-   0        0        0      290 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/templates/page.html
+-rw-rw-rw-   0        0        0     5008 2023-04-12 12:53:22.000000 jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/templates/signup.html
+drwxrwxrwx   0        0        0        0 2023-04-15 17:43:16.750424 jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/tests/__init__.py
+-rw-rw-rw-   0        0        0    12828 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/tests/test_authenticator.py
+-rw-rw-rw-   0        0        0     1291 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/tests/test_orm.py
+-rw-rw-rw-   0        0        0       42 2023-04-15 17:43:16.753426 jupyterhub-tmpnativeauthenticator-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      662 2023-04-15 17:43:13.000000 jupyterhub-tmpnativeauthenticator-1.0.5/setup.py
```

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/LICENSE` & `jupyterhub-tmpnativeauthenticator-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/PKG-INFO` & `jupyterhub-tmpnativeauthenticator-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterhub-tmpnativeauthenticator
-Version: 1.0.4
+Version: 1.0.5
 Summary: JupyterHub Native Authenticator with tmp login
 Home-page: https://github.com/Gorbacheb/tmpnativeauthenticator
 Author: Vladimir Nedugov
 Author-email: MegaRs1@yandex.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/README.md` & `jupyterhub-tmpnativeauthenticator-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/docs/Makefile` & `jupyterhub-tmpnativeauthenticator-1.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/docs/make.bat` & `jupyterhub-tmpnativeauthenticator-1.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/docs/source/_static/authorization_area.png` & `jupyterhub-tmpnativeauthenticator-1.0.5/docs/source/_static/authorization_area.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/docs/source/_static/block_user_failed_logins.png` & `jupyterhub-tmpnativeauthenticator-1.0.5/docs/source/_static/block_user_failed_logins.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/docs/source/_static/change_password_self.png` & `jupyterhub-tmpnativeauthenticator-1.0.5/docs/source/_static/change_password_self.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/docs/source/_static/change_password_user.png` & `jupyterhub-tmpnativeauthenticator-1.0.5/docs/source/_static/change_password_user.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/docs/source/_static/login-two-factor-auth.png` & `jupyterhub-tmpnativeauthenticator-1.0.5/docs/source/_static/login-two-factor-auth.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/docs/source/_static/native_auth_flow.png` & `jupyterhub-tmpnativeauthenticator-1.0.5/docs/source/_static/native_auth_flow.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/docs/source/_static/signup-two-factor-auth.png` & `jupyterhub-tmpnativeauthenticator-1.0.5/docs/source/_static/signup-two-factor-auth.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/docs/source/_static/wrong_signup.png` & `jupyterhub-tmpnativeauthenticator-1.0.5/docs/source/_static/wrong_signup.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/docs/source/conf.py` & `jupyterhub-tmpnativeauthenticator-1.0.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/docs/source/index.md` & `jupyterhub-tmpnativeauthenticator-1.0.5/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/docs/source/options.md` & `jupyterhub-tmpnativeauthenticator-1.0.5/docs/source/options.md`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/docs/source/quickstart.md` & `jupyterhub-tmpnativeauthenticator-1.0.5/docs/source/quickstart.md`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/docs/source/troubleshooting.md` & `jupyterhub-tmpnativeauthenticator-1.0.5/docs/source/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/jupyterhub_tmpnativeauthenticator.egg-info/PKG-INFO` & `jupyterhub-tmpnativeauthenticator-1.0.5/jupyterhub_tmpnativeauthenticator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterhub-tmpnativeauthenticator
-Version: 1.0.4
+Version: 1.0.5
 Summary: JupyterHub Native Authenticator with tmp login
 Home-page: https://github.com/Gorbacheb/tmpnativeauthenticator
 Author: Vladimir Nedugov
 Author-email: MegaRs1@yandex.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/jupyterhub_tmpnativeauthenticator.egg-info/SOURCES.txt` & `jupyterhub-tmpnativeauthenticator-1.0.5/jupyterhub_tmpnativeauthenticator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/common-credentials.txt` & `jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/common-credentials.txt`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/crypto/crypto.py` & `jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/crypto/encoding.py` & `jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/crypto/encoding.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/crypto/signing.py` & `jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/crypto/signing.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/handlers.py` & `jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -548,16 +548,16 @@
         self.force_new_server = force_new_server
         self.process_user = process_user
 
     @gen.coroutine
     def get(self):
         raw_user = yield self.get_current_user()
 
-        for user_name, user in self.users.items():
-            if (datetime.utcnow() - user.last_activity).total_seconds() >= self.tmp_user_lifetime:
+        for user_name in self.users.keys():
+            if (datetime.utcnow() - self.users.get(user_name).last_activity).total_seconds() >= self.tmp_user_lifetime:
                 self.users.delete(user_name)
 
         if raw_user:
             if self.force_new_server and raw_user.running:
                 # Stop user's current server if it is running
                 # so we get a new one.
                 status = yield raw_user.spawner.poll_and_notify()
```

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/nativeauthenticator.py` & `jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/nativeauthenticator.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/orm.py` & `jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/orm.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/templates/authorization-area.html` & `jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/templates/authorization-area.html`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/templates/change-password-admin.html` & `jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/templates/change-password-admin.html`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/templates/change-password.html` & `jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/templates/change-password.html`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/templates/native-login.html` & `jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/templates/native-login.html`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/templates/signup.html` & `jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/templates/signup.html`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/tests/test_authenticator.py` & `jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/tests/test_authenticator.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/nativeauthenticator/tests/test_orm.py` & `jupyterhub-tmpnativeauthenticator-1.0.5/nativeauthenticator/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.4/setup.py` & `jupyterhub-tmpnativeauthenticator-1.0.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setup(
     name="jupyterhub-tmpnativeauthenticator",
-    version="1.0.4",
+    version="1.0.5",
     description="JupyterHub Native Authenticator with tmp login",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Gorbacheb/tmpnativeauthenticator",
     author="Vladimir Nedugov",
     author_email="MegaRs1@yandex.ru",
     license="MIT",
```

