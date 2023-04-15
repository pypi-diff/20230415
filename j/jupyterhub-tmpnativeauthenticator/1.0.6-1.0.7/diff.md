# Comparing `tmp/jupyterhub-tmpnativeauthenticator-1.0.6.tar.gz` & `tmp/jupyterhub-tmpnativeauthenticator-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-tmpnativeauthenticator-1.0.6.tar", last modified: Sat Apr 15 17:47:50 2023, max compression
+gzip compressed data, was "jupyterhub-tmpnativeauthenticator-1.0.7.tar", last modified: Sat Apr 15 17:49:29 2023, max compression
```

## Comparing `jupyterhub-tmpnativeauthenticator-1.0.6.tar` & `jupyterhub-tmpnativeauthenticator-1.0.7.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 17:47:50.699613 jupyterhub-tmpnativeauthenticator-1.0.6/
--rw-rw-rw-   0        0        0     1539 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/LICENSE
--rw-rw-rw-   0        0        0      179 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     2947 2023-04-15 17:47:50.699613 jupyterhub-tmpnativeauthenticator-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2607 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/README.md
--rw-rw-rw-   0        0        0       98 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/dev-requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 17:47:50.654612 jupyterhub-tmpnativeauthenticator-1.0.6/docs/
--rw-rw-rw-   0        0        0     1353 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/docs/Makefile
--rwxrwxrwx   0        0        0     1108 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/docs/make.bat
--rw-rw-rw-   0        0        0      321 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 17:47:50.658612 jupyterhub-tmpnativeauthenticator-1.0.6/docs/source/
-drwxrwxrwx   0        0        0        0 2023-04-15 17:47:50.673614 jupyterhub-tmpnativeauthenticator-1.0.6/docs/source/_static/
--rw-rw-rw-   0        0        0    62232 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/docs/source/_static/authorization_area.png
--rw-rw-rw-   0        0        0  2487640 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/docs/source/_static/block_user_failed_logins.png
--rw-rw-rw-   0        0        0    59939 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/docs/source/_static/change_password_self.png
--rw-rw-rw-   0        0        0    52206 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/docs/source/_static/change_password_user.png
--rw-rw-rw-   0        0        0    85574 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/docs/source/_static/login-two-factor-auth.png
--rw-rw-rw-   0        0        0  1355938 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/docs/source/_static/native_auth_flow.png
--rw-rw-rw-   0        0        0    91790 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/docs/source/_static/signup-two-factor-auth.png
--rw-rw-rw-   0        0        0    78767 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/docs/source/_static/wrong_signup.png
--rw-rw-rw-   0        0        0     1939 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/docs/source/conf.py
--rw-rw-rw-   0        0        0     1127 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/docs/source/index.md
--rw-rw-rw-   0        0        0    10165 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/docs/source/options.md
--rw-rw-rw-   0        0        0     4435 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/docs/source/quickstart.md
--rw-rw-rw-   0        0        0     2033 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/docs/source/troubleshooting.md
-drwxrwxrwx   0        0        0        0 2023-04-15 17:47:50.678642 jupyterhub-tmpnativeauthenticator-1.0.6/jupyterhub_tmpnativeauthenticator.egg-info/
--rw-rw-rw-   0        0        0     2947 2023-04-15 17:47:50.000000 jupyterhub-tmpnativeauthenticator-1.0.6/jupyterhub_tmpnativeauthenticator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1659 2023-04-15 17:47:50.000000 jupyterhub-tmpnativeauthenticator-1.0.6/jupyterhub_tmpnativeauthenticator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 17:47:50.000000 jupyterhub-tmpnativeauthenticator-1.0.6/jupyterhub_tmpnativeauthenticator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-15 17:47:50.000000 jupyterhub-tmpnativeauthenticator-1.0.6/jupyterhub_tmpnativeauthenticator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-15 17:47:50.000000 jupyterhub-tmpnativeauthenticator-1.0.6/jupyterhub_tmpnativeauthenticator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 17:47:50.684614 jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/
--rw-rw-rw-   0        0        0      123 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/__init__.py
--rw-rw-rw-   0        0        0    86508 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/common-credentials.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 17:47:50.687625 jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/crypto/
--rw-rw-rw-   0        0        0        0 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/crypto/__init__.py
--rw-rw-rw-   0        0        0     2584 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/crypto/crypto.py
--rw-rw-rw-   0        0        0     6660 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/crypto/encoding.py
--rw-rw-rw-   0        0        0     7948 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/crypto/signing.py
--rw-rw-rw-   0        0        0    22116 2023-04-15 17:47:12.000000 jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/handlers.py
--rw-rw-rw-   0        0        0    16265 2023-04-15 17:38:41.000000 jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/nativeauthenticator.py
--rw-rw-rw-   0        0        0     4470 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/orm.py
-drwxrwxrwx   0        0        0        0 2023-04-15 17:47:50.694638 jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/templates/
--rw-rw-rw-   0        0        0     1915 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/templates/authorization-area.html
--rw-rw-rw-   0        0        0     2333 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/templates/change-password-admin.html
--rw-rw-rw-   0        0        0     2944 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/templates/change-password.html
--rw-rw-rw-   0        0        0      256 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/templates/my_message.html
--rw-rw-rw-   0        0        0     3207 2023-04-12 11:55:33.000000 jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/templates/native-login.html
--rw-rw-rw-   0        0        0      290 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/templates/page.html
--rw-rw-rw-   0        0        0     5008 2023-04-12 12:53:22.000000 jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/templates/signup.html
-drwxrwxrwx   0        0        0        0 2023-04-15 17:47:50.697649 jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/tests/
--rw-rw-rw-   0        0        0        0 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/tests/__init__.py
--rw-rw-rw-   0        0        0    12828 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/tests/test_authenticator.py
--rw-rw-rw-   0        0        0     1291 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/tests/test_orm.py
--rw-rw-rw-   0        0        0       42 2023-04-15 17:47:50.699613 jupyterhub-tmpnativeauthenticator-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      662 2023-04-15 17:47:41.000000 jupyterhub-tmpnativeauthenticator-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 17:49:29.545765 jupyterhub-tmpnativeauthenticator-1.0.7/
+-rw-rw-rw-   0        0        0     1539 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0      179 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     2947 2023-04-15 17:49:29.544703 jupyterhub-tmpnativeauthenticator-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2607 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/README.md
+-rw-rw-rw-   0        0        0       98 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/dev-requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 17:49:29.490738 jupyterhub-tmpnativeauthenticator-1.0.7/docs/
+-rw-rw-rw-   0        0        0     1353 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/Makefile
+-rwxrwxrwx   0        0        0     1108 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/make.bat
+-rw-rw-rw-   0        0        0      321 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 17:49:29.496702 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/
+drwxrwxrwx   0        0        0        0 2023-04-15 17:49:29.511703 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/
+-rw-rw-rw-   0        0        0    62232 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/authorization_area.png
+-rw-rw-rw-   0        0        0  2487640 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/block_user_failed_logins.png
+-rw-rw-rw-   0        0        0    59939 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/change_password_self.png
+-rw-rw-rw-   0        0        0    52206 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/change_password_user.png
+-rw-rw-rw-   0        0        0    85574 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/login-two-factor-auth.png
+-rw-rw-rw-   0        0        0  1355938 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/native_auth_flow.png
+-rw-rw-rw-   0        0        0    91790 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/signup-two-factor-auth.png
+-rw-rw-rw-   0        0        0    78767 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/wrong_signup.png
+-rw-rw-rw-   0        0        0     1939 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/conf.py
+-rw-rw-rw-   0        0        0     1127 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/index.md
+-rw-rw-rw-   0        0        0    10165 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/options.md
+-rw-rw-rw-   0        0        0     4435 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/quickstart.md
+-rw-rw-rw-   0        0        0     2033 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/troubleshooting.md
+drwxrwxrwx   0        0        0        0 2023-04-15 17:49:29.517727 jupyterhub-tmpnativeauthenticator-1.0.7/jupyterhub_tmpnativeauthenticator.egg-info/
+-rw-rw-rw-   0        0        0     2947 2023-04-15 17:49:29.000000 jupyterhub-tmpnativeauthenticator-1.0.7/jupyterhub_tmpnativeauthenticator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1659 2023-04-15 17:49:29.000000 jupyterhub-tmpnativeauthenticator-1.0.7/jupyterhub_tmpnativeauthenticator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 17:49:29.000000 jupyterhub-tmpnativeauthenticator-1.0.7/jupyterhub_tmpnativeauthenticator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-04-15 17:49:29.000000 jupyterhub-tmpnativeauthenticator-1.0.7/jupyterhub_tmpnativeauthenticator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-15 17:49:29.000000 jupyterhub-tmpnativeauthenticator-1.0.7/jupyterhub_tmpnativeauthenticator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 17:49:29.525704 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/
+-rw-rw-rw-   0        0        0      123 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/__init__.py
+-rw-rw-rw-   0        0        0    86508 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/common-credentials.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 17:49:29.531702 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/crypto/
+-rw-rw-rw-   0        0        0        0 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/crypto/__init__.py
+-rw-rw-rw-   0        0        0     2584 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/crypto/crypto.py
+-rw-rw-rw-   0        0        0     6660 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/crypto/encoding.py
+-rw-rw-rw-   0        0        0     7948 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/crypto/signing.py
+-rw-rw-rw-   0        0        0    22117 2023-04-15 17:49:14.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/handlers.py
+-rw-rw-rw-   0        0        0    16265 2023-04-15 17:38:41.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/nativeauthenticator.py
+-rw-rw-rw-   0        0        0     4470 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/orm.py
+drwxrwxrwx   0        0        0        0 2023-04-15 17:49:29.539727 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/templates/
+-rw-rw-rw-   0        0        0     1915 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/templates/authorization-area.html
+-rw-rw-rw-   0        0        0     2333 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/templates/change-password-admin.html
+-rw-rw-rw-   0        0        0     2944 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/templates/change-password.html
+-rw-rw-rw-   0        0        0      256 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/templates/my_message.html
+-rw-rw-rw-   0        0        0     3207 2023-04-12 11:55:33.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/templates/native-login.html
+-rw-rw-rw-   0        0        0      290 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/templates/page.html
+-rw-rw-rw-   0        0        0     5008 2023-04-12 12:53:22.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/templates/signup.html
+drwxrwxrwx   0        0        0        0 2023-04-15 17:49:29.543703 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/tests/__init__.py
+-rw-rw-rw-   0        0        0    12828 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/tests/test_authenticator.py
+-rw-rw-rw-   0        0        0     1291 2023-04-12 11:03:44.000000 jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/tests/test_orm.py
+-rw-rw-rw-   0        0        0       42 2023-04-15 17:49:29.545765 jupyterhub-tmpnativeauthenticator-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      662 2023-04-15 17:49:26.000000 jupyterhub-tmpnativeauthenticator-1.0.7/setup.py
```

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/LICENSE` & `jupyterhub-tmpnativeauthenticator-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/PKG-INFO` & `jupyterhub-tmpnativeauthenticator-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterhub-tmpnativeauthenticator
-Version: 1.0.6
+Version: 1.0.7
 Summary: JupyterHub Native Authenticator with tmp login
 Home-page: https://github.com/Gorbacheb/tmpnativeauthenticator
 Author: Vladimir Nedugov
 Author-email: MegaRs1@yandex.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/README.md` & `jupyterhub-tmpnativeauthenticator-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/docs/Makefile` & `jupyterhub-tmpnativeauthenticator-1.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/docs/make.bat` & `jupyterhub-tmpnativeauthenticator-1.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/docs/source/_static/authorization_area.png` & `jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/authorization_area.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/docs/source/_static/block_user_failed_logins.png` & `jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/block_user_failed_logins.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/docs/source/_static/change_password_self.png` & `jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/change_password_self.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/docs/source/_static/change_password_user.png` & `jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/change_password_user.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/docs/source/_static/login-two-factor-auth.png` & `jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/login-two-factor-auth.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/docs/source/_static/native_auth_flow.png` & `jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/native_auth_flow.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/docs/source/_static/signup-two-factor-auth.png` & `jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/signup-two-factor-auth.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/docs/source/_static/wrong_signup.png` & `jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/_static/wrong_signup.png`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/docs/source/conf.py` & `jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/docs/source/index.md` & `jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/docs/source/options.md` & `jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/options.md`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/docs/source/quickstart.md` & `jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/quickstart.md`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/docs/source/troubleshooting.md` & `jupyterhub-tmpnativeauthenticator-1.0.7/docs/source/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/jupyterhub_tmpnativeauthenticator.egg-info/PKG-INFO` & `jupyterhub-tmpnativeauthenticator-1.0.7/jupyterhub_tmpnativeauthenticator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterhub-tmpnativeauthenticator
-Version: 1.0.6
+Version: 1.0.7
 Summary: JupyterHub Native Authenticator with tmp login
 Home-page: https://github.com/Gorbacheb/tmpnativeauthenticator
 Author: Vladimir Nedugov
 Author-email: MegaRs1@yandex.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/jupyterhub_tmpnativeauthenticator.egg-info/SOURCES.txt` & `jupyterhub-tmpnativeauthenticator-1.0.7/jupyterhub_tmpnativeauthenticator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/common-credentials.txt` & `jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/common-credentials.txt`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/crypto/crypto.py` & `jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/crypto/encoding.py` & `jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/crypto/encoding.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/crypto/signing.py` & `jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/crypto/signing.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/handlers.py` & `jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -548,15 +548,15 @@
         self.force_new_server = force_new_server
         self.process_user = process_user
 
     @gen.coroutine
     def get(self):
         raw_user = yield self.get_current_user()
 
-        for user_name, user in list(self.users.keys()):
+        for user_name, user in list(self.users.items()):
             if (datetime.utcnow() - user.last_activity).total_seconds() >= self.tmp_user_lifetime:
                 self.users.delete(user_name)
 
         if raw_user:
             if self.force_new_server and raw_user.running:
                 # Stop user's current server if it is running
                 # so we get a new one.
```

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/nativeauthenticator.py` & `jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/nativeauthenticator.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/orm.py` & `jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/orm.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/templates/authorization-area.html` & `jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/templates/authorization-area.html`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/templates/change-password-admin.html` & `jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/templates/change-password-admin.html`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/templates/change-password.html` & `jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/templates/change-password.html`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/templates/native-login.html` & `jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/templates/native-login.html`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/templates/signup.html` & `jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/templates/signup.html`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/tests/test_authenticator.py` & `jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/tests/test_authenticator.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/nativeauthenticator/tests/test_orm.py` & `jupyterhub-tmpnativeauthenticator-1.0.7/nativeauthenticator/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-tmpnativeauthenticator-1.0.6/setup.py` & `jupyterhub-tmpnativeauthenticator-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setup(
     name="jupyterhub-tmpnativeauthenticator",
-    version="1.0.6",
+    version="1.0.7",
     description="JupyterHub Native Authenticator with tmp login",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Gorbacheb/tmpnativeauthenticator",
     author="Vladimir Nedugov",
     author_email="MegaRs1@yandex.ru",
     license="MIT",
```

