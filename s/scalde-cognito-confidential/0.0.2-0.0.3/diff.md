# Comparing `tmp/scalde_cognito_confidential-0.0.2-py3-none-any.whl.zip` & `tmp/scalde_cognito_confidential-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 7147 bytes, number of entries: 13
--rw-r--r--  2.0 unx      573 b- defN 23-Apr-15 15:01 cognito_confidential/__init__.py
--rw-r--r--  2.0 unx     3265 b- defN 23-Apr-15 15:01 cognito_confidential/authentications.py
--rw-r--r--  2.0 unx     1847 b- defN 23-Apr-15 15:01 cognito_confidential/clients.py
--rw-r--r--  2.0 unx      272 b- defN 23-Apr-15 15:01 cognito_confidential/config.py
--rw-r--r--  2.0 unx      176 b- defN 23-Apr-15 15:01 cognito_confidential/exceptions.py
--rw-r--r--  2.0 unx      532 b- defN 23-Apr-15 15:01 cognito_confidential/models.py
--rw-r--r--  2.0 unx     2420 b- defN 23-Apr-15 15:01 cognito_confidential/parsers.py
--rw-r--r--  2.0 unx     1065 b- defN 23-Apr-15 15:01 cognito_confidential/stores.py
--rw-r--r--  2.0 unx     2529 b- defN 23-Apr-15 15:01 cognito_confidential/validations.py
--rw-r--r--  2.0 unx      558 b- defN 23-Apr-15 15:01 scalde_cognito_confidential-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-15 15:01 scalde_cognito_confidential-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       26 b- defN 23-Apr-15 15:01 scalde_cognito_confidential-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1178 b- defN 23-Apr-15 15:01 scalde_cognito_confidential-0.0.2.dist-info/RECORD
-13 files, 14533 bytes uncompressed, 5137 bytes compressed:  64.7%
+Zip file size: 7156 bytes, number of entries: 13
+-rw-rw-r--  2.0 unx      573 b- defN 23-Apr-15 15:18 cognito_confidential/__init__.py
+-rw-rw-r--  2.0 unx     3265 b- defN 23-Apr-15 15:18 cognito_confidential/authentications.py
+-rw-rw-r--  2.0 unx     1847 b- defN 23-Apr-15 15:18 cognito_confidential/clients.py
+-rw-rw-r--  2.0 unx      272 b- defN 23-Apr-15 15:18 cognito_confidential/config.py
+-rw-rw-r--  2.0 unx      176 b- defN 23-Apr-15 15:18 cognito_confidential/exceptions.py
+-rw-rw-r--  2.0 unx      532 b- defN 23-Apr-15 15:18 cognito_confidential/models.py
+-rw-rw-r--  2.0 unx     2420 b- defN 23-Apr-15 15:18 cognito_confidential/parsers.py
+-rw-rw-r--  2.0 unx     1065 b- defN 23-Apr-15 15:18 cognito_confidential/stores.py
+-rw-rw-r--  2.0 unx     2529 b- defN 23-Apr-15 15:18 cognito_confidential/validations.py
+-rw-rw-r--  2.0 unx      588 b- defN 23-Apr-15 15:18 scalde_cognito_confidential-0.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-15 15:18 scalde_cognito_confidential-0.0.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       26 b- defN 23-Apr-15 15:18 scalde_cognito_confidential-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1178 b- defN 23-Apr-15 15:18 scalde_cognito_confidential-0.0.3.dist-info/RECORD
+13 files, 14563 bytes uncompressed, 5146 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: cognito_confidential/stores.py
 Comment: 
 
 Filename: cognito_confidential/validations.py
 Comment: 
 
-Filename: scalde_cognito_confidential-0.0.2.dist-info/METADATA
+Filename: scalde_cognito_confidential-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: scalde_cognito_confidential-0.0.2.dist-info/WHEEL
+Filename: scalde_cognito_confidential-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: scalde_cognito_confidential-0.0.2.dist-info/top_level.txt
+Filename: scalde_cognito_confidential-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: scalde_cognito_confidential-0.0.2.dist-info/RECORD
+Filename: scalde_cognito_confidential-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `scalde_cognito_confidential-0.0.2.dist-info/METADATA` & `scalde_cognito_confidential-0.0.3.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: scalde-cognito-confidential
-Version: 0.0.2
+Version: 0.0.3
 Summary: AWS Cognito client library for confidential clients
 Author-email: Thomas Marquis <thomas.marquis.dev@gmail.com>
 Keywords: security,aws,cognito,oicd
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: requests (>=2.28.2)
 Requires-Dist: python-jose[cryptography] (>=3.3.0)
 Requires-Dist: authlib (>=1.2.0)
 
+# scalde-cognito-confidential
```

## Comparing `scalde_cognito_confidential-0.0.2.dist-info/RECORD` & `scalde_cognito_confidential-0.0.3.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -3,11 +3,11 @@
 cognito_confidential/clients.py,sha256=NT0V8lZhgBDf_SkiM4ZGS9sskBmMW6ISPokrzvnn1RU,1847
 cognito_confidential/config.py,sha256=f69FJTurtNDvQ8QOB6lVjJnNVNLt924e_Nf6VdnI7tc,272
 cognito_confidential/exceptions.py,sha256=97iKaoi7O2x09q2ezpdrBloK2n5W6cuO3NNx8Kl8NvI,176
 cognito_confidential/models.py,sha256=l_tTwZpu-4xj0iGYjYTLxhGkBIYxU0y0GPBZzfD7IAI,532
 cognito_confidential/parsers.py,sha256=OsEjxC6BdH6FWrAwhmDsOOKuU3uWCtEYdUDzjrbJouQ,2420
 cognito_confidential/stores.py,sha256=pXiW1WHj3qoTz8HiEA28j8L-hfgFv9V5B-f143eaha0,1065
 cognito_confidential/validations.py,sha256=ZJE6CyqzKaAV6kFppsiwMoVbDRDzIgmf0qm69_w4b_k,2529
-scalde_cognito_confidential-0.0.2.dist-info/METADATA,sha256=-KW2JUilkOJlVFSR5qeL3Ez5NKpk0Db4ikjeMW4aKPw,558
-scalde_cognito_confidential-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-scalde_cognito_confidential-0.0.2.dist-info/top_level.txt,sha256=ZxDEYiuaeQKPxrRU4zr9RvSYUEtxr4rY9W-dSvjHOM4,26
-scalde_cognito_confidential-0.0.2.dist-info/RECORD,,
+scalde_cognito_confidential-0.0.3.dist-info/METADATA,sha256=ny2YO1RcxfU30NdgP7smQomFu-fKQbvzVlhjOMwz6-c,588
+scalde_cognito_confidential-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+scalde_cognito_confidential-0.0.3.dist-info/top_level.txt,sha256=ZxDEYiuaeQKPxrRU4zr9RvSYUEtxr4rY9W-dSvjHOM4,26
+scalde_cognito_confidential-0.0.3.dist-info/RECORD,,
```

