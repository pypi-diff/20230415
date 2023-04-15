# Comparing `tmp/modProcesso-0.0.4.tar.gz` & `tmp/modProcesso-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modProcesso-0.0.4.tar", last modified: Fri Apr 14 23:59:53 2023, max compression
+gzip compressed data, was "modProcesso-0.0.5.tar", last modified: Sat Apr 15 02:45:56 2023, max compression
```

## Comparing `modProcesso-0.0.4.tar` & `modProcesso-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-04-14 23:59:53.005733 modProcesso-0.0.4/
--rw-rw-r--   0 yuri      (1000) yuri      (1000)     1069 2023-04-10 03:41:03.000000 modProcesso-0.0.4/LICENSE
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      802 2023-04-14 23:59:53.005733 modProcesso-0.0.4/PKG-INFO
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      351 2023-04-10 13:38:20.000000 modProcesso-0.0.4/README.md
-drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-04-14 23:59:52.997732 modProcesso-0.0.4/modProcesso/
--rw-rw-r--   0 yuri      (1000) yuri      (1000)       25 2023-04-10 03:28:38.000000 modProcesso-0.0.4/modProcesso/__init__.py
--rw-rw-r--   0 yuri      (1000) yuri      (1000)    64058 2023-04-14 23:54:34.000000 modProcesso-0.0.4/modProcesso/modProcesso.py
-drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-04-14 23:59:53.005733 modProcesso-0.0.4/modProcesso.egg-info/
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      802 2023-04-14 23:59:51.000000 modProcesso-0.0.4/modProcesso.egg-info/PKG-INFO
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      251 2023-04-14 23:59:51.000000 modProcesso-0.0.4/modProcesso.egg-info/SOURCES.txt
--rw-rw-r--   0 yuri      (1000) yuri      (1000)        1 2023-04-14 23:59:51.000000 modProcesso-0.0.4/modProcesso.egg-info/dependency_links.txt
--rw-rw-r--   0 yuri      (1000) yuri      (1000)       40 2023-04-14 23:59:51.000000 modProcesso-0.0.4/modProcesso.egg-info/requires.txt
--rw-rw-r--   0 yuri      (1000) yuri      (1000)       12 2023-04-14 23:59:51.000000 modProcesso-0.0.4/modProcesso.egg-info/top_level.txt
--rw-rw-r--   0 yuri      (1000) yuri      (1000)       38 2023-04-14 23:59:53.005733 modProcesso-0.0.4/setup.cfg
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      727 2023-04-14 23:54:50.000000 modProcesso-0.0.4/setup.py
+drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-04-15 02:45:56.325354 modProcesso-0.0.5/
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)     1069 2023-04-10 03:41:03.000000 modProcesso-0.0.5/LICENSE
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      802 2023-04-15 02:45:56.325354 modProcesso-0.0.5/PKG-INFO
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      351 2023-04-10 13:38:20.000000 modProcesso-0.0.5/README.md
+drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-04-15 02:45:56.293355 modProcesso-0.0.5/modProcesso/
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)       25 2023-04-10 03:28:38.000000 modProcesso-0.0.5/modProcesso/__init__.py
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)    69125 2023-04-15 02:38:16.000000 modProcesso-0.0.5/modProcesso/modProcesso.py
+drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-04-15 02:45:56.325354 modProcesso-0.0.5/modProcesso.egg-info/
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      802 2023-04-15 02:45:54.000000 modProcesso-0.0.5/modProcesso.egg-info/PKG-INFO
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      251 2023-04-15 02:45:54.000000 modProcesso-0.0.5/modProcesso.egg-info/SOURCES.txt
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)        1 2023-04-15 02:45:54.000000 modProcesso-0.0.5/modProcesso.egg-info/dependency_links.txt
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)       40 2023-04-15 02:45:54.000000 modProcesso-0.0.5/modProcesso.egg-info/requires.txt
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)       12 2023-04-15 02:45:54.000000 modProcesso-0.0.5/modProcesso.egg-info/top_level.txt
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)       38 2023-04-15 02:45:56.325354 modProcesso-0.0.5/setup.cfg
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      727 2023-04-15 02:38:22.000000 modProcesso-0.0.5/setup.py
```

### Comparing `modProcesso-0.0.4/LICENSE` & `modProcesso-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `modProcesso-0.0.4/PKG-INFO` & `modProcesso-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modProcesso
-Version: 0.0.4
+Version: 0.0.5
 Summary: modProcesso is a library for automata modularisation.
 Home-page: https://github.com/flavioyuri/modProcesso
 Author: Flávio Yuri de Sousa
 Author-email: flavioyuri22@gmail.com
 License: MIT
 Keywords: Theory of Computing,Automata Theory,Languages,Process Mining,Automata Decomposition,Process Modularisation
 Platform: UNKNOWN
```

### Comparing `modProcesso-0.0.4/modProcesso/modProcesso.py` & `modProcesso-0.0.5/modProcesso/modProcesso.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,19 @@
 from pm4py.objects.conversion.log import converter as log_converter
 from pm4py.visualization.bpmn import visualizer as bpmn_visualizer
 from pm4py.objects.conversion.wf_net import converter as wf_converter
 import csv
 from os import write
 from pm4py.objects.log.importer.xes import importer as xes_importer
 from pm4py.objects.conversion.log import converter as xes_converter
+from pm4py.objects.conversion.wf_net.variants import to_bpmn
+from pm4py.algo.discovery.inductive import algorithm as inductive_miner    
+from pm4py.visualization.bpmn import visualizer as bpmn_visualizer
+from pm4py.visualization.process_tree import visualizer as pt_visualizer
+from pm4py.objects.conversion.process_tree import converter as pt_converter
 import ipywidgets as widgets
 import matplotlib.pyplot as plt
 
 ### Funções em comum
 
 
 ######Funções necessárias para encontrar subprocessos
@@ -1578,8 +1583,150 @@
       display(textfreq)
 
     display(textSum)
 
     display(pd.DataFrame(resultadosBPMN,columns=["Referente à:", "Gateways","Tasks","Transições","Componentes"]))
 
 
+def comparacao(train, test, train_csv, test_csv, camMin=True, sRet=True, join=True):
+  comparacaoBPMN = []
+  net, initial_marking, final_marking = pm4py.discover_petri_net_alpha(train, case_id_key='Case ID', activity_key="Activity", timestamp_key='Complete Timestamp')
+  fitness = pm4py.fitness_token_based_replay(test, net, initial_marking, final_marking)
+  bpmn = to_bpmn.apply(net, initial_marking, final_marking)
+  gateways, tasks, flows = countBPMN(bpmn)
+  comparacaoBPMN.append([f"Alpha miner BPMN", gateways, tasks, flows, gateways+tasks, fitness])
+
+  net, im, fm = pm4py.discover_petri_net_heuristics(train)
+  fitness = pm4py.fitness_token_based_replay(test, net, im, fm)
+  bpmn = to_bpmn.apply(net, im, fm)
+  gateways, tasks, flows = countBPMN(bpmn)
+  comparacaoBPMN.append([f"Heuristic miner BPMN", gateways, tasks, flows, gateways+tasks, fitness])
+
+  tree = pm4py.discovery.discover_process_tree_inductive(train)   
+  bpmn_graph = pt_converter.apply(tree, variant=pt_converter.Variants.TO_BPMN)
+  net, im, fm = pm4py.convert_to_petri_net(tree)
+  fitness = pm4py.fitness_token_based_replay(test, net, im, fm)
+  gateways, tasks, flows = countBPMN(bpmn_graph)
+  comparacaoBPMN.append([f"Inductive miner BPMN", gateways, tasks, flows, gateways+tasks, fitness])
+
+  if join:
+    if sRet:
+      nfaJoinFalse = to_nfa_minimum_path_join_traces(train_csv, rework=False)
+      
+      
+      dfaJoinFalse = nfaJoinFalse.determinization()
+      
+
+
+      minJoinFalse= dfaJoinFalse.minimization()
+      minJoinFalse.rename()
+      
+
+
+      min = dfaToNfa(minJoinFalse)
+      nfaResultado= operacaoSequencias(min, 3, 25)
+      fit = fitnessAutomata(nfaResultado, test_csv, sRet, sRetTest=False)
+      bpmn = nfaBB_to_bpmn(nfaResultado, remGat=True)
+      gateways, tasks, flows = countBPMN(bpmn)
+      comparacaoBPMN.append(["Operação Sequencias min/max:3-25 estados DFA min sem retrabalho join", gateways, tasks, flows, gateways+tasks, fit])
+    else:
+      nfaJoin = to_nfa_minimum_path_join_traces(train_csv, rework=True)
+      
+      
+      dfaJoin = nfaJoin.determinization()
+      
+
+
+      minJoin= dfaJoin.minimization()
+      minJoin.rename()
+      
+
+
+      min = dfaToNfa(minJoin)
+      nfaResultado= operacaoSequencias(min, 3, 25)
+      fit = fitnessAutomata(nfaResultado, test_csv, sRet, sRetTest=False)
+      bpmn = nfaBB_to_bpmn(nfaResultado, remGat=True)
+      gateways, tasks, flows = countBPMN(bpmn)
+      comparacaoBPMN.append(["Operação Sequencias min/max:3-25 estados DFA min join", gateways, tasks, flows, gateways+tasks, fit])
+    
+
+  elif camMin:
+    if sRet:
+      nfaCamMin = to_nfa_minimum_path(train_csv, rework=False, nfa_bb=False)
+
+      
+
+      dfa = nfaCamMin.determinization()
+      
+
+
+      min = dfa.minimization()
+      
+
+
+      min = dfaToNfa(min)
+      nfaResultado = operacaoSequencias(min, 3, 25)
+      fit = fitnessAutomata(nfaResultado, test_csv, sRet, sRetTest=False)
+      bpmn = nfaBB_to_bpmn(nfaResultado, remGat=True)
+      gateways, tasks, flows = countBPMN(bpmn)
+      comparacaoBPMN.append(["Operação Sequencias min/max:3-25 estados DFA min caminhos mínimos s retrabalho", gateways, tasks, flows, gateways+tasks, fit])  
+
+    else:
+      nfaCamMin = to_nfa_minimum_path(train_csv, nfa_bb=False)
+
+      
+
+      dfa = nfaCamMin.determinization()
+      
+
+
+      min = dfa.minimization()
+      
+
+
+      min = dfaToNfa(min)
+      nfaResultado = operacaoSequencias(min, 3, 25)
+      fit = fitnessAutomata(nfaResultado, test_csv, sRet, sRetTest=False)
+      bpmn = nfaBB_to_bpmn(nfaResultado, remGat=True)
+      gateways, tasks, flows = countBPMN(bpmn)
+      comparacaoBPMN.append(["Operação Sequencias min/max:3-25 estados DFA min caminhos mínimos", gateways, tasks, flows, gateways+tasks, fit])  
+
+  else: 
+    nfa = to_nfa(train_csv)
+
+    
+
+    dfa = nfa.determinization()
+    
+
+
+    min = dfa.minimization()
+    
+
+
+    min = dfaToNfa(min)
+    nfaResultado = operacaoSequencias(min, 3, 25)
+    fit = fitnessAutomata(nfaResultado, test_csv, sRet, sRetTest=False)
+    bpmn = nfaBB_to_bpmn(nfaResultado, remGat=True)
+    gateways, tasks, flows = countBPMN(bpmn)
+    comparacaoBPMN.append(["Operação Sequencias min/max:3-25 estados DFA min caminhos mínimos", gateways, tasks, flows, gateways+tasks, fit])  
+
+
+
+  outBPMN = widgets.Output()
+  tabsBPMN = widgets.Tab(children=[outBPMN])
+  tabsBPMN.set_title(0, 'BPMN')
+  display(tabsBPMN)
+  with outBPMN:
+    text = "Tam log: " + str(len(train_csv))
+    sum = 0
+    for x in train_csv:
+      sum+=len(x)
+    textSum = "N° eventos: " + str(sum)
+
+
+    display(text)
+
+
+    display(textSum)
 
+    display(pd.DataFrame(comparacaoBPMN,columns=["Referente à:", "Gateways","Tasks","Transições","Componentes", "Acurácia"]))
```

### Comparing `modProcesso-0.0.4/modProcesso.egg-info/PKG-INFO` & `modProcesso-0.0.5/modProcesso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modProcesso
-Version: 0.0.4
+Version: 0.0.5
 Summary: modProcesso is a library for automata modularisation.
 Home-page: https://github.com/flavioyuri/modProcesso
 Author: Flávio Yuri de Sousa
 Author-email: flavioyuri22@gmail.com
 License: MIT
 Keywords: Theory of Computing,Automata Theory,Languages,Process Mining,Automata Decomposition,Process Modularisation
 Platform: UNKNOWN
```

### Comparing `modProcesso-0.0.4/setup.py` & `modProcesso-0.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as arq:
   readme = arq.read()
 
 setup(
     name='modProcesso',
-    version='0.0.4',
+    version='0.0.5',
     license='MIT',
     author="Flávio Yuri de Sousa",
     author_email='flavioyuri22@gmail.com',
     packages=['modProcesso'],
     url='https://github.com/flavioyuri/modProcesso',
     description='''modProcesso is a library for automata modularisation.''',
     long_description=readme,
```

