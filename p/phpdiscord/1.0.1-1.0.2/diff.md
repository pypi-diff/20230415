# Comparing `tmp/phpdiscord-1.0.1.tar.gz` & `tmp/phpdiscord-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phpdiscord-1.0.1.tar", last modified: Fri Apr 14 14:42:45 2023, max compression
+gzip compressed data, was "phpdiscord-1.0.2.tar", last modified: Sat Apr 15 06:01:11 2023, max compression
```

## Comparing `phpdiscord-1.0.1.tar` & `phpdiscord-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-14 14:42:45.036392 phpdiscord-1.0.1/
--rw-rw----   0 root         (0) everybody  (9997)      221 2023-04-14 14:42:45.028392 phpdiscord-1.0.1/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     1439 2023-04-10 13:24:56.000000 phpdiscord-1.0.1/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-14 14:42:44.968392 phpdiscord-1.0.1/phpdiscord/
--rw-rw----   0 root         (0) everybody  (9997)     2296 2023-04-14 13:24:00.000000 phpdiscord-1.0.1/phpdiscord/phpdiscord.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-14 14:42:45.020392 phpdiscord-1.0.1/phpdiscord.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      221 2023-04-14 14:42:44.000000 phpdiscord-1.0.1/phpdiscord.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      179 2023-04-14 14:42:44.000000 phpdiscord-1.0.1/phpdiscord.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-14 14:42:44.000000 phpdiscord-1.0.1/phpdiscord.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       11 2023-04-14 14:42:44.000000 phpdiscord-1.0.1/phpdiscord.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-14 14:42:45.036392 phpdiscord-1.0.1/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      237 2023-04-14 14:42:04.000000 phpdiscord-1.0.1/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-15 06:01:11.789251 phpdiscord-1.0.2/
+-rw-rw----   0 root         (0) everybody  (9997)     2854 2023-04-15 06:01:11.757251 phpdiscord-1.0.2/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     2600 2023-04-15 06:00:34.000000 phpdiscord-1.0.2/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-15 06:01:11.701251 phpdiscord-1.0.2/phpdiscord/
+-rw-rw----   0 root         (0) everybody  (9997)     4222 2023-04-15 05:55:00.000000 phpdiscord-1.0.2/phpdiscord/phpdiscord.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-15 06:01:11.749251 phpdiscord-1.0.2/phpdiscord.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     2854 2023-04-15 06:01:11.000000 phpdiscord-1.0.2/phpdiscord.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      179 2023-04-15 06:01:11.000000 phpdiscord-1.0.2/phpdiscord.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-15 06:01:11.000000 phpdiscord-1.0.2/phpdiscord.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       11 2023-04-15 06:01:11.000000 phpdiscord-1.0.2/phpdiscord.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-15 06:01:11.793251 phpdiscord-1.0.2/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      334 2023-04-15 04:57:11.000000 phpdiscord-1.0.2/setup.py
```

