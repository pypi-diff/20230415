# Comparing `tmp/bk_clustering-0.1.1.tar.gz` & `tmp/bk_clustering-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bk_clustering-0.1.1.tar", max compression
+gzip compressed data, was "bk_clustering-0.2.tar", max compression
```

## Comparing `bk_clustering-0.1.1.tar` & `bk_clustering-0.2.tar`

### file list

```diff
@@ -1,32 +1,17 @@
--rw-r--r--   0        0        0        0 2023-03-09 12:14:06.008282 bk_clustering-0.1.1/README.md
--rw-r--r--   0        0        0   893611 2023-04-09 07:14:20.570222 bk_clustering-0.1.1/bk_clustering/.ipynb_checkpoints/boxplots-checkpoint.ipynb
--rw-r--r--   0        0        0       40 2023-04-08 23:59:03.211844 bk_clustering-0.1.1/bk_clustering/__init__.py
--rw-r--r--   0        0        0    33769 2023-03-25 12:39:17.568753 bk_clustering-0.1.1/bk_clustering/_hierarchy.pyx
--rw-r--r--   0        0        0     9101 2023-04-10 21:45:41.383464 bk_clustering-0.1.1/bk_clustering/main.py
--rw-r--r--   0        0        0     3635 2023-04-10 13:47:29.443057 bk_clustering-0.1.1/bk_clustering/run_batch.py
--rw-r--r--   0        0        0        2 2023-04-10 20:34:39.948587 bk_clustering-0.1.1/bk_clustering/utilities/__init__.py
--rw-r--r--   0        0        0      182 2023-03-28 10:42:47.293233 bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2394 2023-04-08 23:27:42.220376 bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/calculation_utilities.cpython-310.pyc
--rw-r--r--   0        0        0     4423 2023-04-08 23:26:04.015216 bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/cluster_calculations.cpython-310.pyc
--rw-r--r--   0        0        0     6256 2023-03-30 17:31:31.888383 bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/density_peak.cpython-310.pyc
--rw-r--r--   0        0        0     1386 2023-04-03 15:10:41.814013 bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/ext_linkage_matrix.cpython-310.pyc
--rw-r--r--   0        0        0     1708 2023-03-11 12:30:08.257315 bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/hutils.cpython-310.pyc
--rw-r--r--   0        0        0     1002 2023-03-11 11:40:12.461914 bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/hutils_calc.cpython-310.pyc
--rw-r--r--   0        0        0    14683 2023-03-11 11:40:12.469914 bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/hutils_cluster.cpython-310.pyc
--rw-r--r--   0        0        0     4614 2023-04-08 23:27:42.548380 bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/hutils_viz.cpython-310.pyc
--rw-r--r--   0        0        0     2108 2023-04-09 21:44:29.698931 bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/load_save.cpython-310.pyc
--rw-r--r--   0        0        0     9148 2023-04-10 09:17:41.631628 bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/method_comparison.cpython-310.pyc
--rw-r--r--   0        0        0     7864 2023-04-08 19:37:52.265849 bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/metrics.cpython-310.pyc
--rw-r--r--   0        0        0     2738 2023-04-04 11:10:14.591320 bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/preprocessing.cpython-310.pyc
--rw-r--r--   0        0        0     9262 2023-04-08 23:26:04.015216 bk_clustering-0.1.1/bk_clustering/utilities/__pycache__/tree_traversal.cpython-310.pyc
--rw-r--r--   0        0        0     2012 2023-04-08 23:21:19.153823 bk_clustering-0.1.1/bk_clustering/utilities/calculation_utilities.py
--rw-r--r--   0        0        0     5154 2023-04-09 13:33:11.001718 bk_clustering-0.1.1/bk_clustering/utilities/cluster_calculations.py
--rw-r--r--   0        0        0     6955 2023-03-30 17:31:18.984431 bk_clustering-0.1.1/bk_clustering/utilities/density_peak.py
--rw-r--r--   0        0        0     2953 2023-04-10 14:02:09.832507 bk_clustering-0.1.1/bk_clustering/utilities/load_save.py
--rw-r--r--   0        0        0    16414 2023-04-10 13:46:07.358769 bk_clustering-0.1.1/bk_clustering/utilities/method_comparison.py
--rw-r--r--   0        0        0     8236 2023-04-08 19:36:44.802893 bk_clustering-0.1.1/bk_clustering/utilities/metrics.py
--rw-r--r--   0        0        0     4511 2023-04-09 08:12:54.956531 bk_clustering-0.1.1/bk_clustering/utilities/plot_utilities.py
--rw-r--r--   0        0        0     2582 2023-04-04 11:10:05.075192 bk_clustering-0.1.1/bk_clustering/utilities/preprocessing.py
--rw-r--r--   0        0        0    13106 2023-04-09 08:13:24.269397 bk_clustering-0.1.1/bk_clustering/utilities/tree_traversal.py
--rw-r--r--   0        0        0      441 2023-04-10 21:46:13.091338 bk_clustering-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      506 1970-01-01 00:00:00.000000 bk_clustering-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-09 12:14:06.008282 bk_clustering-0.2/README.md
+-rw-r--r--   0        0        0       40 2023-04-08 23:59:03.211844 bk_clustering-0.2/bk_clustering/__init__.py
+-rw-r--r--   0        0        0    33769 2023-03-25 12:39:17.568753 bk_clustering-0.2/bk_clustering/_hierarchy.pyx
+-rw-r--r--   0        0        0     9236 2023-04-14 23:25:00.737155 bk_clustering-0.2/bk_clustering/main.py
+-rw-r--r--   0        0        0     3586 2023-04-14 23:24:33.837484 bk_clustering-0.2/bk_clustering/run_batch.py
+-rw-r--r--   0        0        0        1 2023-04-11 00:55:31.723142 bk_clustering-0.2/bk_clustering/utilities/__init__.py
+-rw-r--r--   0        0        0     2012 2023-04-08 23:21:19.153823 bk_clustering-0.2/bk_clustering/utilities/calculation_utilities.py
+-rw-r--r--   0        0        0     5155 2023-04-11 00:55:31.879142 bk_clustering-0.2/bk_clustering/utilities/cluster_calculations.py
+-rw-r--r--   0        0        0     6955 2023-03-30 17:31:18.984431 bk_clustering-0.2/bk_clustering/utilities/density_peak.py
+-rw-r--r--   0        0        0     3788 2023-04-13 23:18:23.103160 bk_clustering-0.2/bk_clustering/utilities/load_save.py
+-rw-r--r--   0        0        0    17756 2023-04-15 17:21:26.122830 bk_clustering-0.2/bk_clustering/utilities/method_comparison.py
+-rw-r--r--   0        0        0     8278 2023-04-13 11:16:17.707177 bk_clustering-0.2/bk_clustering/utilities/metrics.py
+-rw-r--r--   0        0        0     4511 2023-04-09 08:12:54.956531 bk_clustering-0.2/bk_clustering/utilities/plot_utilities.py
+-rw-r--r--   0        0        0     2607 2023-04-15 00:03:42.881455 bk_clustering-0.2/bk_clustering/utilities/preprocessing.py
+-rw-r--r--   0        0        0    13106 2023-04-09 08:13:24.269397 bk_clustering-0.2/bk_clustering/utilities/tree_traversal.py
+-rw-r--r--   0        0        0      453 2023-04-15 17:20:13.435314 bk_clustering-0.2/pyproject.toml
+-rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 bk_clustering-0.2/PKG-INFO
```

### Comparing `bk_clustering-0.1.1/bk_clustering/_hierarchy.pyx` & `bk_clustering-0.2/bk_clustering/_hierarchy.pyx`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.1.1/bk_clustering/main.py` & `bk_clustering-0.2/bk_clustering/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 from scipy.cluster.hierarchy import linkage
 from collections import Counter
 import pandas as pd
 from timeit import default_timer as timer
 
 import sys
+
 # TODO: think of a better way
 sys.setrecursionlimit(25000)
 
+# TODO: confidence of the split through sum of solidity/number of points
+# TODO: Find dataset with ground truth for mulitlabelling?
+
 from bk_clustering.utilities import (
     calculation_utilities,
     cluster_calculations,
     tree_traversal,
     load_save,
     plot_utilities,
 )
 
+
 class BurjKhalifaClustering:
     def __init__(
         self,
         dH0: float = 0,
         depth: int = 2,
         chain_ratio: float = 5,
         parent_split_ratio: float = 10,
```

### Comparing `bk_clustering-0.1.1/bk_clustering/run_batch.py` & `bk_clustering-0.2/bk_clustering/run_batch.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,102 +1,100 @@
-import numpy as np
 from utilities import load_save, metrics, method_comparison
-import uuid
 import os
 from timeit import default_timer as timer
 from main import BurjKhalifaClustering
-from collections import Counter
 
 SKIP_COLUMNS_IN_DATASET = {
     ("real", "wdbc"): ["idnumber"],
-    ("real","spectrometer"): ["LRS-name"],
-    ("real","WISDM_ar_v1.1_transformed"): ["UNIQUE_ID"],
+    ("real", "spectrometer"): ["LRS-name"],
 }
 
+
 def run_multiple_datasets(
     dataset_names,
     depth=2,
     chain_ratio=5,
     parent_split_ratio=10,
     min_leaves=0,
     n_clusters=None,
 ):
-
     result_dict = {}
     for idx, dataset_name in enumerate(dataset_names):
         try:
-            print(dataset_name)
             start = timer()
-            skip_columns = [] if dataset_name not in SKIP_COLUMNS_IN_DATASET else SKIP_COLUMNS_IN_DATASET[dataset_name]
+            skip_columns = (
+                []
+                if dataset_name not in SKIP_COLUMNS_IN_DATASET
+                else SKIP_COLUMNS_IN_DATASET[dataset_name]
+            )
             df = load_save.read_arff(dataset_name[0], dataset_name[1], skip_columns)
             X, true_labels = df.loc[:, df.columns != "class"], df["class"]
-            bk_model = BurjKhalifaClustering(depth=depth, chain_ratio=chain_ratio, parent_split_ratio=parent_split_ratio,min_leaves=min_leaves, n_clusters =n_clusters)
+            bk_model = BurjKhalifaClustering(
+                depth=depth,
+                chain_ratio=chain_ratio,
+                parent_split_ratio=parent_split_ratio,
+                min_leaves=min_leaves,
+                n_clusters=n_clusters,
+                linkage="ward",
+            )
             bk_model.fit(X)
             predict_labels = bk_model.labels_
             error_results = metrics.calculate_metrics(true_labels, predict_labels)
             result_dict[dataset_name] = load_save.format_results(
                 error_results, timer() - start
             )
         except Exception as e:
-            print (e)
+            print(e)
 
     return result_dict
 
+
 def run_batch():
     skip_datasets = [
-        "water-treatment",
-        "audiology",
+        "water-treatment",  # no class
         "autos",
-        "credit.a",
-        "credit.g",  # copy of "german"
-        "cylinder.bands",
-        "eucalyptus",
-        "hepatitis",
-        "hypothyroid",
-        "mushroom",
-        "primary.tumor",
-        "sick",
-        "soybean",
-        "vote",
-        "Autism_Data",
-        "WISDM_ar_v1.1_transformed",
-        "Lymphoma",
+        "credit.a",  # duplicate dataset
+        "credit.g",  # duplicate dataset
+        "sick",  # duplicate dataset
+        "golfball",  # as 1 cluster, incorrect metric definition for clustering methods
         "Colon",  # multiple duplicated column names
         "jm1",  # gmm throws error
         "KDDTest+",  # gmm throws error
         "Rice_MSC_Dataset",  # run separately
-        "click_data",  # click_data - why does it takes so long for kmeans?
+        "click_data",  # takes forever long for kmeans?
     ]
     folders = ["real", "artificial"]
+
     dataset_names = []
     for folder in folders:
         dataset_names += [
             (folder, x[:-5])
             for x in os.listdir(f"./../data/{folder}")
             if x[:-5] not in skip_datasets
         ]
+
     number_of_clusters = [
         load_save.read_arff(x[0], x[1]).iloc[:, -1].nunique() for x in dataset_names
     ]
 
     # run bk_clustering
-    '''
+    """
     results = run_multiple_datasets(dataset_names)
-    filename = (
-        f"./../results/bk_clustering_results.json"  # Define the filename to save the results
-    )
+    filename = f"./../results/bk_clustering_results.json"  # Define the filename to save the results
     load_save.save_json(results, filename)  # Save the results to a JSON file
-    '''
+    """
     # method_comparison.run_birch(dataset_names, number_of_clusters)
     # method_comparison.run_dbscan(dataset_names, number_of_clusters)
     # method_comparison.run_kmeans(dataset_names, number_of_clusters)
     # method_comparison.run_kmeans_mini_batch(dataset_names, number_of_clusters)
     # method_comparison.run_mean_shift(dataset_names, number_of_clusters)
     # method_comparison.run_agglomerative(dataset_names, number_of_clusters)
+    # method_comparison.run_gmm(dataset_names, number_of_clusters)
     # method_comparison.run_affinity_propagation(dataset_names, number_of_clusters)
-    #method_comparison.run_density_peak(dataset_names, number_of_clusters)
-    #method_comparison.run_optics(dataset_names, number_of_clusters)
-    #method_comparison.run_gmm(dataset_names, number_of_clusters)
+    # method_comparison.run_density_peak(dataset_names, number_of_clusters)
+    # method_comparison.run_optics(dataset_names, number_of_clusters)
+    # method_comparison.run_hdbscan(dataset_names, number_of_clusters)
+
 
 # python3 run_batch.py
 if __name__ == "__main__":
     run_batch()
```

### Comparing `bk_clustering-0.1.1/bk_clustering/utilities/calculation_utilities.py` & `bk_clustering-0.2/bk_clustering/utilities/calculation_utilities.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.1.1/bk_clustering/utilities/cluster_calculations.py` & `bk_clustering-0.2/bk_clustering/utilities/cluster_calculations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from anytree import AnyNode
 
+
 class ClusterTree:
     def __init__(self, dtf):
         self.dtf = dtf
 
     def build_tree(self):
         self.tree_structure = {}
         for i, row in self.dtf.sort_values(by="point_id", ascending=False)[
```

### Comparing `bk_clustering-0.1.1/bk_clustering/utilities/density_peak.py` & `bk_clustering-0.2/bk_clustering/utilities/density_peak.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.1.1/bk_clustering/utilities/load_save.py` & `bk_clustering-0.2/bk_clustering/utilities/load_save.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,61 @@
 import numpy as np
+import arff
 import pandas as pd
 from scipy.io import arff as scipy_arff
 from bk_clustering.utilities import preprocessing
 import ujson
 
 
-def read_arff(folder, filename, skip_columns = []):
+def read_arff(
+    folder, filename, skip_columns=[], miss_thresh_hard=5, miss_thresh_rel=0.05
+):
     """
     Read an ARFF file from a specified folder and filename, and preprocess the data.
 
     Args:
         folder (str): The folder containing the ARFF file.
         filename (str): The filename of the ARFF file without the extension.
 
     Returns:
         pd.DataFrame: The preprocessed data as a pandas DataFrame, or None if the file is not found.
     """
     try:
         # Load ARFF data using scipy_arff and create a pandas DataFrame
         data = scipy_arff.loadarff(f"../data/{folder}/{filename}.arff")
         df = pd.DataFrame(data[0])
-        df.columns = df.columns.str.lower()  # Convert column names to lowercase
+    except NotImplementedError:
+        data = []
+        for x in arff.load(f"../data/{folder}/{filename}.arff"):
+            data.append(x._data)
+        df = pd.DataFrame(data)
+        df = df[[x for x in df.columns if type(x) == str]]
+        save_column_list = []
+        for col in df.columns:
+            if df[df[col] == ""][col].count() and (
+                df[df[col] == ""][col].count() <= miss_thresh_hard
+                or df[df[col] == ""][col].count() <= miss_thresh_rel * df.shape[0]
+            ):
+                save_column_list.append(col)
+        new_idx = df[df[save_column_list] != ""][save_column_list].dropna(axis=0).index
+        if save_column_list:
+            df = df.loc[new_idx]
+        df = df[df != ""].dropna(axis=1)
+
     except FileNotFoundError:
         print(f"Dataset {folder}/{filename} not present")
         return None  # Return None if the file is not found
+    df.columns = df.columns.str.lower()  # Convert column names to lowercase
     for col in skip_columns:
         if col in df.columns:
             df.drop(col, axis=1, inplace=True)
     df = preprocessing.preprocessing(
         df
     )  # Preprocess the data using a preprocessing function
+    df = df.dropna(axis=1)
     return df  # Return the preprocessed data as a DataFrame
 
 
 '''
 def read_dataset(filename: str, train=True, validation=True):
     """
     filename -- dataset name. Example: a1,a2,s1,etc
```

### Comparing `bk_clustering-0.1.1/bk_clustering/utilities/method_comparison.py` & `bk_clustering-0.2/bk_clustering/utilities/method_comparison.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     Birch,
     DBSCAN,
     MeanShift,
     OPTICS,
     SpectralClustering,
 )
 from sklearn.mixture import GaussianMixture
+import hdbscan
 
 
 def get_data(dataset_name: str):
     """
     Load and preprocess a dataset from an ARFF file.
 
     Args:
@@ -57,15 +58,15 @@
     results[dataset_name] = load_save.format_results(error_results, timer() - start)
 
     return results
 
 
 # TODO: itterate kmeans through different random seeds and check if some our outliered?
 # TODO: check how the results change with number of clusters mistaken
-def run_kmeans(dataset_names: List, number_of_clusters: List, random_state: int = 0):
+def run_kmeans(dataset_names: List, number_of_clusters: List, random_state: int = 1):
     """
     Run the K-means clustering algorithm on multiple datasets and collect and save the results.
 
     Args:
         dataset_names (list): A list of dataset names.
         number_of_clusters (list): A list of the number of clusters to use for each dataset.
         random_state (int): An optional random seed for reproducibility. Default is 0.
@@ -91,15 +92,15 @@
     filename = (
         f"./../results/k_means_results.json"  # Define the filename to save the results
     )
     load_save.save_json(results, filename)  # Save the results to a JSON file
 
 
 def run_kmeans_mini_batch(
-    dataset_names: List, number_of_clusters: List, random_state: int = 0
+    dataset_names: List, number_of_clusters: List, random_state: int = 1
 ):
     """
     Run the Mini-Batch K-means clustering algorithm on multiple datasets and collect and save the results.
 
     Args:
         dataset_names (list): A list of dataset names.
         number_of_clusters (list): A list of the number of clusters to use for each dataset.
@@ -124,15 +125,15 @@
         )  # Collect and store results
 
     filename = f"./../results/mini_batch_kmeans_results.json"  # Define the filename to save the results
     load_save.save_json(results, filename)  # Save the results to a JSON file
 
 
 def run_affinity_propagation(
-    dataset_names: List, number_of_clusters: List, random_state: int = 0
+    dataset_names: List, number_of_clusters: List, random_state: int = 1
 ):
     """
     Run the Affinity Propagation clustering algorithm on multiple datasets and collect and save the results.
 
     Args:
         dataset_names (list): A list of dataset names.
         number_of_clusters (list): A list of the number of clusters to use for each dataset.
@@ -184,17 +185,15 @@
         model = AgglomerativeClustering(n_clusters=n_clusters).fit(
             X
         )  # Train the Agglomerative Clustering model
         results = collect_all_results(
             results, dataset_name, true_labels, model, start
         )  # Collect and store results
 
-    filename = (
-        f"./../results/agglomerative_results.json"  # Define the filename to save the results
-    )
+    filename = f"./../results/agglomerative_results.json"  # Define the filename to save the results
     load_save.save_json(results, filename)  # Save the results to a JSON file
 
 
 def run_birch(dataset_names, number_of_clusters):
     """
     Run the Birch Clustering algorithm on multiple datasets and collect and save the results.
 
@@ -214,15 +213,17 @@
             dataset_name
         )  # Load the dataset and extract true labels
         model = Birch(n_clusters=n_clusters).fit(X)  # Train the Birch Clustering model
         results = collect_all_results(
             results, dataset_name, true_labels, model, start
         )  # Collect and store results
 
-    filename = f"./../results/birch_results.json"  # Define the filename to save the results
+    filename = (
+        f"./../results/birch_results.json"  # Define the filename to save the results
+    )
     load_save.save_json(results, filename)  # Save the results to a JSON file
 
 
 def run_dbscan(dataset_names: List, number_of_clusters: List):
     """
     Run the DBSCAN clustering algorithm on multiple datasets and collect and save the results.
 
@@ -242,15 +243,17 @@
             dataset_name
         )  # Load the dataset and extract true labels
         model = DBSCAN().fit(X)  # Train the DBSCAN model
         results = collect_all_results(
             results, dataset_name, true_labels, model, start
         )  # Collect and store results
 
-    filename = f"./../results/dbscan_results.json"  # Define the filename to save the results
+    filename = (
+        f"./../results/dbscan_results.json"  # Define the filename to save the results
+    )
     load_save.save_json(results, filename)  # Save the results to a JSON file
 
 
 def run_mean_shift(dataset_names: List, number_of_clusters: List):
     """
     Run the Mean Shift clustering algorithm on multiple datasets and collect and save the results.
 
@@ -270,17 +273,15 @@
             dataset_name
         )  # Load the dataset and extract true labels
         model = MeanShift().fit(X)  # Train the Mean Shift model
         results = collect_all_results(
             results, dataset_name, true_labels, model, start
         )  # Collect and store results
 
-    filename = (
-        f"./../results/mean_shift_results.json"  # Define the filename to save the results
-    )
+    filename = f"./../results/mean_shift_results.json"  # Define the filename to save the results
     load_save.save_json(results, filename)  # Save the results to a JSON file
 
 
 def run_optics(dataset_names: List, number_of_clusters: List):
     """
     Run the OPTICS clustering algorithm on multiple datasets and collect and save the results.
 
@@ -291,25 +292,26 @@
     Returns:
         None
     """
     results = {}  # Initialize an empty dictionary to store the results
 
     # Loop through each dataset and corresponding number of clusters
     for dataset_name, n_clusters in zip(dataset_names, number_of_clusters):
-        print(dataset_name)
         start = timer()  # Record the start time of model evaluation
         X, true_labels = get_data(
             dataset_name
         )  # Load the dataset and extract true labels
         model = OPTICS().fit(X)  # Train the OPTICS model
         results = collect_all_results(
             results, dataset_name, true_labels, model, start
         )  # Collect and store results
 
-    filename = f"./../results/optics_results.json"  # Define the filename to save the results
+    filename = (
+        f"./../results/optics_results.json"  # Define the filename to save the results
+    )
     load_save.save_json(results, filename)  # Save the results to a JSON file
 
 
 def run_spectral(dataset_names: List, number_of_clusters: List):
     """
     Run the Spectral Clustering algorithm on multiple datasets and collect and save the results.
 
@@ -337,37 +339,39 @@
 
     filename = (
         f"./../results/spectral_results.json"  # Define the filename to save the results
     )
     load_save.save_json(results, filename)  # Save the results to a JSON file
 
 
-def run_gmm(dataset_names: List, number_of_clusters: List):
+def run_gmm(dataset_names: List, number_of_clusters: List, random_state=1):
     """
     Run the Gaussian Mixture Model (GMM) clustering algorithm on multiple datasets and collect and save the results.
 
     Args:
         dataset_names (list): A list of dataset names.
         number_of_clusters (list): A list of the number of clusters to use for each dataset.
+        random_state (int): An optional random seed for reproducibility. Default is 1.
 
     Returns:
         None
     """
     results = {}  # Initialize an empty dictionary to store the results
 
     # Loop through each dataset and corresponding number of clusters
     for dataset_name, n_clusters in zip(dataset_names, number_of_clusters):
-        print(dataset_name)
         # as it was discovered for some datasets ("jm1", "KDDTest+", etc.) GaussianMixture throws an error
         try:
             start = timer()  # Record the start time of model evaluation
             X, true_labels = get_data(
                 dataset_name
             )  # Load the dataset and extract true labels
-            model = GaussianMixture(n_components=n_clusters).fit(
+            model = GaussianMixture(
+                n_components=n_clusters, random_state=random_state
+            ).fit(
                 X
             )  # Train the GMM model
             pred_labels = model.predict(X)  # Predict the cluster labels
             error_results = metrics.calculate_metrics(
                 true_labels, pred_labels
             )  # Calculate error metrics
             results[dataset_name] = load_save.format_results(
@@ -391,26 +395,52 @@
     Returns:
         None
     """
     results = {}  # Initialize an empty dictionary to store the results
 
     # Loop through each dataset and corresponding number of clusters
     for dataset_name, n_clusters in zip(dataset_names, number_of_clusters):
-        print(dataset_name)
         start = timer()  # Record the start time of model evaluation
         X, true_labels = get_data(
             dataset_name
         )  # Load the dataset and extract true labels
         pred_labels = density_peak.run_density_peak(
             X
         )  # Run the Density Peak algorithm to get predicted labels
         error_results = metrics.calculate_metrics(
             true_labels, pred_labels
         )  # Calculate clustering metrics
         results[dataset_name] = load_save.format_results(
             error_results, timer() - start
         )  # Collect and store results
 
+    filename = f"./../results/density_peak_results.json"  # Define the filename to save the results
+    load_save.save_json(results, filename)  # Save the results to a JSON file
+
+
+def run_hdbscan(dataset_names: List, number_of_clusters: List, random_state=1):
+    results = {}  # Initialize an empty dictionary to store the results
+
+    # Loop through each dataset and corresponding number of clusters
+    for dataset_name, n_clusters in zip(dataset_names, number_of_clusters):
+        try:
+            start = timer()  # Record the start time of model evaluation
+            X, true_labels = get_data(
+                dataset_name
+            )  # Load the dataset and extract true labels
+
+            model = hdbscan.HDBSCAN()
+            model.fit(X)  # Train the hdbscan model
+            pred_labels = model.labels_  # Cluster labels
+            error_results = metrics.calculate_metrics(
+                true_labels, pred_labels
+            )  # Calculate error metrics
+            results[dataset_name] = load_save.format_results(
+                error_results, timer() - start
+            )  # Collect and store results
+        except Exception as e:
+            print(e)  # Print any exception that occurs during model evaluation
+
     filename = (
-        f"./../results/density_peak_results.json"  # Define the filename to save the results
+        f"./../results/hdbscan_results.json"  # Define the filename to save the results
     )
     load_save.save_json(results, filename)  # Save the results to a JSON file
```

### Comparing `bk_clustering-0.1.1/bk_clustering/utilities/metrics.py` & `bk_clustering-0.2/bk_clustering/utilities/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,17 @@
         true_labels (List): True labels
         pred_labels (List): Predicted labels
 
     Returns:
         Tuple[float, float, float]: mutual_score, normalized_mutual_score, adjusted_mutual_score
     """
     mi = mutual_info_score(true_labels, pred_labels)
-    nmi = normalized_mutual_info_score(true_labels, pred_labels)
+    nmi = normalized_mutual_info_score(
+        true_labels, pred_labels, average_method="geometric"
+    )
     ami = adjusted_mutual_info_score(true_labels, pred_labels)
     return mi, nmi, ami
 
 
 def calculate_rand_index(true_labels: List, pred_labels: List) -> Tuple[float, float]:
     """Rand Index (RI, ARI) measures the similarity between the cluster assignments by making pair-wise comparisons.
     A higher score signifies higher similarity.
```

### Comparing `bk_clustering-0.1.1/bk_clustering/utilities/plot_utilities.py` & `bk_clustering-0.2/bk_clustering/utilities/plot_utilities.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.1.1/bk_clustering/utilities/preprocessing.py` & `bk_clustering-0.2/bk_clustering/utilities/preprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
     Return:
         df: pd.DataFrame - preprocessed pandas dataFrame
     """
     df = df.apply(pd.to_numeric, errors="ignore")
     df = string_handling(df)
     df = numeric_handling(df)
+    df = df.dropna(axis=1)
     columns = [x for x in df.columns if x != "class"] + ["class"]
     return df[columns]
 
 
 def numeric_handling(df: pd.DataFrame) -> pd.DataFrame:
     """
     Numeric handling method. Converting string to numeric where possible
@@ -67,15 +68,15 @@
     """
     for col in df.select_dtypes("object"):
         # check for binary values
         _col = df[col].str.decode(decoder)
         if not _col.isnull().all():
             df[col] = _col
 
-        # one-hot encoding
+        # dummy encoding
         if (
             create_dummy_columns
             and col != "class"
             and df[col].nunique() <= thresh_dummies
         ):
             _dummies = pd.get_dummies(df[col])
             _dummies.columns = [f"{col}_{value}" for value in _dummies.columns]
```

### Comparing `bk_clustering-0.1.1/bk_clustering/utilities/tree_traversal.py` & `bk_clustering-0.2/bk_clustering/utilities/tree_traversal.py`

 * *Files identical despite different names*

