# Comparing `tmp/pyPhasesML-0.4.4.tar.gz` & `tmp/pyPhasesML-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPhasesML-0.4.4.tar", last modified: Wed Apr 12 11:53:07 2023, max compression
+gzip compressed data, was "pyPhasesML-0.4.5.tar", last modified: Sat Apr 15 12:12:43 2023, max compression
```

## Comparing `pyPhasesML-0.4.4.tar` & `pyPhasesML-0.4.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:53:07.865352 pyPhasesML-0.4.4/
--rw-rw-rw-   0 root         (0) root         (0)     1065 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3691 2023-04-12 11:53:07.865352 pyPhasesML-0.4.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3184 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:53:07.859351 pyPhasesML-0.4.4/pyPhasesML/
--rw-rw-rw-   0 root         (0) root         (0)     2348 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/DataAugmentation.py
--rw-rw-rw-   0 root         (0) root         (0)      895 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/DataSet.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/FeatureExtraction.py
--rw-rw-rw-   0 root         (0) root         (0)     3887 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/Model.py
--rw-rw-rw-   0 root         (0) root         (0)     4368 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/ModelManager.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     4558 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/SignalPreprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:53:07.862352 pyPhasesML-0.4.4/pyPhasesML/adapter/
--rw-rw-rw-   0 root         (0) root         (0)    10212 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/adapter/ModelKerasAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)     7116 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/adapter/ModelTf1Adapter.py
--rw-rw-rw-   0 root         (0) root         (0)    17734 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/adapter/ModelTorchAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/adapter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1106 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:53:07.863352 pyPhasesML-0.4.4/pyPhasesML/exporter/
--rw-rw-rw-   0 root         (0) root         (0)     5358 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/exporter/MemmapRecordExporter.py
--rw-rw-rw-   0 root         (0) root         (0)     3201 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/exporter/ModelExporter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/exporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:53:07.864352 pyPhasesML-0.4.4/pyPhasesML/scorer/
--rw-rw-rw-   0 root         (0) root         (0)    22289 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/scorer/Scorer.py
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/scorer/ScorerTF.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/scorer/ScorerTorch.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyPhasesML/scorer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:53:07.861352 pyPhasesML-0.4.4/pyPhasesML.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3691 2023-04-12 11:53:07.000000 pyPhasesML-0.4.4/pyPhasesML.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      838 2023-04-12 11:53:07.000000 pyPhasesML-0.4.4/pyPhasesML.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:53:07.000000 pyPhasesML-0.4.4/pyPhasesML.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-04-12 11:53:07.000000 pyPhasesML-0.4.4/pyPhasesML.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-12 11:53:07.000000 pyPhasesML-0.4.4/pyPhasesML.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      484 2023-04-12 11:52:39.000000 pyPhasesML-0.4.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 11:53:07.865352 pyPhasesML-0.4.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      858 2023-04-12 11:52:41.000000 pyPhasesML-0.4.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:12:43.739615 pyPhasesML-0.4.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2023-04-15 12:12:16.000000 pyPhasesML-0.4.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-15 12:12:16.000000 pyPhasesML-0.4.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-04-15 12:12:43.739615 pyPhasesML-0.4.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3184 2023-04-15 12:12:16.000000 pyPhasesML-0.4.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:12:43.733614 pyPhasesML-0.4.5/pyPhasesML/
+-rw-rw-rw-   0 root         (0) root         (0)     2348 2023-04-15 12:12:16.000000 pyPhasesML-0.4.5/pyPhasesML/DataAugmentation.py
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-04-15 12:12:16.000000 pyPhasesML-0.4.5/pyPhasesML/DataSet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-04-15 12:12:16.000000 pyPhasesML-0.4.5/pyPhasesML/FeatureExtraction.py
+-rw-rw-rw-   0 root         (0) root         (0)     3887 2023-04-15 12:12:16.000000 pyPhasesML-0.4.5/pyPhasesML/Model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4368 2023-04-15 12:12:16.000000 pyPhasesML-0.4.5/pyPhasesML/ModelManager.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2023-04-15 12:12:16.000000 pyPhasesML-0.4.5/pyPhasesML/Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4558 2023-04-15 12:12:16.000000 pyPhasesML-0.4.5/pyPhasesML/SignalPreprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-04-15 12:12:16.000000 pyPhasesML-0.4.5/pyPhasesML/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:12:43.736614 pyPhasesML-0.4.5/pyPhasesML/adapter/
+-rw-rw-rw-   0 root         (0) root         (0)    10212 2023-04-15 12:12:16.000000 pyPhasesML-0.4.5/pyPhasesML/adapter/ModelKerasAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     7116 2023-04-15 12:12:16.000000 pyPhasesML-0.4.5/pyPhasesML/adapter/ModelTf1Adapter.py
+-rw-rw-rw-   0 root         (0) root         (0)    17734 2023-04-15 12:12:16.000000 pyPhasesML-0.4.5/pyPhasesML/adapter/ModelTorchAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 12:12:16.000000 pyPhasesML-0.4.5/pyPhasesML/adapter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-04-15 12:12:16.000000 pyPhasesML-0.4.5/pyPhasesML/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:12:43.737614 pyPhasesML-0.4.5/pyPhasesML/exporter/
+-rw-rw-rw-   0 root         (0) root         (0)     5358 2023-04-15 12:12:16.000000 pyPhasesML-0.4.5/pyPhasesML/exporter/MemmapRecordExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2023-04-15 12:12:16.000000 pyPhasesML-0.4.5/pyPhasesML/exporter/ModelExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 12:12:16.000000 pyPhasesML-0.4.5/pyPhasesML/exporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:12:43.739615 pyPhasesML-0.4.5/pyPhasesML/scorer/
+-rw-rw-rw-   0 root         (0) root         (0)    19512 2023-04-15 12:12:16.000000 pyPhasesML-0.4.5/pyPhasesML/scorer/Scorer.py
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-04-15 12:12:16.000000 pyPhasesML-0.4.5/pyPhasesML/scorer/ScorerTF.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-04-15 12:12:16.000000 pyPhasesML-0.4.5/pyPhasesML/scorer/ScorerTorch.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-15 12:12:16.000000 pyPhasesML-0.4.5/pyPhasesML/scorer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 12:12:43.735614 pyPhasesML-0.4.5/pyPhasesML.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-04-15 12:12:43.000000 pyPhasesML-0.4.5/pyPhasesML.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      838 2023-04-15 12:12:43.000000 pyPhasesML-0.4.5/pyPhasesML.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 12:12:43.000000 pyPhasesML-0.4.5/pyPhasesML.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-15 12:12:43.000000 pyPhasesML-0.4.5/pyPhasesML.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-15 12:12:43.000000 pyPhasesML-0.4.5/pyPhasesML.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-04-15 12:12:16.000000 pyPhasesML-0.4.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-15 12:12:43.740615 pyPhasesML-0.4.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      858 2023-04-15 12:12:17.000000 pyPhasesML-0.4.5/setup.py
```

### Comparing `pyPhasesML-0.4.4/LICENSE` & `pyPhasesML-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.4/PKG-INFO` & `pyPhasesML-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.4.4
+Version: 0.4.5
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.4.4/README.md` & `pyPhasesML-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.4/pyPhasesML/DataAugmentation.py` & `pyPhasesML-0.4.5/pyPhasesML/DataAugmentation.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.4/pyPhasesML/DataSet.py` & `pyPhasesML-0.4.5/pyPhasesML/DataSet.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.4/pyPhasesML/FeatureExtraction.py` & `pyPhasesML-0.4.5/pyPhasesML/FeatureExtraction.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.4/pyPhasesML/Model.py` & `pyPhasesML-0.4.5/pyPhasesML/Model.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.4/pyPhasesML/ModelManager.py` & `pyPhasesML-0.4.5/pyPhasesML/ModelManager.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.4/pyPhasesML/Plugin.py` & `pyPhasesML-0.4.5/pyPhasesML/Plugin.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.4/pyPhasesML/SignalPreprocessing.py` & `pyPhasesML-0.4.5/pyPhasesML/SignalPreprocessing.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.4/pyPhasesML/adapter/ModelKerasAdapter.py` & `pyPhasesML-0.4.5/pyPhasesML/adapter/ModelKerasAdapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.4/pyPhasesML/adapter/ModelTf1Adapter.py` & `pyPhasesML-0.4.5/pyPhasesML/adapter/ModelTf1Adapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.4/pyPhasesML/adapter/ModelTorchAdapter.py` & `pyPhasesML-0.4.5/pyPhasesML/adapter/ModelTorchAdapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.4/pyPhasesML/config.yaml` & `pyPhasesML-0.4.5/pyPhasesML/config.yaml`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.4/pyPhasesML/exporter/MemmapRecordExporter.py` & `pyPhasesML-0.4.5/pyPhasesML/exporter/MemmapRecordExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.4/pyPhasesML/exporter/ModelExporter.py` & `pyPhasesML-0.4.5/pyPhasesML/exporter/ModelExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.4/pyPhasesML/scorer/Scorer.py` & `pyPhasesML-0.4.5/pyPhasesML/scorer/Scorer.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     title = "Segmentbasiert"
     cmScaleByClass = 4
 
     metricNameMap = {}
     addedMetrics = {}
 
     def getMetricDefinition(self, name):
-
         metricDefinition = {
             # init value, useAsBest, biggerIsBetter
             "AUC": [0.5, False, True],
             "AP": [0.0, True, True],
             "accuracy": [0.0, False, True],
             "acc": [0.0, False, True],
             "kappa": [-1, True, True],
@@ -34,15 +33,14 @@
             metric = Scorer.addedMetrics[name]
             return [metric["initValue"], metric["useAsBest"], metric["biggerIsBetter"]]
 
         return metricDefinition[name]
 
     @staticmethod
     def registerMetric(metricName, metricFunction, combineFunction, biggerIsBetter=True, useAsBest=True, initValue=None):
-
         Scorer.addedMetrics[metricName] = {
             "score": metricFunction,
             "combine": combineFunction,
             "biggerIsBetter": biggerIsBetter,
             "useAsBest": useAsBest,
             "initValue": initValue if initValue is not None else 0.0 if biggerIsBetter else np.inf,
         }
@@ -110,15 +108,14 @@
             self.recordResult[recordName] = self.recordEntry(truthOrg, predictionOrg, self.results, recordName)
 
             self.recordIndex += 1
 
         return metrics
 
     def recordEntry(self, truth, prediction, metrics, recordName=None):
-
         # prediction = self.flattenPrediction(prediction)
 
         # if "confusion" in metrics and self.addEvents:
         #     events = self.getValidationEvents(truth, prediction, recordName=recordName)
         # else:
         #     events = None
 
@@ -127,27 +124,25 @@
             "prediction": prediction,
             # "events": events,
         }
         entry.update(metrics)
         return entry
 
     def getRecords(self):
-
         return self.recordResult.values()
 
     def getRecordsAsDataframe(self):
         import pandas as pd
 
         return pd.DataFrame(
             self.getRecords(),
             index=list(self.recordResult.keys()),
         )
 
     def combineMetric(self, metricName):
-
         metricName = self.getMetricName(metricName)
 
         result = None
 
         if metricName in self.addedMetrics:
             truth = np.concatenate([self.recordResult[id]["truth"] for id in self.recordResult], axis=0)
             prediction = np.concatenate([self.recordResult[id]["prediction"] for id in self.recordResult], axis=0)
@@ -159,15 +154,14 @@
             self.combineMetric("confusion")
             self.scoreMetric("f1", None, None)
         elif metricName == "confusion":  # combine all confusion
             result = np.array(
                 [self.recordResult[id]["confusion"] for id in self.recordResult if len(self.recordResult[id]["confusion"]) > 0]
             ).sum(axis=0)
         elif metricName in ["auprc", "auroc"]:
-
             if self.numClasses != 2:
                 raise Exception("Metric auprc, auroc only support binary classification at the moment")
 
             self.results["all_values"] = np.array([self.recordResult[id]["all_values"] for id in self.recordResult]).sum(axis=0)
             self.results["pos_values"] = np.array([self.recordResult[id]["pos_values"] for id in self.recordResult]).sum(axis=0)
             self.results["ign_values"] = np.array([self.recordResult[id]["ign_values"] for id in self.recordResult]).sum(axis=0)
 
@@ -274,22 +268,23 @@
         prediction = np.full(prediction.shape[0], 0)
         prediction[likelyhood > self.threshold] = 1
         return prediction
 
     def flattenPrediction(self, prediction, binaryLikelyHood=False, threshold=None):
         if binaryLikelyHood and self.numClasses != 2:
             raise Exception("Selected metric only support binary classification at the moment")
+        useThreshold = threshold is not None and self.numClasses <= 2
 
-        if threshold is not None:
+        if useThreshold:
             return self.getClassPrediction(prediction)
 
         if self.isHotEncoded(prediction):
             prediction = prediction.argmax(-1)
         else:
-            threshhold = 0.5 if self.threshold is None else self.threshold
+            threshhold = self.threshold if useThreshold is None else 0.5
             prediction[prediction >= threshhold] = 1
             prediction[prediction < threshhold] = 0
         return prediction
 
     def getMetricScorer(self, metricName):
         def score(truth, prediction):
             prediction = self.prepareInput(prediction)
@@ -299,15 +294,14 @@
             self.results = {}
             return self.scoreMetric(metricName, truth, prediction)
 
         score.__name__ = metricName
         return score
 
     def scoreMetric(self, metricName, truth, prediction):
-
         metricName = self.getMetricName(metricName)
 
         if metricName in self.results:
             return self.results[metricName]
 
         result = None
 
@@ -315,26 +309,37 @@
             self.results[metricName] = self.addedMetrics[metricName]["score"](truth, prediction)
         elif metricName in ["kappa", "accuracy"]:
             confusion = self.scoreMetric("confusion", truth, prediction)
             k, acc = self.calculateKappaAccFromConfusion(confusion)
             self.results["accuracy"] = acc
             self.results["kappa"] = k
         elif metricName in ["f1"]:
-            (tn, fn), (fp, tp) = self.scoreMetric("confusion", truth, prediction)
-            f1 = tp / (tp + 0.5 * (fp + fn))
-            self.results["f1"] = f1
+            if self.numClasses > 2:
+                f1s = []
+                confusion = self.scoreMetric("confusion", truth, prediction)
+                for i in range(self.numClasses):
+                    # first = truth, second = predicted
+                    tp = confusion[i][i]
+                    fp = sum(confusion[i][:]) - tp
+                    fn = sum(confusion[:][i]) - tp
+                    f1 = tp / (tp + 0.5 * (fp + fn))
+                    self.results["f1-%i" % i] = f1
+                    f1s.append(f1)
+                self.results["f1"] = np.mean(f1s)
+            else:
+                self.results["f1"] = f1
         elif metricName == "confusion":
             prediction = self.flattenPrediction(prediction, threshold=self.threshold)
             result = confusion_matrix(
                 truth, prediction, labels=range(self.numClasses)
             )  # , labels=range(self.numClasses) # HPC comp
         elif metricName in ["auprc", "auroc"]:
             classLikelyhood = self.getClassLikelyhood(prediction)
 
-            scale = 10 ** 3
+            scale = 10**3
             b = scale + 1
             r = (-0.5 / scale, 1.0 + 0.5 / scale)
 
             self.results["all_values"] = np.histogram(classLikelyhood, bins=b, range=r)[0]
 
             pred_pos = classLikelyhood[truth > 0]
             self.results["pos_values"] = np.histogram(pred_pos, bins=b, range=r)[0]
@@ -414,101 +419,21 @@
             self.results[metricName] = result
 
         return self.results[metricName]
 
     def getValuesFromClasses(self):
         if self.possibleValues is None:
             values = []
-            for id in range(self.numClasses ** 2):
+            for id in range(self.numClasses**2):
                 trueValue, preditedValue = (id // self.numClasses, id % self.numClasses)
                 values.append("%s as %s" % (self.classNames[trueValue], self.classNames[preditedValue]))
             self.possibleValues = values
 
         return self.possibleValues
 
-    # def getValidationEvents(self, truth, prediction, recordName=None):
-
-    #     validationSignal = self.numClasses * truth + prediction
-    #     validationSignal[truth == -1] = -1
-
-    #     values = self.getValuesFromClasses()
-
-    #     em = EventManager(None)
-    #     return em.getEventsFromSignal(validationSignal, values, owner=recordName)
-
-    # def confusionMatrix(self, resultEntry, labels=None, title="confusion matrix"):
-    #     confusion = resultEntry["confusion"]
-    #     labels = self.classNames
-
-    #     label_list = [labels[i] for i in range(len(labels))]
-    #     df_cm = pd.DataFrame(confusion, index=label_list, columns=label_list)
-
-    #     blue = cm.get_cmap("Blues", 256)
-    #     darkencolor = blue(np.linspace(0.3, 1, 256))
-    #     newcmp = ListedColormap(darkencolor, name="DarkenBlue")
-    #     figSize = self.numClasses * Scorer.cmScaleByClass
-    #     return pp_matrix(df_cm, title=title, figsize=[figSize, figSize], cmap=newcmp, cbar=False)
-
-    # def confusionMatrixTrailor(self, resultEntry, labels=None, title="sub confusion matrix", rowsSplit=slice(0,2), colSplit=slice(None), colNames = None, rowNames=None):
-    #     #remove NoneRow
-    #     colNames = self.classNames if colNames is None else colNames
-    #     rowNames = self.classNames if rowNames is None else rowNames
-    #     confusion = resultEntry["confusion"][colSplit, rowsSplit]
-    #     labelsCol = np.array(colNames)[colSplit]
-    #     labelsRow = np.array(rowNames)[rowsSplit]
-    #     df_cm = pd.DataFrame(confusion, index=labelsCol, columns=labelsRow)
-
-    #     blue = cm.get_cmap("Blues", 256)
-    #     darkencolor = blue(np.linspace(0.3, 1, 256))
-    #     newcmp = ListedColormap(darkencolor, name="DarkenBlue")
-    #     figSizeL = (len(labelsCol) + 1 ) * Scorer.cmScaleByClass
-    #     figSizeH = (len(labelsRow) +  1) * Scorer.cmScaleByClass
-    #     return pp_matrix(df_cm, title=title, figsize=[figSizeL, figSizeH], cmap=newcmp, cbar=False)
-
-    # def prCurve(self, resultEntry, title="ROC"):
-    #     _, _, precision, _, recall = self._auc(resultEntry["pos_values"], resultEntry["neg_values"])
-    #     fig = plt.figure(figsize=(6, 6))
-    #     lw = 2
-    #     plt.plot(
-    #         recall,
-    #         precision,
-    #         color="darkorange",
-    #         lw=lw,
-    #         label=title,
-    #     )
-    #     plt.xlim([0.0, 1.0])
-    #     plt.ylim([0.0, 1.05])
-    #     plt.xlabel("Recall")
-    #     plt.ylabel("Precision")
-    #     plt.title("Precision/Recall Curve")
-    #     plt.legend(loc="lower right")
-
-    #     return fig
-
-    # def rocCurve(self, resultEntry, title="ROC"):
-    #     _, _, tpr, fpr, _ = self._auc(resultEntry["pos_values"], resultEntry["neg_values"])
-
-    #     fig = plt.figure(figsize=(6, 6))
-    #     lw = 2
-    #     plt.plot(
-    #         fpr,
-    #         tpr,
-    #         color="darkorange",
-    #         lw=lw,
-    #         label=title,
-    #     )
-    #     plt.plot([0, 1], [0, 1], color="navy", lw=lw, linestyle="--")
-    #     plt.xlim([0.0, 1.0])
-    #     plt.ylim([0.0, 1.05])
-    #     plt.xlabel("False Positive Rate")
-    #     plt.ylabel("True Positive Rate")
-    #     plt.title("Receiver operating characteristic")
-    #     plt.legend(loc="lower right")
-    #     return fig
-
     def _auc(self, pos_values, neg_values):
         # Calculate areas under the ROC and PR curves by iterating
         # over the possible threshold values.
 
         # At the minimum threshold value, all samples are classified as
         # positive, and thus TPR = 1 and TNR = 0.
         tp = np.sum(pos_values)
@@ -531,15 +456,15 @@
         tpr_arr = []
         fpr_arr = []
         precisions = []
 
         # As the threshold increases, TP decreases (and FN increases)
         # by pos_values[i], while TN increases (and FP decreases) by
         # neg_values[i].
-        for (n_pos, n_neg) in zip(pos_values, neg_values):
+        for n_pos, n_neg in zip(pos_values, neg_values):
             tp -= n_pos
             fn += n_pos
             fp -= n_neg
             tn += n_neg
             tpr_prev = tpr
             tnr_prev = tnr
             ppv_prev = ppv
```

### Comparing `pyPhasesML-0.4.4/pyPhasesML.egg-info/PKG-INFO` & `pyPhasesML-0.4.5/pyPhasesML.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.4.4
+Version: 0.4.5
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.4.4/pyPhasesML.egg-info/SOURCES.txt` & `pyPhasesML-0.4.5/pyPhasesML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.4/setup.py` & `pyPhasesML-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyPhasesML",
-    version="v0.4.4"[1:],
+    version="v0.4.5"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="A Framework for creating a boilerplate template for ai projects that are ready for MLOps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/",
     packages=setuptools.find_packages(),
```

