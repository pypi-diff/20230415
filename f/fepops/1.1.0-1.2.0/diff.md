# Comparing `tmp/fepops-1.1.0.tar.gz` & `tmp/fepops-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fepops-1.1.0.tar", last modified: Tue Apr  4 18:45:19 2023, max compression
+gzip compressed data, was "fepops-1.2.0.tar", last modified: Sat Apr 15 21:05:36 2023, max compression
```

## Comparing `fepops-1.1.0.tar` & `fepops-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-04-04 18:45:19.061326 fepops-1.1.0/
--rw-rw-r--   0 justin    (1002) justin    (1002)     1068 2022-12-16 13:40:46.000000 fepops-1.1.0/LICENSE.md
--rw-rw-r--   0 justin    (1002) justin    (1002)     4475 2023-04-04 18:45:19.061326 fepops-1.1.0/PKG-INFO
--rw-rw-r--   0 justin    (1002) justin    (1002)     4054 2023-03-28 16:17:49.000000 fepops-1.1.0/README.md
-drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-04-04 18:45:19.061326 fepops-1.1.0/fepops/
--rw-rw-r--   0 justin    (1002) justin    (1002)       26 2023-03-28 16:17:49.000000 fepops-1.1.0/fepops/__init__.py
--rw-rw-r--   0 justin    (1002) justin    (1002)     3597 2023-03-29 13:52:34.000000 fepops-1.1.0/fepops/__main__.py
--rw-rw-r--   0 justin    (1002) justin    (1002)    28409 2023-04-04 12:17:04.000000 fepops-1.1.0/fepops/fepops.py
-drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-04-04 18:45:19.061326 fepops-1.1.0/fepops.egg-info/
--rw-rw-r--   0 justin    (1002) justin    (1002)     4475 2023-04-04 18:45:18.000000 fepops-1.1.0/fepops.egg-info/PKG-INFO
--rw-rw-r--   0 justin    (1002) justin    (1002)      269 2023-04-04 18:45:19.000000 fepops-1.1.0/fepops.egg-info/SOURCES.txt
--rw-rw-r--   0 justin    (1002) justin    (1002)        1 2023-04-04 18:45:18.000000 fepops-1.1.0/fepops.egg-info/dependency_links.txt
--rw-rw-r--   0 justin    (1002) justin    (1002)      119 2023-04-04 18:45:18.000000 fepops-1.1.0/fepops.egg-info/requires.txt
--rw-rw-r--   0 justin    (1002) justin    (1002)        7 2023-04-04 18:45:18.000000 fepops-1.1.0/fepops.egg-info/top_level.txt
--rw-rw-r--   0 justin    (1002) justin    (1002)      118 2023-04-01 11:25:23.000000 fepops-1.1.0/pyproject.toml
--rw-rw-r--   0 justin    (1002) justin    (1002)      680 2023-04-04 18:45:19.061326 fepops-1.1.0/setup.cfg
-drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-04-04 18:45:19.061326 fepops-1.1.0/test/
--rw-rw-r--   0 justin    (1002) justin    (1002)      956 2023-04-01 11:25:23.000000 fepops-1.1.0/test/tests.py
+drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-04-15 21:05:36.973395 fepops-1.2.0/
+-rw-rw-r--   0 justin    (1002) justin    (1002)     1068 2022-12-16 13:40:46.000000 fepops-1.2.0/LICENSE.md
+-rw-rw-r--   0 justin    (1002) justin    (1002)     4499 2023-04-15 21:05:36.973395 fepops-1.2.0/PKG-INFO
+-rw-rw-r--   0 justin    (1002) justin    (1002)     4078 2023-04-04 21:29:22.000000 fepops-1.2.0/README.md
+drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-04-15 21:05:36.973395 fepops-1.2.0/fepops/
+-rw-rw-r--   0 justin    (1002) justin    (1002)       26 2023-03-28 16:17:49.000000 fepops-1.2.0/fepops/__init__.py
+-rw-rw-r--   0 justin    (1002) justin    (1002)     3717 2023-04-08 17:08:41.000000 fepops-1.2.0/fepops/__main__.py
+-rw-rw-r--   0 justin    (1002) justin    (1002)    20613 2023-04-14 16:19:38.000000 fepops-1.2.0/fepops/fepops.py
+drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-04-15 21:05:36.973395 fepops-1.2.0/fepops.egg-info/
+-rw-rw-r--   0 justin    (1002) justin    (1002)     4499 2023-04-15 21:05:36.000000 fepops-1.2.0/fepops.egg-info/PKG-INFO
+-rw-rw-r--   0 justin    (1002) justin    (1002)      269 2023-04-15 21:05:36.000000 fepops-1.2.0/fepops.egg-info/SOURCES.txt
+-rw-rw-r--   0 justin    (1002) justin    (1002)        1 2023-04-15 21:05:36.000000 fepops-1.2.0/fepops.egg-info/dependency_links.txt
+-rw-rw-r--   0 justin    (1002) justin    (1002)      119 2023-04-15 21:05:36.000000 fepops-1.2.0/fepops.egg-info/requires.txt
+-rw-rw-r--   0 justin    (1002) justin    (1002)        7 2023-04-15 21:05:36.000000 fepops-1.2.0/fepops.egg-info/top_level.txt
+-rw-rw-r--   0 justin    (1002) justin    (1002)      118 2023-04-01 11:25:23.000000 fepops-1.2.0/pyproject.toml
+-rw-rw-r--   0 justin    (1002) justin    (1002)      680 2023-04-15 21:05:36.973395 fepops-1.2.0/setup.cfg
+drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-04-15 21:05:36.973395 fepops-1.2.0/test/
+-rw-rw-r--   0 justin    (1002) justin    (1002)      956 2023-04-01 11:25:23.000000 fepops-1.2.0/test/tests.py
```

### Comparing `fepops-1.1.0/LICENSE.md` & `fepops-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fepops-1.1.0/PKG-INFO` & `fepops-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fepops
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python implementation of the FEPOPS molecular descriptors
 Home-page: https://github.com/JustinYKC/FEPOPS
 Author: Yan-Kai Chen
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -26,16 +26,17 @@
 # Requirements
 This FEPOPS implementation requires the following packages:
 - rdkit (>=2019.09.x.x)
 - numpy (>=1.19.x)
 - pandas (>=1.5.0)
 - scikit-learn (>=0.20.x)
 - scipy (>=1.7.x)
-- PyTorch (>= 1.0.0)
-- kmeans-pytorch (>=0.3)
+- PyTorch (>=1.0.0)
+- fast-pytorch-kmeans (>=0.1.9)
+- tqdm (>=4.48.0)
 
 # Usage
 A quickstart example to generate the FEPOPS descriptors for a molecule directly from its SMILES as follows: In terminal:
 ```
 python fepops.py get_fepops -ismi "O=C1OC2=CC3(C)C(CC4OC(=O)C(OC(=O)C)C5C6(OCC45C3C(O)C6O)C(=O)OC)C(C2=C1)C" 
 ```
```

### Comparing `fepops-1.1.0/README.md` & `fepops-1.2.0/fepops.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: fepops
+Version: 1.2.0
+Summary: Python implementation of the FEPOPS molecular descriptors
+Home-page: https://github.com/JustinYKC/FEPOPS
+Author: Yan-Kai Chen
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 # FEPOPS(feature point pharmacophores)
 Python implementation of the FEPOPS molecular similarity method and descriptor generator. The FEPOPS descriptors is a 3D method of molecular representation by four centroids with five pharmacophoric features (i.e. atomic logP, atomic partial charges, hydrogen bond acceptors, hydrogen bond donors, and 6 distances between the four centroids). This implementation was recreated following the original paper: [https://pubs.acs.org/doi/10.1021/jm049654z](https://pubs.acs.org/doi/10.1021/jm049654z)
 
 ### Steps for implementation:
 1. Preprocessing: Molecules were filtered by the number of atoms (< 4), the number of rings (> 9), and the number of rotatable bonds (< 40). A salt/ions filter was then applied. Filtering carried out using `mol_filter.py`.
 2. Tautomer enumeration: Tautomers for each molecule were enumerated and saved as mol objects (codes in `fepops.py`).
 3. Sample conformers through rotation of flexible bonds: Each tautomer underwent conformer generation, changing the angles of all rotatable bonds. Up to 1024 conformers are sampled from the pool of conformers if more than 5 rotatable bonds are found in a molecule (codes in `fepops.py`).
@@ -13,16 +26,17 @@
 # Requirements
 This FEPOPS implementation requires the following packages:
 - rdkit (>=2019.09.x.x)
 - numpy (>=1.19.x)
 - pandas (>=1.5.0)
 - scikit-learn (>=0.20.x)
 - scipy (>=1.7.x)
-- PyTorch (>= 1.0.0)
-- kmeans-pytorch (>=0.3)
+- PyTorch (>=1.0.0)
+- fast-pytorch-kmeans (>=0.1.9)
+- tqdm (>=4.48.0)
 
 # Usage
 A quickstart example to generate the FEPOPS descriptors for a molecule directly from its SMILES as follows: In terminal:
 ```
 python fepops.py get_fepops -ismi "O=C1OC2=CC3(C)C(CC4OC(=O)C(OC(=O)C)C5C6(OCC45C3C(O)C6O)C(=O)OC)C(C2=C1)C" 
 ```
 
@@ -61,8 +75,8 @@
                 continue
             elif "SMILES Parse Error" in err:
                 print (f"# {id} SMILES_parse_error\n")
                 continue
 
         fepops_features = f.get_fepops(smiles)
         print (f"{fepops_features}\n")
-```
+```
```

### Comparing `fepops-1.1.0/fepops.egg-info/PKG-INFO` & `fepops-1.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: fepops
-Version: 1.1.0
-Summary: Python implementation of the FEPOPS molecular descriptors
-Home-page: https://github.com/JustinYKC/FEPOPS
-Author: Yan-Kai Chen
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # FEPOPS(feature point pharmacophores)
 Python implementation of the FEPOPS molecular similarity method and descriptor generator. The FEPOPS descriptors is a 3D method of molecular representation by four centroids with five pharmacophoric features (i.e. atomic logP, atomic partial charges, hydrogen bond acceptors, hydrogen bond donors, and 6 distances between the four centroids). This implementation was recreated following the original paper: [https://pubs.acs.org/doi/10.1021/jm049654z](https://pubs.acs.org/doi/10.1021/jm049654z)
 
 ### Steps for implementation:
 1. Preprocessing: Molecules were filtered by the number of atoms (< 4), the number of rings (> 9), and the number of rotatable bonds (< 40). A salt/ions filter was then applied. Filtering carried out using `mol_filter.py`.
 2. Tautomer enumeration: Tautomers for each molecule were enumerated and saved as mol objects (codes in `fepops.py`).
 3. Sample conformers through rotation of flexible bonds: Each tautomer underwent conformer generation, changing the angles of all rotatable bonds. Up to 1024 conformers are sampled from the pool of conformers if more than 5 rotatable bonds are found in a molecule (codes in `fepops.py`).
@@ -26,16 +13,17 @@
 # Requirements
 This FEPOPS implementation requires the following packages:
 - rdkit (>=2019.09.x.x)
 - numpy (>=1.19.x)
 - pandas (>=1.5.0)
 - scikit-learn (>=0.20.x)
 - scipy (>=1.7.x)
-- PyTorch (>= 1.0.0)
-- kmeans-pytorch (>=0.3)
+- PyTorch (>=1.0.0)
+- fast-pytorch-kmeans (>=0.1.9)
+- tqdm (>=4.48.0)
 
 # Usage
 A quickstart example to generate the FEPOPS descriptors for a molecule directly from its SMILES as follows: In terminal:
 ```
 python fepops.py get_fepops -ismi "O=C1OC2=CC3(C)C(CC4OC(=O)C(OC(=O)C)C5C6(OCC45C3C(O)C6O)C(=O)OC)C(C2=C1)C" 
 ```
 
@@ -74,8 +62,8 @@
                 continue
             elif "SMILES Parse Error" in err:
                 print (f"# {id} SMILES_parse_error\n")
                 continue
 
         fepops_features = f.get_fepops(smiles)
         print (f"{fepops_features}\n")
-```
+```
```

### Comparing `fepops-1.1.0/setup.cfg` & `fepops-1.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fepops
-version = 1.1.0
+version = 1.2.0
 author = Yan-Kai Chen
 description = Python implementation of the FEPOPS molecular descriptors
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/JustinYKC/FEPOPS
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `fepops-1.1.0/test/tests.py` & `fepops-1.2.0/test/tests.py`

 * *Files identical despite different names*

