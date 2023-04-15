# Comparing `tmp/e621-data-0.0.1.tar.gz` & `tmp/e621-data-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e621-data-0.0.1.tar", last modified: Sat Apr 15 11:32:57 2023, max compression
+gzip compressed data, was "e621-data-1.0.0.tar", last modified: Sat Apr 15 11:51:58 2023, max compression
```

## Comparing `e621-data-0.0.1.tar` & `e621-data-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1066 2023-04-15 11:31:10.497048 e621-data-0.0.1/LICENSE
--rw-r--r--   0        0        0       39 2023-04-15 11:31:39.237116 e621-data-0.0.1/README.md
--rw-r--r--   0        0        0      189 2023-04-15 11:29:22.194609 e621-data-0.0.1/e621_data/__init__.py
--rw-r--r--   0        0        0     1032 2023-04-15 11:29:08.639051 e621-data-0.0.1/e621_data/download.py
--rw-r--r--   0        0        0     2716 2023-04-15 11:27:39.540065 e621-data-0.0.1/e621_data/posts.py
--rw-r--r--   0        0        0      806 2023-04-14 23:44:07.399257 e621-data-0.0.1/e621_data/tag_aliases.py
--rw-r--r--   0        0        0      834 2023-04-14 23:50:46.298698 e621-data-0.0.1/e621_data/tag_implications.py
--rw-r--r--   0        0        0      880 2023-04-14 23:58:21.067030 e621-data-0.0.1/e621_data/tags.py
--rw-r--r--   0        0        0      806 2023-04-15 11:32:29.973620 e621-data-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 e621-data-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-15 11:31:10.497048 e621-data-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1691 2023-04-15 11:51:45.955148 e621-data-1.0.0/README.md
+-rw-r--r--   0        0        0      189 2023-04-15 11:29:22.194609 e621-data-1.0.0/e621_data/__init__.py
+-rw-r--r--   0        0        0     2580 2023-04-15 11:46:22.011265 e621-data-1.0.0/e621_data/posts.py
+-rw-r--r--   0        0        0      766 2023-04-15 11:46:31.971103 e621-data-1.0.0/e621_data/tag_aliases.py
+-rw-r--r--   0        0        0      762 2023-04-15 11:46:37.955012 e621-data-1.0.0/e621_data/tag_implications.py
+-rw-r--r--   0        0        0      837 2023-04-15 11:45:06.297537 e621-data-1.0.0/e621_data/tags.py
+-rw-r--r--   0        0        0      434 2023-04-15 11:49:06.618007 e621-data-1.0.0/e621_data/utils.py
+-rw-r--r--   0        0        0      806 2023-04-15 11:51:57.023297 e621-data-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2381 1970-01-01 00:00:00.000000 e621-data-1.0.0/PKG-INFO
```

### Comparing `e621-data-0.0.1/LICENSE` & `e621-data-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `e621-data-0.0.1/e621_data/posts.py` & `e621-data-1.0.0/e621_data/posts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from .download import download
+from .utils import iterate_csv, parse_date_string
 from dataclasses import dataclass
+from pathlib import Path
 from datetime import datetime
 from csv import DictReader
 from typing import Iterator
 
 
 @dataclass(frozen=True, slots=True)
 class Post:
@@ -39,50 +40,47 @@
     is_pending: bool
     is_flagged: bool
     is_rating_locked: bool
     is_status_locked: bool
     is_note_locked: bool
 
 
-def load_posts() -> "Iterator[Post]":
-    filepath = download("posts")
-
-    with filepath.open("r") as f:
-        for line in DictReader(f):
-            yield Post(
-                id=int(line["id"]),
-
-                created_at=datetime.fromisoformat(line["created_at"]) if line["created_at"] else None,
-                updated_at=datetime.fromisoformat(line["updated_at"]) if line["updated_at"] else None,
-
-                parent_id=int(line["parent_id"]) if line["parent_id"] else None,
-                uploader_id=int(line["uploader_id"]),
-                approver_id=int(line["approver_id"]) if line["approver_id"] else None,
-
-                rating=str(line["rating"]),
-                tags=str(line["tag_string"]).split(" "),
-
-                description=str(line["description"]),
-                change_seq=int(line["change_seq"]),
-                source=str(line["source"]),
-                locked_tags=str(line["locked_tags"]),
-                fav_count=int(line["fav_count"]),
-                comment_count=int(line["comment_count"]),
-
-                duration=int(line["duration"]) if line["duration"] else None,
-                md5=str(line["md5"]),
-                file_size=int(line["file_size"]),
-                file_ext=str(line["file_ext"]),
-                image_width=int(line["image_width"]),
-                image_height=int(line["image_height"]),
-
-                score=int(line["score"]),
-                up_score=int(line["up_score"]),
-                down_score=int(line["down_score"]),
-
-                is_deleted=line["is_deleted"] == "t",
-                is_flagged=line["is_flagged"] == "t",
-                is_pending=line["is_pending"] == "t",
-                is_note_locked=line["is_note_locked"] == "t",
-                is_rating_locked=line["is_rating_locked"] == "t",
-                is_status_locked=line["is_status_locked"] == "t",
-            )
+def load_posts(filepath: str|Path) -> "Iterator[Post]":
+    for line in iterate_csv(filepath):
+        yield Post(
+            id=int(line["id"]),
+
+            created_at=parse_date_string(line["created_at"]) if line["created_at"] else None,
+            updated_at=parse_date_string(line["updated_at"]) if line["updated_at"] else None,
+
+            parent_id=int(line["parent_id"]) if line["parent_id"] else None,
+            uploader_id=int(line["uploader_id"]),
+            approver_id=int(line["approver_id"]) if line["approver_id"] else None,
+
+            rating=str(line["rating"]),
+            tags=str(line["tag_string"]).split(" "),
+
+            description=str(line["description"]),
+            change_seq=int(line["change_seq"]),
+            source=str(line["source"]),
+            locked_tags=str(line["locked_tags"]),
+            fav_count=int(line["fav_count"]),
+            comment_count=int(line["comment_count"]),
+
+            duration=int(line["duration"]) if line["duration"] else None,
+            md5=str(line["md5"]),
+            file_size=int(line["file_size"]),
+            file_ext=str(line["file_ext"]),
+            image_width=int(line["image_width"]),
+            image_height=int(line["image_height"]),
+
+            score=int(line["score"]),
+            up_score=int(line["up_score"]),
+            down_score=int(line["down_score"]),
+
+            is_deleted=line["is_deleted"] == "t",
+            is_flagged=line["is_flagged"] == "t",
+            is_pending=line["is_pending"] == "t",
+            is_note_locked=line["is_note_locked"] == "t",
+            is_rating_locked=line["is_rating_locked"] == "t",
+            is_status_locked=line["is_status_locked"] == "t",
+        )
```

### Comparing `e621-data-0.0.1/e621_data/tag_aliases.py` & `e621-data-1.0.0/e621_data/tag_aliases.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-from .download import download
+from .utils import iterate_csv, parse_date_string
 from dataclasses import dataclass
 from datetime import datetime
 from csv import DictReader
 from typing import Iterator
+from pathlib import Path
 
 
 @dataclass(frozen=True, slots=True)
 class TagAlias:
     id: int
     antecedent_name: str
     consequent_name: str
     created_at: "datetime|None"
     status: str
 
 
-def load_tag_aliases() -> "Iterator[TagAlias]":
-    filepath = download("tag_aliases")
-    with filepath.open("r") as f:
-        for line in DictReader(f):
-            yield TagAlias(
-                id=int(line["id"]),
-                antecedent_name=line["antecedent_name"],
-                consequent_name=line["consequent_name"],
-                created_at=datetime.fromisoformat(line["created_at"]) if line["created_at"] else None,
-                status=line["status"],
-            )
+def load_tag_aliases(filepath: str|Path) -> "Iterator[TagAlias]":
+    for line in iterate_csv(filepath):
+        yield TagAlias(
+            id=int(line["id"]),
+            antecedent_name=line["antecedent_name"],
+            consequent_name=line["consequent_name"],
+            created_at=parse_date_string(line["created_at"]) if line["created_at"] else None,
+            status=line["status"],
+        )
```

### Comparing `e621-data-0.0.1/e621_data/tag_implications.py` & `e621-data-1.0.0/e621_data/tag_implications.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-from .download import download
+from .utils import iterate_csv, parse_date_string
 from dataclasses import dataclass
 from datetime import datetime
-from csv import DictReader
 from typing import Iterator
+from pathlib import Path
 
 
 @dataclass(frozen=True, slots=True)
 class TagImplication:
     id: int
     antecedent_name: str
     consequent_name: str
     created_at: "datetime|None"
     status: str
 
 
-def load_tag_implications() -> "Iterator[TagImplication]":
-    filepath = download("tag_implications")
-    with filepath.open("r") as f:
-        for line in DictReader(f):
-            yield TagImplication(
-                id=int(line["id"]),
-                antecedent_name=line["antecedent_name"],
-                consequent_name=line["consequent_name"],
-                created_at=datetime.fromisoformat(line["created_at"]) if line["created_at"] else None,
-                status=line["status"],
-            )
+def load_tag_implications(filepath: str|Path) -> "Iterator[TagImplication]":
+    for line in iterate_csv(filepath):
+        yield TagImplication(
+            id=int(line["id"]),
+            antecedent_name=line["antecedent_name"],
+            consequent_name=line["consequent_name"],
+            created_at=parse_date_string(line["created_at"]) if line["created_at"] else None,
+            status=line["status"],
+        )
```

### Comparing `e621-data-0.0.1/e621_data/tags.py` & `e621-data-1.0.0/e621_data/tags.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-from .download import download
+from .utils import iterate_csv
 from dataclasses import dataclass
 from csv import DictReader
 from typing import Iterator
+from pathlib import Path
 
 
 @dataclass(frozen=True, slots=True)
 class Tag:
     id: int
     name: str
     category: str
     post_count: int
 
 
-def load_tags() -> "Iterator[Tag]":
-    filepath = download("tags")
-    with filepath.open("r") as f:
-        for line in DictReader(f):
-            yield Tag(
-                id=int(line["id"]),
-                name=line["name"],
-                category=category_number_to_name(line["category"]),
-                post_count=int(line["post_count"]),
-            )
+def load_tags(filepath: str|Path) -> "Iterator[Tag]":
+    for line in iterate_csv(filepath):
+        yield Tag(
+            id=int(line["id"]),
+            name=line["name"],
+            category=category_number_to_name(line["category"]),
+            post_count=int(line["post_count"]),
+        )
 
 
 def category_number_to_name(category: str) -> str:
     lookup = {
         0: "general",
         1: "artist",
         3: "copyright",
```

### Comparing `e621-data-0.0.1/pyproject.toml` & `e621-data-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.8.0,<4"]
 
 [project]
 name = "e621-data"
-version = "0.0.1"
+version = "1.0.0"
 description = "Load the e621 exported data"
 license = {file = "LICENSE"}
 readme = "README.md"
 authors = [
     {name = "Ben Brady", email = "benbradybusiness@gmail.com"},
 ]
 classifiers = [
```

