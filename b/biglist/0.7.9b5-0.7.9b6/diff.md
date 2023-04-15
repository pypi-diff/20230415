# Comparing `tmp/biglist-0.7.9b5.tar.gz` & `tmp/biglist-0.7.9b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biglist-0.7.9b5.tar", last modified: Thu Apr 13 07:47:04 2023, max compression
+gzip compressed data, was "biglist-0.7.9b6.tar", last modified: Fri Apr 14 06:54:05 2023, max compression
```

## Comparing `biglist-0.7.9b5.tar` & `biglist-0.7.9b6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1067 2023-01-09 08:46:44.766242 biglist-0.7.9b5/LICENSE
--rw-r--r--   0        0        0      931 2023-04-10 09:40:14.837561 biglist-0.7.9b5/README.rst
--rw-r--r--   0        0        0     1628 2023-04-11 16:08:19.638866 biglist-0.7.9b5/pyproject.toml
--rw-r--r--   0        0        0     2217 2023-04-13 07:43:36.928982 biglist-0.7.9b5/src/biglist/__init__.py
--rw-r--r--   0        0        0    18555 2023-04-13 07:44:02.101802 biglist-0.7.9b5/src/biglist/_base.py
--rw-r--r--   0        0        0    44004 2023-04-13 07:44:02.431804 biglist-0.7.9b5/src/biglist/_biglist.py
--rw-r--r--   0        0        0    34691 2023-04-13 07:44:02.651805 biglist-0.7.9b5/src/biglist/_parquet.py
--rw-r--r--   0        0        0    12025 2023-04-10 09:40:14.847560 biglist-0.7.9b5/src/biglist/_util.py
--rw-r--r--   0        0        0        0 2023-01-09 08:46:44.766242 biglist-0.7.9b5/src/biglist/py.typed
--rw-r--r--   0        0        0     2209 1970-01-01 00:00:00.000000 biglist-0.7.9b5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-01-09 08:46:44.766242 biglist-0.7.9b6/LICENSE
+-rw-r--r--   0        0        0      931 2023-04-10 09:40:14.837561 biglist-0.7.9b6/README.rst
+-rw-r--r--   0        0        0     1628 2023-04-11 16:08:19.638866 biglist-0.7.9b6/pyproject.toml
+-rw-r--r--   0        0        0     2217 2023-04-14 06:27:24.443094 biglist-0.7.9b6/src/biglist/__init__.py
+-rw-r--r--   0        0        0    17990 2023-04-14 06:46:49.671033 biglist-0.7.9b6/src/biglist/_base.py
+-rw-r--r--   0        0        0    44172 2023-04-14 05:23:32.226273 biglist-0.7.9b6/src/biglist/_biglist.py
+-rw-r--r--   0        0        0    34770 2023-04-14 06:49:13.536597 biglist-0.7.9b6/src/biglist/_parquet.py
+-rw-r--r--   0        0        0    12025 2023-04-10 09:40:14.847560 biglist-0.7.9b6/src/biglist/_util.py
+-rw-r--r--   0        0        0        0 2023-01-09 08:46:44.766242 biglist-0.7.9b6/src/biglist/py.typed
+-rw-r--r--   0        0        0     2209 1970-01-01 00:00:00.000000 biglist-0.7.9b6/PKG-INFO
```

### Comparing `biglist-0.7.9b5/LICENSE` & `biglist-0.7.9b6/LICENSE`

 * *Files identical despite different names*

### Comparing `biglist-0.7.9b5/README.rst` & `biglist-0.7.9b6/README.rst`

 * *Files identical despite different names*

### Comparing `biglist-0.7.9b5/pyproject.toml` & `biglist-0.7.9b6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `biglist-0.7.9b5/src/biglist/__init__.py` & `biglist-0.7.9b6/src/biglist/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,8 +48,8 @@
 )
 from ._util import (
     Chain,
     Seq,
     Slicer,
 )
 
-__version__ = "0.7.9b5"
+__version__ = "0.7.9b6"
```

### Comparing `biglist-0.7.9b5/src/biglist/_base.py` & `biglist-0.7.9b6/src/biglist/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 import os
 import queue
 import tempfile
 import uuid
 from abc import abstractmethod
 from collections.abc import Iterator
 from typing import (
-    Any,
-    Callable,
     Optional,
     TypeVar,
 )
 
 from mpservice.util import get_shared_thread_pool
 from upathlib import LocalUpath, PathType, Upath, resolve_path
 
@@ -50,54 +48,34 @@
     contained in the file.
     For example you can write::
 
         def func(file_reader: FileReader[int]):
             ...
     """
 
-    def __init__(self, path: PathType, loader: Callable[[Upath], Any]):
-        """
-        Parameters
-        ----------
-        path
-            Path of the data file.
-        loader
-            A function that will be used to load the data file.
-            This must be pickle-able.
-        """
-        self.path: Upath = resolve_path(path)
-        """Path of the file."""
-        self.loader: Callable[[Upath], Any] = loader
-        """A function that will be used to read the data file."""
-
     def __repr__(self):
         return f"<{self.__class__.__name__} for '{self.path}'>"
 
     def __str__(self):
         return self.__repr__()
 
-    def __getstate__(self):
-        return self.path, self.loader
-
-    def __setstate__(self, data):
-        self.path, self.loader = data
-
     @abstractmethod
     def load(self) -> None:
         """
         This method *eagerly* loads all the data from the file.
 
         Once this method has been called, typically the entire data file is loaded
         into memory, and subsequent data consumption should all draw upon this
         in-memory copy. However, if the data file is large, and especially
         if only part of the data is of interest, calling this method may not be
         the best approach. This all depends on the specifics of the subclass.
 
         A subclass may allow consuming the data and load parts of data
-        in a "as-needed" or "streaming" fashion.
+        in a "as-needed" or "streaming" fashion. In that approach,
+        this method is not called, although it is available.
         """
         raise NotImplementedError
 
 
 FileReaderType = TypeVar("FileReaderType", bound=FileReader)
 
 
@@ -378,15 +356,15 @@
 
     def destroy(self, *, concurrent=True) -> None:
         self.keep_files = False
         self.path.rmrf(concurrent=concurrent)
 
     def __del__(self):
         if getattr(self, "keep_files", True) is False:
-            self.destroy()
+            self.destroy(concurrent=False)
 
     def __getitem__(self, idx: int) -> Element:
         """
         Access a data item by its index; negative index works as expected.
         """
         # This is not optimized for speed.
         # For better speed, use ``__iter__``.
```

### Comparing `biglist-0.7.9b5/src/biglist/_biglist.py` & `biglist-0.7.9b6/src/biglist/_biglist.py`

 * *Files 1% similar despite different names*

```diff
@@ -725,25 +725,29 @@
     def __init__(self, path: PathType, loader: Callable[[Upath], Any]):
         """
         Parameters
         ----------
         path
             Path of a data file.
         loader
+            A function that will be used to load the data file.
+            This must be pickle-able.
             Usually this is :meth:`Biglist.load_data_file`.
             If you customize this, please see the doc of :meth:`FileReader.__init__`.
         """
+        super().__init__()
+        self.path: Upath = resolve_path(path)
+        self.loader = loader
         self._data: Optional[list] = None
-        super().__init__(path, loader)
 
     def __getstate__(self):
-        return super().__getstate__()
+        return self.path, self.loader
 
     def __setstate__(self, data):
-        super().__setstate__(data)
+        self.path, self.loader = data
         self._data = None
 
     def load(self) -> None:
         if self._data is None:
             self._data = self.loader(self.path)
 
     def data(self) -> list[Element]:
```

### Comparing `biglist-0.7.9b5/src/biglist/_parquet.py` & `biglist-0.7.9b6/src/biglist/_parquet.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import annotations
 
+import io
 import itertools
 import logging
 from collections.abc import Iterable, Iterator, Sequence
 from multiprocessing.util import Finalize
 from pathlib import Path
-from typing import Any, Callable, Optional
+from typing import Optional
 
 import pyarrow
 from deprecation import deprecated
 from pyarrow.fs import FileSystem, GcsFileSystem
 from pyarrow.parquet import FileMetaData, ParquetFile
 from upathlib import LocalUpath, PathType, Upath, resolve_path
 
 try:
-    from google.cloud.storage import retry as gcs_retry
     from upathlib.gcs import get_google_auth
 except ImportError:
     pass
 
 from ._base import (
     BiglistBase,
     FileReader,
@@ -54,64 +54,14 @@
     it points to pre-existing Parquet files and provides facilities to read them.
     As long as you use a ParquetBiglist object to read, it is assumed that
     the dataset (all the data files) have not changed since the object was created
     by :meth:`new`.
     """
 
     @classmethod
-    def get_gcsfs(cls, *, good_for_seconds=600) -> GcsFileSystem:
-        """
-        Obtain a `pyarrow.fs.GcsFileSystem`_ object with credentials given so that
-        the GCP default process of inferring credentials (which involves
-        env vars and file reading etc) will not be triggered.
-
-        This is provided under the (un-verified) assumption that the
-        default credential inference process is a high overhead.
-        """
-        cls._GCP_PROJECT_ID, cls._GCP_CREDENTIALS, renewed = get_google_auth(
-            project_id=getattr(cls, '_GCP_PROJECT_ID', None),
-            credentials=getattr(cls, "_GCP_CREDENTIALS", None),
-            valid_for_seconds=good_for_seconds,
-        )
-        if renewed or getattr(cls, '_GCSFS', None) is None:
-            fs = GcsFileSystem(
-                access_token=cls._GCP_CREDENTIALS.token,
-                credential_token_expiration=cls._GCP_CREDENTIALS.expiry,
-            )
-            cls._GCSFS = fs
-        return cls._GCSFS
-
-    @classmethod
-    def _gcs_retry(cls):
-        def _should_retry(exc):
-            if isinstance(exc, pyarrow.lib.ArrowException) and str(exc).startswith(
-                'Unknown error'
-            ):
-                return True
-            return gcs_retry.DEFAULT_RETRY._predicate(exc)
-
-        return gcs_retry.DEFAULT_RETRY.with_predicate(_should_retry)
-
-    @classmethod
-    def load_data_file(cls, path: Upath) -> ParquetFile:
-        """
-        Load the data file given by ``path``.
-
-        This function is used as the argument ``loader`` to :meth:`ParquetFileReader.__init__`.
-        The value it returns is contained in :class:`FileReader` for subsequent use.
-        """
-        ff, pp = FileSystem.from_uri(str(path))
-        if isinstance(ff, GcsFileSystem):
-            ff = cls.get_gcsfs()
-            pf = cls._gcs_retry()(ParquetFile)  # a retry-wrapped func
-        else:
-            pf = ParquetFile
-        return pf(pp, filesystem=ff)
-
-    @classmethod
     def new(
         cls,
         data_path: PathType | Sequence[PathType],
         path: Optional[PathType] = None,
         *,
         suffix: str = ".parquet",
         **kwargs,
@@ -159,16 +109,16 @@
         if isinstance(data_path, (str, Path, Upath)):
             #  TODO: in py 3.10, we will be able to do `isinstance(data_path, PathType)`
             data_path = [resolve_path(data_path)]
         else:
             data_path = [resolve_path(p) for p in data_path]
 
         def get_file_meta(p: Upath):
-            with cls.load_data_file(p) as ff:
-                meta = ff.metadata
+            ff = ParquetFileReader.load_file(p)
+            meta = ff.metadata
             return {
                 "path": str(p),  # str of full path
                 "num_rows": meta.num_rows,
                 # "row_groups_num_rows": [
                 #     meta.row_group(k).num_rows for k in range(meta.num_row_groups)
                 # ],
             }
@@ -258,30 +208,86 @@
 
     @property
     def files(self):
         # This method should be cheap to call.
         return ParquetFileSeq(
             self.path,
             self.info["data_files_info"],
-            self.load_data_file,
         )
 
 
 class ParquetFileReader(FileReader):
-    def __init__(self, path: PathType, loader: Callable[[Upath], Any]):
+    @classmethod
+    def get_gcsfs(cls, *, good_for_seconds=600) -> GcsFileSystem:
+        """
+        Obtain a `pyarrow.fs.GcsFileSystem`_ object with credentials given so that
+        the GCP default process of inferring credentials (which involves
+        env vars and file reading etc) will not be triggered.
+
+        This is provided under the (un-verified) assumption that the
+        default credential inference process is a high overhead.
+        """
+        cls._GCP_PROJECT_ID, cls._GCP_CREDENTIALS, renewed = get_google_auth(
+            project_id=getattr(cls, '_GCP_PROJECT_ID', None),
+            credentials=getattr(cls, "_GCP_CREDENTIALS", None),
+            valid_for_seconds=good_for_seconds,
+        )
+        if renewed or getattr(cls, '_GCSFS', None) is None:
+            fs = GcsFileSystem(
+                access_token=cls._GCP_CREDENTIALS.token,
+                credential_token_expiration=cls._GCP_CREDENTIALS.expiry,
+            )
+            cls._GCSFS = fs
+        return cls._GCSFS
+
+    @classmethod
+    def load_file(cls, path: Upath, *, lazy: bool = True) -> ParquetFile:
+        '''
+        Depending on the implementation, this may read *meta* info only, or
+        load in the entire file eagerly.
+
+        Parameters
+        ----------
+        path
+            Path of the file.
+        lazy
+            If ``True`` (the default), only *meta* info is loaded to construct
+            a ``ParquetFile`` object.
+            If ``False``, ``path.read_bytes()`` is called to read in the entire file into memory,
+            and the bytes are then used to construct a ``ParquetFile`` object.
+            The second route is provided to work around an issue encountered when
+            ``path`` is in Google Cloud Storage.
+        '''
+        if lazy:
+            ff, pp = FileSystem.from_uri(str(path))
+            if isinstance(ff, GcsFileSystem):
+                ff = cls.get_gcsfs()
+            file = ParquetFile(pp, filesystem=ff)
+        else:
+            data = io.BytesIO(path.read_bytes())
+            file = ParquetFile(data)
+        Finalize(file, file.close)
+        return file
+
+    def __init__(self, path: PathType):
         """
         Parameters
         ----------
         path
             Path of a Parquet file.
-        loader
-            Usually this is :meth:`ParquetBiglist.load_data_file`.
-            If you customize this, please see the doc of :meth:`FileReader.__init__`.
         """
-        super().__init__(path, loader)
+        self.path: Upath = resolve_path(path)
+        self.lazy = True
+        # ``self.lazy`` is used in ``self.file`` when it calls ``self.load_file``.
+        # If you change ``self.lazy`` after ``self.file`` has been called, then
+        # the change has no effect.
+        # This attribute is not controlled by a parameter conveniently because
+        # this may be removed later once the issue it is working around is resolved.
+        # To use this, just set its value directly on the ``ParquetFileReader`` object
+        # before the object has been used (hence its ``file`` may have been called).
         self._reset()
 
     def _reset(self):
         self._file: Optional[ParquetFile] = None
         self._data: Optional[ParquetBatchData] = None
 
         self._row_groups_num_rows = None
@@ -292,18 +298,18 @@
         self._columns = {}
         self._getitem_last_row_group = None
 
         self._scalar_as_py = None
         self.scalar_as_py = True
 
     def __getstate__(self):
-        return super().__getstate__()
+        return self.path, self.lazy
 
     def __setstate__(self, data):
-        super().__setstate__(data)
+        self.path, self.lazy = data
         self._reset()
 
     @property
     def scalar_as_py(self) -> bool:
         """
         ``scalar_as_py`` controls whether the values returned by :meth:`__getitem__`
         (or indirectly by :meth:`__iter__`) are converted from a `pyarrow.Scalar`_ type
@@ -344,20 +350,19 @@
 
     @property
     def file(self) -> ParquetFile:
         """Return a `pyarrow.parquet.ParquetFile`_ object.
 
         Upon initiation of a :class:`ParquetFileReader` object,
         the file is not read at all. When this property is requested,
-        the file is accessed to construct a `pyarrow.parquet.ParquetFile`_ object,
-        but this only reads *meta* info; it does not read the *data*.
+        the file is accessed to construct a `pyarrow.parquet.ParquetFile`_ object.
+
         """
         if self._file is None:
-            self._file = self.loader(self.path)
-            Finalize(self, self._file.close)
+            self._file = self.load_file(self.path, lazy=self.lazy)
         return self._file
 
     @property
     def metadata(self) -> FileMetaData:
         return self.file.metadata
 
     @property
@@ -517,15 +522,15 @@
                     return self
             else:
                 cc = [col for col in cols if col not in self._column_names]
                 raise ValueError(
                     f"cannot select the columns {cc} because they are not in existing set of columns"
                 )
 
-        obj = self.__class__(self.path, self.loader)
+        obj = self.__class__(self.path)
         obj.scalar_as_py = self.scalar_as_py
         obj._file = self._file
         obj._row_groups_num_rows = self._row_groups_num_rows
         obj._row_groups_num_rows_cumsum = self._row_groups_num_rows_cumsum
         if self._row_groups:
             obj._row_groups = [
                 None if v is None else v.columns(cols) for v in self._row_groups
@@ -560,46 +565,41 @@
 
 
 class ParquetFileSeq(FileSeq[ParquetFileReader]):
     def __init__(
         self,
         root_dir: Upath,
         data_files_info: list[tuple[str, int, int]],
-        file_loader: Callable[[Upath], Any],
     ):
         """
         Parameters
         ----------
         root_dir
             Root directory for storage of meta info.
         data_files_info
             A list of data files that constitute the file sequence.
             Each tuple in the list is comprised of a file path (relative to
             ``root_dir``), number of data items in the file, and cumulative
             number of data items in the files up to the one at hand.
             Therefore, the order of the files in the list is significant.
-        file_loader
-            A function that will be used to load a data file.
         """
         self._root_dir = root_dir
         self._data_files_info = data_files_info
-        self._file_loader = file_loader
 
     @property
     def path(self):
         return self._root_dir
 
     @property
     def data_files_info(self):
         return self._data_files_info
 
     def __getitem__(self, idx: int):
         return ParquetFileReader(
             self._data_files_info[idx][0],
-            self._file_loader,
         )
 
 
 class ParquetBatchData(Seq):
     """
     ``ParquetBatchData`` wraps a `pyarrow.Table`_ or `pyarrow.RecordBatch`_.
     The data is already in memory; this class does not involve file reading.
@@ -750,15 +750,15 @@
 def read_parquet_file(path: PathType) -> ParquetFileReader:
     """
     Parameters
     ----------
     path
         Path of the file.
     """
-    return ParquetFileReader(path, ParquetBiglist.load_data_file)
+    return ParquetFileReader(path)
 
 
 def make_parquet_type(type_spec: str | Sequence):
     """
     ``type_spec`` is a spec of arguments to one of pyarrow's data type
     `factory functions <https://arrow.apache.org/docs/python/api/datatypes.html#factory-functions>`_.
```

### Comparing `biglist-0.7.9b5/src/biglist/_util.py` & `biglist-0.7.9b6/src/biglist/_util.py`

 * *Files identical despite different names*

### Comparing `biglist-0.7.9b5/PKG-INFO` & `biglist-0.7.9b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biglist
-Version: 0.7.9b5
+Version: 0.7.9b6
 Summary: The package `biglist <https://github.com/zpz/biglist>`_ provides persisted, out-of-memory Python data structures
 Author-email: Zepu Zhang <zepu.zhang@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

