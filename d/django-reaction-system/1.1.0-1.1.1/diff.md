# Comparing `tmp/django-reaction-system-1.1.0.tar.gz` & `tmp/django-reaction-system-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-reaction-system-1.1.0.tar", last modified: Mon Apr 10 11:16:15 2023, max compression
+gzip compressed data, was "django-reaction-system-1.1.1.tar", last modified: Sat Apr 15 12:13:01 2023, max compression
```

## Comparing `django-reaction-system-1.1.0.tar` & `django-reaction-system-1.1.1.tar`

### file list

```diff
@@ -1,48 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:15.474034 django-reaction-system-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-10 11:16:15.474034 django-reaction-system-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:15.474034 django-reaction-system-1.1.0/django_reaction_system.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-10 11:16:15.000000 django-reaction-system-1.1.0/django_reaction_system.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:15.474034 django-reaction-system-1.1.0/reaction/
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:15.474034 django-reaction-system-1.1.0/reaction/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/migrations/0002_config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:15.470034 django-reaction-system-1.1.0/reaction/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:15.470034 django-reaction-system-1.1.0/reaction/static/reaction/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:15.474034 django-reaction-system-1.1.0/reaction/static/reaction/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/static/reaction/css/style.css
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/static/reaction/css/style.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:15.474034 django-reaction-system-1.1.0/reaction/static/reaction/js/
--rw-r--r--   0 runner    (1001) docker     (123)    89574 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/static/reaction/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/static/reaction/js/reaction.js
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/static/reaction/js/reaction.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:15.474034 django-reaction-system-1.1.0/reaction/static/reaction/tailwindcss/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/static/reaction/tailwindcss/style.css
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/static/reaction/tailwindcss/tailwind.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:15.470034 django-reaction-system-1.1.0/reaction/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:15.470034 django-reaction-system-1.1.0/reaction/templates/reaction/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:15.474034 django-reaction-system-1.1.0/reaction/templates/reaction/reaction/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/templates/reaction/reaction/reaction.html
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/templates/reaction/reaction/reaction_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:15.474034 django-reaction-system-1.1.0/reaction/templates/reaction/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/templates/reaction/utils/IMPORTS.html
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/templates/reaction/utils/SCRIPTS.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:15.474034 django-reaction-system-1.1.0/reaction/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/templatetags/reaction_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/reaction/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-10 11:16:15.478034 django-reaction-system-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 11:16:12.000000 django-reaction-system-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:13:01.972516 django-reaction-system-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-15 12:13:01.972516 django-reaction-system-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:13:01.972516 django-reaction-system-1.1.1/django_reaction_system.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-15 12:13:01.000000 django-reaction-system-1.1.1/django_reaction_system.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:13:01.968516 django-reaction-system-1.1.1/reaction/
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/reaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/reaction/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/reaction/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:13:01.968516 django-reaction-system-1.1.1/reaction/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/reaction/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/reaction/migrations/0002_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/reaction/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/reaction/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/reaction/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:13:01.968516 django-reaction-system-1.1.1/reaction/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:13:01.968516 django-reaction-system-1.1.1/reaction/static/reaction/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:13:01.968516 django-reaction-system-1.1.1/reaction/static/reaction/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/reaction/static/reaction/css/reaction.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/reaction/static/reaction/css/reaction.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:13:01.972516 django-reaction-system-1.1.1/reaction/static/reaction/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/reaction/static/reaction/js/reaction.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/reaction/static/reaction/js/reaction.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:13:01.972516 django-reaction-system-1.1.1/reaction/static/reaction/tailwindcss/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/reaction/static/reaction/tailwindcss/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/reaction/static/reaction/tailwindcss/tailwind.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:13:01.968516 django-reaction-system-1.1.1/reaction/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:13:01.968516 django-reaction-system-1.1.1/reaction/templates/reaction/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:13:01.972516 django-reaction-system-1.1.1/reaction/templates/reaction/reaction/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/reaction/templates/reaction/reaction/reaction.html
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/reaction/templates/reaction/reaction/reaction_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:13:01.972516 django-reaction-system-1.1.1/reaction/templates/reaction/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/reaction/templates/reaction/utils/IMPORTS.html
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/reaction/templates/reaction/utils/SCRIPTS.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 12:13:01.972516 django-reaction-system-1.1.1/reaction/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/reaction/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/reaction/templatetags/reaction_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/reaction/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/reaction/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/reaction/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-15 12:13:01.972516 django-reaction-system-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 12:12:57.000000 django-reaction-system-1.1.1/setup.py
```

### Comparing `django-reaction-system-1.1.0/LICENSE` & `django-reaction-system-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-reaction-system-1.1.0/PKG-INFO` & `django-reaction-system-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-reaction-system
-Version: 1.1.0
+Version: 1.1.1
 Summary: Django reaction System, It can be associated with any given model.
 Home-page: https://github.com/mahyar-amiri/django-reaction-system
 Author: Mahyar Amiri
 Author-email: mmaahhyyaarr@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/mahyar-amiri/django-reaction-system/README.md
 Project-URL: Source Code, https://github.com/mahyar-amiri/django-reaction-system
```

### Comparing `django-reaction-system-1.1.0/README.md` & `django-reaction-system-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -205,16 +205,16 @@
 <details>
 <summary>Static Folder Tree</summary>
 <p>
 
 ```text
 static
    ├── css
-   │    ├── style.css
-   │    └── style.min.css
+   │    ├── reaction.css
+   │    └── reaction.min.css
    ├── js
    │    ├── reaction.js
    │    ├── reaction.min.js
    │    └── jquery.min.js
    └── tailwindcss
         ├── style.css
         └── tailwind.config.js
```

### Comparing `django-reaction-system-1.1.0/README.rst` & `django-reaction-system-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `django-reaction-system-1.1.0/django_reaction_system.egg-info/SOURCES.txt` & `django-reaction-system-1.1.1/django_reaction_system.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -13,17 +13,16 @@
 reaction/settings.py
 reaction/tests.py
 reaction/urls.py
 reaction/views.py
 reaction/migrations/0001_initial.py
 reaction/migrations/0002_config.py
 reaction/migrations/__init__.py
-reaction/static/reaction/css/style.css
-reaction/static/reaction/css/style.min.css
-reaction/static/reaction/js/jquery.min.js
+reaction/static/reaction/css/reaction.css
+reaction/static/reaction/css/reaction.min.css
 reaction/static/reaction/js/reaction.js
 reaction/static/reaction/js/reaction.min.js
 reaction/static/reaction/tailwindcss/style.css
 reaction/static/reaction/tailwindcss/tailwind.config.js
 reaction/templates/reaction/reaction/reaction.html
 reaction/templates/reaction/reaction/reaction_form.html
 reaction/templates/reaction/utils/IMPORTS.html
```

### Comparing `django-reaction-system-1.1.0/reaction/__init__.py` & `django-reaction-system-1.1.1/reaction/__init__.py`

 * *Files identical despite different names*

### Comparing `django-reaction-system-1.1.0/reaction/admin.py` & `django-reaction-system-1.1.1/reaction/admin.py`

 * *Files identical despite different names*

### Comparing `django-reaction-system-1.1.0/reaction/migrations/0001_initial.py` & `django-reaction-system-1.1.1/reaction/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-reaction-system-1.1.0/reaction/migrations/0002_config.py` & `django-reaction-system-1.1.1/reaction/migrations/0002_config.py`

 * *Files identical despite different names*

### Comparing `django-reaction-system-1.1.0/reaction/models.py` & `django-reaction-system-1.1.1/reaction/models.py`

 * *Files identical despite different names*

### Comparing `django-reaction-system-1.1.0/reaction/static/reaction/css/style.css` & `django-reaction-system-1.1.1/reaction/static/reaction/css/reaction.css`

 * *Files identical despite different names*

### Comparing `django-reaction-system-1.1.0/reaction/static/reaction/css/style.min.css` & `django-reaction-system-1.1.1/reaction/static/reaction/css/reaction.min.css`

 * *Files 14% similar despite different names*

```diff
@@ -1 +1 @@
-.inline{display: inline}.h-12{height: 3rem}.h-6{height: 1.5rem}.w-6{width: 1.5rem}.cursor-pointer{cursor:pointer}.origin-bottom{transform-origin: bottom}.rounded-full{border-radius: 9999px}.border-2{border-width: 2px}.border-solid{border-style: solid}.border-react-default-border-light{--tw-border-opacity: 1;border-color: rgb(229 231 235 / var(--tw-border-opacity))}.border-react-selected-border-light{--tw-border-opacity: 1;border-color: rgb(191 219 254 / var(--tw-border-opacity))}.bg-react-default-bg-light{--tw-bg-opacity: 1;background-color: rgb(243 244 246 / var(--tw-bg-opacity))}.bg-react-selected-bg-light{--tw-bg-opacity: 1;background-color: rgb(219 234 254 / var(--tw-bg-opacity))}.px-2{padding-left: 0.5rem;padding-right: 0.5rem}.py-2{padding-top: 0.5rem;padding-bottom: 0.5rem}.text-base{font-size: 1rem;line-height: 1.5rem}.text-react-count-text-light{--tw-text-opacity: 1;color: rgb(0 0 0 / var(--tw-text-opacity))}.transition-transform{transition-property: transform;transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);transition-duration: 150ms}.duration-200{transition-duration: 200ms}.group:hover .group-hover\:scale-150{--tw-scale-x: 1.5;--tw-scale-y: 1.5;transform: translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}[dir="ltr"] .ltr\:pr-1{padding-right: 0.25rem}[dir="rtl"] .rtl\:pl-1{padding-left: 0.25rem}[data-mode="dark"] .dark\:border-react-default-border-dark{--tw-border-opacity: 1;border-color: rgb(107 114 128 / var(--tw-border-opacity))}[data-mode="dark"] .dark\:border-react-selected-border-dark{--tw-border-opacity: 1;border-color: rgb(30 41 59 / var(--tw-border-opacity))}[data-mode="dark"] .dark\:bg-react-default-bg-dark{--tw-bg-opacity: 1;background-color: rgb(51 65 85 / var(--tw-bg-opacity))}[data-mode="dark"] .dark\:bg-react-selected-bg-dark{--tw-bg-opacity: 1;background-color: rgb(100 116 139 / var(--tw-bg-opacity))}[data-mode="dark"] .dark\:text-react-count-text-dark{--tw-text-opacity: 1;color: rgb(243 244 246 / var(--tw-text-opacity))}
+.inline{display:inline}.h-12{height:3rem}.h-6{height:1.5rem}.w-6{width:1.5rem}.cursor-pointer{cursor:pointer}.origin-bottom{transform-origin:bottom}.rounded-full{border-radius:9999px}.border-2{border-width:2px}.border-solid{border-style:solid}.border-react-default-border-light{--tw-border-opacity:1;border-color:rgb(229 231 235 / var(--tw-border-opacity))}.border-react-selected-border-light{--tw-border-opacity:1;border-color:rgb(191 219 254 / var(--tw-border-opacity))}.bg-react-default-bg-light{--tw-bg-opacity:1;background-color:rgb(243 244 246 / var(--tw-bg-opacity))}.bg-react-selected-bg-light{--tw-bg-opacity:1;background-color:rgb(219 234 254 / var(--tw-bg-opacity))}.px-2{padding-left:0.5rem;padding-right:0.5rem}.py-2{padding-top:0.5rem;padding-bottom:0.5rem}.text-base{font-size:1rem;line-height:1.5rem}.text-react-count-text-light{--tw-text-opacity:1;color:rgb(0 0 0 / var(--tw-text-opacity))}.transition-transform{transition-property:transform;transition-timing-function:cubic-bezier(0.4,0,0.2,1);transition-duration:150ms}.duration-200{transition-duration:200ms}.group:hover .group-hover\:scale-150{--tw-scale-x:1.5;--tw-scale-y:1.5;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}[dir="ltr"] .ltr\:pr-1{padding-right:0.25rem}[dir="rtl"] .rtl\:pl-1{padding-left:0.25rem}[data-mode="dark"] .dark\:border-react-default-border-dark{--tw-border-opacity:1;border-color:rgb(107 114 128 / var(--tw-border-opacity))}[data-mode="dark"] .dark\:border-react-selected-border-dark{--tw-border-opacity:1;border-color:rgb(30 41 59 / var(--tw-border-opacity))}[data-mode="dark"] .dark\:bg-react-default-bg-dark{--tw-bg-opacity:1;background-color:rgb(51 65 85 / var(--tw-bg-opacity))}[data-mode="dark"] .dark\:bg-react-selected-bg-dark{--tw-bg-opacity:1;background-color:rgb(100 116 139 / var(--tw-bg-opacity))}[data-mode="dark"] .dark\:text-react-count-text-dark{--tw-text-opacity:1;color:rgb(243 244 246 / var(--tw-text-opacity))}
```

### Comparing `django-reaction-system-1.1.0/reaction/static/reaction/js/reaction.js` & `django-reaction-system-1.1.1/reaction/static/reaction/js/reaction.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -67,35 +67,14 @@
                 );
             } else {
                 alert('ERROR in Submitting Reaction!')
             }
         }
     }
     http.send(JSON.stringify(data));
-    // $.ajax({
-    //     type: method,
-    //     url: action,
-    //     data: {
-    //         urlhash,
-    //         react_slug
-    //     },
-    //     headers: {
-    //         'X-Requested-With': 'XMLHttpRequest',
-    //         'X-CSRFToken': getCookie('csrftoken'),
-    //     },
-    //     success: function () {
-    //         load(
-    //             document.querySelector(`#form-reaction-${urlhash}`),
-    //             `/reaction/react?urlhash=${urlhash}`
-    //         );
-    //     },
-    //     error: function () {
-    //         alert('ERROR in Submitting Reaction!')
-    //     }
-    // });
 }
 
 document.addEventListener("DOMContentLoaded", () => {
     const reaction_items = document.querySelectorAll(`[id^='form-reaction-']`)
     reaction_items.forEach(function(item) {
         const urlhash = item.id.replace('form-reaction-', '')
         load(
```

### Comparing `django-reaction-system-1.1.0/reaction/static/reaction/js/reaction.min.js` & `django-reaction-system-1.1.1/reaction/static/reaction/js/reaction.min.js`

 * *Files identical despite different names*

### Comparing `django-reaction-system-1.1.0/reaction/static/reaction/tailwindcss/tailwind.config.js` & `django-reaction-system-1.1.1/reaction/static/reaction/tailwindcss/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `django-reaction-system-1.1.0/reaction/templates/reaction/reaction/reaction.html` & `django-reaction-system-1.1.1/reaction/templates/reaction/reaction/reaction.html`

 * *Files identical despite different names*

### Comparing `django-reaction-system-1.1.0/reaction/templatetags/reaction_tags.py` & `django-reaction-system-1.1.1/reaction/templatetags/reaction_tags.py`

 * *Files identical despite different names*

### Comparing `django-reaction-system-1.1.0/reaction/views.py` & `django-reaction-system-1.1.1/reaction/views.py`

 * *Files identical despite different names*

### Comparing `django-reaction-system-1.1.0/setup.cfg` & `django-reaction-system-1.1.1/setup.cfg`

 * *Files identical despite different names*

