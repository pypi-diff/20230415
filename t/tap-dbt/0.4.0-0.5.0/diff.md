# Comparing `tmp/tap_dbt-0.4.0.tar.gz` & `tmp/tap_dbt-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_dbt-0.4.0.tar", max compression
+gzip compressed data, was "tap_dbt-0.5.0.tar", max compression
```

## Comparing `tap_dbt-0.4.0.tar` & `tap_dbt-0.5.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-03-30 18:53:04.947056 tap_dbt-0.4.0/LICENSE
--rw-r--r--   0        0        0     4798 2023-03-30 18:53:04.947056 tap_dbt-0.4.0/README.md
--rw-r--r--   0        0        0     1148 2023-03-30 18:53:04.951056 tap_dbt-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       40 2023-03-30 18:53:04.951056 tap_dbt-0.4.0/tap_dbt/__init__.py
--rw-r--r--   0        0        0     2360 2023-03-30 18:53:04.951056 tap_dbt-0.4.0/tap_dbt/client.py
--rw-r--r--   0        0        0     1780 2023-03-30 18:53:04.951056 tap_dbt-0.4.0/tap_dbt/schemas/accounts.json
--rw-r--r--   0        0        0     2264 2023-03-30 18:53:04.951056 tap_dbt-0.4.0/tap_dbt/schemas/jobs.json
--rw-r--r--   0        0        0     1821 2023-03-30 18:53:04.951056 tap_dbt-0.4.0/tap_dbt/schemas/projects.json
--rw-r--r--   0        0        0     3368 2023-03-30 18:53:04.951056 tap_dbt-0.4.0/tap_dbt/schemas/runs.json
--rw-r--r--   0        0        0     3086 2023-03-30 18:53:04.951056 tap_dbt-0.4.0/tap_dbt/streams.py
--rw-r--r--   0        0        0     1767 2023-03-30 18:53:04.951056 tap_dbt-0.4.0/tap_dbt/tap.py
--rw-r--r--   0        0        0     5692 1970-01-01 00:00:00.000000 tap_dbt-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-15 00:25:27.799289 tap_dbt-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5269 2023-04-15 00:25:27.799289 tap_dbt-0.5.0/README.md
+-rw-r--r--   0        0        0     1148 2023-04-15 00:25:27.799289 tap_dbt-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       40 2023-04-15 00:25:27.799289 tap_dbt-0.5.0/tap_dbt/__init__.py
+-rw-r--r--   0        0        0     2360 2023-04-15 00:25:27.799289 tap_dbt-0.5.0/tap_dbt/client.py
+-rw-r--r--   0        0        0     1780 2023-04-15 00:25:27.799289 tap_dbt-0.5.0/tap_dbt/schemas/accounts.json
+-rw-r--r--   0        0        0     2264 2023-04-15 00:25:27.803289 tap_dbt-0.5.0/tap_dbt/schemas/jobs.json
+-rw-r--r--   0        0        0     1821 2023-04-15 00:25:27.803289 tap_dbt-0.5.0/tap_dbt/schemas/projects.json
+-rw-r--r--   0        0        0     3368 2023-04-15 00:25:27.803289 tap_dbt-0.5.0/tap_dbt/schemas/runs.json
+-rw-r--r--   0        0        0     3538 2023-04-15 00:25:27.803289 tap_dbt-0.5.0/tap_dbt/streams.py
+-rw-r--r--   0        0        0     2033 2023-04-15 00:25:27.803289 tap_dbt-0.5.0/tap_dbt/tap.py
+-rw-r--r--   0        0        0     6163 1970-01-01 00:00:00.000000 tap_dbt-0.5.0/PKG-INFO
```

### Comparing `tap_dbt-0.4.0/LICENSE` & `tap_dbt-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.4.0/README.md` & `tap_dbt-0.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -51,45 +51,48 @@
 
 ```shell
 tap-dbt --config=config.json
 ```
 
 ### Inputs
 
-| Field         | Description                      | Type           | Required | Default                                          |
-|---------------|----------------------------------|----------------|----------|--------------------------------------------------|
-| `api_key`     | API key for the dbt Cloud API    | `string`       | yes      |                                                  |
-| `account_ids` | dbt Cloud account IDs            | `list(string)` | yes      |                                                  |
-| `user_agent`  | User-Agent to make requests with | `string`       | no       | `tap-dbt/0.1.0 Singer Tap for the dbt Cloud API` |
-| `base_url`    | Base URL for the dbt Cloud API   | `string`       | no       | `https://cloud.getdbt.com/api/v2`                |
+| Field         | Description                                                     | Type           | Required | Default                                          |
+|---------------|-----------------------------------------------------------------|----------------|----------|--------------------------------------------------|
+| `api_key`     | API key for the dbt Cloud API                                   | `string`       | yes      |                                                  |
+| `account_ids` | dbt Cloud account IDs                                           | `list(string)` | yes      |                                                  |
+| `user_agent`  | User-Agent to make requests with                                | `string`       | no       | `tap-dbt/0.1.0 Singer Tap for the dbt Cloud API` |
+| `base_url`    | Base URL for the dbt Cloud API                                  | `string`       | no       | `https://cloud.getdbt.com/api/v2`                |
+| `page_size`   | Number of records per API call, sets the `limit=` url parameter | `integer`      | no       | 5000                                             |
 
 A full list of supported settings and capabilities for this tap is available by running:
 
 ```shell
 tap-dbt --about --format json
 ```
 
 ### JSON example
 
 ```json
 {
   "api_key": "da39a3ee5e6b4b0d3255bfef95601890afd80709",
   "account_ids": ["51341"],
   "user_agent": "tap-dbt/0.1.0 Singer Tap for the dbt Cloud API",
-  "base_url": "https://my-dbt-cloud-api.com"
+  "base_url": "https://my-dbt-cloud-api.com",
+  "page_size": 5000
 }
 ```
 
 ### Environment variables example
 
 ```dotenv
 TAP_DBT_API_KEY=da39a3ee5e6b4b0d3255bfef95601890afd80709
 TAP_DBT_ACCOUNT_IDS=51341
 TAP_DBT_USER_AGENT='tap-dbt/0.1.0 Singer Tap for the dbt Cloud API'
 TAP_DBT_BASE_URL=https://my-dbt-cloud-api.com"
+TAP_DBT_PAGE_SIZE=5000
 ```
 
 ### Meltano Example
 
 ```yaml
 plugins:
   extractors:
@@ -114,14 +117,18 @@
           docs: "https://docs.getdbt.com/dbt-cloud/api#section/Authentication"
         - name: account_ids
           kind: array
           label: Account IDs
         - name: user_agent
           label: User-Agent
           placeholder: "tap-dbt/0.1.0 Singer Tap for the dbt Cloud API"
+        - name: page_size
+          kind: integer
+          label: Page Size
+
 ```
 
 ## Usage
 
 You can easily run `tap-dbt` with the CLI or using [Meltano][meltano].
 
 ### Executing the Tap Directly
```

### Comparing `tap_dbt-0.4.0/pyproject.toml` & `tap_dbt-0.5.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 [tool.isort]
 profile = "black"
 multi_line_output = 3 # Vertical Hanging Indent
 src_paths = "tap_dbt"
 
 [tool.poetry]
 name = "tap-dbt"
-version = "0.4.0"
+version = "0.5.0"
 description = "Singer tap for dbt, built with the Singer SDK."
 license = "Apache-2.0"
 authors = ["Edgar Ramírez Mondragón <edgarrm358@sample.com>"]
 maintainers = ["Edgar Ramírez Mondragón <edgarrm358@sample.com>"]
 readme = "README.md"
 repository = "https://github.com/edgarrmondragon/tap-dbt"
 keywords = ["singer.io", "elt", "dbt", "singer-sdk"]
 
 [tool.poetry.dependencies]
 python = "<3.12,>=3.7.1"
 pyyaml = "^6.0"
-singer-sdk = "==0.22.1"
+singer-sdk = "==0.24.0"
 
 [tool.poetry.group.dev.dependencies]
 faker = ">=17.6,<19.0"
 pytest = "^7.2.2"
 responses = "^0.23.1"
 
 [tool.poetry.scripts]
```

### Comparing `tap_dbt-0.4.0/tap_dbt/client.py` & `tap_dbt-0.5.0/tap_dbt/client.py`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.4.0/tap_dbt/schemas/accounts.json` & `tap_dbt-0.5.0/tap_dbt/schemas/accounts.json`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.4.0/tap_dbt/schemas/jobs.json` & `tap_dbt-0.5.0/tap_dbt/schemas/jobs.json`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.4.0/tap_dbt/schemas/projects.json` & `tap_dbt-0.5.0/tap_dbt/schemas/projects.json`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.4.0/tap_dbt/schemas/runs.json` & `tap_dbt-0.5.0/tap_dbt/schemas/runs.json`

 * *Files identical despite different names*

### Comparing `tap_dbt-0.4.0/tap_dbt/streams.py` & `tap_dbt-0.5.0/tap_dbt/streams.py`

 * *Files 20% similar despite different names*

```diff
@@ -55,29 +55,42 @@
             f"'{self.name}' ({self.path}). "
             "Expected a URL path containing '{account_id}'. "
         )
         raise ValueError(errmsg)
 
     def get_new_paginator(self) -> DbtPaginator:
         """Return a new paginator instance for this stream."""
-        return DbtPaginator(start_value=0, page_size=100)
+        page_size = self.config["page_size"]
+
+        self.logger.debug(
+            "Using page size of %s for the limit URL parameter",
+            page_size,
+        )
+
+        return DbtPaginator(start_value=0, page_size=page_size)
 
     def get_url_params(
         self,
         context: dict,
         next_page_token: int,
     ) -> dict:
         """Return offset as the next page token."""
         params = {}
         _ = context
+        # TODO: Get page size from the pagination object when it's available
+        # in this scope (https://github.com/meltano/sdk/issues/1606)
+        params["limit"] = self.config["page_size"]
 
         # Next page token is an offset
         if next_page_token:
             params["offset"] = next_page_token
 
+        self.logger.debug("context=%s", context)
+        self.logger.debug("params=%s", params)
+
         return params
 
 
 class AccountsStream(DBTStream):
     """A stream for the accounts endpoint."""
 
     name = "accounts"
@@ -104,8 +117,7 @@
 
 class RunsStream(AccountBasedStream):
     """A stream for the runs endpoint."""
 
     name = "runs"
     path = "/accounts/{account_id}/runs"
     openapi_ref = "Run"
-    page_size = 100
```

### Comparing `tap_dbt-0.4.0/tap_dbt/tap.py` & `tap_dbt-0.5.0/tap_dbt/tap.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 """dbt tap class."""
 
 from typing import List
 
 from singer_sdk import Stream, Tap
 from singer_sdk.helpers._classproperty import classproperty
-from singer_sdk.typing import ArrayType, PropertiesList, Property, StringType
+from singer_sdk.typing import (
+    ArrayType,
+    IntegerType,
+    PropertiesList,
+    Property,
+    StringType,
+)
 
 from tap_dbt.streams import AccountsStream, JobsStream, ProjectsStream, RunsStream
 
 TAP_NAME = "tap-dbt"
 STREAM_TYPES = [
     AccountsStream,
     JobsStream,
@@ -50,14 +56,21 @@
             ),
             Property(
                 "user_agent",
                 StringType,
                 default=f"{cls.name}/{cls.plugin_version} {cls.__doc__}",
                 description="User-Agent to make requests with",
             ),
+            Property(
+                "page_size",
+                IntegerType,
+                default=5000,
+                description="Page size to use in limit= url parameter",
+                required=True,
+            ),
         ).to_dict()
 
     def discover_streams(self) -> List[Stream]:
         """Return a list of discovered streams."""
         return [stream_class(tap=self) for stream_class in STREAM_TYPES]
```

### Comparing `tap_dbt-0.4.0/PKG-INFO` & `tap_dbt-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-dbt
-Version: 0.4.0
+Version: 0.5.0
 Summary: Singer tap for dbt, built with the Singer SDK.
 Home-page: https://github.com/edgarrmondragon/tap-dbt
 License: Apache-2.0
 Keywords: singer.io,elt,dbt,singer-sdk
 Author: Edgar Ramírez Mondragón
 Author-email: edgarrm358@sample.com
 Maintainer: Edgar Ramírez Mondragón
@@ -13,15 +13,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: singer-sdk (==0.22.1)
+Requires-Dist: singer-sdk (==0.24.0)
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-dbt
 Description-Content-Type: text/markdown
 
 # tap-dbt
 
 [![PyPI](https://img.shields.io/pypi/v/tap-dbt.svg?color=blue)](https://pypi.org/project/tap-dbt/)
 [![Python versions](https://img.shields.io/pypi/pyversions/tap-dbt.svg)](https://pypi.org/project/tap-dbt/)
@@ -74,45 +74,48 @@
 
 ```shell
 tap-dbt --config=config.json
 ```
 
 ### Inputs
 
-| Field         | Description                      | Type           | Required | Default                                          |
-|---------------|----------------------------------|----------------|----------|--------------------------------------------------|
-| `api_key`     | API key for the dbt Cloud API    | `string`       | yes      |                                                  |
-| `account_ids` | dbt Cloud account IDs            | `list(string)` | yes      |                                                  |
-| `user_agent`  | User-Agent to make requests with | `string`       | no       | `tap-dbt/0.1.0 Singer Tap for the dbt Cloud API` |
-| `base_url`    | Base URL for the dbt Cloud API   | `string`       | no       | `https://cloud.getdbt.com/api/v2`                |
+| Field         | Description                                                     | Type           | Required | Default                                          |
+|---------------|-----------------------------------------------------------------|----------------|----------|--------------------------------------------------|
+| `api_key`     | API key for the dbt Cloud API                                   | `string`       | yes      |                                                  |
+| `account_ids` | dbt Cloud account IDs                                           | `list(string)` | yes      |                                                  |
+| `user_agent`  | User-Agent to make requests with                                | `string`       | no       | `tap-dbt/0.1.0 Singer Tap for the dbt Cloud API` |
+| `base_url`    | Base URL for the dbt Cloud API                                  | `string`       | no       | `https://cloud.getdbt.com/api/v2`                |
+| `page_size`   | Number of records per API call, sets the `limit=` url parameter | `integer`      | no       | 5000                                             |
 
 A full list of supported settings and capabilities for this tap is available by running:
 
 ```shell
 tap-dbt --about --format json
 ```
 
 ### JSON example
 
 ```json
 {
   "api_key": "da39a3ee5e6b4b0d3255bfef95601890afd80709",
   "account_ids": ["51341"],
   "user_agent": "tap-dbt/0.1.0 Singer Tap for the dbt Cloud API",
-  "base_url": "https://my-dbt-cloud-api.com"
+  "base_url": "https://my-dbt-cloud-api.com",
+  "page_size": 5000
 }
 ```
 
 ### Environment variables example
 
 ```dotenv
 TAP_DBT_API_KEY=da39a3ee5e6b4b0d3255bfef95601890afd80709
 TAP_DBT_ACCOUNT_IDS=51341
 TAP_DBT_USER_AGENT='tap-dbt/0.1.0 Singer Tap for the dbt Cloud API'
 TAP_DBT_BASE_URL=https://my-dbt-cloud-api.com"
+TAP_DBT_PAGE_SIZE=5000
 ```
 
 ### Meltano Example
 
 ```yaml
 plugins:
   extractors:
@@ -137,14 +140,18 @@
           docs: "https://docs.getdbt.com/dbt-cloud/api#section/Authentication"
         - name: account_ids
           kind: array
           label: Account IDs
         - name: user_agent
           label: User-Agent
           placeholder: "tap-dbt/0.1.0 Singer Tap for the dbt Cloud API"
+        - name: page_size
+          kind: integer
+          label: Page Size
+
 ```
 
 ## Usage
 
 You can easily run `tap-dbt` with the CLI or using [Meltano][meltano].
 
 ### Executing the Tap Directly
```

