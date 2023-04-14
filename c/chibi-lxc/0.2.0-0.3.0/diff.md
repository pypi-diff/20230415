# Comparing `tmp/chibi_lxc-0.2.0.tar.gz` & `tmp/chibi_lxc-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chibi_lxc-0.2.0.tar", last modified: Wed Feb  9 18:52:01 2022, max compression
+gzip compressed data, was "chibi_lxc-0.3.0.tar", last modified: Fri Apr 14 23:01:59 2023, max compression
```

## Comparing `chibi_lxc-0.2.0.tar` & `chibi_lxc-0.3.0.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2022-02-09 18:52:01.935491 chibi_lxc-0.2.0/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      150 2020-04-05 18:46:40.000000 chibi_lxc-0.2.0/AUTHORS.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3550 2020-04-05 18:46:40.000000 chibi_lxc-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       89 2020-04-05 18:46:40.000000 chibi_lxc-0.2.0/HISTORY.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      470 2020-04-05 18:46:40.000000 chibi_lxc-0.2.0/LICENSE
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      262 2020-04-05 18:46:40.000000 chibi_lxc-0.2.0/MANIFEST.in
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3207 2022-02-09 18:52:01.935491 chibi_lxc-0.2.0/PKG-INFO
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1852 2022-01-27 11:41:26.000000 chibi_lxc-0.2.0/README.rst
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2022-02-09 18:52:01.918825 chibi_lxc-0.2.0/chibi_lxc/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      156 2022-02-09 18:51:54.000000 chibi_lxc-0.2.0/chibi_lxc/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     9519 2022-01-27 11:49:30.000000 chibi_lxc-0.2.0/chibi_lxc/cli.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      589 2020-04-15 21:08:43.000000 chibi_lxc-0.2.0/chibi_lxc/config.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)    10680 2022-02-09 18:29:47.000000 chibi_lxc-0.2.0/chibi_lxc/container.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2022-02-09 18:52:01.918825 chibi_lxc-0.2.0/chibi_lxc/file/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2020-04-09 06:20:36.000000 chibi_lxc-0.2.0/chibi_lxc/file/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1456 2020-04-12 16:07:34.000000 chibi_lxc-0.2.0/chibi_lxc/file/config.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2020-04-08 21:55:30.000000 chibi_lxc-0.2.0/chibi_lxc/snippets.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2022-02-09 18:52:01.918825 chibi_lxc-0.2.0/chibi_lxc.egg-info/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3207 2022-02-09 18:52:00.000000 chibi_lxc-0.2.0/chibi_lxc.egg-info/PKG-INFO
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      903 2022-02-09 18:52:00.000000 chibi_lxc-0.2.0/chibi_lxc.egg-info/SOURCES.txt
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        1 2022-02-09 18:52:00.000000 chibi_lxc-0.2.0/chibi_lxc.egg-info/dependency_links.txt
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       50 2022-02-09 18:52:00.000000 chibi_lxc-0.2.0/chibi_lxc.egg-info/entry_points.txt
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        1 2022-02-09 18:52:00.000000 chibi_lxc-0.2.0/chibi_lxc.egg-info/not-zip-safe
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       67 2022-02-09 18:52:00.000000 chibi_lxc-0.2.0/chibi_lxc.egg-info/requires.txt
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       10 2022-02-09 18:52:00.000000 chibi_lxc-0.2.0/chibi_lxc.egg-info/top_level.txt
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2022-02-09 18:52:01.932158 chibi_lxc-0.2.0/docs/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      610 2020-04-05 18:46:40.000000 chibi_lxc-0.2.0/docs/Makefile
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       28 2020-04-05 18:46:40.000000 chibi_lxc-0.2.0/docs/authors.rst
--rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)     4820 2020-04-05 18:46:40.000000 chibi_lxc-0.2.0/docs/conf.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       33 2020-04-05 18:46:40.000000 chibi_lxc-0.2.0/docs/contributing.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       28 2020-04-05 18:46:40.000000 chibi_lxc-0.2.0/docs/history.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      306 2020-04-05 18:46:40.000000 chibi_lxc-0.2.0/docs/index.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1126 2020-04-05 18:46:40.000000 chibi_lxc-0.2.0/docs/installation.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      771 2020-04-05 18:46:40.000000 chibi_lxc-0.2.0/docs/make.bat
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       27 2020-04-05 18:46:40.000000 chibi_lxc-0.2.0/docs/readme.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       73 2020-04-05 18:46:40.000000 chibi_lxc-0.2.0/docs/usage.rst
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      454 2022-02-09 18:52:01.935491 chibi_lxc-0.2.0/setup.cfg
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1239 2022-02-09 18:51:54.000000 chibi_lxc-0.2.0/setup.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2022-02-09 18:52:01.935491 chibi_lxc-0.2.0/tests/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       94 2021-03-29 17:31:32.000000 chibi_lxc-0.2.0/tests/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1292 2020-04-07 23:38:52.000000 chibi_lxc-0.2.0/tests/provision.py
-drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2022-02-09 18:52:01.935491 chibi_lxc-0.2.0/tests/scripts/
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2020-04-07 22:54:32.000000 chibi_lxc-0.2.0/tests/scripts/__init__.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       39 2022-02-09 18:28:18.000000 chibi_lxc-0.2.0/tests/scripts/asdf.sh
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       49 2020-04-07 22:58:05.000000 chibi_lxc-0.2.0/tests/scripts/script_test.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       34 2020-04-08 02:00:56.000000 chibi_lxc-0.2.0/tests/scripts/script_test.sh
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      507 2020-04-27 19:59:54.000000 chibi_lxc-0.2.0/tests/test_config.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3326 2022-01-27 11:27:42.000000 chibi_lxc-0.2.0/tests/test_container.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1369 2021-03-29 17:26:31.000000 chibi_lxc-0.2.0/tests/test_envars.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2565 2022-02-09 18:36:51.000000 chibi_lxc-0.2.0/tests/test_scripts.py
--rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1886 2021-03-29 17:30:36.000000 chibi_lxc-0.2.0/tests/test_status_scripts.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-14 23:01:59.892755 chibi_lxc-0.3.0/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      150 2020-04-05 18:46:40.000000 chibi_lxc-0.3.0/AUTHORS.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3550 2020-04-05 18:46:40.000000 chibi_lxc-0.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       89 2020-04-05 18:46:40.000000 chibi_lxc-0.3.0/HISTORY.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      470 2020-04-05 18:46:40.000000 chibi_lxc-0.3.0/LICENSE
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      262 2020-04-05 18:46:40.000000 chibi_lxc-0.3.0/MANIFEST.in
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2516 2023-04-14 23:01:59.892755 chibi_lxc-0.3.0/PKG-INFO
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1852 2022-01-27 11:41:26.000000 chibi_lxc-0.3.0/README.rst
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-14 23:01:59.882755 chibi_lxc-0.3.0/chibi_lxc/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      156 2023-04-14 23:01:46.000000 chibi_lxc-0.3.0/chibi_lxc/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)    10163 2023-04-14 21:40:19.000000 chibi_lxc-0.3.0/chibi_lxc/cli.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      589 2020-04-15 21:08:43.000000 chibi_lxc-0.3.0/chibi_lxc/config.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)    11342 2023-04-14 22:55:59.000000 chibi_lxc-0.3.0/chibi_lxc/container.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-14 23:01:59.882755 chibi_lxc-0.3.0/chibi_lxc/file/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2020-04-09 06:20:36.000000 chibi_lxc-0.3.0/chibi_lxc/file/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1456 2020-04-12 16:07:34.000000 chibi_lxc-0.3.0/chibi_lxc/file/config.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2020-04-08 21:55:30.000000 chibi_lxc-0.3.0/chibi_lxc/snippets.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-14 23:01:59.882755 chibi_lxc-0.3.0/chibi_lxc.egg-info/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2516 2023-04-14 23:01:59.000000 chibi_lxc-0.3.0/chibi_lxc.egg-info/PKG-INFO
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      918 2023-04-14 23:01:59.000000 chibi_lxc-0.3.0/chibi_lxc.egg-info/SOURCES.txt
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        1 2023-04-14 23:01:59.000000 chibi_lxc-0.3.0/chibi_lxc.egg-info/dependency_links.txt
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       49 2023-04-14 23:01:59.000000 chibi_lxc-0.3.0/chibi_lxc.egg-info/entry_points.txt
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        1 2023-04-14 23:01:59.000000 chibi_lxc-0.3.0/chibi_lxc.egg-info/not-zip-safe
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       67 2023-04-14 23:01:59.000000 chibi_lxc-0.3.0/chibi_lxc.egg-info/requires.txt
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       10 2023-04-14 23:01:59.000000 chibi_lxc-0.3.0/chibi_lxc.egg-info/top_level.txt
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-14 23:01:59.886089 chibi_lxc-0.3.0/docs/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      610 2020-04-05 18:46:40.000000 chibi_lxc-0.3.0/docs/Makefile
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       28 2020-04-05 18:46:40.000000 chibi_lxc-0.3.0/docs/authors.rst
+-rwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)     4820 2020-04-05 18:46:40.000000 chibi_lxc-0.3.0/docs/conf.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       33 2020-04-05 18:46:40.000000 chibi_lxc-0.3.0/docs/contributing.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       28 2020-04-05 18:46:40.000000 chibi_lxc-0.3.0/docs/history.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      306 2020-04-05 18:46:40.000000 chibi_lxc-0.3.0/docs/index.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1126 2020-04-05 18:46:40.000000 chibi_lxc-0.3.0/docs/installation.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      771 2020-04-05 18:46:40.000000 chibi_lxc-0.3.0/docs/make.bat
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       27 2020-04-05 18:46:40.000000 chibi_lxc-0.3.0/docs/readme.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       73 2020-04-05 18:46:40.000000 chibi_lxc-0.3.0/docs/usage.rst
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      454 2023-04-14 23:01:59.892755 chibi_lxc-0.3.0/setup.cfg
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1239 2023-04-14 23:01:46.000000 chibi_lxc-0.3.0/setup.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-14 23:01:59.886089 chibi_lxc-0.3.0/tests/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       94 2021-03-29 17:31:32.000000 chibi_lxc-0.3.0/tests/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2011 2023-04-14 22:47:38.000000 chibi_lxc-0.3.0/tests/mount.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1289 2023-04-14 21:52:17.000000 chibi_lxc-0.3.0/tests/provision.py
+drwxr-xr-x   0 dem4ply   (1000) dem4ply   (1000)        0 2023-04-14 23:01:59.892755 chibi_lxc-0.3.0/tests/scripts/
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)        0 2020-04-07 22:54:32.000000 chibi_lxc-0.3.0/tests/scripts/__init__.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       39 2022-02-09 18:28:18.000000 chibi_lxc-0.3.0/tests/scripts/asdf.sh
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       49 2020-04-07 22:58:05.000000 chibi_lxc-0.3.0/tests/scripts/script_test.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)       34 2020-04-08 02:00:56.000000 chibi_lxc-0.3.0/tests/scripts/script_test.sh
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)      507 2023-04-14 21:40:39.000000 chibi_lxc-0.3.0/tests/test_config.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     3323 2023-04-14 21:52:29.000000 chibi_lxc-0.3.0/tests/test_container.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1357 2023-04-14 21:52:52.000000 chibi_lxc-0.3.0/tests/test_envars.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     2547 2023-04-14 21:53:09.000000 chibi_lxc-0.3.0/tests/test_scripts.py
+-rw-r--r--   0 dem4ply   (1000) dem4ply   (1000)     1874 2023-04-14 21:53:18.000000 chibi_lxc-0.3.0/tests/test_status_scripts.py
```

### Comparing `chibi_lxc-0.2.0/CONTRIBUTING.rst` & `chibi_lxc-0.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `chibi_lxc-0.2.0/PKG-INFO` & `chibi_lxc-0.3.0/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,108 +1,81 @@
-Metadata-Version: 1.1
-Name: chibi_lxc
-Version: 0.2.0
-Summary: definition of lxc containers using python
-Home-page: https://github.com/dem4ply/chibi_lxc
-Author: dem4ply
-Author-email: dem4ply@gmail.com
-License: WTFPL
-Description: =========
-        chibi_lxc
-        =========
-        
-        
-        .. image:: https://img.shields.io/pypi/v/chibi_lxc.svg
-                :target: https://pypi.python.org/pypi/chibi_lxc
-        
-        .. image:: https://img.shields.io/travis/dem4ply/chibi_lxc.svg
-                :target: https://travis-ci.org/dem4ply/chibi_lxc
-        
-        .. image:: https://readthedocs.org/projects/chibi-lxc/badge/?version=latest
-                :target: https://chibi-lxc.readthedocs.io/en/latest/?badge=latest
-                :alt: Documentation Status
-        
-        definition of lxc containers using python class and manage lxc
-        similar to vagrant
-        
-        
-        Example
-        -------
-        
-        write a file with the container
-        
-        .. sourcecode:: python
-        
-        	from chibi_lxc import Container
-        	class Centos_8( Container ):
-        		name = 'centos_8'
-        		distribution = 'centos'
-        		arch = 'amd64'
-        		version = '8'
-        		provision_folders = { 'scripts': 'provision' }
-        		env_vars = { 'LC_ALL': 'es_MX.utf8' }
-        		scripts = ( 'install_python.sh', ( 'add_user.py', 'chibi', ) )
-        
-        write a config.py
-        
-        with the next conten
-        
-        .. sourcecode:: python
-        
-        	import sys
-        	from chibi.config import configuration
-        	from chibi.file import Chibi_path
-        	from chibi.module import import_
-        
-        	sys.path.append( Chibi_path( '.' ).inflate )
-        
-        	from containers.base import Centos_7
-        
-        
-        	configuration.chibi_lxc.containers.add( Centos_7 )
-        
-        
-        the scripts should be in the folder provision_folders[ 'scripts' ]
-        
-        
-        create the container
-        
-        ::
-        
-        	chibi_lxc up Centos_8 # create the container
-        	chibi_lxc provision Centos_8 # not needed the first time
-        	chibi_lxc list # lista los container configurados
-        	chibi_lxc status # lista el status de los container
-        	chibi_lxc host # lista el estado y hosts de los container
-        	chibi_lxc stop Centos_8 # stop the container
-        	chibi_lxc destroy Centos_8 # destroy the container
-        
-        
-        * Free software: WTFPL
-        * Documentation: https://chibi-lxc.readthedocs.io.
-        
-        
-        Features
-        --------
-        
-        * create container
-        * provision container
-        * destroy container
-        
-        
-        =======
-        History
-        =======
-        
-        0.0.1 (2020-04-05)
-        ------------------
-        
-        * First release on PyPI.
-        
-Keywords: chibi_lxc
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: Public Domain
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+=========
+chibi_lxc
+=========
+
+
+.. image:: https://img.shields.io/pypi/v/chibi_lxc.svg
+        :target: https://pypi.python.org/pypi/chibi_lxc
+
+.. image:: https://img.shields.io/travis/dem4ply/chibi_lxc.svg
+        :target: https://travis-ci.org/dem4ply/chibi_lxc
+
+.. image:: https://readthedocs.org/projects/chibi-lxc/badge/?version=latest
+        :target: https://chibi-lxc.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+definition of lxc containers using python class and manage lxc
+similar to vagrant
+
+
+Example
+-------
+
+write a file with the container
+
+.. sourcecode:: python
+
+	from chibi_lxc import Container
+	class Centos_8( Container ):
+		name = 'centos_8'
+		distribution = 'centos'
+		arch = 'amd64'
+		version = '8'
+		provision_folders = { 'scripts': 'provision' }
+		env_vars = { 'LC_ALL': 'es_MX.utf8' }
+		scripts = ( 'install_python.sh', ( 'add_user.py', 'chibi', ) )
+
+write a config.py
+
+with the next conten
+
+.. sourcecode:: python
+
+	import sys
+	from chibi.config import configuration
+	from chibi.file import Chibi_path
+	from chibi.module import import_
+
+	sys.path.append( Chibi_path( '.' ).inflate )
+
+	from containers.base import Centos_7
+
+
+	configuration.chibi_lxc.containers.add( Centos_7 )
+
+
+the scripts should be in the folder provision_folders[ 'scripts' ]
+
+
+create the container
+
+::
+
+	chibi_lxc up Centos_8 # create the container
+	chibi_lxc provision Centos_8 # not needed the first time
+	chibi_lxc list # lista los container configurados
+	chibi_lxc status # lista el status de los container
+	chibi_lxc host # lista el estado y hosts de los container
+	chibi_lxc stop Centos_8 # stop the container
+	chibi_lxc destroy Centos_8 # destroy the container
+
+
+* Free software: WTFPL
+* Documentation: https://chibi-lxc.readthedocs.io.
+
+
+Features
+--------
+
+* create container
+* provision container
+* destroy container
```

### Comparing `chibi_lxc-0.2.0/chibi_lxc/cli.py` & `chibi_lxc-0.3.0/chibi_lxc/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,19 +62,54 @@
         init_hosts_file()
         hosts_in_file = read_hosts()
     hosts_in_file.add( [ HostsEntry(
         entry_type='ipv4', address=address, names=list( hosts ) ) ] )
     hosts_in_file.write()
 
 
+def check_if_containers_exists_in_config( containers ):
+    result = True
+    for container in containers:
+        if container not in configuration.chibi_lxc.containers:
+            print( f"no se encontro {container}" )
+            result = False
+    return result
+
+
+def list_containers(  ):
+    containers = configuration.chibi_lxc.containers
+    padding = max( map( lambda k: len( k ), containers.keys() ) )
+    padding += 2
+    padding_ip = len( '255.255.255.255' ) + 2
+    space_ip = " " * padding_ip
+    group_container = group_by(
+        containers.values(), lambda c: c.__module__ )
+    for group, list_of_container in group_container.items():
+        print( group )
+        for container in list_of_container:
+            try:
+                if container.is_running:
+                    ip = container.info.ip
+                    print(
+                        f"\t{container.name:{padding}} "
+                        f"{ip:{padding_ip}} {container}" )
+                else:
+                    print(
+                        f"\t{container.name:{padding}} "
+                        f"{space_ip} {container}" )
+            except Not_exists_error:
+                print(
+                    f"\t{container.name:{padding}}{space_ip} {container}" )
+
+
 def main():
     parser = argparse.ArgumentParser(
         "tool for build containers" )
     parser.add_argument(
-        "--log_level", dest="log_level", default="INFO",
+        "--log_level", dest="log_level", default='INFO',
         help="nivel de log", )
 
     parser.add_argument(
         "--config", type=Chibi_path, default=Chibi_path( 'config.py' ),
         help="python, yaml o json archivo con los settings" )
 
     sub_parsers = parser.add_subparsers(
@@ -140,42 +175,26 @@
         'host', help='update the host file', )
     parser_host.add_argument(
         "--update", "-u", action="store_true",
         help="actualiza el archivo de hosts en /etc/hosts" )
 
     args = parser.parse_args()
     basic_config( level=args.log_level )
+    if not args.config.exists:
+        logger.error( f"no se encontro el config {args.config}" )
+        return
     load_config( args.config )
 
     if args.command == 'list':
-        containers = configuration.chibi_lxc.containers
-        padding = max( map( lambda k: len( k ), containers.keys() ) )
-        padding += 2
-        padding_ip = len( '255.255.255.255' ) + 2
-        space_ip = " " * padding_ip
-        group_container = group_by(
-            containers.values(), lambda c: c.__module__ )
-        for group, list_of_container in group_container.items():
-            print( group )
-            for container in list_of_container:
-                try:
-                    if container.is_running:
-                        ip = container.info.ip
-                        print(
-                            f"\t{container.name:{padding}} "
-                            f"{ip:{padding_ip}} {container}" )
-                    else:
-                        print(
-                            f"\t{container.name:{padding}} "
-                            f"{space_ip} {container}" )
-                except Not_exists_error:
-                    print( f"\t{container.name:{padding}} {space_ip} {container}" )
+        list_containers()
 
     if args.command == 'up':
         containers = configuration.chibi_lxc.containers
+        if not check_if_containers_exists_in_config( args.containers ):
+            return 1
         for container in args.containers:
             container = containers[ container ]
             exists = container.exists
             if not exists:
                 container.create()
             container.provision()
             container.start()
@@ -183,14 +202,16 @@
             add_address_to_host( ip, *container.hosts )
             if not exists:
                 container.provision()
                 container.run_scripts()
 
     if args.command == 'provision':
         containers = configuration.chibi_lxc.containers
+        if not check_if_containers_exists_in_config( args.containers ):
+            return 1
         for container in args.containers:
             if args.only_files:
                 container = containers[ container ]
                 container.provision()
             else:
                 container = containers[ container ]
                 container.provision()
@@ -198,14 +219,16 @@
                 time.sleep( 10 )
                 add_address_to_host( container.info.ip, *container.hosts )
                 container.provision()
                 container.run_scripts()
 
     if args.command == 'status':
         containers = configuration.chibi_lxc.containers
+        if not check_if_containers_exists_in_config( args.containers ):
+            return 1
         for container in args.containers:
             print( container )
             container = containers[ container ]
             if args.scripts:
                 print()
                 container.run_status_scripts()
             else:
```

### Comparing `chibi_lxc-0.2.0/chibi_lxc/config.py` & `chibi_lxc-0.3.0/chibi_lxc/config.py`

 * *Files identical despite different names*

### Comparing `chibi_lxc-0.2.0/chibi_lxc/container.py` & `chibi_lxc-0.3.0/chibi_lxc/container.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 class Destruction_error( Exception ):
     pass
 
 
 class Container_meta( type ):
     def __new__( cls, clsname, bases, clsdict ):
         clsobj = super().__new__( cls, clsname, bases, clsdict )
+
         if isinstance( clsobj.provision_folders, dict ):
             for k, v in clsobj.provision_folders.items():
                 clsobj.provision_folders[k] = Chibi_path( v )
 
         containers = list(
             filter( lambda x: issubclass( x, Container ), bases ) )
         containers_with_env_vars = list(
@@ -110,20 +111,21 @@
             cls_obj.status_scripts = tuple( status_scripts )
         else:
             cls_obj.status_scripts = status_scripts
 
 
 class Container( metaclass=Container_meta ):
     name = "unset"
-    distribution = 'centos'
+    distribution = 'rockylinux'
     arch = 'amd64'
     version = '8'
 
     provision_root = Chibi_path( 'home/chibi/provision/' )
     provision_folders = Chibi_atlas()
+    mounts = Chibi_atlas()
     scripts = None
     status_scripts = None
     extra_hosts = None
 
     delegate = True
 
     env_vars = Chibi_atlas( {
@@ -168,14 +170,19 @@
     @Class_property
     def provision_folder( cls ):
         return Chibi_atlas( {
             k: cls.root + '..' + k
             for k, v in cls.provision_folders.items() } )
 
     @Class_property
+    def mount( cls ):
+        config = cls.config.open().read()
+        return config.lxc.mount
+
+    @Class_property
     def script_folder( cls ):
         return '/' + cls.provision_root + 'scripts/'
 
     @Class_property
     def is_running( cls ):
         return cls.info.state == 'running'
 
@@ -217,47 +224,62 @@
             raise Destruction_error(
                 "un error en la destruscion del contenedor"
                 f" '{result.return_code}' revise los output" )
         return result
 
     @classmethod
     def provision( cls ):
-        config = cls.config.open().read()
         hosts = configuration.chibi_lxc.hosts
 
+        for mount_entry in cls.mounts:
+            cls.add_mount_entry( mount_entry )
+
         for k, v in cls.provision_folders.items():
             real_folder = cls.provision_folder[k]
             mount = (
                 f"{real_folder}  {cls.provision_root}/{k} "
                 "none bind,create=dir 0 0" )
 
-            if "mount" not in config.lxc:
-                config.lxc.mount = Chibi_atlas( entry=[] )
-            entries = config.lxc.mount.entry
-            if not isinstance( entries, list ):
-                entries = [ entries ]
-            for entry in entries:
-                if entry == mount:
-                    break
-            else:
-                entries.append( mount )
-                cls.config.open().write( config )
-                config = cls.config.open().read()
+            cls.add_mount_entry( mount )
 
-            if not real_folder.exists:
-                real_folder.mkdir()
             if v.is_a_folder and not v.endswith( '/' ):
                 v = str( v ) + '/'
-            if not real_folder.exists:
-                real_folder.mkdir()
             Rsync.clone_dir().human().verbose().run(
                 v, real_folder )
             if hosts and hosts.exists:
                 hosts.copy( real_folder + 'hosts' )
 
+    @classmethod
+    def add_mount_entry( cls, mount_entry ):
+        if not isinstance( mount_entry, str ):
+            raise NotImplementedError(
+                "no esta implementado mandar un mount.entry "
+                "que no es un string" )
+
+        config = cls.config.open().read()
+        if "mount" not in config.lxc:
+            config.lxc.mount = Chibi_atlas( entry=[] )
+        entries = config.lxc.mount.entry
+        if not isinstance( entries, list ):
+            config.lxc.mount.entry = [ config.lxc.mount.entry ]
+            entries = config.lxc.mount.entry
+
+        mount_entry = mount_entry.replace( '$USER', os.environ[ 'USER' ] )
+        if mount_entry not in entries:
+            entries.append( mount_entry )
+            cls.config.open().write( config )
+        else:
+            logger.warning(
+                f'el mount.entry "{mount_entry}" ya se '
+                'encontraba en el config' )
+
+        real_folder = Chibi_path( mount_entry.split( ' ', 1 )[0] )
+        if not real_folder.exists:
+            real_folder.mkdir()
+
     @Class_property
     def hosts( cls ):
         if cls.extra_hosts:
             return [ cls.name, *cls.extra_hosts ]
         return [ cls.name ]
 
     @classmethod
```

### Comparing `chibi_lxc-0.2.0/chibi_lxc/file/config.py` & `chibi_lxc-0.3.0/chibi_lxc/file/config.py`

 * *Files identical despite different names*

### Comparing `chibi_lxc-0.2.0/chibi_lxc.egg-info/SOURCES.txt` & `chibi_lxc-0.3.0/chibi_lxc.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 tests/__init__.py
+tests/mount.py
 tests/provision.py
 tests/test_config.py
 tests/test_container.py
 tests/test_envars.py
 tests/test_scripts.py
 tests/test_status_scripts.py
 tests/scripts/__init__.py
```

### Comparing `chibi_lxc-0.2.0/docs/Makefile` & `chibi_lxc-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chibi_lxc-0.2.0/docs/conf.py` & `chibi_lxc-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `chibi_lxc-0.2.0/docs/installation.rst` & `chibi_lxc-0.3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `chibi_lxc-0.2.0/docs/make.bat` & `chibi_lxc-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `chibi_lxc-0.2.0/setup.py` & `chibi_lxc-0.3.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,10 +36,10 @@
     license="WTFPL",
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='chibi_lxc',
     name='chibi_lxc',
     packages=find_packages(include=['chibi_lxc', 'chibi_lxc.*']),
     url='https://github.com/dem4ply/chibi_lxc',
-    version='0.2.0',
+    version='0.3.0',
     zip_safe=False,
 )
```

### Comparing `chibi_lxc-0.2.0/tests/provision.py` & `chibi_lxc-0.3.0/tests/provision.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from chibi.atlas import Chibi_atlas
 from chibi.file import Chibi_path
 import unittest
 from chibi_lxc.container import Container, Not_exists_error
 
 
 class Centos_test( Container ):
-    name = 'centos_7_test'
+    name = 'rocky_test'
     provision_folders = {
         'scripts': 'tests/scripts'
     }
 
 
 class Test_provision( unittest.TestCase ):
     @classmethod
```

### Comparing `chibi_lxc-0.2.0/tests/test_container.py` & `chibi_lxc-0.3.0/tests/test_container.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 class Unexisting_container( Container ):
     name = 'this container should no exists'
 
 
 class Centos_test( Container ):
-    name = 'centos_7_test'
+    name = 'rocky_test'
 
 
 class Centos_test_auto_rename( Centos_test ):
     pass
 
 
 class Centos_hosts_extra( Centos_test ):
```

### Comparing `chibi_lxc-0.2.0/tests/test_envars.py` & `chibi_lxc-0.3.0/tests/test_envars.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import unittest
 from chibi_lxc.container import Container
 
 
 class Centos_test( Container ):
-    name = 'centos_7_test'
+    name = 'rocky_test'
     env_vars = {
         'envar': 'test_1'
     }
 
 
 class Centos_one_test( Centos_test ):
-    name = 'centos_7_test'
+    name = 'rocky_test'
     env_vars = {
         'envar': 'test_1_1'
     }
 
 
 class Centos_two_test( Centos_one_test ):
-    name = 'centos_7_test'
+    name = 'rocky_test'
     env_vars = {
         'envar2': 'test_2'
     }
 
 
 class Centos_child( Centos_two_test ):
-    name = 'centos_7_test'
+    name = 'rocky_test'
     env_vars = {
         'envar2': 'test_2_2'
     }
 
 
 class Test_envars( unittest.TestCase ):
```

### Comparing `chibi_lxc-0.2.0/tests/test_scripts.py` & `chibi_lxc-0.3.0/tests/test_scripts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import unittest
 from chibi_lxc.container import Container
 
 
 class Centos_test( Container ):
-    name = 'centos_7_test'
+    name = 'rocky_test'
     provision_folders = {
         'scripts': 'tests/scripts/'
     }
     scripts = (
         'script_test.sh',
     )
 
 
 class Centos_test_cls_script( Container ):
-    name = 'centos_7_test'
+    name = 'rocky_test'
     some_script = 'asdf.sh'
     provision_folders = {
         'scripts': 'tests/scripts/'
     }
     scripts = (
         'cls.some_script',
     )
 
 class Centos_test_cls_script_params( Container ):
-    name = 'centos_7_test'
+    name = 'rocky_test'
     some_script = 'asdf.sh'
     provision_folders = {
         'scripts': 'tests/scripts/'
     }
     scripts = (
         ( 'cls.some_script', 'asdf' ),
     )
 
 
 class Centos_one_test( Centos_test ):
-    name = 'centos_7_test'
+    name = 'rocky_test'
     provision_folders = {
         'scripts': 'tests/scripts/'
     }
     scripts = (
         ( 'tuple_script.sh', 'asdfsadfasfd' )
     )
 
 
 class Centos_two_test( Centos_one_test ):
-    name = 'centos_7_test'
+    name = 'rocky_test'
     provision_folders = {
         'scripts': 'tests/scripts/'
     }
 
 
 class Centos_child( Centos_test ):
-    name = 'centos_7_test'
+    name = 'rocky_test'
     provision_folders = {
         'scripts': 'tests/scripts/'
     }
     scripts = (
         'another.sh',
     )
```

### Comparing `chibi_lxc-0.2.0/tests/test_status_scripts.py` & `chibi_lxc-0.3.0/tests/test_status_scripts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import unittest
 from chibi_lxc.container import Container
 
 
 class Centos_test( Container ):
-    name = 'centos_7_test'
+    name = 'rocky_test'
     provision_folders = {
         'scripts': 'tests/scripts/'
     }
     status_scripts = (
         'script_test.sh',
     )
 
 
 class Centos_one_test( Centos_test ):
-    name = 'centos_7_test'
+    name = 'rocky_test'
     provision_folders = {
         'scripts': 'tests/scripts/'
     }
     status_scripts = (
         ( 'tuple_script.sh', 'asdfsadfasfd' )
     )
 
 
 class Centos_two_test( Centos_one_test ):
-    name = 'centos_7_test'
+    name = 'rocky_test'
     provision_folders = {
         'scripts': 'tests/scripts/'
     }
 
 
 class Centos_child( Centos_test ):
-    name = 'centos_7_test'
+    name = 'rocky_test'
     provision_folders = {
         'scripts': 'tests/scripts/'
     }
     status_scripts = (
         'another.sh',
     )
```

