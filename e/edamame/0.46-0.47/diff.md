# Comparing `tmp/edamame-0.46.tar.gz` & `tmp/edamame-0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edamame-0.46.tar", last modified: Sat Apr  8 08:51:17 2023, max compression
+gzip compressed data, was "edamame-0.47.tar", last modified: Sat Apr 15 12:36:12 2023, max compression
```

## Comparing `edamame-0.46.tar` & `edamame-0.47.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-08 08:51:17.845163 edamame-0.46/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 edamame-0.46/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     9481 2023-04-08 08:51:17.844519 edamame-0.46/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     7727 2023-04-07 13:57:59.000000 edamame-0.46/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-08 08:51:17.835412 edamame-0.46/edamame/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       21 2023-04-02 09:57:16.000000 edamame-0.46/edamame/__init__.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-08 08:51:17.838981 edamame-0.46/edamame/classifier/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       81 2023-04-06 20:59:47.000000 edamame-0.46/edamame/classifier/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    19334 2023-04-07 08:17:08.000000 edamame-0.46/edamame/classifier/classification.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-08 08:51:17.841612 edamame-0.46/edamame/eda/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      860 2023-04-06 20:58:22.000000 edamame-0.46/edamame/eda/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    32458 2023-03-25 15:28:28.000000 edamame-0.46/edamame/eda/eda.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3814 2023-03-25 15:57:39.000000 edamame-0.46/edamame/eda/tools.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-08 08:51:17.843665 edamame-0.46/edamame/regressor/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      189 2023-04-06 20:53:01.000000 edamame-0.46/edamame/regressor/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8324 2023-04-02 09:56:35.000000 edamame-0.46/edamame/regressor/diagnose.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    21388 2023-04-04 20:19:13.000000 edamame-0.46/edamame/regressor/regression.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-08 08:51:17.837787 edamame-0.46/edamame.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     9481 2023-04-08 08:51:17.000000 edamame-0.46/edamame.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      430 2023-04-08 08:51:17.000000 edamame-0.46/edamame.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-08 08:51:17.000000 edamame-0.46/edamame.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       83 2023-04-08 08:51:17.000000 edamame-0.46/edamame.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        8 2023-04-08 08:51:17.000000 edamame-0.46/edamame.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      803 2023-04-02 09:57:12.000000 edamame-0.46/pyproject.toml
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-08 08:51:17.845274 edamame-0.46/setup.cfg
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-15 12:36:12.813456 edamame-0.47/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 edamame-0.47/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     9635 2023-04-15 12:36:12.813107 edamame-0.47/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     7881 2023-04-15 12:20:06.000000 edamame-0.47/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-15 12:36:12.806535 edamame-0.47/edamame/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       21 2023-04-15 12:30:37.000000 edamame-0.47/edamame/__init__.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-15 12:36:12.809297 edamame-0.47/edamame/classifier/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       81 2023-04-06 20:59:47.000000 edamame-0.47/edamame/classifier/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    20589 2023-04-15 12:18:35.000000 edamame-0.47/edamame/classifier/classification.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-15 12:36:12.811287 edamame-0.47/edamame/eda/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      860 2023-04-06 20:58:22.000000 edamame-0.47/edamame/eda/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    32458 2023-03-25 15:28:28.000000 edamame-0.47/edamame/eda/eda.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3814 2023-03-25 15:57:39.000000 edamame-0.47/edamame/eda/tools.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-15 12:36:12.812599 edamame-0.47/edamame/regressor/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      189 2023-04-06 20:53:01.000000 edamame-0.47/edamame/regressor/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8324 2023-04-02 09:56:35.000000 edamame-0.47/edamame/regressor/diagnose.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    21388 2023-04-04 20:19:13.000000 edamame-0.47/edamame/regressor/regression.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-15 12:36:12.808361 edamame-0.47/edamame.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     9635 2023-04-15 12:36:12.000000 edamame-0.47/edamame.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      430 2023-04-15 12:36:12.000000 edamame-0.47/edamame.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-15 12:36:12.000000 edamame-0.47/edamame.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       83 2023-04-15 12:36:12.000000 edamame-0.47/edamame.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        8 2023-04-15 12:36:12.000000 edamame-0.47/edamame.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      803 2023-04-15 12:30:43.000000 edamame-0.47/pyproject.toml
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-15 12:36:12.813556 edamame-0.47/setup.cfg
```

### Comparing `edamame-0.46/LICENSE` & `edamame-0.47/LICENSE`

 * *Files identical despite different names*

### Comparing `edamame-0.46/PKG-INFO` & `edamame-0.47/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edamame
-Version: 0.46
+Version: 0.47
 Summary: Exploratory data analysis tools
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -31,15 +31,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 
 # Edamame
 
-[![Documentation Status](https://readthedocs.org/projects/ansicolortags/badge/?version=latest)](https://edamame-doc.readthedocs.io/en/latest/index.html)
+[![Documentation Status](https://readthedocs.org/projects/ansicolortags/badge/?version=latest)](https://edamame-doc.readthedocs.io/en/latest/index.html) [![PyPI version](https://badge.fury.io/py/edamame.svg)](https://badge.fury.io/py/edamame) ![PyPI - Downloads](https://img.shields.io/pypi/dm/edamame) 
 
 Edamame is inspired by packages such as [pandas-profiling](https://github.com/ydataai/pandas-profiling), [pycaret](https://github.com/pycaret/pycaret>), and [yellowbrick](https://github.com/DistrictDataLabs/yellowbrick>). The goal of Edamame is to provide user-friendly functions for conducting exploratory data analysis (EDA) on datasets, as well as for training and analyzing batteries of models for regression or classification problems.
 
 To install the package,
 
 ```console
 pip install edamame
@@ -87,15 +87,15 @@
 
 * Correlation Analysis functions:
 
    - **correlation_pearson**: The function performs the Pearson's correlation between the columns pairs. 
    - **correlation_categorical**: The function performs the Chi-Square Test of Independence between categorical variables of the dataset. 
    - **correlation_phik**: Calculate the Phik correlation coefficient between all pairs of columns ([Paper link](https://arxiv.org/pdf/1811.11440.pdf)).
 
-* Useful function:
+* Useful functions:
 
    - **load_model**: The function load the model saved in the pickle format.
    - **setup**: The function returns the following elements: X_train, y_train, X_test, y_test.
    - **scaling**: The function returns the normalised/standardized matrix.
 
 <hr>
 
@@ -150,23 +150,21 @@
 
 * **logistic**: Fits a logistic model to the training data.
 * **gaussian_nb**: Fits a Gaussina Naive Bayes model to the training data.
 * **knn**: Fits a k-Nearest Neighbors classification model to the training data.
 * **tree**: Fits a decision tree classification model to the training data.
 * **random_forest**: Fits a random forest classification model to the training data.
 * **xgboost**: Fits an XGBoost classification model to the training data.
+* * **svm**: Fits an Support Vector classification model to the training data.
 * **auto_ml**: Uses AutoML to select the best model based on performance metrics.
 * **model_metrics**: Computes and prints the performance metrics for each trained model.
 * **save_model**: Saves the trained model to a file.
 
 <hr>
 
 ## Todos
 
-
-* Add support for SVM to the classifier module.
 * Add the ClassifierDiagnose class to the classifier module.
 * Add the notebook for EDA in a classification problem to the edamame-notebook repository.
 * Add the notebook for training/diagnosing classification models to the edamame-notebook repository.
-* **Add link to docs url**.
```

### Comparing `edamame-0.46/README.md` & `edamame-0.47/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 # Edamame
 
-[![Documentation Status](https://readthedocs.org/projects/ansicolortags/badge/?version=latest)](https://edamame-doc.readthedocs.io/en/latest/index.html)
+[![Documentation Status](https://readthedocs.org/projects/ansicolortags/badge/?version=latest)](https://edamame-doc.readthedocs.io/en/latest/index.html) [![PyPI version](https://badge.fury.io/py/edamame.svg)](https://badge.fury.io/py/edamame) ![PyPI - Downloads](https://img.shields.io/pypi/dm/edamame) 
 
 Edamame is inspired by packages such as [pandas-profiling](https://github.com/ydataai/pandas-profiling), [pycaret](https://github.com/pycaret/pycaret>), and [yellowbrick](https://github.com/DistrictDataLabs/yellowbrick>). The goal of Edamame is to provide user-friendly functions for conducting exploratory data analysis (EDA) on datasets, as well as for training and analyzing batteries of models for regression or classification problems.
 
 To install the package,
 
 ```console
 pip install edamame
@@ -54,15 +54,15 @@
 
 * Correlation Analysis functions:
 
    - **correlation_pearson**: The function performs the Pearson's correlation between the columns pairs. 
    - **correlation_categorical**: The function performs the Chi-Square Test of Independence between categorical variables of the dataset. 
    - **correlation_phik**: Calculate the Phik correlation coefficient between all pairs of columns ([Paper link](https://arxiv.org/pdf/1811.11440.pdf)).
 
-* Useful function:
+* Useful functions:
 
    - **load_model**: The function load the model saved in the pickle format.
    - **setup**: The function returns the following elements: X_train, y_train, X_test, y_test.
    - **scaling**: The function returns the normalised/standardized matrix.
 
 <hr>
 
@@ -117,23 +117,21 @@
 
 * **logistic**: Fits a logistic model to the training data.
 * **gaussian_nb**: Fits a Gaussina Naive Bayes model to the training data.
 * **knn**: Fits a k-Nearest Neighbors classification model to the training data.
 * **tree**: Fits a decision tree classification model to the training data.
 * **random_forest**: Fits a random forest classification model to the training data.
 * **xgboost**: Fits an XGBoost classification model to the training data.
+* * **svm**: Fits an Support Vector classification model to the training data.
 * **auto_ml**: Uses AutoML to select the best model based on performance metrics.
 * **model_metrics**: Computes and prints the performance metrics for each trained model.
 * **save_model**: Saves the trained model to a file.
 
 <hr>
 
 ## Todos
 
-
-* Add support for SVM to the classifier module.
 * Add the ClassifierDiagnose class to the classifier module.
 * Add the notebook for EDA in a classification problem to the edamame-notebook repository.
 * Add the notebook for training/diagnosing classification models to the edamame-notebook repository.
-* **Add link to docs url**.
```

### Comparing `edamame-0.46/edamame/classifier/classification.py` & `edamame-0.47/edamame/classifier/classification.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from sklearn.model_selection import GridSearchCV, KFold, cross_val_score
 from sklearn.metrics import confusion_matrix, classification_report
 import seaborn as sns
 import pickle
 from IPython.display import display, Markdown
 import matplotlib.pyplot as plt 
 from typing import Tuple, Literal, List
+from sklearn.svm import SVC
 # pandas options
 pd.set_option('display.max_columns', None)
 pd.set_option('display.width', None)
 pd.set_option('display.max_colwidth', None)
 
 
 class TrainClassifier:
@@ -40,14 +41,15 @@
         >>> classifier.model_metrics(model_name="logisitc")
         >>> classifier.model_save(model_name="logisitc")
         >>> nb = classifier.gaussian_nb()
         >>> knn = classifier.knn()
         >>> tree = classifier.tree()
         >>> rf = classifier.random_forest()
         >>> xgb = classifier.xgboost()
+        >>> svm = classifier.svm()
         >>> classifier.model_metrics()
         >>> # using AutoML
         >>> models = classifier.auto_ml()
         >>> classifier.save_model()
     """
     def __init__(self, X_train, y_train, X_test, y_test):
         self.X_train = X_train
@@ -63,14 +65,15 @@
         # init the model 
         self.__logistic_fit = {}
         self.__gaussian_nb_fit = {}
         self.__knn_fit = {}
         self.__tree_fit = {}
         self.__random_forest_fit = {}
         self.__xgb_fit = {}
+        self.__svm_fit = {}
 
 
     def logistic(self) -> LogisticRegression:
         """
         Trains a logistic regression model using the training data and returns the fitted model.
 
         Returns:
@@ -220,34 +223,57 @@
         xgb_m = XGBClassifier()
         reg_xgb = GridSearchCV(xgb_m, tuned_parameters, cv=n_folds, refit=True, verbose=0, scoring='accuracy')
         reg_xgb.fit(self.X_train, self.y_train.squeeze())
         # save the model in the instance attributes
         self.__xgb_fit = reg_xgb.best_estimator_
         # return step 
         return self.__xgb_fit
+    
 
+    def svm(self, kernel: Literal["linear", "poly", "rbf", "sigmoid", "precomputed"] = "rbf", *args, **kwargs) -> SVC:
+        """
+        Trains an SVM classifier using the training data and returns the fitted model.
 
-    def model_metrics(self, model_name: Literal["all", "logistic", "guassian_nb", "knn", "tree", "random_forest", "xgboost"] = 'all') -> None:
+        Args:
+            kernel (Literal["linear", "poly", "rbf", "sigmoid", "precomputed"]): The kernel type to be used in the algorithm. Default is "rbf".
+            *args: Variable length argument list to be passed to the `SVC` constructor.
+            **kwargs: Arbitrary keyword arguments to be passed to the `SVC` constructor.
+        
+        Returns:
+            SVC: The trained SVM classifier.
+        
+        Example: 
+            >>> from edamame.classifier import TrainClassifier
+            >>> classifier = TrainClassifier(X_train=X_train, y_train=y_train, X_test=X_test, y_test=y_test)
+            >>> svm = classifier.svm(kernel="linear", C=1.0, gamma="auto")
+        """
+        svm_c = SVC(kernel=kernel, *args, **kwargs)
+        svm_c.fit(self.X_train, self.y_train.squeeze())
+        self.__svm_fit = svm_c
+        return self.__svm_fit
+
+
+    def model_metrics(self, model_name: Literal["all", "logistic", "guassian_nb", "knn", "tree", "random_forest", "xgboost", "svm"] = 'all') -> None:
         """
         Display classification metrics (confusion matrix and classification report) for specified or all trained models.
 
         Args:
-            model_name (Literal["all", "logistic", "guassian_nb", "knn", "tree", "random_forest", "xgboost"]): The name of the model to display the metrics for. Defaults to 'all'.
+            model_name (Literal["all", "logistic", "guassian_nb", "knn", "tree", "random_forest", "xgboost", "svm"]): The name of the model to display the metrics for. Defaults to 'all'.
 
         Returns:
             None
 
         Example:
             >>> from edamame.classifier import TrainClassifier
             >>> classifier = TrainClassifier(X_train=X_train, y_train=y_train, X_test=X_test, y_test=y_test)
             >>> xgboost = classifier.xgboost(n_estimators=(10, 100, 5), n_folds=2) 
             >>> classifier.model_metrics(model_name="xgboost")
         """
-        model_dct = {'logistic': 0, 'guassian_nb': 1, 'knn': 2, 'tree': 3, 'random_forest': 4, 'xgboost': 5}
-        model_list = [self.__logistic_fit, self.__gaussian_nb_fit, self.__knn_fit, self.__tree_fit, self.__random_forest_fit, self.__xgb_fit]
+        model_dct = {'logistic': 0, 'guassian_nb': 1, 'knn': 2, 'tree': 3, 'random_forest': 4, 'xgboost': 5, 'svm': 6}
+        model_list = [self.__logistic_fit, self.__gaussian_nb_fit, self.__knn_fit, self.__tree_fit, self.__random_forest_fit, self.__xgb_fit, self.__svm_fit]
         if model_name == 'all':
             for key in model_dct:
                 if model_list[model_dct[key]].__class__.__name__ == 'dict':
                         display(f'unable to show {key} model metrics')
                 else:
                     title = f'### {key} model metrics:'
                     display(Markdown(title))
@@ -287,17 +313,14 @@
                 display(Markdown(title))
                 print(classification_report(self.y_train, y_pred_train))
                 title = f'#### Test classification report'
                 display(Markdown(title))
                 print(classification_report(self.y_test, y_pred_test))
 
 
-    # ------------ #
-    # auto_ml
-    # ------------ #
     def auto_ml(self, n_folds: int = 5, data: Literal['train', 'test'] = 'train') -> List:
         """
         Perform automated machine learning with cross validation on a list of classification models.
         
         Args:
             n_folds (int): Number of cross-validation folds. Defaults to 5.
             data (Literal['train', 'test']): Target dataset for cross-validation. 
@@ -311,33 +334,35 @@
             >>> classifier = TrainClassifier(X_train=X_train, y_train=y_train, X_test=X_test, y_test=y_test)
             >>> model_list = classifier.auto_ml()
         """
         kfold = KFold(n_splits=n_folds)
         cv_mean = []
         score = []
         std = []
-        classifier = ["Logistic", "Gaussian NB", "KNN", "Tree", "Random forest", "Xgboost"]
+        classifier = ["Logistic", "Gaussian NB", "KNN", "Tree", "Random forest", "Xgboost", "SVM"]
         try:
             model_list = [LogisticRegression(), GaussianNB(), KNeighborsClassifier(n_neighbors=self.__knn_fit.n_neighbors),
                           DecisionTreeClassifier(ccp_alpha=self.__tree_fit.ccp_alpha, min_impurity_decrease=self.__tree_fit.min_impurity_decrease),
-                          RandomForestClassifier(n_estimators = self.__random_forest_fit.n_estimators, warm_start=True, n_jobs=-1), 
-                          XGBClassifier(n_estimators = self.__xgb_fit.n_estimators)]
+                          RandomForestClassifier(n_estimators=self.__random_forest_fit.n_estimators, warm_start=True, n_jobs=-1), 
+                          XGBClassifier(n_estimators=self.__xgb_fit.n_estimators),
+                          SVC(kernel=self.__svm_fit.kernel)]
         except:
             # find best hyperparameters
             self.logistic()
             self.gaussian_nb()
             self.knn()
             self.tree()
             self.random_forest()
             self.xgboost()
             # model list 
             model_list = [LogisticRegression(), GaussianNB(), KNeighborsClassifier(n_neighbors=self.__knn_fit.n_neighbors),
                           DecisionTreeClassifier(ccp_alpha=self.__tree_fit.ccp_alpha, min_impurity_decrease=self.__tree_fit.min_impurity_decrease),
                           RandomForestClassifier(n_estimators = self.__random_forest_fit.n_estimators, warm_start=True, n_jobs=-1),
-                          XGBClassifier(n_estimators = self.__xgb_fit.n_estimators)]
+                          XGBClassifier(n_estimators = self.__xgb_fit.n_estimators),
+                          SVC()]
         # cross validation loop 
         for model in model_list:
             if data == 'train':
                 cv_result = cross_val_score(model, self.X_train, self.y_train.squeeze(), cv=kfold, scoring="accuracy")
             elif data == 'test':
                 cv_result = cross_val_score(model, self.X_test, self.y_test.squeeze(), cv=kfold, scoring="accuracy")
             else:
@@ -353,39 +378,36 @@
         display(df_kfold_result)
         # boxplot on R2
         box = pd.DataFrame(score, index=classifier)
         plt.figure(figsize=(10,8))
         box.T.boxplot()
         plt.show()
 
-        return [self.__logistic_fit, self.__gaussian_nb_fit, self.__knn_fit, self.__tree_fit, self.__random_forest_fit, self.__xgb_fit]
+        return [self.__logistic_fit, self.__gaussian_nb_fit, self.__knn_fit, self.__tree_fit, self.__random_forest_fit, self.__xgb_fit, self.__svm_fit]
 
 
-    # ------------ #
-    # save model
-    # ------------ #
-    def save_model(self, model_name: Literal["all", "logistic", "guassian_nb", "knn", "tree", "random_forest", "xgboost"] = 'all') -> None:
+    def save_model(self, model_name: Literal["all", "logistic", "guassian_nb", "knn", "tree", "random_forest", "xgboost", "svm"] = 'all') -> None:
         """
         Saves the specified machine learning model or all models in the instance to a pickle file.
 
         Args:
-            model_name (Literal["all", "linear", "lasso", "ridge", "tree", "random_forest", "xgboost"]): 
+            model_name (Literal["all", "linear", "lasso", "ridge", "tree", "random_forest", "xgboost", "svm"]): 
                 The name of the model to save. Defaults to 'all'.
             
         Returns:
             None
 
         Example:
             >>> from edamame.classifier import TrainClassifier
             >>> classifier = TrainClassifier(X_train=X_train, y_train=y_train, X_test=X_test, y_test=y_test)
             >>> model_list = classifier.auto_ml()
             >>> classifier.save_model(model_name="all")
         """
-        model_dct = {'logistic': 0, 'guassian_nb': 1, 'knn': 2, 'tree': 3, 'random_forest': 4, 'xgboost': 5}
-        model_list = [self.__logistic_fit, self.__gaussian_nb_fit, self.__knn_fit, self.__tree_fit, self.__random_forest_fit, self.__xgb_fit]
+        model_dct = {'logistic': 0, 'guassian_nb': 1, 'knn': 2, 'tree': 3, 'random_forest': 4, 'xgboost': 5, 'svm': 6}
+        model_list = [self.__logistic_fit, self.__gaussian_nb_fit, self.__knn_fit, self.__tree_fit, self.__random_forest_fit, self.__xgb_fit, self.__svm_fit]
         if model_name == 'all':
             for key in model_dct:
                 if model_list[model_dct[key]].__class__.__name__ == 'dict':
                         display(f'unable to save {key} model')
                 else:
                     filename = f'{key}.pkl'
                     with open(filename, 'wb') as file:
```

### Comparing `edamame-0.46/edamame/eda/__init__.py` & `edamame-0.47/edamame/eda/__init__.py`

 * *Files identical despite different names*

### Comparing `edamame-0.46/edamame/eda/eda.py` & `edamame-0.47/edamame/eda/eda.py`

 * *Files identical despite different names*

### Comparing `edamame-0.46/edamame/eda/tools.py` & `edamame-0.47/edamame/eda/tools.py`

 * *Files identical despite different names*

### Comparing `edamame-0.46/edamame/regressor/diagnose.py` & `edamame-0.47/edamame/regressor/diagnose.py`

 * *Files identical despite different names*

### Comparing `edamame-0.46/edamame/regressor/regression.py` & `edamame-0.47/edamame/regressor/regression.py`

 * *Files identical despite different names*

### Comparing `edamame-0.46/edamame.egg-info/PKG-INFO` & `edamame-0.47/edamame.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edamame
-Version: 0.46
+Version: 0.47
 Summary: Exploratory data analysis tools
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -31,15 +31,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 
 # Edamame
 
-[![Documentation Status](https://readthedocs.org/projects/ansicolortags/badge/?version=latest)](https://edamame-doc.readthedocs.io/en/latest/index.html)
+[![Documentation Status](https://readthedocs.org/projects/ansicolortags/badge/?version=latest)](https://edamame-doc.readthedocs.io/en/latest/index.html) [![PyPI version](https://badge.fury.io/py/edamame.svg)](https://badge.fury.io/py/edamame) ![PyPI - Downloads](https://img.shields.io/pypi/dm/edamame) 
 
 Edamame is inspired by packages such as [pandas-profiling](https://github.com/ydataai/pandas-profiling), [pycaret](https://github.com/pycaret/pycaret>), and [yellowbrick](https://github.com/DistrictDataLabs/yellowbrick>). The goal of Edamame is to provide user-friendly functions for conducting exploratory data analysis (EDA) on datasets, as well as for training and analyzing batteries of models for regression or classification problems.
 
 To install the package,
 
 ```console
 pip install edamame
@@ -87,15 +87,15 @@
 
 * Correlation Analysis functions:
 
    - **correlation_pearson**: The function performs the Pearson's correlation between the columns pairs. 
    - **correlation_categorical**: The function performs the Chi-Square Test of Independence between categorical variables of the dataset. 
    - **correlation_phik**: Calculate the Phik correlation coefficient between all pairs of columns ([Paper link](https://arxiv.org/pdf/1811.11440.pdf)).
 
-* Useful function:
+* Useful functions:
 
    - **load_model**: The function load the model saved in the pickle format.
    - **setup**: The function returns the following elements: X_train, y_train, X_test, y_test.
    - **scaling**: The function returns the normalised/standardized matrix.
 
 <hr>
 
@@ -150,23 +150,21 @@
 
 * **logistic**: Fits a logistic model to the training data.
 * **gaussian_nb**: Fits a Gaussina Naive Bayes model to the training data.
 * **knn**: Fits a k-Nearest Neighbors classification model to the training data.
 * **tree**: Fits a decision tree classification model to the training data.
 * **random_forest**: Fits a random forest classification model to the training data.
 * **xgboost**: Fits an XGBoost classification model to the training data.
+* * **svm**: Fits an Support Vector classification model to the training data.
 * **auto_ml**: Uses AutoML to select the best model based on performance metrics.
 * **model_metrics**: Computes and prints the performance metrics for each trained model.
 * **save_model**: Saves the trained model to a file.
 
 <hr>
 
 ## Todos
 
-
-* Add support for SVM to the classifier module.
 * Add the ClassifierDiagnose class to the classifier module.
 * Add the notebook for EDA in a classification problem to the edamame-notebook repository.
 * Add the notebook for training/diagnosing classification models to the edamame-notebook repository.
-* **Add link to docs url**.
```

### Comparing `edamame-0.46/pyproject.toml` & `edamame-0.47/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "edamame"
-version = "0.46"
+version = "0.47"
 authors = [
   { name="Marco Salvalaggio", email="mar.salvalaggio@gmail.com" },
 ]
 description = "Exploratory data analysis tools"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

