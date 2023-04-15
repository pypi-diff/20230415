# Comparing `tmp/pandasgwas-0.99.8.tar.gz` & `tmp/pandasgwas-0.99.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pandasgwas-0.99.8.tar", last modified: Thu Jun 30 11:40:18 2022, max compression
+gzip compressed data, was "dist\pandasgwas-0.99.9.tar", last modified: Tue Jul 19 13:44:10 2022, max compression
```

## Comparing `pandasgwas-0.99.8.tar` & `pandasgwas-0.99.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2022-06-30 11:40:18.898263 pandasgwas-0.99.8/
--rw-rw-rw-   0        0        0     1118 2022-06-28 05:00:31.000000 pandasgwas-0.99.8/LICENSE
--rw-rw-rw-   0        0        0     4273 2022-06-30 11:40:18.897263 pandasgwas-0.99.8/PKG-INFO
--rw-rw-rw-   0        0        0     3591 2022-06-30 11:34:37.000000 pandasgwas-0.99.8/README.md
-drwxrwxrwx   0        0        0        0 2022-06-30 11:40:18.825308 pandasgwas-0.99.8/pandasgwas/
--rw-rw-rw-   0        0        0     8634 2022-06-22 01:52:14.000000 pandasgwas-0.99.8/pandasgwas/Association.py
--rw-rw-rw-   0        0        0     1362 2022-06-05 12:18:01.000000 pandasgwas-0.99.8/pandasgwas/Browser.py
--rw-rw-rw-   0        0        0     6538 2022-06-21 08:07:17.000000 pandasgwas-0.99.8/pandasgwas/SingleNucleotidePolymorphism.py
--rw-rw-rw-   0        0        0     7950 2022-06-21 08:07:16.000000 pandasgwas-0.99.8/pandasgwas/Study.py
--rw-rw-rw-   0        0        0     3833 2022-06-21 08:05:22.000000 pandasgwas-0.99.8/pandasgwas/Trait.py
--rw-rw-rw-   0        0        0      228 2022-06-22 01:52:14.000000 pandasgwas-0.99.8/pandasgwas/__init__.py
--rw-rw-rw-   0        0        0     8427 2022-06-05 12:18:01.000000 pandasgwas-0.99.8/pandasgwas/client.py
--rw-rw-rw-   0        0        0    78270 2022-06-06 13:16:18.000000 pandasgwas-0.99.8/pandasgwas/cytogenetic_bands.csv
--rw-rw-rw-   0        0        0     8267 2022-06-30 00:45:07.000000 pandasgwas-0.99.8/pandasgwas/get_SNPs.py
--rw-rw-rw-   0        0        0     4871 2022-06-05 12:18:01.000000 pandasgwas-0.99.8/pandasgwas/get_associations.py
--rw-rw-rw-   0        0        0     6828 2022-06-30 01:58:25.000000 pandasgwas-0.99.8/pandasgwas/get_studies.py
--rw-rw-rw-   0        0        0     4369 2022-06-05 12:18:01.000000 pandasgwas-0.99.8/pandasgwas/get_traits.py
--rw-rw-rw-   0        0        0     1695 2022-06-21 07:58:27.000000 pandasgwas-0.99.8/pandasgwas/set_operation.py
-drwxrwxrwx   0        0        0        0 2022-06-30 11:40:18.894266 pandasgwas-0.99.8/pandasgwas.egg-info/
--rw-rw-rw-   0        0        0     4273 2022-06-30 11:40:17.000000 pandasgwas-0.99.8/pandasgwas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2022-06-30 11:40:18.000000 pandasgwas-0.99.8/pandasgwas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-30 11:40:17.000000 pandasgwas-0.99.8/pandasgwas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2022-06-30 11:40:17.000000 pandasgwas-0.99.8/pandasgwas.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-06-30 11:40:18.000000 pandasgwas-0.99.8/pandasgwas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-06-07 12:29:56.000000 pandasgwas-0.99.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-06-30 11:40:18.898263 pandasgwas-0.99.8/setup.cfg
--rw-rw-rw-   0        0        0     1130 2022-06-30 11:34:57.000000 pandasgwas-0.99.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-07-19 13:44:10.912633 pandasgwas-0.99.9/
+-rw-rw-rw-   0        0        0     1118 2022-06-28 05:00:31.000000 pandasgwas-0.99.9/LICENSE
+-rw-rw-rw-   0        0        0     4281 2022-07-19 13:44:10.912633 pandasgwas-0.99.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3580 2022-07-19 13:34:05.000000 pandasgwas-0.99.9/README.md
+drwxrwxrwx   0        0        0        0 2022-07-19 13:44:10.865762 pandasgwas-0.99.9/pandasgwas/
+-rw-rw-rw-   0        0        0     8634 2022-06-22 01:52:14.000000 pandasgwas-0.99.9/pandasgwas/Association.py
+-rw-rw-rw-   0        0        0     1362 2022-06-05 12:18:01.000000 pandasgwas-0.99.9/pandasgwas/Browser.py
+-rw-rw-rw-   0        0        0     6538 2022-06-21 08:07:17.000000 pandasgwas-0.99.9/pandasgwas/SingleNucleotidePolymorphism.py
+-rw-rw-rw-   0        0        0     7950 2022-06-21 08:07:16.000000 pandasgwas-0.99.9/pandasgwas/Study.py
+-rw-rw-rw-   0        0        0     3833 2022-06-21 08:05:22.000000 pandasgwas-0.99.9/pandasgwas/Trait.py
+-rw-rw-rw-   0        0        0      228 2022-06-22 01:52:14.000000 pandasgwas-0.99.9/pandasgwas/__init__.py
+-rw-rw-rw-   0        0        0     8427 2022-06-05 12:18:01.000000 pandasgwas-0.99.9/pandasgwas/client.py
+-rw-rw-rw-   0        0        0    78270 2022-06-06 13:16:18.000000 pandasgwas-0.99.9/pandasgwas/cytogenetic_bands.csv
+-rw-rw-rw-   0        0        0     8267 2022-06-30 00:45:07.000000 pandasgwas-0.99.9/pandasgwas/get_SNPs.py
+-rw-rw-rw-   0        0        0     4871 2022-06-05 12:18:01.000000 pandasgwas-0.99.9/pandasgwas/get_associations.py
+-rw-rw-rw-   0        0        0     6828 2022-06-30 01:58:25.000000 pandasgwas-0.99.9/pandasgwas/get_studies.py
+-rw-rw-rw-   0        0        0     4369 2022-06-05 12:18:01.000000 pandasgwas-0.99.9/pandasgwas/get_traits.py
+-rw-rw-rw-   0        0        0     1695 2022-06-21 07:58:27.000000 pandasgwas-0.99.9/pandasgwas/set_operation.py
+drwxrwxrwx   0        0        0        0 2022-07-19 13:44:10.912633 pandasgwas-0.99.9/pandasgwas.egg-info/
+-rw-rw-rw-   0        0        0     4281 2022-07-19 13:44:09.000000 pandasgwas-0.99.9/pandasgwas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2022-07-19 13:44:10.000000 pandasgwas-0.99.9/pandasgwas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-07-19 13:44:09.000000 pandasgwas-0.99.9/pandasgwas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2022-07-19 13:44:09.000000 pandasgwas-0.99.9/pandasgwas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2022-07-19 13:44:09.000000 pandasgwas-0.99.9/pandasgwas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2022-06-07 12:29:56.000000 pandasgwas-0.99.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2022-07-19 13:44:10.912633 pandasgwas-0.99.9/setup.cfg
+-rw-rw-rw-   0        0        0     1162 2022-07-19 13:31:55.000000 pandasgwas-0.99.9/setup.py
```

### Comparing `pandasgwas-0.99.8/LICENSE` & `pandasgwas-0.99.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasgwas-0.99.8/PKG-INFO` & `pandasgwas-0.99.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: pandasgwas
-Version: 0.99.8
-Summary: A Python package to query, download and wrangle GWAS catalog data
+Version: 0.99.9
+Summary: A Python package for easy retrieval of GWAS catalog data
 Home-page: https://github.com/caotianze/pandasgwas
 Author: Cao Tianze
 Author-email: hnrcao@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/caotianze/pandasgwas/issues
-Keywords: GWAS pandas
+Keywords: gwas,genomics,snp,bioinformatics,pandas
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# pandasGWAS: a Python package to query, download and wrangle GWAS catalog data
+# pandasGWAS: a Python package for easy retrieval of GWAS catalog data
 ## Dependencies
 python: 3.8  
 pandas: 1.1.3  
 requests: 2.28.1  
 progressbar2: 4.0.0
 ## Documentation
 See [pandasGWAS Documentation](https://caotianze.github.io/pandasgwas/)
 ## Development Environment
 OS: Windows10 Professional  
 IDE: PyCharm 2022.1 (Community Edition)
 ## Installation
 `pip install pandasgwas`
 ## Example
+Get studies related to triple-negative breast cancer:
 ```Python
-# Get studies related to triple-negative breast cancer:
 from pandasgwas.get_studies import get_studies
 studies = get_studies(efo_trait = 'triple-negative breast cancer')
 studies.studies[0:4]
 #                  initialSampleSize                    gxe    gxg   snpCount  qualifier  imputed  pooled studyDesignComment  accessionId   fullPvalueSet  userRequested            platforms                                ancestries                                   genotypingTechnologies                             replicationSampleSize                                diseaseTrait.trait                 publicationInfo.pubmedId publicationInfo.publicationDate publicationInfo.publication               publicationInfo.title                publicationInfo.author.fullname publicationInfo.author.orcid
 #0  1,529 European ancestry cases, 3,399 European ...  False  False        NaN    None     True     False        None           GCST002305      False          False      [{'manufacturer': 'Illumina'}]  [{'type': 'replication', 'numberOfIndividuals'...  [{'genotypingTechnology': 'Genome-wide genotyp...  2,148 European ancestry cases, 1,309 European ...  Breast cancer (estrogen-receptor negative, pro...         24325915                    2013-12-09                    Carcinogenesis      Genome-wide association study identifies 25 kn...           Purrington KS              0000-0002-5710-1692    
 #1  8,602 European ancestry triple negative cases,...  False  False  9.700e+06       ~     True     False        None           GCST010100      False           True      [{'manufacturer': 'Illumina'}]  [{'type': 'initial', 'numberOfIndividuals': 11...  [{'genotypingTechnology': 'Genome-wide genotyp...                                                 NA  Breast cancer (estrogen-receptor negative, pro...         32424353                    2020-05-18                         Nat Genet      Genome-wide association study identifies 32 no...                 Zhang H                             None    
 #2                5,631 European ancestry individuals  False  False  1.000e+07    None     True     False        None         GCST90029052      False          False                                  []  [{'type': 'initial', 'numberOfIndividuals': 56...  [{'genotypingTechnology': 'Genome-wide genotyp...                                                 NA  15-year breast cancer-specific survival (ER ne...         34407845                    2021-08-18                 Breast Cancer Res      Association of germline genetic variants with ...                 Morra A                             None
```

### Comparing `pandasgwas-0.99.8/README.md` & `pandasgwas-0.99.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# pandasGWAS: a Python package to query, download and wrangle GWAS catalog data
+# pandasGWAS: a Python package for easy retrieval of GWAS catalog data
 ## Dependencies
 python: 3.8  
 pandas: 1.1.3  
 requests: 2.28.1  
 progressbar2: 4.0.0
 ## Documentation
 See [pandasGWAS Documentation](https://caotianze.github.io/pandasgwas/)
 ## Development Environment
 OS: Windows10 Professional  
 IDE: PyCharm 2022.1 (Community Edition)
 ## Installation
 `pip install pandasgwas`
 ## Example
+Get studies related to triple-negative breast cancer:
 ```Python
-# Get studies related to triple-negative breast cancer:
 from pandasgwas.get_studies import get_studies
 studies = get_studies(efo_trait = 'triple-negative breast cancer')
 studies.studies[0:4]
 #                  initialSampleSize                    gxe    gxg   snpCount  qualifier  imputed  pooled studyDesignComment  accessionId   fullPvalueSet  userRequested            platforms                                ancestries                                   genotypingTechnologies                             replicationSampleSize                                diseaseTrait.trait                 publicationInfo.pubmedId publicationInfo.publicationDate publicationInfo.publication               publicationInfo.title                publicationInfo.author.fullname publicationInfo.author.orcid
 #0  1,529 European ancestry cases, 3,399 European ...  False  False        NaN    None     True     False        None           GCST002305      False          False      [{'manufacturer': 'Illumina'}]  [{'type': 'replication', 'numberOfIndividuals'...  [{'genotypingTechnology': 'Genome-wide genotyp...  2,148 European ancestry cases, 1,309 European ...  Breast cancer (estrogen-receptor negative, pro...         24325915                    2013-12-09                    Carcinogenesis      Genome-wide association study identifies 25 kn...           Purrington KS              0000-0002-5710-1692    
 #1  8,602 European ancestry triple negative cases,...  False  False  9.700e+06       ~     True     False        None           GCST010100      False           True      [{'manufacturer': 'Illumina'}]  [{'type': 'initial', 'numberOfIndividuals': 11...  [{'genotypingTechnology': 'Genome-wide genotyp...                                                 NA  Breast cancer (estrogen-receptor negative, pro...         32424353                    2020-05-18                         Nat Genet      Genome-wide association study identifies 32 no...                 Zhang H                             None    
 #2                5,631 European ancestry individuals  False  False  1.000e+07    None     True     False        None         GCST90029052      False          False                                  []  [{'type': 'initial', 'numberOfIndividuals': 56...  [{'genotypingTechnology': 'Genome-wide genotyp...                                                 NA  15-year breast cancer-specific survival (ER ne...         34407845                    2021-08-18                 Breast Cancer Res      Association of germline genetic variants with ...                 Morra A                             None
```

### Comparing `pandasgwas-0.99.8/pandasgwas/Association.py` & `pandasgwas-0.99.9/pandasgwas/Association.py`

 * *Files identical despite different names*

### Comparing `pandasgwas-0.99.8/pandasgwas/Browser.py` & `pandasgwas-0.99.9/pandasgwas/Browser.py`

 * *Files identical despite different names*

### Comparing `pandasgwas-0.99.8/pandasgwas/SingleNucleotidePolymorphism.py` & `pandasgwas-0.99.9/pandasgwas/SingleNucleotidePolymorphism.py`

 * *Files identical despite different names*

### Comparing `pandasgwas-0.99.8/pandasgwas/Study.py` & `pandasgwas-0.99.9/pandasgwas/Study.py`

 * *Files identical despite different names*

### Comparing `pandasgwas-0.99.8/pandasgwas/Trait.py` & `pandasgwas-0.99.9/pandasgwas/Trait.py`

 * *Files identical despite different names*

### Comparing `pandasgwas-0.99.8/pandasgwas/client.py` & `pandasgwas-0.99.9/pandasgwas/client.py`

 * *Files identical despite different names*

### Comparing `pandasgwas-0.99.8/pandasgwas/cytogenetic_bands.csv` & `pandasgwas-0.99.9/pandasgwas/cytogenetic_bands.csv`

 * *Files identical despite different names*

### Comparing `pandasgwas-0.99.8/pandasgwas/get_SNPs.py` & `pandasgwas-0.99.9/pandasgwas/get_SNPs.py`

 * *Files identical despite different names*

### Comparing `pandasgwas-0.99.8/pandasgwas/get_associations.py` & `pandasgwas-0.99.9/pandasgwas/get_associations.py`

 * *Files identical despite different names*

### Comparing `pandasgwas-0.99.8/pandasgwas/get_studies.py` & `pandasgwas-0.99.9/pandasgwas/get_studies.py`

 * *Files identical despite different names*

### Comparing `pandasgwas-0.99.8/pandasgwas/get_traits.py` & `pandasgwas-0.99.9/pandasgwas/get_traits.py`

 * *Files identical despite different names*

### Comparing `pandasgwas-0.99.8/pandasgwas/set_operation.py` & `pandasgwas-0.99.9/pandasgwas/set_operation.py`

 * *Files identical despite different names*

### Comparing `pandasgwas-0.99.8/pandasgwas.egg-info/PKG-INFO` & `pandasgwas-0.99.9/pandasgwas.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: pandasgwas
-Version: 0.99.8
-Summary: A Python package to query, download and wrangle GWAS catalog data
+Version: 0.99.9
+Summary: A Python package for easy retrieval of GWAS catalog data
 Home-page: https://github.com/caotianze/pandasgwas
 Author: Cao Tianze
 Author-email: hnrcao@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/caotianze/pandasgwas/issues
-Keywords: GWAS pandas
+Keywords: gwas,genomics,snp,bioinformatics,pandas
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# pandasGWAS: a Python package to query, download and wrangle GWAS catalog data
+# pandasGWAS: a Python package for easy retrieval of GWAS catalog data
 ## Dependencies
 python: 3.8  
 pandas: 1.1.3  
 requests: 2.28.1  
 progressbar2: 4.0.0
 ## Documentation
 See [pandasGWAS Documentation](https://caotianze.github.io/pandasgwas/)
 ## Development Environment
 OS: Windows10 Professional  
 IDE: PyCharm 2022.1 (Community Edition)
 ## Installation
 `pip install pandasgwas`
 ## Example
+Get studies related to triple-negative breast cancer:
 ```Python
-# Get studies related to triple-negative breast cancer:
 from pandasgwas.get_studies import get_studies
 studies = get_studies(efo_trait = 'triple-negative breast cancer')
 studies.studies[0:4]
 #                  initialSampleSize                    gxe    gxg   snpCount  qualifier  imputed  pooled studyDesignComment  accessionId   fullPvalueSet  userRequested            platforms                                ancestries                                   genotypingTechnologies                             replicationSampleSize                                diseaseTrait.trait                 publicationInfo.pubmedId publicationInfo.publicationDate publicationInfo.publication               publicationInfo.title                publicationInfo.author.fullname publicationInfo.author.orcid
 #0  1,529 European ancestry cases, 3,399 European ...  False  False        NaN    None     True     False        None           GCST002305      False          False      [{'manufacturer': 'Illumina'}]  [{'type': 'replication', 'numberOfIndividuals'...  [{'genotypingTechnology': 'Genome-wide genotyp...  2,148 European ancestry cases, 1,309 European ...  Breast cancer (estrogen-receptor negative, pro...         24325915                    2013-12-09                    Carcinogenesis      Genome-wide association study identifies 25 kn...           Purrington KS              0000-0002-5710-1692    
 #1  8,602 European ancestry triple negative cases,...  False  False  9.700e+06       ~     True     False        None           GCST010100      False           True      [{'manufacturer': 'Illumina'}]  [{'type': 'initial', 'numberOfIndividuals': 11...  [{'genotypingTechnology': 'Genome-wide genotyp...                                                 NA  Breast cancer (estrogen-receptor negative, pro...         32424353                    2020-05-18                         Nat Genet      Genome-wide association study identifies 32 no...                 Zhang H                             None    
 #2                5,631 European ancestry individuals  False  False  1.000e+07    None     True     False        None         GCST90029052      False          False                                  []  [{'type': 'initial', 'numberOfIndividuals': 56...  [{'genotypingTechnology': 'Genome-wide genotyp...                                                 NA  15-year breast cancer-specific survival (ER ne...         34407845                    2021-08-18                 Breast Cancer Res      Association of germline genetic variants with ...                 Morra A                             None
```

### Comparing `pandasgwas-0.99.8/pandasgwas.egg-info/SOURCES.txt` & `pandasgwas-0.99.9/pandasgwas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pandasgwas-0.99.8/setup.py` & `pandasgwas-0.99.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pandasgwas",
-    version="0.99.8",
+    version="0.99.9",
     author="Cao Tianze",
     author_email="hnrcao@qq.com",
-    description="A Python package to query, download and wrangle GWAS catalog data",
+    description="A Python package for easy retrieval of GWAS catalog data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/caotianze/pandasgwas",
     project_urls={
         "Bug Tracker": "https://github.com/caotianze/pandasgwas/issues",
     },
     classifiers=[
@@ -23,12 +23,12 @@
         "Operating System :: OS Independent",
     ],
     # package_dir={"": "pandasgwas"},
     packages=['pandasgwas'],
     python_requires=">=3.8",
     install_requires=['pandas>=1.1.3, <=1.2.5', 'requests>=2.28.1', 'progressbar2>=4.0.0'],
     license="MIT",
-    keywords="GWAS pandas",
+    keywords=['gwas', 'genomics', 'snp', 'bioinformatics','pandas'],
     package_data={
         "": ["*.csv"]
     }
 )
```

