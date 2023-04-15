# Comparing `tmp/django-username-email-2.5.3.tar.gz` & `tmp/django-username-email-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-username-email-2.5.3.tar", last modified: Wed Jun  8 02:13:34 2022, max compression
+gzip compressed data, was "django-username-email-2.5.4.tar", last modified: Sat Apr 15 03:18:12 2023, max compression
```

## Comparing `django-username-email-2.5.3.tar` & `django-username-email-2.5.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 taylors    (501) staff       (20)        0 2022-06-08 02:13:34.812551 django-username-email-2.5.3/
--rw-r--r--   0 taylors    (501) staff       (20)     1087 2022-06-08 02:13:23.000000 django-username-email-2.5.3/LICENSE
--rw-r--r--   0 taylors    (501) staff       (20)       71 2022-06-08 02:13:23.000000 django-username-email-2.5.3/MANIFEST.in
--rw-r--r--   0 taylors    (501) staff       (20)     8447 2022-06-08 02:13:34.812229 django-username-email-2.5.3/PKG-INFO
--rw-r--r--   0 taylors    (501) staff       (20)     7386 2022-06-08 02:13:23.000000 django-username-email-2.5.3/README.rst
-drwxr-xr-x   0 taylors    (501) staff       (20)        0 2022-06-08 02:13:34.808760 django-username-email-2.5.3/cuser/
--rw-r--r--   0 taylors    (501) staff       (20)        0 2022-06-08 02:13:23.000000 django-username-email-2.5.3/cuser/__init__.py
--rw-r--r--   0 taylors    (501) staff       (20)     1437 2022-06-08 02:13:23.000000 django-username-email-2.5.3/cuser/admin.py
--rw-r--r--   0 taylors    (501) staff       (20)      230 2022-06-08 02:13:23.000000 django-username-email-2.5.3/cuser/apps.py
--rw-r--r--   0 taylors    (501) staff       (20)     6158 2022-06-08 02:13:23.000000 django-username-email-2.5.3/cuser/forms.py
-drwxr-xr-x   0 taylors    (501) staff       (20)        0 2022-06-08 02:13:34.809878 django-username-email-2.5.3/cuser/migrations/
--rw-r--r--   0 taylors    (501) staff       (20)     3209 2022-06-08 02:13:23.000000 django-username-email-2.5.3/cuser/migrations/0001_initial.py
--rw-r--r--   0 taylors    (501) staff       (20)      365 2022-06-08 02:13:23.000000 django-username-email-2.5.3/cuser/migrations/0002_alter_user_last_name_max_length.py
--rw-r--r--   0 taylors    (501) staff       (20)      391 2022-06-08 02:13:23.000000 django-username-email-2.5.3/cuser/migrations/0003_alter_user_first_name_max_length.py
--rw-r--r--   0 taylors    (501) staff       (20)        0 2022-06-08 02:13:23.000000 django-username-email-2.5.3/cuser/migrations/__init__.py
--rw-r--r--   0 taylors    (501) staff       (20)     5155 2022-06-08 02:13:23.000000 django-username-email-2.5.3/cuser/models.py
--rw-r--r--   0 taylors    (501) staff       (20)      272 2022-06-08 02:13:23.000000 django-username-email-2.5.3/cuser/settings.py
-drwxr-xr-x   0 taylors    (501) staff       (20)        0 2022-06-08 02:13:34.806110 django-username-email-2.5.3/cuser/templates/
-drwxr-xr-x   0 taylors    (501) staff       (20)        0 2022-06-08 02:13:34.806176 django-username-email-2.5.3/cuser/templates/admin/
-drwxr-xr-x   0 taylors    (501) staff       (20)        0 2022-06-08 02:13:34.806243 django-username-email-2.5.3/cuser/templates/admin/cuser/
-drwxr-xr-x   0 taylors    (501) staff       (20)        0 2022-06-08 02:13:34.810094 django-username-email-2.5.3/cuser/templates/admin/cuser/cuser/
--rw-r--r--   0 taylors    (501) staff       (20)      324 2022-06-08 02:13:23.000000 django-username-email-2.5.3/cuser/templates/admin/cuser/cuser/add_form.html
-drwxr-xr-x   0 taylors    (501) staff       (20)        0 2022-06-08 02:13:34.811769 django-username-email-2.5.3/django_username_email.egg-info/
--rw-r--r--   0 taylors    (501) staff       (20)     8447 2022-06-08 02:13:34.000000 django-username-email-2.5.3/django_username_email.egg-info/PKG-INFO
--rw-r--r--   0 taylors    (501) staff       (20)      584 2022-06-08 02:13:34.000000 django-username-email-2.5.3/django_username_email.egg-info/SOURCES.txt
--rw-r--r--   0 taylors    (501) staff       (20)        1 2022-06-08 02:13:34.000000 django-username-email-2.5.3/django_username_email.egg-info/dependency_links.txt
--rw-r--r--   0 taylors    (501) staff       (20)       12 2022-06-08 02:13:34.000000 django-username-email-2.5.3/django_username_email.egg-info/requires.txt
--rw-r--r--   0 taylors    (501) staff       (20)        6 2022-06-08 02:13:34.000000 django-username-email-2.5.3/django_username_email.egg-info/top_level.txt
--rw-r--r--   0 taylors    (501) staff       (20)       38 2022-06-08 02:13:34.812622 django-username-email-2.5.3/setup.cfg
--rw-r--r--   0 taylors    (501) staff       (20)     1434 2022-06-08 02:13:23.000000 django-username-email-2.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:12.351209 django-username-email-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-15 03:18:03.000000 django-username-email-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-15 03:18:03.000000 django-username-email-2.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-04-15 03:18:12.351209 django-username-email-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-04-15 03:18:03.000000 django-username-email-2.5.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:12.347209 django-username-email-2.5.4/cuser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:03.000000 django-username-email-2.5.4/cuser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-15 03:18:03.000000 django-username-email-2.5.4/cuser/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-15 03:18:03.000000 django-username-email-2.5.4/cuser/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-04-15 03:18:03.000000 django-username-email-2.5.4/cuser/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:12.347209 django-username-email-2.5.4/cuser/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-15 03:18:03.000000 django-username-email-2.5.4/cuser/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-15 03:18:03.000000 django-username-email-2.5.4/cuser/migrations/0002_alter_user_last_name_max_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-15 03:18:03.000000 django-username-email-2.5.4/cuser/migrations/0003_alter_user_first_name_max_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:03.000000 django-username-email-2.5.4/cuser/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-04-15 03:18:03.000000 django-username-email-2.5.4/cuser/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-15 03:18:03.000000 django-username-email-2.5.4/cuser/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:12.347209 django-username-email-2.5.4/cuser/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:12.347209 django-username-email-2.5.4/cuser/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:12.347209 django-username-email-2.5.4/cuser/templates/admin/cuser/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:12.347209 django-username-email-2.5.4/cuser/templates/admin/cuser/cuser/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-15 03:18:03.000000 django-username-email-2.5.4/cuser/templates/admin/cuser/cuser/add_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:18:12.351209 django-username-email-2.5.4/django_username_email.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8576 2023-04-15 03:18:12.000000 django-username-email-2.5.4/django_username_email.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-15 03:18:12.000000 django-username-email-2.5.4/django_username_email.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 03:18:12.000000 django-username-email-2.5.4/django_username_email.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-15 03:18:12.000000 django-username-email-2.5.4/django_username_email.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-15 03:18:12.000000 django-username-email-2.5.4/django_username_email.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 03:18:12.351209 django-username-email-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-15 03:18:03.000000 django-username-email-2.5.4/setup.py
```

### Comparing `django-username-email-2.5.3/LICENSE` & `django-username-email-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-username-email-2.5.3/PKG-INFO` & `django-username-email-2.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-username-email
-Version: 2.5.3
+Version: 2.5.4
 Summary: Custom Django User model that makes email the USERNAME_FIELD.
 Home-page: https://github.com/tmm/django-username-email/
 Author: Adam Taylor
 Author-email: ataylor32@gmail.com
 License: MIT
 Keywords: user email username
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,18 +14,21 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
 
 CUser, make email the USERNAME\_FIELD
 =====================================
 
 CUser makes it easy to use email address as your identification token
@@ -33,15 +36,15 @@
 
 CUser is a custom Django user model (extends ``AbstractBaseUser``) so it
 takes a tiny amount of effort to use.
 
 The only difference between CUser and the vanilla Django ``User`` is email
 address is the ``USERNAME_FIELD`` (and username does not exist).
 
-CUser supports Django 3.2 - 4.0. If you need to use CUser with
+CUser supports Django 3.2 - 4.2. If you need to use CUser with
 Django 1.8 - 3.1, you must install an older, unmaintained version of
 CUser, as noted in the "Install & Set up" section.
 
 Why use CUser?
 --------------
 
 Because you want everything in ``django.contrib.auth`` except for the
@@ -76,15 +79,15 @@
    custom user models, jump to **Notes** first (then come
    back). Otherwise, continue onward!
 
 2. Install with ``pip``:
 
    .. code-block:: shell
 
-       # Django 3.2 - 4.0
+       # Django 3.2 - 4.2
        pip install django-username-email
 
        # Django 3.1 (unmaintained)
        pip install django-username-email==2.4.2
 
        # Django 2.2 or 3.0 (unmaintained)
        pip install django-username-email==2.3.1
```

### Comparing `django-username-email-2.5.3/README.rst` & `django-username-email-2.5.4/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 CUser is a custom Django user model (extends ``AbstractBaseUser``) so it
 takes a tiny amount of effort to use.
 
 The only difference between CUser and the vanilla Django ``User`` is email
 address is the ``USERNAME_FIELD`` (and username does not exist).
 
-CUser supports Django 3.2 - 4.0. If you need to use CUser with
+CUser supports Django 3.2 - 4.2. If you need to use CUser with
 Django 1.8 - 3.1, you must install an older, unmaintained version of
 CUser, as noted in the "Install & Set up" section.
 
 Why use CUser?
 --------------
 
 Because you want everything in ``django.contrib.auth`` except for the
@@ -49,15 +49,15 @@
    custom user models, jump to **Notes** first (then come
    back). Otherwise, continue onward!
 
 2. Install with ``pip``:
 
    .. code-block:: shell
 
-       # Django 3.2 - 4.0
+       # Django 3.2 - 4.2
        pip install django-username-email
 
        # Django 3.1 (unmaintained)
        pip install django-username-email==2.4.2
 
        # Django 2.2 or 3.0 (unmaintained)
        pip install django-username-email==2.3.1
```

### Comparing `django-username-email-2.5.3/cuser/admin.py` & `django-username-email-2.5.4/cuser/admin.py`

 * *Files identical despite different names*

### Comparing `django-username-email-2.5.3/cuser/forms.py` & `django-username-email-2.5.4/cuser/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,16 @@
                 self.add_error('password2', error)
 
     def save(self, commit=True):
         user = super().save(commit=False)
         user.set_password(self.cleaned_data["password1"])
         if commit:
             user.save()
+            if django.VERSION >= (4, 2) and hasattr(self, "save_m2m"):
+                self.save_m2m()
         return user
 
 
 class UserChangeForm(forms.ModelForm):
     email = forms.EmailField(
         label=_("Email address"),
         max_length=254,
@@ -165,15 +167,20 @@
         fields = '__all__'
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         password = self.fields.get('password')
         if password:
-            password.help_text = password.help_text.format('../password/')
+            if django.VERSION >= (4, 2):
+                password.help_text = password.help_text.format(
+                    f"../../{self.instance.pk}/password/"
+                )
+            else:
+                password.help_text = password.help_text.format('../password/')
         user_permissions = self.fields.get('user_permissions')
         if user_permissions:
             user_permissions.queryset = user_permissions.queryset.select_related('content_type')
 
     if django.VERSION < (3, 2):
         def clean_password(self):
             # Regardless of what the user provides, return the initial value.
```

### Comparing `django-username-email-2.5.3/cuser/migrations/0001_initial.py` & `django-username-email-2.5.4/cuser/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-username-email-2.5.3/cuser/models.py` & `django-username-email-2.5.4/cuser/models.py`

 * *Files identical despite different names*

### Comparing `django-username-email-2.5.3/django_username_email.egg-info/PKG-INFO` & `django-username-email-2.5.4/django_username_email.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-username-email
-Version: 2.5.3
+Version: 2.5.4
 Summary: Custom Django User model that makes email the USERNAME_FIELD.
 Home-page: https://github.com/tmm/django-username-email/
 Author: Adam Taylor
 Author-email: ataylor32@gmail.com
 License: MIT
 Keywords: user email username
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,18 +14,21 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
 
 CUser, make email the USERNAME\_FIELD
 =====================================
 
 CUser makes it easy to use email address as your identification token
@@ -33,15 +36,15 @@
 
 CUser is a custom Django user model (extends ``AbstractBaseUser``) so it
 takes a tiny amount of effort to use.
 
 The only difference between CUser and the vanilla Django ``User`` is email
 address is the ``USERNAME_FIELD`` (and username does not exist).
 
-CUser supports Django 3.2 - 4.0. If you need to use CUser with
+CUser supports Django 3.2 - 4.2. If you need to use CUser with
 Django 1.8 - 3.1, you must install an older, unmaintained version of
 CUser, as noted in the "Install & Set up" section.
 
 Why use CUser?
 --------------
 
 Because you want everything in ``django.contrib.auth`` except for the
@@ -76,15 +79,15 @@
    custom user models, jump to **Notes** first (then come
    back). Otherwise, continue onward!
 
 2. Install with ``pip``:
 
    .. code-block:: shell
 
-       # Django 3.2 - 4.0
+       # Django 3.2 - 4.2
        pip install django-username-email
 
        # Django 3.1 (unmaintained)
        pip install django-username-email==2.4.2
 
        # Django 2.2 or 3.0 (unmaintained)
        pip install django-username-email==2.3.1
```

### Comparing `django-username-email-2.5.3/django_username_email.egg-info/SOURCES.txt` & `django-username-email-2.5.4/django_username_email.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-username-email-2.5.3/setup.py` & `django-username-email-2.5.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from os import path
-from setuptools import setup, find_packages
+from setuptools import setup, find_namespace_packages
 
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.rst')) as f:
     long_description = f.read()
 
 setup(
     name='django-username-email',
 
-    version='2.5.3',
+    version='2.5.4',
 
     description='Custom Django User model that makes email the USERNAME_FIELD.',
     long_description=long_description,
 
     url='https://github.com/tmm/django-username-email/',
 
     author='Adam Taylor',
@@ -32,23 +32,26 @@
 
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
 
         'Environment :: Web Environment',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
         'Operating System :: OS Independent',
     ],
     keywords='user email username',
 
-    packages=find_packages(),
+    packages=find_namespace_packages(),
     include_package_data=True,
 
     install_requires=[
         'django>=3.2',
     ]
 )
```

