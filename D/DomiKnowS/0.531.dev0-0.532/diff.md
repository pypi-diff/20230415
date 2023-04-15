# Comparing `tmp/DomiKnowS-0.531.dev0.tar.gz` & `tmp/DomiKnowS-0.532.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DomiKnowS-0.531.dev0.tar", last modified: Thu Apr 13 18:00:05 2023, max compression
+gzip compressed data, was "DomiKnowS-0.532.tar", last modified: Sat Apr 15 02:19:04 2023, max compression
```

## Comparing `DomiKnowS-0.531.dev0.tar` & `DomiKnowS-0.532.tar`

### file list

```diff
@@ -1,114 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:05.892777 DomiKnowS-0.531.dev0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:05.880776 DomiKnowS-0.531.dev0/DomiKnowS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-13 18:00:05.000000 DomiKnowS-0.531.dev0/DomiKnowS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-13 18:00:05.000000 DomiKnowS-0.531.dev0/DomiKnowS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:00:05.000000 DomiKnowS-0.531.dev0/DomiKnowS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-13 18:00:05.000000 DomiKnowS-0.531.dev0/DomiKnowS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 18:00:05.000000 DomiKnowS-0.531.dev0/DomiKnowS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-13 18:00:05.892777 DomiKnowS-0.531.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:05.880776 DomiKnowS-0.531.dev0/domiknows/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14139 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:05.880776 DomiKnowS-0.531.dev0/domiknows/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/compiler/OntologyMLGraph.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/compiler/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:05.884777 DomiKnowS-0.531.dev0/domiknows/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:05.884777 DomiKnowS-0.531.dev0/domiknows/data/allennlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/data/allennlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/data/allennlp/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/data/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:05.884777 DomiKnowS-0.531.dev0/domiknows/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/graph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:05.884777 DomiKnowS-0.531.dev0/domiknows/graph/allennlp/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/graph/allennlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18149 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/graph/allennlp/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11710 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/graph/allennlp/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12506 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/graph/allennlp/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    19624 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/graph/allennlp/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/graph/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/graph/candidates.py
--rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/graph/concept.py
--rw-r--r--   0 runner    (1001) docker     (123)   108934 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/graph/dataNode.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/graph/dataNodeConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    31317 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/graph/logicalConstrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/graph/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/graph/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/graph/trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:05.884777 DomiKnowS-0.531.dev0/domiknows/program/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/program/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/program/batchprogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/program/callbackprogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/program/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    13778 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/program/lossprogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/program/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:05.888777 DomiKnowS-0.531.dev0/domiknows/program/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/program/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/program/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/program/model/gbi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/program/model/ilpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/program/model/iml.py
--rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/program/model/lossModel.py
--rw-r--r--   0 runner    (1001) docker     (123)    18808 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/program/model/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/program/model/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/program/model_program.py
--rw-r--r--   0 runner    (1001) docker     (123)    13988 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/program/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/program/tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:05.888777 DomiKnowS-0.531.dev0/domiknows/sensor/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/sensor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:05.888777 DomiKnowS-0.531.dev0/domiknows/sensor/allennlp/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/sensor/allennlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/sensor/allennlp/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/sensor/allennlp/learner.py
--rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/sensor/allennlp/module.py
--rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/sensor/allennlp/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/sensor/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:05.888777 DomiKnowS-0.531.dev0/domiknows/sensor/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/sensor/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/sensor/pytorch/learnerModels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/sensor/pytorch/learners.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/sensor/pytorch/query_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/sensor/pytorch/relation_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)    24604 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/sensor/pytorch/sensors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:05.888777 DomiKnowS-0.531.dev0/domiknows/sensor/pytorch/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/sensor/pytorch/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/sensor/pytorch/tokenizers/spacy.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/sensor/pytorch/tokenizers/transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/sensor/pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/sensor/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:05.888777 DomiKnowS-0.531.dev0/domiknows/sensor/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/sensor/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/sensor/torch/learner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/sensor/torch/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:05.892777 DomiKnowS-0.531.dev0/domiknows/solver/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/solver/allennlpInferenceSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/solver/allennlplogInferenceSolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:05.892777 DomiKnowS-0.531.dev0/domiknows/solver/constructor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/solver/constructor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/solver/constructor/constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/solver/dummyILPOntSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/solver/gekkoILPBooleanMethods.py
--rw-r--r--   0 runner    (1001) docker     (123)    38888 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/solver/gekkoILPOntSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    38508 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/solver/gurobiILPBooleanMethods.py
--rw-r--r--   0 runner    (1001) docker     (123)   102640 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/solver/gurobiILPOntSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/solver/ilpBooleanMethods.py
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/solver/ilpBooleanMethodsCalculator.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/solver/ilpConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/solver/ilpOntSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/solver/ilpOntSolverFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)    16520 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/solver/lcLossBooleanMethods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7343 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/solver/lcLossSampleBooleanMethods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/solver/mini_solver_debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:00:05.892777 DomiKnowS-0.531.dev0/domiknows/solver/session/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/solver/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/solver/session/gurobi_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/solver/session/solver_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/solver/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/domiknows/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 18:00:05.892777 DomiKnowS-0.531.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-13 17:59:54.000000 DomiKnowS-0.531.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.450684 DomiKnowS-0.532/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.422683 DomiKnowS-0.532/DomiKnowS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-15 02:19:04.000000 DomiKnowS-0.532/DomiKnowS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-15 02:19:04.000000 DomiKnowS-0.532/DomiKnowS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 02:19:04.000000 DomiKnowS-0.532/DomiKnowS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-15 02:19:04.000000 DomiKnowS-0.532/DomiKnowS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-15 02:19:04.000000 DomiKnowS-0.532/DomiKnowS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-15 02:19:04.450684 DomiKnowS-0.532/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-15 02:18:54.000000 DomiKnowS-0.532/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.426683 DomiKnowS-0.532/domiknows/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14139 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.426683 DomiKnowS-0.532/domiknows/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/compiler/OntologyMLGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/compiler/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.426683 DomiKnowS-0.532/domiknows/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.426683 DomiKnowS-0.532/domiknows/data/allennlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/data/allennlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/data/allennlp/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/data/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.430683 DomiKnowS-0.532/domiknows/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.430683 DomiKnowS-0.532/domiknows/graph/allennlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/allennlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18149 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/allennlp/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11710 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/allennlp/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12506 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/allennlp/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19624 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/allennlp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/concept.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107933 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/dataNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/dataNodeConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27042 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/logicalConstrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/graph/trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.434683 DomiKnowS-0.532/domiknows/program/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/batchprogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/callbackprogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/lossprogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.434683 DomiKnowS-0.532/domiknows/program/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/model/ilpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/model/iml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/model/lossModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18686 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/model/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/model/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/model_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13988 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/program/tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.438684 DomiKnowS-0.532/domiknows/sensor/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.438684 DomiKnowS-0.532/domiknows/sensor/allennlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/allennlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/allennlp/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/allennlp/learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/allennlp/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/allennlp/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.438684 DomiKnowS-0.532/domiknows/sensor/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/pytorch/learnerModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/pytorch/learners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/pytorch/query_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/pytorch/relation_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24604 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/pytorch/sensors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.442684 DomiKnowS-0.532/domiknows/sensor/pytorch/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/pytorch/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/pytorch/tokenizers/spacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/pytorch/tokenizers/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.442684 DomiKnowS-0.532/domiknows/sensor/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/torch/learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/sensor/torch/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.446684 DomiKnowS-0.532/domiknows/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/allennlpInferenceSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/allennlplogInferenceSolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.446684 DomiKnowS-0.532/domiknows/solver/constructor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/constructor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/constructor/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/dummyILPOntSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/gekkoILPBooleanMethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38888 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/gekkoILPOntSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38508 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/gurobiILPBooleanMethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107605 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/gurobiILPOntSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/ilpBooleanMethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/ilpBooleanMethodsCalculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/ilpConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/ilpOntSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/ilpOntSolverFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16520 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/lcLossBooleanMethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7343 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/lcLossSampleBooleanMethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/mini_solver_debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 02:19:04.446684 DomiKnowS-0.532/domiknows/solver/session/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/session/gurobi_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/session/solver_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/solver/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-04-15 02:18:54.000000 DomiKnowS-0.532/domiknows/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 02:19:04.450684 DomiKnowS-0.532/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-15 02:18:54.000000 DomiKnowS-0.532/setup.py
```

### Comparing `DomiKnowS-0.531.dev0/DomiKnowS.egg-info/PKG-INFO` & `DomiKnowS-0.532/DomiKnowS.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DomiKnowS
-Version: 0.531.dev0
+Version: 0.532
 Summary: A library provides integration between Domain Knowledge and Deep Learning.
 Home-page: https://github.com/HLR/DomiKnowS
 Author: Andrzej Uszok
 Author-email: auszok@ihmc.org
 License: MIT
 Description: The library allows to specify a problem domain with a conceptual [graph](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/KNOWLEDGE.md#graph) including declarations of edges and nodes, as well as [logical constraints](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/KNOWLEDGE.md#constraints) on the graph concepts and relations. [Neural network](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/MODEL.md#model-declaration) outputs bounded to the graph edges and nodes. The logical constraints are converted to ILP and Gurobi Solver is used for inferring. This adds a relational overlay over elements in a network that relates physical concepts in applications. <br> <br> The example running in Google CoLab environment, presenting the usage of the library is [here](https://colab.research.google.com/drive/1FvdePHv3h3NDSTkBw1VKwAmaZFWuGgTi).
 Platform: UNKNOWN
```

### Comparing `DomiKnowS-0.531.dev0/DomiKnowS.egg-info/SOURCES.txt` & `DomiKnowS-0.532/DomiKnowS.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 domiknows/compiler/compiler.py
 domiknows/data/__init__.py
 domiknows/data/reader.py
 domiknows/data/allennlp/__init__.py
 domiknows/data/allennlp/reader.py
 domiknows/graph/__init__.py
 domiknows/graph/base.py
-domiknows/graph/candidates.py
 domiknows/graph/concept.py
 domiknows/graph/dataNode.py
 domiknows/graph/dataNodeConfig.py
 domiknows/graph/graph.py
 domiknows/graph/logicalConstrain.py
 domiknows/graph/property.py
 domiknows/graph/relation.py
@@ -39,15 +38,14 @@
 domiknows/program/lossprogram.py
 domiknows/program/metric.py
 domiknows/program/model_program.py
 domiknows/program/program.py
 domiknows/program/tracker.py
 domiknows/program/model/__init__.py
 domiknows/program/model/base.py
-domiknows/program/model/gbi.py
 domiknows/program/model/ilpu.py
 domiknows/program/model/iml.py
 domiknows/program/model/lossModel.py
 domiknows/program/model/pytorch.py
 domiknows/program/model/torch.py
 domiknows/sensor/__init__.py
 domiknows/sensor/learner.py
```

### Comparing `DomiKnowS-0.531.dev0/PKG-INFO` & `DomiKnowS-0.532/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DomiKnowS
-Version: 0.531.dev0
+Version: 0.532
 Summary: A library provides integration between Domain Knowledge and Deep Learning.
 Home-page: https://github.com/HLR/DomiKnowS
 Author: Andrzej Uszok
 Author-email: auszok@ihmc.org
 License: MIT
 Description: The library allows to specify a problem domain with a conceptual [graph](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/KNOWLEDGE.md#graph) including declarations of edges and nodes, as well as [logical constraints](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/KNOWLEDGE.md#constraints) on the graph concepts and relations. [Neural network](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/MODEL.md#model-declaration) outputs bounded to the graph edges and nodes. The logical constraints are converted to ILP and Gurobi Solver is used for inferring. This adds a relational overlay over elements in a network that relates physical concepts in applications. <br> <br> The example running in Google CoLab environment, presenting the usage of the library is [here](https://colab.research.google.com/drive/1FvdePHv3h3NDSTkBw1VKwAmaZFWuGgTi).
 Platform: UNKNOWN
```

### Comparing `DomiKnowS-0.531.dev0/README.md` & `DomiKnowS-0.532/README.md`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/base.py` & `DomiKnowS-0.532/domiknows/base.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/compiler/OntologyMLGraph.py` & `DomiKnowS-0.532/domiknows/compiler/OntologyMLGraph.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/data/allennlp/reader.py` & `DomiKnowS-0.532/domiknows/data/allennlp/reader.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/data/reader.py` & `DomiKnowS-0.532/domiknows/data/reader.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/graph/allennlp/base.py` & `DomiKnowS-0.532/domiknows/graph/allennlp/base.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/graph/allennlp/metrics.py` & `DomiKnowS-0.532/domiknows/graph/allennlp/metrics.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/graph/allennlp/model.py` & `DomiKnowS-0.532/domiknows/graph/allennlp/model.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/graph/allennlp/utils.py` & `DomiKnowS-0.532/domiknows/graph/allennlp/utils.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/graph/base.py` & `DomiKnowS-0.532/domiknows/graph/base.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/graph/concept.py` & `DomiKnowS-0.532/domiknows/graph/concept.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/graph/dataNode.py` & `DomiKnowS-0.532/domiknows/graph/dataNode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import torch
 from collections import OrderedDict, namedtuple
-from time import process_time_ns
+from  time import process_time_ns
 import re
-
 from .dataNodeConfig import dnConfig 
 
 from ordered_set import OrderedSet 
 
 from domiknows import getRegrTimer_logger, getProductionModeStatus
 from domiknows.graph.logicalConstrain import eqL
 from domiknows.solver import ilpOntSolverFactory
@@ -73,16 +72,14 @@
 # Class representing single data instance with relation links to other data nodes
 class DataNode:
     def __init__(self, instanceID = None, instanceValue = None, ontologyNode = None, relationLinks = {}, attributes = {}):
 
         self.instanceID = instanceID                     # The data instance id (e.g. paragraph number, sentence number, phrase  number, image number, etc.)
         self.instanceValue = instanceValue               # Optional value of the instance (e.g. paragraph text, sentence text, phrase text, image bitmap, etc.)
         self.ontologyNode = ontologyNode                 # Reference to the node in the ontology graph (e.g. Concept) which is the type of this instance (e.g. paragraph, sentence, phrase, etc.)
-        
-        self.graph =  self.ontologyNode.sup
         if relationLinks:
             self.relationLinks = relationLinks           # Dictionary mapping relation name to RealtionLinks
         else:
             self.relationLinks = {}
             
         self.impactLinks = {}                            # Dictionary with dataNodes impacting this dataNode by having it as a subject of its relation
         
@@ -843,16 +840,14 @@
             path0 = path[0].e[0][0]
         else:
             path0 = path[0]
 
         relDns = None         
         if self.isRelation(path0):
             relDns = self.getDnsForRelation(path0)
-        elif isinstance(path0, str):
-            relDns = self.getDnsForRelation(path0)
         else: # if not relation then has to be attribute in eql
             attributeValue = self.getAttribute(path[0].e[1]).item()
             requiredValue = path[0].e[2]
              
             if attributeValue in requiredValue:
                 return [self]
             elif (True in  requiredValue ) and attributeValue == 1:
@@ -1148,27 +1143,14 @@
         
         # Call ilpOntsolver with the collected probabilities for chosen candidates
         _DataNode__Logger.info("Calling ILP solver")
         
         self.inferLocal()
         myilpOntSolver.calculateILPSelection(self, *conceptsRelations, fun=fun, epsilon = epsilon, minimizeObjective = minimizeObjective, ignorePinLCs = ignorePinLCs)    
         
-    def inferGBIResults(self, *_conceptsRelations, model, builder):
-        if len(_conceptsRelations) == 0:
-            _DataNode__Logger.info('Called with empty list of concepts and relations for inference')
-        else:
-            _DataNode__Logger.info('Called with - %s - list of concepts and relations for inference'%([x.name if isinstance(x, Concept) else x for x in _conceptsRelations]))
-            
-        # Check if concepts and/or relations have been provided for inference, if provide translate then to tuple concept info form
-        _conceptsRelations = self.collectConceptsAndRelations(_conceptsRelations) # Collect all concepts and relations from graph as default set
-
-        from domiknows.program.model.gbi import GBIModel
-        myGBIModel = GBIModel(self.graph, model)
-        myGBIModel.calculateGBISelection(builder, _conceptsRelations)
-        
     # Calculate the percentage of results satisfying each logical constraint 
     def verifyResultsLC(self, key = "/local/argmax"):
                 
         myilpOntSolver, _ = self.__getILPSolver(conceptsRelations = self.collectConceptsAndRelations())
 
         self.inferLocal()
         self.infer()
@@ -1616,15 +1598,15 @@
         isRoot = True    
         for _, iDnList in testedDn.impactLinks.items(): # Check if its impacts are connected to Dn in the new Root list
             if iDnList:
                 for iDn in iDnList:
                     if iDn in visitedDns:
                         continue
                     
-                    if self.__isRootDn(iDn, checkedDns, visitedDns):
+                    if not self.__isRootDn(iDn, checkedDns, visitedDns):
                         isRoot = False
                         break
                     
             if not isRoot:
                 break
             
         return isRoot
@@ -1716,15 +1698,15 @@
             # Find if all the needed attribute were initialized
             allAttrInit = True
             for relationAttributeName, _ in conceptInfo['relationAttrsGraph'].items():
                 if relationAttributeName not in relationAttrsCache:
                     allAttrInit = False
                     break
             
-            if allAttrInit: #Create links for the relation DataNode
+            if allAttrInit: #Create links for the ralation DataNode
                 # Find DataNodes connected by this relation based on graph definition
                 existingDnsForAttr = OrderedDict() # DataNodes for Attributes of the relation
                 for relationAttributeName, relationAttributeConcept in conceptInfo['relationAttrsGraph'].items():
                     _existingDnsForAttr = self.findDataNodesInBuilder(select = relationAttributeConcept.name)
                      
                     if _existingDnsForAttr:
                         existingDnsForAttr[relationAttributeName] = _existingDnsForAttr
@@ -1745,15 +1727,15 @@
                             isInRelation = candidate.item()
                             if isInRelation == 0:
                                 continue
                             
                             candidateDn = existingDnsForAttr[attribute][candidateIndex]
                             
                             if attributeIndex == 0:
-                                candidateDn.addRelationLink(attribute, relationDn)
+                                candidateDn.addRelationLink(relationName, relationDn)
                             
                             relationDn.addRelationLink(attribute, candidateDn)  
                             relationDn.attributes[keyDataName] = vInfo.value[relationDnIndex] # Add / /Update value of the attribute
                 
                 _DataNodeBulder__Logger.info('Create links between the relation %s and instance dataNode of types'%(conceptInfo['concept'].name))
             else:
                 # Just add the sensor value to relation DataNodes
@@ -1775,15 +1757,15 @@
  
             if len(existingDnsForRelation) != vInfo.len:
                 _DataNodeBulder__Logger.error('Number of relations is %i and is different then the length of the provided tensor %i'%(len(existingDnsForRelation),vInfo.len))
                 raise ValueError('Number of relations is %i and is different then the length of the provided tensor %i'%(len(existingDnsForRelation),vInfo.len))
  
             if len(existingDnsForRelationSorted) == 1:
                 if vInfo.dim == 0:
-                    existingDnsForRelationSorted[0].attributes[keyDataName] = vInfo.value # Add / /Update value of the attribute
+                    existingDnsForRelationSorted[0].attributes[keyDataName] = vInfo.value.item() # Add / /Update value of the attribute
             elif vInfo.dim > 0:
                 for i, rDn in existingDnsForRelationSorted.items(): # Loop through all relations links dataNodes
                     rDn.attributes[keyDataName] = vInfo.value[i] # Add / /Update value of the attribute
             else:
                 pass
 
     def __createInitialdDataNode(self, vInfo, conceptInfo, keyDataName):
```

### Comparing `DomiKnowS-0.531.dev0/domiknows/graph/graph.py` & `DomiKnowS-0.532/domiknows/graph/graph.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/graph/logicalConstrain.py` & `DomiKnowS-0.532/domiknows/graph/logicalConstrain.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,23 +5,27 @@
 import logging
 import torch
 myLogger = logging.getLogger(ilpConfig['log_name'])
 ifLog =  ilpConfig['ifLog']
         
 V = namedtuple("V", ['name', 'v'], defaults= [None, None])
 
-class LcElement:
-    def __init__(self, *e,  name = None):
+class LogicalConstrain:
+    def __init__(self, *e, p=100, active = True, sampleEntries  = False, name = None):
+        self.headLC = True # Indicate that it is head constrain and should be process individually
+        self.active = active
+        self.sampleEntries = sampleEntries
+        
         if not e:
-            myLogger.error("Logical Element initialized is empty")
-            raise LcElement.LcElementError("Logical Element initialized is empty")
+            myLogger.error("Logical Constraint initialized is empty")
+            raise LogicalConstrain.LogicalConstrainError("Logical Constraint initialized is empty")
         
         updatedE = []
         for _, eItem in enumerate(e):
-            if isinstance(eItem, (LcElement, Concept)):
+            if isinstance(eItem, (LogicalConstrain, Concept)):
                 updatedE.append(eItem)
             elif callable(eItem):
                 newEItem = eItem.__call__()
                 updatedE.extend(newEItem)
             elif isinstance(eItem, list):
                 updatedE.extend(eItem)
             else:
@@ -34,97 +38,87 @@
             if isinstance(eItem, Concept):
                 updatedE.append((eItem, eItem.name, None, 1))
             else:
                 updatedE.append(eItem)
                 
         self.e = updatedE
 
-        # -- Find the graph for this Logical Element - based on context defined in the concept used in constraint definition
+        # -- Find the graph for this Logical Constraint - based on context defined in the concept used in constrain definition
         self.graph = None
        
         conceptOrLc = None
         
         for _, eItem in enumerate(self.e):
-            if isinstance(eItem, LcElement):
+            if isinstance(eItem, LogicalConstrain):
                 conceptOrLc = eItem
                 break
             elif isinstance(eItem, tuple):
-                if isinstance(eItem[0], Concept):
-                    conceptOrLc = eItem[0]
-                    break
+                conceptOrLc = eItem[0]
+                break
     
         if conceptOrLc is None:
-            myLogger.error("Logical Element is incorrect")
-            raise LcElement.LcElementError("Logical Element is incorrect")
+            myLogger.error("Logical Constraint is incorrect")
+            raise LogicalConstrain.LogicalConstrainError("Logical Constraint is incorrect")
             
         if isinstance(conceptOrLc, Concept):
             if self.__getContext(conceptOrLc):
                 self.graph = self.__getContext(conceptOrLc)[-1]
         elif isinstance(conceptOrLc, str):
             self.graph = None
         else:
             self.graph = conceptOrLc.graph
                 
         if self.graph == None:
-            myLogger.error("Logical Element initialized is not associated with graph")
-            raise LcElement.LcElementError("Logical Element initialized is not associated with graph")
+            myLogger.error("Logical Constraint initialized is not associated with graph")
+            raise LogicalConstrain.LogicalConstrainError("Logical Constraint initialized is not associated with graph")
                      
-        # Create Logical Element id based on number of existing Logical Element in the graph
+        # Create Logical Constraint id based on number of existing Logical Constraint in the graph
         self.lcName = "LC%i"%(len(self.graph.logicalConstrains))
         
         if name is not None:
             self.name = name
         else:
             self.name = self.lcName
-     
-    class LcElementError(Exception):
-        pass
-    
-    def __str__(self):
-        return self.__class__.__name__
-    
-    def __repr__(self):
-        return  self.lcName + '(' + self.__class__.__name__ + ')'
             
-    def __getContext(self, e):
-        if isinstance(e, LcElement):
-            return self.__getContext(e.e[0])
-        else:
-            return e._context
-
-class LogicalConstrain(LcElement):
-    def __init__(self, *e, p=100, active = True, sampleEntries  = False, name = None):
-        super().__init__(*e, name = name)
-        
-        self.headLC = True # Indicate that it is head constraint and should be process individually
-        self.active = active
-        self.sampleEntries = sampleEntries
-        
-        # Add the constraint to the graph
-        assert self.graph is not None
+        # Add the constrain to the graph
         self.graph.logicalConstrains[self.lcName] = self
-        
-         # Go though constraint, find nested constrains and change their property headLC to indicate that their are nested and should not be process individually
+                
+        # Go though constrain, find nested constrains and change their property headLC to indicate that their are nested and should not be process individually
         for e_item in self.e:
             if isinstance(e_item, LogicalConstrain):
                 e_item.headLC = False
                 
-        # Check soft constraint is activated though p - if certainty in the validity of the constraint or the user preference is provided by p
+        # Check soft constrain is activated though p - if certainty in the validity of the constrain or the user preference is provided by p
         if p < 0:
             self.p = 0
             myLogger.warning("%s Logical Constraint created with p equal %i sets it to 0"%(self.lcName,p))
         elif p > 100:
             self.p = 100
             myLogger.warning("%s Logical Constraint created with p equal %i sets it to 100"%(self.lcName,p))
         else:
             self.p = p
-        
+     
+    class LogicalConstrainError(Exception):
+        pass
+    
+    def __str__(self):
+        return self.__class__.__name__
+    
+    def __repr__(self):
+        return  self.lcName + '(' + self.__class__.__name__ + ')'
+          
     def __call__(self, model, myIlpBooleanProcessor, v): 
         pass 
-    
+            
+    def __getContext(self, e):
+        if isinstance(e, LogicalConstrain):
+            return self.__getContext(e.e[0])
+        else:
+            return e._context
+       
     def getLcConcepts(self):
         lcConcepts = set()
         
         for _, eItem in enumerate(self.e):
             if isinstance(eItem, V):
                 if eItem[1] and eItem[1][1]:
                     if isinstance(eItem[1][1], eqL):
@@ -135,15 +129,15 @@
             elif isinstance(eItem, LogicalConstrain):
                 lcConcepts.update(eItem.getLcConcepts())
             elif isinstance(eItem, tuple) and (len(eItem) == 4):
                 lcConcepts.add(eItem[0].name)
                 
         return lcConcepts
         
-    # Get string representation of  Logical Constraint
+    # Get string representation of  Logical Constraintt
     def strEs(self):
         strsE = []
         for _, eItem in enumerate(self.e):
             if isinstance(eItem, V):
                 new_V = []
                 if eItem[0] is not None:
                     new_V.append(eItem[0])
@@ -200,15 +194,15 @@
             for cv in currentILPVars:
                 singleVar = lcFun(model, cv, onlyConstrains = headConstrain)
                 cSingleVar.append(singleVar)
                 
             singleV.append(cSingleVar)
         
         if headConstrain:
-            if ifLog: myLogger.debug("%s Logical Constraint is the head constraint - only ILP constraint created"%(lcName))
+            if ifLog: myLogger.debug("%s Logical Constraint is the head constrain - only ILP constrain created"%(lcName))
         
         if model is not None:
             model.update()
         
         return singleV
     
     # Collects setups of ILP variables for logical methods calls for the created Logical Constraint - recursive method
@@ -319,97 +313,14 @@
                 
             rVars.append(tVars)
         
         # Return results from created ILP constraints - 
         # None if headConstrain is True or no ILP constraint created, ILP variable representing the value of ILP constraint, loss calculated
         return rVars
     
-    
-     # Collects combination setups of ILP variables for logical methods calls for the created Logical Constraint - recursive method
-    def _collectCombinationILPVariableSetups(self, lcVariableName, lcVariableNames, v, lcVars = []): 
-        
-        # Get set of ILP variables lists for the current variable name
-        cLcVariables = v[lcVariableName]
-        
-        # List of lists containing sets of ILP variables for particular position 
-        newLcVars = []
-        
-        # --- Update the lcVars setup with ILP variables from this iteration
-        
-        if not lcVars: # If ILP variables setup is not initialized yet - this is the first iteration of the _collectILPVariableSetups method
-            if cLcVariables is None:
-                newV = [[None]]
-                newLcVars.append(newV)
-            else:
-                for cV in cLcVariables:
-                    newV = []
-                    for cvElement in cV:
-                        if cvElement is None:
-                            pass
-                        newElement = [cvElement]
-                        newV.append(newElement)
-                    newLcVars.append(newV)
-        else: # Many ILP variables in the current set
-            for indexLcV, lcV in enumerate(lcVars):
-                newV = []
-                if cLcVariables is None:
-                    for _, lcVelement in enumerate(lcV):
-                        newLcVelement = lcVelement.copy()
-                        newLcVelement.append(None)
-                        
-                        newV.append(newLcVelement)
-                else:
-                    for cV in cLcVariables:
-                        for indexElement, lcVelement in enumerate(lcV):
-                        
-                            newLcVelement = lcVelement.copy()
-                            newLcVelement.append(cV[indexElement])
-                            
-                            newV.append(newLcVelement)
-                            
-                    newLcVars.append(newV)                
-                            
-        if lcVariableNames:
-            # Recursive call - lcVars contains currently collected ILP variables setups
-            return self._collectCombinationILPVariableSetups(lcVariableNames[0], lcVariableNames[1:], v, lcVars=newLcVars)
-        else:
-            # Return collected setups
-            return newLcVars
-
-    def createILPConstrainsCombination(self, lcName, lcFun, model, v, headConstrain):
-        if len(v) < 2:
-            myLogger.error("%s Logical Constraint created with %i sets of variables which is less then two"%(lcName, len(v)))
-            return None
-        
-        # Input variable names
-        try:
-            lcVariableNames = [e for e in iter(v)]
-        except StopIteration:
-            pass
-                
-        lcVariableName0 = lcVariableNames[0]
-
-        rVars = [] # Output variables
-            
-        # Collect variables setups for ILP constraints
-        sVar = self._collectCombinationILPVariableSetups(lcVariableName0, lcVariableNames[1:], v)
-        
-        # Apply collected setups and create ILP constraint
-        for z in sVar:
-            tVars = [] # Collect ILP constraints results
-            for t in z:
-                tVars.append(lcFun(model, *t, onlyConstrains = headConstrain))
-                
-            rVars.append(tVars)
-        
-        # Return results from created ILP constraints - 
-        # None if headConstrain is True or no ILP constraint created, ILP variable representing the value of ILP constraint, loss calculated
-        return rVars
-        
-
     def createILPCount(self, model, myIlpBooleanProcessor, v, headConstrain, cOperation, cLimit, integrate, logicMethodName = "COUNT"):         
         try:
             lcVariableNames = [e for e in iter(v)]
         except StopIteration:
             pass
         
         if cLimit== None:
@@ -698,19 +609,8 @@
             cLimit = self.e[-1]
         else:
             cLimit = 1
             
         cOperation = '<='
         
         with torch.set_grad_enabled(myIlpBooleanProcessor.grad):
-            return self.createILPAccumulatedCount(model, myIlpBooleanProcessor, v, headConstrain, cOperation, cLimit, integrate, logicMethodName = str(self))
-        
-# ----------------- forall
-class forAllL(LogicalConstrain):
-    def __init__(self, *e, p=100, active = True, sampleEntries = False, name = None):
-        LogicalConstrain.__init__(self, *e, p=p, active=active, sampleEntries  = sampleEntries, name=name)
-        
-    def __call__(self, model, myIlpBooleanProcessor, v, headConstrain = False, integrate = False): 
-        with torch.set_grad_enabled(myIlpBooleanProcessor.grad):
-            return self.createILPConstrains('If', myIlpBooleanProcessor.ifVar, model, v, headConstrain)        
-    
-        
+            return self.createILPAccumulatedCount(model, myIlpBooleanProcessor, v, headConstrain, cOperation, cLimit, integrate, logicMethodName = str(self))
```

### Comparing `DomiKnowS-0.531.dev0/domiknows/graph/property.py` & `DomiKnowS-0.532/domiknows/graph/property.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/graph/relation.py` & `DomiKnowS-0.532/domiknows/graph/relation.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/graph/trial.py` & `DomiKnowS-0.532/domiknows/graph/trial.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/program/batchprogram.py` & `DomiKnowS-0.532/domiknows/program/batchprogram.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/program/callbackprogram.py` & `DomiKnowS-0.532/domiknows/program/callbackprogram.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/program/loss.py` & `DomiKnowS-0.532/domiknows/program/loss.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/program/lossprogram.py` & `DomiKnowS-0.532/domiknows/program/lossprogram.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 import logging
 import torch
 import numpy as np
 from tqdm import tqdm
 
-from domiknows.program.model.pytorch import SolverModel
-
-
 from .program import LearningBasedProgram, get_len
 from ..utils import consume, entuple, detuple
-from .model.lossModel import PrimalDualModel, SampleLossModel
+from .model.lossModel import PrimalDualModel, SampleLosslModel
 from .model.base import Mode
 
-from .model.gbi import GBIModel
-
 # Primal-dual need multiple backward through constraint loss.
 # It requires retain_graph=True.
 # Memory leak problem with `backward(create_graph=True)`
 # https://github.com/pytorch/pytorch/issues/4661#issuecomment-596526199
 # workaround with following functions based on `grad()`
 def backward(loss, parameters):
     parameters = list(parameters)
@@ -156,14 +151,17 @@
                     if key == 'ILP':
                         ilpMetric = metric
 
                     if key == 'softmax':
                         softmaxMetric = metric
 #         super().call_epoch(name=name, dataset=dataset, epoch_fn=epoch_fn, **kwargs)
         
+
+    
+
     def train_epoch(
         self, dataset,
         c_lr=1,
         c_warmup_iters=10,  # warmup
         c_freq_increase=1,  # d
         c_freq_increase_freq=1,
         c_lr_decay=0,  # strategy
@@ -274,15 +272,15 @@
     def __init__(self, graph, Model, beta=1, **kwargs):
         super().__init__(graph, Model, CModel=PrimalDualModel, beta=beta, **kwargs)
         
 class SampleLossProgram(LossProgram):
     logger = logging.getLogger(__name__)
 
     def __init__(self, graph, Model, beta=1, **kwargs):
-        super().__init__(graph, Model, CModel=SampleLossModel, beta=beta, **kwargs)
+        super().__init__(graph, Model, CModel=SampleLosslModel, beta=beta, **kwargs)
 
 
     def train(
         self,
         training_set,
         valid_set=None,
         test_set=None,
@@ -356,20 +354,8 @@
                 self.copt is not None and
                 loss
             ):
                 self.copt.step()
             
             yield (loss, metric, *output[:1])
 
-        c_session['iter'] = iter    
-        
-class GBIProgram(LossProgram):
-    logger = logging.getLogger(__name__)
-
-    def __init__(self, graph, Model, poi, beta=1, **kwargs):
-        mySolverModel= SolverModel(graph,
-                           poi=poi,
-                           inferTypes=['local/argmax', 'local/softmax'],
-                           metric={})
-        super().__init__(graph, Model, CModel=GBIModel, beta=beta, solver_model = mySolverModel, poi=poi, **kwargs)
-        from domiknows.utils import setDnSkeletonMode
-        setDnSkeletonMode(True)
+        c_session['iter'] = iter
```

### Comparing `DomiKnowS-0.531.dev0/domiknows/program/metric.py` & `DomiKnowS-0.532/domiknows/program/metric.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/program/model/ilpu.py` & `DomiKnowS-0.532/domiknows/program/model/ilpu.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/program/model/iml.py` & `DomiKnowS-0.532/domiknows/program/model/iml.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import warnings
 
 import torch
 
 from .pytorch import SolverModel
 from ...graph.concept import EnumConcept
 
-# Inference-Masked Loss
+
 class IMLModel(SolverModel):
     def poi_loss(self, data_item, prop, sensors):
         output_sensor, target_sensor = sensors
         logit = output_sensor(data_item)
         labels = target_sensor(data_item)
         if len(logit) == 0:
             return None
```

### Comparing `DomiKnowS-0.531.dev0/domiknows/program/model/lossModel.py` & `DomiKnowS-0.532/domiknows/program/model/lossModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     
 class PrimalDualModel(LossModel):
     logger = logging.getLogger(__name__)
 
     def __init__(self, graph, tnorm=DataNode.tnormsDefault, device='auto'):
         super().__init__(graph, tnorm=tnorm, device=device)
         
-class SampleLossModel(torch.nn.Module):
+class SampleLosslModel(torch.nn.Module):
     logger = logging.getLogger(__name__)
 
     # def __init__(self, graph, sample = False, sampleSize = 0, sampleGlobalLoss = False):
     #     super().__init__(graph, sample=sample, sampleSize=sampleSize, sampleGlobalLoss=sampleGlobalLoss)
 
     def __init__(self, graph, 
                  tnorm=DataNode.tnormsDefault, 
@@ -161,15 +161,15 @@
             
         if not build and not isinstance(builder, DataNodeBuilder):
             raise ValueError('PrimalDualModel must be invoked with `build` on or with provided DataNode Builder.')
         
         if (builder.needsBatchRootDN()):
             builder.addBatchRootDN()
         
-#       self.loss.reset()
+#         self.loss.reset()
 
         datanode = builder.getDataNode(device=self.device)
         
         # Call the loss calculation returns a dictionary, keys are matching the constraints
         constr_loss = datanode.calculateLcLoss(tnorm=self.tnorm, sample=self.sample, sampleSize = self.sampleSize, sampleGlobalLoss = self.sampleGlobalLoss)
         import math
         lmbd_loss = []
@@ -202,15 +202,15 @@
                         loss_ = -1 * torch.log(loss_value)
                         key_loss += loss_
 
                     else:
                         loss_ = 0
                     
                 else:
-                    if constr_loss["globalSuccessCounter"] > 0:
+                    if constr_loss["globalSuccessCountet"] > 0:
                         lcSuccesses = constr_loss["globalSuccesses"]
                     if lossTensor.sum().item() != 0:
                         tidx = (lcSuccesses == 1).nonzero().squeeze(-1)
                         true_val = lossTensor[tidx]
                         
                         if true_val.sum().item() != 0: 
                             if not replace_mul:
@@ -230,14 +230,16 @@
                             else:
                                 loss_value = true_val.logsumexp(dim=0) - lossTensor.logsumexp(dim=0)
                                 key_loss += -1 * loss_value
 
                         else:
                             loss_ = 0
                         
+                        
+
                         # if loss['lossTensor'].nansum().item() <= 1:
                         #     loss_value = loss['lossTensor']
                         #     # loss_value = loss_value[loss_value.nonzero()].squeeze(-1)
                         # else:
                         #     _idx = []
                         #     for i in torch.unique(loss['lossTensor']):
                         #         _idx.append((loss['lossTensor'] == i.item()).nonzero(as_tuple=True)[0][0].item())
@@ -263,15 +265,15 @@
         all_losses = [key_losses[key] for key in key_losses]
         if all_losses:
             all_losses = torch.stack(all_losses)
 
             satisfied_num = len( set(constr_loss.keys()) - set(key_losses.keys()) )
             unsatisfied_num = len(set(constr_loss.keys())) - satisfied_num
             #self.logger.info(f'-- number of satisfied constraints are {satisfied_num}')
-            #self.logger.info(f'-- number of unsatisfied constraints are {unsatisfied_num}')
+            #self.logger.info(f'-- number of unstatisfied constraints are {unsatisfied_num}')
             for key in key_losses:
                 if self.sampleSize != -1:
                     if replace_mul:
                         loss_val = (key_losses[key] / all_losses.sum()) * key_losses[key]
                     else:
                         loss_val = key_losses[key]
                 else:
```

### Comparing `DomiKnowS-0.531.dev0/domiknows/program/model/pytorch.py` & `DomiKnowS-0.532/domiknows/program/model/pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,17 +87,17 @@
             data_hash = data_hash or self.data_hash(data_item)
             sensor.fill_hash(data_hash)
         for sensor in self.graph.get_sensors(ReaderSensor):
             sensor.fill_data(data_item)
         if build:
             data_item.update({"graph": self.graph, 'READER': 0})
             builder = DataNodeBuilder(data_item)
-            *out, = self.populate(builder)
             if (builder.needsBatchRootDN()):
                 builder.addBatchRootDN()
+            *out, = self.populate(builder)
             datanode = builder.getDataNode(context="build", device=self.device)
             return (*out, datanode, builder)
         else:
             *out, = self.populate(data_item)
             return (*out,)
 
     def populate(self):
@@ -225,15 +225,15 @@
             
         if inference_with == None:
             self.inference_with = []
         else:
             self.inference_with = inference_with
 
     def inference(self, builder):
-        for i, prop in enumerate(self.poi):
+        for prop in self.poi:
             for sensor in prop.find(TorchSensor):
                 sensor(builder)
 #             for output_sensor, target_sensor in self.find_sensors(prop):
 #             # make sure the sensors are evaluated
 #                 output = output_sensor(builder)
 #                 target = target_sensor(builder)
 #         print("Done with the computation")
@@ -247,15 +247,14 @@
         for infertype in self.inferTypes:
             {
                 'ILP': lambda :datanode.inferILPResults(*self.inference_with, fun=None, epsilon=None),
                 'local/argmax': lambda :datanode.inferLocal(),
                 'local/softmax': lambda :datanode.inferLocal(),
                 'argmax': lambda :datanode.infer(),
                 'softmax': lambda :datanode.infer(),
-                'GBI': lambda :datanode.inferGBIResults(*self.inference_with, model=self, builder=builder),
             }[infertype]()
 #         print("Done with the inference")
         return builder
 
     def populate(self, builder, run=True):
         data_item = self.inference(builder)
         return super().populate(builder, run=False)
```

### Comparing `DomiKnowS-0.531.dev0/domiknows/program/model/torch.py` & `DomiKnowS-0.532/domiknows/program/model/torch.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/program/model_program.py` & `DomiKnowS-0.532/domiknows/program/model_program.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,20 @@
-from domiknows.utils import setDnSkeletonMode
 from .program import LearningBasedProgram
 from .model.pytorch import PoiModel, PoiModelToWorkWithLearnerWithLoss, SolverModel, SolverModelDictLoss
 from .model.iml import IMLModel
 
+
 class POIProgram(LearningBasedProgram):
     def __init__(self, graph, **kwargs):
         super().__init__(graph, PoiModel, **kwargs)
 
 
 class SolverPOIProgram(LearningBasedProgram):
     def __init__(self, graph, **kwargs):
         super().__init__(graph, SolverModel, **kwargs)
-        # Check if the 'inferTypes' is in the kwargs and has GBI then setDnSkeletonMode(True)
-        if 'inferTypes' in kwargs:         
-            if 'GBI' in kwargs['inferTypes']:
-                setDnSkeletonMode(True)
         
         
 class SolverPOIDictLossProgram(LearningBasedProgram):
     def __init__(self, graph, **kwargs):
         super().__init__(graph, SolverModelDictLoss, **kwargs)
```

### Comparing `DomiKnowS-0.531.dev0/domiknows/program/program.py` & `DomiKnowS-0.532/domiknows/program/program.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/program/tracker.py` & `DomiKnowS-0.532/domiknows/program/tracker.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/sensor/allennlp/base.py` & `DomiKnowS-0.532/domiknows/sensor/allennlp/base.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/sensor/allennlp/learner.py` & `DomiKnowS-0.532/domiknows/sensor/allennlp/learner.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/sensor/allennlp/module.py` & `DomiKnowS-0.532/domiknows/sensor/allennlp/module.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/sensor/allennlp/sensor.py` & `DomiKnowS-0.532/domiknows/sensor/allennlp/sensor.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/sensor/pytorch/learnerModels.py` & `DomiKnowS-0.532/domiknows/sensor/pytorch/learnerModels.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/sensor/pytorch/learners.py` & `DomiKnowS-0.532/domiknows/sensor/pytorch/learners.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/sensor/pytorch/query_sensor.py` & `DomiKnowS-0.532/domiknows/sensor/pytorch/query_sensor.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/sensor/pytorch/relation_sensors.py` & `DomiKnowS-0.532/domiknows/sensor/pytorch/relation_sensors.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/sensor/pytorch/sensors.py` & `DomiKnowS-0.532/domiknows/sensor/pytorch/sensors.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/sensor/pytorch/tokenizers/spacy.py` & `DomiKnowS-0.532/domiknows/sensor/pytorch/tokenizers/spacy.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/sensor/pytorch/tokenizers/transformers.py` & `DomiKnowS-0.532/domiknows/sensor/pytorch/tokenizers/transformers.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/sensor/pytorch/utils.py` & `DomiKnowS-0.532/domiknows/sensor/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/sensor/sensor.py` & `DomiKnowS-0.532/domiknows/sensor/sensor.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/sensor/torch/learner.py` & `DomiKnowS-0.532/domiknows/sensor/torch/learner.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/sensor/torch/sensor.py` & `DomiKnowS-0.532/domiknows/sensor/torch/sensor.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/solver/allennlpInferenceSolver.py` & `DomiKnowS-0.532/domiknows/solver/allennlpInferenceSolver.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/solver/allennlplogInferenceSolver.py` & `DomiKnowS-0.532/domiknows/solver/allennlplogInferenceSolver.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/solver/constructor/constructor.py` & `DomiKnowS-0.532/domiknows/solver/constructor/constructor.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/solver/dummyILPOntSolver.py` & `DomiKnowS-0.532/domiknows/solver/dummyILPOntSolver.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/solver/gekkoILPBooleanMethods.py` & `DomiKnowS-0.532/domiknows/solver/gekkoILPBooleanMethods.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/solver/gekkoILPOntSolver.py` & `DomiKnowS-0.532/domiknows/solver/gekkoILPOntSolver.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/solver/gurobiILPBooleanMethods.py` & `DomiKnowS-0.532/domiknows/solver/gurobiILPBooleanMethods.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/solver/gurobiILPOntSolver.py` & `DomiKnowS-0.532/domiknows/solver/gurobiILPOntSolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,18 @@
 from domiknows.graph.concept import Concept, EnumConcept
 from domiknows.solver.ilpOntSolver import ilpOntSolver
 from domiknows.solver.gurobiILPBooleanMethods import gurobiILPBooleanProcessor
 from domiknows.solver.lcLossBooleanMethods import lcLossBooleanMethods
 from domiknows.solver.lcLossSampleBooleanMethods import lcLossSampleBooleanMethods
 from domiknows.solver.ilpBooleanMethodsCalculator import booleanMethodsCalculator
 
-from domiknows.graph import LcElement, LogicalConstrain, V, fixedL, ifL, forAllL
-from domiknows.graph import CandidateSelection
+from domiknows.graph import LogicalConstrain, V, fixedL, ifL
+from _functools import reduce
 from domiknows.utils import getReuseModel
 
-from domiknows.graph.candidates import getCandidates
-
 class gurobiILPOntSolver(ilpOntSolver):
     ilpSolver = 'Gurobi'
 
     def __init__(self, graph, ontologiesTuple, _ilpConfig, reuse_model=False) -> None:
         super().__init__(graph, ontologiesTuple, _ilpConfig)
         self.myIlpBooleanProcessor = gurobiILPBooleanProcessor()
         self.myLcLossBooleanMethods = lcLossBooleanMethods()
@@ -300,15 +298,15 @@
             
             if c[0] not in multiclassDict:
                 multiclassDict[c[0]] = []
             
             multiclassDict[c[0]].append(c)
             
         for mc in multiclassDict:
-            # Add constraint which restrict number of muliclass labels assigned to one for the given instance
+            # Add constrain which restrict number of muliclass labels assigned to one for the given instance
             rootConcept = rootDn.findRootConceptOrRelation(mc)
             dns = rootDn.findDatanodes(select = rootConcept)
             xkey = '<' + mc.name + '>/ILP/x'  
             
             for dn in dns:
                 var = []
                 for mlabel in multiclassDict[mc]: 
@@ -928,84 +926,46 @@
             if vDnLabel == -100:
                 return None
             elif vDnLabel == i:
                 return 1
             else:
                 return 0
         
-        
-    def __addLossTovDns(self, loss, vDns):
-        if loss and vDns:
-            vDnsOriginal = vDns
-            vDnsList = [v[0] for v in  vDns]
-            
-            updatedVDns = []
-            try:
-                if len(vDnsList) > 1:
-                    tStack = torch.stack(vDnsList, dim=1)
-                else:
-                    tStack = vDnsList[0]
-                tsqueezed = torch.squeeze(tStack, dim=0)
-
-            except IndexError as ie:
-                tsqueezed = torch.stack(vDnsList, dim=0)
-                pass
-        
-            if not len(tsqueezed.shape):
-                tsqueezed = torch.unsqueeze(tsqueezed, 0)
-                
-            tList = [tsqueezed]
-            updatedVDns.append(tList)
-            
-            return updatedVDns
-        else:
-            return vDns
-    
-    def __constructLogicalConstrains(self, lc, booleanProcessor, m, dn, p, key = None, lcVariablesDns = None, headLC = False, loss = False, sample = False, vNo = None, verify=False):
+    def __constructLogicalConstrains(self, lc, booleanProcesor, m, dn, p, key = None, lcVariablesDns = None, headLC = False, loss = False, sample = False, vNo = None, verify=False):
         if key == None:
             key = ""
-            
         if lcVariablesDns == None:
             lcVariablesDns = OrderedDict()
             
         lcVariables = OrderedDict()
-        
         if sample:
             sampleInfo = OrderedDict()
             lcVariablesSet = OrderedDict()
-            
         if vNo == None:
             vNo = [1, 1]
         
         firstV = None
         integrate = False
         
         for eIndex, e in enumerate(lc.e): 
             if  isinstance(e, V):
                 continue # Already processed in the previous Concept 
             
-            if isinstance(e, (Concept,  LcElement, tuple)): 
+            if isinstance(e, (Concept,  LogicalConstrain, tuple)): 
                 # Look one step ahead in the parsed logical constraint and get variables names (if present) after the current concept
                 if eIndex + 1 < len(lc.e) and isinstance(lc.e[eIndex+1], V):
                     variable = lc.e[eIndex+1]
                 else:
                     if isinstance(e, LogicalConstrain):
                         variable = V(name="_lc" + str(vNo[1]))
                         vNo[1] += 1
-                    elif isinstance(e, tuple) and isinstance(e[0], CandidateSelection):
-                        e[0].CandidateSelectionVariable = e[1]
-                        e = e[0]
-                        
-                        variable = V(name="_cs" + str(vNo[1]))
-                        vNo[1] += 1
                     else:
                         if firstV == None:
                             variable = V(name="_x" + str(vNo[0]) )
-                            if not isinstance(lc, CandidateSelection):
-                                firstV = variable.name
+                            firstV = variable.name
                             vNo[0] += 1
                         else:
                             variable = V(name="_x" + str(vNo[0]), v = (firstV,))
                             vNo[0] += 1
                     
                 if variable.name:
                     variableName = variable.name
@@ -1020,24 +980,135 @@
                     lcVariablesDns[newvVariableName] = lcVariablesDns[variableName]
                     if None in lcVariablesDns:
                         pass
   
                     lcVariables[newvVariableName] = lcVariables[variableName]
 
                 elif isinstance(e, (Concept, tuple)): # -- Concept 
-                    # -- Get dataNodes candidates 
-                    dnsList = getCandidates(dn, e, variable, lcVariablesDns, lc, self.myLogger)
-                    lcVariablesDns[variableName] = dnsList
-                                
-                    if isinstance(lc, CandidateSelection):
-                        continue
+                    conceptName = e[0].name
+                        
+                    # -- Collect dataNode for the logical constraint (path)
                     
+                    dnsList = [] # Stores lists of dataNodes for each corresponding dataNode 
+                    
+                    if variable.v == None: # No path - just concept
+                        if variable.name == None:
+                            self.myLogger.error('The element %s of logical constraint %s has no name for variable'%(conceptName, lc.lcName))
+                            return None
+                                                 
+                        rootConcept = dn.findRootConceptOrRelation(conceptName)
+                        _dns = dn.findDatanodes(select = rootConcept)
+                        dnsList = [[dn] for dn in _dns]
+                    else: # Path specified
+                        from domiknows.graph.logicalConstrain import eqL
+                        if not isinstance(variable.v, eqL):
+                            if len(variable.v) == 0:
+                                self.myLogger.error('The element %s of logical constraint %s has empty part v of the variable'%(conceptName, lc.lcName))
+                                return None
+                          
+                        # -- Prepare paths
+                        path = variable.v
+                        paths = []
+                        
+                        if isinstance(path, eqL):
+                            paths.append(path)
+                        elif isinstance(path[0], str) and len(path) == 1:
+                            paths.append(path)
+                        elif isinstance(path[0], str) and not isinstance(path[1], tuple):
+                            paths.append(path)
+                        else: # If many paths
+                            for i, vE in enumerate(variable.v):
+                                if i == 0 and isinstance(vE, str):
+                                    continue
+                                
+                                paths.append(vE)
+                                
+                        pathsCount = len(paths)
+                        
+                        # -- Process  paths
+                        dnsListForPaths = []
+                        for i, v in enumerate(paths):
+                            dnsListForPaths.append([])
+                            
+                            # Get name of the referred variable 
+                            if isinstance(path, eqL):
+                                referredVariableName = None
+                            else:
+                                referredVariableName = v[0] 
+                        
+                            if referredVariableName not in lcVariablesDns: # Not yet defined - it has to be the current lc element dataNodes list
+                                rootConcept = dn.findRootConceptOrRelation(conceptName)
+                                _dns = dn.findDatanodes(select = rootConcept)
+                                referredDns = [[dn] for dn in _dns]
+                                integrate = True
+                            else: # already defined in the logical constraint from the v part 
+                                referredDns = lcVariablesDns[referredVariableName] # Get DataNodes for referred variables already defined in the logical constraint
+                                
+                            # Get variables from dataNodes selected  based on referredVariableName
+                            for listOfDataNodes in referredDns:
+                                eDns = [] 
+                                
+                                for currentReferredDataNode in listOfDataNodes:
+                                    if currentReferredDataNode is None:
+                                        continue
+                                    
+                                    # -- Get DataNodes for the edge defined by the path part of the v
+                                    if isinstance(path, eqL):
+                                        _eDns = currentReferredDataNode.getEdgeDataNode(v) 
+                                    else:
+                                        _eDns = currentReferredDataNode.getEdgeDataNode(v[1:]) 
+                                    
+                                    if _eDns and _eDns[0]:
+                                        eDns.extend(_eDns)
+                                    elif not isinstance(path, eqL):
+                                        vNames = [v if isinstance(v, str) else v.name for v in v[1:]]
+                                        if lc.__str__() != "fixedL":
+                                            self.myLogger.info('%s has no path %s requested by %s for concept %s'%(currentReferredDataNode, vNames, lc.lcName, conceptName))
+                                if not eDns:
+                                    eDns = [None] # None - to keep track of candidates
+                                    
+                                dnsListForPaths[i].append(eDns)
+                           
+                        # -- Select a single dns list or Combine the collected lists of dataNodes based on paths 
+                        dnsList = []
+                        newIntersection = True
+                        if newIntersection:
+                            if pathsCount == 1: # Single path
+                                dnsList = dnsListForPaths[0]
+                            else:
+                                # --- Assume Intersection - TODO: in future use lo if defined to determine if different operation                                
+                                for i in range(len(dnsListForPaths[0])):
+                                    try:
+                                        se = [set(dnsListForPaths[item][i]) for item in range(pathsCount)]
+                                    except IndexError as ei:
+                                        continue
+                                    dnsListR = reduce(set.intersection, se)
+                                    dnsList.append(list(dnsListR))
+                        else:
+                            dnsList = dnsListForPaths[0]
+                           
+                            # -- Combine the collected lists of dataNodes based on paths 
+                            for l in dnsListForPaths[1:]:
+                                # --- Assume Intersection - TODO: in future use lo if defined to determine if different  operation
+                                _d = []
+                                for i in range(len(l)):
+                                    di = []
+                                    for x in dnsList[i]:
+                                        if x in l[i]:
+                                            di.append(x)
+                                            
+                                    if not di:
+                                        di = [None]
+                                        
+                                    _d.append(di)
+                                    
+                                dnsList = _d
+                                
                     # -- Get ILP variables from collected DataNodes for the given element of logical constraint
                     
-                    conceptName = e[0].name
                     vDns = [] # Stores ILP variables
                     if sample:
                         sampleInfoForVariable = []
                     xPkey = '<' + conceptName + ">" + key
                     
                     for dns in dnsList:
                         _vDns = []
@@ -1097,15 +1168,17 @@
                             pass
                         
                         vDns.append(_vDns)
                         
                         if sample:
                             sampleInfoForVariable.append(_sampleInfoForVariable)
                         
-                    # -- Store ILP variables
+                    # -- Store dataNodes and ILP variables
+                    
+                    lcVariablesDns[variableName] = dnsList
                     
                     if None in lcVariablesDns:
                         pass
                     
                     if vDns and loss and not sample:
                         vDnsList = [v[0] for v in vDns]
                         try:
@@ -1122,49 +1195,47 @@
                             lcVariables[variableName] = vDns
                     else:
                         lcVariables[variableName] = vDns
                     
                     if sample:
                         sampleInfo[variableName] = sampleInfoForVariable
                 
-                if isinstance(e, LcElement):
-
-                    if isinstance(e, CandidateSelection): # -- nested LogicalConstrain - process recursively 
-                        lcVariablesDnsNew = self.__constructLogicalConstrains(e, booleanProcessor, m, dn, p, key = key, 
-                                                                     lcVariablesDns = lcVariablesDns, headLC = False, loss = loss, sample = sample, vNo=vNo, verify=verify)
-                         
-                        lcVariablesDns = lcVariablesDnsNew
-                        vDns = None
-                        if lcVariablesDns:
-                            length_of_list = len(next(iter(lcVariablesDns.values())))
-
-                            if sample:
-                                vDns = [[torch.ones(p, device=self.current_device, requires_grad=False, dtype=torch.bool)] for _ in range(length_of_list)]
-                            elif loss:
-                                vDns = [[torch.zeros(length_of_list, device=self.current_device, requires_grad=True, dtype=torch.float64)]]
-                                vDns = self.__addLossTovDns(loss, vDns)
-                            else:
-                                vDns = [[1] for _ in range(length_of_list)]
-                                   
-                    if isinstance(e, LogicalConstrain): # -- nested LogicalConstrain - process recursively 
-                        self.myLogger.info('Processing Nested %s(%s) - %s'%(e.lcName, e, e.strEs()))
+                elif isinstance(e, LogicalConstrain): # -- nested LogicalConstrain - process recursively 
+                    self.myLogger.info('Processing Nested %s(%s) - %s'%(e.lcName, e, e.strEs()))
+                    if sample:
+                        vDns, sampleInfoLC, lcVariablesLC = self.__constructLogicalConstrains(e, booleanProcesor, m, dn, p, key = key, 
+                                                                               lcVariablesDns = lcVariablesDns, headLC = False, loss = loss, sample = sample, vNo=vNo, verify=verify)
+                        sampleInfo = {**sampleInfo, **sampleInfoLC} # sampleInfo|sampleInfoLC in python 9
+                        
+                        lcVariablesSet = {**lcVariablesSet, **lcVariablesLC}
+                    else:
+                        vDns = self.__constructLogicalConstrains(e, booleanProcesor, m, dn, p, key = key, 
+                                                                 lcVariablesDns = lcVariablesDns, headLC = False, loss = loss, sample = sample, vNo=vNo, verify=verify)
+                        
+                        if loss and vDns:
+                            vDnsOriginal = vDns
+                            vDnsList = [v[0] for v in  vDns]
+                            vDns = []
+                            try:
+                                if len(vDnsList) > 1:
+                                    tStack = torch.stack(vDnsList, dim=1)
+                                else:
+                                    tStack = vDnsList[0]
+                                tsqueezed = torch.squeeze(tStack, dim=0)
 
-                        if sample:
-                            vDns, sampleInfoLC, lcVariablesLC = self.__constructLogicalConstrains(e, booleanProcessor, m, dn, p, key = key, 
-                                                                                   lcVariablesDns = lcVariablesDns, headLC = False, loss = loss, sample = sample, vNo=vNo, verify=verify)
-                            sampleInfo = {**sampleInfo, **sampleInfoLC} # sampleInfo|sampleInfoLC in python 9
-                            
-                            lcVariablesSet = {**lcVariablesSet, **lcVariablesLC}
-                        else:
-                            vDns = self.__constructLogicalConstrains(e, booleanProcessor, m, dn, p, key = key, 
-                                                                     lcVariablesDns = lcVariablesDns, headLC = False, loss = loss, sample = sample, vNo=vNo, verify=verify)
-                            
-                            vDns = self.__addLossTovDns(loss, vDns)
+                            except IndexError as ie:
+                                tsqueezed = torch.stack(vDnsList, dim=0)
+                                pass
                         
-                                                    
+                            if not len(tsqueezed.shape):
+                                tsqueezed = torch.unsqueeze(tsqueezed, 0)
+                                
+                            tList = [tsqueezed]
+                            vDns.append(tList)
+                                                
                     if vDns == None:
                         self.myLogger.warning('Not found data for %s(%s) nested Logical Constraint required to build %s(%s) - skipping it'%(e.lcName,e,lc.lcName,lc))
                         return None
                         
                     lcVariables[variableName] = vDns   
             # Int - limit 
             elif isinstance(e, int): 
@@ -1176,22 +1247,19 @@
                 if eIndex == 2:
                     pass # if this lc using it
                 else:
                     pass # error!
             else:
                 self.myLogger.error('Logical Constraint %s has incorrect element %s'%(lc,e))
                 return None
-            
-        if isinstance(lc, CandidateSelection):
-            return lc(lcVariablesDns, keys=lc.CandidateSelectionVariable)
-        elif sample:
+        if sample:
             lcVariablesSet[lc] = lcVariables
-            return lc(m, booleanProcessor, lcVariables, headConstrain = headLC, integrate = integrate), sampleInfo, lcVariablesSet
+            return lc(m, booleanProcesor, lcVariables, headConstrain = headLC, integrate = integrate), sampleInfo, lcVariablesSet
         elif verify and headLC:
-            return lc(m, booleanProcessor, lcVariables, headConstrain = headLC, integrate = integrate), lcVariables
+            return lc(m, booleanProcesor, lcVariables, headConstrain = headLC, integrate = integrate), lcVariables
         else:
             if loss:
                 slpitT = False
                 for v in lcVariables:
                     if lcVariables[v] and len(lcVariables[v]) > 1:
                         slpitT = True
                         break
@@ -1203,15 +1271,15 @@
                          
                         lcVSplitted = torch.split(lcVariables[v][0][0], 1)
                         lcVariables[v] = []
                         
                         for s in lcVSplitted:
                             lcVariables[v].append([s]) 
                     
-            return lc(m, booleanProcessor, lcVariables, headConstrain = headLC, integrate = integrate)
+            return lc(m, booleanProcesor, lcVariables, headConstrain = headLC, integrate = integrate)
     
     # ---------------
                 
     # -- Main method of the solver - creating ILP constraints plus objective, invoking the ILP solver and returning the result of the ILP solver classification  
     def calculateILPSelection(self, dn, *conceptsRelations, fun=None, epsilon = 0.00001, minimizeObjective = False, ignorePinLCs = False):
         if self.ilpSolver == None:
             self.myLogger.warning('ILP solver not provided - returning')
@@ -2094,15 +2162,15 @@
                 
                 if verifyListLen:
                     current_verifyResult['satisfied'] = (verifyListSatisfied / verifyListLen) * 100
                 else:
                     current_verifyResult['satisfied'] = float("nan")
                     
                 # If  this if logical constraints
-                if type(lc) is ifL or type(lc) is forAllL: # if LC
+                if type(lc) is ifL: # if LC
                     firstKey = next(iter(lcVariables)) # antecedent variable name in the given if LC
                     firstLcV = lcVariables[firstKey]   # values of antecedent 
                     
                     ifVerifyList = []
                     
                     ifVerifyListLen = 0
                     ifVerifyListSatisfied = 0
```

### Comparing `DomiKnowS-0.531.dev0/domiknows/solver/ilpBooleanMethods.py` & `DomiKnowS-0.532/domiknows/solver/ilpBooleanMethods.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,143 +8,143 @@
 class ilpBooleanProcessor(object):
     __metaclass__ = abc.ABCMeta
     
     def __init__(self, _ildConfig = ilpConfig) -> None:
         super().__init__()
 
     # NOT Negation
-    # Create new variable varNOT, create constraint 1 - var == varNOT, return varNOT
+    # Create new variable varNOT, create constrain 1 - var == varNOT, return varNOT
     # 1 - var == varNOT
-    # if onlyConstrains then only construct constraint 1 - var >= 0
+    # if onlyConstrains then only construct constrain 1 - var >= 0
     @abc.abstractmethod
     def notVar(self, m, _var, onlyConstrains = False): pass
     
     # AND Conjunction with 2 variable
     # Create new variable varAND, create constrains:
     # varAND <= var1
     # varAND <= var2 
     # var1 + var2 <= varAND + 2 - 1
     # return varAND
-    # if onlyConstrains then only construct constraint var1 + var2 >= 2
+    # if onlyConstrains then only construct constrain var1 + var2 >= 2
     @abc.abstractmethod
     def and2Var(self, m, _var1, _var2,  onlyConstrains = False): pass
         
     # AND Conjunction
     # Create new variable varAND, create constrains:
     # varAND <= var1
     # varAND <= var2
     # ....
     # varAND <= varN
     # var1 + var2 + .. + varN <= varAND + N - 1
     # return varAND
-    # if onlyConstrains then only construct constraint var1 + var2 + .. + varN >= N
+    # if onlyConstrains then only construct constrain var1 + var2 + .. + varN >= N
     @abc.abstractmethod
     def andVar(self, m, *_var, onlyConstrains = False): pass
        
     # OR Disjunction with 2 variables
     # Create new variable varOR, create constrains:
     # var1 <= varOR
     # var2 <= varOR 
     # var1 + var2 >= varOR 
     # return varOR
-    # if onlyConstrains then only construct constraint var1 + var2 >= 1
+    # if onlyConstrains then only construct constrain var1 + var2 >= 1
     #
     # if limit > 1
     # var1 + var2 - (limit - 1) >= varOR 
-    # if onlyConstrains then only construct constraint var1 + var2 >= limit
+    # if onlyConstrains then only construct constrain var1 + var2 >= limit
     @abc.abstractmethod
     def or2Var(self, m, _var1, _var2,  onlyConstrains = False): pass
         
     # OR Disjunction
     # Create new variable varOR, create constrains:
     # var1 <= varOR
     # var2 <= varOR 
     # ...
     # varN <= varOR
     # var1 + var2 + ... + varN >= varOR
     # return varOR
-    # if onlyConstrains then only construct constraint var1 + var2 + ... + varN >= 1
+    # if onlyConstrains then only construct constrain var1 + var2 + ... + varN >= 1
     # if limit > 1
     # var1 + var2 + ... + varN - (limit - 1) >= varOR 
-    # if onlyConstrains then only construct constraint var1 + var2 + ... + varN >= limit
+    # if onlyConstrains then only construct constrain var1 + var2 + ... + varN >= limit
     @abc.abstractmethod
     def orVar(self, m, *_var, onlyConstrains = False): pass
 
     # NAND (Alternative denial) with 2 variables
     # Create new variable varNAND, create constrains:
     # not(varNAND) <= var1
     # not(varNAND) <= var2 
     # var1 + var2 <= not(varNAND) + 2 - 1
     # return varNAND
-    # if onlyConstrains then only construct constraint var1 + var2 <= 1
+    # if onlyConstrains then only construct constrain var1 + var2 <= 1
     @abc.abstractmethod
     def nand2Var(self, m, _var1, _var2): pass
 
     # NAND (Alternative denial)
     # Create new variable varNAND, create constrains:
     # not(varNAND) <= var1
     # not(varNAND) <= var2 
     # ...
     # not(varNAND <= varN 
     # var1 + var2 + ... + varN <= not(varNAND) + N - 1
     # return varNAND
-    # if onlyConstrains then only construct constraint var1 + var2 + ... + varN <= N -1
+    # if onlyConstrains then only construct constrain var1 + var2 + ... + varN <= N -1
     @abc.abstractmethod
     def nandVar(self, m, *_var, onlyConstrains = False): pass
   
     # NOR (Joint Denial) 2 variables
     # Create new variable varNOR, create constrains:
     # var1 <= not(varNOR)
     # var2 <= not(varNOR) 
     # var1 + var2 >= not(varNOR)
     # return varNOR
-    # if onlyConstrains then only construct constraint var1 + var2 <= 0
+    # if onlyConstrains then only construct constrain var1 + var2 <= 0
     @abc.abstractmethod
     def nor2Var(self, m, _var1, _var2): pass
 
     # NOR (Joint Denial)
     # Create new variable varNOR, create constrains:
     # var1 <= not(varNOR)
     # var2 <= not(varNOR) 
     # ...
     # varN <= not(varNOR)
     # var1 + var2 + ... + varN >= not(varNOR)
     # return varNOR
-    # if onlyConstrains then only construct constraint var1 + var2 + ... + varN <= 0
+    # if onlyConstrains then only construct constrain var1 + var2 + ... + varN <= 0
     @abc.abstractmethod
     def norVar(self, m, *_var, onlyConstrains = False): pass
 
     # XOR Exclusive Disjunction 
     # Create new variable varXOR, create constrains:
     # var1 + var2 + varXOR <= 2
     # -var1 - var2 + varXOR <= 0
     # var1 - var2 + varXOR >= 0
     # -var1 + var2 + varXOR >= 0
     # return varXOR
-    # if onlyConstrains then only construct constraint var1 + var2 <= 1 and var1 + var2 >= 1 
+    # if onlyConstrains then only construct constrain var1 + var2 <= 1 and var1 + var2 >= 1 
     @abc.abstractmethod
     def xorVar(self, m, _var1, _var2,  onlyConstrains = False): pass
 
     # IF Implication
     # Create new variable varIF, create constrains:
     # 1 - var1 <= varIF
     # var2 <= varIF
     # 1 - var1 + var2 >= varIF
     # return varIF
-    # if onlyConstrains then only construct constraint var1 <= var2
+    # if onlyConstrains then only construct constrain var1 <= var2
     @abc.abstractmethod
     def ifVar(self, m, _var1, _var2,  onlyConstrains = False): pass
 
     # XNOR Equivalence (EQ)
     # Create new variable varEQ, create constrains:
     # var1 + var2 - varEQ <= 1
     # var1 + var2 + varEQ >= 1
     # -var1 + var2 + varEQ <= 1
     # var1 - var2 + varEQ <= 1
     # return varEQ
-    # if onlyConstrains then only construct constraint var1 >= var2 and var1 <= var2
+    # if onlyConstrains then only construct constrain var1 >= var2 and var1 <= var2
     @abc.abstractmethod
     def epqVar(self, m, _var1, _var2,  onlyConstrains = False): pass
     
-    # Create constraint var == label, return 1
+    # Create constrain var == label, return 1
     @abc.abstractmethod
     def fixedVar(self, m, _var, onlyConstrains = False): pass
```

### Comparing `DomiKnowS-0.531.dev0/domiknows/solver/ilpBooleanMethodsCalculator.py` & `DomiKnowS-0.532/domiknows/solver/ilpBooleanMethodsCalculator.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/solver/ilpOntSolver.py` & `DomiKnowS-0.532/domiknows/solver/ilpOntSolver.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/solver/ilpOntSolverFactory.py` & `DomiKnowS-0.532/domiknows/solver/ilpOntSolverFactory.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/solver/lcLossBooleanMethods.py` & `DomiKnowS-0.532/domiknows/solver/lcLossBooleanMethods.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/solver/lcLossSampleBooleanMethods.py` & `DomiKnowS-0.532/domiknows/solver/lcLossSampleBooleanMethods.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/solver/mini_solver_debug.py` & `DomiKnowS-0.532/domiknows/solver/mini_solver_debug.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/solver/session/gurobi_session.py` & `DomiKnowS-0.532/domiknows/solver/session/gurobi_session.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/solver/session/solver_session.py` & `DomiKnowS-0.532/domiknows/solver/session/solver_session.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/domiknows/utils.py` & `DomiKnowS-0.532/domiknows/utils.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.531.dev0/setup.py` & `DomiKnowS-0.532/setup.py`

 * *Files identical despite different names*

