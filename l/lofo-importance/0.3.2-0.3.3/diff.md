# Comparing `tmp/lofo-importance-0.3.2.tar.gz` & `tmp/lofo-importance-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lofo-importance-0.3.2.tar", last modified: Wed Apr 27 12:54:41 2022, max compression
+gzip compressed data, was "lofo-importance-0.3.3.tar", last modified: Sat Apr 15 05:42:58 2023, max compression
```

## Comparing `lofo-importance-0.3.2.tar` & `lofo-importance-0.3.3.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxrwxr-x   0 aerdem    (1000) aerdem    (1000)        0 2022-04-27 12:54:41.956785 lofo-importance-0.3.2/
--rw-rw-r--   0 aerdem    (1000) aerdem    (1000)     6987 2022-04-27 12:54:41.956785 lofo-importance-0.3.2/PKG-INFO
--rw-rw-r--   0 aerdem    (1000) aerdem    (1000)     5758 2022-04-27 12:07:22.000000 lofo-importance-0.3.2/README.md
-drwxrwxr-x   0 aerdem    (1000) aerdem    (1000)        0 2022-04-27 12:54:41.956785 lofo-importance-0.3.2/lofo/
--rw-rw-r--   0 aerdem    (1000) aerdem    (1000)      157 2022-04-27 12:07:22.000000 lofo-importance-0.3.2/lofo/__init__.py
--rw-rw-r--   0 aerdem    (1000) aerdem    (1000)     5541 2022-04-27 12:09:36.000000 lofo-importance-0.3.2/lofo/dataset.py
--rw-rw-r--   0 aerdem    (1000) aerdem    (1000)     4572 2022-04-27 12:07:22.000000 lofo-importance-0.3.2/lofo/flofo_importance.py
--rw-rw-r--   0 aerdem    (1000) aerdem    (1000)      694 2022-04-27 12:07:22.000000 lofo-importance-0.3.2/lofo/infer_defaults.py
--rw-rw-r--   0 aerdem    (1000) aerdem    (1000)     3376 2022-04-27 12:07:22.000000 lofo-importance-0.3.2/lofo/lofo_importance.py
--rw-rw-r--   0 aerdem    (1000) aerdem    (1000)     1200 2022-04-27 12:07:22.000000 lofo-importance-0.3.2/lofo/plotting.py
--rw-rw-r--   0 aerdem    (1000) aerdem    (1000)      984 2022-04-27 12:07:22.000000 lofo-importance-0.3.2/lofo/utils.py
-drwxrwxr-x   0 aerdem    (1000) aerdem    (1000)        0 2022-04-27 12:54:41.956785 lofo-importance-0.3.2/lofo_importance.egg-info/
--rw-rw-r--   0 aerdem    (1000) aerdem    (1000)     6987 2022-04-27 12:54:41.000000 lofo-importance-0.3.2/lofo_importance.egg-info/PKG-INFO
--rw-rw-r--   0 aerdem    (1000) aerdem    (1000)      348 2022-04-27 12:54:41.000000 lofo-importance-0.3.2/lofo_importance.egg-info/SOURCES.txt
--rw-rw-r--   0 aerdem    (1000) aerdem    (1000)        1 2022-04-27 12:54:41.000000 lofo-importance-0.3.2/lofo_importance.egg-info/dependency_links.txt
--rw-rw-r--   0 aerdem    (1000) aerdem    (1000)       71 2022-04-27 12:54:41.000000 lofo-importance-0.3.2/lofo_importance.egg-info/requires.txt
--rw-rw-r--   0 aerdem    (1000) aerdem    (1000)        5 2022-04-27 12:54:41.000000 lofo-importance-0.3.2/lofo_importance.egg-info/top_level.txt
--rw-rw-r--   0 aerdem    (1000) aerdem    (1000)       38 2022-04-27 12:54:41.956785 lofo-importance-0.3.2/setup.cfg
--rw-rw-r--   0 aerdem    (1000) aerdem    (1000)      831 2022-04-27 12:09:08.000000 lofo-importance-0.3.2/setup.py
+drwxrwxr-x   0 aerdem    (1000) aerdem    (1000)        0 2023-04-15 05:42:58.089758 lofo-importance-0.3.3/
+-rw-rw-r--   0 aerdem    (1000) aerdem    (1000)     1068 2022-04-27 12:07:22.000000 lofo-importance-0.3.3/LICENSE
+-rw-rw-r--   0 aerdem    (1000) aerdem    (1000)       48 2023-04-15 05:41:05.000000 lofo-importance-0.3.3/MANIFEST.in
+-rw-rw-r--   0 aerdem    (1000) aerdem    (1000)     7162 2023-04-15 05:42:58.089758 lofo-importance-0.3.3/PKG-INFO
+-rw-rw-r--   0 aerdem    (1000) aerdem    (1000)     5885 2023-04-15 05:41:05.000000 lofo-importance-0.3.3/README.md
+drwxrwxr-x   0 aerdem    (1000) aerdem    (1000)        0 2023-04-15 05:42:58.089758 lofo-importance-0.3.3/lofo/
+-rw-rw-r--   0 aerdem    (1000) aerdem    (1000)      157 2022-04-27 12:07:22.000000 lofo-importance-0.3.3/lofo/__init__.py
+-rw-rw-r--   0 aerdem    (1000) aerdem    (1000)     5541 2023-04-15 05:41:05.000000 lofo-importance-0.3.3/lofo/dataset.py
+-rw-rw-r--   0 aerdem    (1000) aerdem    (1000)     4572 2022-04-27 12:07:22.000000 lofo-importance-0.3.3/lofo/flofo_importance.py
+-rw-rw-r--   0 aerdem    (1000) aerdem    (1000)      694 2022-04-27 12:07:22.000000 lofo-importance-0.3.3/lofo/infer_defaults.py
+-rw-rw-r--   0 aerdem    (1000) aerdem    (1000)     3376 2022-04-27 12:07:22.000000 lofo-importance-0.3.3/lofo/lofo_importance.py
+-rw-rw-r--   0 aerdem    (1000) aerdem    (1000)     1200 2022-04-27 12:07:22.000000 lofo-importance-0.3.3/lofo/plotting.py
+-rw-rw-r--   0 aerdem    (1000) aerdem    (1000)      984 2022-04-27 12:07:22.000000 lofo-importance-0.3.3/lofo/utils.py
+drwxrwxr-x   0 aerdem    (1000) aerdem    (1000)        0 2023-04-15 05:42:58.089758 lofo-importance-0.3.3/lofo_importance.egg-info/
+-rw-rw-r--   0 aerdem    (1000) aerdem    (1000)     7162 2023-04-15 05:42:58.000000 lofo-importance-0.3.3/lofo_importance.egg-info/PKG-INFO
+-rw-rw-r--   0 aerdem    (1000) aerdem    (1000)      385 2023-04-15 05:42:58.000000 lofo-importance-0.3.3/lofo_importance.egg-info/SOURCES.txt
+-rw-rw-r--   0 aerdem    (1000) aerdem    (1000)        1 2023-04-15 05:42:58.000000 lofo-importance-0.3.3/lofo_importance.egg-info/dependency_links.txt
+-rw-rw-r--   0 aerdem    (1000) aerdem    (1000)       71 2023-04-15 05:42:58.000000 lofo-importance-0.3.3/lofo_importance.egg-info/requires.txt
+-rw-rw-r--   0 aerdem    (1000) aerdem    (1000)        5 2023-04-15 05:42:58.000000 lofo-importance-0.3.3/lofo_importance.egg-info/top_level.txt
+-rw-rw-r--   0 aerdem    (1000) aerdem    (1000)       70 2023-04-15 05:41:05.000000 lofo-importance-0.3.3/requirements.txt
+-rw-rw-r--   0 aerdem    (1000) aerdem    (1000)       38 2023-04-15 05:42:58.089758 lofo-importance-0.3.3/setup.cfg
+-rw-rw-r--   0 aerdem    (1000) aerdem    (1000)      831 2023-04-15 05:41:55.000000 lofo-importance-0.3.3/setup.py
```

### Comparing `lofo-importance-0.3.2/PKG-INFO` & `lofo-importance-0.3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,103 +1,109 @@
 Metadata-Version: 2.1
 Name: lofo-importance
-Version: 0.3.2
+Version: 0.3.3
 Summary: Leave One Feature Out Importance
 Home-page: https://github.com/aerdem4/lofo-importance
 Author: Ahmet Erdem
 Author-email: ahmeterd4@gmail.com
 License: UNKNOWN
 Description: ![alt text](docs/lofo_logo.png?raw=true "Title")
         
         LOFO (Leave One Feature Out) Importance calculates the importances of a set of features based on a metric of choice, for a model of choice, by iteratively removing each feature from the set, and evaluating the performance of the model, with a validation scheme of choice, based on the chosen metric.
         
         LOFO first evaluates the performance of the model with all the input features included, then iteratively removes one feature at a time, retrains the model, and evaluates its performance on a validation set. The mean and standard deviation (across the folds) of the importance of each feature is then reported.
         
         If a model is not passed as an argument to LOFO Importance, it will run LightGBM as a default model.
         
         ## Install
+        
         LOFO Importance can be installed using
+        
         ```
         pip install lofo-importance
         ```
         
-        ## Advantages of LOFO Importance 
+        ## Advantages of LOFO Importance
+        
         LOFO has several advantages compared to other importance types:
+        
         * It does not favor granular features
         * It generalises well to unseen test sets
         * It is model agnostic
         * It gives negative importance to features that hurt performance upon inclusion
         * It can group the features. Especially useful for high dimensional features like TFIDF or OHE features.
         * It can automatically group highly correlated features to avoid underestimating their importance.
         
         ## Example on Kaggle's Microsoft Malware Prediction Competition
+        
         In this Kaggle competition, Microsoft provides a malware dataset to predict whether or not a machine will soon be hit with malware. One of the features, Centos_OSVersion is very predictive on the training set, since some OS versions are probably more prone to bugs and failures than others. However, upon splitting the data out of time, we obtain validation sets with OS versions that have not occurred in the training set. Therefore, the model will not have learned the relationship between the target and this seasonal feature. By evaluating this feature's importance using other importance types, Centos_OSVersion seems to have high importance, because its importance was evaluated using only the training set. However, LOFO Importance depends on a validation scheme, so it will not only give this feature low importance, but even negative importance.
         
-        ```
-        import pandas as pd
+        ```python
+         import pandas as pd
         from sklearn.model_selection import KFold
         from lofo import LOFOImportance, Dataset, plot_importance
         %matplotlib inline
         
         # import data
         train_df = pd.read_csv("../input/train.csv", dtype=dtypes)
         
         # extract a sample of the data
         sample_df = train_df.sample(frac=0.01, random_state=0)
-        sample_df.sort_values("AvSigVersion", inplace=True)
+        sample_df.sort_values("AvSigVersion", inplace=True) # Sort by time for time split validation
         
         # define the validation scheme
-        cv = KFold(n_splits=4, shuffle=False, random_state=0)
+        cv = KFold(n_splits=4, shuffle=False, random_state=None) # Don't shuffle to keep the time split split validation
         
         # define the binary target and the features
-        dataset = Dataset(df=sample_df, target="HasDetections", features=[col for col in train_df.columns if col != target])
+        dataset = Dataset(df=sample_df, target="HasDetections", features=[col for col in train_df.columns if col != "HasDetections"])
         
         # define the validation scheme and scorer. The default model is LightGBM
         lofo_imp = LOFOImportance(dataset, cv=cv, scoring="roc_auc")
         
         # get the mean and standard deviation of the importances in pandas format
         importance_df = lofo_imp.get_importance()
         
         # plot the means and standard deviations of the importances
         plot_importance(importance_df, figsize=(12, 20))
         ```
-        ![alt text](docs/plot_importance.png?raw=true "Title")
         
+        ![alt text](docs/plot_importance.png?raw=true "Title")
         
         ## Another Example: Kaggle's TReNDS Competition
+        
         In this Kaggle competition, pariticipants are asked to predict some cognitive properties of patients.
         Independent component features (IC) from sMRI and very high dimensional correlation features (FNC) from 3D fMRIs are provided.
         LOFO can group the fMRI correlation features into one.
         
-        ```
+        ```python
         def get_lofo_importance(target):
             cv = KFold(n_splits=7, shuffle=True, random_state=17)
         
             dataset = Dataset(df=df[df[target].notnull()], target=target, features=loading_features,
                               feature_groups={"fnc": df[df[target].notnull()][fnc_features].values
                               })
         
             model = Ridge(alpha=0.01)
             lofo_imp = LOFOImportance(dataset, cv=cv, scoring="neg_mean_absolute_error", model=model)
         
             return lofo_imp.get_importance()
         
         plot_importance(get_lofo_importance(target="domain1_var1"), figsize=(8, 8), kind="box")
         ```
+        
         ![alt text](docs/plot_importance_box.png?raw=true "Title")
         
         ## Flofo Importance
         
         If running the LOFO Importance package is too time-costly for you, you can use Fast LOFO. Fast LOFO, or FLOFO takes, as inputs, an already trained model and a validation set, and does a pseudo-random permutation on the values of each feature, one by one, then uses the trained model to make predictions on the validation set. The mean of the FLOFO importance is then the difference in the performance of the model on the validation set over several randomised permutations.
         The difference between FLOFO importance and permutation importance is that the permutations on a feature's values are done within groups, where groups are obtained by grouping the validation set by k=2 features. These k features are chosen at random n=10 times, and the mean and standard deviation of the FLOFO importance are calculated based on these n runs.
         The reason this grouping makes the measure of importance better is that permuting a feature's value is no longer completely random. In fact, the permutations are done within groups of similar samples, so the permutations are equivalent to noising the samples. This ensures that:
+        
         * The permuted feature values are very unlikely to be replaced by unrealistic values.
         * A feature that is predictable by features among the chosen n*k features will be replaced by very similar values during permutation. Therefore, it will only slightly affect the model performance (and will yield a small FLOFO importance). This solves the correlated feature overestimation problem.
         
-        
-        
 Keywords: feature importance selection explainable data-science machine-learning
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `lofo-importance-0.3.2/README.md` & `lofo-importance-0.3.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,86 +3,92 @@
 LOFO (Leave One Feature Out) Importance calculates the importances of a set of features based on a metric of choice, for a model of choice, by iteratively removing each feature from the set, and evaluating the performance of the model, with a validation scheme of choice, based on the chosen metric.
 
 LOFO first evaluates the performance of the model with all the input features included, then iteratively removes one feature at a time, retrains the model, and evaluates its performance on a validation set. The mean and standard deviation (across the folds) of the importance of each feature is then reported.
 
 If a model is not passed as an argument to LOFO Importance, it will run LightGBM as a default model.
 
 ## Install
+
 LOFO Importance can be installed using
+
 ```
 pip install lofo-importance
 ```
 
-## Advantages of LOFO Importance 
+## Advantages of LOFO Importance
+
 LOFO has several advantages compared to other importance types:
+
 * It does not favor granular features
 * It generalises well to unseen test sets
 * It is model agnostic
 * It gives negative importance to features that hurt performance upon inclusion
 * It can group the features. Especially useful for high dimensional features like TFIDF or OHE features.
 * It can automatically group highly correlated features to avoid underestimating their importance.
 
 ## Example on Kaggle's Microsoft Malware Prediction Competition
+
 In this Kaggle competition, Microsoft provides a malware dataset to predict whether or not a machine will soon be hit with malware. One of the features, Centos_OSVersion is very predictive on the training set, since some OS versions are probably more prone to bugs and failures than others. However, upon splitting the data out of time, we obtain validation sets with OS versions that have not occurred in the training set. Therefore, the model will not have learned the relationship between the target and this seasonal feature. By evaluating this feature's importance using other importance types, Centos_OSVersion seems to have high importance, because its importance was evaluated using only the training set. However, LOFO Importance depends on a validation scheme, so it will not only give this feature low importance, but even negative importance.
 
-```
-import pandas as pd
+```python
+ import pandas as pd
 from sklearn.model_selection import KFold
 from lofo import LOFOImportance, Dataset, plot_importance
 %matplotlib inline
 
 # import data
 train_df = pd.read_csv("../input/train.csv", dtype=dtypes)
 
 # extract a sample of the data
 sample_df = train_df.sample(frac=0.01, random_state=0)
-sample_df.sort_values("AvSigVersion", inplace=True)
+sample_df.sort_values("AvSigVersion", inplace=True) # Sort by time for time split validation
 
 # define the validation scheme
-cv = KFold(n_splits=4, shuffle=False, random_state=0)
+cv = KFold(n_splits=4, shuffle=False, random_state=None) # Don't shuffle to keep the time split split validation
 
 # define the binary target and the features
-dataset = Dataset(df=sample_df, target="HasDetections", features=[col for col in train_df.columns if col != target])
+dataset = Dataset(df=sample_df, target="HasDetections", features=[col for col in train_df.columns if col != "HasDetections"])
 
 # define the validation scheme and scorer. The default model is LightGBM
 lofo_imp = LOFOImportance(dataset, cv=cv, scoring="roc_auc")
 
 # get the mean and standard deviation of the importances in pandas format
 importance_df = lofo_imp.get_importance()
 
 # plot the means and standard deviations of the importances
 plot_importance(importance_df, figsize=(12, 20))
 ```
-![alt text](docs/plot_importance.png?raw=true "Title")
 
+![alt text](docs/plot_importance.png?raw=true "Title")
 
 ## Another Example: Kaggle's TReNDS Competition
+
 In this Kaggle competition, pariticipants are asked to predict some cognitive properties of patients.
 Independent component features (IC) from sMRI and very high dimensional correlation features (FNC) from 3D fMRIs are provided.
 LOFO can group the fMRI correlation features into one.
 
-```
+```python
 def get_lofo_importance(target):
     cv = KFold(n_splits=7, shuffle=True, random_state=17)
 
     dataset = Dataset(df=df[df[target].notnull()], target=target, features=loading_features,
                       feature_groups={"fnc": df[df[target].notnull()][fnc_features].values
                       })
 
     model = Ridge(alpha=0.01)
     lofo_imp = LOFOImportance(dataset, cv=cv, scoring="neg_mean_absolute_error", model=model)
 
     return lofo_imp.get_importance()
 
 plot_importance(get_lofo_importance(target="domain1_var1"), figsize=(8, 8), kind="box")
 ```
+
 ![alt text](docs/plot_importance_box.png?raw=true "Title")
 
 ## Flofo Importance
 
 If running the LOFO Importance package is too time-costly for you, you can use Fast LOFO. Fast LOFO, or FLOFO takes, as inputs, an already trained model and a validation set, and does a pseudo-random permutation on the values of each feature, one by one, then uses the trained model to make predictions on the validation set. The mean of the FLOFO importance is then the difference in the performance of the model on the validation set over several randomised permutations.
 The difference between FLOFO importance and permutation importance is that the permutations on a feature's values are done within groups, where groups are obtained by grouping the validation set by k=2 features. These k features are chosen at random n=10 times, and the mean and standard deviation of the FLOFO importance are calculated based on these n runs.
 The reason this grouping makes the measure of importance better is that permuting a feature's value is no longer completely random. In fact, the permutations are done within groups of similar samples, so the permutations are equivalent to noising the samples. This ensures that:
+
 * The permuted feature values are very unlikely to be replaced by unrealistic values.
 * A feature that is predictable by features among the chosen n*k features will be replaced by very similar values during permutation. Therefore, it will only slightly affect the model performance (and will yield a small FLOFO importance). This solves the correlated feature overestimation problem.
-
-
```

### Comparing `lofo-importance-0.3.2/lofo/dataset.py` & `lofo-importance-0.3.3/lofo/dataset.py`

 * *Files identical despite different names*

### Comparing `lofo-importance-0.3.2/lofo/flofo_importance.py` & `lofo-importance-0.3.3/lofo/flofo_importance.py`

 * *Files identical despite different names*

### Comparing `lofo-importance-0.3.2/lofo/infer_defaults.py` & `lofo-importance-0.3.3/lofo/infer_defaults.py`

 * *Files identical despite different names*

### Comparing `lofo-importance-0.3.2/lofo/lofo_importance.py` & `lofo-importance-0.3.3/lofo/lofo_importance.py`

 * *Files identical despite different names*

### Comparing `lofo-importance-0.3.2/lofo/plotting.py` & `lofo-importance-0.3.3/lofo/plotting.py`

 * *Files identical despite different names*

### Comparing `lofo-importance-0.3.2/lofo/utils.py` & `lofo-importance-0.3.3/lofo/utils.py`

 * *Files identical despite different names*

### Comparing `lofo-importance-0.3.2/lofo_importance.egg-info/PKG-INFO` & `lofo-importance-0.3.3/lofo_importance.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,103 +1,109 @@
 Metadata-Version: 2.1
 Name: lofo-importance
-Version: 0.3.2
+Version: 0.3.3
 Summary: Leave One Feature Out Importance
 Home-page: https://github.com/aerdem4/lofo-importance
 Author: Ahmet Erdem
 Author-email: ahmeterd4@gmail.com
 License: UNKNOWN
 Description: ![alt text](docs/lofo_logo.png?raw=true "Title")
         
         LOFO (Leave One Feature Out) Importance calculates the importances of a set of features based on a metric of choice, for a model of choice, by iteratively removing each feature from the set, and evaluating the performance of the model, with a validation scheme of choice, based on the chosen metric.
         
         LOFO first evaluates the performance of the model with all the input features included, then iteratively removes one feature at a time, retrains the model, and evaluates its performance on a validation set. The mean and standard deviation (across the folds) of the importance of each feature is then reported.
         
         If a model is not passed as an argument to LOFO Importance, it will run LightGBM as a default model.
         
         ## Install
+        
         LOFO Importance can be installed using
+        
         ```
         pip install lofo-importance
         ```
         
-        ## Advantages of LOFO Importance 
+        ## Advantages of LOFO Importance
+        
         LOFO has several advantages compared to other importance types:
+        
         * It does not favor granular features
         * It generalises well to unseen test sets
         * It is model agnostic
         * It gives negative importance to features that hurt performance upon inclusion
         * It can group the features. Especially useful for high dimensional features like TFIDF or OHE features.
         * It can automatically group highly correlated features to avoid underestimating their importance.
         
         ## Example on Kaggle's Microsoft Malware Prediction Competition
+        
         In this Kaggle competition, Microsoft provides a malware dataset to predict whether or not a machine will soon be hit with malware. One of the features, Centos_OSVersion is very predictive on the training set, since some OS versions are probably more prone to bugs and failures than others. However, upon splitting the data out of time, we obtain validation sets with OS versions that have not occurred in the training set. Therefore, the model will not have learned the relationship between the target and this seasonal feature. By evaluating this feature's importance using other importance types, Centos_OSVersion seems to have high importance, because its importance was evaluated using only the training set. However, LOFO Importance depends on a validation scheme, so it will not only give this feature low importance, but even negative importance.
         
-        ```
-        import pandas as pd
+        ```python
+         import pandas as pd
         from sklearn.model_selection import KFold
         from lofo import LOFOImportance, Dataset, plot_importance
         %matplotlib inline
         
         # import data
         train_df = pd.read_csv("../input/train.csv", dtype=dtypes)
         
         # extract a sample of the data
         sample_df = train_df.sample(frac=0.01, random_state=0)
-        sample_df.sort_values("AvSigVersion", inplace=True)
+        sample_df.sort_values("AvSigVersion", inplace=True) # Sort by time for time split validation
         
         # define the validation scheme
-        cv = KFold(n_splits=4, shuffle=False, random_state=0)
+        cv = KFold(n_splits=4, shuffle=False, random_state=None) # Don't shuffle to keep the time split split validation
         
         # define the binary target and the features
-        dataset = Dataset(df=sample_df, target="HasDetections", features=[col for col in train_df.columns if col != target])
+        dataset = Dataset(df=sample_df, target="HasDetections", features=[col for col in train_df.columns if col != "HasDetections"])
         
         # define the validation scheme and scorer. The default model is LightGBM
         lofo_imp = LOFOImportance(dataset, cv=cv, scoring="roc_auc")
         
         # get the mean and standard deviation of the importances in pandas format
         importance_df = lofo_imp.get_importance()
         
         # plot the means and standard deviations of the importances
         plot_importance(importance_df, figsize=(12, 20))
         ```
-        ![alt text](docs/plot_importance.png?raw=true "Title")
         
+        ![alt text](docs/plot_importance.png?raw=true "Title")
         
         ## Another Example: Kaggle's TReNDS Competition
+        
         In this Kaggle competition, pariticipants are asked to predict some cognitive properties of patients.
         Independent component features (IC) from sMRI and very high dimensional correlation features (FNC) from 3D fMRIs are provided.
         LOFO can group the fMRI correlation features into one.
         
-        ```
+        ```python
         def get_lofo_importance(target):
             cv = KFold(n_splits=7, shuffle=True, random_state=17)
         
             dataset = Dataset(df=df[df[target].notnull()], target=target, features=loading_features,
                               feature_groups={"fnc": df[df[target].notnull()][fnc_features].values
                               })
         
             model = Ridge(alpha=0.01)
             lofo_imp = LOFOImportance(dataset, cv=cv, scoring="neg_mean_absolute_error", model=model)
         
             return lofo_imp.get_importance()
         
         plot_importance(get_lofo_importance(target="domain1_var1"), figsize=(8, 8), kind="box")
         ```
+        
         ![alt text](docs/plot_importance_box.png?raw=true "Title")
         
         ## Flofo Importance
         
         If running the LOFO Importance package is too time-costly for you, you can use Fast LOFO. Fast LOFO, or FLOFO takes, as inputs, an already trained model and a validation set, and does a pseudo-random permutation on the values of each feature, one by one, then uses the trained model to make predictions on the validation set. The mean of the FLOFO importance is then the difference in the performance of the model on the validation set over several randomised permutations.
         The difference between FLOFO importance and permutation importance is that the permutations on a feature's values are done within groups, where groups are obtained by grouping the validation set by k=2 features. These k features are chosen at random n=10 times, and the mean and standard deviation of the FLOFO importance are calculated based on these n runs.
         The reason this grouping makes the measure of importance better is that permuting a feature's value is no longer completely random. In fact, the permutations are done within groups of similar samples, so the permutations are equivalent to noising the samples. This ensures that:
+        
         * The permuted feature values are very unlikely to be replaced by unrealistic values.
         * A feature that is predictable by features among the chosen n*k features will be replaced by very similar values during permutation. Therefore, it will only slightly affect the model performance (and will yield a small FLOFO importance). This solves the correlated feature overestimation problem.
         
-        
-        
 Keywords: feature importance selection explainable data-science machine-learning
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `lofo-importance-0.3.2/setup.py` & `lofo-importance-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='lofo-importance',
-    version='0.3.2',
+    version='0.3.3',
     url="https://github.com/aerdem4/lofo-importance",
     author="Ahmet Erdem",
     author_email="ahmeterd4@gmail.com",
     description="Leave One Feature Out Importance",
     keywords="feature importance selection explainable data-science machine-learning",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

