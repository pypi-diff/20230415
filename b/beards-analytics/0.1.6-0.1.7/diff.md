# Comparing `tmp/beards_analytics-0.1.6-py3-none-any.whl.zip` & `tmp/beards_analytics-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 10182 bytes, number of entries: 20
--rw-r--r--  2.0 unx       22 b- defN 23-Apr-15 15:06 beards_analytics/__init__.py
+Zip file size: 10179 bytes, number of entries: 20
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-15 15:35 beards_analytics/__init__.py
 -rw-r--r--  2.0 unx       19 b- defN 23-Apr-15 14:34 beards_analytics/cloud_functions/__init__.py
 -rw-r--r--  2.0 unx     3087 b- defN 23-Apr-15 14:45 beards_analytics/cloud_functions/http.py
 -rw-r--r--  2.0 unx       51 b- defN 23-Apr-15 14:30 beards_analytics/common/__init__.py
 -rw-r--r--  2.0 unx      847 b- defN 23-Apr-11 15:43 beards_analytics/common/date.py
 -rw-r--r--  2.0 unx     3008 b- defN 23-Apr-15 14:29 beards_analytics/common/logger.py
 -rw-r--r--  2.0 unx     1342 b- defN 23-Apr-15 14:43 beards_analytics/common/tasks.py
 -rw-r--r--  2.0 unx       82 b- defN 23-Apr-14 14:04 beards_analytics/common/types.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-30 11:18 beards_analytics/data/__init__.py
 -rw-r--r--  2.0 unx      514 b- defN 23-Apr-11 13:34 beards_analytics/data/models.py
 -rw-r--r--  2.0 unx      782 b- defN 23-Apr-14 21:27 beards_analytics/data/operations.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 21:32 beards_analytics/public_api/__init__.py
 -rw-r--r--  2.0 unx     2846 b- defN 23-Apr-15 14:17 beards_analytics/public_api/_metadata.py
--rw-r--r--  2.0 unx     2174 b- defN 23-Apr-15 15:05 beards_analytics/public_api/client.py
+-rw-r--r--  2.0 unx     2135 b- defN 23-Apr-15 15:34 beards_analytics/public_api/client.py
 -rw-r--r--  2.0 unx      202 b- defN 23-Apr-14 20:48 beards_analytics/public_api/models.py
--rw-r--r--  2.0 unx     1060 b- defN 23-Apr-15 15:06 beards_analytics-0.1.6.dist-info/LICENCE.txt
--rw-r--r--  2.0 unx      731 b- defN 23-Apr-15 15:06 beards_analytics-0.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-15 15:06 beards_analytics-0.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Apr-15 15:06 beards_analytics-0.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1798 b- defN 23-Apr-15 15:06 beards_analytics-0.1.6.dist-info/RECORD
-20 files, 18674 bytes uncompressed, 7170 bytes compressed:  61.6%
+-rw-r--r--  2.0 unx     1060 b- defN 23-Apr-15 15:36 beards_analytics-0.1.7.dist-info/LICENCE.txt
+-rw-r--r--  2.0 unx      731 b- defN 23-Apr-15 15:36 beards_analytics-0.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-15 15:36 beards_analytics-0.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Apr-15 15:36 beards_analytics-0.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1798 b- defN 23-Apr-15 15:36 beards_analytics-0.1.7.dist-info/RECORD
+20 files, 18635 bytes uncompressed, 7167 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: beards_analytics/public_api/client.py
 Comment: 
 
 Filename: beards_analytics/public_api/models.py
 Comment: 
 
-Filename: beards_analytics-0.1.6.dist-info/LICENCE.txt
+Filename: beards_analytics-0.1.7.dist-info/LICENCE.txt
 Comment: 
 
-Filename: beards_analytics-0.1.6.dist-info/METADATA
+Filename: beards_analytics-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: beards_analytics-0.1.6.dist-info/WHEEL
+Filename: beards_analytics-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: beards_analytics-0.1.6.dist-info/top_level.txt
+Filename: beards_analytics-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: beards_analytics-0.1.6.dist-info/RECORD
+Filename: beards_analytics-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## beards_analytics/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.1.6'
+__version__ = '0.1.7'
```

## beards_analytics/public_api/client.py

```diff
@@ -21,15 +21,15 @@
                 
         if self._credentials.expired or not self._credentials.token:
             self._credentials.refresh(GoogleRequest())
             
         res = requests.request(method, self._url_base + endpoint, json=json, params=params, headers={'x-id-token': self._credentials.token})
         
         if res.status_code == 403:
-            raise GoogleAuthError('Failed to authorise BA public API service (403)')
+            raise GoogleAuthError(res.json())
         
         if res.status_code >= 500:
             raise RuntimeWarning('Failed to use a BA service. Please report the issue to developers of Beards Analytics.')
         
         return res.json()
     
     def create_cloud_log(self, log_name: str, message: str, severity: LogSeverity, k_service: str, project_id: Optional[str] = None, labels: Optional[Mapping[str, str]] = None, extra: Optional[Any] = None):
```

## Comparing `beards_analytics-0.1.6.dist-info/LICENCE.txt` & `beards_analytics-0.1.7.dist-info/LICENCE.txt`

 * *Files identical despite different names*

## Comparing `beards_analytics-0.1.6.dist-info/METADATA` & `beards_analytics-0.1.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beards-analytics
-Version: 0.1.6
+Version: 0.1.7
 Summary: Beards Analytics packages
 Home-page: https://beardsanalytics.com
 Author: Beards Analytics
 Author-email: tz@or.com.ua
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `beards_analytics-0.1.6.dist-info/RECORD` & `beards_analytics-0.1.7.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-beards_analytics/__init__.py,sha256=gW5NUxwGdPsiQjn0cOuuQT11pfthByI5DITDg_HMhLQ,22
+beards_analytics/__init__.py,sha256=mFY0GwwuN-a3M8w93_mskS6GZIvv9SNdjLfJaWNsm-I,22
 beards_analytics/cloud_functions/__init__.py,sha256=VmjSBaoSqXDln4jRE0CLkl_3OHZSs7hhNWcKx2B77hY,19
 beards_analytics/cloud_functions/http.py,sha256=JMIPreFkfLdLLmHKPbPrZbJVwro_-iqAtWOUxJXXVYo,3087
 beards_analytics/common/__init__.py,sha256=NeB4cKiZbcqp0STfAXFSD4iJ3DhoWxFFamzES17ldA4,51
 beards_analytics/common/date.py,sha256=amLlla8Smayw8ZnEAS0lJebusnIaBBAdxA0u-h_tl7M,847
 beards_analytics/common/logger.py,sha256=gX0EdwwGXVbMoxYpHgFvJfuRVVJUAUyzDGFLaRoVpyo,3008
 beards_analytics/common/tasks.py,sha256=AtqrXtAGLQglvZ_F-jiiO7QBE1gLmaTOs-QAfvkaM8w,1342
 beards_analytics/common/types.py,sha256=xZytT7TyUMhpYvYjlAPQd5mcn56nn6npq_EcEPF3Hs4,82
 beards_analytics/data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 beards_analytics/data/models.py,sha256=79oHvRbMaWTz_o1GK2dIqL6Uh2cIIVbnel4JcxUkHxk,514
 beards_analytics/data/operations.py,sha256=QwIoW6LXlhAVH7RGM8xkW7DgC7qAD1De_1sulm_zBLU,782
 beards_analytics/public_api/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 beards_analytics/public_api/_metadata.py,sha256=J_DTAsBfsssGvp09MY9y_pUQQqpbdVpwOE_H2RFJZh0,2846
-beards_analytics/public_api/client.py,sha256=URxNsBLlNu5Npz4BMpOqRSn5KpHrV1ushNgIDcMXWA0,2174
+beards_analytics/public_api/client.py,sha256=7ju-k8wfKzom-EjfpodakzGvcC8OyjfprhHCgIpJ2Nk,2135
 beards_analytics/public_api/models.py,sha256=E4CLlm9ddN3r5w1S-GDmxBGLbWhStNJG85u-jgBXZUk,202
-beards_analytics-0.1.6.dist-info/LICENCE.txt,sha256=ffCT6E6aOB-bR3LUuUAjS9TRLU8XHZJMf9Y37cnwYaU,1060
-beards_analytics-0.1.6.dist-info/METADATA,sha256=zt05UobG6ghYnUpPJDh5d6d_TSgszLRjiZHpqkxSJUA,731
-beards_analytics-0.1.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-beards_analytics-0.1.6.dist-info/top_level.txt,sha256=d1eTQ99gRKVHzIDAHRUTj17UqgawtQWbIf2vA7AdtW4,17
-beards_analytics-0.1.6.dist-info/RECORD,,
+beards_analytics-0.1.7.dist-info/LICENCE.txt,sha256=ffCT6E6aOB-bR3LUuUAjS9TRLU8XHZJMf9Y37cnwYaU,1060
+beards_analytics-0.1.7.dist-info/METADATA,sha256=wQplmTRVk2SS8bxSioEfrG-aTNX5OvWAEQDyslydp3A,731
+beards_analytics-0.1.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+beards_analytics-0.1.7.dist-info/top_level.txt,sha256=d1eTQ99gRKVHzIDAHRUTj17UqgawtQWbIf2vA7AdtW4,17
+beards_analytics-0.1.7.dist-info/RECORD,,
```

