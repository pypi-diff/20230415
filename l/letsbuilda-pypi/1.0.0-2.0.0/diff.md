# Comparing `tmp/letsbuilda-pypi-1.0.0.tar.gz` & `tmp/letsbuilda-pypi-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "letsbuilda-pypi-1.0.0.tar", last modified: Wed Mar 29 22:11:41 2023, max compression
+gzip compressed data, was "letsbuilda-pypi-2.0.0.tar", last modified: Sat Apr 15 00:40:40 2023, max compression
```

## Comparing `letsbuilda-pypi-1.0.0.tar` & `letsbuilda-pypi-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 bradleyreynolds  (1000) bradleyreynolds  (1000)        0 2023-03-29 22:11:41.103110 letsbuilda-pypi-1.0.0/
--rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)     1074 2023-01-24 05:19:25.000000 letsbuilda-pypi-1.0.0/LICENSE
--rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)      588 2023-03-29 22:11:41.103110 letsbuilda-pypi-1.0.0/PKG-INFO
--rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)      113 2023-03-29 21:38:26.000000 letsbuilda-pypi-1.0.0/README.md
--rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)     1034 2023-03-29 21:19:38.000000 letsbuilda-pypi-1.0.0/pyproject.toml
--rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)       38 2023-03-29 22:11:41.103110 letsbuilda-pypi-1.0.0/setup.cfg
-drwxr-xr-x   0 bradleyreynolds  (1000) bradleyreynolds  (1000)        0 2023-03-29 22:11:41.099776 letsbuilda-pypi-1.0.0/src/
-drwxr-xr-x   0 bradleyreynolds  (1000) bradleyreynolds  (1000)        0 2023-03-29 22:11:41.099776 letsbuilda-pypi-1.0.0/src/letsbuilda/
-drwxr-xr-x   0 bradleyreynolds  (1000) bradleyreynolds  (1000)        0 2023-03-29 22:11:41.099776 letsbuilda-pypi-1.0.0/src/letsbuilda/pypi/
--rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)     2401 2023-03-29 21:55:11.000000 letsbuilda-pypi-1.0.0/src/letsbuilda/pypi/__init__.py
-drwxr-xr-x   0 bradleyreynolds  (1000) bradleyreynolds  (1000)        0 2023-03-29 22:11:41.103110 letsbuilda-pypi-1.0.0/src/letsbuilda_pypi.egg-info/
--rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)      588 2023-03-29 22:11:41.000000 letsbuilda-pypi-1.0.0/src/letsbuilda_pypi.egg-info/PKG-INFO
--rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)      310 2023-03-29 22:11:41.000000 letsbuilda-pypi-1.0.0/src/letsbuilda_pypi.egg-info/SOURCES.txt
--rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)        1 2023-03-29 22:11:41.000000 letsbuilda-pypi-1.0.0/src/letsbuilda_pypi.egg-info/dependency_links.txt
--rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)      109 2023-03-29 22:11:41.000000 letsbuilda-pypi-1.0.0/src/letsbuilda_pypi.egg-info/requires.txt
--rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)       11 2023-03-29 22:11:41.000000 letsbuilda-pypi-1.0.0/src/letsbuilda_pypi.egg-info/top_level.txt
-drwxr-xr-x   0 bradleyreynolds  (1000) bradleyreynolds  (1000)        0 2023-03-29 22:11:41.103110 letsbuilda-pypi-1.0.0/tests/
--rw-r--r--   0 bradleyreynolds  (1000) bradleyreynolds  (1000)     1611 2023-03-29 21:58:56.000000 letsbuilda-pypi-1.0.0/tests/test_new_packages_feed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:40:40.792339 letsbuilda-pypi-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-15 00:40:26.000000 letsbuilda-pypi-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-15 00:40:40.792339 letsbuilda-pypi-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-15 00:40:26.000000 letsbuilda-pypi-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-15 00:40:26.000000 letsbuilda-pypi-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 00:40:40.792339 letsbuilda-pypi-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:40:40.788339 letsbuilda-pypi-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:40:40.788339 letsbuilda-pypi-2.0.0/src/letsbuilda/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:40:40.792339 letsbuilda-pypi-2.0.0/src/letsbuilda/pypi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-15 00:40:26.000000 letsbuilda-pypi-2.0.0/src/letsbuilda/pypi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:40:40.792339 letsbuilda-pypi-2.0.0/src/letsbuilda_pypi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-15 00:40:40.000000 letsbuilda-pypi-2.0.0/src/letsbuilda_pypi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-15 00:40:40.000000 letsbuilda-pypi-2.0.0/src/letsbuilda_pypi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 00:40:40.000000 letsbuilda-pypi-2.0.0/src/letsbuilda_pypi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-15 00:40:40.000000 letsbuilda-pypi-2.0.0/src/letsbuilda_pypi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-15 00:40:40.000000 letsbuilda-pypi-2.0.0/src/letsbuilda_pypi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 00:40:40.792339 letsbuilda-pypi-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-15 00:40:26.000000 letsbuilda-pypi-2.0.0/tests/test_new_packages_feed.py
```

### Comparing `letsbuilda-pypi-1.0.0/LICENSE` & `letsbuilda-pypi-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `letsbuilda-pypi-1.0.0/PKG-INFO` & `letsbuilda-pypi-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: letsbuilda-pypi
-Version: 1.0.0
+Version: 2.0.0
 Summary: A wrapper for PyPI's API and RSS feed
 Author-email: Bradley Reynolds <bradley.reynolds@darbia.dev>
 License: MIT
 Project-URL: repository, https://github.com/letsbuilda/letsbuilda-pypi/
 Project-URL: documentation, https://docs.letsbuilda.dev/letsbuilda-pypi/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `letsbuilda-pypi-1.0.0/pyproject.toml` & `letsbuilda-pypi-2.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "letsbuilda-pypi"
-version = "1.0.0"
+version = "2.0.0"
 description = "A wrapper for PyPI's API and RSS feed"
 authors = [
     { name = "Bradley Reynolds", email = "bradley.reynolds@darbia.dev" },
 ]
 license = { text = "MIT" }
 readme = "README.md"
 requires-python = ">=3.10"
@@ -17,15 +17,15 @@
 repository = "https://github.com/letsbuilda/letsbuilda-pypi/"
 documentation = "https://docs.letsbuilda.dev/letsbuilda-pypi/"
 
 [project.optional-dependencies]
 dev = [
     "black",
     "isort",
-    "pylint",
+    "ruff",
 ]
 tests = [
     "pytest",
 ]
 docs = [
     "sphinx",
     "furo",
@@ -38,19 +38,19 @@
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.sphinx]
 copyright = "Let's build a ..."
 author = "Bradley Reynolds"
 
+[tool.isort]
+profile = "black"
+
 [tool.black]
 target-version = ["py310"]
 line-length = 120
 
-[tool.isort]
-profile = "black"
+[tool.ruff]
+line-length = 120
 
 [tool.pytest.ini_options]
 addopts = "tests -r a -v --doctest-modules src"
-
-[tool.pylint.format]
-max-line-length = 120
```

### Comparing `letsbuilda-pypi-1.0.0/src/letsbuilda/pypi/__init__.py` & `letsbuilda-pypi-2.0.0/src/letsbuilda/pypi/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,65 +7,58 @@
 from typing import Final
 
 import xmltodict
 from aiohttp import ClientSession
 
 __all__: list[str] = [
     "PyPIServices",
-    "NewPackageMetadata",
+    "PackageMetadata",
 ]
 
 
 def _parse_publication_date(publication_date: str) -> datetime:
     return datetime.strptime(publication_date, "%a, %d %b %Y %H:%M:%S %Z")
 
 
 @dataclass(frozen=True, slots=True)
-class NewPackageMetadata:
+class PackageMetadata:
     """Package metadata"""
 
     title: str
     package_link: str
     guid: str
     description: str | None
     author: str | None
     publication_date: datetime
 
     @classmethod
-    def build_from(cls, data: dict[str, str]) -> "NewPackageMetadata":
+    def build_from(cls, data: dict[str, str]) -> "PackageMetadata":
         """Build an instance from raw data"""
         publication_date: str | None = data.get("pubDate")
         if publication_date is not None:
             publication_date: datetime = _parse_publication_date(publication_date)
 
         return cls(
-            title=data.get("title").removesuffix(" added to PyPI"),
+            title=data.get("title").split()[0],
             package_link=data.get("link"),
             guid=data.get("guid"),
             description=data.get("description"),
             author=data.get("author"),
             publication_date=publication_date,
         )
 
 
 class PyPIServices:
     """A class for interacting with PyPI"""
 
     NEWEST_PACKAGES_FEED_URL: Final[str] = "https://pypi.org/rss/packages.xml"
     PACKAGE_UPDATES_FEED_URL: Final[str] = "https://pypi.org/rss/updates.xml"
 
-    def __init__(self, http_session: ClientSession | None = None) -> None:
-        self.http_session = http_session or ClientSession()
+    def __init__(self, http_session: ClientSession) -> None:
+        self.http_session = http_session
 
-    async def get_new_packages_feed(self) -> list[NewPackageMetadata]:
+    async def get_rss_feed(self, feed_url: str) -> list[PackageMetadata]:
         """Get the new packages RSS feed"""
-        async with self.http_session.get(self.NEWEST_PACKAGES_FEED_URL) as response:
+        async with self.http_session.get(feed_url) as response:
             response_text = await response.text()
             rss_data = xmltodict.parse(response_text)["rss"]["channel"]["item"]
-            return [NewPackageMetadata.build_from(package_data) for package_data in rss_data]
-
-    async def get_package_updates_feed(self) -> dict:
-        """Get the package updates RSS feed"""
-        async with self.http_session.get(self.PACKAGE_UPDATES_FEED_URL) as response:
-            response_text = await response.text()
-            rss_data = xmltodict.parse(response_text)["rss"]["channel"]["item"]
-            return rss_data
+            return [PackageMetadata.build_from(package_data) for package_data in rss_data]
```

### Comparing `letsbuilda-pypi-1.0.0/src/letsbuilda_pypi.egg-info/PKG-INFO` & `letsbuilda-pypi-2.0.0/src/letsbuilda_pypi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: letsbuilda-pypi
-Version: 1.0.0
+Version: 2.0.0
 Summary: A wrapper for PyPI's API and RSS feed
 Author-email: Bradley Reynolds <bradley.reynolds@darbia.dev>
 License: MIT
 Project-URL: repository, https://github.com/letsbuilda/letsbuilda-pypi/
 Project-URL: documentation, https://docs.letsbuilda.dev/letsbuilda-pypi/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `letsbuilda-pypi-1.0.0/tests/test_new_packages_feed.py` & `letsbuilda-pypi-2.0.0/tests/test_new_packages_feed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 """Test parsing metadata from the new packages RSS feed"""
 
 from datetime import datetime
 
-from letsbuilda.pypi import NewPackageMetadata
+from letsbuilda.pypi import PackageMetadata
 
 
 def test_parse_publication_date() -> None:
     """Confirm publication date gets parsed correctly"""
     data = {
         "title": "test-package added to PyPI",
         "link": "https://pypi.org/project/test-package",
         "guid": "https://pypi.org/project/test-package",
         "description": "a test package",
         "author": "test-author@example.com",
         "pubDate": "Wed, 29 Mar 2023 21:30:05 GMT",
     }
-    parsed_data = NewPackageMetadata.build_from(data)
+    parsed_data = PackageMetadata.build_from(data)
     assert parsed_data.publication_date == datetime(2023, 3, 29, 21, 30, 5)
 
 
 def test_author_missing() -> None:
     """Confirm missing author gets set to None"""
     data = {
         "title": "test-package added to PyPI",
         "link": "https://pypi.org/project/test-package",
         "guid": "https://pypi.org/project/test-package",
         "description": "a test package",
         "pubDate": "Wed, 29 Mar 2023 21:30:05 GMT",
     }
-    parsed_data = NewPackageMetadata.build_from(data)
+    parsed_data = PackageMetadata.build_from(data)
     assert parsed_data.author is None
 
 
 def test_description_missing() -> None:
     """Confirm missing description gets set to None"""
     data = {
         "title": "test-package added to PyPI",
         "link": "https://pypi.org/project/test-package",
         "guid": "https://pypi.org/project/test-package",
         "author": "test-author@example.com",
         "pubDate": "Wed, 29 Mar 2023 21:30:05 GMT",
     }
-    parsed_data = NewPackageMetadata.build_from(data)
+    parsed_data = PackageMetadata.build_from(data)
     assert parsed_data.description is None
```

