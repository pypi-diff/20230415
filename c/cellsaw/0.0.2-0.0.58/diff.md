# Comparing `tmp/cellsaw-0.0.2.tar.gz` & `tmp/cellsaw-0.0.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellsaw-0.0.2.tar", last modified: Tue Aug  2 14:27:43 2022, max compression
+gzip compressed data, was "dist/cellsaw-0.0.58.tar", last modified: Sat Apr 15 09:10:16 2023, max compression
```

## Comparing `cellsaw-0.0.2.tar` & `cellsaw-0.0.58.tar`

### file list

```diff
@@ -1,28 +1,43 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-02 14:27:43.368000 cellsaw-0.0.2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      280 2022-08-02 14:27:43.368000 cellsaw-0.0.2/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       30 2022-08-02 14:14:35.000000 cellsaw-0.0.2/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-02 14:27:43.364000 cellsaw-0.0.2/cellsaw/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      178 2022-08-02 14:27:42.000000 cellsaw-0.0.2/cellsaw/__version__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      178 2022-08-02 14:22:38.000000 cellsaw-0.0.2/cellsaw/_version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-02 14:27:43.364000 cellsaw-0.0.2/cellsaw/load/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      644 2022-07-27 13:48:03.000000 cellsaw-0.0.2/cellsaw/load/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13186 2022-07-27 14:02:35.000000 cellsaw-0.0.2/cellsaw/load/loadadata.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5572 2022-07-24 22:36:44.000000 cellsaw-0.0.2/cellsaw/load/preprocess.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-02 14:27:43.368000 cellsaw-0.0.2/cellsaw/merge/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2832 2022-07-29 16:47:18.000000 cellsaw-0.0.2/cellsaw/merge/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2372 2022-07-29 16:45:34.000000 cellsaw-0.0.2/cellsaw/merge/diffusion.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4964 2022-08-02 13:26:07.000000 cellsaw-0.0.2/cellsaw/merge/draw.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      325 2022-08-01 12:51:15.000000 cellsaw-0.0.2/cellsaw/merge/eval.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3527 2022-07-29 14:01:03.000000 cellsaw-0.0.2/cellsaw/merge/mergehelpers.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-02 14:27:43.368000 cellsaw-0.0.2/cellsaw/similarity/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1396 2022-07-28 21:55:36.000000 cellsaw-0.0.2/cellsaw/similarity/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1640 2022-07-28 17:48:10.000000 cellsaw-0.0.2/cellsaw/similarity/draw.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1196 2022-07-28 21:27:56.000000 cellsaw-0.0.2/cellsaw/similarity/measures.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-02 14:27:43.364000 cellsaw-0.0.2/cellsaw.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      280 2022-08-02 14:27:42.000000 cellsaw-0.0.2/cellsaw.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      509 2022-08-02 14:27:43.000000 cellsaw-0.0.2/cellsaw.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-08-02 14:27:42.000000 cellsaw-0.0.2/cellsaw.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      147 2022-08-02 14:27:43.000000 cellsaw-0.0.2/cellsaw.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        8 2022-08-02 14:27:43.000000 cellsaw-0.0.2/cellsaw.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2022-08-02 14:27:43.368000 cellsaw-0.0.2/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3603 2022-08-02 14:27:02.000000 cellsaw-0.0.2/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-15 09:10:16.580000 cellsaw-0.0.58/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      281 2023-04-15 09:10:16.580000 cellsaw-0.0.58/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       32 2022-11-02 08:27:23.000000 cellsaw-0.0.58/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-15 09:10:16.572000 cellsaw-0.0.58/cellsaw/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-08-02 16:03:28.000000 cellsaw-0.0.58/cellsaw/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      179 2023-04-15 09:10:15.000000 cellsaw-0.0.58/cellsaw/__version__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      178 2022-08-02 14:22:38.000000 cellsaw-0.0.58/cellsaw/_version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-15 09:10:16.576000 cellsaw-0.0.58/cellsaw/annotate/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5744 2023-01-24 13:45:58.000000 cellsaw-0.0.58/cellsaw/annotate/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7171 2023-01-20 22:18:58.000000 cellsaw-0.0.58/cellsaw/annotate/annotators.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1529 2022-11-03 18:58:29.000000 cellsaw-0.0.58/cellsaw/annotate/draw.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12533 2023-02-02 15:24:55.000000 cellsaw-0.0.58/cellsaw/draw.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-15 09:10:16.576000 cellsaw-0.0.58/cellsaw/io_utils/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6578 2022-12-30 14:53:04.000000 cellsaw-0.0.58/cellsaw/io_utils/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13850 2023-01-03 17:15:57.000000 cellsaw-0.0.58/cellsaw/io_utils/loadadata.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-15 09:10:16.576000 cellsaw-0.0.58/cellsaw/merge/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4773 2023-02-27 13:26:00.000000 cellsaw-0.0.58/cellsaw/merge/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-15 09:10:16.580000 cellsaw-0.0.58/cellsaw/merge/diffusion/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3317 2023-01-20 16:01:31.000000 cellsaw-0.0.58/cellsaw/merge/diffusion/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11449 2023-02-20 18:07:44.000000 cellsaw-0.0.58/cellsaw/merge/diffusion/kernel.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      329 2022-08-09 16:42:26.000000 cellsaw-0.0.58/cellsaw/merge/eval.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4296 2023-01-13 09:58:39.000000 cellsaw-0.0.58/cellsaw/merge/hungarianEM.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4273 2023-04-10 06:48:33.000000 cellsaw-0.0.58/cellsaw/merge/mergehelpers.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9153 2023-02-27 22:28:27.000000 cellsaw-0.0.58/cellsaw/preprocess.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-15 09:10:16.580000 cellsaw-0.0.58/cellsaw/similarity/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5173 2023-01-05 16:53:41.000000 cellsaw-0.0.58/cellsaw/similarity/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2239 2023-02-23 12:41:59.000000 cellsaw-0.0.58/cellsaw/similarity/measures.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      505 2023-01-23 17:34:16.000000 cellsaw-0.0.58/cellsaw/util.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-15 09:10:16.576000 cellsaw-0.0.58/cellsaw.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      281 2023-04-15 09:10:15.000000 cellsaw-0.0.58/cellsaw.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      755 2023-04-15 09:10:16.000000 cellsaw-0.0.58/cellsaw.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-15 09:10:15.000000 cellsaw-0.0.58/cellsaw.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      147 2023-04-15 09:10:16.000000 cellsaw-0.0.58/cellsaw.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       13 2023-04-15 09:10:16.000000 cellsaw-0.0.58/cellsaw.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-15 09:10:16.580000 cellsaw-0.0.58/lucy/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9904 2023-04-09 07:26:38.000000 cellsaw-0.0.58/lucy/adatas.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7362 2023-03-03 12:02:03.000000 cellsaw-0.0.58/lucy/draw.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12654 2023-04-09 04:06:21.000000 cellsaw-0.0.58/lucy/embed.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1544 2023-03-14 14:35:12.000000 cellsaw-0.0.58/lucy/load.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5972 2023-02-19 10:08:16.000000 cellsaw-0.0.58/lucy/merge.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      814 2023-03-16 20:36:18.000000 cellsaw-0.0.58/lucy/score.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-15 09:10:16.580000 cellsaw-0.0.58/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3659 2023-04-15 09:10:00.000000 cellsaw-0.0.58/setup.py
```

### Comparing `cellsaw-0.0.2/cellsaw/load/loadadata.py` & `cellsaw-0.0.58/cellsaw/io_utils/loadadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 import pandas as pd
 from lmz import *
 import anndata as ad
 import numpy as np
 import random
 
 
-####
-# oldest datasets
-#######
+
+'''
+You can ignore this file :)
+'''
+
+
 load = lambda f: [l for l in open(f,'r').read().split('\n') if len(l)>1]
 
 
 def do_subsample(adata, subsample, seed = None):
     if not subsample:
         return adata
 
@@ -159,8 +162,26 @@
         barcode_cid[bc]= int(cl)
     #adata = ad.read_h5ad(fname)
     adata.obs['true'] = [barcode_cid.get(a,-1)  for a in adata.obs.index]
     fname = f"{path}/{item}.h5"
     adata.write(fname, compression='gzip')
 
 
+import csv
+import re
+def loadpangalolabels(path):
+    with open(path+"/cell_type_annotations.txt",'r') as f:
+        data = csv.reader(f)
+        return { "_".join(line[:3]):line[3]  for line in data}
+
+def annotatetruecelltype(dic, adata, name, f_out = 'truecelltype', f_in = 'clusterid'):
+    match = re.search(r'SRA\d*-SRS\d*', name)
+    eh = match.group().replace('-',"_")
+    adata.obs[f_out] = [  dic.get(f'{eh}_{c}', 'no pangalo')  for c in adata.obs[f_in]  ]
+    return adata
+
+
+def annotatepangalo(pangaloLabelPath, adatas, names):
+    d = loadpangalolabels(pangaloLabelPath)
+    return [ annotatetruecelltype(d,a,n) for a,n in zip(adatas,names) ]
+
```

### Comparing `cellsaw-0.0.2/cellsaw/merge/mergehelpers.py` & `cellsaw-0.0.58/cellsaw/merge/mergehelpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,69 +22,87 @@
                                 n_obs=smallest,
                                 random_state=0,
                                 copy=False)
         return data
 
 
 def unioncut(scores, numGenes, data):
+
     indices = np.argpartition(scores, -numGenes)[:,-numGenes:]
     indices = np.unique(indices.flatten())
-    return [d[:,indices].copy() for d in data]
-
+    [d._inplace_subset_var(indices) for d in data]
+    return data
+    #return [d[:,indices].copy() for d in data]
+
+
+def equal_contrib_gene_cut(scores,numgenes,data):
+    ar = np.array(scores)
+    ind = np.argsort(ar)
+
+    def calcoverlap(scores,number):
+        indices = scores[:,-number:]
+        indices = np.unique(indices.flatten())
+        return indices
+
+    def findcutoff(low,high, lp = -1):
+        probe = int((low+high)/2)
+        y = calcoverlap(ind,probe)
+        if probe == lp:
+            return y
+        if len(y) > numgenes:
+            return findcutoff(low,probe,probe)
+        else:
+            return findcutoff(probe,high,probe)
+
+    indices = findcutoff(0,numgenes)
+    [d._inplace_subset_var(indices) for d in data]
+    return data
 
 def dimension_reduction(adatas, scale, zero_center, PCA, umaps, joint_space=True):
-
-
     # get a (scaled) dx
     if scale or PCA:
         adatas= [sc.pp.scale(adata, zero_center=False, copy=True,max_value=10) for adata in adatas]
     dx = [adata.to_df().to_numpy() for adata in adatas]
     if joint_space == False:
         return disjoint_dimension_reduction(dx, PCA, umaps)
 
-
     res = []
-
-
     if PCA:
         pca = decomposition.PCA(n_components=PCA)
         pca.fit(np.vstack(dx))
         #print('printing explained_variance\n',list(pca.explained_variance_ratio_))# rm this:)
         dx = [ pca.transform(e) for e in dx  ]
         res.append(dx)
 
     for dim in umaps:
-        assert 0 < dim < PCA
+        assert 0 < dim < PCA, f'{dim=} {PCA=}'
         res.append(umapify(dx,dim))
 
     return res
 
 
-def umapify(dx, dimensions):
+def umapify(dx, dimensions,n_neighbors=10):
     mymap = umap.UMAP(n_components=dimensions,
-                      n_neighbors=10,
+                      n_neighbors=n_neighbors,
                       random_state=1337).fit(np.vstack(dx))
     return [mymap.transform(a) for a in dx]
 
 
 def disjoint_dimension_reduction(dx, PCA, umaps):
     res = []
     if PCA:
         pcaList = [decomposition.PCA(n_components=PCA) for x in dx]
         for pca, x in zip(pcaList, dx):
             pca.fit(np.vstack(x))
         #print('printing explained_variance\n',list(pca.explained_variance_ratio_))# rm this:)
         dx = [ pca.transform(e) for pca, e in zip(pcaList,dx)  ]
         res.append(dx)
-
     for dim in umaps:
         assert 0 < dim < PCA
         res.append(umapify(dx,dim))
-
-
     return res
 
 def hungarian(X1, X2, debug = False,metric='euclidean'):
     # get the matches:
     # import time
     # print("STARTING CALC")
     # now = time.time()
@@ -111,9 +129,8 @@
 
     if debug:
         x = distances[row_ind, col_ind]
         num_bins = 100
         print("hungarian: debug hist")
         plt.hist(x, num_bins, facecolor='blue', alpha=0.5)
         plt.show()
-
     return (row_ind, col_ind), distances
```

### Comparing `cellsaw-0.0.2/setup.py` & `cellsaw-0.0.58/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,15 +91,15 @@
             sys.stderr.write("Error: {}".format(e))
 
 setup(
     name='cellsaw',
     version=get_version(),
     author='Stefan Mautner',
     author_email='myl4stn4m3@cs.uni-freiburg.de',
-        packages=['cellsaw','cellsaw.similarity','cellsaw.merge','cellsaw.load'],
+        packages=['cellsaw','cellsaw.similarity','cellsaw.merge','cellsaw.annotate','cellsaw.io_utils','cellsaw.merge.diffusion','lucy'],
     scripts=[ ],
     include_package_data=True,
     package_data={},
     url='https://github.com/smautner/cellsaw',
     license='LICENSE',
     description='match clusters of sincle cell experiments with the Hungarian',
     #long_description=open('README.md').read(),
```

