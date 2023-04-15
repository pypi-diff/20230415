# Comparing `tmp/snc-0.1.0.tar.gz` & `tmp/snc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/snc-0.1.0.tar", last modified: Fri Jul  1 04:50:56 2022, max compression
+gzip compressed data, was "snc-0.2.0.tar", last modified: Sat Apr 15 09:19:02 2023, max compression
```

## Comparing `snc-0.1.0.tar` & `snc-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2022-07-01 04:50:56.308646 snc-0.1.0/
--rw-rw-r--   0 hj        (1010) hj        (1010)    21420 2022-07-01 04:50:56.308646 snc-0.1.0/PKG-INFO
--rw-rw-r--   0 hj        (1010) hj        (1010)    18534 2022-07-01 01:52:04.000000 snc-0.1.0/README.md
--rw-rw-r--   0 hj        (1010) hj        (1010)       38 2022-07-01 04:50:56.308646 snc-0.1.0/setup.cfg
--rw-rw-r--   0 hj        (1010) hj        (1010)      755 2022-07-01 04:49:08.000000 snc-0.1.0/setup.py
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2022-07-01 04:50:56.304646 snc-0.1.0/src/
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2022-07-01 04:50:56.304646 snc-0.1.0/src/snc/
--rw-rw-r--   0 hj        (1010) hj        (1010)       13 2022-07-01 01:52:04.000000 snc-0.1.0/src/snc/__init__.py
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2022-07-01 04:50:56.308646 snc-0.1.0/src/snc/helpers/
--rw-rw-r--   0 hj        (1010) hj        (1010)       13 2022-07-01 01:52:04.000000 snc-0.1.0/src/snc/helpers/__init__.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     1953 2022-07-01 01:52:04.000000 snc-0.1.0/src/snc/helpers/distance_matrix.py
--rw-rw-r--   0 hj        (1010) hj        (1010)    10830 2022-07-01 01:52:04.000000 snc-0.1.0/src/snc/helpers/hparam_functions.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     2836 2022-07-01 02:05:00.000000 snc-0.1.0/src/snc/helpers/snn_knn.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     3892 2022-07-01 01:52:04.000000 snc-0.1.0/src/snc/helpers/visualization.py
--rw-rw-r--   0 hj        (1010) hj        (1010)     7869 2022-07-01 02:47:59.000000 snc-0.1.0/src/snc/snc.py
-drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2022-07-01 04:50:56.308646 snc-0.1.0/src/snc.egg-info/
--rw-rw-r--   0 hj        (1010) hj        (1010)    21420 2022-07-01 04:50:56.000000 snc-0.1.0/src/snc.egg-info/PKG-INFO
--rw-rw-r--   0 hj        (1010) hj        (1010)      366 2022-07-01 04:50:56.000000 snc-0.1.0/src/snc.egg-info/SOURCES.txt
--rw-rw-r--   0 hj        (1010) hj        (1010)        1 2022-07-01 04:50:56.000000 snc-0.1.0/src/snc.egg-info/dependency_links.txt
--rw-rw-r--   0 hj        (1010) hj        (1010)       46 2022-07-01 04:50:56.000000 snc-0.1.0/src/snc.egg-info/requires.txt
--rw-rw-r--   0 hj        (1010) hj        (1010)        4 2022-07-01 04:50:56.000000 snc-0.1.0/src/snc.egg-info/top_level.txt
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-15 09:19:02.653434 snc-0.2.0/
+-rw-rw-r--   0 hj        (1010) hj        (1010)     1067 2023-04-15 01:39:47.000000 snc-0.2.0/LICENSE
+-rw-rw-r--   0 hj        (1010) hj        (1010)    19599 2023-04-15 09:19:02.653434 snc-0.2.0/PKG-INFO
+-rw-rw-r--   0 hj        (1010) hj        (1010)    19155 2023-04-15 09:18:19.000000 snc-0.2.0/README.md
+-rw-rw-r--   0 hj        (1010) hj        (1010)       38 2023-04-15 09:19:02.653434 snc-0.2.0/setup.cfg
+-rw-rw-r--   0 hj        (1010) hj        (1010)      755 2023-04-15 09:18:33.000000 snc-0.2.0/setup.py
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-15 09:19:02.649434 snc-0.2.0/src/
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-15 09:19:02.649434 snc-0.2.0/src/snc/
+-rw-rw-r--   0 hj        (1010) hj        (1010)       13 2023-04-15 01:39:47.000000 snc-0.2.0/src/snc/__init__.py
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-15 09:19:02.653434 snc-0.2.0/src/snc/helpers/
+-rw-rw-r--   0 hj        (1010) hj        (1010)       13 2023-04-15 01:39:47.000000 snc-0.2.0/src/snc/helpers/__init__.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     1953 2023-04-15 01:39:47.000000 snc-0.2.0/src/snc/helpers/distance_matrix.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)    11911 2023-04-15 02:32:27.000000 snc-0.2.0/src/snc/helpers/hparam_functions.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     2836 2023-04-15 01:39:47.000000 snc-0.2.0/src/snc/helpers/snn_knn.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     4601 2023-04-15 02:04:50.000000 snc-0.2.0/src/snc/helpers/visualization.py
+-rw-rw-r--   0 hj        (1010) hj        (1010)     8160 2023-04-15 02:20:45.000000 snc-0.2.0/src/snc/snc.py
+drwxrwxr-x   0 hj        (1010) hj        (1010)        0 2023-04-15 09:19:02.649434 snc-0.2.0/src/snc.egg-info/
+-rw-rw-r--   0 hj        (1010) hj        (1010)    19599 2023-04-15 09:19:02.000000 snc-0.2.0/src/snc.egg-info/PKG-INFO
+-rw-rw-r--   0 hj        (1010) hj        (1010)      374 2023-04-15 09:19:02.000000 snc-0.2.0/src/snc.egg-info/SOURCES.txt
+-rw-rw-r--   0 hj        (1010) hj        (1010)        1 2023-04-15 09:19:02.000000 snc-0.2.0/src/snc.egg-info/dependency_links.txt
+-rw-rw-r--   0 hj        (1010) hj        (1010)       46 2023-04-15 09:19:02.000000 snc-0.2.0/src/snc.egg-info/requires.txt
+-rw-rw-r--   0 hj        (1010) hj        (1010)        4 2023-04-15 09:19:02.000000 snc-0.2.0/src/snc.egg-info/top_level.txt
```

### Comparing `snc-0.1.0/PKG-INFO` & `snc-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,317 +1,323 @@
 Metadata-Version: 2.1
 Name: snc
-Version: 0.1.0
+Version: 0.2.0
 Summary: Implementation of Steadiness & Cohesiveness
 Home-page: https://github.com/hj-n/steadiness-cohesiveness
 Author: Hyeon Jeon
 Author-email: hj@hcil.snu.ac.kr
-License: UNKNOWN
-Description: <p align="center">
-        <img src="https://user-images.githubusercontent.com/38465539/123574467-d9c87e00-d80a-11eb-8d19-36a9f8498a95.png" alt="" data-canonical-src="https://user-images.githubusercontent.com/38465539/123574467-d9c87e00-d80a-11eb-8d19-36a9f8498a95.png" width="80%"/>
-        </p>
-        
-        <p align="center">
-          <i><b>Quality Metrics for evaluating the inter-cluster reliability of Mutldimensional Projections</b></i> 
-          <br />
-            <a href="">Docs</a>
-            ·
-        <!--     <a href=""> -->
-              <a href="http://hcil.snu.ac.kr/system/publications/pdfs/000/000/157/original/jeon_2021_tvcg.pdf?1626669574">Paper</a>
-        <!--   </a> -->
-            ·
-            <a href="mailto:hj@hcil.snu.ac.kr">Contact</a>
-          
-        </p>
-        
-        
-        ## Steadiness & Cohesiveness
-        
-        We cannot trust the embedding results (i.e., the results of multidimensional projections (MDP) such as [*t*-SNE](https://lvdmaaten.github.io/tsne/), [UMAP](https://github.com/lmcinnes/umap), or [PCA](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html)). As distortions inherently occur when reducing dimensionality, meaningful patterns in projections can be less trustworthy and thus disturb users’ accurate comprehension of the original data, leading to interpretation bias. Therefore, it is vital to measure the overall distortions using quantitative metrics or visualize where and how the distortions occurred in the projection.
-        
-        So- which aspects of MDP should we evaluate? There are numerous criteria to test if MDP well preserved the characteristics of the original high-dimensional data. Here, we focus on **inter-cluster reliability**, representing how well the projection depicts the **inter-cluster structure** (e.g., number of clusters, outliers, the distance between clusters...). It is important for MDP to have high inter-cluster reliability, as cluster analysis is one of the most critical tasks in MDP. 
-        
-        However, previous local metrics to evaluate MDP (e.g., Trustworthiness & Continuity, Mean Relative Rank Errors) focused on measuring the preservation of nearest neighbors or naively checked the maintenance of predefined clustering results or classes. These approaches cannot properly measure the reliability of the complex inter-cluster structure.
-        
-        By repeatedly extracting a random cluster from one space and measuring how well the cluster stays still in the opposite space, Steadiness & Cohesiveness measure inter-cluster reliability. Note that Steadiness measures the extent to which clusters in the projected space form clusters in the original space, and Cohesiveness measures the opposite.
-        
-        For more details, please refer to our [paper](http://hcil.snu.ac.kr/system/publications/pdfs/000/000/157/original/jeon_2021_tvcg.pdf?1626669574).
-        
-        ## Basic Usage 
-        
-        If you have trouble using Steadiness & Cohesiveness in your project or research, feel free to contact us ([hj@hcil.snu.ac.kr](mailto:hj@hcil.snu.ac.kr)).
-        We appreciate all requests about utilizing our metrics!!
-        
-        ### Installation
-        Steadiness and Cohesiveness are served with conda virtual environment.
-        
-        ```sh
-        git clone https://github.com/hj-n/steadiness-cohesiveness snc
-        conda env create -f snc/env/snc_virtual_env.yaml
-        conda activate sncvirtual
-        ```
-        
-        
-        
-        ### How to use Stediness & Cohesiveness
-        
-        ```python
-        from snc import SNC
-        
-        ...
-        
-        # k value for computing Shared Nearest Neighbor-based dissimilarity 
-        parameter = { "k": 100, "alpha": 0.1 }
-        
-        metrics = SNC(
-          raw=raw_data, 
-          emb=emb_data, 
-          iteration=300, 
-          dist_parameter = parameter
-        )
-        metrics.fit()
-        print(metrics.steadiness(), metrics.cohesiveness())
-        
-        ```
-        
-        if you installed Steadiness & Cohesiveness outside your project directory:
-        
-        ```python
-        import sys
-        
-        sys.path.append("/absolute/path/to/steadiness-cohesiveness")
-        from snc import SNC
-        
-        ...
-        ```
-        
-        As there exists a number of parameters for Steadiness & Cohesiveness, we recommend you to use the default setting (which is described in our paper) by locating the original data into `raw` and projection data into `emb` as arguments.
-        - **`raw`**: the original (raw) high-dimensional data which used to generate multidimensional projections. Should be a 2D array (or a 2D np array) with shape `(n_samples, n_dim)` where `n_samples` denotes the number of data points in dataset and `n_dim` is the original size of dimensionality (number of features).
-        - **`emb`**: the projected (embedded) data of **`raw`** (i.e., MDP result). Should be a 2D array (or a 2D np array) with shape `(n_samples, n_reduced_dim)` where `n_reduced_dim` denotes the dimensionality of projection. 
-        
-        Refer [API description](#api) for more details about hyperparameter setting.  
-        
-        ## API
-        
-        
-        ### Initialization
-        
-        ```python
-        class SNC(
-            raw, 
-            emb, 
-            iteration=200, 
-            walk_num_ratio=0.4, 
-            dist_strategy="snn", 
-            dist_paramter={}, 
-            dist_function=None,
-            cluster_strategy="dbscan"
-        )
-        ```
-        
-        > ***`raw`*** : *`Array, shape=(n_samples, n_dim), dtype=float or int`*
-        > - The original (raw) high-dimensional data used to generate MDP result.
-        > - `n_samples`: the number of data points in dataset / `n_dim`: is the original size of dimensionality
-        >
-        >
-        > ***`emb`*** : *`Array, shape=(n_samples, n_reduced_dim), dtype=float or int`*
-        > - The projected (embedded) data of **`raw`**.
-        > - `n_reduced_dim`: dimensionality of the projection
-        > 
-        > ***`iteration`*** : *`int, (optional, default: 200)`*
-        > - The number of partial distortion computation (extracting => evaluating maintainence in the opposite side).
-        > - Higher `iteration` generates the more deterministic / reliable result, but computation time increases linearly to `iteration`.
-        > - We recommend 200 iterations as a minimum.
-        > 
-        > ***`walk_num_ratio`*** : *`float, (optional, default: 0.4)`*
-        > - The amount of traverse held to extract a cluster.
-        > - For a data with `n_samples` samples, the total traverse number to extract a cluster is `n_samples * walk_num_ratio`.
-        > - The size of extracted cluster grows as `walk_num_ratio` increases, but does not effect the result significantly.
-        > 
-        > ***`dist_strategy`*** : *`string, (optional, default: "snn")`*
-        > - The selection of the way to compute distance.
-        > - We currently support: 
-        >   - `"snn"` : utilizes Shared Nearest Neighbor based on dissimilarity 
-        >   - `"euclidean"`
-        >   - `"predefined"` : allows user-defined distance function
-        > - We highly recommend to use default distance strategy "snn".
-        > - If you set `dist_strategy` as "predefined", you should also explicitly pass the way to compute distance as `dist_function` parameter. THe distance for cluster automatically computed as average linkage.
-        > 
-        > ***`dist_parameter`*** : *`dict, (optional, default: { "alpha": 0.1, "k": 100 })`*
-        > - Parameters for distance computations 
-        > - if `dist_strategy == "snn`, `dist_parameter` dictionary should hold:
-        >   - `"alpha"` : *`float, (optional, default: 0.1)`*
-        >     - The hyperparameter which panalizes low similarity between data points / clusters.
-        >     - A low `"alpha"` converts smaller similarities to higher dissimilarities (distances).
-        >   - `"k"` : *`int, (optional, default: 100)`* 
-        >     - The number of nearest neighbors for `k`-Nearest Neighbror graph which becomes a basis to compute SNN similarity.
-        > - if `dist_parameter == "euclidean"`, `dist_parameter` does nothing.
-        > - if `dist_parameter == "predefined"`, you can freely utilize `dist_parameter` in `dist_function`.
-        >   - Note that unlike `"snn"` and `"euclidean"`, the computation of "predefined" is not parallelized, thus requries much time to be computed
-        >   
-        > ***`dist_function`*** : *`function, (optional, default: None)`*
-        > - If you set `dist_strategy` as `"predefined"`, you should pass the function to calculate distance as parameter (otherwise the class raises error).
-        > - The function must get three parameters as arguments: two points `a`,`b`, their length `n_dim`, and `dist_parameter` which is given by user.
-        >   - `a` and `b` will be 1D numpy array with size `n_dim`
-        >   - `n_dim` will be an integer number
-        > - return value should be a single float value which denotes the distance between `a` and `b`.
-        >
-        > ***`cluster_strategy`*** : *`string, (optional, default: "dbscan")`*
-        > - Remind: Steadiness and Cohesiveness measures inter-cluster reliability by checking the maintenance of clusters from one space in the opposite space (Refer to [Why Steadiness and Cohesiveness](#why-steadiness-and-cohesiveness)). 
-        > - This is done by again "clustering" the cluster in the opposite side and measuring how much the cluster is splitted. `cluster_strategy` is a hyperparameter to determine the way to conduct such "clustering
-        > - We currently supports:
-        >   - `"dbscan"` : based on density-based clustering algorithm, mainly utilizing [HDBSCAN](https://hdbscan.readthedocs.io/en/latest/how_hdbscan_works.html) ligrary.
-        >   - `"x-means"` : based on X-Means clustering algorithm
-        >   - `"'K'-means"` : based on K-Means clustering algorithm, where users can freely change `'K'` value by substituting it with integer number.
-        >     - e.g., `15-means`, `20-means`, etc. 
-        
-        
-        ### Methods
-        
-        ```python3
-        SNC.fit(record_vis_info=False)
-        ```
-        
-        > Initializating Steadiness & Cohesiveness : Preprocessing (e.g., distance matrix computation) and preparation for computing Steadiness and Cohesiveness. 
-        > 
-        > ***`record_vis_info`*** : *`bool, (optional, default: False)`*
-        > - If `True`, SNC object records the information needed to make [distortion visualization of Steadiness & Cohesiveness](#visualizing-steadiness-and-cohesiveness)
-        > - method `vis_info()` becomes able to called when the parameter is set as `True`
-        > - Recording the informations incurs extra overhead!!
-        
-        
-        ```python3
-        SNC.steadiness()
-        SNC.cohesiveness()
-        ```
-        
-        > Performs the main computation of Steadiness and Cohesiveness and return the result.
-        > Note that this step generates large proportion of the computation.
-        
-        ```python3
-        SNC.vis_info(file_path=None, label=None, k=10)
-        ```
-        
-        > Able to be performed when `record_vis_info` parameter is set as `True` (Otherwise raises Error)
-        >
-        > ***`file_path`*** : *`string, (optional, default: None)`*
-        > - if `file_path` is not given as arugment, returns visualization infos
-        > - if `file_path` is given, visualization info is saved in the file with designated name (and path)
-        > - if you only designate the directory (`file_path` ends with `/`), info is saved as `info.json` inside the directory
-        > 
-        > ***`label`*** : *`Array, (optional, default: None), shape=(n_samples), dtype=int`*
-        > - 1D array which holds the label (class) information of dataset
-        > - if `None`, all points are considered to have a identical label "0"
-        > 
-        > ***`k`*** : *`int, (optional, default: 10)`*
-        > - the `k` value for constructing kNN graph used in visualization
-        
-        
-        ## Examples
-        
-        This section provides some examples to show how Steadiness and Cohesiveness respond to the projections with diverse qualities and characteristics. For more detailed experiments and evaluations, please refer to our [paper](http://hcil.snu.ac.kr/system/publications/pdfs/000/000/157/original/jeon_2021_tvcg.pdf?1626669574).
-        
-        ### vs. Varying UMAP hyperparameters
-        
-        #### Increasing `n_neighbors`
-        
-        UMAP has two important hyperparameters: `n_neighbors` (nearest neighbors) and `min_dist`. Here, we test how Steadiness and Cohesiveness vary against UMAP embeddings with increasing `n_neighbors`. `n_neighbors` denotes the number of nearest neighbors used to formulate the graph representing the original structure of data. Low `n_neighbors` values make UMAP focus more on local structure, while high values work in the opposite. 
-        
-        The [Spheres](http://proceedings.mlr.press/v119/moor20a.html) and the [Mammoth](https://pair-code.github.io/understanding-umap/) dataset are used for the test. The Spheres dataset consists of eleven spheres living in a 101-dimensional space. The dataset represents ten spheres with each consisting of 250 points, which are enclosed by another larger sphere with 2,500 points. The Mammoth dataset consists of 5,000 points constituting the 3D structure of a mammoth skeleton. 
-        
-        The UMAP projections of Mammoth (upper row) Spheres (bottom row) dataset with increasing `n_neighbors` are as follows:
-        
-        ![](https://user-images.githubusercontent.com/38465539/124187732-353f8800-daf9-11eb-9754-3c7ba19aea84.png) 
-        
-        Let's first examine the projections carefully. For the Mammoth dataset, projections with larger `n_neighbors` preserves the skeleton structure. For the Spheres dataset, you can see the points from the outer sphere (blue points) escapes from the cluster mainly formed by inner spheres when `n_neighbors` grow. Therefore, we can intuitively indicate that the projections with larger `n_neighbors` values better preserve the original inter-cluster structure for both datasets.
-        
-        Now it's time to conduct a test!! We applied Steadiness & Cohesiveness (with default hyperparameter setting) to the projections. Previous local metrics (Trustworthiness & Continuity, Mean Relative Rank Errors) with *k*=10 and global metrics (Stress, DTM) were also applied for the comparison. For global metrics, we used the values that are subtracted from 1, to assign lower values to low-quality projections.
-        
-        <p align="center">
-        <img src="https://user-images.githubusercontent.com/38465539/124186611-8a7a9a00-daf7-11eb-8df8-9ef94560467c.png" alt="" data-canonical-src="https://user-images.githubusercontent.com/38465539/124186611-8a7a9a00-daf7-11eb-8df8-9ef94560467c.png" width="80%"/>
-        </p>
-        
-        As a result, we can find that Steadiness well captured the increment of the projection quality occurred by the increasing `n_neighbors` values, both for Mammoth (left) and Spheres (right). 
-        However, Cohesiveness increased only for the Mammoth dataset.
-        Still, other metrics, except DTM, failed to capture the increment of projection quality.
-        
-        
-        
-        
-        #### Increasing `min_dist`
-        
-        Then how about `min_dist`? This time, we generated projections of [Fashion-MNIST](https://github.com/zalandoresearch/fashion-mnist) dataset with increasing `min_dist`. 
-        Alike `n_neighbors`, low `min_dist` values pack points together (focusing on local structure), and high values do the opposite. 
-        The projections and their evaluation result is as follows.
-        
-        
-        ![](https://user-images.githubusercontent.com/38465539/124188004-a121f080-daf9-11eb-818e-cf4a96990e32.png)
-        <p align="center">
-        <img src="https://user-images.githubusercontent.com/38465539/124189744-2c03ea80-dafc-11eb-89fd-38305bcec254.png" alt="" data-canonical-src="https://user-images.githubusercontent.com/38465539/124189744-2c03ea80-dafc-11eb-89fd-38305bcec254.png" width="45%"/>
-        </p>
-        
-        We previously noted that large `min_dist` values make projections focus more on the global structure. Thus, the decrement of Trustworthiness and MRRE [Missing] is quite natural, as they focus on small local structures around each point. The surprising thing here is that Cohesiveness increases as `min_dist` increases. This result indicates that classes of the Fashion-MNIST dataset are not well separated as represented in the projections with a low `min_dist` value. 
-        According to our case study (refer to the [paper](http://hcil.snu.ac.kr/system/publications/pdfs/000/000/157/original/jeon_2021_tvcg.pdf?1626669574), it is common to perceive that projections with well-divided clusters better reflect the inter-cluster structure; this result shows that such a common perception could lead to a misinterpretation of inter-cluster structure. 
-        
-        
-        
-        
-        ### Capturing PCA quality alteration
-        
-        MDP metrics *must* capture the obvious quality degradation or increment. To test our metrics' ability to capture such alteration, we conducted two tests utilizing PCA. In the first experiment, we generated 2D PCA projections of [MNIST](https://en.wikipedia.org/wiki/MNIST_database) dataset by utilizing principal component pairs with decreasing ranks (from (1st, 2nd) to (21th, 22nd)). The projections with low-rank principal components will have a lower score, as they cannot well preserve the variance of the dataset. For the second experiment, we varied the number of principal components from 2 to 22. Obviously, the quality of projections should be increase when they can utilize more principal components (i.e., lie in higher dimension). 
-        
-        <p align="center">
-        <img src="https://user-images.githubusercontent.com/38465539/124189753-2e664480-dafc-11eb-8b4b-67e3c585bdf1.png" alt="" data-canonical-src="https://user-images.githubusercontent.com/38465539/124189753-2e664480-dafc-11eb-8b4b-67e3c585bdf1.png" width="80%"/>
-        </p>
-        
-        Unsurprisingly, all metrics, including Steadiness and Cohesiveness, well captured the quality alteration for both the first (left) and the second (right) experiment. 
-        
-        
-        ## Visualizing Steadiness and Cohesiveness
-        
-        
-        ![vis](https://user-images.githubusercontent.com/38465539/123515745-b0590680-d6d3-11eb-816d-e725fd5841ee.png)
-        
-        By visualizing the result of Steadiness and Cohesiveness through the reliability map, we get more insight into how inter-cluster structure is distorted in MDP. You only need to inject visualization info file generated by `vis_info` method.
-        Please check [relability map repository](https://github.com/hj-n/snc-reliability-map) and follow the instructions to visualize Steadiness and Cohesiveness on your web browser.
-        
-        *The reliability map also supports interactions to show Missing Groups — please enjoy it!!*
-        
-        <p align="center">
-        <img src="https://user-images.githubusercontent.com/38465539/123516175-c49e0300-d6d5-11eb-9a1c-2215b924ef79.gif" alt="" data-canonical-src="https://user-images.githubusercontent.com/38465539/123516175-c49e0300-d6d5-11eb-9a1c-2215b924ef79.gif" width="55%"/>
-        </p>
-         
-        
-        ## References / Citation
-        
-        If you have used Steadiness & Cohesvieness for your project and wish to reference it, please cite our TVCG paper.
-        
-        > H. Jeon, H.-K. Ko, J. Jo, Y. Kim, and J. Seo, “Measuring and explaining the inter-cluster reliability of multidimensional projections,” *IEEE Transactions on Visualization and Computer Graphics (TVCG, Proc. VIS)*, 2021. to appear. 
-        
-        
-        #### Bibtex
-        
-        ```bib
-        @article{jeon21tvcg,
-          author={Jeon, Hyeon and Ko, Hyung-Kwon and Jo, Jaemin and Kim, Youngtaek and Seo, Jinwook},
-          journal={IEEE Transactions on Visualization and Computer Graphics (TVCG, Proc. VIS)}, 
-          title={Measuring and Explaining the Inter-Cluster Reliability of Multidimensional Projections}, 
-          year={2021},
-          note={to appear.}
-        }
-        
-        ```
-        
-        
-        ## Contributors
-        
-        [Hyeon Jeon](https://github.com/hj-n), [Hyung-Kwon Ko](https://github.com/hyungkwonko), [Jaemin Jo](https://github.com/e-), [Youngtaek Kim](https://github.com/ytaek), and Jinwook Seo.
-        
-        This software is mainly developed / maintained by Human-computer Interaction Laboratory @ Seoul National University.
-        
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center">
+<img src="https://user-images.githubusercontent.com/38465539/123574467-d9c87e00-d80a-11eb-8d19-36a9f8498a95.png" alt="" data-canonical-src="https://user-images.githubusercontent.com/38465539/123574467-d9c87e00-d80a-11eb-8d19-36a9f8498a95.png" width="80%"/>
+</p>
+
+<p align="center">
+  <i><b>Quality Metrics for evaluating the inter-cluster reliability of Mutldimensional Projections</b></i> 
+  <br />
+    <a href="">Docs</a>
+    ·
+<!--     <a href=""> -->
+      <a href="http://hcil.snu.ac.kr/system/publications/pdfs/000/000/157/original/jeon_2021_tvcg.pdf?1626669574">Paper</a>
+<!--   </a> -->
+    ·
+    <a href="mailto:hj@hcil.snu.ac.kr">Contact</a>
+  
+</p>
+
+
+## Steadiness & Cohesiveness
+
+We cannot trust the embedding results (i.e., the results of multidimensional projections (MDP) such as [*t*-SNE](https://lvdmaaten.github.io/tsne/), [UMAP](https://github.com/lmcinnes/umap), or [PCA](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html)). As distortions inherently occur when reducing dimensionality, meaningful patterns in projections can be less trustworthy and thus disturb users’ accurate comprehension of the original data, leading to interpretation bias. Therefore, it is vital to measure the overall distortions using quantitative metrics or visualize where and how the distortions occurred in the projection.
+
+So- which aspects of MDP should we evaluate? There are numerous criteria to test if MDP well preserved the characteristics of the original high-dimensional data. Here, we focus on **inter-cluster reliability**, representing how well the projection depicts the **inter-cluster structure** (e.g., number of clusters, outliers, the distance between clusters...). It is important for MDP to have high inter-cluster reliability, as cluster analysis is one of the most critical tasks in MDP. 
+
+However, previous local metrics to evaluate MDP (e.g., Trustworthiness & Continuity, Mean Relative Rank Errors) focused on measuring the preservation of nearest neighbors or naively checked the maintenance of predefined clustering results or classes. These approaches cannot properly measure the reliability of the complex inter-cluster structure.
+
+By repeatedly extracting a random cluster from one space and measuring how well the cluster stays still in the opposite space, Steadiness & Cohesiveness measure inter-cluster reliability. Note that Steadiness measures the extent to which clusters in the projected space form clusters in the original space, and Cohesiveness measures the opposite.
+
+For more details, please refer to our [paper](http://hcil.snu.ac.kr/system/publications/pdfs/000/000/157/original/jeon_2021_tvcg.pdf?1626669574).
+
+## Basic Usage 
+
+If you have trouble using Steadiness & Cohesiveness in your project or research, feel free to contact us ([hj@hcil.snu.ac.kr](mailto:hj@hcil.snu.ac.kr)).
+We appreciate all requests about utilizing our metrics!!
+
+### Installation
+Steadiness and Cohesiveness can be installed via pip
+
+```sh
+pip install snc
+```
+
+
+
+### How to use Stediness & Cohesiveness
+
+```python
+from snc.snc import SNC
+
+...
+
+parameter = { "k": 'sqrt', "alpha": 0.1 }
+
+metrics = SNC(
+  raw=raw_data, 
+  emb=emb_data, 
+  iteration=300, 
+  dist_parameter = parameter
+)
+metrics.fit()
+print(metrics.steadiness(), metrics.cohesiveness())
+
+```
+
+if you installed Steadiness & Cohesiveness outside your project directory:
+
+```python
+import sys
+
+sys.path.append("/absolute/path/to/steadiness-cohesiveness")
+from snc import SNC
+
+...
+```
+
+As there exists a number of parameters for Steadiness & Cohesiveness, we recommend you to use the default setting (which is described in our paper) by locating the original data into `raw` and projection data into `emb` as arguments.
+- **`raw`**: the original (raw) high-dimensional data which used to generate multidimensional projections. Should be a 2D array (or a 2D np array) with shape `(n_samples, n_dim)` where `n_samples` denotes the number of data points in dataset and `n_dim` is the original size of dimensionality (number of features).
+- **`emb`**: the projected (embedded) data of **`raw`** (i.e., MDP result). Should be a 2D array (or a 2D np array) with shape `(n_samples, n_reduced_dim)` where `n_reduced_dim` denotes the dimensionality of projection. 
+
+Refer [API description](#api) for more details about hyperparameter setting.  
+
+## API
+
+
+### Initialization
+
+```python
+class SNC(
+    raw, 
+    emb, 
+    iteration=150, 
+    walk_num_ratio=0.3, 
+    dist_strategy="snn", 
+    dist_paramter={}, 
+    dist_function=None,
+    cluster_strategy="dbscan",
+    snn_knn_matrix=None
+)
+```
+
+> ***`raw`*** : *`Array, shape=(n_samples, n_dim), dtype=float or int`*
+> - The original (raw) high-dimensional data used to generate MDP result.
+> - `n_samples`: the number of data points in dataset / `n_dim`: is the original size of dimensionality
+>
+>
+> ***`emb`*** : *`Array, shape=(n_samples, n_reduced_dim), dtype=float or int`*
+> - The projected (embedded) data of **`raw`**.
+> - `n_reduced_dim`: dimensionality of the projection
+> 
+> ***`iteration`*** : *`int, (optional, default: 150)`*
+> - The number of partial distortion computation (extracting => evaluating maintainence in the opposite side).
+> - Higher `iteration` generates the more deterministic / reliable result, but computation time increases linearly to `iteration`.
+> - We recommend 150 iterations as a minimum.
+> 
+> ***`walk_num_ratio`*** : *`float, (optional, default: 0.3)`*
+> - The amount of traverse held to extract a cluster.
+> - For a data with `n_samples` samples, the total traverse number to extract a cluster is `n_samples * walk_num_ratio`.
+> - The size of extracted cluster grows as `walk_num_ratio` increases, but does not effect the result significantly.
+> 
+> ***`dist_strategy`*** : *`string, (optional, default: "snn")`*
+> - The selection of the way to compute distance.
+> - We currently support: 
+>   - `"snn"` : utilizes Shared Nearest Neighbor based on dissimilarity 
+>   - `"euclidean"`
+>   - `"predefined"` : allows user-defined distance function
+>   - `"inject_snn"` : inject knn and snn info
+> - We highly recommend to use default distance strategy "snn".
+> - If you set `dist_strategy` as "predefined", you should also explicitly pass the way to compute distance as `dist_function` parameter. THe distance for cluster automatically computed as average linkage.
+> 
+> ***`dist_parameter`*** : *`dict, (optional, default: { "alpha": 0.1, "k": 'sqrt' })`*
+> - Parameters for distance computations 
+> - if `dist_strategy == "snn`, `dist_parameter` dictionary should hold:
+>   - `"alpha"` : *`float, (optional, default: 0.1)`*
+>     - The hyperparameter which panalizes low similarity between data points / clusters.
+>     - A low `"alpha"` converts smaller similarities to higher dissimilarities (distances).
+>   - `"k"` : *`int or string, (optional, default: 'sqrt')`* 
+>     - The number of nearest neighbors for `k`-Nearest Neighbror graph which becomes a basis to compute SNN similarity.
+>     - If `k == 'sqrt'`, `k` is set as the square root of the length of data
+> - if `dist_parameter == "euclidean"`, `dist_parameter` does nothing.
+> - if `dist_parameter == "predefined"`, you can freely utilize `dist_parameter` in `dist_function`.
+>   - Note that unlike `"snn"` and `"euclidean"`, the computation of "predefined" is not parallelized, thus requries much time to be computed
+>   
+> ***`dist_function`*** : *`function, (optional, default: None)`*
+> - If you set `dist_strategy` as `"predefined"`, you should pass the function to calculate distance as parameter (otherwise the class raises error).
+> - The function must get three parameters as arguments: two points `a`,`b`, their length `n_dim`, and `dist_parameter` which is given by user.
+>   - `a` and `b` will be 1D numpy array with size `n_dim`
+>   - `n_dim` will be an integer number
+> - return value should be a single float value which denotes the distance between `a` and `b`.
+>
+> ***`cluster_strategy`*** : *`string, (optional, default: "dbscan")`*
+> - Remind: Steadiness and Cohesiveness measures inter-cluster reliability by checking the maintenance of clusters from one space in the opposite space (Refer to [Why Steadiness and Cohesiveness](#why-steadiness-and-cohesiveness)). 
+> - This is done by again "clustering" the cluster in the opposite side and measuring how much the cluster is splitted. `cluster_strategy` is a hyperparameter to determine the way to conduct such "clustering
+> - We currently supports:
+>   - `"dbscan"` : based on density-based clustering algorithm, mainly utilizing [HDBSCAN](https://hdbscan.readthedocs.io/en/latest/how_hdbscan_works.html) ligrary.
+>   - `"x-means"` : based on X-Means clustering algorithm
+>   - `"'K'-means"` : based on K-Means clustering algorithm, where users can freely change `'K'` value by substituting it with integer number.
+>     - e.g., `15-means`, `20-means`, etc. 
+> ***`snn_knn_matrix`*** : *`dict, (optional, default: None)`*
+> - If you want to inject precomputed snn and knn, use this parameter
+> - To inject the parameter, you should set `dist_strategy` as `"inject_snn"`
+> - The dictionary should hold:
+>	  - `"raw_snn"` : *`Array, shape=(n_samples, n_samples), dtype=float`*, the snn matrix of raw data
+>	  - `"raw_knn"` : *`Array, shape=(n_samples, n_samples), dtype=float`*, the knn matrix of raw data
+>	  - `"emb_snn"` : *`Array, shape=(n_samples, n_samples), dtype=float`*, the snn matrix of embedded data
+>	  - `"emb_knn"` : *`Array, shape=(n_samples, n_samples), dtype=float`*, the knn matrix of embedded data
+
+### Methods
+
+```python3
+SNC.fit(record_vis_info=False)
+```
+
+> Initializating Steadiness & Cohesiveness : Preprocessing (e.g., distance matrix computation) and preparation for computing Steadiness and Cohesiveness. 
+> 
+> ***`record_vis_info`*** : *`bool, (optional, default: False)`*
+> - If `True`, SNC object records the information needed to make [distortion visualization of Steadiness & Cohesiveness](#visualizing-steadiness-and-cohesiveness)
+> - method `vis_info()` becomes able to called when the parameter is set as `True`
+> - Recording the informations incurs extra overhead!!
+
+
+```python3
+SNC.steadiness()
+SNC.cohesiveness()
+```
+
+> Performs the main computation of Steadiness and Cohesiveness and return the result.
+> Note that this step generates large proportion of the computation.
+
+```python3
+SNC.vis_info(file_path=None, label=None, k=10)
+```
+
+> Able to be performed when `record_vis_info` parameter is set as `True` (Otherwise raises Error)
+>
+> ***`file_path`*** : *`string, (optional, default: None)`*
+> - if `file_path` is not given as arugment, returns visualization infos
+> - if `file_path` is given, visualization info is saved in the file with designated name (and path)
+> - if you only designate the directory (`file_path` ends with `/`), info is saved as `info.json` inside the directory
+> 
+> ***`label`*** : *`Array, (optional, default: None), shape=(n_samples), dtype=int`*
+> - 1D array which holds the label (class) information of dataset
+> - if `None`, all points are considered to have a identical label "0"
+> 
+> ***`k`*** : *`int, (optional, default: 10)`*
+> - the `k` value for constructing kNN graph used in visualization
+
+
+## Examples
+
+This section provides some examples to show how Steadiness and Cohesiveness respond to the projections with diverse qualities and characteristics. For more detailed experiments and evaluations, please refer to our [paper](http://hcil.snu.ac.kr/system/publications/pdfs/000/000/157/original/jeon_2021_tvcg.pdf?1626669574).
+
+### vs. Varying UMAP hyperparameters
+
+#### Increasing `n_neighbors`
+
+UMAP has two important hyperparameters: `n_neighbors` (nearest neighbors) and `min_dist`. Here, we test how Steadiness and Cohesiveness vary against UMAP embeddings with increasing `n_neighbors`. `n_neighbors` denotes the number of nearest neighbors used to formulate the graph representing the original structure of data. Low `n_neighbors` values make UMAP focus more on local structure, while high values work in the opposite. 
+
+The [Spheres](http://proceedings.mlr.press/v119/moor20a.html) and the [Mammoth](https://pair-code.github.io/understanding-umap/) dataset are used for the test. The Spheres dataset consists of eleven spheres living in a 101-dimensional space. The dataset represents ten spheres with each consisting of 250 points, which are enclosed by another larger sphere with 2,500 points. The Mammoth dataset consists of 5,000 points constituting the 3D structure of a mammoth skeleton. 
+
+The UMAP projections of Mammoth (upper row) Spheres (bottom row) dataset with increasing `n_neighbors` are as follows:
+
+![](https://user-images.githubusercontent.com/38465539/124187732-353f8800-daf9-11eb-9754-3c7ba19aea84.png) 
+
+Let's first examine the projections carefully. For the Mammoth dataset, projections with larger `n_neighbors` preserves the skeleton structure. For the Spheres dataset, you can see the points from the outer sphere (blue points) escapes from the cluster mainly formed by inner spheres when `n_neighbors` grow. Therefore, we can intuitively indicate that the projections with larger `n_neighbors` values better preserve the original inter-cluster structure for both datasets.
+
+Now it's time to conduct a test!! We applied Steadiness & Cohesiveness (with default hyperparameter setting) to the projections. Previous local metrics (Trustworthiness & Continuity, Mean Relative Rank Errors) with *k*=10 and global metrics (Stress, DTM) were also applied for the comparison. For global metrics, we used the values that are subtracted from 1, to assign lower values to low-quality projections.
+
+<p align="center">
+<img src="https://user-images.githubusercontent.com/38465539/124186611-8a7a9a00-daf7-11eb-8df8-9ef94560467c.png" alt="" data-canonical-src="https://user-images.githubusercontent.com/38465539/124186611-8a7a9a00-daf7-11eb-8df8-9ef94560467c.png" width="80%"/>
+</p>
+
+As a result, we can find that Steadiness well captured the increment of the projection quality occurred by the increasing `n_neighbors` values, both for Mammoth (left) and Spheres (right). 
+However, Cohesiveness increased only for the Mammoth dataset.
+Still, other metrics, except DTM, failed to capture the increment of projection quality.
+
+
+
+
+#### Increasing `min_dist`
+
+Then how about `min_dist`? This time, we generated projections of [Fashion-MNIST](https://github.com/zalandoresearch/fashion-mnist) dataset with increasing `min_dist`. 
+Alike `n_neighbors`, low `min_dist` values pack points together (focusing on local structure), and high values do the opposite. 
+The projections and their evaluation result is as follows.
+
+
+![](https://user-images.githubusercontent.com/38465539/124188004-a121f080-daf9-11eb-818e-cf4a96990e32.png)
+<p align="center">
+<img src="https://user-images.githubusercontent.com/38465539/124189744-2c03ea80-dafc-11eb-89fd-38305bcec254.png" alt="" data-canonical-src="https://user-images.githubusercontent.com/38465539/124189744-2c03ea80-dafc-11eb-89fd-38305bcec254.png" width="45%"/>
+</p>
+
+We previously noted that large `min_dist` values make projections focus more on the global structure. Thus, the decrement of Trustworthiness and MRRE [Missing] is quite natural, as they focus on small local structures around each point. The surprising thing here is that Cohesiveness increases as `min_dist` increases. This result indicates that classes of the Fashion-MNIST dataset are not well separated as represented in the projections with a low `min_dist` value. 
+According to our case study (refer to the [paper](http://hcil.snu.ac.kr/system/publications/pdfs/000/000/157/original/jeon_2021_tvcg.pdf?1626669574), it is common to perceive that projections with well-divided clusters better reflect the inter-cluster structure; this result shows that such a common perception could lead to a misinterpretation of inter-cluster structure. 
+
+
+
+
+### Capturing PCA quality alteration
+
+MDP metrics *must* capture the obvious quality degradation or increment. To test our metrics' ability to capture such alteration, we conducted two tests utilizing PCA. In the first experiment, we generated 2D PCA projections of [MNIST](https://en.wikipedia.org/wiki/MNIST_database) dataset by utilizing principal component pairs with decreasing ranks (from (1st, 2nd) to (21th, 22nd)). The projections with low-rank principal components will have a lower score, as they cannot well preserve the variance of the dataset. For the second experiment, we varied the number of principal components from 2 to 22. Obviously, the quality of projections should be increase when they can utilize more principal components (i.e., lie in higher dimension). 
+
+<p align="center">
+<img src="https://user-images.githubusercontent.com/38465539/124189753-2e664480-dafc-11eb-8b4b-67e3c585bdf1.png" alt="" data-canonical-src="https://user-images.githubusercontent.com/38465539/124189753-2e664480-dafc-11eb-8b4b-67e3c585bdf1.png" width="80%"/>
+</p>
+
+Unsurprisingly, all metrics, including Steadiness and Cohesiveness, well captured the quality alteration for both the first (left) and the second (right) experiment. 
+
+
+## Visualizing Steadiness and Cohesiveness
+
+
+![vis](https://user-images.githubusercontent.com/38465539/123515745-b0590680-d6d3-11eb-816d-e725fd5841ee.png)
+
+By visualizing the result of Steadiness and Cohesiveness through the reliability map, we get more insight into how inter-cluster structure is distorted in MDP. You only need to inject visualization info file generated by `vis_info` method.
+Please check [relability map repository](https://github.com/hj-n/snc-reliability-map) and follow the instructions to visualize Steadiness and Cohesiveness on your web browser.
+
+*The reliability map also supports interactions to show Missing Groups — please enjoy it!!*
+
+<p align="center">
+<img src="https://user-images.githubusercontent.com/38465539/123516175-c49e0300-d6d5-11eb-9a1c-2215b924ef79.gif" alt="" data-canonical-src="https://user-images.githubusercontent.com/38465539/123516175-c49e0300-d6d5-11eb-9a1c-2215b924ef79.gif" width="55%"/>
+</p>
+ 
+
+## References / Citation
+
+If you have used Steadiness & Cohesvieness for your project and wish to reference it, please cite our TVCG paper.
+
+> H. Jeon, H.-K. Ko, J. Jo, Y. Kim, and J. Seo, “Measuring and explaining the inter-cluster reliability of multidimensional projections,” *IEEE Transactions on Visualization and Computer Graphics (TVCG, Proc. VIS)*, 2021. to appear. 
+
+
+#### Bibtex
+
+```bib
+@article{jeon21tvcg,
+  author={Jeon, Hyeon and Ko, Hyung-Kwon and Jo, Jaemin and Kim, Youngtaek and Seo, Jinwook},
+  journal={IEEE Transactions on Visualization and Computer Graphics (TVCG, Proc. VIS)}, 
+  title={Measuring and Explaining the Inter-Cluster Reliability of Multidimensional Projections}, 
+  year={2021},
+  note={to appear.}
+}
+
+```
+
+
+## Contributors
+
+[Hyeon Jeon](https://github.com/hj-n), [Hyung-Kwon Ko](https://github.com/hyungkwonko), [Jaemin Jo](https://github.com/e-), [Youngtaek Kim](https://github.com/ytaek), and Jinwook Seo.
+
+This software is mainly developed / maintained by Human-computer Interaction Laboratory @ Seoul National University.
+
```

#### html2text {}

```diff
@@ -1,11 +1,13 @@
-Metadata-Version: 2.1 Name: snc Version: 0.1.0 Summary: Implementation of
+Metadata-Version: 2.1 Name: snc Version: 0.2.0 Summary: Implementation of
 Steadiness & Cohesiveness Home-page: https://github.com/hj-n/steadiness-
-cohesiveness Author: Hyeon Jeon Author-email: hj@hcil.snu.ac.kr License:
-UNKNOWN Description:
+cohesiveness Author: Hyeon Jeon Author-email: hj@hcil.snu.ac.kr Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Requires-Python: >=3.8.5
+Description-Content-Type: text/markdown License-File: LICENSE
 Quality Metrics for evaluating the inter-cluster reliability of Mutldimensional
                                  Projections
                           Docs Â·  Paper  Â· Contact
 ## Steadiness & Cohesiveness We cannot trust the embedding results (i.e., the
 results of multidimensional projections (MDP) such as [*t*-SNE](https://
 lvdmaaten.github.io/tsne/), [UMAP](https://github.com/lmcinnes/umap), or [PCA]
 (https://scikit-learn.org/stable/modules/generated/
@@ -31,92 +33,100 @@
 Steadiness measures the extent to which clusters in the projected space form
 clusters in the original space, and Cohesiveness measures the opposite. For
 more details, please refer to our [paper](http://hcil.snu.ac.kr/system/
 publications/pdfs/000/000/157/original/jeon_2021_tvcg.pdf?1626669574). ## Basic
 Usage If you have trouble using Steadiness & Cohesiveness in your project or
 research, feel free to contact us ([hj@hcil.snu.ac.kr](mailto:
 hj@hcil.snu.ac.kr)). We appreciate all requests about utilizing our metrics!!
-### Installation Steadiness and Cohesiveness are served with conda virtual
-environment. ```sh git clone https://github.com/hj-n/steadiness-cohesiveness
-snc conda env create -f snc/env/snc_virtual_env.yaml conda activate sncvirtual
-``` ### How to use Stediness & Cohesiveness ```python from snc import SNC ... #
-k value for computing Shared Nearest Neighbor-based dissimilarity parameter =
-{ "k": 100, "alpha": 0.1 } metrics = SNC( raw=raw_data, emb=emb_data,
-iteration=300, dist_parameter = parameter ) metrics.fit() print
-(metrics.steadiness(), metrics.cohesiveness()) ``` if you installed Steadiness
-& Cohesiveness outside your project directory: ```python import sys
-sys.path.append("/absolute/path/to/steadiness-cohesiveness") from snc import
-SNC ... ``` As there exists a number of parameters for Steadiness &
+### Installation Steadiness and Cohesiveness can be installed via pip ```sh pip
+install snc ``` ### How to use Stediness & Cohesiveness ```python from snc.snc
+import SNC ... parameter = { "k": 'sqrt', "alpha": 0.1 } metrics = SNC
+( raw=raw_data, emb=emb_data, iteration=300, dist_parameter = parameter )
+metrics.fit() print(metrics.steadiness(), metrics.cohesiveness()) ``` if you
+installed Steadiness & Cohesiveness outside your project directory: ```python
+import sys sys.path.append("/absolute/path/to/steadiness-cohesiveness") from
+snc import SNC ... ``` As there exists a number of parameters for Steadiness &
 Cohesiveness, we recommend you to use the default setting (which is described
 in our paper) by locating the original data into `raw` and projection data into
 `emb` as arguments. - **`raw`**: the original (raw) high-dimensional data which
 used to generate multidimensional projections. Should be a 2D array (or a 2D np
 array) with shape `(n_samples, n_dim)` where `n_samples` denotes the number of
 data points in dataset and `n_dim` is the original size of dimensionality
 (number of features). - **`emb`**: the projected (embedded) data of **`raw`**
 (i.e., MDP result). Should be a 2D array (or a 2D np array) with shape `
 (n_samples, n_reduced_dim)` where `n_reduced_dim` denotes the dimensionality of
 projection. Refer [API description](#api) for more details about hyperparameter
 setting. ## API ### Initialization ```python class SNC( raw, emb,
-iteration=200, walk_num_ratio=0.4, dist_strategy="snn", dist_paramter={},
-dist_function=None, cluster_strategy="dbscan" ) ``` > ***`raw`*** : *`Array,
-shape=(n_samples, n_dim), dtype=float or int`* > - The original (raw) high-
-dimensional data used to generate MDP result. > - `n_samples`: the number of
-data points in dataset / `n_dim`: is the original size of dimensionality > > >
-***`emb`*** : *`Array, shape=(n_samples, n_reduced_dim), dtype=float or int`* >
-- The projected (embedded) data of **`raw`**. > - `n_reduced_dim`:
-dimensionality of the projection > > ***`iteration`*** : *`int, (optional,
-default: 200)`* > - The number of partial distortion computation (extracting =>
-evaluating maintainence in the opposite side). > - Higher `iteration` generates
-the more deterministic / reliable result, but computation time increases
-linearly to `iteration`. > - We recommend 200 iterations as a minimum. > >
-***`walk_num_ratio`*** : *`float, (optional, default: 0.4)`* > - The amount of
-traverse held to extract a cluster. > - For a data with `n_samples` samples,
-the total traverse number to extract a cluster is `n_samples * walk_num_ratio`.
-> - The size of extracted cluster grows as `walk_num_ratio` increases, but does
-not effect the result significantly. > > ***`dist_strategy`*** : *`string,
-(optional, default: "snn")`* > - The selection of the way to compute distance.
-> - We currently support: > - `"snn"` : utilizes Shared Nearest Neighbor based
-on dissimilarity > - `"euclidean"` > - `"predefined"` : allows user-defined
-distance function > - We highly recommend to use default distance strategy
-"snn". > - If you set `dist_strategy` as "predefined", you should also
-explicitly pass the way to compute distance as `dist_function` parameter. THe
-distance for cluster automatically computed as average linkage. > >
-***`dist_parameter`*** : *`dict, (optional, default: { "alpha": 0.1, "k": 100
-})`* > - Parameters for distance computations > - if `dist_strategy == "snn`,
-`dist_parameter` dictionary should hold: > - `"alpha"` : *`float, (optional,
-default: 0.1)`* > - The hyperparameter which panalizes low similarity between
-data points / clusters. > - A low `"alpha"` converts smaller similarities to
-higher dissimilarities (distances). > - `"k"` : *`int, (optional, default:
-100)`* > - The number of nearest neighbors for `k`-Nearest Neighbror graph
-which becomes a basis to compute SNN similarity. > - if `dist_parameter ==
-"euclidean"`, `dist_parameter` does nothing. > - if `dist_parameter ==
-"predefined"`, you can freely utilize `dist_parameter` in `dist_function`. > -
-Note that unlike `"snn"` and `"euclidean"`, the computation of "predefined" is
-not parallelized, thus requries much time to be computed > >
-***`dist_function`*** : *`function, (optional, default: None)`* > - If you set
-`dist_strategy` as `"predefined"`, you should pass the function to calculate
-distance as parameter (otherwise the class raises error). > - The function must
-get three parameters as arguments: two points `a`,`b`, their length `n_dim`,
-and `dist_parameter` which is given by user. > - `a` and `b` will be 1D numpy
-array with size `n_dim` > - `n_dim` will be an integer number > - return value
-should be a single float value which denotes the distance between `a` and `b`.
-> > ***`cluster_strategy`*** : *`string, (optional, default: "dbscan")`* > -
-Remind: Steadiness and Cohesiveness measures inter-cluster reliability by
-checking the maintenance of clusters from one space in the opposite space
-(Refer to [Why Steadiness and Cohesiveness](#why-steadiness-and-cohesiveness)).
-> - This is done by again "clustering" the cluster in the opposite side and
-measuring how much the cluster is splitted. `cluster_strategy` is a
-hyperparameter to determine the way to conduct such "clustering > - We
-currently supports: > - `"dbscan"` : based on density-based clustering
-algorithm, mainly utilizing [HDBSCAN](https://hdbscan.readthedocs.io/en/latest/
-how_hdbscan_works.html) ligrary. > - `"x-means"` : based on X-Means clustering
-algorithm > - `"'K'-means"` : based on K-Means clustering algorithm, where
-users can freely change `'K'` value by substituting it with integer number. > -
-e.g., `15-means`, `20-means`, etc. ### Methods ```python3 SNC.fit
+iteration=150, walk_num_ratio=0.3, dist_strategy="snn", dist_paramter={},
+dist_function=None, cluster_strategy="dbscan", snn_knn_matrix=None ) ``` >
+***`raw`*** : *`Array, shape=(n_samples, n_dim), dtype=float or int`* > - The
+original (raw) high-dimensional data used to generate MDP result. > -
+`n_samples`: the number of data points in dataset / `n_dim`: is the original
+size of dimensionality > > > ***`emb`*** : *`Array, shape=(n_samples,
+n_reduced_dim), dtype=float or int`* > - The projected (embedded) data of
+**`raw`**. > - `n_reduced_dim`: dimensionality of the projection > >
+***`iteration`*** : *`int, (optional, default: 150)`* > - The number of partial
+distortion computation (extracting => evaluating maintainence in the opposite
+side). > - Higher `iteration` generates the more deterministic / reliable
+result, but computation time increases linearly to `iteration`. > - We
+recommend 150 iterations as a minimum. > > ***`walk_num_ratio`*** : *`float,
+(optional, default: 0.3)`* > - The amount of traverse held to extract a
+cluster. > - For a data with `n_samples` samples, the total traverse number to
+extract a cluster is `n_samples * walk_num_ratio`. > - The size of extracted
+cluster grows as `walk_num_ratio` increases, but does not effect the result
+significantly. > > ***`dist_strategy`*** : *`string, (optional, default:
+"snn")`* > - The selection of the way to compute distance. > - We currently
+support: > - `"snn"` : utilizes Shared Nearest Neighbor based on dissimilarity
+> - `"euclidean"` > - `"predefined"` : allows user-defined distance function >
+- `"inject_snn"` : inject knn and snn info > - We highly recommend to use
+default distance strategy "snn". > - If you set `dist_strategy` as
+"predefined", you should also explicitly pass the way to compute distance as
+`dist_function` parameter. THe distance for cluster automatically computed as
+average linkage. > > ***`dist_parameter`*** : *`dict, (optional, default:
+{ "alpha": 0.1, "k": 'sqrt' })`* > - Parameters for distance computations > -
+if `dist_strategy == "snn`, `dist_parameter` dictionary should hold: > -
+`"alpha"` : *`float, (optional, default: 0.1)`* > - The hyperparameter which
+panalizes low similarity between data points / clusters. > - A low `"alpha"`
+converts smaller similarities to higher dissimilarities (distances). > - `"k"`
+: *`int or string, (optional, default: 'sqrt')`* > - The number of nearest
+neighbors for `k`-Nearest Neighbror graph which becomes a basis to compute SNN
+similarity. > - If `k == 'sqrt'`, `k` is set as the square root of the length
+of data > - if `dist_parameter == "euclidean"`, `dist_parameter` does nothing.
+> - if `dist_parameter == "predefined"`, you can freely utilize
+`dist_parameter` in `dist_function`. > - Note that unlike `"snn"` and
+`"euclidean"`, the computation of "predefined" is not parallelized, thus
+requries much time to be computed > > ***`dist_function`*** : *`function,
+(optional, default: None)`* > - If you set `dist_strategy` as `"predefined"`,
+you should pass the function to calculate distance as parameter (otherwise the
+class raises error). > - The function must get three parameters as arguments:
+two points `a`,`b`, their length `n_dim`, and `dist_parameter` which is given
+by user. > - `a` and `b` will be 1D numpy array with size `n_dim` > - `n_dim`
+will be an integer number > - return value should be a single float value which
+denotes the distance between `a` and `b`. > > ***`cluster_strategy`*** :
+*`string, (optional, default: "dbscan")`* > - Remind: Steadiness and
+Cohesiveness measures inter-cluster reliability by checking the maintenance of
+clusters from one space in the opposite space (Refer to [Why Steadiness and
+Cohesiveness](#why-steadiness-and-cohesiveness)). > - This is done by again
+"clustering" the cluster in the opposite side and measuring how much the
+cluster is splitted. `cluster_strategy` is a hyperparameter to determine the
+way to conduct such "clustering > - We currently supports: > - `"dbscan"` :
+based on density-based clustering algorithm, mainly utilizing [HDBSCAN](https:/
+/hdbscan.readthedocs.io/en/latest/how_hdbscan_works.html) ligrary. > - `"x-
+means"` : based on X-Means clustering algorithm > - `"'K'-means"` : based on K-
+Means clustering algorithm, where users can freely change `'K'` value by
+substituting it with integer number. > - e.g., `15-means`, `20-means`, etc. >
+***`snn_knn_matrix`*** : *`dict, (optional, default: None)`* > - If you want to
+inject precomputed snn and knn, use this parameter > - To inject the parameter,
+you should set `dist_strategy` as `"inject_snn"` > - The dictionary should
+hold: > - `"raw_snn"` : *`Array, shape=(n_samples, n_samples), dtype=float`*,
+the snn matrix of raw data > - `"raw_knn"` : *`Array, shape=(n_samples,
+n_samples), dtype=float`*, the knn matrix of raw data > - `"emb_snn"` :
+*`Array, shape=(n_samples, n_samples), dtype=float`*, the snn matrix of
+embedded data > - `"emb_knn"` : *`Array, shape=(n_samples, n_samples),
+dtype=float`*, the knn matrix of embedded data ### Methods ```python3 SNC.fit
 (record_vis_info=False) ``` > Initializating Steadiness & Cohesiveness :
 Preprocessing (e.g., distance matrix computation) and preparation for computing
 Steadiness and Cohesiveness. > > ***`record_vis_info`*** : *`bool, (optional,
 default: False)`* > - If `True`, SNC object records the information needed to
 make [distortion visualization of Steadiness & Cohesiveness](#visualizing-
 steadiness-and-cohesiveness) > - method `vis_info()` becomes able to called
 when the parameter is set as `True` > - Recording the informations incurs extra
@@ -219,11 +229,8 @@
 Jo, Jaemin and Kim, Youngtaek and Seo, Jinwook}, journal={IEEE Transactions on
 Visualization and Computer Graphics (TVCG, Proc. VIS)}, title={Measuring and
 Explaining the Inter-Cluster Reliability of Multidimensional Projections},
 year={2021}, note={to appear.} } ``` ## Contributors [Hyeon Jeon](https://
 github.com/hj-n), [Hyung-Kwon Ko](https://github.com/hyungkwonko), [Jaemin Jo]
 (https://github.com/e-), [Youngtaek Kim](https://github.com/ytaek), and Jinwook
 Seo. This software is mainly developed / maintained by Human-computer
-Interaction Laboratory @ Seoul National University. Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8.5 Description-Content-Type: text/markdown
+Interaction Laboratory @ Seoul National University.
```

### Comparing `snc-0.1.0/README.md` & `snc-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -30,33 +30,30 @@
 
 ## Basic Usage 
 
 If you have trouble using Steadiness & Cohesiveness in your project or research, feel free to contact us ([hj@hcil.snu.ac.kr](mailto:hj@hcil.snu.ac.kr)).
 We appreciate all requests about utilizing our metrics!!
 
 ### Installation
-Steadiness and Cohesiveness are served with conda virtual environment.
+Steadiness and Cohesiveness can be installed via pip
 
 ```sh
-git clone https://github.com/hj-n/steadiness-cohesiveness snc
-conda env create -f snc/env/snc_virtual_env.yaml
-conda activate sncvirtual
+pip install snc
 ```
 
 
 
 ### How to use Stediness & Cohesiveness
 
 ```python
-from snc import SNC
+from snc.snc import SNC
 
 ...
 
-# k value for computing Shared Nearest Neighbor-based dissimilarity 
-parameter = { "k": 100, "alpha": 0.1 }
+parameter = { "k": 'sqrt', "alpha": 0.1 }
 
 metrics = SNC(
   raw=raw_data, 
   emb=emb_data, 
   iteration=300, 
   dist_parameter = parameter
 )
@@ -87,59 +84,62 @@
 
 ### Initialization
 
 ```python
 class SNC(
     raw, 
     emb, 
-    iteration=200, 
-    walk_num_ratio=0.4, 
+    iteration=150, 
+    walk_num_ratio=0.3, 
     dist_strategy="snn", 
     dist_paramter={}, 
     dist_function=None,
-    cluster_strategy="dbscan"
+    cluster_strategy="dbscan",
+    snn_knn_matrix=None
 )
 ```
 
 > ***`raw`*** : *`Array, shape=(n_samples, n_dim), dtype=float or int`*
 > - The original (raw) high-dimensional data used to generate MDP result.
 > - `n_samples`: the number of data points in dataset / `n_dim`: is the original size of dimensionality
 >
 >
 > ***`emb`*** : *`Array, shape=(n_samples, n_reduced_dim), dtype=float or int`*
 > - The projected (embedded) data of **`raw`**.
 > - `n_reduced_dim`: dimensionality of the projection
 > 
-> ***`iteration`*** : *`int, (optional, default: 200)`*
+> ***`iteration`*** : *`int, (optional, default: 150)`*
 > - The number of partial distortion computation (extracting => evaluating maintainence in the opposite side).
 > - Higher `iteration` generates the more deterministic / reliable result, but computation time increases linearly to `iteration`.
-> - We recommend 200 iterations as a minimum.
+> - We recommend 150 iterations as a minimum.
 > 
-> ***`walk_num_ratio`*** : *`float, (optional, default: 0.4)`*
+> ***`walk_num_ratio`*** : *`float, (optional, default: 0.3)`*
 > - The amount of traverse held to extract a cluster.
 > - For a data with `n_samples` samples, the total traverse number to extract a cluster is `n_samples * walk_num_ratio`.
 > - The size of extracted cluster grows as `walk_num_ratio` increases, but does not effect the result significantly.
 > 
 > ***`dist_strategy`*** : *`string, (optional, default: "snn")`*
 > - The selection of the way to compute distance.
 > - We currently support: 
 >   - `"snn"` : utilizes Shared Nearest Neighbor based on dissimilarity 
 >   - `"euclidean"`
 >   - `"predefined"` : allows user-defined distance function
+>   - `"inject_snn"` : inject knn and snn info
 > - We highly recommend to use default distance strategy "snn".
 > - If you set `dist_strategy` as "predefined", you should also explicitly pass the way to compute distance as `dist_function` parameter. THe distance for cluster automatically computed as average linkage.
 > 
-> ***`dist_parameter`*** : *`dict, (optional, default: { "alpha": 0.1, "k": 100 })`*
+> ***`dist_parameter`*** : *`dict, (optional, default: { "alpha": 0.1, "k": 'sqrt' })`*
 > - Parameters for distance computations 
 > - if `dist_strategy == "snn`, `dist_parameter` dictionary should hold:
 >   - `"alpha"` : *`float, (optional, default: 0.1)`*
 >     - The hyperparameter which panalizes low similarity between data points / clusters.
 >     - A low `"alpha"` converts smaller similarities to higher dissimilarities (distances).
->   - `"k"` : *`int, (optional, default: 100)`* 
+>   - `"k"` : *`int or string, (optional, default: 'sqrt')`* 
 >     - The number of nearest neighbors for `k`-Nearest Neighbror graph which becomes a basis to compute SNN similarity.
+>     - If `k == 'sqrt'`, `k` is set as the square root of the length of data
 > - if `dist_parameter == "euclidean"`, `dist_parameter` does nothing.
 > - if `dist_parameter == "predefined"`, you can freely utilize `dist_parameter` in `dist_function`.
 >   - Note that unlike `"snn"` and `"euclidean"`, the computation of "predefined" is not parallelized, thus requries much time to be computed
 >   
 > ***`dist_function`*** : *`function, (optional, default: None)`*
 > - If you set `dist_strategy` as `"predefined"`, you should pass the function to calculate distance as parameter (otherwise the class raises error).
 > - The function must get three parameters as arguments: two points `a`,`b`, their length `n_dim`, and `dist_parameter` which is given by user.
@@ -151,15 +151,22 @@
 > - Remind: Steadiness and Cohesiveness measures inter-cluster reliability by checking the maintenance of clusters from one space in the opposite space (Refer to [Why Steadiness and Cohesiveness](#why-steadiness-and-cohesiveness)). 
 > - This is done by again "clustering" the cluster in the opposite side and measuring how much the cluster is splitted. `cluster_strategy` is a hyperparameter to determine the way to conduct such "clustering
 > - We currently supports:
 >   - `"dbscan"` : based on density-based clustering algorithm, mainly utilizing [HDBSCAN](https://hdbscan.readthedocs.io/en/latest/how_hdbscan_works.html) ligrary.
 >   - `"x-means"` : based on X-Means clustering algorithm
 >   - `"'K'-means"` : based on K-Means clustering algorithm, where users can freely change `'K'` value by substituting it with integer number.
 >     - e.g., `15-means`, `20-means`, etc. 
-
+> ***`snn_knn_matrix`*** : *`dict, (optional, default: None)`*
+> - If you want to inject precomputed snn and knn, use this parameter
+> - To inject the parameter, you should set `dist_strategy` as `"inject_snn"`
+> - The dictionary should hold:
+>	  - `"raw_snn"` : *`Array, shape=(n_samples, n_samples), dtype=float`*, the snn matrix of raw data
+>	  - `"raw_knn"` : *`Array, shape=(n_samples, n_samples), dtype=float`*, the knn matrix of raw data
+>	  - `"emb_snn"` : *`Array, shape=(n_samples, n_samples), dtype=float`*, the snn matrix of embedded data
+>	  - `"emb_knn"` : *`Array, shape=(n_samples, n_samples), dtype=float`*, the knn matrix of embedded data
 
 ### Methods
 
 ```python3
 SNC.fit(record_vis_info=False)
 ```
```

#### html2text {}

```diff
@@ -27,92 +27,100 @@
 Steadiness measures the extent to which clusters in the projected space form
 clusters in the original space, and Cohesiveness measures the opposite. For
 more details, please refer to our [paper](http://hcil.snu.ac.kr/system/
 publications/pdfs/000/000/157/original/jeon_2021_tvcg.pdf?1626669574). ## Basic
 Usage If you have trouble using Steadiness & Cohesiveness in your project or
 research, feel free to contact us ([hj@hcil.snu.ac.kr](mailto:
 hj@hcil.snu.ac.kr)). We appreciate all requests about utilizing our metrics!!
-### Installation Steadiness and Cohesiveness are served with conda virtual
-environment. ```sh git clone https://github.com/hj-n/steadiness-cohesiveness
-snc conda env create -f snc/env/snc_virtual_env.yaml conda activate sncvirtual
-``` ### How to use Stediness & Cohesiveness ```python from snc import SNC ... #
-k value for computing Shared Nearest Neighbor-based dissimilarity parameter =
-{ "k": 100, "alpha": 0.1 } metrics = SNC( raw=raw_data, emb=emb_data,
-iteration=300, dist_parameter = parameter ) metrics.fit() print
-(metrics.steadiness(), metrics.cohesiveness()) ``` if you installed Steadiness
-& Cohesiveness outside your project directory: ```python import sys
-sys.path.append("/absolute/path/to/steadiness-cohesiveness") from snc import
-SNC ... ``` As there exists a number of parameters for Steadiness &
+### Installation Steadiness and Cohesiveness can be installed via pip ```sh pip
+install snc ``` ### How to use Stediness & Cohesiveness ```python from snc.snc
+import SNC ... parameter = { "k": 'sqrt', "alpha": 0.1 } metrics = SNC
+( raw=raw_data, emb=emb_data, iteration=300, dist_parameter = parameter )
+metrics.fit() print(metrics.steadiness(), metrics.cohesiveness()) ``` if you
+installed Steadiness & Cohesiveness outside your project directory: ```python
+import sys sys.path.append("/absolute/path/to/steadiness-cohesiveness") from
+snc import SNC ... ``` As there exists a number of parameters for Steadiness &
 Cohesiveness, we recommend you to use the default setting (which is described
 in our paper) by locating the original data into `raw` and projection data into
 `emb` as arguments. - **`raw`**: the original (raw) high-dimensional data which
 used to generate multidimensional projections. Should be a 2D array (or a 2D np
 array) with shape `(n_samples, n_dim)` where `n_samples` denotes the number of
 data points in dataset and `n_dim` is the original size of dimensionality
 (number of features). - **`emb`**: the projected (embedded) data of **`raw`**
 (i.e., MDP result). Should be a 2D array (or a 2D np array) with shape `
 (n_samples, n_reduced_dim)` where `n_reduced_dim` denotes the dimensionality of
 projection. Refer [API description](#api) for more details about hyperparameter
 setting. ## API ### Initialization ```python class SNC( raw, emb,
-iteration=200, walk_num_ratio=0.4, dist_strategy="snn", dist_paramter={},
-dist_function=None, cluster_strategy="dbscan" ) ``` > ***`raw`*** : *`Array,
-shape=(n_samples, n_dim), dtype=float or int`* > - The original (raw) high-
-dimensional data used to generate MDP result. > - `n_samples`: the number of
-data points in dataset / `n_dim`: is the original size of dimensionality > > >
-***`emb`*** : *`Array, shape=(n_samples, n_reduced_dim), dtype=float or int`* >
-- The projected (embedded) data of **`raw`**. > - `n_reduced_dim`:
-dimensionality of the projection > > ***`iteration`*** : *`int, (optional,
-default: 200)`* > - The number of partial distortion computation (extracting =>
-evaluating maintainence in the opposite side). > - Higher `iteration` generates
-the more deterministic / reliable result, but computation time increases
-linearly to `iteration`. > - We recommend 200 iterations as a minimum. > >
-***`walk_num_ratio`*** : *`float, (optional, default: 0.4)`* > - The amount of
-traverse held to extract a cluster. > - For a data with `n_samples` samples,
-the total traverse number to extract a cluster is `n_samples * walk_num_ratio`.
-> - The size of extracted cluster grows as `walk_num_ratio` increases, but does
-not effect the result significantly. > > ***`dist_strategy`*** : *`string,
-(optional, default: "snn")`* > - The selection of the way to compute distance.
-> - We currently support: > - `"snn"` : utilizes Shared Nearest Neighbor based
-on dissimilarity > - `"euclidean"` > - `"predefined"` : allows user-defined
-distance function > - We highly recommend to use default distance strategy
-"snn". > - If you set `dist_strategy` as "predefined", you should also
-explicitly pass the way to compute distance as `dist_function` parameter. THe
-distance for cluster automatically computed as average linkage. > >
-***`dist_parameter`*** : *`dict, (optional, default: { "alpha": 0.1, "k": 100
-})`* > - Parameters for distance computations > - if `dist_strategy == "snn`,
-`dist_parameter` dictionary should hold: > - `"alpha"` : *`float, (optional,
-default: 0.1)`* > - The hyperparameter which panalizes low similarity between
-data points / clusters. > - A low `"alpha"` converts smaller similarities to
-higher dissimilarities (distances). > - `"k"` : *`int, (optional, default:
-100)`* > - The number of nearest neighbors for `k`-Nearest Neighbror graph
-which becomes a basis to compute SNN similarity. > - if `dist_parameter ==
-"euclidean"`, `dist_parameter` does nothing. > - if `dist_parameter ==
-"predefined"`, you can freely utilize `dist_parameter` in `dist_function`. > -
-Note that unlike `"snn"` and `"euclidean"`, the computation of "predefined" is
-not parallelized, thus requries much time to be computed > >
-***`dist_function`*** : *`function, (optional, default: None)`* > - If you set
-`dist_strategy` as `"predefined"`, you should pass the function to calculate
-distance as parameter (otherwise the class raises error). > - The function must
-get three parameters as arguments: two points `a`,`b`, their length `n_dim`,
-and `dist_parameter` which is given by user. > - `a` and `b` will be 1D numpy
-array with size `n_dim` > - `n_dim` will be an integer number > - return value
-should be a single float value which denotes the distance between `a` and `b`.
-> > ***`cluster_strategy`*** : *`string, (optional, default: "dbscan")`* > -
-Remind: Steadiness and Cohesiveness measures inter-cluster reliability by
-checking the maintenance of clusters from one space in the opposite space
-(Refer to [Why Steadiness and Cohesiveness](#why-steadiness-and-cohesiveness)).
-> - This is done by again "clustering" the cluster in the opposite side and
-measuring how much the cluster is splitted. `cluster_strategy` is a
-hyperparameter to determine the way to conduct such "clustering > - We
-currently supports: > - `"dbscan"` : based on density-based clustering
-algorithm, mainly utilizing [HDBSCAN](https://hdbscan.readthedocs.io/en/latest/
-how_hdbscan_works.html) ligrary. > - `"x-means"` : based on X-Means clustering
-algorithm > - `"'K'-means"` : based on K-Means clustering algorithm, where
-users can freely change `'K'` value by substituting it with integer number. > -
-e.g., `15-means`, `20-means`, etc. ### Methods ```python3 SNC.fit
+iteration=150, walk_num_ratio=0.3, dist_strategy="snn", dist_paramter={},
+dist_function=None, cluster_strategy="dbscan", snn_knn_matrix=None ) ``` >
+***`raw`*** : *`Array, shape=(n_samples, n_dim), dtype=float or int`* > - The
+original (raw) high-dimensional data used to generate MDP result. > -
+`n_samples`: the number of data points in dataset / `n_dim`: is the original
+size of dimensionality > > > ***`emb`*** : *`Array, shape=(n_samples,
+n_reduced_dim), dtype=float or int`* > - The projected (embedded) data of
+**`raw`**. > - `n_reduced_dim`: dimensionality of the projection > >
+***`iteration`*** : *`int, (optional, default: 150)`* > - The number of partial
+distortion computation (extracting => evaluating maintainence in the opposite
+side). > - Higher `iteration` generates the more deterministic / reliable
+result, but computation time increases linearly to `iteration`. > - We
+recommend 150 iterations as a minimum. > > ***`walk_num_ratio`*** : *`float,
+(optional, default: 0.3)`* > - The amount of traverse held to extract a
+cluster. > - For a data with `n_samples` samples, the total traverse number to
+extract a cluster is `n_samples * walk_num_ratio`. > - The size of extracted
+cluster grows as `walk_num_ratio` increases, but does not effect the result
+significantly. > > ***`dist_strategy`*** : *`string, (optional, default:
+"snn")`* > - The selection of the way to compute distance. > - We currently
+support: > - `"snn"` : utilizes Shared Nearest Neighbor based on dissimilarity
+> - `"euclidean"` > - `"predefined"` : allows user-defined distance function >
+- `"inject_snn"` : inject knn and snn info > - We highly recommend to use
+default distance strategy "snn". > - If you set `dist_strategy` as
+"predefined", you should also explicitly pass the way to compute distance as
+`dist_function` parameter. THe distance for cluster automatically computed as
+average linkage. > > ***`dist_parameter`*** : *`dict, (optional, default:
+{ "alpha": 0.1, "k": 'sqrt' })`* > - Parameters for distance computations > -
+if `dist_strategy == "snn`, `dist_parameter` dictionary should hold: > -
+`"alpha"` : *`float, (optional, default: 0.1)`* > - The hyperparameter which
+panalizes low similarity between data points / clusters. > - A low `"alpha"`
+converts smaller similarities to higher dissimilarities (distances). > - `"k"`
+: *`int or string, (optional, default: 'sqrt')`* > - The number of nearest
+neighbors for `k`-Nearest Neighbror graph which becomes a basis to compute SNN
+similarity. > - If `k == 'sqrt'`, `k` is set as the square root of the length
+of data > - if `dist_parameter == "euclidean"`, `dist_parameter` does nothing.
+> - if `dist_parameter == "predefined"`, you can freely utilize
+`dist_parameter` in `dist_function`. > - Note that unlike `"snn"` and
+`"euclidean"`, the computation of "predefined" is not parallelized, thus
+requries much time to be computed > > ***`dist_function`*** : *`function,
+(optional, default: None)`* > - If you set `dist_strategy` as `"predefined"`,
+you should pass the function to calculate distance as parameter (otherwise the
+class raises error). > - The function must get three parameters as arguments:
+two points `a`,`b`, their length `n_dim`, and `dist_parameter` which is given
+by user. > - `a` and `b` will be 1D numpy array with size `n_dim` > - `n_dim`
+will be an integer number > - return value should be a single float value which
+denotes the distance between `a` and `b`. > > ***`cluster_strategy`*** :
+*`string, (optional, default: "dbscan")`* > - Remind: Steadiness and
+Cohesiveness measures inter-cluster reliability by checking the maintenance of
+clusters from one space in the opposite space (Refer to [Why Steadiness and
+Cohesiveness](#why-steadiness-and-cohesiveness)). > - This is done by again
+"clustering" the cluster in the opposite side and measuring how much the
+cluster is splitted. `cluster_strategy` is a hyperparameter to determine the
+way to conduct such "clustering > - We currently supports: > - `"dbscan"` :
+based on density-based clustering algorithm, mainly utilizing [HDBSCAN](https:/
+/hdbscan.readthedocs.io/en/latest/how_hdbscan_works.html) ligrary. > - `"x-
+means"` : based on X-Means clustering algorithm > - `"'K'-means"` : based on K-
+Means clustering algorithm, where users can freely change `'K'` value by
+substituting it with integer number. > - e.g., `15-means`, `20-means`, etc. >
+***`snn_knn_matrix`*** : *`dict, (optional, default: None)`* > - If you want to
+inject precomputed snn and knn, use this parameter > - To inject the parameter,
+you should set `dist_strategy` as `"inject_snn"` > - The dictionary should
+hold: > - `"raw_snn"` : *`Array, shape=(n_samples, n_samples), dtype=float`*,
+the snn matrix of raw data > - `"raw_knn"` : *`Array, shape=(n_samples,
+n_samples), dtype=float`*, the knn matrix of raw data > - `"emb_snn"` :
+*`Array, shape=(n_samples, n_samples), dtype=float`*, the snn matrix of
+embedded data > - `"emb_knn"` : *`Array, shape=(n_samples, n_samples),
+dtype=float`*, the knn matrix of embedded data ### Methods ```python3 SNC.fit
 (record_vis_info=False) ``` > Initializating Steadiness & Cohesiveness :
 Preprocessing (e.g., distance matrix computation) and preparation for computing
 Steadiness and Cohesiveness. > > ***`record_vis_info`*** : *`bool, (optional,
 default: False)`* > - If `True`, SNC object records the information needed to
 make [distortion visualization of Steadiness & Cohesiveness](#visualizing-
 steadiness-and-cohesiveness) > - method `vis_info()` becomes able to called
 when the parameter is set as `True` > - Recording the informations incurs extra
```

### Comparing `snc-0.1.0/setup.py` & `snc-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="snc",
-	version="0.1.0",
+	version="0.2.0",
 	author="Hyeon Jeon",
 	author_email="hj@hcil.snu.ac.kr",
 	description="Implementation of Steadiness & Cohesiveness",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/hj-n/steadiness-cohesiveness",
 	classifiers=[
```

### Comparing `snc-0.1.0/src/snc/helpers/distance_matrix.py` & `snc-0.2.0/src/snc/helpers/distance_matrix.py`

 * *Files identical despite different names*

### Comparing `snc-0.1.0/src/snc/helpers/hparam_functions.py` & `snc-0.2.0/src/snc/helpers/hparam_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 '''
 Helper functions for generating basic infos
 e.g., knn info, distance matrix...
 '''
 
-def get_euclidean_infos(raw, emb, dist_parameter, dist_function, length, k):
+def get_euclidean_infos(raw, emb, dist_parameter, dist_function, length, k, snn_knn_matrix):
     raw_dist_matrix = dm.dist_matrix_gpu(raw)
     emb_dist_matrix = dm.dist_matrix_gpu(emb)
     
     raw_dist_max = np.max(raw_dist_matrix)
     emb_dist_max = np.max(emb_dist_matrix)
 
     raw_dist_matrix /= raw_dist_max
@@ -31,15 +31,15 @@
         "emb_dist_matrix" : emb_dist_matrix, 
         "raw_dist_max"    : raw_dist_max,
         "emb_dist_max"    : emb_dist_max, 
         "raw_knn"         : raw_knn_info,
         "emb_knn"         : emb_knn_info
     }
 
-def get_predefined_infos(raw, emb, dist_parameter, dist_function, length, k):
+def get_predefined_infos(raw, emb, dist_parameter, dist_function, length, k, snn_knn_matrix):
     raw_dist_matrix = np.zeros((length, length))
     emb_dist_matrix = np.zeros((length, length))
 
     for i in range(length):
         for j in range(length):
             raw_dist_matrix[i, j] = dist_function(raw[i], raw[j], dist_parameter)
             emb_dist_matrix[i, j] = dist_function(emb[i], emb[i], dist_parameter)
@@ -61,17 +61,17 @@
         "raw_knn"         : raw_knn_info,
         "emb_knn"         : emb_knn_info
     }
 
 
 
 
-def get_snn_infos(raw, emb, dist_parameter, dist_function, length, k):
+def get_snn_infos(raw, emb, dist_parameter, dist_function, length, k, snn_knn_matrix):
 
-    infos = get_euclidean_infos(raw, emb, dist_parameter, dist_function, length, k)
+    infos = get_euclidean_infos(raw, emb, dist_parameter, dist_function, length, k, snn_knn_matrix)
     
     # Compute snn matrix
     raw_snn_matrix = sk.snn_gpu(infos["raw_knn"], length, k)
     emb_snn_matrix = sk.snn_gpu(infos["emb_knn"], length, k)
     raw_snn_max    = np.max(raw_snn_matrix)
     emb_snn_max    = np.max(emb_snn_matrix)
 
@@ -87,14 +87,32 @@
     infos["raw_dist_matrix"] = raw_snn_dist_matrix
     infos["emb_dist_matrix"] = emb_snn_dist_matrix
     infos["raw_snn_matrix"]  = raw_snn_matrix
     infos["emb_snn_matrix"]  = emb_snn_matrix
 
     return infos
 
+def get_inject_snn_infos(raw, emb, dist_parameter, dist_function, length, k, snn_knn_matrix):
+    infos = {}
+    infos["raw_knn"] = snn_knn_matrix["raw_knn"]
+    infos["emb_knn"] = snn_knn_matrix["emb_knn"]
+    
+    infos["raw_snn_matrix"] = snn_knn_matrix["raw_snn"]
+    infos["emb_snn_matrix"] = snn_knn_matrix["emb_snn"]
+    
+    raw_snn_max		= np.max(infos["raw_snn_matrix"])
+    emb_snn_max		= np.max(infos["emb_snn_matrix"])
+    
+    infos["raw_snn_matrix"] /= raw_snn_max
+    infos["emb_snn_matrix"] /= emb_snn_max
+    
+    infos["raw_dist_matrix"] = 1 / (infos["raw_snn_matrix"] + dist_parameter["alpha"])
+    infos["emb_dist_matrix"] = 1 / (infos["emb_snn_matrix"] + dist_parameter["alpha"])
+    
+    return infos
 
 '''
 Helper functions to extract a cluster
 used to extract_cluster 
 '''
 
 def get_a_cluster_snn(infos, mode, seed_idx, walk_num):
@@ -196,15 +214,15 @@
 
     return raw_dist, emb_dist
 
 '''
 INSTALLING Hyperparameter functions
 '''
 
-def install_hparam(dist_strategy, dist_parameter, dist_function, cluster_strategy, raw, emb):
+def install_hparam(dist_strategy, dist_parameter, dist_function, cluster_strategy, snn_knn_matrix, raw, emb):
     get_infos = None
     get_a_cluster = None
     get_clusterinng = None 
     get_cluster_distance = None
 
     ## Prepare proper functions for distance strategy
     if dist_strategy == "snn": 
@@ -215,14 +233,18 @@
         get_infos = get_euclidean_infos
         get_a_cluster = get_a_cluster_naive
         get_cluster_distance = get_euc_cluster_distance
     elif dist_strategy == "predefined":
         get_infos = get_predefined_infos
         get_a_cluster = get_a_cluster_naive
         get_cluster_distance = get_predefined_cluster_distance
+    elif dist_strategy == "inject_snn":
+        get_infos = get_inject_snn_infos
+        get_a_cluster = get_a_cluster_snn
+        get_cluster_distance = get_snn_cluster_distance
     else:
         raise Exception("Wrong strategy choice!! check dist_strategy ('" + dist_strategy + "')")
 
     ## Prepare proper functions for cluster strategy
     if cluster_strategy == "dbscan":
         get_clustering = get_clustering_dbscan
     elif cluster_strategy == "x-means":
@@ -234,38 +256,40 @@
             dist_parameter["K"] = K_val
             get_clustering = get_clustering_kmeans
         else:
             raise Exception("Wrong strategy choice!! check cluster_strategy ('" + cluster_strategy + "')")
 
     return HparamFunctions(
         raw, emb, dist_parameter, dist_function,
-        get_infos, get_a_cluster, get_clustering, get_cluster_distance
+        get_infos, get_a_cluster, get_clustering, get_cluster_distance, snn_knn_matrix
     )
     
 
 class HparamFunctions():
     '''
     Saving raw, emb info and setting parameter
     '''
-    def __init__(self, raw, emb, dist_parameter, dist_function, get_infos, get_a_cluster, get_clustering, get_cluster_distance):
+    def __init__(self, raw, emb, dist_parameter, dist_function, get_infos, get_a_cluster, get_clustering, get_cluster_distance, snn_knn_matrix):
         self.raw = raw
         self.emb = emb
         self.length = len(self.raw)
         self.dist_parameter = dist_parameter
         self.dist_function  = dist_function
         self.k = dist_parameter["k"]
+        self.snn_knn_matrix = snn_knn_matrix
 
         ## Inject functions
         self.get_infos = get_infos
         self.get_a_cluster = get_a_cluster
         self.get_clustering = get_clustering
         self.get_cluster_distance = get_cluster_distance
 
+
     def preprocessing(self):
-        self.infos = self.get_infos(self.raw, self.emb, self.dist_parameter, self.dist_function, self.length, self.k)
+        self.infos = self.get_infos(self.raw, self.emb, self.dist_parameter, self.dist_function, self.length, self.k, self.snn_knn_matrix)
         dissim_matrix = self.infos["raw_dist_matrix"] - self.infos["emb_dist_matrix"]
 
         dissim_max = np.max(dissim_matrix)
         dissim_min = np.min(dissim_matrix)
 
         max_compress = dissim_max if dissim_max > 0 else 0
         min_compress = dissim_min if dissim_min > 0 else 0
```

### Comparing `snc-0.1.0/src/snc/helpers/snn_knn.py` & `snc-0.2.0/src/snc/helpers/snn_knn.py`

 * *Files identical despite different names*

### Comparing `snc-0.1.0/src/snc/helpers/visualization.py` & `snc-0.2.0/src/snc/helpers/visualization.py`

 * *Files 20% similar despite different names*

```diff
@@ -39,14 +39,25 @@
 
         edge_vis_infos.append({
             "start": nodes[0],
             "end": nodes[1],
             "missing_val": edges_cohev_info[key] * stead_score_ratio if key in edges_cohev_info else 0,
             "false_val": edges_stead_info[key] * cohev_score_ratio if key in edges_stead_info else 0
         })
+        
+    vertices_stead_info = get_vertices_info(stead_log)
+    vertices_cohev_info = get_vertices_info(cohev_log)
+    
+    vertices_vis_infos = []
+    for i, _ in enumerate(emb):
+        vertices_vis_infos.append({
+						"index": i,
+						"missing_val": vertices_cohev_info[i] * stead_score_ratio,
+						"false_val": vertices_stead_info[i] * cohev_score_ratio
+				})
 
 
     ## get missing info from cohev_log
     max_missing_val = 0
     for datum in cohev_log:
         for key in datum:
             max_missing_val = max_missing_val if datum[key] < max_missing_val else datum[key]
@@ -67,15 +78,15 @@
         info_dict = {}
         info_dict["coor"] = coor.tolist()
         info_dict["cont"] = conti_trust[i][0]
         info_dict["trust"] = conti_trust[i][1]
         info_dict["label"] = label[i] if label != None else 0
         points.append(info_dict)
 
-    return points, missing_log, edge_vis_infos
+    return points, missing_log, edge_vis_infos, vertices_vis_infos
     
   
 
 # for checkviz visualization
 # show trustworthiness / continuity score per point
 def knn_based_measure(raw, emb, raw_neighbors, emb_neighbors, k):
 
@@ -115,7 +126,18 @@
         edges_info[str(start) + "_" + str(end)] = acc
     values = edges_info.values()
     max_value = max(values)
     for key in edges_info.keys():
         edges_info[key] /= max_value
 
     return edges_info
+
+def get_vertices_info(log):
+    vertices_info = np.zeros(len(log))
+    for i, datum in enumerate(log):
+        for key in datum:
+            vertices_info[i] += datum[key]
+    max_value = max(vertices_info)
+    for i, _ in enumerate(vertices_info):
+        vertices_info[i] /= max_value
+    
+    return vertices_info
```

### Comparing `snc-0.1.0/src/snc/snc.py` & `snc-0.2.0/src/snc/snc.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,29 +13,31 @@
                  iteration=150,            # iteration number
                  walk_num_ratio=0.3,       # random walk number,
                  dist_strategy="snn",      # determines the way to compute distance 
                  dist_parameter={          # parameters used to compute distance
                      "alpha": 0.1, "k": "sqrt"
                  },        
                  dist_function=None,       # inject predefined distance function
-                 cluster_strategy="dbscan" # determines the way to consider clusters
+                 cluster_strategy="dbscan", # determines the way to consider clusters
+                 snn_knn_matrix=None,  # inject predefined similarity matrix (dist_strategy should be "inject_snn")
                 ):
         self.raw  = np.array(raw, dtype=np.float64)
         self.emb  = np.array(emb, dtype=np.float64)
         self.N    = len(raw)    # number of points
         self.iter = iteration
         self.walk_num = int(self.N * walk_num_ratio)
 
         self.dist_strategy    = dist_strategy
         if ("k" not in dist_parameter) or (dist_parameter["k"] == "sqrt"):
           dist_parameter["k"] = int(np.sqrt(self.N))
 
         self.dist_parameter   = dist_parameter
         self.dist_function    = dist_function
         self.cluster_strategy = cluster_strategy
+        self.snn_knn_matrix   = snn_knn_matrix
 
         ## target score
         self.cohev_score = None
         self.stead_score = None
 
         ## Distortion log 
         self.stead_log = [] 
@@ -59,15 +61,15 @@
         self.max_stretch  = None
         self.min_stretch  = None
         
         self.record = record_vis_info
 
         self.cstrat = hp.install_hparam(
             self.dist_strategy, self.dist_parameter, self.dist_function,
-            self.cluster_strategy,
+            self.cluster_strategy, self.snn_knn_matrix,
             self.raw, self.emb
         )
         
         self.max_compress, self.min_compress, self.max_stretch, self.min_stretch = self.cstrat.preprocessing()
 
         
 
@@ -86,40 +88,44 @@
         ## Exception handling
         if not self.record:
             raise Exception("The record_vis_info flag currently has 'False' value.")
         if not self.finished_stead:
             raise Exception("Please compute steadiness before extracting visualization infos")
         if not self.finished_cohev:
             raise Exception("Please compute cohesiveness before extracting visualization infos")
+      
+
+
 
         for datum_log in self.stead_log:
             for key_idx in datum_log:
                 datum_log[key_idx] = datum_log[key_idx][0] / datum_log[key_idx][1]
         for datum_log in self.cohev_log:
             for key_idx in datum_log:
                 datum_log[key_idx] = datum_log[key_idx][0] / datum_log[key_idx][1]
 
-        points, missing_log, edge_vis_infos = vis.generate_visualization_data( 
+        points, missing_log, edge_vis_infos, vertices_vis_infos = vis.generate_visualization_data( 
             self.stead_log, self.cohev_log, 
             self.stead_score, self.cohev_score, label, 
             self.raw, self.emb, k
         )
 
         if file_path == None:
-            return points, missing_log, edge_vis_infos
+            return points, missing_log, edge_vis_infos, vertices_vis_infos
         else:
             if file_path[-1] == "/":
                 file_path += "info.json"
             elif not (file_path[-5:] == ".json"):
                 file_path += ".json"
             with open(file_path, "w") as file:
                 json.dump({
                     "points": points,
                     "missing_info": missing_log,
-                    "edge_info": edge_vis_infos
+                    "edge_info": edge_vis_infos,
+                    "vertices_info": vertices_vis_infos
                 }, file)
 
     
 
 
     def record_result(self):
         if self.record:
```

### Comparing `snc-0.1.0/src/snc.egg-info/PKG-INFO` & `snc-0.2.0/src/snc.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,317 +1,323 @@
 Metadata-Version: 2.1
 Name: snc
-Version: 0.1.0
+Version: 0.2.0
 Summary: Implementation of Steadiness & Cohesiveness
 Home-page: https://github.com/hj-n/steadiness-cohesiveness
 Author: Hyeon Jeon
 Author-email: hj@hcil.snu.ac.kr
-License: UNKNOWN
-Description: <p align="center">
-        <img src="https://user-images.githubusercontent.com/38465539/123574467-d9c87e00-d80a-11eb-8d19-36a9f8498a95.png" alt="" data-canonical-src="https://user-images.githubusercontent.com/38465539/123574467-d9c87e00-d80a-11eb-8d19-36a9f8498a95.png" width="80%"/>
-        </p>
-        
-        <p align="center">
-          <i><b>Quality Metrics for evaluating the inter-cluster reliability of Mutldimensional Projections</b></i> 
-          <br />
-            <a href="">Docs</a>
-            ·
-        <!--     <a href=""> -->
-              <a href="http://hcil.snu.ac.kr/system/publications/pdfs/000/000/157/original/jeon_2021_tvcg.pdf?1626669574">Paper</a>
-        <!--   </a> -->
-            ·
-            <a href="mailto:hj@hcil.snu.ac.kr">Contact</a>
-          
-        </p>
-        
-        
-        ## Steadiness & Cohesiveness
-        
-        We cannot trust the embedding results (i.e., the results of multidimensional projections (MDP) such as [*t*-SNE](https://lvdmaaten.github.io/tsne/), [UMAP](https://github.com/lmcinnes/umap), or [PCA](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html)). As distortions inherently occur when reducing dimensionality, meaningful patterns in projections can be less trustworthy and thus disturb users’ accurate comprehension of the original data, leading to interpretation bias. Therefore, it is vital to measure the overall distortions using quantitative metrics or visualize where and how the distortions occurred in the projection.
-        
-        So- which aspects of MDP should we evaluate? There are numerous criteria to test if MDP well preserved the characteristics of the original high-dimensional data. Here, we focus on **inter-cluster reliability**, representing how well the projection depicts the **inter-cluster structure** (e.g., number of clusters, outliers, the distance between clusters...). It is important for MDP to have high inter-cluster reliability, as cluster analysis is one of the most critical tasks in MDP. 
-        
-        However, previous local metrics to evaluate MDP (e.g., Trustworthiness & Continuity, Mean Relative Rank Errors) focused on measuring the preservation of nearest neighbors or naively checked the maintenance of predefined clustering results or classes. These approaches cannot properly measure the reliability of the complex inter-cluster structure.
-        
-        By repeatedly extracting a random cluster from one space and measuring how well the cluster stays still in the opposite space, Steadiness & Cohesiveness measure inter-cluster reliability. Note that Steadiness measures the extent to which clusters in the projected space form clusters in the original space, and Cohesiveness measures the opposite.
-        
-        For more details, please refer to our [paper](http://hcil.snu.ac.kr/system/publications/pdfs/000/000/157/original/jeon_2021_tvcg.pdf?1626669574).
-        
-        ## Basic Usage 
-        
-        If you have trouble using Steadiness & Cohesiveness in your project or research, feel free to contact us ([hj@hcil.snu.ac.kr](mailto:hj@hcil.snu.ac.kr)).
-        We appreciate all requests about utilizing our metrics!!
-        
-        ### Installation
-        Steadiness and Cohesiveness are served with conda virtual environment.
-        
-        ```sh
-        git clone https://github.com/hj-n/steadiness-cohesiveness snc
-        conda env create -f snc/env/snc_virtual_env.yaml
-        conda activate sncvirtual
-        ```
-        
-        
-        
-        ### How to use Stediness & Cohesiveness
-        
-        ```python
-        from snc import SNC
-        
-        ...
-        
-        # k value for computing Shared Nearest Neighbor-based dissimilarity 
-        parameter = { "k": 100, "alpha": 0.1 }
-        
-        metrics = SNC(
-          raw=raw_data, 
-          emb=emb_data, 
-          iteration=300, 
-          dist_parameter = parameter
-        )
-        metrics.fit()
-        print(metrics.steadiness(), metrics.cohesiveness())
-        
-        ```
-        
-        if you installed Steadiness & Cohesiveness outside your project directory:
-        
-        ```python
-        import sys
-        
-        sys.path.append("/absolute/path/to/steadiness-cohesiveness")
-        from snc import SNC
-        
-        ...
-        ```
-        
-        As there exists a number of parameters for Steadiness & Cohesiveness, we recommend you to use the default setting (which is described in our paper) by locating the original data into `raw` and projection data into `emb` as arguments.
-        - **`raw`**: the original (raw) high-dimensional data which used to generate multidimensional projections. Should be a 2D array (or a 2D np array) with shape `(n_samples, n_dim)` where `n_samples` denotes the number of data points in dataset and `n_dim` is the original size of dimensionality (number of features).
-        - **`emb`**: the projected (embedded) data of **`raw`** (i.e., MDP result). Should be a 2D array (or a 2D np array) with shape `(n_samples, n_reduced_dim)` where `n_reduced_dim` denotes the dimensionality of projection. 
-        
-        Refer [API description](#api) for more details about hyperparameter setting.  
-        
-        ## API
-        
-        
-        ### Initialization
-        
-        ```python
-        class SNC(
-            raw, 
-            emb, 
-            iteration=200, 
-            walk_num_ratio=0.4, 
-            dist_strategy="snn", 
-            dist_paramter={}, 
-            dist_function=None,
-            cluster_strategy="dbscan"
-        )
-        ```
-        
-        > ***`raw`*** : *`Array, shape=(n_samples, n_dim), dtype=float or int`*
-        > - The original (raw) high-dimensional data used to generate MDP result.
-        > - `n_samples`: the number of data points in dataset / `n_dim`: is the original size of dimensionality
-        >
-        >
-        > ***`emb`*** : *`Array, shape=(n_samples, n_reduced_dim), dtype=float or int`*
-        > - The projected (embedded) data of **`raw`**.
-        > - `n_reduced_dim`: dimensionality of the projection
-        > 
-        > ***`iteration`*** : *`int, (optional, default: 200)`*
-        > - The number of partial distortion computation (extracting => evaluating maintainence in the opposite side).
-        > - Higher `iteration` generates the more deterministic / reliable result, but computation time increases linearly to `iteration`.
-        > - We recommend 200 iterations as a minimum.
-        > 
-        > ***`walk_num_ratio`*** : *`float, (optional, default: 0.4)`*
-        > - The amount of traverse held to extract a cluster.
-        > - For a data with `n_samples` samples, the total traverse number to extract a cluster is `n_samples * walk_num_ratio`.
-        > - The size of extracted cluster grows as `walk_num_ratio` increases, but does not effect the result significantly.
-        > 
-        > ***`dist_strategy`*** : *`string, (optional, default: "snn")`*
-        > - The selection of the way to compute distance.
-        > - We currently support: 
-        >   - `"snn"` : utilizes Shared Nearest Neighbor based on dissimilarity 
-        >   - `"euclidean"`
-        >   - `"predefined"` : allows user-defined distance function
-        > - We highly recommend to use default distance strategy "snn".
-        > - If you set `dist_strategy` as "predefined", you should also explicitly pass the way to compute distance as `dist_function` parameter. THe distance for cluster automatically computed as average linkage.
-        > 
-        > ***`dist_parameter`*** : *`dict, (optional, default: { "alpha": 0.1, "k": 100 })`*
-        > - Parameters for distance computations 
-        > - if `dist_strategy == "snn`, `dist_parameter` dictionary should hold:
-        >   - `"alpha"` : *`float, (optional, default: 0.1)`*
-        >     - The hyperparameter which panalizes low similarity between data points / clusters.
-        >     - A low `"alpha"` converts smaller similarities to higher dissimilarities (distances).
-        >   - `"k"` : *`int, (optional, default: 100)`* 
-        >     - The number of nearest neighbors for `k`-Nearest Neighbror graph which becomes a basis to compute SNN similarity.
-        > - if `dist_parameter == "euclidean"`, `dist_parameter` does nothing.
-        > - if `dist_parameter == "predefined"`, you can freely utilize `dist_parameter` in `dist_function`.
-        >   - Note that unlike `"snn"` and `"euclidean"`, the computation of "predefined" is not parallelized, thus requries much time to be computed
-        >   
-        > ***`dist_function`*** : *`function, (optional, default: None)`*
-        > - If you set `dist_strategy` as `"predefined"`, you should pass the function to calculate distance as parameter (otherwise the class raises error).
-        > - The function must get three parameters as arguments: two points `a`,`b`, their length `n_dim`, and `dist_parameter` which is given by user.
-        >   - `a` and `b` will be 1D numpy array with size `n_dim`
-        >   - `n_dim` will be an integer number
-        > - return value should be a single float value which denotes the distance between `a` and `b`.
-        >
-        > ***`cluster_strategy`*** : *`string, (optional, default: "dbscan")`*
-        > - Remind: Steadiness and Cohesiveness measures inter-cluster reliability by checking the maintenance of clusters from one space in the opposite space (Refer to [Why Steadiness and Cohesiveness](#why-steadiness-and-cohesiveness)). 
-        > - This is done by again "clustering" the cluster in the opposite side and measuring how much the cluster is splitted. `cluster_strategy` is a hyperparameter to determine the way to conduct such "clustering
-        > - We currently supports:
-        >   - `"dbscan"` : based on density-based clustering algorithm, mainly utilizing [HDBSCAN](https://hdbscan.readthedocs.io/en/latest/how_hdbscan_works.html) ligrary.
-        >   - `"x-means"` : based on X-Means clustering algorithm
-        >   - `"'K'-means"` : based on K-Means clustering algorithm, where users can freely change `'K'` value by substituting it with integer number.
-        >     - e.g., `15-means`, `20-means`, etc. 
-        
-        
-        ### Methods
-        
-        ```python3
-        SNC.fit(record_vis_info=False)
-        ```
-        
-        > Initializating Steadiness & Cohesiveness : Preprocessing (e.g., distance matrix computation) and preparation for computing Steadiness and Cohesiveness. 
-        > 
-        > ***`record_vis_info`*** : *`bool, (optional, default: False)`*
-        > - If `True`, SNC object records the information needed to make [distortion visualization of Steadiness & Cohesiveness](#visualizing-steadiness-and-cohesiveness)
-        > - method `vis_info()` becomes able to called when the parameter is set as `True`
-        > - Recording the informations incurs extra overhead!!
-        
-        
-        ```python3
-        SNC.steadiness()
-        SNC.cohesiveness()
-        ```
-        
-        > Performs the main computation of Steadiness and Cohesiveness and return the result.
-        > Note that this step generates large proportion of the computation.
-        
-        ```python3
-        SNC.vis_info(file_path=None, label=None, k=10)
-        ```
-        
-        > Able to be performed when `record_vis_info` parameter is set as `True` (Otherwise raises Error)
-        >
-        > ***`file_path`*** : *`string, (optional, default: None)`*
-        > - if `file_path` is not given as arugment, returns visualization infos
-        > - if `file_path` is given, visualization info is saved in the file with designated name (and path)
-        > - if you only designate the directory (`file_path` ends with `/`), info is saved as `info.json` inside the directory
-        > 
-        > ***`label`*** : *`Array, (optional, default: None), shape=(n_samples), dtype=int`*
-        > - 1D array which holds the label (class) information of dataset
-        > - if `None`, all points are considered to have a identical label "0"
-        > 
-        > ***`k`*** : *`int, (optional, default: 10)`*
-        > - the `k` value for constructing kNN graph used in visualization
-        
-        
-        ## Examples
-        
-        This section provides some examples to show how Steadiness and Cohesiveness respond to the projections with diverse qualities and characteristics. For more detailed experiments and evaluations, please refer to our [paper](http://hcil.snu.ac.kr/system/publications/pdfs/000/000/157/original/jeon_2021_tvcg.pdf?1626669574).
-        
-        ### vs. Varying UMAP hyperparameters
-        
-        #### Increasing `n_neighbors`
-        
-        UMAP has two important hyperparameters: `n_neighbors` (nearest neighbors) and `min_dist`. Here, we test how Steadiness and Cohesiveness vary against UMAP embeddings with increasing `n_neighbors`. `n_neighbors` denotes the number of nearest neighbors used to formulate the graph representing the original structure of data. Low `n_neighbors` values make UMAP focus more on local structure, while high values work in the opposite. 
-        
-        The [Spheres](http://proceedings.mlr.press/v119/moor20a.html) and the [Mammoth](https://pair-code.github.io/understanding-umap/) dataset are used for the test. The Spheres dataset consists of eleven spheres living in a 101-dimensional space. The dataset represents ten spheres with each consisting of 250 points, which are enclosed by another larger sphere with 2,500 points. The Mammoth dataset consists of 5,000 points constituting the 3D structure of a mammoth skeleton. 
-        
-        The UMAP projections of Mammoth (upper row) Spheres (bottom row) dataset with increasing `n_neighbors` are as follows:
-        
-        ![](https://user-images.githubusercontent.com/38465539/124187732-353f8800-daf9-11eb-9754-3c7ba19aea84.png) 
-        
-        Let's first examine the projections carefully. For the Mammoth dataset, projections with larger `n_neighbors` preserves the skeleton structure. For the Spheres dataset, you can see the points from the outer sphere (blue points) escapes from the cluster mainly formed by inner spheres when `n_neighbors` grow. Therefore, we can intuitively indicate that the projections with larger `n_neighbors` values better preserve the original inter-cluster structure for both datasets.
-        
-        Now it's time to conduct a test!! We applied Steadiness & Cohesiveness (with default hyperparameter setting) to the projections. Previous local metrics (Trustworthiness & Continuity, Mean Relative Rank Errors) with *k*=10 and global metrics (Stress, DTM) were also applied for the comparison. For global metrics, we used the values that are subtracted from 1, to assign lower values to low-quality projections.
-        
-        <p align="center">
-        <img src="https://user-images.githubusercontent.com/38465539/124186611-8a7a9a00-daf7-11eb-8df8-9ef94560467c.png" alt="" data-canonical-src="https://user-images.githubusercontent.com/38465539/124186611-8a7a9a00-daf7-11eb-8df8-9ef94560467c.png" width="80%"/>
-        </p>
-        
-        As a result, we can find that Steadiness well captured the increment of the projection quality occurred by the increasing `n_neighbors` values, both for Mammoth (left) and Spheres (right). 
-        However, Cohesiveness increased only for the Mammoth dataset.
-        Still, other metrics, except DTM, failed to capture the increment of projection quality.
-        
-        
-        
-        
-        #### Increasing `min_dist`
-        
-        Then how about `min_dist`? This time, we generated projections of [Fashion-MNIST](https://github.com/zalandoresearch/fashion-mnist) dataset with increasing `min_dist`. 
-        Alike `n_neighbors`, low `min_dist` values pack points together (focusing on local structure), and high values do the opposite. 
-        The projections and their evaluation result is as follows.
-        
-        
-        ![](https://user-images.githubusercontent.com/38465539/124188004-a121f080-daf9-11eb-818e-cf4a96990e32.png)
-        <p align="center">
-        <img src="https://user-images.githubusercontent.com/38465539/124189744-2c03ea80-dafc-11eb-89fd-38305bcec254.png" alt="" data-canonical-src="https://user-images.githubusercontent.com/38465539/124189744-2c03ea80-dafc-11eb-89fd-38305bcec254.png" width="45%"/>
-        </p>
-        
-        We previously noted that large `min_dist` values make projections focus more on the global structure. Thus, the decrement of Trustworthiness and MRRE [Missing] is quite natural, as they focus on small local structures around each point. The surprising thing here is that Cohesiveness increases as `min_dist` increases. This result indicates that classes of the Fashion-MNIST dataset are not well separated as represented in the projections with a low `min_dist` value. 
-        According to our case study (refer to the [paper](http://hcil.snu.ac.kr/system/publications/pdfs/000/000/157/original/jeon_2021_tvcg.pdf?1626669574), it is common to perceive that projections with well-divided clusters better reflect the inter-cluster structure; this result shows that such a common perception could lead to a misinterpretation of inter-cluster structure. 
-        
-        
-        
-        
-        ### Capturing PCA quality alteration
-        
-        MDP metrics *must* capture the obvious quality degradation or increment. To test our metrics' ability to capture such alteration, we conducted two tests utilizing PCA. In the first experiment, we generated 2D PCA projections of [MNIST](https://en.wikipedia.org/wiki/MNIST_database) dataset by utilizing principal component pairs with decreasing ranks (from (1st, 2nd) to (21th, 22nd)). The projections with low-rank principal components will have a lower score, as they cannot well preserve the variance of the dataset. For the second experiment, we varied the number of principal components from 2 to 22. Obviously, the quality of projections should be increase when they can utilize more principal components (i.e., lie in higher dimension). 
-        
-        <p align="center">
-        <img src="https://user-images.githubusercontent.com/38465539/124189753-2e664480-dafc-11eb-8b4b-67e3c585bdf1.png" alt="" data-canonical-src="https://user-images.githubusercontent.com/38465539/124189753-2e664480-dafc-11eb-8b4b-67e3c585bdf1.png" width="80%"/>
-        </p>
-        
-        Unsurprisingly, all metrics, including Steadiness and Cohesiveness, well captured the quality alteration for both the first (left) and the second (right) experiment. 
-        
-        
-        ## Visualizing Steadiness and Cohesiveness
-        
-        
-        ![vis](https://user-images.githubusercontent.com/38465539/123515745-b0590680-d6d3-11eb-816d-e725fd5841ee.png)
-        
-        By visualizing the result of Steadiness and Cohesiveness through the reliability map, we get more insight into how inter-cluster structure is distorted in MDP. You only need to inject visualization info file generated by `vis_info` method.
-        Please check [relability map repository](https://github.com/hj-n/snc-reliability-map) and follow the instructions to visualize Steadiness and Cohesiveness on your web browser.
-        
-        *The reliability map also supports interactions to show Missing Groups — please enjoy it!!*
-        
-        <p align="center">
-        <img src="https://user-images.githubusercontent.com/38465539/123516175-c49e0300-d6d5-11eb-9a1c-2215b924ef79.gif" alt="" data-canonical-src="https://user-images.githubusercontent.com/38465539/123516175-c49e0300-d6d5-11eb-9a1c-2215b924ef79.gif" width="55%"/>
-        </p>
-         
-        
-        ## References / Citation
-        
-        If you have used Steadiness & Cohesvieness for your project and wish to reference it, please cite our TVCG paper.
-        
-        > H. Jeon, H.-K. Ko, J. Jo, Y. Kim, and J. Seo, “Measuring and explaining the inter-cluster reliability of multidimensional projections,” *IEEE Transactions on Visualization and Computer Graphics (TVCG, Proc. VIS)*, 2021. to appear. 
-        
-        
-        #### Bibtex
-        
-        ```bib
-        @article{jeon21tvcg,
-          author={Jeon, Hyeon and Ko, Hyung-Kwon and Jo, Jaemin and Kim, Youngtaek and Seo, Jinwook},
-          journal={IEEE Transactions on Visualization and Computer Graphics (TVCG, Proc. VIS)}, 
-          title={Measuring and Explaining the Inter-Cluster Reliability of Multidimensional Projections}, 
-          year={2021},
-          note={to appear.}
-        }
-        
-        ```
-        
-        
-        ## Contributors
-        
-        [Hyeon Jeon](https://github.com/hj-n), [Hyung-Kwon Ko](https://github.com/hyungkwonko), [Jaemin Jo](https://github.com/e-), [Youngtaek Kim](https://github.com/ytaek), and Jinwook Seo.
-        
-        This software is mainly developed / maintained by Human-computer Interaction Laboratory @ Seoul National University.
-        
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center">
+<img src="https://user-images.githubusercontent.com/38465539/123574467-d9c87e00-d80a-11eb-8d19-36a9f8498a95.png" alt="" data-canonical-src="https://user-images.githubusercontent.com/38465539/123574467-d9c87e00-d80a-11eb-8d19-36a9f8498a95.png" width="80%"/>
+</p>
+
+<p align="center">
+  <i><b>Quality Metrics for evaluating the inter-cluster reliability of Mutldimensional Projections</b></i> 
+  <br />
+    <a href="">Docs</a>
+    ·
+<!--     <a href=""> -->
+      <a href="http://hcil.snu.ac.kr/system/publications/pdfs/000/000/157/original/jeon_2021_tvcg.pdf?1626669574">Paper</a>
+<!--   </a> -->
+    ·
+    <a href="mailto:hj@hcil.snu.ac.kr">Contact</a>
+  
+</p>
+
+
+## Steadiness & Cohesiveness
+
+We cannot trust the embedding results (i.e., the results of multidimensional projections (MDP) such as [*t*-SNE](https://lvdmaaten.github.io/tsne/), [UMAP](https://github.com/lmcinnes/umap), or [PCA](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html)). As distortions inherently occur when reducing dimensionality, meaningful patterns in projections can be less trustworthy and thus disturb users’ accurate comprehension of the original data, leading to interpretation bias. Therefore, it is vital to measure the overall distortions using quantitative metrics or visualize where and how the distortions occurred in the projection.
+
+So- which aspects of MDP should we evaluate? There are numerous criteria to test if MDP well preserved the characteristics of the original high-dimensional data. Here, we focus on **inter-cluster reliability**, representing how well the projection depicts the **inter-cluster structure** (e.g., number of clusters, outliers, the distance between clusters...). It is important for MDP to have high inter-cluster reliability, as cluster analysis is one of the most critical tasks in MDP. 
+
+However, previous local metrics to evaluate MDP (e.g., Trustworthiness & Continuity, Mean Relative Rank Errors) focused on measuring the preservation of nearest neighbors or naively checked the maintenance of predefined clustering results or classes. These approaches cannot properly measure the reliability of the complex inter-cluster structure.
+
+By repeatedly extracting a random cluster from one space and measuring how well the cluster stays still in the opposite space, Steadiness & Cohesiveness measure inter-cluster reliability. Note that Steadiness measures the extent to which clusters in the projected space form clusters in the original space, and Cohesiveness measures the opposite.
+
+For more details, please refer to our [paper](http://hcil.snu.ac.kr/system/publications/pdfs/000/000/157/original/jeon_2021_tvcg.pdf?1626669574).
+
+## Basic Usage 
+
+If you have trouble using Steadiness & Cohesiveness in your project or research, feel free to contact us ([hj@hcil.snu.ac.kr](mailto:hj@hcil.snu.ac.kr)).
+We appreciate all requests about utilizing our metrics!!
+
+### Installation
+Steadiness and Cohesiveness can be installed via pip
+
+```sh
+pip install snc
+```
+
+
+
+### How to use Stediness & Cohesiveness
+
+```python
+from snc.snc import SNC
+
+...
+
+parameter = { "k": 'sqrt', "alpha": 0.1 }
+
+metrics = SNC(
+  raw=raw_data, 
+  emb=emb_data, 
+  iteration=300, 
+  dist_parameter = parameter
+)
+metrics.fit()
+print(metrics.steadiness(), metrics.cohesiveness())
+
+```
+
+if you installed Steadiness & Cohesiveness outside your project directory:
+
+```python
+import sys
+
+sys.path.append("/absolute/path/to/steadiness-cohesiveness")
+from snc import SNC
+
+...
+```
+
+As there exists a number of parameters for Steadiness & Cohesiveness, we recommend you to use the default setting (which is described in our paper) by locating the original data into `raw` and projection data into `emb` as arguments.
+- **`raw`**: the original (raw) high-dimensional data which used to generate multidimensional projections. Should be a 2D array (or a 2D np array) with shape `(n_samples, n_dim)` where `n_samples` denotes the number of data points in dataset and `n_dim` is the original size of dimensionality (number of features).
+- **`emb`**: the projected (embedded) data of **`raw`** (i.e., MDP result). Should be a 2D array (or a 2D np array) with shape `(n_samples, n_reduced_dim)` where `n_reduced_dim` denotes the dimensionality of projection. 
+
+Refer [API description](#api) for more details about hyperparameter setting.  
+
+## API
+
+
+### Initialization
+
+```python
+class SNC(
+    raw, 
+    emb, 
+    iteration=150, 
+    walk_num_ratio=0.3, 
+    dist_strategy="snn", 
+    dist_paramter={}, 
+    dist_function=None,
+    cluster_strategy="dbscan",
+    snn_knn_matrix=None
+)
+```
+
+> ***`raw`*** : *`Array, shape=(n_samples, n_dim), dtype=float or int`*
+> - The original (raw) high-dimensional data used to generate MDP result.
+> - `n_samples`: the number of data points in dataset / `n_dim`: is the original size of dimensionality
+>
+>
+> ***`emb`*** : *`Array, shape=(n_samples, n_reduced_dim), dtype=float or int`*
+> - The projected (embedded) data of **`raw`**.
+> - `n_reduced_dim`: dimensionality of the projection
+> 
+> ***`iteration`*** : *`int, (optional, default: 150)`*
+> - The number of partial distortion computation (extracting => evaluating maintainence in the opposite side).
+> - Higher `iteration` generates the more deterministic / reliable result, but computation time increases linearly to `iteration`.
+> - We recommend 150 iterations as a minimum.
+> 
+> ***`walk_num_ratio`*** : *`float, (optional, default: 0.3)`*
+> - The amount of traverse held to extract a cluster.
+> - For a data with `n_samples` samples, the total traverse number to extract a cluster is `n_samples * walk_num_ratio`.
+> - The size of extracted cluster grows as `walk_num_ratio` increases, but does not effect the result significantly.
+> 
+> ***`dist_strategy`*** : *`string, (optional, default: "snn")`*
+> - The selection of the way to compute distance.
+> - We currently support: 
+>   - `"snn"` : utilizes Shared Nearest Neighbor based on dissimilarity 
+>   - `"euclidean"`
+>   - `"predefined"` : allows user-defined distance function
+>   - `"inject_snn"` : inject knn and snn info
+> - We highly recommend to use default distance strategy "snn".
+> - If you set `dist_strategy` as "predefined", you should also explicitly pass the way to compute distance as `dist_function` parameter. THe distance for cluster automatically computed as average linkage.
+> 
+> ***`dist_parameter`*** : *`dict, (optional, default: { "alpha": 0.1, "k": 'sqrt' })`*
+> - Parameters for distance computations 
+> - if `dist_strategy == "snn`, `dist_parameter` dictionary should hold:
+>   - `"alpha"` : *`float, (optional, default: 0.1)`*
+>     - The hyperparameter which panalizes low similarity between data points / clusters.
+>     - A low `"alpha"` converts smaller similarities to higher dissimilarities (distances).
+>   - `"k"` : *`int or string, (optional, default: 'sqrt')`* 
+>     - The number of nearest neighbors for `k`-Nearest Neighbror graph which becomes a basis to compute SNN similarity.
+>     - If `k == 'sqrt'`, `k` is set as the square root of the length of data
+> - if `dist_parameter == "euclidean"`, `dist_parameter` does nothing.
+> - if `dist_parameter == "predefined"`, you can freely utilize `dist_parameter` in `dist_function`.
+>   - Note that unlike `"snn"` and `"euclidean"`, the computation of "predefined" is not parallelized, thus requries much time to be computed
+>   
+> ***`dist_function`*** : *`function, (optional, default: None)`*
+> - If you set `dist_strategy` as `"predefined"`, you should pass the function to calculate distance as parameter (otherwise the class raises error).
+> - The function must get three parameters as arguments: two points `a`,`b`, their length `n_dim`, and `dist_parameter` which is given by user.
+>   - `a` and `b` will be 1D numpy array with size `n_dim`
+>   - `n_dim` will be an integer number
+> - return value should be a single float value which denotes the distance between `a` and `b`.
+>
+> ***`cluster_strategy`*** : *`string, (optional, default: "dbscan")`*
+> - Remind: Steadiness and Cohesiveness measures inter-cluster reliability by checking the maintenance of clusters from one space in the opposite space (Refer to [Why Steadiness and Cohesiveness](#why-steadiness-and-cohesiveness)). 
+> - This is done by again "clustering" the cluster in the opposite side and measuring how much the cluster is splitted. `cluster_strategy` is a hyperparameter to determine the way to conduct such "clustering
+> - We currently supports:
+>   - `"dbscan"` : based on density-based clustering algorithm, mainly utilizing [HDBSCAN](https://hdbscan.readthedocs.io/en/latest/how_hdbscan_works.html) ligrary.
+>   - `"x-means"` : based on X-Means clustering algorithm
+>   - `"'K'-means"` : based on K-Means clustering algorithm, where users can freely change `'K'` value by substituting it with integer number.
+>     - e.g., `15-means`, `20-means`, etc. 
+> ***`snn_knn_matrix`*** : *`dict, (optional, default: None)`*
+> - If you want to inject precomputed snn and knn, use this parameter
+> - To inject the parameter, you should set `dist_strategy` as `"inject_snn"`
+> - The dictionary should hold:
+>	  - `"raw_snn"` : *`Array, shape=(n_samples, n_samples), dtype=float`*, the snn matrix of raw data
+>	  - `"raw_knn"` : *`Array, shape=(n_samples, n_samples), dtype=float`*, the knn matrix of raw data
+>	  - `"emb_snn"` : *`Array, shape=(n_samples, n_samples), dtype=float`*, the snn matrix of embedded data
+>	  - `"emb_knn"` : *`Array, shape=(n_samples, n_samples), dtype=float`*, the knn matrix of embedded data
+
+### Methods
+
+```python3
+SNC.fit(record_vis_info=False)
+```
+
+> Initializating Steadiness & Cohesiveness : Preprocessing (e.g., distance matrix computation) and preparation for computing Steadiness and Cohesiveness. 
+> 
+> ***`record_vis_info`*** : *`bool, (optional, default: False)`*
+> - If `True`, SNC object records the information needed to make [distortion visualization of Steadiness & Cohesiveness](#visualizing-steadiness-and-cohesiveness)
+> - method `vis_info()` becomes able to called when the parameter is set as `True`
+> - Recording the informations incurs extra overhead!!
+
+
+```python3
+SNC.steadiness()
+SNC.cohesiveness()
+```
+
+> Performs the main computation of Steadiness and Cohesiveness and return the result.
+> Note that this step generates large proportion of the computation.
+
+```python3
+SNC.vis_info(file_path=None, label=None, k=10)
+```
+
+> Able to be performed when `record_vis_info` parameter is set as `True` (Otherwise raises Error)
+>
+> ***`file_path`*** : *`string, (optional, default: None)`*
+> - if `file_path` is not given as arugment, returns visualization infos
+> - if `file_path` is given, visualization info is saved in the file with designated name (and path)
+> - if you only designate the directory (`file_path` ends with `/`), info is saved as `info.json` inside the directory
+> 
+> ***`label`*** : *`Array, (optional, default: None), shape=(n_samples), dtype=int`*
+> - 1D array which holds the label (class) information of dataset
+> - if `None`, all points are considered to have a identical label "0"
+> 
+> ***`k`*** : *`int, (optional, default: 10)`*
+> - the `k` value for constructing kNN graph used in visualization
+
+
+## Examples
+
+This section provides some examples to show how Steadiness and Cohesiveness respond to the projections with diverse qualities and characteristics. For more detailed experiments and evaluations, please refer to our [paper](http://hcil.snu.ac.kr/system/publications/pdfs/000/000/157/original/jeon_2021_tvcg.pdf?1626669574).
+
+### vs. Varying UMAP hyperparameters
+
+#### Increasing `n_neighbors`
+
+UMAP has two important hyperparameters: `n_neighbors` (nearest neighbors) and `min_dist`. Here, we test how Steadiness and Cohesiveness vary against UMAP embeddings with increasing `n_neighbors`. `n_neighbors` denotes the number of nearest neighbors used to formulate the graph representing the original structure of data. Low `n_neighbors` values make UMAP focus more on local structure, while high values work in the opposite. 
+
+The [Spheres](http://proceedings.mlr.press/v119/moor20a.html) and the [Mammoth](https://pair-code.github.io/understanding-umap/) dataset are used for the test. The Spheres dataset consists of eleven spheres living in a 101-dimensional space. The dataset represents ten spheres with each consisting of 250 points, which are enclosed by another larger sphere with 2,500 points. The Mammoth dataset consists of 5,000 points constituting the 3D structure of a mammoth skeleton. 
+
+The UMAP projections of Mammoth (upper row) Spheres (bottom row) dataset with increasing `n_neighbors` are as follows:
+
+![](https://user-images.githubusercontent.com/38465539/124187732-353f8800-daf9-11eb-9754-3c7ba19aea84.png) 
+
+Let's first examine the projections carefully. For the Mammoth dataset, projections with larger `n_neighbors` preserves the skeleton structure. For the Spheres dataset, you can see the points from the outer sphere (blue points) escapes from the cluster mainly formed by inner spheres when `n_neighbors` grow. Therefore, we can intuitively indicate that the projections with larger `n_neighbors` values better preserve the original inter-cluster structure for both datasets.
+
+Now it's time to conduct a test!! We applied Steadiness & Cohesiveness (with default hyperparameter setting) to the projections. Previous local metrics (Trustworthiness & Continuity, Mean Relative Rank Errors) with *k*=10 and global metrics (Stress, DTM) were also applied for the comparison. For global metrics, we used the values that are subtracted from 1, to assign lower values to low-quality projections.
+
+<p align="center">
+<img src="https://user-images.githubusercontent.com/38465539/124186611-8a7a9a00-daf7-11eb-8df8-9ef94560467c.png" alt="" data-canonical-src="https://user-images.githubusercontent.com/38465539/124186611-8a7a9a00-daf7-11eb-8df8-9ef94560467c.png" width="80%"/>
+</p>
+
+As a result, we can find that Steadiness well captured the increment of the projection quality occurred by the increasing `n_neighbors` values, both for Mammoth (left) and Spheres (right). 
+However, Cohesiveness increased only for the Mammoth dataset.
+Still, other metrics, except DTM, failed to capture the increment of projection quality.
+
+
+
+
+#### Increasing `min_dist`
+
+Then how about `min_dist`? This time, we generated projections of [Fashion-MNIST](https://github.com/zalandoresearch/fashion-mnist) dataset with increasing `min_dist`. 
+Alike `n_neighbors`, low `min_dist` values pack points together (focusing on local structure), and high values do the opposite. 
+The projections and their evaluation result is as follows.
+
+
+![](https://user-images.githubusercontent.com/38465539/124188004-a121f080-daf9-11eb-818e-cf4a96990e32.png)
+<p align="center">
+<img src="https://user-images.githubusercontent.com/38465539/124189744-2c03ea80-dafc-11eb-89fd-38305bcec254.png" alt="" data-canonical-src="https://user-images.githubusercontent.com/38465539/124189744-2c03ea80-dafc-11eb-89fd-38305bcec254.png" width="45%"/>
+</p>
+
+We previously noted that large `min_dist` values make projections focus more on the global structure. Thus, the decrement of Trustworthiness and MRRE [Missing] is quite natural, as they focus on small local structures around each point. The surprising thing here is that Cohesiveness increases as `min_dist` increases. This result indicates that classes of the Fashion-MNIST dataset are not well separated as represented in the projections with a low `min_dist` value. 
+According to our case study (refer to the [paper](http://hcil.snu.ac.kr/system/publications/pdfs/000/000/157/original/jeon_2021_tvcg.pdf?1626669574), it is common to perceive that projections with well-divided clusters better reflect the inter-cluster structure; this result shows that such a common perception could lead to a misinterpretation of inter-cluster structure. 
+
+
+
+
+### Capturing PCA quality alteration
+
+MDP metrics *must* capture the obvious quality degradation or increment. To test our metrics' ability to capture such alteration, we conducted two tests utilizing PCA. In the first experiment, we generated 2D PCA projections of [MNIST](https://en.wikipedia.org/wiki/MNIST_database) dataset by utilizing principal component pairs with decreasing ranks (from (1st, 2nd) to (21th, 22nd)). The projections with low-rank principal components will have a lower score, as they cannot well preserve the variance of the dataset. For the second experiment, we varied the number of principal components from 2 to 22. Obviously, the quality of projections should be increase when they can utilize more principal components (i.e., lie in higher dimension). 
+
+<p align="center">
+<img src="https://user-images.githubusercontent.com/38465539/124189753-2e664480-dafc-11eb-8b4b-67e3c585bdf1.png" alt="" data-canonical-src="https://user-images.githubusercontent.com/38465539/124189753-2e664480-dafc-11eb-8b4b-67e3c585bdf1.png" width="80%"/>
+</p>
+
+Unsurprisingly, all metrics, including Steadiness and Cohesiveness, well captured the quality alteration for both the first (left) and the second (right) experiment. 
+
+
+## Visualizing Steadiness and Cohesiveness
+
+
+![vis](https://user-images.githubusercontent.com/38465539/123515745-b0590680-d6d3-11eb-816d-e725fd5841ee.png)
+
+By visualizing the result of Steadiness and Cohesiveness through the reliability map, we get more insight into how inter-cluster structure is distorted in MDP. You only need to inject visualization info file generated by `vis_info` method.
+Please check [relability map repository](https://github.com/hj-n/snc-reliability-map) and follow the instructions to visualize Steadiness and Cohesiveness on your web browser.
+
+*The reliability map also supports interactions to show Missing Groups — please enjoy it!!*
+
+<p align="center">
+<img src="https://user-images.githubusercontent.com/38465539/123516175-c49e0300-d6d5-11eb-9a1c-2215b924ef79.gif" alt="" data-canonical-src="https://user-images.githubusercontent.com/38465539/123516175-c49e0300-d6d5-11eb-9a1c-2215b924ef79.gif" width="55%"/>
+</p>
+ 
+
+## References / Citation
+
+If you have used Steadiness & Cohesvieness for your project and wish to reference it, please cite our TVCG paper.
+
+> H. Jeon, H.-K. Ko, J. Jo, Y. Kim, and J. Seo, “Measuring and explaining the inter-cluster reliability of multidimensional projections,” *IEEE Transactions on Visualization and Computer Graphics (TVCG, Proc. VIS)*, 2021. to appear. 
+
+
+#### Bibtex
+
+```bib
+@article{jeon21tvcg,
+  author={Jeon, Hyeon and Ko, Hyung-Kwon and Jo, Jaemin and Kim, Youngtaek and Seo, Jinwook},
+  journal={IEEE Transactions on Visualization and Computer Graphics (TVCG, Proc. VIS)}, 
+  title={Measuring and Explaining the Inter-Cluster Reliability of Multidimensional Projections}, 
+  year={2021},
+  note={to appear.}
+}
+
+```
+
+
+## Contributors
+
+[Hyeon Jeon](https://github.com/hj-n), [Hyung-Kwon Ko](https://github.com/hyungkwonko), [Jaemin Jo](https://github.com/e-), [Youngtaek Kim](https://github.com/ytaek), and Jinwook Seo.
+
+This software is mainly developed / maintained by Human-computer Interaction Laboratory @ Seoul National University.
+
```

#### html2text {}

```diff
@@ -1,11 +1,13 @@
-Metadata-Version: 2.1 Name: snc Version: 0.1.0 Summary: Implementation of
+Metadata-Version: 2.1 Name: snc Version: 0.2.0 Summary: Implementation of
 Steadiness & Cohesiveness Home-page: https://github.com/hj-n/steadiness-
-cohesiveness Author: Hyeon Jeon Author-email: hj@hcil.snu.ac.kr License:
-UNKNOWN Description:
+cohesiveness Author: Hyeon Jeon Author-email: hj@hcil.snu.ac.kr Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Requires-Python: >=3.8.5
+Description-Content-Type: text/markdown License-File: LICENSE
 Quality Metrics for evaluating the inter-cluster reliability of Mutldimensional
                                  Projections
                           Docs Â·  Paper  Â· Contact
 ## Steadiness & Cohesiveness We cannot trust the embedding results (i.e., the
 results of multidimensional projections (MDP) such as [*t*-SNE](https://
 lvdmaaten.github.io/tsne/), [UMAP](https://github.com/lmcinnes/umap), or [PCA]
 (https://scikit-learn.org/stable/modules/generated/
@@ -31,92 +33,100 @@
 Steadiness measures the extent to which clusters in the projected space form
 clusters in the original space, and Cohesiveness measures the opposite. For
 more details, please refer to our [paper](http://hcil.snu.ac.kr/system/
 publications/pdfs/000/000/157/original/jeon_2021_tvcg.pdf?1626669574). ## Basic
 Usage If you have trouble using Steadiness & Cohesiveness in your project or
 research, feel free to contact us ([hj@hcil.snu.ac.kr](mailto:
 hj@hcil.snu.ac.kr)). We appreciate all requests about utilizing our metrics!!
-### Installation Steadiness and Cohesiveness are served with conda virtual
-environment. ```sh git clone https://github.com/hj-n/steadiness-cohesiveness
-snc conda env create -f snc/env/snc_virtual_env.yaml conda activate sncvirtual
-``` ### How to use Stediness & Cohesiveness ```python from snc import SNC ... #
-k value for computing Shared Nearest Neighbor-based dissimilarity parameter =
-{ "k": 100, "alpha": 0.1 } metrics = SNC( raw=raw_data, emb=emb_data,
-iteration=300, dist_parameter = parameter ) metrics.fit() print
-(metrics.steadiness(), metrics.cohesiveness()) ``` if you installed Steadiness
-& Cohesiveness outside your project directory: ```python import sys
-sys.path.append("/absolute/path/to/steadiness-cohesiveness") from snc import
-SNC ... ``` As there exists a number of parameters for Steadiness &
+### Installation Steadiness and Cohesiveness can be installed via pip ```sh pip
+install snc ``` ### How to use Stediness & Cohesiveness ```python from snc.snc
+import SNC ... parameter = { "k": 'sqrt', "alpha": 0.1 } metrics = SNC
+( raw=raw_data, emb=emb_data, iteration=300, dist_parameter = parameter )
+metrics.fit() print(metrics.steadiness(), metrics.cohesiveness()) ``` if you
+installed Steadiness & Cohesiveness outside your project directory: ```python
+import sys sys.path.append("/absolute/path/to/steadiness-cohesiveness") from
+snc import SNC ... ``` As there exists a number of parameters for Steadiness &
 Cohesiveness, we recommend you to use the default setting (which is described
 in our paper) by locating the original data into `raw` and projection data into
 `emb` as arguments. - **`raw`**: the original (raw) high-dimensional data which
 used to generate multidimensional projections. Should be a 2D array (or a 2D np
 array) with shape `(n_samples, n_dim)` where `n_samples` denotes the number of
 data points in dataset and `n_dim` is the original size of dimensionality
 (number of features). - **`emb`**: the projected (embedded) data of **`raw`**
 (i.e., MDP result). Should be a 2D array (or a 2D np array) with shape `
 (n_samples, n_reduced_dim)` where `n_reduced_dim` denotes the dimensionality of
 projection. Refer [API description](#api) for more details about hyperparameter
 setting. ## API ### Initialization ```python class SNC( raw, emb,
-iteration=200, walk_num_ratio=0.4, dist_strategy="snn", dist_paramter={},
-dist_function=None, cluster_strategy="dbscan" ) ``` > ***`raw`*** : *`Array,
-shape=(n_samples, n_dim), dtype=float or int`* > - The original (raw) high-
-dimensional data used to generate MDP result. > - `n_samples`: the number of
-data points in dataset / `n_dim`: is the original size of dimensionality > > >
-***`emb`*** : *`Array, shape=(n_samples, n_reduced_dim), dtype=float or int`* >
-- The projected (embedded) data of **`raw`**. > - `n_reduced_dim`:
-dimensionality of the projection > > ***`iteration`*** : *`int, (optional,
-default: 200)`* > - The number of partial distortion computation (extracting =>
-evaluating maintainence in the opposite side). > - Higher `iteration` generates
-the more deterministic / reliable result, but computation time increases
-linearly to `iteration`. > - We recommend 200 iterations as a minimum. > >
-***`walk_num_ratio`*** : *`float, (optional, default: 0.4)`* > - The amount of
-traverse held to extract a cluster. > - For a data with `n_samples` samples,
-the total traverse number to extract a cluster is `n_samples * walk_num_ratio`.
-> - The size of extracted cluster grows as `walk_num_ratio` increases, but does
-not effect the result significantly. > > ***`dist_strategy`*** : *`string,
-(optional, default: "snn")`* > - The selection of the way to compute distance.
-> - We currently support: > - `"snn"` : utilizes Shared Nearest Neighbor based
-on dissimilarity > - `"euclidean"` > - `"predefined"` : allows user-defined
-distance function > - We highly recommend to use default distance strategy
-"snn". > - If you set `dist_strategy` as "predefined", you should also
-explicitly pass the way to compute distance as `dist_function` parameter. THe
-distance for cluster automatically computed as average linkage. > >
-***`dist_parameter`*** : *`dict, (optional, default: { "alpha": 0.1, "k": 100
-})`* > - Parameters for distance computations > - if `dist_strategy == "snn`,
-`dist_parameter` dictionary should hold: > - `"alpha"` : *`float, (optional,
-default: 0.1)`* > - The hyperparameter which panalizes low similarity between
-data points / clusters. > - A low `"alpha"` converts smaller similarities to
-higher dissimilarities (distances). > - `"k"` : *`int, (optional, default:
-100)`* > - The number of nearest neighbors for `k`-Nearest Neighbror graph
-which becomes a basis to compute SNN similarity. > - if `dist_parameter ==
-"euclidean"`, `dist_parameter` does nothing. > - if `dist_parameter ==
-"predefined"`, you can freely utilize `dist_parameter` in `dist_function`. > -
-Note that unlike `"snn"` and `"euclidean"`, the computation of "predefined" is
-not parallelized, thus requries much time to be computed > >
-***`dist_function`*** : *`function, (optional, default: None)`* > - If you set
-`dist_strategy` as `"predefined"`, you should pass the function to calculate
-distance as parameter (otherwise the class raises error). > - The function must
-get three parameters as arguments: two points `a`,`b`, their length `n_dim`,
-and `dist_parameter` which is given by user. > - `a` and `b` will be 1D numpy
-array with size `n_dim` > - `n_dim` will be an integer number > - return value
-should be a single float value which denotes the distance between `a` and `b`.
-> > ***`cluster_strategy`*** : *`string, (optional, default: "dbscan")`* > -
-Remind: Steadiness and Cohesiveness measures inter-cluster reliability by
-checking the maintenance of clusters from one space in the opposite space
-(Refer to [Why Steadiness and Cohesiveness](#why-steadiness-and-cohesiveness)).
-> - This is done by again "clustering" the cluster in the opposite side and
-measuring how much the cluster is splitted. `cluster_strategy` is a
-hyperparameter to determine the way to conduct such "clustering > - We
-currently supports: > - `"dbscan"` : based on density-based clustering
-algorithm, mainly utilizing [HDBSCAN](https://hdbscan.readthedocs.io/en/latest/
-how_hdbscan_works.html) ligrary. > - `"x-means"` : based on X-Means clustering
-algorithm > - `"'K'-means"` : based on K-Means clustering algorithm, where
-users can freely change `'K'` value by substituting it with integer number. > -
-e.g., `15-means`, `20-means`, etc. ### Methods ```python3 SNC.fit
+iteration=150, walk_num_ratio=0.3, dist_strategy="snn", dist_paramter={},
+dist_function=None, cluster_strategy="dbscan", snn_knn_matrix=None ) ``` >
+***`raw`*** : *`Array, shape=(n_samples, n_dim), dtype=float or int`* > - The
+original (raw) high-dimensional data used to generate MDP result. > -
+`n_samples`: the number of data points in dataset / `n_dim`: is the original
+size of dimensionality > > > ***`emb`*** : *`Array, shape=(n_samples,
+n_reduced_dim), dtype=float or int`* > - The projected (embedded) data of
+**`raw`**. > - `n_reduced_dim`: dimensionality of the projection > >
+***`iteration`*** : *`int, (optional, default: 150)`* > - The number of partial
+distortion computation (extracting => evaluating maintainence in the opposite
+side). > - Higher `iteration` generates the more deterministic / reliable
+result, but computation time increases linearly to `iteration`. > - We
+recommend 150 iterations as a minimum. > > ***`walk_num_ratio`*** : *`float,
+(optional, default: 0.3)`* > - The amount of traverse held to extract a
+cluster. > - For a data with `n_samples` samples, the total traverse number to
+extract a cluster is `n_samples * walk_num_ratio`. > - The size of extracted
+cluster grows as `walk_num_ratio` increases, but does not effect the result
+significantly. > > ***`dist_strategy`*** : *`string, (optional, default:
+"snn")`* > - The selection of the way to compute distance. > - We currently
+support: > - `"snn"` : utilizes Shared Nearest Neighbor based on dissimilarity
+> - `"euclidean"` > - `"predefined"` : allows user-defined distance function >
+- `"inject_snn"` : inject knn and snn info > - We highly recommend to use
+default distance strategy "snn". > - If you set `dist_strategy` as
+"predefined", you should also explicitly pass the way to compute distance as
+`dist_function` parameter. THe distance for cluster automatically computed as
+average linkage. > > ***`dist_parameter`*** : *`dict, (optional, default:
+{ "alpha": 0.1, "k": 'sqrt' })`* > - Parameters for distance computations > -
+if `dist_strategy == "snn`, `dist_parameter` dictionary should hold: > -
+`"alpha"` : *`float, (optional, default: 0.1)`* > - The hyperparameter which
+panalizes low similarity between data points / clusters. > - A low `"alpha"`
+converts smaller similarities to higher dissimilarities (distances). > - `"k"`
+: *`int or string, (optional, default: 'sqrt')`* > - The number of nearest
+neighbors for `k`-Nearest Neighbror graph which becomes a basis to compute SNN
+similarity. > - If `k == 'sqrt'`, `k` is set as the square root of the length
+of data > - if `dist_parameter == "euclidean"`, `dist_parameter` does nothing.
+> - if `dist_parameter == "predefined"`, you can freely utilize
+`dist_parameter` in `dist_function`. > - Note that unlike `"snn"` and
+`"euclidean"`, the computation of "predefined" is not parallelized, thus
+requries much time to be computed > > ***`dist_function`*** : *`function,
+(optional, default: None)`* > - If you set `dist_strategy` as `"predefined"`,
+you should pass the function to calculate distance as parameter (otherwise the
+class raises error). > - The function must get three parameters as arguments:
+two points `a`,`b`, their length `n_dim`, and `dist_parameter` which is given
+by user. > - `a` and `b` will be 1D numpy array with size `n_dim` > - `n_dim`
+will be an integer number > - return value should be a single float value which
+denotes the distance between `a` and `b`. > > ***`cluster_strategy`*** :
+*`string, (optional, default: "dbscan")`* > - Remind: Steadiness and
+Cohesiveness measures inter-cluster reliability by checking the maintenance of
+clusters from one space in the opposite space (Refer to [Why Steadiness and
+Cohesiveness](#why-steadiness-and-cohesiveness)). > - This is done by again
+"clustering" the cluster in the opposite side and measuring how much the
+cluster is splitted. `cluster_strategy` is a hyperparameter to determine the
+way to conduct such "clustering > - We currently supports: > - `"dbscan"` :
+based on density-based clustering algorithm, mainly utilizing [HDBSCAN](https:/
+/hdbscan.readthedocs.io/en/latest/how_hdbscan_works.html) ligrary. > - `"x-
+means"` : based on X-Means clustering algorithm > - `"'K'-means"` : based on K-
+Means clustering algorithm, where users can freely change `'K'` value by
+substituting it with integer number. > - e.g., `15-means`, `20-means`, etc. >
+***`snn_knn_matrix`*** : *`dict, (optional, default: None)`* > - If you want to
+inject precomputed snn and knn, use this parameter > - To inject the parameter,
+you should set `dist_strategy` as `"inject_snn"` > - The dictionary should
+hold: > - `"raw_snn"` : *`Array, shape=(n_samples, n_samples), dtype=float`*,
+the snn matrix of raw data > - `"raw_knn"` : *`Array, shape=(n_samples,
+n_samples), dtype=float`*, the knn matrix of raw data > - `"emb_snn"` :
+*`Array, shape=(n_samples, n_samples), dtype=float`*, the snn matrix of
+embedded data > - `"emb_knn"` : *`Array, shape=(n_samples, n_samples),
+dtype=float`*, the knn matrix of embedded data ### Methods ```python3 SNC.fit
 (record_vis_info=False) ``` > Initializating Steadiness & Cohesiveness :
 Preprocessing (e.g., distance matrix computation) and preparation for computing
 Steadiness and Cohesiveness. > > ***`record_vis_info`*** : *`bool, (optional,
 default: False)`* > - If `True`, SNC object records the information needed to
 make [distortion visualization of Steadiness & Cohesiveness](#visualizing-
 steadiness-and-cohesiveness) > - method `vis_info()` becomes able to called
 when the parameter is set as `True` > - Recording the informations incurs extra
@@ -219,11 +229,8 @@
 Jo, Jaemin and Kim, Youngtaek and Seo, Jinwook}, journal={IEEE Transactions on
 Visualization and Computer Graphics (TVCG, Proc. VIS)}, title={Measuring and
 Explaining the Inter-Cluster Reliability of Multidimensional Projections},
 year={2021}, note={to appear.} } ``` ## Contributors [Hyeon Jeon](https://
 github.com/hj-n), [Hyung-Kwon Ko](https://github.com/hyungkwonko), [Jaemin Jo]
 (https://github.com/e-), [Youngtaek Kim](https://github.com/ytaek), and Jinwook
 Seo. This software is mainly developed / maintained by Human-computer
-Interaction Laboratory @ Seoul National University. Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8.5 Description-Content-Type: text/markdown
+Interaction Laboratory @ Seoul National University.
```

