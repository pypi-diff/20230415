# Comparing `tmp/hfmirror-0.0.2.tar.gz` & `tmp/hfmirror-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hfmirror-0.0.2.tar", last modified: Fri Apr 14 14:54:03 2023, max compression
+gzip compressed data, was "hfmirror-0.0.3.tar", last modified: Sat Apr 15 11:27:23 2023, max compression
```

## Comparing `hfmirror-0.0.2.tar` & `hfmirror-0.0.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:54:03.289446 hfmirror-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-14 14:53:30.000000 hfmirror-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-14 14:53:30.000000 hfmirror-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-04-14 14:54:03.289446 hfmirror-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-04-14 14:53:30.000000 hfmirror-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:54:03.285446 hfmirror-0.0.2/hfmirror/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:54:03.285446 hfmirror-0.0.2/hfmirror/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:54:03.285446 hfmirror-0.0.2/hfmirror/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/resource/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/resource/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/resource/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/resource/sourceforge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/resource/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:54:03.285446 hfmirror-0.0.2/hfmirror/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/storage/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/storage/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:54:03.285446 hfmirror-0.0.2/hfmirror/sync/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/sync/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:54:03.289446 hfmirror-0.0.2/hfmirror/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/utils/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/utils/segments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/utils/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/utils/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:54:03.285446 hfmirror-0.0.2/hfmirror.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-04-14 14:54:03.000000 hfmirror-0.0.2/hfmirror.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-14 14:54:03.000000 hfmirror-0.0.2/hfmirror.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 14:54:03.000000 hfmirror-0.0.2/hfmirror.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-14 14:54:03.000000 hfmirror-0.0.2/hfmirror.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 14:54:03.000000 hfmirror-0.0.2/hfmirror.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-14 14:53:30.000000 hfmirror-0.0.2/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-14 14:53:30.000000 hfmirror-0.0.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-14 14:53:30.000000 hfmirror-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 14:54:03.289446 hfmirror-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-14 14:53:30.000000 hfmirror-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:27:23.290458 hfmirror-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-15 11:26:43.000000 hfmirror-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-15 11:26:43.000000 hfmirror-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-04-15 11:27:23.290458 hfmirror-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-04-15 11:26:43.000000 hfmirror-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:27:23.290458 hfmirror-0.0.3/hfmirror/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:27:23.290458 hfmirror-0.0.3/hfmirror/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:27:23.290458 hfmirror-0.0.3/hfmirror/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/resource/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/resource/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/resource/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/resource/sourceforge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/resource/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:27:23.290458 hfmirror-0.0.3/hfmirror/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/storage/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/storage/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:27:23.290458 hfmirror-0.0.3/hfmirror/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/sync/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:27:23.290458 hfmirror-0.0.3/hfmirror/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/utils/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/utils/segments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/utils/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-15 11:26:43.000000 hfmirror-0.0.3/hfmirror/utils/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:27:23.290458 hfmirror-0.0.3/hfmirror.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-04-15 11:27:23.000000 hfmirror-0.0.3/hfmirror.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-15 11:27:23.000000 hfmirror-0.0.3/hfmirror.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 11:27:23.000000 hfmirror-0.0.3/hfmirror.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-15 11:27:23.000000 hfmirror-0.0.3/hfmirror.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-15 11:27:23.000000 hfmirror-0.0.3/hfmirror.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-15 11:26:43.000000 hfmirror-0.0.3/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-15 11:26:43.000000 hfmirror-0.0.3/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-15 11:26:43.000000 hfmirror-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 11:27:23.290458 hfmirror-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-15 11:26:43.000000 hfmirror-0.0.3/setup.py
```

### Comparing `hfmirror-0.0.2/LICENSE` & `hfmirror-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.2/PKG-INFO` & `hfmirror-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfmirror
-Version: 0.0.2
+Version: 0.0.3
 Summary: Mirror for resources to local and huggingface.
 Home-page: https://github.com/narugo1992/hfmirror
 Author: narugo1992
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: A simple tool for automatic parameter tuning.
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hfmirror-0.0.2/README.md` & `hfmirror-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.2/hfmirror/resource/github.py` & `hfmirror-0.0.3/hfmirror/resource/github.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.2/hfmirror/resource/item.py` & `hfmirror-0.0.3/hfmirror/resource/item.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,64 +35,72 @@
         return hash_anything((type(self), self._value, self.metadata, self.segments))
 
     def __eq__(self, other):
         if self is other:
             return True
         elif isinstance(self, type(other)) and isinstance(other, type(self)):
             return (self._value, self.metadata, self.segments) == \
-                   (other._value, other.metadata, other.segments)
+                (other._value, other.metadata, other.segments)
         else:
             return False
 
 
 class RemoteSyncItem(SyncItem):
     __type__ = 'remote'
     __headers__ = {}
+    __request_kwargs__ = {}
 
     def __init__(self, url, metadata, segments: List[str]):
         SyncItem.__init__(self, url, metadata, segments)
         self.url = url
         self._session = None
 
+    def get_new_session(self):
+        return get_requests_session(headers=self.__headers__)
+
     def _get_session(self) -> requests.Session:
         if self._session is None:
-            self._session = get_requests_session(headers=self.__headers__)
+            self._session = self.get_new_session()
 
         return self._session
 
     def _file_process(self, filename):
         pass
 
     @contextmanager
     def load_file(self) -> ContextManager[str]:
         with TemporaryDirectory() as td:
             filename = os.path.join(td, urlsplit(self.url).filename or 'unnamed_file')
-            download_file(self.url, filename, session=self._session)
+            download_file(self.url, filename, session=self._get_session(), **self.__request_kwargs__)
             self._file_process(filename)
             yield filename
 
     def refresh_mark(self, mark: Optional[Dict[str, Any]]):
         mark = dict(mark or {})
         url = mark.get('url')
         if url == self.url:  # url not changed
             expires = mark.get('expires')
             if expires is not None and time.time() < expires:
                 raise ResourceNotChange
 
             etag = mark.get('etag')
-            resp = srequest(
-                self._get_session(), 'HEAD', self.url,
-                allow_redirects=True, headers={'If-None-Match': etag} if etag else {}
-            )
+            headers = {'If-None-Match': etag} if etag else {}
         else:
-            resp = srequest(
-                self._get_session(), 'HEAD', self.url,
-                allow_redirects=True, headers={}
-            )
+            headers = {}
 
+        kwargs = self.__request_kwargs__.copy()
+        if 'headers' in kwargs:
+            headers.update(kwargs['headers'])
+            kwargs.pop('headers')
+
+        resp = srequest(
+            self._get_session(), 'HEAD', self.url,
+            allow_redirects=True, headers=headers,
+            **kwargs
+        )
         if resp.status_code == 304:
             raise ResourceNotChange
 
         headers = resp.headers
         etag = headers.get('ETag')
         expires = headers.get('Expires')
         expires = parsedate_to_datetime(expires).timestamp() if expires else None
```

### Comparing `hfmirror-0.0.2/hfmirror/resource/resource.py` & `hfmirror-0.0.3/hfmirror/resource/resource.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.2/hfmirror/resource/sourceforge.py` & `hfmirror-0.0.3/hfmirror/resource/sourceforge.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.2/hfmirror/resource/version.py` & `hfmirror-0.0.3/hfmirror/resource/version.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.2/hfmirror/storage/base.py` & `hfmirror-0.0.3/hfmirror/storage/base.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.2/hfmirror/storage/huggingface.py` & `hfmirror-0.0.3/hfmirror/storage/huggingface.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,17 @@
     :param repo_id: Repository id, the same as that in huggingface library.
     :param repo_type: Repository type, the same as that in huggingface library.
     :param revision: Revision of repository, the same as that in huggingface library.
     :param chunk_for_hash: Chunk size for hashing calculation.
     :param session: Session of requests, will be auto created when not given.
     :return: Uploads are necessary or not, in form of lists of boolean.
     """
+    if not uploads:
+        return []
+
     session = session or get_requests_session()
     files_in_repo = [f for _, f in uploads]
     resp = srequest(
         session,
         'POST', f"https://huggingface.co/api/{repo_type}s/{repo_id}/paths-info/{revision}",
         json={"paths": files_in_repo},
     )
```

### Comparing `hfmirror-0.0.2/hfmirror/storage/local.py` & `hfmirror-0.0.3/hfmirror/storage/local.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.2/hfmirror/sync/sync.py` & `hfmirror-0.0.3/hfmirror/sync/sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         m_folders = []
         for key, folder in folders:
             self._sync_tree(folder, [*segments, key], tqdms)
             m_folders.append({'name': key, 'metadata': folder.metadata})
 
         m_files = []
         need_load_files = []
-        for key, item in items:
+        for key, item in tqdm(items, desc=f"Mark for {'/'.join(segments)}"):
             old_file_data = old_files.get(key)
             if old_file_data and old_file_data['type'] == item.__type__:
                 try:
                     mark = item.refresh_mark(old_file_data['mark'])
                 except ResourceNotChange:
                     need_load, mark = False, old_file_data['mark']
                 else:
```

### Comparing `hfmirror-0.0.2/hfmirror/utils/download.py` & `hfmirror-0.0.3/hfmirror/utils/download.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import requests
 from tqdm.auto import tqdm
 
 from .session import get_requests_session, srequest
 
 
-def download_file(url, filename, expected_size: int = None, desc=None, session=None):
+def download_file(url, filename, expected_size: int = None, desc=None, session=None, **kwargs):
     session = session or get_requests_session()
-    response = srequest(session, 'GET', url, stream=True, allow_redirects=True)
+    response = srequest(session, 'GET', url, stream=True, allow_redirects=True, **kwargs)
     expected_size = expected_size or response.headers.get('Content-Length', None)
     expected_size = int(expected_size) if expected_size is not None else expected_size
 
     desc = desc or os.path.basename(filename)
     directory = os.path.dirname(filename)
     if directory:
         os.makedirs(directory, exist_ok=True)
```

### Comparing `hfmirror-0.0.2/hfmirror/utils/hash.py` & `hfmirror-0.0.3/hfmirror/utils/hash.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.2/hfmirror/utils/segments.py` & `hfmirror-0.0.3/hfmirror/utils/segments.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.2/hfmirror/utils/session.py` & `hfmirror-0.0.3/hfmirror/utils/session.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.2/hfmirror/utils/text.py` & `hfmirror-0.0.3/hfmirror/utils/text.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.2/hfmirror.egg-info/PKG-INFO` & `hfmirror-0.0.3/hfmirror.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfmirror
-Version: 0.0.2
+Version: 0.0.3
 Summary: Mirror for resources to local and huggingface.
 Home-page: https://github.com/narugo1992/hfmirror
 Author: narugo1992
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: A simple tool for automatic parameter tuning.
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hfmirror-0.0.2/hfmirror.egg-info/SOURCES.txt` & `hfmirror-0.0.3/hfmirror.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.2/hfmirror.egg-info/requires.txt` & `hfmirror-0.0.3/hfmirror.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.2/setup.py` & `hfmirror-0.0.3/setup.py`

 * *Files identical despite different names*

