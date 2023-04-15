# Comparing `tmp/modProcesso-0.0.6.tar.gz` & `tmp/modProcesso-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modProcesso-0.0.6.tar", last modified: Sat Apr 15 03:10:37 2023, max compression
+gzip compressed data, was "modProcesso-0.0.7.tar", last modified: Sat Apr 15 03:27:15 2023, max compression
```

## Comparing `modProcesso-0.0.6.tar` & `modProcesso-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-04-15 03:10:37.253281 modProcesso-0.0.6/
--rw-rw-r--   0 yuri      (1000) yuri      (1000)     1069 2023-04-10 03:41:03.000000 modProcesso-0.0.6/LICENSE
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      802 2023-04-15 03:10:37.249281 modProcesso-0.0.6/PKG-INFO
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      351 2023-04-10 13:38:20.000000 modProcesso-0.0.6/README.md
-drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-04-15 03:10:37.245281 modProcesso-0.0.6/modProcesso/
--rw-rw-r--   0 yuri      (1000) yuri      (1000)       25 2023-04-10 03:28:38.000000 modProcesso-0.0.6/modProcesso/__init__.py
--rw-rw-r--   0 yuri      (1000) yuri      (1000)    69563 2023-04-15 03:09:53.000000 modProcesso-0.0.6/modProcesso/modProcesso.py
-drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-04-15 03:10:37.249281 modProcesso-0.0.6/modProcesso.egg-info/
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      802 2023-04-15 03:10:36.000000 modProcesso-0.0.6/modProcesso.egg-info/PKG-INFO
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      251 2023-04-15 03:10:36.000000 modProcesso-0.0.6/modProcesso.egg-info/SOURCES.txt
--rw-rw-r--   0 yuri      (1000) yuri      (1000)        1 2023-04-15 03:10:36.000000 modProcesso-0.0.6/modProcesso.egg-info/dependency_links.txt
--rw-rw-r--   0 yuri      (1000) yuri      (1000)       40 2023-04-15 03:10:36.000000 modProcesso-0.0.6/modProcesso.egg-info/requires.txt
--rw-rw-r--   0 yuri      (1000) yuri      (1000)       12 2023-04-15 03:10:36.000000 modProcesso-0.0.6/modProcesso.egg-info/top_level.txt
--rw-rw-r--   0 yuri      (1000) yuri      (1000)       38 2023-04-15 03:10:37.253281 modProcesso-0.0.6/setup.cfg
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      727 2023-04-15 03:10:01.000000 modProcesso-0.0.6/setup.py
+drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-04-15 03:27:15.197912 modProcesso-0.0.7/
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)     1069 2023-04-10 03:41:03.000000 modProcesso-0.0.7/LICENSE
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      802 2023-04-15 03:27:15.193912 modProcesso-0.0.7/PKG-INFO
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      351 2023-04-10 13:38:20.000000 modProcesso-0.0.7/README.md
+drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-04-15 03:27:15.193912 modProcesso-0.0.7/modProcesso/
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)       25 2023-04-10 03:28:38.000000 modProcesso-0.0.7/modProcesso/__init__.py
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)    69550 2023-04-15 03:26:36.000000 modProcesso-0.0.7/modProcesso/modProcesso.py
+drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-04-15 03:27:15.193912 modProcesso-0.0.7/modProcesso.egg-info/
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      802 2023-04-15 03:27:14.000000 modProcesso-0.0.7/modProcesso.egg-info/PKG-INFO
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      251 2023-04-15 03:27:14.000000 modProcesso-0.0.7/modProcesso.egg-info/SOURCES.txt
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)        1 2023-04-15 03:27:14.000000 modProcesso-0.0.7/modProcesso.egg-info/dependency_links.txt
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)       40 2023-04-15 03:27:14.000000 modProcesso-0.0.7/modProcesso.egg-info/requires.txt
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)       12 2023-04-15 03:27:14.000000 modProcesso-0.0.7/modProcesso.egg-info/top_level.txt
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)       38 2023-04-15 03:27:15.197912 modProcesso-0.0.7/setup.cfg
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      727 2023-04-15 03:26:43.000000 modProcesso-0.0.7/setup.py
```

### Comparing `modProcesso-0.0.6/LICENSE` & `modProcesso-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `modProcesso-0.0.6/PKG-INFO` & `modProcesso-0.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modProcesso
-Version: 0.0.6
+Version: 0.0.7
 Summary: modProcesso is a library for automata modularisation.
 Home-page: https://github.com/flavioyuri/modProcesso
 Author: Flávio Yuri de Sousa
 Author-email: flavioyuri22@gmail.com
 License: MIT
 Keywords: Theory of Computing,Automata Theory,Languages,Process Mining,Automata Decomposition,Process Modularisation
 Platform: UNKNOWN
```

### Comparing `modProcesso-0.0.6/modProcesso/modProcesso.py` & `modProcesso-0.0.7/modProcesso/modProcesso.py`

 * *Files 0% similar despite different names*

```diff
@@ -1722,15 +1722,15 @@
     min = dfa.minimization()
     
 
 
     min = dfaToNfa(min)
     nfaResultado = operacaoSequencias(min, 3, 25)
     fit = fitnessAutomata(nfaResultado, test_csv, sRet, sRetTest=False)
-    bpmn = nfaBB_to_bpmn(nfaResultado, remGat=True)
+    bpmn = nfaBB_to_bpmn(nfaResultado)
     gateways, tasks, flows = countBPMN(bpmn)
     comparacaoBPMN.append(["Operação Sequencias min/max:3-25 estados DFA min caminhos mínimos", gateways, tasks, flows, gateways+tasks, fit])  
 
 
 
   outBPMN = widgets.Output()
   tabsBPMN = widgets.Tab(children=[outBPMN])
```

### Comparing `modProcesso-0.0.6/modProcesso.egg-info/PKG-INFO` & `modProcesso-0.0.7/modProcesso.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modProcesso
-Version: 0.0.6
+Version: 0.0.7
 Summary: modProcesso is a library for automata modularisation.
 Home-page: https://github.com/flavioyuri/modProcesso
 Author: Flávio Yuri de Sousa
 Author-email: flavioyuri22@gmail.com
 License: MIT
 Keywords: Theory of Computing,Automata Theory,Languages,Process Mining,Automata Decomposition,Process Modularisation
 Platform: UNKNOWN
```

### Comparing `modProcesso-0.0.6/setup.py` & `modProcesso-0.0.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as arq:
   readme = arq.read()
 
 setup(
     name='modProcesso',
-    version='0.0.6',
+    version='0.0.7',
     license='MIT',
     author="Flávio Yuri de Sousa",
     author_email='flavioyuri22@gmail.com',
     packages=['modProcesso'],
     url='https://github.com/flavioyuri/modProcesso',
     description='''modProcesso is a library for automata modularisation.''',
     long_description=readme,
```

