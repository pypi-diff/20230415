# Comparing `tmp/pvrpm-1.8.0-py3-none-any.whl.zip` & `tmp/pvrpm-1.8.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 44550 bytes, number of entries: 20
+Zip file size: 44523 bytes, number of entries: 20
 -rw-r--r--  2.0 unx      126 b- defN 22-Jun-07 22:01 pvrpm/__init__.py
 -rw-r--r--  2.0 unx     3505 b- defN 22-Oct-26 05:54 pvrpm/__main__.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Feb-23 20:23 pvrpm/core/__init__.py
--rw-r--r--  2.0 unx    37912 b- defN 23-Feb-16 18:51 pvrpm/core/case.py
+-rw-r--r--  2.0 unx    37893 b- defN 23-Apr-14 23:10 pvrpm/core/case.py
 -rw-r--r--  2.0 unx    23148 b- defN 22-Oct-26 06:00 pvrpm/core/components.py
 -rw-r--r--  2.0 unx     4700 b- defN 22-Jun-07 22:01 pvrpm/core/enums.py
 -rw-r--r--  2.0 unx       37 b- defN 22-Jun-07 22:02 pvrpm/core/exceptions.py
 -rw-r--r--  2.0 unx      397 b- defN 22-Jun-07 22:02 pvrpm/core/logger.py
 -rw-r--r--  2.0 unx    37465 b- defN 22-Oct-26 07:25 pvrpm/core/simulation.py
 -rw-r--r--  2.0 unx    10732 b- defN 22-Oct-26 07:25 pvrpm/core/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Feb-23 20:23 pvrpm/core/modules/__init__.py
 -rw-r--r--  2.0 unx    22847 b- defN 22-Oct-26 07:25 pvrpm/core/modules/failure.py
 -rw-r--r--  2.0 unx    17755 b- defN 22-Jun-07 22:02 pvrpm/core/modules/monitor.py
 -rw-r--r--  2.0 unx    12897 b- defN 22-Oct-26 07:25 pvrpm/core/modules/repair.py
--rw-r--r--  2.0 unx     1512 b- defN 23-Feb-16 19:16 pvrpm-1.8.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1941 b- defN 23-Feb-16 19:16 pvrpm-1.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-16 19:16 pvrpm-1.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-Feb-16 19:16 pvrpm-1.8.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Feb-16 19:16 pvrpm-1.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1583 b- defN 23-Feb-16 19:16 pvrpm-1.8.0.dist-info/RECORD
-20 files, 176701 bytes uncompressed, 41994 bytes compressed:  76.2%
+-rw-r--r--  2.0 unx     1512 b- defN 23-Apr-14 23:13 pvrpm-1.8.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1931 b- defN 23-Apr-14 23:13 pvrpm-1.8.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 23:13 pvrpm-1.8.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-Apr-14 23:13 pvrpm-1.8.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Apr-14 23:13 pvrpm-1.8.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1583 b- defN 23-Apr-14 23:13 pvrpm-1.8.1.dist-info/RECORD
+20 files, 176672 bytes uncompressed, 41967 bytes compressed:  76.2%
```

## zipnote {}

```diff
@@ -36,26 +36,26 @@
 
 Filename: pvrpm/core/modules/monitor.py
 Comment: 
 
 Filename: pvrpm/core/modules/repair.py
 Comment: 
 
-Filename: pvrpm-1.8.0.dist-info/LICENSE
+Filename: pvrpm-1.8.1.dist-info/LICENSE
 Comment: 
 
-Filename: pvrpm-1.8.0.dist-info/METADATA
+Filename: pvrpm-1.8.1.dist-info/METADATA
 Comment: 
 
-Filename: pvrpm-1.8.0.dist-info/WHEEL
+Filename: pvrpm-1.8.1.dist-info/WHEEL
 Comment: 
 
-Filename: pvrpm-1.8.0.dist-info/entry_points.txt
+Filename: pvrpm-1.8.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: pvrpm-1.8.0.dist-info/top_level.txt
+Filename: pvrpm-1.8.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pvrpm-1.8.0.dist-info/RECORD
+Filename: pvrpm-1.8.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pvrpm/core/case.py

```diff
@@ -605,15 +605,15 @@
         """
         try:
             return self.output("npv")
         except AttributeError:
             pass
 
         try:
-            return np.array(self.output("cf_project_return_aftertax_npv")).sum()
+            return self.output("project_return_aftertax_npv")
         except AttributeError:
             pass
 
         try:
             return self.output("tax_investor_aftertax_npv")
         except AttributeError:
             return None
```

## Comparing `pvrpm-1.8.0.dist-info/LICENSE` & `pvrpm-1.8.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pvrpm-1.8.0.dist-info/METADATA` & `pvrpm-1.8.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvrpm
-Version: 1.8.0
+Version: 1.8.1
 Summary: Run simulations to estimate LCOE costs for PV systems using SAM.
 Home-page: https://github.com/FSEC-Photovoltaics/pvrpm-lcoe
 Author: ['Brandon Silva', 'Paul Lunis']
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nrel-pysam (==4.0.0)
@@ -26,15 +26,15 @@
 [![Tests](https://github.com/FSEC-Photovoltaics/pvrpm-lcoe/actions/workflows/tests.yml/badge.svg?branch=master&event=push)](https://github.com/FSEC-Photovoltaics/pvrpm-lcoe/actions/workflows/tests.yml) [![black-checker](https://github.com/FSEC-Photovoltaics/pvrpm-lcoe/actions/workflows/black-checker.yml/badge.svg)](https://github.com/FSEC-Photovoltaics/pvrpm-lcoe/actions/workflows/black-checker.yml)
 
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.04093/status.svg)](https://doi.org/10.21105/joss.04093)
 
 ---
 
 ### Quick Reference
-[Documentation](https://pvrpm.readthedocs.io/en/latest/)
+[Documentation](https://pvrpm.readthedocs.io/)
 
 [License](LICENSE)
 
 [Issues](https://github.com/FSEC-Photovoltaics/pvrpm-lcoe/issues/)
 
 [Contributing Guide](.github/CONTRIBUTING.md)
```

## Comparing `pvrpm-1.8.0.dist-info/RECORD` & `pvrpm-1.8.1.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 pvrpm/__init__.py,sha256=zbgjXCXQdapflfiKKLMBcgKKrdRGylqNgDfhURO9zmI,126
 pvrpm/__main__.py,sha256=K7JQRPZTEzAv9Q2ZSfeue9pE9dnjji5kA7DiC06ExNQ,3505
 pvrpm/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pvrpm/core/case.py,sha256=2naSLiFBdbPQ0aoGNsDZBlRW-QdHRq8PFWJXWprszh8,37912
+pvrpm/core/case.py,sha256=W4Rzlsen21UI_obCyLzJfNaX2MgDJD3GmNtTCwIoatM,37893
 pvrpm/core/components.py,sha256=XwLmSrwwPkgxLJf1ihYu8HMyn7jDi2zPQT8Gols6zSI,23148
 pvrpm/core/enums.py,sha256=SqPFb1kbo7FzbhGBth46bm-8I-HV-h0s4u8KDnlZ7mA,4700
 pvrpm/core/exceptions.py,sha256=RLWj_CWV1xLNYSGRHs0lXwuuBoQjVcAnJBg2FrabFXA,37
 pvrpm/core/logger.py,sha256=Rp4wG76Jo9rBohNmV6Ae7xMszxLZzIUJenNWm7pvH8w,397
 pvrpm/core/simulation.py,sha256=is2o8f7M5Kc_1LObF6z8bJCa2LfhN_TCF926ix-sQ0o,37465
 pvrpm/core/utils.py,sha256=6eCTmGy494UFkd5MbyS1jLhLujiyvhpU0si5oK0TyRI,10732
 pvrpm/core/modules/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pvrpm/core/modules/failure.py,sha256=ZIBUu7HffCe49DajAVQzbCJxur0T5k6jDgi7XSRez2Y,22847
 pvrpm/core/modules/monitor.py,sha256=5gRf2nDDImsSBo3PFhGAX2CWCpdytRW4mim3GALa4b8,17755
 pvrpm/core/modules/repair.py,sha256=5l1jARmshdgPG4B_K-fSkB4RmzYBqsUGQI5TYvHmrmU,12897
-pvrpm-1.8.0.dist-info/LICENSE,sha256=bcPdSA0J0Ot6Rf9a8JzbQiuInEwqgI7IRg3zgO8XN00,1512
-pvrpm-1.8.0.dist-info/METADATA,sha256=hqoxAYHF_FbaG_5rHfXm2F_4fCe07aAoDmJuhWtOGcE,1941
-pvrpm-1.8.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pvrpm-1.8.0.dist-info/entry_points.txt,sha256=dNFVdNQOolsGC4axg8zLK32-gP4_qQw4JH_bQQJNh5c,46
-pvrpm-1.8.0.dist-info/top_level.txt,sha256=G1BC0evGjHwL5iyYC0V68SX7OpmDWgS4soVddNpNTHU,6
-pvrpm-1.8.0.dist-info/RECORD,,
+pvrpm-1.8.1.dist-info/LICENSE,sha256=bcPdSA0J0Ot6Rf9a8JzbQiuInEwqgI7IRg3zgO8XN00,1512
+pvrpm-1.8.1.dist-info/METADATA,sha256=W17-SiE4uYY3GkcmbQM88HyzM9wgjCl2DWR3wHO8Qpg,1931
+pvrpm-1.8.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pvrpm-1.8.1.dist-info/entry_points.txt,sha256=dNFVdNQOolsGC4axg8zLK32-gP4_qQw4JH_bQQJNh5c,46
+pvrpm-1.8.1.dist-info/top_level.txt,sha256=G1BC0evGjHwL5iyYC0V68SX7OpmDWgS4soVddNpNTHU,6
+pvrpm-1.8.1.dist-info/RECORD,,
```

