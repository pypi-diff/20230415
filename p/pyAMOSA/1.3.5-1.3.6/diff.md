# Comparing `tmp/pyAMOSA-1.3.5.tar.gz` & `tmp/pyAMOSA-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyAMOSA-1.3.5.tar", last modified: Sat Feb  4 11:11:00 2023, max compression
+gzip compressed data, was "pyAMOSA-1.3.6.tar", last modified: Sat Apr 15 09:33:48 2023, max compression
```

## Comparing `pyAMOSA-1.3.5.tar` & `pyAMOSA-1.3.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-02-04 11:11:00.487113 pyAMOSA-1.3.5/
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)    35149 2023-02-04 09:39:41.000000 pyAMOSA-1.3.5/LICENSE
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)      919 2023-02-04 11:11:00.487113 pyAMOSA-1.3.5/PKG-INFO
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)    10688 2023-02-04 09:39:41.000000 pyAMOSA-1.3.5/README.md
-drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-02-04 11:11:00.487113 pyAMOSA-1.3.5/pyAMOSA.egg-info/
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)      919 2023-02-04 11:11:00.000000 pyAMOSA-1.3.5/pyAMOSA.egg-info/PKG-INFO
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)      446 2023-02-04 11:11:00.000000 pyAMOSA-1.3.5/pyAMOSA.egg-info/SOURCES.txt
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)        1 2023-02-04 11:11:00.000000 pyAMOSA-1.3.5/pyAMOSA.egg-info/dependency_links.txt
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)       28 2023-02-04 11:11:00.000000 pyAMOSA-1.3.5/pyAMOSA.egg-info/requires.txt
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)        8 2023-02-04 11:11:00.000000 pyAMOSA-1.3.5/pyAMOSA.egg-info/top_level.txt
-drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-02-04 11:11:00.487113 pyAMOSA-1.3.5/pyamosa/
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1480 2023-02-04 11:08:11.000000 pyAMOSA-1.3.5/pyamosa/CombinedStopCriterion.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     2784 2023-02-04 09:39:41.000000 pyAMOSA-1.3.5/pyamosa/Config.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)      787 2023-02-04 09:39:41.000000 pyAMOSA-1.3.5/pyamosa/DataType.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     2412 2023-02-04 09:39:41.000000 pyAMOSA-1.3.5/pyamosa/MultiFileCacheHandle.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)    33418 2023-02-04 09:39:41.000000 pyAMOSA-1.3.5/pyamosa/Optimizer.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     3169 2023-02-04 09:39:41.000000 pyAMOSA-1.3.5/pyamosa/Problem.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)      868 2023-02-04 09:39:41.000000 pyAMOSA-1.3.5/pyamosa/StopCriterion.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1344 2023-02-04 11:10:36.000000 pyAMOSA-1.3.5/pyamosa/StopMaxTime.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1218 2023-02-04 11:10:32.000000 pyAMOSA-1.3.5/pyamosa/StopMinTemperature.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1264 2023-02-04 11:10:27.000000 pyAMOSA-1.3.5/pyamosa/StopPhyWindow.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1280 2023-02-04 11:10:51.000000 pyAMOSA-1.3.5/pyamosa/__init__.py
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)       38 2023-02-04 11:11:00.487113 pyAMOSA-1.3.5/setup.cfg
--rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1638 2023-02-04 11:10:48.000000 pyAMOSA-1.3.5/setup.py
+drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-04-15 09:33:48.430606 pyAMOSA-1.3.6/
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)    35149 2023-02-04 09:39:41.000000 pyAMOSA-1.3.6/LICENSE
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)      919 2023-04-15 09:33:48.430606 pyAMOSA-1.3.6/PKG-INFO
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)    10688 2023-02-04 09:39:41.000000 pyAMOSA-1.3.6/README.md
+drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-04-15 09:33:48.429606 pyAMOSA-1.3.6/pyAMOSA.egg-info/
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)      919 2023-04-15 09:33:48.000000 pyAMOSA-1.3.6/pyAMOSA.egg-info/PKG-INFO
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)      446 2023-04-15 09:33:48.000000 pyAMOSA-1.3.6/pyAMOSA.egg-info/SOURCES.txt
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)        1 2023-04-15 09:33:48.000000 pyAMOSA-1.3.6/pyAMOSA.egg-info/dependency_links.txt
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)       28 2023-04-15 09:33:48.000000 pyAMOSA-1.3.6/pyAMOSA.egg-info/requires.txt
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)        8 2023-04-15 09:33:48.000000 pyAMOSA-1.3.6/pyAMOSA.egg-info/top_level.txt
+drwxr-xr-x   0 ssaa      (1000) ssaa      (1000)        0 2023-04-15 09:33:48.430606 pyAMOSA-1.3.6/pyamosa/
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1480 2023-02-04 11:08:11.000000 pyAMOSA-1.3.6/pyamosa/CombinedStopCriterion.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     2784 2023-02-04 09:39:41.000000 pyAMOSA-1.3.6/pyamosa/Config.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)      787 2023-02-04 09:39:41.000000 pyAMOSA-1.3.6/pyamosa/DataType.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     2412 2023-02-04 09:39:41.000000 pyAMOSA-1.3.6/pyamosa/MultiFileCacheHandle.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)    34674 2023-04-15 09:26:18.000000 pyAMOSA-1.3.6/pyamosa/Optimizer.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     3169 2023-02-04 09:39:41.000000 pyAMOSA-1.3.6/pyamosa/Problem.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)      868 2023-02-04 09:39:41.000000 pyAMOSA-1.3.6/pyamosa/StopCriterion.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1344 2023-02-04 11:10:36.000000 pyAMOSA-1.3.6/pyamosa/StopMaxTime.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1218 2023-02-04 11:10:32.000000 pyAMOSA-1.3.6/pyamosa/StopMinTemperature.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1264 2023-02-04 11:10:27.000000 pyAMOSA-1.3.6/pyamosa/StopPhyWindow.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1280 2023-04-15 09:29:35.000000 pyAMOSA-1.3.6/pyamosa/__init__.py
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)       38 2023-04-15 09:33:48.430606 pyAMOSA-1.3.6/setup.cfg
+-rw-r--r--   0 ssaa      (1000) ssaa      (1000)     1638 2023-04-15 09:29:33.000000 pyAMOSA-1.3.6/setup.py
```

### Comparing `pyAMOSA-1.3.5/LICENSE` & `pyAMOSA-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyAMOSA-1.3.5/PKG-INFO` & `pyAMOSA-1.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyAMOSA
-Version: 1.3.5
+Version: 1.3.6
 Summary: Python implementation of the Archived Multi-Objective Simulated Annealing optimization heuristic
 Home-page: https://github.com/SalvatoreBarone/pyAMOSA
 Author: Salvatore Barone
 Author-email: salvatore.barone@unina.it
 Project-URL: Bug Reports, https://github.com/SalvatoreBarone/pyAMOSA/issues
 Project-URL: Source, https://github.com/SalvatoreBarone/pyAMOSA
 Keywords: Verilator Wrapper Verilog
```

### Comparing `pyAMOSA-1.3.5/README.md` & `pyAMOSA-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pyAMOSA-1.3.5/pyAMOSA.egg-info/PKG-INFO` & `pyAMOSA-1.3.6/pyAMOSA.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyAMOSA
-Version: 1.3.5
+Version: 1.3.6
 Summary: Python implementation of the Archived Multi-Objective Simulated Annealing optimization heuristic
 Home-page: https://github.com/SalvatoreBarone/pyAMOSA
 Author: Salvatore Barone
 Author-email: salvatore.barone@unina.it
 Project-URL: Bug Reports, https://github.com/SalvatoreBarone/pyAMOSA/issues
 Project-URL: Source, https://github.com/SalvatoreBarone/pyAMOSA
 Keywords: Verilator Wrapper Verilog
```

### Comparing `pyAMOSA-1.3.5/pyamosa/CombinedStopCriterion.py` & `pyAMOSA-1.3.6/pyamosa/CombinedStopCriterion.py`

 * *Files identical despite different names*

### Comparing `pyAMOSA-1.3.5/pyamosa/Config.py` & `pyAMOSA-1.3.6/pyamosa/Config.py`

 * *Files identical despite different names*

### Comparing `pyAMOSA-1.3.5/pyamosa/DataType.py` & `pyAMOSA-1.3.6/pyamosa/DataType.py`

 * *Files identical despite different names*

### Comparing `pyAMOSA-1.3.5/pyamosa/MultiFileCacheHandle.py` & `pyAMOSA-1.3.6/pyamosa/MultiFileCacheHandle.py`

 * *Files identical despite different names*

### Comparing `pyAMOSA-1.3.5/pyamosa/Optimizer.py` & `pyAMOSA-1.3.6/pyamosa/Optimizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,35 +99,53 @@
 
     def pareto_set(self):
         return np.array([s["x"] for s in self.archive])
 
     def constraint_violation(self):
         return np.array([s["g"] for s in self.archive])
 
-    def plot_pareto(self, problem : Problem, pdf_file : str, fig_title : str = "Pareto front", axis_labels : list = None):
+    def plot_pareto(self, problem : Problem, pdf_file : str, fig_title : str = "Pareto front", axis_labels : list = None, color = "k", marker = "."):
+        def draw_proj(axis, data_x, data_y, data_z, color, ranges = [0.1, 0.1, 0.1]):
+            xlim = axis.get_xlim()
+            ylim = axis.get_ylim()
+            zlim = axis.get_zlim()
+            for x, y, z in zip (data_x, data_y, data_z):
+                line_x = np.arange(x, xlim[1], ranges[0])
+                line_y = np.arange(ylim[0], y, ranges[1])
+                line_z = np.arange(zlim[0], z, ranges[2])
+                axis.plot(line_x, np.full(np.shape(line_x), y), np.full(np.shape(line_x), zlim[0]), f":{color}")
+                axis.plot(np.full(np.shape(line_y), x), line_y, np.full(np.shape(line_y), zlim[0]), f":{color}")
+                axis.plot(np.full(np.shape(line_z), x), np.full(np.shape(line_z), y), line_z,       f":{color}")
+            axis.set_xlim(xlim)
+            axis.set_ylim(ylim)
+            axis.set_zlim(zlim)
+
         if axis_labels is None:
             axis_labels = [f"f{str(i)}" for i in range(problem.num_of_objectives)]
+            
         F = self.pareto_front()
         if problem.num_of_objectives == 2:
             plt.figure(figsize = (10, 10), dpi = 300)
-            plt.plot(F[:, 0], F[:, 1], 'k.')
+            plt.plot(F[:, 0], F[:, 1], f'{color}{marker}')
             plt.xlabel(axis_labels[0])
             plt.ylabel(axis_labels[1])
             plt.title(fig_title)
             plt.savefig(pdf_file, bbox_inches = 'tight', pad_inches = 0)
         elif problem.num_of_objectives == 3:
             fig = plt.figure()
             ax = fig.add_subplot(projection = '3d')
+            ax.scatter(F[:, 0], F[:, 1], F[:, 2], marker = marker, color = color, depthshade = False)
+            draw_proj(ax, F[:, 0], F[:, 1], F[:, 2], color = color)
             ax.set_xlabel(axis_labels[0])
             ax.set_ylabel(axis_labels[1])
             ax.set_zlabel(axis_labels[2])
+            ax.set_proj_type('ortho')
             plt.title(fig_title)
-            ax.scatter(F[:, 0], F[:, 1], F[:, 2], marker = '.', color = 'k')
             plt.tight_layout()
-            plt.savefig(pdf_file, bbox_inches = 'tight', pad_inches = 0)
+            plt.savefig(pdf_file, bbox_inches = 'tight', pad_inches = 0.5)
 
     def archive_to_json(self, json_file : str):
         try:
             with open(json_file, 'w') as outfile:
                 outfile.write(json.dumps(self.archive))
         except TypeError as e:
             print(self.archive)
@@ -434,22 +452,29 @@
         dimention = random.randrange(0, problem.num_of_variables)
         while current_dimention == dimention:
             dimention = random.randrange(0, problem.num_of_variables)
         return dimention, increase
 
     @staticmethod
     def impose_domain_constraints(problem, x):
-        # impose constraints the hard way
-        lb = np.array(problem.lower_bound)
-        ub = np.array(problem.upper_bound)
-        dv = np.array(x["x"])
-        dv = np.where(dv < ub, dv, ub - problem.min_step)
-        dv = np.where(dv >= lb, dv, lb)
-        return dv.tolist()
-        
+        try: 
+            lb = np.array(problem.lower_bound)
+            ub = np.array(problem.upper_bound)
+            dv = np.array(x["x"])
+            dv = np.where(dv < ub, dv, ub - problem.min_step)
+            dv = np.where(dv >= lb, dv, lb)
+            return dv.tolist()
+        except ValueError as e:
+            print(e)
+            print(f"dv: {dv}, len(dv) {len(dv)}")
+            print(f"lb: {lb}, len(lb) {len(lb)}")
+            print(f"ub: {ub}, len(ub) {len(ub)}")
+            exit()
+
+
     @staticmethod
     def hill_climbing_adaptive_step(problem, x, dimention, increase):
         safety_exit = problem.max_attempt # a safety-exit prevents infinite loop, using a counter variable
         while safety_exit >= 0 and problem.is_cached(x):
             safety_exit -= 1
             tp = problem.types[dimention]
             min_step = 1 if tp == Type.INTEGER else (2 * np.finfo(float).eps)
```

### Comparing `pyAMOSA-1.3.5/pyamosa/Problem.py` & `pyAMOSA-1.3.6/pyamosa/Problem.py`

 * *Files identical despite different names*

### Comparing `pyAMOSA-1.3.5/pyamosa/StopCriterion.py` & `pyAMOSA-1.3.6/pyamosa/StopCriterion.py`

 * *Files identical despite different names*

### Comparing `pyAMOSA-1.3.5/pyamosa/StopMaxTime.py` & `pyAMOSA-1.3.6/pyamosa/StopMaxTime.py`

 * *Files identical despite different names*

### Comparing `pyAMOSA-1.3.5/pyamosa/StopMinTemperature.py` & `pyAMOSA-1.3.6/pyamosa/StopMinTemperature.py`

 * *Files identical despite different names*

### Comparing `pyAMOSA-1.3.5/pyamosa/StopPhyWindow.py` & `pyAMOSA-1.3.6/pyamosa/StopPhyWindow.py`

 * *Files identical despite different names*

### Comparing `pyAMOSA-1.3.5/pyamosa/__init__.py` & `pyAMOSA-1.3.6/pyamosa/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,10 +21,10 @@
 from .StopCriterion import StopCriterion
 from .StopMaxTime import StopMaxTime
 from .StopMinTemperature import StopMinTemperature
 from .StopPhyWindow import StopPhyWindow
 from .CombinedStopCriterion import CombinedStopCriterion
 
 name = "pyamosa"
-__version__ = "1.3.5"
+__version__ = "1.3.6"
 __author__ = "Salvatore Barone"
 __credits__ = "Department of Electrical Engineering and Information Technologies, University of Naples Federico II, Via Claudio 21, Naples, Italy"
```

### Comparing `pyAMOSA-1.3.5/setup.py` & `pyAMOSA-1.3.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="pyAMOSA",
-    version="1.3.5",
+    version="1.3.6",
     description="Python implementation of the Archived Multi-Objective Simulated Annealing optimization heuristic",
     long_description="Python implementation of the Archived Multi-Objective Simulated Annealing optimization heuristic. Take a look at https://github.com/SalvatoreBarone/pyAMOSA.",
     url="https://github.com/SalvatoreBarone/pyAMOSA",
     author="Salvatore Barone",
     author_email="salvatore.barone@unina.it",
     # https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
```

