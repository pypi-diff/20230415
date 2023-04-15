# Comparing `tmp/yascikit-learn-0.1.tar.gz` & `tmp/yascikit-learn-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yascikit-learn-0.1.tar", last modified: Sat Apr 15 05:19:31 2023, max compression
+gzip compressed data, was "yascikit-learn-0.1.1.tar", last modified: Sat Apr 15 06:03:02 2023, max compression
```

## Comparing `yascikit-learn-0.1.tar` & `yascikit-learn-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,27 @@
-drwxr-xr-x   0 yukino     (501) staff       (20)        0 2023-04-15 05:19:31.495080 yascikit-learn-0.1/
--rw-r--r--   0 yukino     (501) staff       (20)     1071 2023-04-15 02:32:35.000000 yascikit-learn-0.1/LICENSE
--rw-r--r--   0 yukino     (501) staff       (20)     3049 2023-04-15 05:19:31.494958 yascikit-learn-0.1/PKG-INFO
--rw-r--r--   0 yukino     (501) staff       (20)     2289 2023-04-15 05:18:56.000000 yascikit-learn-0.1/README.md
--rw-r--r--   0 yukino     (501) staff       (20)       38 2023-04-15 05:19:31.495117 yascikit-learn-0.1/setup.cfg
--rw-r--r--   0 yukino     (501) staff       (20)     1343 2023-04-15 03:49:34.000000 yascikit-learn-0.1/setup.py
-drwxr-xr-x   0 yukino     (501) staff       (20)        0 2023-04-15 05:19:31.494210 yascikit-learn-0.1/yascikit_learn.egg-info/
--rw-r--r--   0 yukino     (501) staff       (20)     3049 2023-04-15 05:19:31.000000 yascikit-learn-0.1/yascikit_learn.egg-info/PKG-INFO
--rw-r--r--   0 yukino     (501) staff       (20)      262 2023-04-15 05:19:31.000000 yascikit-learn-0.1/yascikit_learn.egg-info/SOURCES.txt
--rw-r--r--   0 yukino     (501) staff       (20)        1 2023-04-15 05:19:31.000000 yascikit-learn-0.1/yascikit_learn.egg-info/dependency_links.txt
--rw-r--r--   0 yukino     (501) staff       (20)       38 2023-04-15 05:19:31.000000 yascikit-learn-0.1/yascikit_learn.egg-info/requires.txt
--rw-r--r--   0 yukino     (501) staff       (20)       10 2023-04-15 05:19:31.000000 yascikit-learn-0.1/yascikit_learn.egg-info/top_level.txt
-drwxr-xr-x   0 yukino     (501) staff       (20)        0 2023-04-15 05:19:31.494431 yascikit-learn-0.1/yasklearn/
--rw-r--r--   0 yukino     (501) staff       (20)      135 2023-04-15 02:32:35.000000 yascikit-learn-0.1/yasklearn/__init__.py
--rw-r--r--   0 yukino     (501) staff       (20)    19552 2023-04-15 02:32:35.000000 yascikit-learn-0.1/yasklearn/naive_bayes.py
+drwxr-xr-x   0 yukino     (501) staff       (20)        0 2023-04-15 06:03:02.114770 yascikit-learn-0.1.1/
+-rw-r--r--   0 yukino     (501) staff       (20)     1071 2023-04-15 02:32:35.000000 yascikit-learn-0.1.1/LICENSE
+-rw-r--r--   0 yukino     (501) staff       (20)     3051 2023-04-15 06:03:02.114650 yascikit-learn-0.1.1/PKG-INFO
+-rw-r--r--   0 yukino     (501) staff       (20)     2289 2023-04-15 06:01:42.000000 yascikit-learn-0.1.1/README.md
+-rw-r--r--   0 yukino     (501) staff       (20)       38 2023-04-15 06:03:02.114953 yascikit-learn-0.1.1/setup.cfg
+-rw-r--r--   0 yukino     (501) staff       (20)     1448 2023-04-15 05:50:24.000000 yascikit-learn-0.1.1/setup.py
+drwxr-xr-x   0 yukino     (501) staff       (20)        0 2023-04-15 06:03:02.112033 yascikit-learn-0.1.1/yascikit_learn.egg-info/
+-rw-r--r--   0 yukino     (501) staff       (20)     3051 2023-04-15 06:03:02.000000 yascikit-learn-0.1.1/yascikit_learn.egg-info/PKG-INFO
+-rw-r--r--   0 yukino     (501) staff       (20)      556 2023-04-15 06:03:02.000000 yascikit-learn-0.1.1/yascikit_learn.egg-info/SOURCES.txt
+-rw-r--r--   0 yukino     (501) staff       (20)        1 2023-04-15 06:03:02.000000 yascikit-learn-0.1.1/yascikit_learn.egg-info/dependency_links.txt
+-rw-r--r--   0 yukino     (501) staff       (20)       38 2023-04-15 06:03:02.000000 yascikit-learn-0.1.1/yascikit_learn.egg-info/requires.txt
+-rw-r--r--   0 yukino     (501) staff       (20)       10 2023-04-15 06:03:02.000000 yascikit-learn-0.1.1/yascikit_learn.egg-info/top_level.txt
+drwxr-xr-x   0 yukino     (501) staff       (20)        0 2023-04-15 06:03:02.112236 yascikit-learn-0.1.1/yasklearn/
+-rw-r--r--   0 yukino     (501) staff       (20)      140 2023-04-15 05:53:04.000000 yascikit-learn-0.1.1/yasklearn/__init__.py
+drwxr-xr-x   0 yukino     (501) staff       (20)        0 2023-04-15 06:03:02.113510 yascikit-learn-0.1.1/yasklearn/cluster/
+-rw-r--r--   0 yukino     (501) staff       (20)      137 2023-04-15 03:47:14.000000 yascikit-learn-0.1.1/yasklearn/cluster/__init__.py
+-rw-r--r--   0 yukino     (501) staff       (20)     5503 2023-04-15 04:45:15.000000 yascikit-learn-0.1.1/yasklearn/cluster/k_medoids.py
+-rw-r--r--   0 yukino     (501) staff       (20)     3705 2023-04-15 05:08:40.000000 yascikit-learn-0.1.1/yasklearn/cluster/x_medoids.py
+-rw-r--r--   0 yukino     (501) staff       (20)     4304 2023-04-15 03:46:32.000000 yascikit-learn-0.1.1/yasklearn/cluster/xmeans.py
+drwxr-xr-x   0 yukino     (501) staff       (20)        0 2023-04-15 06:03:02.114177 yascikit-learn-0.1.1/yasklearn/decomposition/
+-rw-r--r--   0 yukino     (501) staff       (20)       98 2023-04-15 02:32:35.000000 yascikit-learn-0.1.1/yasklearn/decomposition/__init__.py
+-rw-r--r--   0 yukino     (501) staff       (20)     2357 2023-04-15 02:32:35.000000 yascikit-learn-0.1.1/yasklearn/decomposition/plsa.py
+-rw-r--r--   0 yukino     (501) staff       (20)     6347 2023-04-15 02:32:35.000000 yascikit-learn-0.1.1/yasklearn/decomposition/plsv.py
+drwxr-xr-x   0 yukino     (501) staff       (20)        0 2023-04-15 06:03:02.114457 yascikit-learn-0.1.1/yasklearn/model_selection/
+-rw-r--r--   0 yukino     (501) staff       (20)      102 2023-04-15 02:32:35.000000 yascikit-learn-0.1.1/yasklearn/model_selection/__init__.py
+-rw-r--r--   0 yukino     (501) staff       (20)     3698 2023-04-15 02:32:35.000000 yascikit-learn-0.1.1/yasklearn/model_selection/_split.py
+-rw-r--r--   0 yukino     (501) staff       (20)    19552 2023-04-15 02:32:35.000000 yascikit-learn-0.1.1/yasklearn/naive_bayes.py
```

### Comparing `yascikit-learn-0.1/LICENSE` & `yascikit-learn-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yascikit-learn-0.1/PKG-INFO` & `yascikit-learn-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yascikit-learn
-Version: 0.1
+Version: 0.1.1
 Summary: Yet another scikit-learn
 Home-page: https://github.com/ikegami-yukino/yascikit-learn
 Author: Yukino Ikegami
 Author-email: yknikgm@gmail.com
 License: MIT License
 Keywords: Machine Learning
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -90,15 +90,15 @@
 #### XMeans
 ```python
 from yasklearn.cluster import XMeans
 from sklearn import datasets
 
 dataset = datasets.load_iris()
 X = dataset.data
-xm = XMeans(n_clusters=2, random_state=1)
+xm = XMeans(n_clusters=3, random_state=1)
 xm.fit_predict(X)
 ```
 
 #### KMedoids
 ```python
 from yasklearn.cluster import KMedoids
 from sklearn import datasets
```

### Comparing `yascikit-learn-0.1/README.md` & `yascikit-learn-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 #### XMeans
 ```python
 from yasklearn.cluster import XMeans
 from sklearn import datasets
 
 dataset = datasets.load_iris()
 X = dataset.data
-xm = XMeans(n_clusters=2, random_state=1)
+xm = XMeans(n_clusters=3, random_state=1)
 xm.fit_predict(X)
 ```
 
 #### KMedoids
 ```python
 from yasklearn.cluster import KMedoids
 from sklearn import datasets
```

### Comparing `yascikit-learn-0.1/setup.py` & `yascikit-learn-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 from setuptools import setup
 
 with open(os.path.join('yasklearn', '__init__.py'), 'r', encoding='utf8') as f:
     version = re.compile(r".*__version__ = '(.*?)'",
                          re.S).match(f.read()).group(1)
 
 setup(name='yascikit-learn',
-      packages=['yasklearn'],
+      packages=[
+          'yasklearn', 'yasklearn.cluster', 'yasklearn.decomposition',
+          'yasklearn.model_selection'
+      ],
       version=version,
       license='MIT License',
       description='Yet another scikit-learn',
       author='Yukino Ikegami',
       author_email='yknikgm@gmail.com',
       url='https://github.com/ikegami-yukino/yascikit-learn',
       keywords=['Machine Learning'],
```

### Comparing `yascikit-learn-0.1/yascikit_learn.egg-info/PKG-INFO` & `yascikit-learn-0.1.1/yascikit_learn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yascikit-learn
-Version: 0.1
+Version: 0.1.1
 Summary: Yet another scikit-learn
 Home-page: https://github.com/ikegami-yukino/yascikit-learn
 Author: Yukino Ikegami
 Author-email: yknikgm@gmail.com
 License: MIT License
 Keywords: Machine Learning
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -90,15 +90,15 @@
 #### XMeans
 ```python
 from yasklearn.cluster import XMeans
 from sklearn import datasets
 
 dataset = datasets.load_iris()
 X = dataset.data
-xm = XMeans(n_clusters=2, random_state=1)
+xm = XMeans(n_clusters=3, random_state=1)
 xm.fit_predict(X)
 ```
 
 #### KMedoids
 ```python
 from yasklearn.cluster import KMedoids
 from sklearn import datasets
```

### Comparing `yascikit-learn-0.1/yasklearn/naive_bayes.py` & `yascikit-learn-0.1.1/yasklearn/naive_bayes.py`

 * *Files identical despite different names*

