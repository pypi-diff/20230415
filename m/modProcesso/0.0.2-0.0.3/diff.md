# Comparing `tmp/modProcesso-0.0.2.tar.gz` & `tmp/modProcesso-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modProcesso-0.0.2.tar", last modified: Mon Apr 10 13:38:41 2023, max compression
+gzip compressed data, was "modProcesso-0.0.3.tar", last modified: Fri Apr 14 23:26:56 2023, max compression
```

## Comparing `modProcesso-0.0.2.tar` & `modProcesso-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-04-10 13:38:40.993959 modProcesso-0.0.2/
--rw-rw-r--   0 yuri      (1000) yuri      (1000)     1069 2023-04-10 03:41:03.000000 modProcesso-0.0.2/LICENSE
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      802 2023-04-10 13:38:40.993959 modProcesso-0.0.2/PKG-INFO
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      351 2023-04-10 13:38:20.000000 modProcesso-0.0.2/README.md
-drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-04-10 13:38:40.993959 modProcesso-0.0.2/modProcesso/
--rw-rw-r--   0 yuri      (1000) yuri      (1000)       25 2023-04-10 03:28:38.000000 modProcesso-0.0.2/modProcesso/__init__.py
--rw-rw-r--   0 yuri      (1000) yuri      (1000)    60717 2023-04-10 13:38:14.000000 modProcesso-0.0.2/modProcesso/modProcesso.py
-drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-04-10 13:38:40.993959 modProcesso-0.0.2/modProcesso.egg-info/
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      802 2023-04-10 13:38:39.000000 modProcesso-0.0.2/modProcesso.egg-info/PKG-INFO
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      251 2023-04-10 13:38:40.000000 modProcesso-0.0.2/modProcesso.egg-info/SOURCES.txt
--rw-rw-r--   0 yuri      (1000) yuri      (1000)        1 2023-04-10 13:38:39.000000 modProcesso-0.0.2/modProcesso.egg-info/dependency_links.txt
--rw-rw-r--   0 yuri      (1000) yuri      (1000)       40 2023-04-10 13:38:39.000000 modProcesso-0.0.2/modProcesso.egg-info/requires.txt
--rw-rw-r--   0 yuri      (1000) yuri      (1000)       12 2023-04-10 13:38:39.000000 modProcesso-0.0.2/modProcesso.egg-info/top_level.txt
--rw-rw-r--   0 yuri      (1000) yuri      (1000)       38 2023-04-10 13:38:40.993959 modProcesso-0.0.2/setup.cfg
--rw-rw-r--   0 yuri      (1000) yuri      (1000)      727 2023-04-10 13:16:31.000000 modProcesso-0.0.2/setup.py
+drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-04-14 23:26:56.904888 modProcesso-0.0.3/
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)     1069 2023-04-10 03:41:03.000000 modProcesso-0.0.3/LICENSE
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      802 2023-04-14 23:26:56.904888 modProcesso-0.0.3/PKG-INFO
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      351 2023-04-10 13:38:20.000000 modProcesso-0.0.3/README.md
+drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-04-14 23:26:56.900888 modProcesso-0.0.3/modProcesso/
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)       25 2023-04-10 03:28:38.000000 modProcesso-0.0.3/modProcesso/__init__.py
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)    63393 2023-04-14 23:17:50.000000 modProcesso-0.0.3/modProcesso/modProcesso.py
+drwxrwxr-x   0 yuri      (1000) yuri      (1000)        0 2023-04-14 23:26:56.904888 modProcesso-0.0.3/modProcesso.egg-info/
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      802 2023-04-14 23:26:56.000000 modProcesso-0.0.3/modProcesso.egg-info/PKG-INFO
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      251 2023-04-14 23:26:56.000000 modProcesso-0.0.3/modProcesso.egg-info/SOURCES.txt
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)        1 2023-04-14 23:26:56.000000 modProcesso-0.0.3/modProcesso.egg-info/dependency_links.txt
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)       40 2023-04-14 23:26:56.000000 modProcesso-0.0.3/modProcesso.egg-info/requires.txt
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)       12 2023-04-14 23:26:56.000000 modProcesso-0.0.3/modProcesso.egg-info/top_level.txt
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)       38 2023-04-14 23:26:56.904888 modProcesso-0.0.3/setup.cfg
+-rw-rw-r--   0 yuri      (1000) yuri      (1000)      727 2023-04-14 23:26:52.000000 modProcesso-0.0.3/setup.py
```

### Comparing `modProcesso-0.0.2/LICENSE` & `modProcesso-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `modProcesso-0.0.2/PKG-INFO` & `modProcesso-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modProcesso
-Version: 0.0.2
+Version: 0.0.3
 Summary: modProcesso is a library for automata modularisation.
 Home-page: https://github.com/flavioyuri/modProcesso
 Author: Flávio Yuri de Sousa
 Author-email: flavioyuri22@gmail.com
 License: MIT
 Keywords: Theory of Computing,Automata Theory,Languages,Process Mining,Automata Decomposition,Process Modularisation
 Platform: UNKNOWN
```

### Comparing `modProcesso-0.0.2/modProcesso/modProcesso.py` & `modProcesso-0.0.3/modProcesso/modProcesso.py`

 * *Files 7% similar despite different names*

```diff
@@ -417,16 +417,16 @@
   
 
   return bpmn  
   
 
 
 
-def fitnessAutomata(automato, df_test2, sRet=False):
-  if sRet == False:
+def fitnessAutomata(automato, df_test2, sRet=False, sRetTest=False):
+  if sRetTest == False:
     
     aceita = 0
     for i in range(len(df_test2)):
       if automato.aceita(df_test2[i]):
         aceita = aceita+1
 
     fitness = (aceita/len(df_test2)) * 100
@@ -436,16 +436,17 @@
     for j in range(len(df_test2)):
       trace, trace_new_transitions = removeAllSequencesOfRepetitions(df_test2[j])
       
       if automato.aceita(trace):
         aceita = aceita+1
     fitness = (aceita/len(df_test2)) * 100
 
-  print("log fit:", fitness)
-
+  #print("log fit:", fitness)
+  return fitness
+  
 
 
 ######Funções de conversão de automatos
 
 def convertToListOfTraces(file_xes, max_traces=-1, sort=False):
       variant = xes_importer.Variants.ITERPARSE
       if(max_traces != -1):
@@ -1117,390 +1118,422 @@
       tasks.append(n)
     elif type(n) == pm4py.objects.bpmn.obj.BPMN.ExclusiveGateway:
       gateways.append(n)
     elif type(n) == pm4py.objects.bpmn.obj.BPMN.ParallelGateway:
       gateways.append(n)
   return len(gateways), len(tasks), len(bpmn.get_flows())
 
-def tabelamento(event_log, df_test, camMin=True, sRet=True, join=True, mFreq=False, p=1, remGat = True):
+def tabelamento(event_log, df_test, sRetTest = True, camMin=True, sRet=True, join=True, mFreq=False, p=1, remGat = True):
 
 
   #Caminhos mais frequêntes
   if mFreq:
     l_mf_traces, acuracia = get_most_frequent_traces(event_log,percentage=p)
     print(f"Frequencia por trace dos {p*100}% mais frequentes:\n",l_mf_traces)
     #print(f"{p*100}% dos traces mais frequentes:\n",[x[0] for x in l_mf_traces])
     event_logFreq = [x[0] for x in l_mf_traces]
 
     resultados = []
     resultadosBPMN = []
     nfa = to_nfa(event_logFreq)
-    resultados.append([f"Não-Determinística",len(nfa.alphabet),len(nfa.states),nfa.len_transition(),len(nfa.acceptStates), 0, nfa.len_states()])
+    fit = fitnessAutomata(nfa, df_test, sRet, sRetTest)
+    resultados.append([f"Não-Determinística",len(nfa.alphabet),len(nfa.states),nfa.len_transition(),len(nfa.acceptStates), 0, nfa.len_states(), fit])
     bpmn = nfa_to_bpmn(nfa, remGat)
     gateways, tasks, flows = countBPMN(bpmn)
     resultadosBPMN.append([f"Não-Determinística", gateways, tasks, flows])
     dfa = nfa.determinization()
     dfa.rename()
-    resultados.append([f"Determinística",len(dfa.alphabet),len(dfa.states),len(dfa.transition),len(dfa.acceptStates), "-", "-"])
+    fit = fitnessAutomata(dfa, df_test, sRet, sRetTest)
+    resultados.append([f"Determinística",len(dfa.alphabet),len(dfa.states),len(dfa.transition),len(dfa.acceptStates), "-", "-", fit])
     bpmn = dfa_to_bpmn(dfa, remGat)
     gateways, tasks, flows = countBPMN(bpmn)
     resultadosBPMN.append([f"Determinística", gateways, tasks, flows])
     
 
     min= dfa.minimization()
     min.rename()
-    resultados.append([f"Determinística min",len(min.alphabet),len(min.states),len(min.transition),len(min.acceptStates), "-", "-"])
+    fit = fitnessAutomata(min, df_test, sRet, sRetTest)
+    resultados.append([f"Determinística min",len(min.alphabet),len(min.states),len(min.transition),len(min.acceptStates), "-", "-", fit])
     bpmn = dfa_to_bpmn(min, remGat)
     gateways, tasks, flows = countBPMN(bpmn)
     resultadosBPMN.append([f"Determinística min", gateways, tasks, flows])
     
 
 
     min = dfaToNfa(min)
     nfaResultado = operacaoSequencias(min, 3, 25)
-    resultados.append([f"Operação Sequencias min/max:3-25 estados DFA min",len(nfaResultado.alphabet),len(nfaResultado.states),len(nfaResultado.transition),len(nfaResultado.acceptStates), len(nfaResultado.NFAs), nfaResultado.len_states()])
+    fit = fitnessAutomata(nfaResultado, df_test, sRet, sRetTest)
+    resultados.append([f"Operação Sequencias min/max:3-25 estados DFA min",len(nfaResultado.alphabet),len(nfaResultado.states),len(nfaResultado.transition),len(nfaResultado.acceptStates), len(nfaResultado.NFAs), nfaResultado.len_states(), fit])
     bpmn = nfaBB_to_bpmn(nfaResultado, remGat)
     gateways, tasks, flows = countBPMN(bpmn)
     resultadosBPMN.append([f"Operação Sequencias min/max:3-25 estados DFA min", gateways, tasks, flows])
     
     
     #Caminho Mínimo
     if camMin:
       nfaCamMin = to_nfa_minimum_path(event_logFreq, nfa_bb=False)
-
-      resultados.append([f"Não-Determinística caminho mínimo",len(nfaCamMin.alphabet),len(nfaCamMin.states),nfaCamMin.len_transition(),len(nfaCamMin.acceptStates), 0, "-"])
+      fit = fitnessAutomata(nfaCamMin, df_test, sRet, sRetTest)
+      resultados.append([f"Não-Determinística caminho mínimo",len(nfaCamMin.alphabet),len(nfaCamMin.states),nfaCamMin.len_transition(),len(nfaCamMin.acceptStates), 0, "-", fit])
       bpmn = nfa_to_bpmn(nfaCamMin, remGat)
       gateways, tasks, flows = countBPMN(bpmn)
       resultadosBPMN.append([f"Não-Determinística caminho mínimo", gateways, tasks, flows])
       
       
       dfa = nfaCamMin.determinization()
       #print(dfa.alphabet)
       dfa.rename()
-      resultados.append([f"Determinística",len(dfa.alphabet),len(dfa.states),len(dfa.transition),len(dfa.acceptStates), "-", "-"])
+      fit = fitnessAutomata(dfa, df_test, sRet, sRetTest)
+      resultados.append([f"Determinística",len(dfa.alphabet),len(dfa.states),len(dfa.transition),len(dfa.acceptStates), "-", "-", fit])
       bpmn = dfa_to_bpmn(dfa, remGat)
       gateways, tasks, flows = countBPMN(bpmn)
       resultadosBPMN.append([f"Determinística", gateways, tasks, flows])
       
 
 
       min = dfa.minimization()
-      resultados.append([f"Determinística min",len(min.alphabet),len(min.states),len(min.transition),len(min.acceptStates), "-", "-"])
+      fit = fitnessAutomata(min, df_test, sRet, sRetTest)
+      resultados.append([f"Determinística min",len(min.alphabet),len(min.states),len(min.transition),len(min.acceptStates), "-", "-", fit])
       bpmn = dfa_to_bpmn(min, remGat)
       gateways, tasks, flows = countBPMN(bpmn)
       resultadosBPMN.append([f"Determinística min", gateways, tasks, flows])
       
 
 
       min = dfaToNfa(min)
       nfaResultado = operacaoSequencias(min, 3, 25)
-      resultados.append([f"Operação Sequencias min/max:3-25 estados DFA min caminhos mínimos",len(nfaResultado.alphabet),len(nfaResultado.states),len(nfaResultado.transition),len(nfaResultado.acceptStates), len(nfaResultado.NFAs), nfaResultado.len_states()])
+      fit = fitnessAutomata(nfaResultado, df_test, sRet, sRetTest)
+      resultados.append([f"Operação Sequencias min/max:3-25 estados DFA min caminhos mínimos",len(nfaResultado.alphabet),len(nfaResultado.states),len(nfaResultado.transition),len(nfaResultado.acceptStates), len(nfaResultado.NFAs), nfaResultado.len_states(), fit])
       bpmn = nfaBB_to_bpmn(nfaResultado, remGat)
       gateways, tasks, flows = countBPMN(bpmn)
       resultadosBPMN.append([f"Operação Sequencias min/max:3-25 estados DFA min caminhos mínimos", gateways, tasks, flows])
       
 
 
     #Sem retrabalho
     if sRet:
       nfaReworkFalse = to_nfa_minimum_path(event_logFreq, rework=False, nfa_bb=False)
-
-      resultados.append([f"Não-Determinística sem retrabalho",len(nfaReworkFalse.alphabet),len(nfaReworkFalse.states),nfaReworkFalse.len_transition(),len(nfaReworkFalse.acceptStates), 0, nfaReworkFalse.len_states()])
+      fit = fitnessAutomata(nfaReworkFalse, df_test, sRet, sRetTest)
+      resultados.append([f"Não-Determinística sem retrabalho",len(nfaReworkFalse.alphabet),len(nfaReworkFalse.states),nfaReworkFalse.len_transition(),len(nfaReworkFalse.acceptStates), 0, nfaReworkFalse.len_states(), fit])
       bpmn = nfa_to_bpmn(nfaReworkFalse, remGat)
       gateways, tasks, flows = countBPMN(bpmn)
       resultadosBPMN.append([f"Não-Determinística sem retrabalho", gateways, tasks, flows])
       
 
 
       dfaFalse = nfaReworkFalse.determinization()
       #print(dfa.alphabet)
       dfaFalse.rename()
-      resultados.append([f"Determinística s retrabalho",len(dfaFalse.alphabet),len(dfaFalse.states),len(dfaFalse.transition),len(dfaFalse.acceptStates), "-", "-"])
+      fit = fitnessAutomata(dfaFalse, df_test, sRet, sRetTest)
+      resultados.append([f"Determinística s retrabalho",len(dfaFalse.alphabet),len(dfaFalse.states),len(dfaFalse.transition),len(dfaFalse.acceptStates), "-", "-", fit])
       bpmn = dfa_to_bpmn(dfaFalse, remGat)
       gateways, tasks, flows = countBPMN(bpmn)
       resultadosBPMN.append([f"Determinística s retrabalho", gateways, tasks, flows])
       
 
 
       minFalse= dfaFalse.minimization()
       minFalse.rename()
-      resultados.append([f"Determinística min s retrabalho",len(minFalse.alphabet),len(minFalse.states),len(minFalse.transition),len(minFalse.acceptStates), "-", "-"])
+      fit = fitnessAutomata(minFalse, df_test, sRet, sRetTest)
+      resultados.append([f"Determinística min s retrabalho",len(minFalse.alphabet),len(minFalse.states),len(minFalse.transition),len(minFalse.acceptStates), "-", "-", fit])
       bpmn = dfa_to_bpmn(minFalse, remGat)
       gateways, tasks, flows = countBPMN(bpmn)
       resultadosBPMN.append([f"Determinística min s retrabalho", gateways, tasks, flows])
       
 
 
       min = dfaToNfa(minFalse)
       nfaResultado = operacaoSequencias(min, 3, 25)
-      resultados.append([f"Operação Sequencias min/max:3-25 estados DFA min sem retrabalho",len(nfaResultado.alphabet),len(nfaResultado.states),len(nfaResultado.transition),len(nfaResultado.acceptStates), len(nfaResultado.NFAs), nfaResultado.len_states()])
+      fit = fitnessAutomata(nfaResultado, df_test, sRet, sRetTest)
+      resultados.append([f"Operação Sequencias min/max:3-25 estados DFA min sem retrabalho",len(nfaResultado.alphabet),len(nfaResultado.states),len(nfaResultado.transition),len(nfaResultado.acceptStates), len(nfaResultado.NFAs), nfaResultado.len_states(), fit])
       bpmn = nfaBB_to_bpmn(nfaResultado, remGat)
       gateways, tasks, flows = countBPMN(bpmn)
       resultadosBPMN.append([f"Operação Sequencias min/max:3-25 estados DFA min sem retrabalho", gateways, tasks, flows])
       
 
     #Sem caminhos repetidos
     if join:
       nfaJoin = to_nfa_minimum_path_join_traces(event_logFreq)
-
-      resultados.append([f"Não-Determinística join",len(nfaJoin.alphabet),len(nfaJoin.states),nfaJoin.len_transition(),len(nfaJoin.acceptStates), 0, "-"])
+      fit = fitnessAutomata(nfaJoin, df_test, sRet, sRetTest)
+      resultados.append([f"Não-Determinística join",len(nfaJoin.alphabet),len(nfaJoin.states),nfaJoin.len_transition(),len(nfaJoin.acceptStates), 0, "-", fit])
       bpmn = nfa_to_bpmn(nfaJoin, remGat)
       gateways, tasks, flows = countBPMN(bpmn)
       resultadosBPMN.append([f"Não-Determinística join", gateways, tasks, flows])
       
 
 
       dfaJoin = nfaJoin.determinization()
       dfaJoin.rename()
-      resultados.append([f"Determinística join",len(nfaJoin.alphabet),len(nfaJoin.states),len(nfaJoin.transition),len(nfaJoin.acceptStates), "-" , "-"])
+      fit = fitnessAutomata(dfaJoin, df_test, sRet, sRetTest)
+      resultados.append([f"Determinística join",len(nfaJoin.alphabet),len(nfaJoin.states),len(nfaJoin.transition),len(nfaJoin.acceptStates), "-" , "-", fit])
       bpmn = dfa_to_bpmn(dfaJoin, remGat)
       gateways, tasks, flows = countBPMN(bpmn)
       resultadosBPMN.append([f"Determinística join", gateways, tasks, flows])
       
 
 
       minJoin= dfaJoin.minimization()
       minJoin.rename()
-      resultados.append([f"Determinística min join",len(minJoin.alphabet),len(minJoin.states),len(minJoin.transition),len(minJoin.acceptStates), "-", "-"])
+      fit = fitnessAutomata(minJoin, df_test, sRet, sRetTest)
+      resultados.append([f"Determinística min join",len(minJoin.alphabet),len(minJoin.states),len(minJoin.transition),len(minJoin.acceptStates), "-", "-", fit])
       bpmn = dfa_to_bpmn(minJoin, remGat)
       gateways, tasks, flows = countBPMN(bpmn)
       resultadosBPMN.append([f"Determinística min join", gateways, tasks, flows])
       
 
 
       min = dfaToNfa(minJoin)
       nfaResultado = operacaoSequencias(min, 3, 25)
-      resultados.append([f"Operação Sequencias min/max:3-25 estados DFA min join",len(nfaResultado.alphabet),len(nfaResultado.states),len(nfaResultado.transition),len(nfaResultado.acceptStates), len(nfaResultado.NFAs), nfaResultado.len_states()])
+      fit = fitnessAutomata(nfaResultado, df_test, sRet, sRetTest)
+      resultados.append([f"Operação Sequencias min/max:3-25 estados DFA min join",len(nfaResultado.alphabet),len(nfaResultado.states),len(nfaResultado.transition),len(nfaResultado.acceptStates), len(nfaResultado.NFAs), nfaResultado.len_states(), fit])
       bpmn = nfaBB_to_bpmn(min, remGat)
       gateways, tasks, flows = countBPMN(bpmn)
       resultadosBPMN.append([f"Operação Sequencias min/max:3-25 estados DFA min join", gateways, tasks, flows])
       
 
       if sRet:
         nfaJoinFalse = to_nfa_minimum_path_join_traces(event_logFreq, rework=False)
-        resultados.append([f"Não-Determinística sem retrabalho join",len(nfaJoinFalse.alphabet),len(nfaJoinFalse.states),nfaJoinFalse.len_transition(),len(nfaJoinFalse.acceptStates), 0,"-"])
+        fit = fitnessAutomata(nfaJoinFalse, df_test, sRet, sRetTest)
+        resultados.append([f"Não-Determinística sem retrabalho join",len(nfaJoinFalse.alphabet),len(nfaJoinFalse.states),nfaJoinFalse.len_transition(),len(nfaJoinFalse.acceptStates), 0,"-", fit])
         bpmn = nfa_to_bpmn(nfaJoinFalse, remGat)
         gateways, tasks, flows = countBPMN(bpmn)
         resultadosBPMN.append([f"Não-Determinística sem retrabalho join", gateways, tasks, flows])
         
         
         dfaJoinFalse = nfaJoinFalse.determinization()
         dfaJoinFalse.rename()
-        resultados.append([f"Determinística sem retrabalho join",len(dfaJoinFalse.alphabet),len(dfaJoinFalse.states),len(dfaJoinFalse.transition),len(dfaJoinFalse.acceptStates), "-", "-"])
+        fit = fitnessAutomata(dfaJoinFalse, df_test, sRet, sRetTest)
+        resultados.append([f"Determinística sem retrabalho join",len(dfaJoinFalse.alphabet),len(dfaJoinFalse.states),len(dfaJoinFalse.transition),len(dfaJoinFalse.acceptStates), "-", "-", fit])
         bpmn = dfa_to_bpmn(dfaJoinFalse, remGat)
         gateways, tasks, flows = countBPMN(bpmn)
         resultadosBPMN.append([f"Determinística sem retrabalho join", gateways, tasks, flows])
         
 
 
         minJoinFalse= dfaJoinFalse.minimization()
         minJoinFalse.rename()
-        resultados.append([f"Determinística min sem retrabalho join",len(minJoinFalse.alphabet),len(minJoinFalse.states),len(minJoinFalse.transition),len(minJoinFalse.acceptStates), "-", "-"])
+        fit = fitnessAutomata(minJoinFalse, df_test, sRet, sRetTest)
+        resultados.append([f"Determinística min sem retrabalho join",len(minJoinFalse.alphabet),len(minJoinFalse.states),len(minJoinFalse.transition),len(minJoinFalse.acceptStates), "-", "-", fit])
         bpmn = dfa_to_bpmn(minJoinFalse, remGat)
         gateways, tasks, flows = countBPMN(bpmn)
         resultadosBPMN.append([f"Determinística min sem retrabalho join", gateways, tasks, flows])
         
 
 
         min = dfaToNfa(minJoinFalse)
         nfaResultado = operacaoSequencias(min, 3, 25)
-        resultados.append([f"Operação Sequencias min/max:3-25 estados DFA min sem retrabalho join",len(nfaResultado.alphabet),len(nfaResultado.states),len(nfaResultado.transition),len(nfaResultado.acceptStates), len(nfaResultado.NFAs), nfaResultado.len_states()])
+        fit = fitnessAutomata(nfaResultado, df_test, sRet, sRetTest)
+        resultados.append([f"Operação Sequencias min/max:3-25 estados DFA min sem retrabalho join",len(nfaResultado.alphabet),len(nfaResultado.states),len(nfaResultado.transition),len(nfaResultado.acceptStates), len(nfaResultado.NFAs), nfaResultado.len_states(), fit])
         bpmn = nfaBB_to_bpmn(min, remGat)
         gateways, tasks, flows = countBPMN(bpmn)
         resultadosBPMN.append([f"Operação Sequencias min/max:3-25 estados DFA min sem retrabalho join", gateways, tasks, flows])
         
-    display(fitnessAutomata(nfaResultado, df_test, sRet))
   
   else:
     resultados = []
     resultadosBPMN = []
     nfa = to_nfa(event_log)
 
-    resultados.append(["Não-Determinística",len(nfa.alphabet),len(nfa.states),nfa.len_transition(),len(nfa.acceptStates), 0, nfa.len_states()])
+    fit = fitnessAutomata(nfa, df_test, sRet, sRetTest)
+    resultados.append(["Não-Determinística",len(nfa.alphabet),len(nfa.states),nfa.len_transition(),len(nfa.acceptStates), 0, nfa.len_states(), fit])
     
     
     bpmn = nfa_to_bpmn(nfa, remGat)
     gateways, tasks, flows = countBPMN(bpmn)
     resultadosBPMN.append(["Não-Determinística", gateways, tasks, flows])
     
     dfa = nfa.determinization()
     dfa.rename()
-    resultados.append(["Determinística",len(dfa.alphabet),len(dfa.states),len(dfa.transition),len(dfa.acceptStates), "-", "-"])
+    fit = fitnessAutomata(dfa, df_test, sRet, sRetTest)
+    resultados.append(["Determinística",len(dfa.alphabet),len(dfa.states),len(dfa.transition),len(dfa.acceptStates), "-", "-", fit])
     bpmn = dfa_to_bpmn(dfa, remGat)
     gateways, tasks, flows = countBPMN(bpmn)
     resultadosBPMN.append(["Determinística", gateways, tasks, flows])
     
 
 
     min= dfa.minimization()
     min.rename()
-    resultados.append(["Determinística min",len(min.alphabet),len(min.states),len(min.transition),len(min.acceptStates), "-", "-"])
+    fit = fitnessAutomata(min, df_test, sRet, sRetTest)
+    resultados.append(["Determinística min",len(min.alphabet),len(min.states),len(min.transition),len(min.acceptStates), "-", "-", fit])
     bpmn = dfa_to_bpmn(min, remGat)
     gateways, tasks, flows = countBPMN(bpmn)
     resultadosBPMN.append(["Determinística min", gateways, tasks, flows])
     
 
 
     min = dfaToNfa(min)
     nfaResultado = operacaoSequencias(min, 3, 25)
-    resultados.append(["Operação Sequencias min/max:3-25 estados DFA min",len(nfaResultado.alphabet),len(nfaResultado.states),len(nfaResultado.transition),len(nfaResultado.acceptStates), len(nfaResultado.NFAs), nfaResultado.len_states()])
+    fit = fitnessAutomata(nfaResultado, df_test, sRet, sRetTest)
+    resultados.append(["Operação Sequencias min/max:3-25 estados DFA min",len(nfaResultado.alphabet),len(nfaResultado.states),len(nfaResultado.transition),len(nfaResultado.acceptStates), len(nfaResultado.NFAs), nfaResultado.len_states(), fit])
     bpmn = nfaBB_to_bpmn(nfaResultado, remGat)
     gateways, tasks, flows = countBPMN(bpmn)
     resultadosBPMN.append(["Operação Sequencias min/max:3-25 estados DFA min", gateways, tasks, flows])
     
 
 
     #Caminho Mínimo
     if camMin:
       nfaCamMin = to_nfa_minimum_path(event_log, nfa_bb=False)
-
-      resultados.append(["Não-Determinística caminho mínimo",len(nfaCamMin.alphabet),len(nfaCamMin.states),nfaCamMin.len_transition(),len(nfaCamMin.acceptStates), 0, "-"])
+      fit = fitnessAutomata(nfaCamMin, df_test, sRet, sRetTest)
+      resultados.append(["Não-Determinística caminho mínimo",len(nfaCamMin.alphabet),len(nfaCamMin.states),nfaCamMin.len_transition(),len(nfaCamMin.acceptStates), 0, "-", fit])
       bpmn = nfa_to_bpmn(nfaCamMin, remGat)
       gateways, tasks, flows = countBPMN(bpmn)
       resultadosBPMN.append(["Não-Determinística caminho mínimo", gateways, tasks, flows])
       
 
       dfa = nfaCamMin.determinization()
       dfa.rename()
-      resultados.append(["Determinística",len(dfa.alphabet),len(dfa.states),len(dfa.transition),len(dfa.acceptStates), "-", "-"])
+      fit = fitnessAutomata(dfa, df_test, sRet, sRetTest)
+      resultados.append(["Determinística",len(dfa.alphabet),len(dfa.states),len(dfa.transition),len(dfa.acceptStates), "-", "-", fit])
       bpmn = dfa_to_bpmn(dfa, remGat)
       gateways, tasks, flows = countBPMN(bpmn)
       resultadosBPMN.append(["Determinística", gateways, tasks, flows])
       
 
 
       min = dfa.minimization()
-      resultados.append(["Determinística min",len(min.alphabet),len(min.states),len(min.transition),len(min.acceptStates), "-", "-"])
+      fit = fitnessAutomata(min, df_test, sRet, sRetTest)
+      resultados.append(["Determinística min",len(min.alphabet),len(min.states),len(min.transition),len(min.acceptStates), "-", "-", fit])
       bpmn = dfa_to_bpmn(min, remGat)
       gateways, tasks, flows = countBPMN(bpmn)
       resultadosBPMN.append(["Determinística min", gateways, tasks, flows])
       
 
 
       min = dfaToNfa(min)
       nfaResultado = operacaoSequencias(min, 3, 25)
-      resultados.append(["Operação Sequencias min/max:3-25 estados DFA min caminhos mínimos",len(nfaResultado.alphabet),len(nfaResultado.states),len(nfaResultado.transition),len(nfaResultado.acceptStates), len(nfaResultado.NFAs), nfaResultado.len_states()])
+      fit = fitnessAutomata(nfaResultado, df_test, sRet, sRetTest)
+      resultados.append(["Operação Sequencias min/max:3-25 estados DFA min caminhos mínimos",len(nfaResultado.alphabet),len(nfaResultado.states),len(nfaResultado.transition),len(nfaResultado.acceptStates), len(nfaResultado.NFAs), nfaResultado.len_states(), fit])
       bpmn = nfaBB_to_bpmn(nfaResultado, remGat)
       gateways, tasks, flows = countBPMN(bpmn)
       resultadosBPMN.append(["Operação Sequencias min/max:3-25 estados DFA min caminhos mínimos", gateways, tasks, flows])
       
 
 
     #Sem retrabalho
     if sRet:
       nfaReworkFalse = to_nfa_minimum_path(event_log, rework=False, nfa_bb=False)
-
-      resultados.append(["Não-Determinística sem retrabalho",len(nfaReworkFalse.alphabet),len(nfaReworkFalse.states),nfaReworkFalse.len_transition(),len(nfaReworkFalse.acceptStates), 0, nfaReworkFalse.len_states()])
+      fit = fitnessAutomata(nfaReworkFalse, df_test, sRet, sRetTest)
+      resultados.append(["Não-Determinística sem retrabalho",len(nfaReworkFalse.alphabet),len(nfaReworkFalse.states),nfaReworkFalse.len_transition(),len(nfaReworkFalse.acceptStates), 0, nfaReworkFalse.len_states(), fit])
       bpmn = nfa_to_bpmn(nfaReworkFalse, remGat)
       gateways, tasks, flows = countBPMN(bpmn)
       resultadosBPMN.append(["Não-Determinística sem retrabalho", gateways, tasks, flows])
       
 
 
       dfaFalse = nfaReworkFalse.determinization()
       #print(dfa.alphabet)
       dfaFalse.rename()
-      resultados.append(["Determinística s retrabalho",len(dfaFalse.alphabet),len(dfaFalse.states),len(dfaFalse.transition),len(dfaFalse.acceptStates), "-", "-"])
+      fit = fitnessAutomata(dfaFalse, df_test, sRet, sRetTest)
+      resultados.append(["Determinística s retrabalho",len(dfaFalse.alphabet),len(dfaFalse.states),len(dfaFalse.transition),len(dfaFalse.acceptStates), "-", "-", fit])
       bpmn = dfa_to_bpmn(dfaFalse, remGat)
       gateways, tasks, flows = countBPMN(bpmn)
       resultadosBPMN.append(["Determinística s retrabalho", gateways, tasks, flows])
       
 
 
       minFalse= dfaFalse.minimization()
       minFalse.rename()
-      resultados.append(["Determinística min s retrabalho",len(minFalse.alphabet),len(minFalse.states),len(minFalse.transition),len(minFalse.acceptStates), "-", "-"])
+      fit = fitnessAutomata(minFalse, df_test, sRet, sRetTest)
+      resultados.append(["Determinística min s retrabalho",len(minFalse.alphabet),len(minFalse.states),len(minFalse.transition),len(minFalse.acceptStates), "-", "-", fit])
       bpmn = dfa_to_bpmn(minFalse, remGat)
       gateways, tasks, flows = countBPMN(bpmn)
       resultadosBPMN.append(["Determinística min s retrabalho", gateways, tasks, flows])
       
 
 
       min = dfaToNfa(minFalse)
       nfaResultado = operacaoSequencias(min, 3, 25)
-      resultados.append(["Operação Sequencias min/max:3-25 estados DFA min sem retrabalho",len(nfaResultado.alphabet),len(nfaResultado.states),len(nfaResultado.transition),len(nfaResultado.acceptStates), len(nfaResultado.NFAs), nfaResultado.len_states()])
+      fit = fitnessAutomata(nfaResultado, df_test, sRet, sRetTest)
+      resultados.append(["Operação Sequencias min/max:3-25 estados DFA min sem retrabalho",len(nfaResultado.alphabet),len(nfaResultado.states),len(nfaResultado.transition),len(nfaResultado.acceptStates), len(nfaResultado.NFAs), nfaResultado.len_states(), fit])
       bpmn = nfaBB_to_bpmn(nfaResultado, remGat)
       gateways, tasks, flows = countBPMN(bpmn)
       resultadosBPMN.append(["Operação Sequencias min/max:3-25 estados DFA min sem retrabalho", gateways, tasks, flows])
       
 
 
     #Sem caminhos repetidos
     if join:
       nfaJoin = to_nfa_minimum_path_join_traces(event_log)
-
-      resultados.append(["Não-Determinística join",len(nfaJoin.alphabet),len(nfaJoin.states),nfaJoin.len_transition(),len(nfaJoin.acceptStates), 0, "-"])
+      fit = fitnessAutomata(nfaJoin, df_test, sRet, sRetTest)
+      resultados.append(["Não-Determinística join",len(nfaJoin.alphabet),len(nfaJoin.states),nfaJoin.len_transition(),len(nfaJoin.acceptStates), 0, "-", fit])
       bpmn = nfa_to_bpmn(nfaJoin, remGat)
       gateways, tasks, flows = countBPMN(bpmn)
       resultadosBPMN.append(["Não-Determinística join", gateways, tasks, flows])
       
 
 
       dfaJoin = nfaJoin.determinization()
       dfaJoin.rename()
-      resultados.append(["Determinística join",len(nfaJoin.alphabet),len(nfaJoin.states),len(nfaJoin.transition),len(nfaJoin.acceptStates), "-" , "-"])
+      fit = fitnessAutomata(dfaJoin, df_test, sRet, sRetTest)
+      resultados.append(["Determinística join",len(nfaJoin.alphabet),len(nfaJoin.states),len(nfaJoin.transition),len(nfaJoin.acceptStates), "-" , "-", fit])
       bpmn = dfa_to_bpmn(dfaJoin, remGat)
       gateways, tasks, flows = countBPMN(bpmn)
       resultadosBPMN.append(["Determinística join", gateways, tasks, flows])
       
 
 
       minJoin= dfaJoin.minimization()
       minJoin.rename()
-      resultados.append(["Determinística min join",len(minJoin.alphabet),len(minJoin.states),len(minJoin.transition),len(minJoin.acceptStates), "-", "-"])
+      fit = fitnessAutomata(minJoin, df_test, sRet, sRetTest)
+      resultados.append(["Determinística min join",len(minJoin.alphabet),len(minJoin.states),len(minJoin.transition),len(minJoin.acceptStates), "-", "-", fit])
       bpmn = dfa_to_bpmn(minJoin, remGat)
       gateways, tasks, flows = countBPMN(bpmn)
       resultadosBPMN.append(["Determinística min join", gateways, tasks, flows])
       
 
 
       min = dfaToNfa(minJoin)
       nfaResultado = operacaoSequencias(min, 3, 25)
-      resultados.append(["Operação Sequencias min/max:3-25 estados DFA min join",len(nfaResultado.alphabet),len(nfaResultado.states),len(nfaResultado.transition),len(nfaResultado.acceptStates), len(nfaResultado.NFAs), nfaResultado.len_states()])
+      fit = fitnessAutomata(nfaResultado, df_test, sRet, sRetTest)
+      resultados.append(["Operação Sequencias min/max:3-25 estados DFA min join",len(nfaResultado.alphabet),len(nfaResultado.states),len(nfaResultado.transition),len(nfaResultado.acceptStates), len(nfaResultado.NFAs), nfaResultado.len_states(), fit])
       bpmn = nfaBB_to_bpmn(nfaResultado, remGat)
       gateways, tasks, flows = countBPMN(bpmn)
       resultadosBPMN.append(["Operação Sequencias min/max:3-25 estados DFA min join", gateways, tasks, flows])
       
 
 
       if sRet:
         nfaJoinFalse = to_nfa_minimum_path_join_traces(event_log, rework=False)
+        fit = fitnessAutomata(nfaJoinFalse, df_test, sRet, sRetTest)
         resultados.append(["Não-Determinística sem retrabalho join",len(nfaJoinFalse.alphabet),len(nfaJoinFalse.states),nfaJoinFalse.len_transition(),len(nfaJoinFalse.acceptStates), 0,"-"])
         bpmn = nfa_to_bpmn(nfaJoinFalse, remGat)
         gateways, tasks, flows = countBPMN(bpmn)
         resultadosBPMN.append(["Não-Determinística sem retrabalho join", gateways, tasks, flows])
         
         
         dfaJoinFalse = nfaJoinFalse.determinization()
         #print(dfa.alphabet)
         dfaJoinFalse.rename()
-        resultados.append(["Determinística sem retrabalho join",len(dfaJoinFalse.alphabet),len(dfaJoinFalse.states),len(dfaJoinFalse.transition),len(dfaJoinFalse.acceptStates), "-", "-"])
+        fit = fitnessAutomata(dfaJoinFalse, df_test, sRet, sRetTest)
+        resultados.append(["Determinística sem retrabalho join",len(dfaJoinFalse.alphabet),len(dfaJoinFalse.states),len(dfaJoinFalse.transition),len(dfaJoinFalse.acceptStates), "-", "-", fit])
         bpmn = dfa_to_bpmn(dfaJoinFalse, remGat)
         gateways, tasks, flows = countBPMN(bpmn)
         resultadosBPMN.append(["Determinística sem retrabalho join", gateways, tasks, flows])
       
 
 
         minJoinFalse= dfaJoinFalse.minimization()
         minJoinFalse.rename()
-        resultados.append(["Determinística min sem retrabalho join",len(minJoinFalse.alphabet),len(minJoinFalse.states),len(minJoinFalse.transition),len(minJoinFalse.acceptStates), "-", "-"])
+        fit = fitnessAutomata(minJoinFalse, df_test, sRet, sRetTest)
+        resultados.append(["Determinística min sem retrabalho join",len(minJoinFalse.alphabet),len(minJoinFalse.states),len(minJoinFalse.transition),len(minJoinFalse.acceptStates), "-", "-", fit])
         bpmn = dfa_to_bpmn(minJoinFalse, remGat)
         gateways, tasks, flows = countBPMN(bpmn)
         resultadosBPMN.append(["Determinística min sem retrabalho join", gateways, tasks, flows])
         
 
 
         min = dfaToNfa(minJoinFalse)
         nfaResultado= operacaoSequencias(min, 3, 25)
-        resultados.append(["Operação Sequencias min/max:3-25 estados DFA min sem retrabalho join",len(nfaResultado.alphabet),len(nfaResultado.states),len(nfaResultado.transition),len(nfaResultado.acceptStates), len(nfaResultado.NFAs), nfaResultado.len_states()])
+        fit = fitnessAutomata(nfaResultado, df_test, sRet, sRetTest)
+        resultados.append(["Operação Sequencias min/max:3-25 estados DFA min sem retrabalho join",len(nfaResultado.alphabet),len(nfaResultado.states),len(nfaResultado.transition),len(nfaResultado.acceptStates), len(nfaResultado.NFAs), nfaResultado.len_states(), fit])
         bpmn = nfaBB_to_bpmn(nfaResultado, remGat)
         gateways, tasks, flows = countBPMN(bpmn)
         resultadosBPMN.append(["Operação Sequencias min/max:3-25 estados DFA min sem retrabalho join", gateways, tasks, flows])
-    display(fitnessAutomata(nfaResultado, df_test, sRet))
-
+    
 
   outMaquinaEstado = widgets.Output()
 
   
   tabs = widgets.Tab(children=[outMaquinaEstado])
   tabs.set_title(0, 'Máquina de Estados')
   display(tabs)
```

### Comparing `modProcesso-0.0.2/modProcesso.egg-info/PKG-INFO` & `modProcesso-0.0.3/modProcesso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modProcesso
-Version: 0.0.2
+Version: 0.0.3
 Summary: modProcesso is a library for automata modularisation.
 Home-page: https://github.com/flavioyuri/modProcesso
 Author: Flávio Yuri de Sousa
 Author-email: flavioyuri22@gmail.com
 License: MIT
 Keywords: Theory of Computing,Automata Theory,Languages,Process Mining,Automata Decomposition,Process Modularisation
 Platform: UNKNOWN
```

### Comparing `modProcesso-0.0.2/setup.py` & `modProcesso-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as arq:
   readme = arq.read()
 
 setup(
     name='modProcesso',
-    version='0.0.2',
+    version='0.0.3',
     license='MIT',
     author="Flávio Yuri de Sousa",
     author_email='flavioyuri22@gmail.com',
     packages=['modProcesso'],
     url='https://github.com/flavioyuri/modProcesso',
     description='''modProcesso is a library for automata modularisation.''',
     long_description=readme,
```

