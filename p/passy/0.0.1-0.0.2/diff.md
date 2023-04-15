# Comparing `tmp/passy-0.0.1.tar.gz` & `tmp/passy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\passy-0.0.1.tar", last modified: Wed Jan 20 16:45:56 2021, max compression
+gzip compressed data, was "passy-0.0.2.tar", last modified: Sat Apr 15 14:36:39 2023, max compression
```

## Comparing `passy-0.0.1.tar` & `passy-0.0.2.tar`

### file list

```diff
@@ -1,37 +1,4 @@
-drwxrwxrwx   0        0        0        0 2021-01-20 16:45:56.000000 passy-0.0.1/
--rw-rw-rw-   0        0        0    19634 2021-01-18 08:34:24.000000 passy-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      285 2021-01-20 16:42:50.000000 passy-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      918 2021-01-20 16:45:56.000000 passy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      490 2021-01-18 08:34:24.000000 passy-0.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2021-01-20 16:45:56.000000 passy-0.0.1/docs/
--rw-rw-rw-   0        0        0     3401 2021-01-20 16:24:03.000000 passy-0.0.1/docs/Documenation.rst
--rw-rw-rw-   0        0        0      326 2021-01-20 01:09:40.000000 passy-0.0.1/docs/Install.rst
--rw-rw-rw-   0        0        0      634 2021-01-20 00:50:57.000000 passy-0.0.1/docs/Makefile
--rw-rw-rw-   0        0        0     1686 2021-01-20 16:23:06.000000 passy-0.0.1/docs/Specification.rst
--rw-rw-rw-   0        0        0     1956 2021-01-20 01:02:58.000000 passy-0.0.1/docs/conf.py
--rw-rw-rw-   0        0        0      344 2021-01-20 16:45:14.000000 passy-0.0.1/docs/index.rst
--rwxrwxrwx   0        0        0      795 2021-01-20 00:50:57.000000 passy-0.0.1/docs/make.bat
--rw-rw-rw-   0        0        0       42 2021-01-20 16:45:56.000000 passy-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      828 2021-01-20 16:45:51.000000 passy-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2021-01-20 16:45:56.000000 passy-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2021-01-20 16:45:56.000000 passy-0.0.1/src/Passy.egg-info/
--rw-rw-rw-   0        0        0      918 2021-01-20 16:45:55.000000 passy-0.0.1/src/Passy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      677 2021-01-20 16:45:56.000000 passy-0.0.1/src/Passy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-01-20 16:45:55.000000 passy-0.0.1/src/Passy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2021-01-20 16:45:55.000000 passy-0.0.1/src/Passy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-01-20 16:45:56.000000 passy-0.0.1/src/internal/
--rw-rw-rw-   0        0        0      914 2021-01-20 16:17:54.000000 passy-0.0.1/src/internal/Encrypt.py
--rw-rw-rw-   0        0        0     2775 2021-01-20 16:18:03.000000 passy-0.0.1/src/passy.py
-drwxrwxrwx   0        0        0        0 2021-01-20 16:45:56.000000 passy-0.0.1/test/
-drwxrwxrwx   0        0        0        0 2021-01-20 16:45:56.000000 passy-0.0.1/test/Test_Data/
--rw-rw-rw-   0        0        0      446 2021-01-20 16:18:30.000000 passy-0.0.1/test/Test_Data/setup.py
--rw-rw-rw-   0        0        0      211 2021-01-18 08:34:31.000000 passy-0.0.1/test/Test_Data/test.txt
--rw-rw-rw-   0        0        0      540 2021-01-20 16:18:10.000000 passy-0.0.1/test/Test_Data/test1.json
--rw-rw-rw-   0        0        0      810 2021-01-20 16:18:10.000000 passy-0.0.1/test/Test_Data/test2.json
--rw-rw-rw-   0        0        0      932 2021-01-20 13:43:59.000000 passy-0.0.1/test/test_DunMethods.py
--rw-rw-rw-   0        0        0      775 2021-01-20 13:42:53.000000 passy-0.0.1/test/test_add.py
--rw-rw-rw-   0        0        0      579 2021-01-20 13:53:48.000000 passy-0.0.1/test/test_check.py
--rw-rw-rw-   0        0        0      503 2021-01-20 13:46:01.000000 passy-0.0.1/test/test_load.py
--rw-rw-rw-   0        0        0      431 2021-01-20 13:45:15.000000 passy-0.0.1/test/test_save.py
--rw-rw-rw-   0        0        0        0 2021-01-20 16:06:05.000000 passy-0.0.1/test.py
--rw-rw-rw-   0        0        0        2 2021-01-20 01:24:11.000000 passy-0.0.1/users.json
+-rw-r--r--   0        0        0     1067 2023-04-15 14:30:49.061192 passy-0.0.2/LICENSE
+-rw-r--r--   0        0        0       57 2023-04-15 14:30:16.196544 passy-0.0.2/passy/__init__.py
+-rw-r--r--   0        0        0      814 2023-04-15 14:36:38.692068 passy-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      676 1970-01-01 00:00:00.000000 passy-0.0.2/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

