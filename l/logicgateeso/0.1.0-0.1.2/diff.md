# Comparing `tmp/LogicGateESO-0.1.0.tar.gz` & `tmp/LogicGateESO-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LogicGateESO-0.1.0.tar", max compression
+gzip compressed data, was "LogicGateESO-0.1.2.tar", max compression
```

## Comparing `LogicGateESO-0.1.0.tar` & `LogicGateESO-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1066 2023-04-15 10:26:11.945774 LogicGateESO-0.1.0/LICENSE
--rw-r--r--   0        0        0    10796 2023-04-15 10:26:48.361498 LogicGateESO-0.1.0/logicgateeso/LogicGate.py
--rw-r--r--   0        0        0       22 2023-04-15 10:25:20.557992 LogicGateESO-0.1.0/logicgateeso/__init__.py
--rw-r--r--   0        0        0      558 2023-04-15 10:28:15.805820 LogicGateESO-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      559 2023-04-15 10:28:42.314187 LogicGateESO-0.1.0/setup.py
--rw-r--r--   0        0        0      303 2023-04-15 10:28:42.314510 LogicGateESO-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-15 10:26:11.945774 LogicGateESO-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4544 2023-04-15 10:25:54.690484 LogicGateESO-0.1.2/README.rst
+-rw-r--r--   0        0        0    10796 2023-04-15 10:26:48.361498 LogicGateESO-0.1.2/logicgateeso/LogicGate.py
+-rw-r--r--   0        0        0      727 2023-04-15 11:22:32.526636 LogicGateESO-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5413 2023-04-15 11:22:55.657191 LogicGateESO-0.1.2/setup.py
+-rw-r--r--   0        0        0     5274 2023-04-15 11:22:55.657788 LogicGateESO-0.1.2/PKG-INFO
```

### Comparing `LogicGateESO-0.1.0/LICENSE` & `LogicGateESO-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `LogicGateESO-0.1.0/logicgateeso/LogicGate.py` & `LogicGateESO-0.1.2/logicgateeso/LogicGate.py`

 * *Files identical despite different names*

