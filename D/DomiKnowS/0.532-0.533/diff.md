# Comparing `tmp/DomiKnowS-0.532.tar.gz` & `tmp/DomiKnowS-0.533.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DomiKnowS-0.532.tar", last modified: Sat Apr 15 02:19:04 2023, max compression
+gzip compressed data, was "DomiKnowS-0.533.tar", last modified: Sat Apr 15 03:29:10 2023, max compression
```

## Comparing `DomiKnowS-0.532.tar` & `DomiKnowS-0.533.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.450684 DomiKnowS-0.532/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.422683 DomiKnowS-0.532/DomiKnowS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-15 02:19:04.000000 DomiKnowS-0.532/DomiKnowS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-15 02:19:04.000000 DomiKnowS-0.532/DomiKnowS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 02:19:04.000000 DomiKnowS-0.532/DomiKnowS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-15 02:19:04.000000 DomiKnowS-0.532/DomiKnowS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-15 02:19:04.000000 DomiKnowS-0.532/DomiKnowS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-15 02:19:04.450684 DomiKnowS-0.532/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-15 02:18:54.000000 DomiKnowS-0.532/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.426683 DomiKnowS-0.532/domiknows/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14139 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.426683 DomiKnowS-0.532/domiknows/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/compiler/OntologyMLGraph.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/compiler/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.426683 DomiKnowS-0.532/domiknows/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.426683 DomiKnowS-0.532/domiknows/data/allennlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/data/allennlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/data/allennlp/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/data/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.430683 DomiKnowS-0.532/domiknows/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.430683 DomiKnowS-0.532/domiknows/graph/allennlp/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/allennlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18149 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/allennlp/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11710 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/allennlp/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12506 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/allennlp/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    19624 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/allennlp/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/concept.py
--rw-r--r--   0 runner    (1001) docker     (123)   107933 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/dataNode.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/dataNodeConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    27042 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/logicalConstrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.434683 DomiKnowS-0.532/domiknows/program/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/batchprogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/callbackprogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/lossprogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.434683 DomiKnowS-0.532/domiknows/program/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/model/ilpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/model/iml.py
--rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/model/lossModel.py
--rw-r--r--   0 runner    (1001) docker     (123)    18686 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/model/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/model/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/model_program.py
--rw-r--r--   0 runner    (1001) docker     (123)    13988 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.438684 DomiKnowS-0.532/domiknows/sensor/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.438684 DomiKnowS-0.532/domiknows/sensor/allennlp/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/allennlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/allennlp/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/allennlp/learner.py
--rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/allennlp/module.py
--rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/allennlp/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.438684 DomiKnowS-0.532/domiknows/sensor/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/pytorch/learnerModels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/pytorch/learners.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/pytorch/query_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/pytorch/relation_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)    24604 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/pytorch/sensors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.442684 DomiKnowS-0.532/domiknows/sensor/pytorch/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/pytorch/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/pytorch/tokenizers/spacy.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/pytorch/tokenizers/transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.442684 DomiKnowS-0.532/domiknows/sensor/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/torch/learner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/torch/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.446684 DomiKnowS-0.532/domiknows/solver/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/allennlpInferenceSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/allennlplogInferenceSolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.446684 DomiKnowS-0.532/domiknows/solver/constructor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/constructor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/constructor/constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/dummyILPOntSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/gekkoILPBooleanMethods.py
--rw-r--r--   0 runner    (1001) docker     (123)    38888 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/gekkoILPOntSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    38508 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/gurobiILPBooleanMethods.py
--rw-r--r--   0 runner    (1001) docker     (123)   107605 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/gurobiILPOntSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/ilpBooleanMethods.py
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/ilpBooleanMethodsCalculator.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/ilpConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/ilpOntSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/ilpOntSolverFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)    16520 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/lcLossBooleanMethods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7343 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/lcLossSampleBooleanMethods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/mini_solver_debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.446684 DomiKnowS-0.532/domiknows/solver/session/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/session/gurobi_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/session/solver_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 02:19:04.450684 DomiKnowS-0.532/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-15 02:18:54.000000 DomiKnowS-0.532/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.608038 DomiKnowS-0.533/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.600038 DomiKnowS-0.533/DomiKnowS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-15 03:29:10.000000 DomiKnowS-0.533/DomiKnowS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-15 03:29:10.000000 DomiKnowS-0.533/DomiKnowS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 03:29:10.000000 DomiKnowS-0.533/DomiKnowS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-15 03:29:10.000000 DomiKnowS-0.533/DomiKnowS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-15 03:29:10.000000 DomiKnowS-0.533/DomiKnowS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-15 03:29:10.608038 DomiKnowS-0.533/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-15 03:28:05.000000 DomiKnowS-0.533/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.600038 DomiKnowS-0.533/domiknows/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14139 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.600038 DomiKnowS-0.533/domiknows/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/compiler/OntologyMLGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/compiler/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.600038 DomiKnowS-0.533/domiknows/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.600038 DomiKnowS-0.533/domiknows/data/allennlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/data/allennlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/data/allennlp/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/data/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.604038 DomiKnowS-0.533/domiknows/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.604038 DomiKnowS-0.533/domiknows/graph/allennlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/allennlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18149 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/allennlp/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11710 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/allennlp/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12506 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/allennlp/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19624 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/allennlp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/concept.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107933 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/dataNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/dataNodeConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27042 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/logicalConstrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/graph/trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.604038 DomiKnowS-0.533/domiknows/program/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/batchprogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/callbackprogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/lossprogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.604038 DomiKnowS-0.533/domiknows/program/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/model/ilpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/model/iml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/model/lossModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18686 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/model/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/model/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/model_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13988 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/program/tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.604038 DomiKnowS-0.533/domiknows/sensor/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.604038 DomiKnowS-0.533/domiknows/sensor/allennlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/allennlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/allennlp/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/allennlp/learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/allennlp/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/allennlp/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.604038 DomiKnowS-0.533/domiknows/sensor/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/pytorch/learnerModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/pytorch/learners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/pytorch/query_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/pytorch/relation_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24604 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/pytorch/sensors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.604038 DomiKnowS-0.533/domiknows/sensor/pytorch/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/pytorch/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/pytorch/tokenizers/spacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/pytorch/tokenizers/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.608038 DomiKnowS-0.533/domiknows/sensor/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/torch/learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/sensor/torch/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.608038 DomiKnowS-0.533/domiknows/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/allennlpInferenceSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/allennlplogInferenceSolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.608038 DomiKnowS-0.533/domiknows/solver/constructor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/constructor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/constructor/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/dummyILPOntSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/gekkoILPBooleanMethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38888 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/gekkoILPOntSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38508 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/gurobiILPBooleanMethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107605 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/gurobiILPOntSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/ilpBooleanMethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/ilpBooleanMethodsCalculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/ilpConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/ilpOntSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/ilpOntSolverFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16520 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/lcLossBooleanMethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7343 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/lcLossSampleBooleanMethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/mini_solver_debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:29:10.608038 DomiKnowS-0.533/domiknows/solver/session/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/session/gurobi_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/session/solver_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/solver/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-04-15 03:28:05.000000 DomiKnowS-0.533/domiknows/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 03:29:10.608038 DomiKnowS-0.533/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-15 03:28:05.000000 DomiKnowS-0.533/setup.py
```

### Comparing `DomiKnowS-0.532/DomiKnowS.egg-info/PKG-INFO` & `DomiKnowS-0.533/DomiKnowS.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DomiKnowS
-Version: 0.532
+Version: 0.533
 Summary: A library provides integration between Domain Knowledge and Deep Learning.
 Home-page: https://github.com/HLR/DomiKnowS
 Author: Andrzej Uszok
 Author-email: auszok@ihmc.org
 License: MIT
 Description: The library allows to specify a problem domain with a conceptual [graph](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/KNOWLEDGE.md#graph) including declarations of edges and nodes, as well as [logical constraints](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/KNOWLEDGE.md#constraints) on the graph concepts and relations. [Neural network](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/MODEL.md#model-declaration) outputs bounded to the graph edges and nodes. The logical constraints are converted to ILP and Gurobi Solver is used for inferring. This adds a relational overlay over elements in a network that relates physical concepts in applications. <br> <br> The example running in Google CoLab environment, presenting the usage of the library is [here](https://colab.research.google.com/drive/1FvdePHv3h3NDSTkBw1VKwAmaZFWuGgTi).
 Platform: UNKNOWN
```

### Comparing `DomiKnowS-0.532/DomiKnowS.egg-info/SOURCES.txt` & `DomiKnowS-0.533/DomiKnowS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/PKG-INFO` & `DomiKnowS-0.533/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DomiKnowS
-Version: 0.532
+Version: 0.533
 Summary: A library provides integration between Domain Knowledge and Deep Learning.
 Home-page: https://github.com/HLR/DomiKnowS
 Author: Andrzej Uszok
 Author-email: auszok@ihmc.org
 License: MIT
 Description: The library allows to specify a problem domain with a conceptual [graph](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/KNOWLEDGE.md#graph) including declarations of edges and nodes, as well as [logical constraints](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/KNOWLEDGE.md#constraints) on the graph concepts and relations. [Neural network](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/MODEL.md#model-declaration) outputs bounded to the graph edges and nodes. The logical constraints are converted to ILP and Gurobi Solver is used for inferring. This adds a relational overlay over elements in a network that relates physical concepts in applications. <br> <br> The example running in Google CoLab environment, presenting the usage of the library is [here](https://colab.research.google.com/drive/1FvdePHv3h3NDSTkBw1VKwAmaZFWuGgTi).
 Platform: UNKNOWN
```

### Comparing `DomiKnowS-0.532/README.md` & `DomiKnowS-0.533/README.md`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/base.py` & `DomiKnowS-0.533/domiknows/base.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/compiler/OntologyMLGraph.py` & `DomiKnowS-0.533/domiknows/compiler/OntologyMLGraph.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/data/allennlp/reader.py` & `DomiKnowS-0.533/domiknows/data/allennlp/reader.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/data/reader.py` & `DomiKnowS-0.533/domiknows/data/reader.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/graph/allennlp/base.py` & `DomiKnowS-0.533/domiknows/graph/allennlp/base.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/graph/allennlp/metrics.py` & `DomiKnowS-0.533/domiknows/graph/allennlp/metrics.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/graph/allennlp/model.py` & `DomiKnowS-0.533/domiknows/graph/allennlp/model.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/graph/allennlp/utils.py` & `DomiKnowS-0.533/domiknows/graph/allennlp/utils.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/graph/base.py` & `DomiKnowS-0.533/domiknows/graph/base.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/graph/concept.py` & `DomiKnowS-0.533/domiknows/graph/concept.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/graph/dataNode.py` & `DomiKnowS-0.533/domiknows/graph/dataNode.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/graph/graph.py` & `DomiKnowS-0.533/domiknows/graph/graph.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/graph/logicalConstrain.py` & `DomiKnowS-0.533/domiknows/graph/logicalConstrain.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/graph/property.py` & `DomiKnowS-0.533/domiknows/graph/property.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/graph/relation.py` & `DomiKnowS-0.533/domiknows/graph/relation.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/graph/trial.py` & `DomiKnowS-0.533/domiknows/graph/trial.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/program/batchprogram.py` & `DomiKnowS-0.533/domiknows/program/batchprogram.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/program/callbackprogram.py` & `DomiKnowS-0.533/domiknows/program/callbackprogram.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/program/loss.py` & `DomiKnowS-0.533/domiknows/program/loss.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/program/lossprogram.py` & `DomiKnowS-0.533/domiknows/program/lossprogram.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/program/metric.py` & `DomiKnowS-0.533/domiknows/program/metric.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/program/model/ilpu.py` & `DomiKnowS-0.533/domiknows/program/model/ilpu.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/program/model/iml.py` & `DomiKnowS-0.533/domiknows/program/model/iml.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/program/model/lossModel.py` & `DomiKnowS-0.533/domiknows/program/model/lossModel.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/program/model/pytorch.py` & `DomiKnowS-0.533/domiknows/program/model/pytorch.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/program/model/torch.py` & `DomiKnowS-0.533/domiknows/program/model/torch.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/program/model_program.py` & `DomiKnowS-0.533/domiknows/program/model_program.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/program/program.py` & `DomiKnowS-0.533/domiknows/program/program.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/program/tracker.py` & `DomiKnowS-0.533/domiknows/program/tracker.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/sensor/allennlp/base.py` & `DomiKnowS-0.533/domiknows/sensor/allennlp/base.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/sensor/allennlp/learner.py` & `DomiKnowS-0.533/domiknows/sensor/allennlp/learner.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/sensor/allennlp/module.py` & `DomiKnowS-0.533/domiknows/sensor/allennlp/module.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/sensor/allennlp/sensor.py` & `DomiKnowS-0.533/domiknows/sensor/allennlp/sensor.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/sensor/pytorch/learnerModels.py` & `DomiKnowS-0.533/domiknows/sensor/pytorch/learnerModels.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/sensor/pytorch/learners.py` & `DomiKnowS-0.533/domiknows/sensor/pytorch/learners.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/sensor/pytorch/query_sensor.py` & `DomiKnowS-0.533/domiknows/sensor/pytorch/query_sensor.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/sensor/pytorch/relation_sensors.py` & `DomiKnowS-0.533/domiknows/sensor/pytorch/relation_sensors.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/sensor/pytorch/sensors.py` & `DomiKnowS-0.533/domiknows/sensor/pytorch/sensors.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/sensor/pytorch/tokenizers/spacy.py` & `DomiKnowS-0.533/domiknows/sensor/pytorch/tokenizers/spacy.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/sensor/pytorch/tokenizers/transformers.py` & `DomiKnowS-0.533/domiknows/sensor/pytorch/tokenizers/transformers.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/sensor/pytorch/utils.py` & `DomiKnowS-0.533/domiknows/sensor/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/sensor/sensor.py` & `DomiKnowS-0.533/domiknows/sensor/sensor.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/sensor/torch/learner.py` & `DomiKnowS-0.533/domiknows/sensor/torch/learner.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/sensor/torch/sensor.py` & `DomiKnowS-0.533/domiknows/sensor/torch/sensor.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/solver/allennlpInferenceSolver.py` & `DomiKnowS-0.533/domiknows/solver/allennlpInferenceSolver.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/solver/allennlplogInferenceSolver.py` & `DomiKnowS-0.533/domiknows/solver/allennlplogInferenceSolver.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/solver/constructor/constructor.py` & `DomiKnowS-0.533/domiknows/solver/constructor/constructor.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/solver/dummyILPOntSolver.py` & `DomiKnowS-0.533/domiknows/solver/dummyILPOntSolver.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/solver/gekkoILPBooleanMethods.py` & `DomiKnowS-0.533/domiknows/solver/gekkoILPBooleanMethods.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/solver/gekkoILPOntSolver.py` & `DomiKnowS-0.533/domiknows/solver/gekkoILPOntSolver.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/solver/gurobiILPBooleanMethods.py` & `DomiKnowS-0.533/domiknows/solver/gurobiILPBooleanMethods.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/solver/gurobiILPOntSolver.py` & `DomiKnowS-0.533/domiknows/solver/gurobiILPOntSolver.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/solver/ilpBooleanMethods.py` & `DomiKnowS-0.533/domiknows/solver/ilpBooleanMethods.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/solver/ilpBooleanMethodsCalculator.py` & `DomiKnowS-0.533/domiknows/solver/ilpBooleanMethodsCalculator.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/solver/ilpOntSolver.py` & `DomiKnowS-0.533/domiknows/solver/ilpOntSolver.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/solver/ilpOntSolverFactory.py` & `DomiKnowS-0.533/domiknows/solver/ilpOntSolverFactory.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/solver/lcLossBooleanMethods.py` & `DomiKnowS-0.533/domiknows/solver/lcLossBooleanMethods.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/solver/lcLossSampleBooleanMethods.py` & `DomiKnowS-0.533/domiknows/solver/lcLossSampleBooleanMethods.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/solver/mini_solver_debug.py` & `DomiKnowS-0.533/domiknows/solver/mini_solver_debug.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/solver/session/gurobi_session.py` & `DomiKnowS-0.533/domiknows/solver/session/gurobi_session.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/solver/session/solver_session.py` & `DomiKnowS-0.533/domiknows/solver/session/solver_session.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/domiknows/utils.py` & `DomiKnowS-0.533/domiknows/utils.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.532/setup.py` & `DomiKnowS-0.533/setup.py`

 * *Files identical despite different names*

