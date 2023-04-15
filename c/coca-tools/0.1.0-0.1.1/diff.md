# Comparing `tmp/coca_tools-0.1.0.tar.gz` & `tmp/coca_tools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coca_tools-0.1.0.tar", max compression
+gzip compressed data, was "coca_tools-0.1.1.tar", max compression
```

## Comparing `coca_tools-0.1.0.tar` & `coca_tools-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0        0 2023-04-15 03:11:37.654934 coca_tools-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-15 03:11:37.654896 coca_tools-0.1.0/cocatools/__init__.py
--rw-r--r--   0        0        0      472 2023-04-15 04:23:26.815220 coca_tools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      744 1970-01-01 00:00:00.000000 coca_tools-0.1.0/setup.py
--rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 coca_tools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-15 10:38:49.334085 coca_tools-0.1.1/README.md
+-rw-r--r--   0        0        0       52 2023-04-15 10:38:49.334085 coca_tools-0.1.1/cocatools/__init__.py
+-rw-r--r--   0        0        0      937 2023-04-15 10:38:49.334085 coca_tools-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 coca_tools-0.1.1/PKG-INFO
```

