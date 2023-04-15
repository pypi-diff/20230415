# Comparing `tmp/modProcesso-0.0.8.tar.gz` & `tmp/modProcesso-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modProcesso-0.0.8.tar", last modified: Sat Apr 15 03:42:39 2023, max compression
+gzip compressed data, was "modProcesso-0.0.9.tar", last modified: Sat Apr 15 04:01:59 2023, max compression
```

## Comparing `modProcesso-0.0.8.tar` & `modProcesso-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-04-15 03:42:39.908019 modProcesso-0.0.8/
--rw-rw-r--   0 yuri      (1000) yuri      (1000)     1069 2023-04-10 03:41:03.000000 modProcesso-0.0.8/LICENSE
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      802 2023-04-15 03:42:39.908019 modProcesso-0.0.8/PKG-INFO
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      351 2023-04-10 13:38:20.000000 modProcesso-0.0.8/README.md
-drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-04-15 03:42:39.860016 modProcesso-0.0.8/modProcesso/
--rw-rw-r--   0 yuri      (1000) yuri      (1000)       25 2023-04-10 03:28:38.000000 modProcesso-0.0.8/modProcesso/__init__.py
--rw-rw-r--   0 yuri      (1000) yuri      (1000)    69498 2023-04-15 03:42:07.000000 modProcesso-0.0.8/modProcesso/modProcesso.py
-drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-04-15 03:42:39.908019 modProcesso-0.0.8/modProcesso.egg-info/
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      802 2023-04-15 03:42:39.000000 modProcesso-0.0.8/modProcesso.egg-info/PKG-INFO
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      251 2023-04-15 03:42:39.000000 modProcesso-0.0.8/modProcesso.egg-info/SOURCES.txt
--rw-rw-r--   0 yuri      (1000) yuri      (1000)        1 2023-04-15 03:42:39.000000 modProcesso-0.0.8/modProcesso.egg-info/dependency_links.txt
--rw-rw-r--   0 yuri      (1000) yuri      (1000)       40 2023-04-15 03:42:39.000000 modProcesso-0.0.8/modProcesso.egg-info/requires.txt
--rw-rw-r--   0 yuri      (1000) yuri      (1000)       12 2023-04-15 03:42:39.000000 modProcesso-0.0.8/modProcesso.egg-info/top_level.txt
--rw-rw-r--   0 yuri      (1000) yuri      (1000)       38 2023-04-15 03:42:39.908019 modProcesso-0.0.8/setup.cfg
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      727 2023-04-15 03:42:15.000000 modProcesso-0.0.8/setup.py
+drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-04-15 04:01:59.513459 modProcesso-0.0.9/
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)     1069 2023-04-10 03:41:03.000000 modProcesso-0.0.9/LICENSE
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      802 2023-04-15 04:01:59.509459 modProcesso-0.0.9/PKG-INFO
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      351 2023-04-10 13:38:20.000000 modProcesso-0.0.9/README.md
+drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-04-15 04:01:59.265454 modProcesso-0.0.9/modProcesso/
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)       25 2023-04-10 03:28:38.000000 modProcesso-0.0.9/modProcesso/__init__.py
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)    69513 2023-04-15 04:00:16.000000 modProcesso-0.0.9/modProcesso/modProcesso.py
+drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-04-15 04:01:59.509459 modProcesso-0.0.9/modProcesso.egg-info/
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      802 2023-04-15 04:01:56.000000 modProcesso-0.0.9/modProcesso.egg-info/PKG-INFO
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      251 2023-04-15 04:01:56.000000 modProcesso-0.0.9/modProcesso.egg-info/SOURCES.txt
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)        1 2023-04-15 04:01:56.000000 modProcesso-0.0.9/modProcesso.egg-info/dependency_links.txt
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)       40 2023-04-15 04:01:56.000000 modProcesso-0.0.9/modProcesso.egg-info/requires.txt
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)       12 2023-04-15 04:01:56.000000 modProcesso-0.0.9/modProcesso.egg-info/top_level.txt
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)       38 2023-04-15 04:01:59.513459 modProcesso-0.0.9/setup.cfg
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      727 2023-04-15 04:01:29.000000 modProcesso-0.0.9/setup.py
```

### Comparing `modProcesso-0.0.8/LICENSE` & `modProcesso-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `modProcesso-0.0.8/PKG-INFO` & `modProcesso-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modProcesso
-Version: 0.0.8
+Version: 0.0.9
 Summary: modProcesso is a library for automata modularisation.
 Home-page: https://github.com/flavioyuri/modProcesso
 Author: Flávio Yuri de Sousa
 Author-email: flavioyuri22@gmail.com
 License: MIT
 Keywords: Theory of Computing,Automata Theory,Languages,Process Mining,Automata Decomposition,Process Modularisation
 Platform: UNKNOWN
```

### Comparing `modProcesso-0.0.8/modProcesso/modProcesso.py` & `modProcesso-0.0.9/modProcesso/modProcesso.py`

 * *Files 0% similar despite different names*

```diff
@@ -1603,17 +1603,17 @@
       display(textfreq)
 
     display(textSum)
 
     display(pd.DataFrame(resultadosBPMN,columns=["Referente à:", "Gateways","Tasks","Transições","Componentes"]))
 
 
-def comparacao(train, test, train_csv, test_csv, camMin=True, sRet=True, join=True):
+def comparacao(train, test, train_csv, test_csv, case_id, activity, timestamp, camMin=True, sRet=True, join=True):
   comparacaoBPMN = []
-  net, initial_marking, final_marking = pm4py.discover_petri_net_alpha(train, case_id_key='Case ID', activity_key="Activity", timestamp_key='Complete Timestamp')
+  net, initial_marking, final_marking = pm4py.discover_petri_net_alpha(train, case_id_key=case_id, activity_key=activity, timestamp_key=timestamp)
   fitness = pm4py.fitness_token_based_replay(test, net, initial_marking, final_marking)
   bpmn = to_bpmn.apply(net, initial_marking, final_marking)
   gateways, tasks, flows = countBPMN(bpmn)
   comparacaoBPMN.append([f"Alpha miner BPMN", gateways, tasks, flows, gateways+tasks, fitness])
 
   net, im, fm = pm4py.discover_petri_net_heuristics(train)
   fitness = pm4py.fitness_token_based_replay(test, net, im, fm)
```

### Comparing `modProcesso-0.0.8/modProcesso.egg-info/PKG-INFO` & `modProcesso-0.0.9/modProcesso.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modProcesso
-Version: 0.0.8
+Version: 0.0.9
 Summary: modProcesso is a library for automata modularisation.
 Home-page: https://github.com/flavioyuri/modProcesso
 Author: Flávio Yuri de Sousa
 Author-email: flavioyuri22@gmail.com
 License: MIT
 Keywords: Theory of Computing,Automata Theory,Languages,Process Mining,Automata Decomposition,Process Modularisation
 Platform: UNKNOWN
```

### Comparing `modProcesso-0.0.8/setup.py` & `modProcesso-0.0.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as arq:
   readme = arq.read()
 
 setup(
     name='modProcesso',
-    version='0.0.8',
+    version='0.0.9',
     license='MIT',
     author="Flávio Yuri de Sousa",
     author_email='flavioyuri22@gmail.com',
     packages=['modProcesso'],
     url='https://github.com/flavioyuri/modProcesso',
     description='''modProcesso is a library for automata modularisation.''',
     long_description=readme,
```

