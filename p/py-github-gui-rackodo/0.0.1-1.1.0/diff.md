# Comparing `tmp/py-github-gui-rackodo-0.0.1.tar.gz` & `tmp/py-github-gui-rackodo-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-github-gui-rackodo-0.0.1.tar", last modified: Mon Apr 10 10:25:17 2023, max compression
+gzip compressed data, was "py-github-gui-rackodo-1.1.0.tar", last modified: Sat Apr 15 15:48:02 2023, max compression
```

## Comparing `py-github-gui-rackodo-0.0.1.tar` & `py-github-gui-rackodo-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:25:17.911017 py-github-gui-rackodo-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-10 10:25:17.911017 py-github-gui-rackodo-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-10 10:25:03.000000 py-github-gui-rackodo-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:25:17.911017 py-github-gui-rackodo-0.0.1/py_github_gui/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-10 10:25:03.000000 py-github-gui-rackodo-0.0.1/py_github_gui/EntryWithPlaceholder.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 10:25:03.000000 py-github-gui-rackodo-0.0.1/py_github_gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-10 10:25:03.000000 py-github-gui-rackodo-0.0.1/py_github_gui/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 10:25:17.911017 py-github-gui-rackodo-0.0.1/py_github_gui_rackodo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-10 10:25:17.000000 py-github-gui-rackodo-0.0.1/py_github_gui_rackodo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-10 10:25:17.000000 py-github-gui-rackodo-0.0.1/py_github_gui_rackodo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 10:25:17.000000 py-github-gui-rackodo-0.0.1/py_github_gui_rackodo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-10 10:25:17.000000 py-github-gui-rackodo-0.0.1/py_github_gui_rackodo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-10 10:25:03.000000 py-github-gui-rackodo-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 10:25:17.911017 py-github-gui-rackodo-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:48:02.723165 py-github-gui-rackodo-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-04-15 15:48:02.723165 py-github-gui-rackodo-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-04-15 15:47:50.000000 py-github-gui-rackodo-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:48:02.723165 py-github-gui-rackodo-1.1.0/py_github_gui_rackodo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-04-15 15:48:02.000000 py-github-gui-rackodo-1.1.0/py_github_gui_rackodo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-15 15:48:02.000000 py-github-gui-rackodo-1.1.0/py_github_gui_rackodo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 15:48:02.000000 py-github-gui-rackodo-1.1.0/py_github_gui_rackodo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-15 15:48:02.000000 py-github-gui-rackodo-1.1.0/py_github_gui_rackodo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-15 15:48:02.000000 py-github-gui-rackodo-1.1.0/py_github_gui_rackodo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-15 15:47:50.000000 py-github-gui-rackodo-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 15:48:02.723165 py-github-gui-rackodo-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-15 15:47:50.000000 py-github-gui-rackodo-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:48:02.723165 py-github-gui-rackodo-1.1.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:47:50.000000 py-github-gui-rackodo-1.1.0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-04-15 15:47:50.000000 py-github-gui-rackodo-1.1.0/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   213773 2023-04-15 15:47:50.000000 py-github-gui-rackodo-1.1.0/src/placeholder.png
```

