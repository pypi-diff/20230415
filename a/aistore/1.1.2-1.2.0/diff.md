# Comparing `tmp/aistore-1.1.2.tar.gz` & `tmp/aistore-1.2.0.tar.gz`

## Comparing `aistore-1.1.2.tar` & `aistore-1.2.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/client.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/common_requirements
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/botocore_patch/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/botocore_patch/__init__.py
--rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/botocore_patch/botocore.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/botocore_patch/botocore_requirements
--rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/pytorch/README.md
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/pytorch/__init__.py
--rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/pytorch/aisio.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/pytorch/dataset.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/pytorch/dev_requirements
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/pytorch/utils.py
--rw-r--r--   0        0        0     8770 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/sdk/README.md
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/sdk/__init__.py
--rw-r--r--   0        0        0    26239 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/sdk/bucket.py
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/sdk/client.py
--rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/sdk/cluster.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/sdk/const.py
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/sdk/errors.py
--rw-r--r--   0        0        0     7006 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/sdk/etl.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/sdk/etl_const.py
--rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/sdk/etl_templates.py
--rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/sdk/job.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/sdk/list_object_flag.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/sdk/namespace.py
--rw-r--r--   0        0        0     8204 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/sdk/object.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/sdk/object_attributes.py
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/sdk/object_iterator.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/sdk/object_reader.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/sdk/request_client.py
--rw-r--r--   0        0        0     9052 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/sdk/types.py
--rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/sdk/utils.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/sdk/multiobj/__init__.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/sdk/multiobj/object_collection.py
--rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/sdk/multiobj/object_group.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/sdk/multiobj/object_names.py
--rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/sdk/multiobj/object_range.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aistore-1.1.2/aistore/sdk/multiobj/object_template.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 aistore-1.1.2/LICENSE
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 aistore-1.1.2/.gitignore
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 aistore-1.1.2/README.md
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 aistore-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 aistore-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/client.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/common_requirements
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/botocore_patch/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/botocore_patch/__init__.py
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/botocore_patch/botocore.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/botocore_patch/botocore_requirements
+-rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/pytorch/README.md
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/pytorch/__init__.py
+-rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/pytorch/aisio.py
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/pytorch/dataset.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/pytorch/dev_requirements
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/pytorch/utils.py
+-rw-r--r--   0        0        0     5511 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/README.md
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/__init__.py
+-rw-r--r--   0        0        0    26239 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/bucket.py
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/client.py
+-rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/cluster.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/const.py
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/errors.py
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/etl.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/etl_const.py
+-rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/etl_templates.py
+-rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/job.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/list_object_flag.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/namespace.py
+-rw-r--r--   0        0        0     8204 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/object.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/object_attributes.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/object_iterator.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/object_reader.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/request_client.py
+-rw-r--r--   0        0        0    10384 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/types.py
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/utils.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/multiobj/__init__.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/multiobj/object_collection.py
+-rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/multiobj/object_group.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/multiobj/object_names.py
+-rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/multiobj/object_range.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aistore-1.2.0/aistore/sdk/multiobj/object_template.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 aistore-1.2.0/LICENSE
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 aistore-1.2.0/.gitignore
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 aistore-1.2.0/README.md
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 aistore-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 aistore-1.2.0/PKG-INFO
```

### Comparing `aistore-1.1.2/aistore/botocore_patch/README.md` & `aistore-1.2.0/aistore/botocore_patch/README.md`

 * *Files identical despite different names*

### Comparing `aistore-1.1.2/aistore/botocore_patch/botocore.py` & `aistore-1.2.0/aistore/botocore_patch/botocore.py`

 * *Files identical despite different names*

### Comparing `aistore-1.1.2/aistore/pytorch/README.md` & `aistore-1.2.0/aistore/pytorch/README.md`

 * *Files identical despite different names*

### Comparing `aistore-1.1.2/aistore/pytorch/aisio.py` & `aistore-1.2.0/aistore/pytorch/aisio.py`

 * *Files 9% similar despite different names*

```diff
@@ -96,19 +96,22 @@
     Iterable DataPipe that loads files from AIStore with the given URLs (functional name: ``load_files_by_ais``).
     Iterates all files in BytesIO format and returns a tuple (url, BytesIO).
 
     Note:
     -   This function also supports files from multiple backends (`aws://..`, `gcp://..`, etc)
     -   Input must be a list and direct URLs are not supported.
     -   This internally uses AIStore Python SDK.
+    -   An `etl_name` can be provided to run an existing ETL on the AIS cluster.
+        See https://github.com/NVIDIA/aistore/blob/master/docs/etl.md for more info on AIStore ETL.
 
     Args:
         source_datapipe(IterDataPipe[str]): a DataPipe that contains URLs/URL prefixes to objects
         length(int): length of the datapipe
         url(str): AIStore endpoint
+        etl_name (str, optional): Optional etl on the AIS cluster to apply to each object
 
     Example:
         >>> from torchdata.datapipes.iter import IterableWrapper, AISFileLister,AISFileLoader
         >>> ais_prefixes = IterableWrapper(['gcp://bucket-name/folder/', 'aws:bucket-name/folder/',
         >>>     'ais://bucket-name/folder/', ...])
         >>> dp_ais_urls = AISFileLister(url='localhost:8080', source_datapipe=ais_prefixes)
         >>> dp_cloud_files = AISFileLoader(url='localhost:8080', source_datapipe=dp_ais_urls)
@@ -117,26 +120,31 @@
         >>> # Functional API
         >>> dp_cloud_files = dp_ais_urls.load_files_by_ais(url='localhost:8080')
         >>> for url, file in dp_cloud_files:
         ...     pass
     """
 
     def __init__(
-        self, source_datapipe: IterDataPipe[str], url: str, length: int = -1
+        self,
+        source_datapipe: IterDataPipe[str],
+        url: str,
+        length: int = -1,
+        etl_name: str = None,
     ) -> None:
         _assert_aistore()
         self.source_datapipe: IterDataPipe[str] = source_datapipe
         self.length = length
         self.client = Client(url)
+        self.etl_name = etl_name
 
     def __iter__(self) -> Iterator[Tuple[str, StreamWrapper]]:
         for url in self.source_datapipe:
             provider, bck_name, obj_name = parse_url(url)
             yield url, StreamWrapper(
                 self.client.bucket(bck_name=bck_name, provider=provider)
                 .object(obj_name=obj_name)
-                .get()
+                .get(etl_name=self.etl_name)
                 .raw()
             )
 
     def __len__(self) -> int:
         return len(self.source_datapipe)
```

### Comparing `aistore-1.1.2/aistore/pytorch/dataset.py` & `aistore-1.2.0/aistore/pytorch/dataset.py`

 * *Files 19% similar despite different names*

```diff
@@ -33,32 +33,37 @@
 
 
 # pylint: disable=unused-variable
 
 
 class AISDataset(AISBaseClass, Dataset):
     """
-    A map-style dataset for objects in AIS
+    A map-style dataset for objects in AIS.
+    If `etl_name` is provided, that ETL must already exist on the AIStore cluster
 
     Args:
-        client_url(str): AIS endpoint URL
-        urls_list(str or List[str]): single or list of url prefixes to load data
+        client_url (str): AIS endpoint URL
+        urls_list (str or List[str]): single or list of url prefixes to load data
+        etl_name (str, optional): Optional etl on the AIS cluster to apply to each object
     """
 
-    def __init__(self, client_url: str, urls_list: Union[str, List[str]]):
+    def __init__(
+        self, client_url: str, urls_list: Union[str, List[str]], etl_name=None
+    ):
         AISBaseClass.__init__(self, client_url, urls_list)
+        self.etl_name = etl_name
 
     def __len__(self):
         return len(self._object_info)
 
     def __getitem__(self, index: int):
         object_name = self._object_info[index]["object"]
         obj = (
             self.client.bucket(
                 bck_name=self._object_info[index]["bck_name"],
                 provider=self._object_info[index]["provider"],
             )
             .object(obj_name=object_name)
-            .get()
+            .get(etl_name=self.etl_name)
             .read_all()
         )
         return object_name, obj
```

### Comparing `aistore-1.1.2/aistore/pytorch/utils.py` & `aistore-1.2.0/aistore/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `aistore-1.1.2/aistore/sdk/bucket.py` & `aistore-1.2.0/aistore/sdk/bucket.py`

 * *Files identical despite different names*

### Comparing `aistore-1.1.2/aistore/sdk/client.py` & `aistore-1.2.0/aistore/sdk/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,17 +69,20 @@
             job_kind (str, optional): Optional specific type of job empty for all kinds
 
         Returns:
             The job object created.
         """
         return Job(client=self._request_client, job_id=job_id, job_kind=job_kind)
 
-    def etl(self):
+    def etl(self, etl_name: str):
         """
         Factory constructor for ETL object.
         Contains APIs related to AIStore ETL operations.
         Does not make any HTTP request, only instantiates an ETL object.
 
+        Args:
+            etl_name (str): Name of the ETL
+
         Returns:
             The ETL object created.
         """
-        return Etl(client=self._request_client)
+        return Etl(client=self._request_client, name=etl_name)
```

### Comparing `aistore-1.1.2/aistore/sdk/cluster.py` & `aistore-1.2.0/aistore/sdk/cluster.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,17 +15,18 @@
     WHAT_SMAP,
     URL_PATH_BUCKETS,
     URL_PATH_HEALTH,
     URL_PATH_DAEMON,
     URL_PATH_CLUSTER,
     WHAT_ALL_XACT_STATUS,
     WHAT_ALL_RUNNING_STATUS,
+    URL_PATH_ETL,
 )
 
-from aistore.sdk.types import BucketModel, JobStatus, JobQuery
+from aistore.sdk.types import BucketModel, JobStatus, JobQuery, ETLInfo
 from aistore.sdk.request_client import RequestClient
 from aistore.sdk.types import ActionMsg, Smap
 
 
 # pylint: disable=unused-variable
 class Cluster:
     """
@@ -126,14 +127,27 @@
             HTTP_METHOD_GET,
             path=URL_PATH_CLUSTER,
             res_model=List[str],
             json=JobQuery(kind=job_kind, target=target_id, active=True).as_dict(),
             params={QPARAM_WHAT: WHAT_ALL_RUNNING_STATUS},
         )
 
+    def list_running_etls(self) -> List[ETLInfo]:
+        """
+        Lists all running ETLs.
+
+        Note: Does not list ETLs that have been stopped or deleted.
+
+        Returns:
+            List[ETLInfo]: A list of details on running ETLs
+        """
+        return self._client.request_deserialize(
+            HTTP_METHOD_GET, path=URL_PATH_ETL, res_model=List[ETLInfo]
+        )
+
     def is_aistore_running(self) -> bool:
         """
         Checks if cluster is ready or still setting up.
 
         Returns:
             bool: True if cluster is ready, or false if cluster is still setting up
         """
```

### Comparing `aistore-1.1.2/aistore/sdk/const.py` & `aistore-1.2.0/aistore/sdk/const.py`

 * *Files identical despite different names*

### Comparing `aistore-1.1.2/aistore/sdk/errors.py` & `aistore-1.2.0/aistore/sdk/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,24 @@
     """
 
     def __init__(self, status_code, message):
         super().__init__(status_code=status_code, message=message)
 
 
 # pylint: disable=unused-variable
+class ErrETLAlreadyExists(AISError):
+    """
+    Raised when an ETL is created but already exists in AIS
+    """
+
+    def __init__(self, status_code, message):
+        super().__init__(status_code=status_code, message=message)
+
+
+# pylint: disable=unused-variable
 class Timeout(Exception):
     """
     Raised when an operation takes too long to complete
     """
 
     def __init__(self, action, message=""):
         super().__init__(f"Timed out while waiting for {action}. {message}")
```

### Comparing `aistore-1.1.2/aistore/sdk/etl.py` & `aistore-1.2.0/aistore/sdk/etl.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 #
 # Copyright (c) 2022-2023, NVIDIA CORPORATION. All rights reserved.
 #
 import sys
 
 import base64
 from typing import Callable, List
+
 import cloudpickle
+
 from aistore.sdk.const import (
     HTTP_METHOD_DELETE,
     HTTP_METHOD_GET,
     HTTP_METHOD_POST,
     HTTP_METHOD_PUT,
     URL_PATH_ETL,
     UTF_ENCODING,
@@ -20,15 +22,15 @@
     DEFAULT_ETL_COMM,
     DEFAULT_ETL_TIMEOUT,
     ETL_COMM_SPEC,
     ETL_COMM_CODE,
     CODE_TEMPLATE,
 )
 
-from aistore.sdk.types import ETL, ETLDetails
+from aistore.sdk.types import ETLDetails, InitCodeETLArgs, InitSpecETLArgs
 
 
 def _get_default_runtime():
     """
     Determines etl runtime to use if not specified
     Returns:
         String of runtime
@@ -47,179 +49,166 @@
 
 
 class Etl:
     """
     A class containing ETL-related functions.
     """
 
-    def __init__(self, client):
+    def __init__(self, client: "Client", name: str):
         self._client = client
+        self._name = name
 
     @property
-    def client(self):
-        """The client bound to this ETL object."""
-        return self._client
+    def name(self) -> str:
+        """Name of the ETL"""
+        return self._name
 
     def init_spec(
         self,
         template: str,
-        etl_name: str,
         communication_type: str = DEFAULT_ETL_COMM,
         timeout: str = DEFAULT_ETL_TIMEOUT,
-    ):
+    ) -> str:
         """
         Initializes ETL based on Kubernetes pod spec template. Returns etl_name.
 
         Args:
             template (str): Kubernetes pod spec template
                 Existing templates can be found at `sdk.etl_templates`
                 For more information visit: https://github.com/NVIDIA/ais-etl/tree/master/transformers
-            etl_name (str): Name of new ETL
             communication_type (str): Communication type of the ETL (options: hpull, hrev, hpush)
             timeout (str): Timeout of the ETL job (e.g. 5m for 5 minutes)
         Returns:
-            etl_name (str): ETL name
+            Job ID string associated with this ETL
         """
         _validate_comm_type(communication_type, ETL_COMM_SPEC)
 
         # spec
         spec_encoded = base64.b64encode(template.encode(UTF_ENCODING)).decode(
             UTF_ENCODING
         )
 
-        action = {
-            "spec": spec_encoded,
-            "id": etl_name,
-            "communication": f"{communication_type}://",
-            "timeout": timeout,
-        }
+        value = InitSpecETLArgs(
+            spec=spec_encoded,
+            etl_name=self._name,
+            communication_type=communication_type,
+            timeout=timeout,
+        ).as_dict()
 
-        resp = self.client.request(HTTP_METHOD_PUT, path=URL_PATH_ETL, json=action)
-        return resp.text
+        return self._client.request(HTTP_METHOD_PUT, path=URL_PATH_ETL, json=value).text
 
     # pylint: disable=too-many-arguments
     def init_code(
         self,
         transform: Callable,
-        etl_name: str,
         dependencies: List[str] = None,
+        preimported_modules: List[str] = None,
         runtime: str = _get_default_runtime(),
         communication_type: str = DEFAULT_ETL_COMM,
         timeout: str = DEFAULT_ETL_TIMEOUT,
         chunk_size: int = None,
-    ):
+    ) -> str:
         """
         Initializes ETL based on the provided source code. Returns etl_name.
 
         Args:
             transform (Callable): Transform function of the ETL
-            etl_name (str): Name of new ETL
             dependencies (list[str]): Python dependencies to install
+            preimported_modules (list[str]): Modules to import before running the transform function. This can
+             be necessary in cases where the modules used both attempt to import each other circularly
             runtime (str): [optional, default= V2 implementation of the current python version if supported, else
                 python3.8v2] Runtime environment of the ETL [choose from: python3.8v2, python3.10v2, python3.11v2]
                 (see ext/etl/runtime/all.go)
             communication_type (str): [optional, default="hpush"] Communication type of the ETL (options: hpull, hrev,
                 hpush, io)
             timeout (str): [optional, default="5m"] Timeout of the ETL job (e.g. 5m for 5 minutes)
             chunk_size (int): Chunk size in bytes if transform function in streaming data.
                 (whole object is read by default)
         Returns:
-            etl_name (str): ETL name
+            Job ID string associated with this ETL
         """
         _validate_comm_type(communication_type, ETL_COMM_CODE)
 
+        # code functions to call
         functions = {
             "transform": "transform",
         }
 
-        action = {
-            "id": etl_name,
-            "runtime": runtime,
-            "communication": f"{communication_type}://",
-            "timeout": timeout,
-            "funcs": functions,
-        }
-
-        if chunk_size:
-            action["chunk_size"] = chunk_size
-
-        # code
-        transform = base64.b64encode(cloudpickle.dumps(transform)).decode(UTF_ENCODING)
-
-        io_comm_context = "transform()" if communication_type == "io" else ""
-        template = CODE_TEMPLATE.format(transform, io_comm_context).encode(UTF_ENCODING)
-        action["code"] = base64.b64encode(template).decode(UTF_ENCODING)
-
-        # dependencies
-        if dependencies is None:
-            dependencies = []
-        dependencies.append("cloudpickle==2.2.0")
-        deps = "\n".join(dependencies).encode(UTF_ENCODING)
-        action["dependencies"] = base64.b64encode(deps).decode(UTF_ENCODING)
+        value = InitCodeETLArgs(
+            etl_name=self._name,
+            runtime=runtime,
+            communication_type=communication_type,
+            timeout=timeout,
+            dependencies=self._encode_dependencies(dependencies),
+            functions=functions,
+            code=self._encode_transform(
+                transform, preimported_modules, communication_type
+            ),
+            chunk_size=chunk_size,
+        ).as_dict()
 
-        resp = self.client.request(
+        return self._client.request(
             HTTP_METHOD_PUT,
             path=URL_PATH_ETL,
-            json=action,
-        )
-        return resp.text
-
-    def list(self) -> List[ETLDetails]:
-        """
-        Lists all running ETLs.
-
-        Note: Does not list ETLs that have been stopped or deleted.
-
-        Returns:
-            List[ETL]: A list of running ETLs
-        """
-        resp = self.client.request_deserialize(
-            HTTP_METHOD_GET, path=URL_PATH_ETL, res_model=List[ETL]
-        )
-        return resp
+            json=value,
+        ).text
 
-    def view(self, etl_name: str) -> ETLDetails:
+    def view(self) -> ETLDetails:
         """
-        View ETLs Init spec/code
+        View ETL details
 
-        Args:
-            etl_name (str): name of ETL
         Returns:
             ETLDetails: details of the ETL
         """
-        resp = self.client.request_deserialize(
-            HTTP_METHOD_GET, path=f"{URL_PATH_ETL}/{etl_name}", res_model=ETLDetails
+        resp = self._client.request_deserialize(
+            HTTP_METHOD_GET, path=f"{URL_PATH_ETL}/{self._name}", res_model=ETLDetails
         )
         return resp
 
-    def start(self, etl_name: str):
+    def start(self):
         """
         Resumes a stopped ETL with given ETL name.
 
         Note: Deleted ETLs cannot be started.
-
-        Args:
-            etl_name (str): name of ETL
         """
-        self.client.request(HTTP_METHOD_POST, path=f"{URL_PATH_ETL}/{etl_name}/start")
+        self._client.request(
+            HTTP_METHOD_POST, path=f"{URL_PATH_ETL}/{self._name}/start"
+        )
 
-    def stop(self, etl_name: str):
+    def stop(self):
         """
-        Stops ETL with given ETL name. Stops (but does not delete) all the pods created by Kubernetes for this ETL and
+        Stops ETL. Stops (but does not delete) all the pods created by Kubernetes for this ETL and
         terminates any transforms.
-
-        Args:
-            etl_name (str): name of ETL
         """
-        self.client.request(HTTP_METHOD_POST, path=f"{URL_PATH_ETL}/{etl_name}/stop")
+        self._client.request(HTTP_METHOD_POST, path=f"{URL_PATH_ETL}/{self._name}/stop")
 
-    def delete(self, etl_name: str):
+    def delete(self):
         """
-        Delete ETL with given ETL name. Deletes pods created by Kubernetes for this ETL and specifications for this ETL
+        Delete ETL. Deletes pods created by Kubernetes for this ETL and specifications for this ETL
         in Kubernetes.
 
         Note: Running ETLs cannot be deleted.
-
-        Args:
-            etl_name (str): name of ETL
         """
-        self.client.request(HTTP_METHOD_DELETE, path=f"{URL_PATH_ETL}/{etl_name}")
+        self._client.request(HTTP_METHOD_DELETE, path=f"{URL_PATH_ETL}/{self._name}")
+
+    @staticmethod
+    def _encode_transform(
+        transform: Callable,
+        preimported_modules: List[str] = None,
+        comm_type: str = None,
+    ):
+        transform = base64.b64encode(cloudpickle.dumps(transform)).decode(UTF_ENCODING)
+
+        io_comm_context = "transform()" if comm_type == "io" else ""
+        modules = preimported_modules if preimported_modules else []
+        template = CODE_TEMPLATE.format(modules, transform, io_comm_context).encode(
+            UTF_ENCODING
+        )
+        return base64.b64encode(template).decode(UTF_ENCODING)
+
+    @staticmethod
+    def _encode_dependencies(dependencies: List[str]):
+        if dependencies is None:
+            dependencies = []
+        dependencies.append("cloudpickle==2.2.0")
+        deps = "\n".join(dependencies).encode(UTF_ENCODING)
+        return base64.b64encode(deps).decode(UTF_ENCODING)
```

### Comparing `aistore-1.1.2/aistore/sdk/etl_const.py` & `aistore-1.2.0/aistore/sdk/etl_const.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,11 +19,15 @@
 ETL_SUPPORTED_PYTHON_VERSIONS = ["3.10", "3.11"]
 
 # templates for ETL
 
 CODE_TEMPLATE = """
 import pickle
 import base64
+import importlib
 
+for mod in {}:
+    importlib.import_module(mod)
+    
 transform = pickle.loads(base64.b64decode('{}'))
 {}
 """
```

### Comparing `aistore-1.1.2/aistore/sdk/etl_templates.py` & `aistore-1.2.0/aistore/sdk/etl_templates.py`

 * *Files identical despite different names*

### Comparing `aistore-1.1.2/aistore/sdk/job.py` & `aistore-1.2.0/aistore/sdk/job.py`

 * *Files identical despite different names*

### Comparing `aistore-1.1.2/aistore/sdk/list_object_flag.py` & `aistore-1.2.0/aistore/sdk/list_object_flag.py`

 * *Files identical despite different names*

### Comparing `aistore-1.1.2/aistore/sdk/object.py` & `aistore-1.2.0/aistore/sdk/object.py`

 * *Files identical despite different names*

### Comparing `aistore-1.1.2/aistore/sdk/object_attributes.py` & `aistore-1.2.0/aistore/sdk/object_attributes.py`

 * *Files identical despite different names*

### Comparing `aistore-1.1.2/aistore/sdk/object_iterator.py` & `aistore-1.2.0/aistore/sdk/object_iterator.py`

 * *Files identical despite different names*

### Comparing `aistore-1.1.2/aistore/sdk/object_reader.py` & `aistore-1.2.0/aistore/sdk/object_reader.py`

 * *Files identical despite different names*

### Comparing `aistore-1.1.2/aistore/sdk/request_client.py` & `aistore-1.2.0/aistore/sdk/request_client.py`

 * *Files identical despite different names*

### Comparing `aistore-1.1.2/aistore/sdk/types.py` & `aistore-1.2.0/aistore/sdk/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -167,20 +167,21 @@
 
     uuid: str = ""
     err: str = ""
     end_time: int = 0
     aborted: bool = False
 
 
-class ETL(BaseModel):  # pylint: disable=too-few-public-methods,unused-variable
+class ETLInfo(BaseModel):  # pylint: disable=too-few-public-methods,unused-variable
     """
     Represents the API response when querying an ETL
     """
 
     id: str = ""
+    xaction_id: str = ""
     obj_count: int = 0
     in_bytes: int = 0
     out_bytes: int = 0
 
 
 class ETLDetails(BaseModel):
     """
@@ -205,14 +206,66 @@
     @validator("spec")
     def set_spec(cls, spec):  # pylint: disable=no-self-argument
         if spec is not None:
             spec = base64.b64decode(spec)
         return spec
 
 
+class InitETLArgs(BaseModel):
+    """
+    Represents the args shared by ETL initialization with code or spec
+    """
+
+    etl_name: str
+    communication_type: str
+    timeout: str
+
+
+class InitSpecETLArgs(InitETLArgs):
+    """
+    Represents the set of args the sdk will pass to AIStore when making a request to initialize an ETL with a spec
+    """
+
+    spec: str
+
+    def as_dict(self):
+        return {
+            "id": self.etl_name,
+            "timeout": self.timeout,
+            "communication": f"{self.communication_type}://",
+            "spec": self.spec,
+        }
+
+
+class InitCodeETLArgs(InitETLArgs):
+    """
+    Represents the set of args the sdk will pass to AIStore when making a request to initialize an ETL with code
+    """
+
+    runtime: str
+    dependencies: str
+    functions: Dict[str, str]
+    code: str
+    chunk_size: int = None
+
+    def as_dict(self):
+        dict_rep = {
+            "id": self.etl_name,
+            "runtime": self.runtime,
+            "communication": f"{self.communication_type}://",
+            "timeout": self.timeout,
+            "funcs": self.functions,
+            "code": self.code,
+            "dependencies": self.dependencies,
+        }
+        if self.chunk_size:
+            dict_rep["chunk_size"] = self.chunk_size
+        return dict_rep
+
+
 class PromoteAPIArgs(BaseModel):
     """
     Represents the set of args the sdk will pass to AIStore when making a promote request and
     provides conversion to the expected json format
     """
 
     target_id: str = ""
```

### Comparing `aistore-1.1.2/aistore/sdk/utils.py` & `aistore-1.2.0/aistore/sdk/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 from aistore.sdk.const import UTF_ENCODING
 from aistore.sdk.errors import (
     AISError,
     ErrBckNotFound,
     ErrRemoteBckNotFound,
     ErrBckAlreadyExists,
+    ErrETLAlreadyExists,
 )
 
 
 class HttpError(BaseModel):
     """
     Represents the errors returned by the API
     """
@@ -39,15 +40,18 @@
         err = pydantic.tools.parse_raw_as(HttpError, text)
         if "does not exist" in err.message:
             if "cloud bucket" in err.message or "remote bucket" in err.message:
                 raise ErrRemoteBckNotFound(err.status, err.message)
             if "bucket" in err.message:
                 raise ErrBckNotFound(err.status, err.message)
         if "already exists" in err.message:
-            raise ErrBckAlreadyExists(err.status, err.message)
+            if "bucket" in err.message:
+                raise ErrBckAlreadyExists(err.status, err.message)
+            if "etl" in err.message:
+                raise ErrETLAlreadyExists(err.status, err.message)
     raise AISError(err.status, err.message)
 
 
 # pylint: disable=unused-variable
 def handle_errors(resp: requests.Response):
     """
     Error handling for requests made to the AIS Client
```

### Comparing `aistore-1.1.2/aistore/sdk/multiobj/object_collection.py` & `aistore-1.2.0/aistore/sdk/multiobj/object_collection.py`

 * *Files identical despite different names*

### Comparing `aistore-1.1.2/aistore/sdk/multiobj/object_group.py` & `aistore-1.2.0/aistore/sdk/multiobj/object_group.py`

 * *Files identical despite different names*

### Comparing `aistore-1.1.2/aistore/sdk/multiobj/object_names.py` & `aistore-1.2.0/aistore/sdk/multiobj/object_names.py`

 * *Files identical despite different names*

### Comparing `aistore-1.1.2/aistore/sdk/multiobj/object_range.py` & `aistore-1.2.0/aistore/sdk/multiobj/object_range.py`

 * *Files identical despite different names*

### Comparing `aistore-1.1.2/aistore/sdk/multiobj/object_template.py` & `aistore-1.2.0/aistore/sdk/multiobj/object_template.py`

 * *Files identical despite different names*

### Comparing `aistore-1.1.2/LICENSE` & `aistore-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aistore-1.1.2/.gitignore` & `aistore-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aistore-1.1.2/README.md` & `aistore-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `aistore-1.1.2/pyproject.toml` & `aistore-1.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 [tool.pytest.ini_options]
 markers = [
     "etl: marks tests as using etl and therefore requiring k8s cluster",
 ]
 
 [project]
 name = "aistore"
-version = "1.1.2"
+version = "1.2.0"
 authors = [
   { name="AIStore Team", email="ais@exchange.nvidia.com" },
 ]
 description = "A (growing) set of client-side APIs to access and utilize clusters, buckets, and objects on AIStore."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT License"}
```

### Comparing `aistore-1.1.2/PKG-INFO` & `aistore-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aistore
-Version: 1.1.2
+Version: 1.2.0
 Summary: A (growing) set of client-side APIs to access and utilize clusters, buckets, and objects on AIStore.
 Project-URL: Homepage, https://aiatscale.org
 Project-URL: Download, https://github.com/NVIDIA/aistore/tags
 Project-URL: Documentation, https://aiatscale.org/docs/
 Project-URL: Release notes, https://github.com/NVIDIA/aistore/releases/
 Project-URL: Source, https://github.com/NVIDIA/aistore/
 Author-email: AIStore Team <ais@exchange.nvidia.com>
```

