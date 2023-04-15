# Comparing `tmp/jupyterhub-tmpnativeauthenticator-1.0.7.tar.gz` & `tmp/jupyterhub-tmpnativeauthenticator-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-tmpnativeauthenticator-1.0.7.tar", last modified: Sat Apr 15 17:49:29 2023, max compression
+gzip compressed data, was "jupyterhub-tmpnativeauthenticator-1.0.8.tar", last modified: Sat Apr 15 18:00:06 2023, max compression
```

## Comparing `jupyterhub-tmpnativeauthenticator-1.0.7.tar` & `jupyterhub-tmpnativeauthenticator-1.0.8.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 17:49:29.545765 jupyterhub-tmpnativeauthenticator-1.0.7/
--rw-rw-rw-   0        0        0     1539 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/LICENSE
--rw-rw-rw-   0        0        0      179 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2947 2023-04-15 17:49:29.544703 jupyterhub-tmpnativeauthenticator-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2607 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/README.md
--rw-rw-rw-   0        0        0       98 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/dev-requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 17:49:29.490738 jupyterhub-tmpnativeauthenticator-1.0.7/docs/
--rw-rw-rw-   0        0        0     1353 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/Makefile
--rwxrwxrwx   0        0        0     1108 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/make.bat
--rw-rw-rw-   0        0        0      321 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 17:49:29.496702 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:49:29.511703 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/
--rw-rw-rw-   0        0        0    62232 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/authorization_area.png
--rw-rw-rw-   0        0        0  2487640 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/block_user_failed_logins.png
--rw-rw-rw-   0        0        0    59939 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/change_password_self.png
--rw-rw-rw-   0        0        0    52206 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/change_password_user.png
--rw-rw-rw-   0        0        0    85574 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/login-two-factor-auth.png
--rw-rw-rw-   0        0        0  1355938 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/native_auth_flow.png
--rw-rw-rw-   0        0        0    91790 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/signup-two-factor-auth.png
--rw-rw-rw-   0        0        0    78767 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/wrong_signup.png
--rw-rw-rw-   0        0        0     1939 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/conf.py
--rw-rw-rw-   0        0        0     1127 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/index.md
--rw-rw-rw-   0        0        0    10165 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/options.md
--rw-rw-rw-   0        0        0     4435 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/quickstart.md
--rw-rw-rw-   0        0        0     2033 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/troubleshooting.md
-drwxrwxrwx   0        0        0        0 2023-04-15 17:49:29.517727 jupyterhub-tmpnativeauthenticator-1.0.7/jupyterhub_tmpnativeauthenticator.egg-info/
--rw-rw-rw-   0        0        0     2947 2023-04-15 17:49:29.000000 jupyterhub-tmpnativeauthenticator-1.0.7/jupyterhub_tmpnativeauthenticator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1659 2023-04-15 17:49:29.000000 jupyterhub-tmpnativeauthenticator-1.0.7/jupyterhub_tmpnativeauthenticator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 17:49:29.000000 jupyterhub-tmpnativeauthenticator-1.0.7/jupyterhub_tmpnativeauthenticator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-15 17:49:29.000000 jupyterhub-tmpnativeauthenticator-1.0.7/jupyterhub_tmpnativeauthenticator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-15 17:49:29.000000 jupyterhub-tmpnativeauthenticator-1.0.7/jupyterhub_tmpnativeauthenticator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 17:49:29.525704 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/
--rw-rw-rw-   0        0        0      123 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/__init__.py
--rw-rw-rw-   0        0        0    86508 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/common-credentials.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 17:49:29.531702 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/crypto/
--rw-rw-rw-   0        0        0        0 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/crypto/__init__.py
--rw-rw-rw-   0        0        0     2584 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/crypto/crypto.py
--rw-rw-rw-   0        0        0     6660 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/crypto/encoding.py
--rw-rw-rw-   0        0        0     7948 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/crypto/signing.py
--rw-rw-rw-   0        0        0    22117 2023-04-15 17:49:14.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/handlers.py
--rw-rw-rw-   0        0        0    16265 2023-04-15 17:38:41.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/nativeauthenticator.py
--rw-rw-rw-   0        0        0     4470 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/orm.py
-drwxrwxrwx   0        0        0        0 2023-04-15 17:49:29.539727 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/templates/
--rw-rw-rw-   0        0        0     1915 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/templates/authorization-area.html
--rw-rw-rw-   0        0        0     2333 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/templates/change-password-admin.html
--rw-rw-rw-   0        0        0     2944 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/templates/change-password.html
--rw-rw-rw-   0        0        0      256 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/templates/my_message.html
--rw-rw-rw-   0        0        0     3207 2023-04-12 11:55:33.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/templates/native-login.html
--rw-rw-rw-   0        0        0      290 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/templates/page.html
--rw-rw-rw-   0        0        0     5008 2023-04-12 12:53:22.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/templates/signup.html
-drwxrwxrwx   0        0        0        0 2023-04-15 17:49:29.543703 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/tests/
--rw-rw-rw-   0        0        0        0 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/tests/__init__.py
--rw-rw-rw-   0        0        0    12828 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/tests/test_authenticator.py
--rw-rw-rw-   0        0        0     1291 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/tests/test_orm.py
--rw-rw-rw-   0        0        0       42 2023-04-15 17:49:29.545765 jupyterhub-tmpnativeauthenticator-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      662 2023-04-15 17:49:26.000000 jupyterhub-tmpnativeauthenticator-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:00:06.216932 jupyterhub-tmpnativeauthenticator-1.0.8/
+-rw-rw-rw-   0        0        0     1539 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0      179 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     2947 2023-04-15 18:00:06.216932 jupyterhub-tmpnativeauthenticator-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2607 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/README.md
+-rw-rw-rw-   0        0        0       98 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/dev-requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 18:00:06.170936 jupyterhub-tmpnativeauthenticator-1.0.8/docs/
+-rw-rw-rw-   0        0        0     1353 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/docs/Makefile
+-rwxrwxrwx   0        0        0     1108 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/docs/make.bat
+-rw-rw-rw-   0        0        0      321 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 18:00:06.175936 jupyterhub-tmpnativeauthenticator-1.0.8/docs/source/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:00:06.189938 jupyterhub-tmpnativeauthenticator-1.0.8/docs/source/_static/
+-rw-rw-rw-   0        0        0    62232 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/docs/source/_static/authorization_area.png
+-rw-rw-rw-   0        0        0  2487640 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/docs/source/_static/block_user_failed_logins.png
+-rw-rw-rw-   0        0        0    59939 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/docs/source/_static/change_password_self.png
+-rw-rw-rw-   0        0        0    52206 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/docs/source/_static/change_password_user.png
+-rw-rw-rw-   0        0        0    85574 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/docs/source/_static/login-two-factor-auth.png
+-rw-rw-rw-   0        0        0  1355938 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/docs/source/_static/native_auth_flow.png
+-rw-rw-rw-   0        0        0    91790 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/docs/source/_static/signup-two-factor-auth.png
+-rw-rw-rw-   0        0        0    78767 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/docs/source/_static/wrong_signup.png
+-rw-rw-rw-   0        0        0     1939 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/docs/source/conf.py
+-rw-rw-rw-   0        0        0     1127 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/docs/source/index.md
+-rw-rw-rw-   0        0        0    10165 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/docs/source/options.md
+-rw-rw-rw-   0        0        0     4435 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/docs/source/quickstart.md
+-rw-rw-rw-   0        0        0     2033 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/docs/source/troubleshooting.md
+drwxrwxrwx   0        0        0        0 2023-04-15 18:00:06.195992 jupyterhub-tmpnativeauthenticator-1.0.8/jupyterhub_tmpnativeauthenticator.egg-info/
+-rw-rw-rw-   0        0        0     2947 2023-04-15 18:00:06.000000 jupyterhub-tmpnativeauthenticator-1.0.8/jupyterhub_tmpnativeauthenticator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1659 2023-04-15 18:00:06.000000 jupyterhub-tmpnativeauthenticator-1.0.8/jupyterhub_tmpnativeauthenticator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 18:00:06.000000 jupyterhub-tmpnativeauthenticator-1.0.8/jupyterhub_tmpnativeauthenticator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-04-15 18:00:06.000000 jupyterhub-tmpnativeauthenticator-1.0.8/jupyterhub_tmpnativeauthenticator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:00:06.000000 jupyterhub-tmpnativeauthenticator-1.0.8/jupyterhub_tmpnativeauthenticator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 18:00:06.200943 jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/
+-rw-rw-rw-   0        0        0      123 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/__init__.py
+-rw-rw-rw-   0        0        0    86508 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/common-credentials.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 18:00:06.204936 jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/crypto/
+-rw-rw-rw-   0        0        0        0 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/crypto/__init__.py
+-rw-rw-rw-   0        0        0     2584 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/crypto/crypto.py
+-rw-rw-rw-   0        0        0     6660 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/crypto/encoding.py
+-rw-rw-rw-   0        0        0     7948 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/crypto/signing.py
+-rw-rw-rw-   0        0        0    22236 2023-04-15 17:59:01.000000 jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/handlers.py
+-rw-rw-rw-   0        0        0    16271 2023-04-15 17:59:47.000000 jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/nativeauthenticator.py
+-rw-rw-rw-   0        0        0     4470 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/orm.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:00:06.212927 jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/templates/
+-rw-rw-rw-   0        0        0     1915 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/templates/authorization-area.html
+-rw-rw-rw-   0        0        0     2333 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/templates/change-password-admin.html
+-rw-rw-rw-   0        0        0     2944 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/templates/change-password.html
+-rw-rw-rw-   0        0        0      256 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/templates/my_message.html
+-rw-rw-rw-   0        0        0     3207 2023-04-12 11:55:33.000000 jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/templates/native-login.html
+-rw-rw-rw-   0        0        0      290 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/templates/page.html
+-rw-rw-rw-   0        0        0     5008 2023-04-12 12:53:22.000000 jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/templates/signup.html
+drwxrwxrwx   0        0        0        0 2023-04-15 18:00:06.214926 jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/tests/__init__.py
+-rw-rw-rw-   0        0        0    12828 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/tests/test_authenticator.py
+-rw-rw-rw-   0        0        0     1291 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/tests/test_orm.py
+-rw-rw-rw-   0        0        0       42 2023-04-15 18:00:06.216932 jupyterhub-tmpnativeauthenticator-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      662 2023-04-15 18:00:03.000000 jupyterhub-tmpnativeauthenticator-1.0.8/setup.py
```

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/LICENSE` & `jupyterhub-tmpnativeauthenticator-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/PKG-INFO` & `jupyterhub-tmpnativeauthenticator-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterhub-tmpnativeauthenticator
-Version: 1.0.7
+Version: 1.0.8
 Summary: JupyterHub Native Authenticator with tmp login
 Home-page: https://github.com/Gorbacheb/tmpnativeauthenticator
 Author: Vladimir Nedugov
 Author-email: MegaRs1@yandex.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/README.md` & `jupyterhub-tmpnativeauthenticator-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/docs/Makefile` & `jupyterhub-tmpnativeauthenticator-1.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/docs/make.bat` & `jupyterhub-tmpnativeauthenticator-1.0.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/authorization_area.png` & `jupyterhub-tmpnativeauthenticator-1.0.8/docs/source/_static/authorization_area.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/block_user_failed_logins.png` & `jupyterhub-tmpnativeauthenticator-1.0.8/docs/source/_static/block_user_failed_logins.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/change_password_self.png` & `jupyterhub-tmpnativeauthenticator-1.0.8/docs/source/_static/change_password_self.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/change_password_user.png` & `jupyterhub-tmpnativeauthenticator-1.0.8/docs/source/_static/change_password_user.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/login-two-factor-auth.png` & `jupyterhub-tmpnativeauthenticator-1.0.8/docs/source/_static/login-two-factor-auth.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/native_auth_flow.png` & `jupyterhub-tmpnativeauthenticator-1.0.8/docs/source/_static/native_auth_flow.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/signup-two-factor-auth.png` & `jupyterhub-tmpnativeauthenticator-1.0.8/docs/source/_static/signup-two-factor-auth.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/wrong_signup.png` & `jupyterhub-tmpnativeauthenticator-1.0.8/docs/source/_static/wrong_signup.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/conf.py` & `jupyterhub-tmpnativeauthenticator-1.0.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/index.md` & `jupyterhub-tmpnativeauthenticator-1.0.8/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/options.md` & `jupyterhub-tmpnativeauthenticator-1.0.8/docs/source/options.md`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/quickstart.md` & `jupyterhub-tmpnativeauthenticator-1.0.8/docs/source/quickstart.md`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/troubleshooting.md` & `jupyterhub-tmpnativeauthenticator-1.0.8/docs/source/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/jupyterhub_tmpnativeauthenticator.egg-info/PKG-INFO` & `jupyterhub-tmpnativeauthenticator-1.0.8/jupyterhub_tmpnativeauthenticator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterhub-tmpnativeauthenticator
-Version: 1.0.7
+Version: 1.0.8
 Summary: JupyterHub Native Authenticator with tmp login
 Home-page: https://github.com/Gorbacheb/tmpnativeauthenticator
 Author: Vladimir Nedugov
 Author-email: MegaRs1@yandex.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/jupyterhub_tmpnativeauthenticator.egg-info/SOURCES.txt` & `jupyterhub-tmpnativeauthenticator-1.0.8/jupyterhub_tmpnativeauthenticator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/common-credentials.txt` & `jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/common-credentials.txt`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/crypto/crypto.py` & `jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/crypto/encoding.py` & `jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/crypto/encoding.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/crypto/signing.py` & `jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/crypto/signing.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/handlers.py` & `jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -548,16 +548,17 @@
         self.force_new_server = force_new_server
         self.process_user = process_user
 
     @gen.coroutine
     def get(self):
         raw_user = yield self.get_current_user()
 
+        #перед созданием нового пользователя удаляем неактивных старых
         for user_name, user in list(self.users.items()):
-            if (datetime.utcnow() - user.last_activity).total_seconds() >= self.tmp_user_lifetime:
+            if (datetime.utcnow() - user.last_activity).seconds >= self.tmp_user_lifetime:
                 self.users.delete(user_name)
 
         if raw_user:
             if self.force_new_server and raw_user.running:
                 # Stop user's current server if it is running
                 # so we get a new one.
                 status = yield raw_user.spawner.poll_and_notify()
```

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/nativeauthenticator.py` & `jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/nativeauthenticator.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,17 +178,17 @@
         new single-user server. When set to False, they'll be
         redirected to their current session if one exists.
         """,
         config=True
     )
 
     tmp_user_lifetime = Integer(
-        48,
+        172800,
         help="""
-        number of hours when temporary user will alive.
+        number of seconds when temporary user will alive.
         """,
         config=True
     )
 
     def process_user(self, user, handler):
         """
         Do additional arbitrary things to the created user before spawn.
```

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/orm.py` & `jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/orm.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/templates/authorization-area.html` & `jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/templates/authorization-area.html`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/templates/change-password-admin.html` & `jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/templates/change-password-admin.html`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/templates/change-password.html` & `jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/templates/change-password.html`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/templates/native-login.html` & `jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/templates/native-login.html`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/templates/signup.html` & `jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/templates/signup.html`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/tests/test_authenticator.py` & `jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/tests/test_authenticator.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/tests/test_orm.py` & `jupyterhub-tmpnativeauthenticator-1.0.8/nativeauthenticator/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.7/setup.py` & `jupyterhub-tmpnativeauthenticator-1.0.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setup(
     name="jupyterhub-tmpnativeauthenticator",
-    version="1.0.7",
+    version="1.0.8",
     description="JupyterHub Native Authenticator with tmp login",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Gorbacheb/tmpnativeauthenticator",
     author="Vladimir Nedugov",
     author_email="MegaRs1@yandex.ru",
     license="MIT",
```

