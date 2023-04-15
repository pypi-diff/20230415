# Comparing `tmp/sqlalchemy_fields-0.3.0.tar.gz` & `tmp/sqlalchemy_fields-0.4.0.tar.gz`

## Comparing `sqlalchemy_fields-0.3.0.tar` & `sqlalchemy_fields-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.3.0/sqlalchemy_fields/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.3.0/sqlalchemy_fields/exceptions.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.3.0/sqlalchemy_fields/storages/__init__.py
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.3.0/sqlalchemy_fields/storages/base.py
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.3.0/sqlalchemy_fields/storages/filesystem.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.3.0/sqlalchemy_fields/types/__init__.py
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.3.0/sqlalchemy_fields/types/email.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.3.0/sqlalchemy_fields/types/file.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.3.0/sqlalchemy_fields/types/image.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.3.0/sqlalchemy_fields/types/ip.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.3.0/sqlalchemy_fields/types/url.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.3.0/sqlalchemy_fields/types/uuid.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.3.0/.gitignore
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.3.0/README.md
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/sqlalchemy_fields/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/sqlalchemy_fields/exceptions.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/sqlalchemy_fields/storages/__init__.py
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/sqlalchemy_fields/storages/base.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/sqlalchemy_fields/storages/filesystem.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/sqlalchemy_fields/storages/s3.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/sqlalchemy_fields/storages/utils.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/sqlalchemy_fields/types/__init__.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/sqlalchemy_fields/types/email.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/sqlalchemy_fields/types/file.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/sqlalchemy_fields/types/image.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/sqlalchemy_fields/types/ip.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/sqlalchemy_fields/types/url.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/sqlalchemy_fields/types/uuid.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/README.md
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 sqlalchemy_fields-0.4.0/PKG-INFO
```

### Comparing `sqlalchemy_fields-0.3.0/sqlalchemy_fields/storages/base.py` & `sqlalchemy_fields-0.4.0/sqlalchemy_fields/storages/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     def get_size(self, name: str) -> int:
         ...
 
     def open(self, name: str) -> BinaryIO:
         ...
 
-    def write(self, file: BinaryIO, name: str) -> None:
+    def write(self, file: BinaryIO, name: str) -> str:
         ...
 
 
 class StorageFile:
     """
     The file obect returned by the storage.
     """
@@ -48,23 +48,23 @@
     def open(self) -> BinaryIO:
         """
         Open a file handle of the file.
         """
 
         return self._storage.open(self._name)
 
-    def write(self, file: BinaryIO) -> None:
+    def write(self, file: BinaryIO) -> str:
         """
         Write input file which is opened in binary mode to destination.
         """
 
         return self._storage.write(file=file, name=self._name)
 
     def __str__(self) -> str:
-        return self.name
+        return self.path
 
 
 class StorageImage(StorageFile):
     """
     Inherits features of `StorageFile` and adds image specific properties.
     """
```

### Comparing `sqlalchemy_fields-0.3.0/sqlalchemy_fields/storages/filesystem.py` & `sqlalchemy_fields-0.4.0/sqlalchemy_fields/storages/filesystem.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,75 +1,65 @@
-import os
-import re
 from pathlib import Path
 from typing import BinaryIO
 
 from sqlalchemy_fields.storages.base import BaseStorage
-
-_filename_ascii_strip_re = re.compile(r"[^A-Za-z0-9_.-]")
+from sqlalchemy_fields.storages.utils import secure_filename
 
 
 class FileSystemStorage(BaseStorage):
     """
     File system storage which stores files in the local filesystem.
     You might want to use this with the `FileType` type.
     """
 
     default_chunk_size = 64 * 1024
 
     def __init__(self, path: str):
         self._path = Path(path)
-        if not self._path.exists():
-            self._path.mkdir()
+        self._path.mkdir(parents=True, exist_ok=True)
 
     def get_name(self, name: str) -> str:
         """
         Get the normalized name of the file.
         """
-        return secure_filename(name)
+
+        return secure_filename(Path(name).name)
 
     def get_path(self, name: str) -> str:
         """
         Get full path to the file.
         """
+
         return str(self._path / Path(name))
 
     def get_size(self, name: str) -> int:
         """
         Get file size in bytes.
         """
+
         return (self._path / name).stat().st_size
 
     def open(self, name: str) -> BinaryIO:
         """
         Open a file handle of the file object in binary mode.
         """
+
         path = self._path / Path(name)
         return open(path, "rb")
 
-    def write(self, file: BinaryIO, name: str) -> None:
+    def write(self, file: BinaryIO, name: str) -> str:
         """
         Write input file which is opened in binary mode to destination.
         """
+
         filename = secure_filename(name)
         path = self._path / Path(filename)
 
         file.seek(0, 0)
         with open(path, "wb") as output:
             while True:
                 chunk = file.read(self.default_chunk_size)
                 if not chunk:
                     break
                 output.write(chunk)
 
-
-def secure_filename(filename: str) -> str:
-    """
-    From Werkzeug secure_filename.
-    """
-    for sep in os.path.sep, os.path.altsep:
-        if sep:
-            filename = filename.replace(sep, " ")
-
-    normalized_filename = _filename_ascii_strip_re.sub("", "_".join(filename.split()))
-    filename = str(normalized_filename).strip("._")
-    return filename
+        return str(path)
```

### Comparing `sqlalchemy_fields-0.3.0/sqlalchemy_fields/types/email.py` & `sqlalchemy_fields-0.4.0/sqlalchemy_fields/types/email.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,16 +27,15 @@
         ```
     """
 
     impl = Unicode
     cache_ok = True
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
-        if email_validator is None:
-            raise ImportError("'email_validator' package is required.")
+        assert email_validator is not None, "'email_validator' package is required."
         super().__init__(*args, **kwargs)
 
     def process_bind_param(self, value: Any, dialect: Dialect) -> None:
         if value is None:
             return value
 
         try:
```

### Comparing `sqlalchemy_fields-0.3.0/sqlalchemy_fields/types/file.py` & `sqlalchemy_fields-0.4.0/sqlalchemy_fields/types/file.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,17 +29,21 @@
     def __init__(self, storage: BaseStorage, *args: Any, **kwargs: Any) -> None:
         self.storage = storage
         super().__init__(*args, **kwargs)
 
     def process_bind_param(self, value: Any, dialect: Dialect) -> Optional[str]:
         if value is None:
             return value
+        if len(value.file.read(1)) != 1:
+            return None
 
         file = StorageFile(name=value.filename, storage=self.storage)
         file.write(file=value.file)
+
+        value.file.close()
         return file.name
 
     def process_result_value(
         self, value: Any, dialect: Dialect
     ) -> Optional[StorageFile]:
         if value is None:
             return value
```

### Comparing `sqlalchemy_fields-0.3.0/sqlalchemy_fields/types/image.py` & `sqlalchemy_fields-0.4.0/sqlalchemy_fields/types/image.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from sqlalchemy.engine.interfaces import Dialect
 from sqlalchemy.types import TypeDecorator, Unicode
 
 try:
     from PIL import Image, UnidentifiedImageError
 
     PIL = True
-except ImportError:
+except ImportError:  # pragma: no cover
     PIL = False
 
 from sqlalchemy_fields.exceptions import ValidationException
 from sqlalchemy_fields.storages.base import BaseStorage, StorageImage
 
 
 class ImageType(TypeDecorator):
@@ -32,37 +32,41 @@
         ```
     """
 
     impl = Unicode
     cache_ok = True
 
     def __init__(self, storage: BaseStorage, *args: Any, **kwargs: Any) -> None:
-        if not PIL:
-            raise ImportError("'Pillow' package is required.")
+        assert PIL is True, "'Pillow' package is required."
 
         self.storage = storage
         super().__init__(*args, **kwargs)
 
     def process_bind_param(self, value: Any, dialect: Dialect) -> Optional[str]:
         if value is None:
             return value
+        if len(value.file.read(1)) != 1:
+            return None
 
         try:
             image_file = Image.open(value.file)
             image_file.verify()
         except UnidentifiedImageError:
             raise ValidationException("Invalid image file")
 
         image = StorageImage(
             name=value.filename,
             storage=self.storage,
             height=image_file.height,
             width=image_file.width,
         )
         image.write(file=value.file)
+
+        image_file.close()
+        value.file.close()
         return image.name
 
     def process_result_value(
         self, value: Any, dialect: Dialect
     ) -> Optional[StorageImage]:
         if value is None:
             return value
```

### Comparing `sqlalchemy_fields-0.3.0/sqlalchemy_fields/types/ip.py` & `sqlalchemy_fields-0.4.0/sqlalchemy_fields/types/ip.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_fields-0.3.0/sqlalchemy_fields/types/url.py` & `sqlalchemy_fields-0.4.0/sqlalchemy_fields/types/url.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_fields-0.3.0/sqlalchemy_fields/types/uuid.py` & `sqlalchemy_fields-0.4.0/sqlalchemy_fields/types/uuid.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_fields-0.3.0/.gitignore` & `sqlalchemy_fields-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sqlalchemy_fields-0.3.0/LICENSE.txt` & `sqlalchemy_fields-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sqlalchemy_fields-0.3.0/pyproject.toml` & `sqlalchemy_fields-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 dependencies = [
   "sqlalchemy>=1.4",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 full = [
+  "boto3~=1.25",
   "email-validator~=1.3",
   "Pillow~=9.4",
 ]
 
 [project.urls]
 Documentation = "https://github.com/aminalaee/sqlalchemy-fields#readme"
 Issues = "https://github.com/aminalaee/sqlalchemy-fields/issues"
@@ -56,18 +57,20 @@
 exclude = [
   "tests/*",
 ]
 
 [tool.hatch.envs.default]
 dependencies = [
   "black==22.10.0",
+  "boto3~=1.25",
   "build==0.9.0",
   "coverage==6.5.0",
   "email-validator==1.3.0",
   "isort==5.10.1",
+  "moto==4.1.2",
   "mypy==0.982",
   "Pillow==9.4.0",
   "psycopg2-binary==2.9.5",
   "pytest==7.2.0",
   "ruff==0.0.237",
 ]
```

