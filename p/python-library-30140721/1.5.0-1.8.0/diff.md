# Comparing `tmp/python-library-30140721-1.5.0.tar.gz` & `tmp/python-library-30140721-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-library-30140721-1.5.0.tar", last modified: Fri Apr 14 23:59:05 2023, max compression
+gzip compressed data, was "python-library-30140721-1.8.0.tar", last modified: Sat Apr 15 01:00:59 2023, max compression
```

## Comparing `python-library-30140721-1.5.0.tar` & `python-library-30140721-1.8.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 nainagupta   (501) staff       (20)        0 2023-04-14 23:59:05.614392 python-library-30140721-1.5.0/
--rw-r--r--   0 nainagupta   (501) staff       (20)      230 2023-04-14 23:59:05.614221 python-library-30140721-1.5.0/PKG-INFO
-drwxr-xr-x   0 nainagupta   (501) staff       (20)        0 2023-04-14 23:59:05.611631 python-library-30140721-1.5.0/linear/
--rw-rw-r--   0 nainagupta   (501) staff       (20)     6694 2023-04-14 23:07:12.000000 python-library-30140721-1.5.0/linear/CDLL.py
--rw-rw-r--   0 nainagupta   (501) staff       (20)     6207 2023-04-14 23:56:49.000000 python-library-30140721-1.5.0/linear/CSLL.py
--rw-rw-r--   0 nainagupta   (501) staff       (20)     6783 2023-04-14 22:49:14.000000 python-library-30140721-1.5.0/linear/DLL.py
--rw-rw-r--   0 nainagupta   (501) staff       (20)     2240 2023-04-14 22:47:58.000000 python-library-30140721-1.5.0/linear/LLQueue.py
--rw-rw-r--   0 nainagupta   (501) staff       (20)     2030 2023-04-14 22:47:44.000000 python-library-30140721-1.5.0/linear/LLStack.py
--rw-rw-r--   0 nainagupta   (501) staff       (20)     6338 2023-04-14 22:46:24.000000 python-library-30140721-1.5.0/linear/SLL.py
--rw-rw-r--   0 nainagupta   (501) staff       (20)        0 2023-04-14 22:42:42.000000 python-library-30140721-1.5.0/linear/__init__.py
-drwxr-xr-x   0 nainagupta   (501) staff       (20)        0 2023-04-14 23:59:05.612560 python-library-30140721-1.5.0/nodes/
--rw-rw-r--   0 nainagupta   (501) staff       (20)      120 2023-04-14 22:48:50.000000 python-library-30140721-1.5.0/nodes/DNode.py
--rw-rw-r--   0 nainagupta   (501) staff       (20)       94 2023-04-14 22:46:28.000000 python-library-30140721-1.5.0/nodes/SNode.py
--rw-r--r--   0 nainagupta   (501) staff       (20)     1407 2023-04-09 21:49:35.000000 python-library-30140721-1.5.0/nodes/Tnode.py
--rw-rw-r--   0 nainagupta   (501) staff       (20)        0 2023-04-14 22:42:42.000000 python-library-30140721-1.5.0/nodes/__init__.py
-drwxr-xr-x   0 nainagupta   (501) staff       (20)        0 2023-04-14 23:59:05.613272 python-library-30140721-1.5.0/python_library_30140721.egg-info/
--rw-r--r--   0 nainagupta   (501) staff       (20)      230 2023-04-14 23:59:05.000000 python-library-30140721-1.5.0/python_library_30140721.egg-info/PKG-INFO
--rw-r--r--   0 nainagupta   (501) staff       (20)      462 2023-04-14 23:59:05.000000 python-library-30140721-1.5.0/python_library_30140721.egg-info/SOURCES.txt
--rw-r--r--   0 nainagupta   (501) staff       (20)        1 2023-04-14 23:59:05.000000 python-library-30140721-1.5.0/python_library_30140721.egg-info/dependency_links.txt
--rw-r--r--   0 nainagupta   (501) staff       (20)       12 2023-04-14 23:59:05.000000 python-library-30140721-1.5.0/python_library_30140721.egg-info/requires.txt
--rw-r--r--   0 nainagupta   (501) staff       (20)       19 2023-04-14 23:59:05.000000 python-library-30140721-1.5.0/python_library_30140721.egg-info/top_level.txt
--rw-r--r--   0 nainagupta   (501) staff       (20)       38 2023-04-14 23:59:05.614449 python-library-30140721-1.5.0/setup.cfg
--rw-r--r--   0 nainagupta   (501) staff       (20)      376 2023-04-14 23:56:54.000000 python-library-30140721-1.5.0/setup.py
-drwxr-xr-x   0 nainagupta   (501) staff       (20)        0 2023-04-14 23:59:05.614008 python-library-30140721-1.5.0/trees/
--rw-r--r--   0 nainagupta   (501) staff       (20)     7870 2023-04-11 01:05:52.000000 python-library-30140721-1.5.0/trees/AVL.py
--rw-r--r--   0 nainagupta   (501) staff       (20)     3604 2023-04-11 01:12:13.000000 python-library-30140721-1.5.0/trees/BST.py
--rw-r--r--   0 nainagupta   (501) staff       (20)        0 2023-04-14 23:24:34.000000 python-library-30140721-1.5.0/trees/__init__.py
+drwxr-xr-x   0 nainagupta   (501) staff       (20)        0 2023-04-15 01:00:59.513850 python-library-30140721-1.8.0/
+-rw-r--r--   0 nainagupta   (501) staff       (20)      230 2023-04-15 01:00:59.513663 python-library-30140721-1.8.0/PKG-INFO
+drwxr-xr-x   0 nainagupta   (501) staff       (20)        0 2023-04-15 01:00:59.510528 python-library-30140721-1.8.0/linear/
+-rw-rw-r--   0 nainagupta   (501) staff       (20)     6694 2023-04-14 23:07:12.000000 python-library-30140721-1.8.0/linear/CDLL.py
+-rw-rw-r--   0 nainagupta   (501) staff       (20)     6207 2023-04-14 23:56:49.000000 python-library-30140721-1.8.0/linear/CSLL.py
+-rw-rw-r--   0 nainagupta   (501) staff       (20)     6783 2023-04-14 22:49:14.000000 python-library-30140721-1.8.0/linear/DLL.py
+-rw-rw-r--   0 nainagupta   (501) staff       (20)     2240 2023-04-14 22:47:58.000000 python-library-30140721-1.8.0/linear/LLQueue.py
+-rw-rw-r--   0 nainagupta   (501) staff       (20)     2030 2023-04-14 22:47:44.000000 python-library-30140721-1.8.0/linear/LLStack.py
+-rw-rw-r--   0 nainagupta   (501) staff       (20)     6338 2023-04-14 22:46:24.000000 python-library-30140721-1.8.0/linear/SLL.py
+-rw-rw-r--   0 nainagupta   (501) staff       (20)        0 2023-04-14 22:42:42.000000 python-library-30140721-1.8.0/linear/__init__.py
+drwxr-xr-x   0 nainagupta   (501) staff       (20)        0 2023-04-15 01:00:59.511688 python-library-30140721-1.8.0/nodes/
+-rw-rw-r--   0 nainagupta   (501) staff       (20)      120 2023-04-14 22:48:50.000000 python-library-30140721-1.8.0/nodes/DNode.py
+-rw-rw-r--   0 nainagupta   (501) staff       (20)       94 2023-04-14 22:46:28.000000 python-library-30140721-1.8.0/nodes/SNode.py
+-rw-r--r--   0 nainagupta   (501) staff       (20)     1407 2023-04-09 21:49:35.000000 python-library-30140721-1.8.0/nodes/Tnode.py
+-rw-rw-r--   0 nainagupta   (501) staff       (20)        0 2023-04-14 22:42:42.000000 python-library-30140721-1.8.0/nodes/__init__.py
+drwxr-xr-x   0 nainagupta   (501) staff       (20)        0 2023-04-15 01:00:59.512496 python-library-30140721-1.8.0/python_library_30140721.egg-info/
+-rw-r--r--   0 nainagupta   (501) staff       (20)      230 2023-04-15 01:00:59.000000 python-library-30140721-1.8.0/python_library_30140721.egg-info/PKG-INFO
+-rw-r--r--   0 nainagupta   (501) staff       (20)      462 2023-04-15 01:00:59.000000 python-library-30140721-1.8.0/python_library_30140721.egg-info/SOURCES.txt
+-rw-r--r--   0 nainagupta   (501) staff       (20)        1 2023-04-15 01:00:59.000000 python-library-30140721-1.8.0/python_library_30140721.egg-info/dependency_links.txt
+-rw-r--r--   0 nainagupta   (501) staff       (20)       12 2023-04-15 01:00:59.000000 python-library-30140721-1.8.0/python_library_30140721.egg-info/requires.txt
+-rw-r--r--   0 nainagupta   (501) staff       (20)       19 2023-04-15 01:00:59.000000 python-library-30140721-1.8.0/python_library_30140721.egg-info/top_level.txt
+-rw-r--r--   0 nainagupta   (501) staff       (20)       38 2023-04-15 01:00:59.513920 python-library-30140721-1.8.0/setup.cfg
+-rw-r--r--   0 nainagupta   (501) staff       (20)      376 2023-04-15 00:58:53.000000 python-library-30140721-1.8.0/setup.py
+drwxr-xr-x   0 nainagupta   (501) staff       (20)        0 2023-04-15 01:00:59.513424 python-library-30140721-1.8.0/trees/
+-rw-r--r--   0 nainagupta   (501) staff       (20)     7882 2023-04-15 00:57:58.000000 python-library-30140721-1.8.0/trees/AVL.py
+-rw-r--r--   0 nainagupta   (501) staff       (20)     3610 2023-04-15 00:58:20.000000 python-library-30140721-1.8.0/trees/BST.py
+-rw-r--r--   0 nainagupta   (501) staff       (20)        0 2023-04-14 23:24:34.000000 python-library-30140721-1.8.0/trees/__init__.py
```

### Comparing `python-library-30140721-1.5.0/linear/CDLL.py` & `python-library-30140721-1.8.0/linear/CDLL.py`

 * *Files identical despite different names*

### Comparing `python-library-30140721-1.5.0/linear/CSLL.py` & `python-library-30140721-1.8.0/linear/CSLL.py`

 * *Files identical despite different names*

### Comparing `python-library-30140721-1.5.0/linear/DLL.py` & `python-library-30140721-1.8.0/linear/DLL.py`

 * *Files identical despite different names*

### Comparing `python-library-30140721-1.5.0/linear/LLQueue.py` & `python-library-30140721-1.8.0/linear/LLQueue.py`

 * *Files identical despite different names*

### Comparing `python-library-30140721-1.5.0/linear/LLStack.py` & `python-library-30140721-1.8.0/linear/LLStack.py`

 * *Files identical despite different names*

### Comparing `python-library-30140721-1.5.0/linear/SLL.py` & `python-library-30140721-1.8.0/linear/SLL.py`

 * *Files identical despite different names*

### Comparing `python-library-30140721-1.5.0/nodes/Tnode.py` & `python-library-30140721-1.8.0/nodes/Tnode.py`

 * *Files identical despite different names*

### Comparing `python-library-30140721-1.5.0/trees/AVL.py` & `python-library-30140721-1.8.0/trees/AVL.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from Tnode import Tnode
-from BST import BST
+from nodes.Tnode import Tnode
+from trees.BST import BST
 
 
 class AVL(BST):
     def __init__(self, val=None, obj=None):
         super().__init__()
         if val is not None:
             self.root = Tnode(val)
```

### Comparing `python-library-30140721-1.5.0/trees/BST.py` & `python-library-30140721-1.8.0/trees/BST.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from Tnode import Tnode
+from nodes.Tnode import Tnode
 from collections import deque
 
 class BST:
 #Initilaizing data member
   def __init__(self, root = None):
     self.root = root
```

