# Comparing `tmp/xata-0.8.0.tar.gz` & `tmp/xata-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xata-0.8.0.tar", max compression
+gzip compressed data, was "xata-0.9.0.tar", max compression
```

## Comparing `xata-0.8.0.tar` & `xata-0.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11357 2023-03-17 12:43:24.211669 xata-0.8.0/LICENSE
--rw-r--r--   0        0        0     1156 2023-03-17 12:43:24.211669 xata-0.8.0/README.md
--rw-r--r--   0        0        0      730 2023-03-17 12:43:24.215669 xata-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      844 2023-03-17 12:43:24.215669 xata-0.8.0/xata/__init__.py
--rw-r--r--   0        0        0    33026 2023-03-17 12:43:24.219669 xata-0.8.0/xata/client.py
--rw-r--r--   0        0        0     1715 2023-03-17 12:43:24.219669 xata-0.8.0/xata/errors.py
--rw-r--r--   0        0        0    10421 2023-03-17 12:43:24.219669 xata-0.8.0/xata/helpers.py
--rw-r--r--   0        0        0     2115 2023-03-17 12:43:24.219669 xata-0.8.0/xata/namespace.py
--rw-r--r--   0        0        0      769 2023-03-17 12:43:24.219669 xata-0.8.0/xata/namespaces/__init__.py
--rw-r--r--   0        0        0      769 2023-03-17 12:43:24.219669 xata-0.8.0/xata/namespaces/core/__init__.py
--rw-r--r--   0        0        0     2735 2023-03-17 12:43:24.219669 xata-0.8.0/xata/namespaces/core/authentication.py
--rw-r--r--   0        0        0     6251 2023-03-17 12:43:24.219669 xata-0.8.0/xata/namespaces/core/databases.py
--rw-r--r--   0        0        0     6273 2023-03-17 12:43:24.219669 xata-0.8.0/xata/namespaces/core/invites.py
--rw-r--r--   0        0        0     2623 2023-03-17 12:43:24.219669 xata-0.8.0/xata/namespaces/core/users.py
--rw-r--r--   0        0        0     7488 2023-03-17 12:43:24.219669 xata-0.8.0/xata/namespaces/core/workspaces.py
--rw-r--r--   0        0        0      769 2023-03-17 12:43:24.219669 xata-0.8.0/xata/namespaces/workspace/__init__.py
--rw-r--r--   0        0        0    12473 2023-03-17 12:43:24.219669 xata-0.8.0/xata/namespaces/workspace/branch.py
--rw-r--r--   0        0        0    10254 2023-03-17 12:43:24.219669 xata-0.8.0/xata/namespaces/workspace/migrations.py
--rw-r--r--   0        0        0    12766 2023-03-17 12:43:24.219669 xata-0.8.0/xata/namespaces/workspace/records.py
--rw-r--r--   0        0        0    29377 2023-03-17 12:43:24.219669 xata-0.8.0/xata/namespaces/workspace/search_and_filter.py
--rw-r--r--   0        0        0    13179 2023-03-17 12:43:24.219669 xata-0.8.0/xata/namespaces/workspace/table.py
--rw-r--r--   0        0        0     1867 1970-01-01 00:00:00.000000 xata-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-15 14:30:22.160620 xata-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1156 2023-04-15 14:30:22.160620 xata-0.9.0/README.md
+-rw-r--r--   0        0        0      749 2023-04-15 14:30:22.188621 xata-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      858 2023-04-15 14:30:22.188621 xata-0.9.0/xata/__init__.py
+-rw-r--r--   0        0        0    31957 2023-04-15 14:30:22.188621 xata-0.9.0/xata/client.py
+-rw-r--r--   0        0        0     1715 2023-04-15 14:30:22.188621 xata-0.9.0/xata/errors.py
+-rw-r--r--   0        0        0    10836 2023-04-15 14:30:22.188621 xata-0.9.0/xata/helpers.py
+-rw-r--r--   0        0        0     2115 2023-04-15 14:30:22.188621 xata-0.9.0/xata/namespace.py
+-rw-r--r--   0        0        0      769 2023-04-15 14:30:22.188621 xata-0.9.0/xata/namespaces/__init__.py
+-rw-r--r--   0        0        0      769 2023-04-15 14:30:22.188621 xata-0.9.0/xata/namespaces/core/__init__.py
+-rw-r--r--   0        0        0     2666 2023-04-15 14:30:22.188621 xata-0.9.0/xata/namespaces/core/authentication.py
+-rw-r--r--   0        0        0     6182 2023-04-15 14:30:22.188621 xata-0.9.0/xata/namespaces/core/databases.py
+-rw-r--r--   0        0        0     6204 2023-04-15 14:30:22.188621 xata-0.9.0/xata/namespaces/core/invites.py
+-rw-r--r--   0        0        0     2554 2023-04-15 14:30:22.188621 xata-0.9.0/xata/namespaces/core/users.py
+-rw-r--r--   0        0        0     7419 2023-04-15 14:30:22.188621 xata-0.9.0/xata/namespaces/core/workspaces.py
+-rw-r--r--   0        0        0      769 2023-04-15 14:30:22.188621 xata-0.9.0/xata/namespaces/workspace/__init__.py
+-rw-r--r--   0        0        0    12315 2023-04-15 14:30:22.188621 xata-0.9.0/xata/namespaces/workspace/branch.py
+-rw-r--r--   0        0        0    10143 2023-04-15 14:30:22.188621 xata-0.9.0/xata/namespaces/workspace/migrations.py
+-rw-r--r--   0        0        0    12491 2023-04-15 14:30:22.188621 xata-0.9.0/xata/namespaces/workspace/records.py
+-rw-r--r--   0        0        0    29615 2023-04-15 14:30:22.188621 xata-0.9.0/xata/namespaces/workspace/search_and_filter.py
+-rw-r--r--   0        0        0    12792 2023-04-15 14:30:22.188621 xata-0.9.0/xata/namespaces/workspace/table.py
+-rw-r--r--   0        0        0     1867 1970-01-01 00:00:00.000000 xata-0.9.0/PKG-INFO
```

### Comparing `xata-0.8.0/LICENSE` & `xata-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xata-0.8.0/README.md` & `xata-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `xata-0.8.0/pyproject.toml` & `xata-0.9.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xata"
-version = "0.8.0"
+version = "0.9.0"
 description = "Python client for Xata.io"
 authors = ["Xata <support@xata.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 documentation = "https://xata-py.readthedocs.io"
 
 [tool.poetry.dependencies]
@@ -23,11 +23,12 @@
 isort = "^5.12.0"
 flake8-bugbear = "^22.10.27"
 flake8-annotations = "^2.9.1"
 pdoc3 = "^0.10.0"
 Faker = "^17.0.0"
 sphinx-rtd-theme = "^1.2.0"
 mako = "^1.2.4"
+pytz = "^2022.7.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `xata-0.8.0/xata/__init__.py` & `xata-0.9.0/xata/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
 
 from .client import XataClient
 
-__all__ = ("XataClient", "BulkProcessor")
+__all__ = ("XataClient", "BulkProcessor", "to_rfc3339")
```

### Comparing `xata-0.8.0/xata/client.py` & `xata-0.9.0/xata/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 from .namespaces.workspace.migrations import Migrations
 from .namespaces.workspace.records import Records
 from .namespaces.workspace.search_and_filter import Search_and_filter
 from .namespaces.workspace.table import Table
 
 # TODO this is a manual task, to keep in sync with pyproject.toml
 # could/should be automated to keep in sync
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 PERSONAL_API_KEY_LOCATION = "~/.config/xata/key"
 DEFAULT_DATA_PLANE_DOMAIN = "xata.sh"
 DEFAULT_CONTROL_PLANE_DOMAIN = "api.xata.io"
 DEFAULT_REGION = "us-east-1"
 DEFAULT_BRANCH_NAME = "main"
 CONFIG_LOCATION = ".xatarc"
@@ -129,22 +129,35 @@
 
         self.db_name = self.get_database_name_if_configured() if db_name is None else db_name
         self.branch_name = self.get_branch_name_if_configured() if branch_name is None else branch_name
 
         self.domain_core = domain_core
         self.domain_workspace = domain_workspace
 
+        # init default headers
         self.headers = {
             "authorization": f"Bearer {self.api_key}",
             "user-agent": f"xataio/xata-py:{__version__}",
             "x-xata-client-id": str(uuid.uuid4()),
             "x-xata-session-id": str(uuid.uuid4()),
             "x-xata-agent": f"client=PY_SDK;version={__version__};",
         }
 
+        # init namespaces
+        self._authentication = Authentication(self)
+        self._branch = Branch(self)
+        self._search_and_filter = Search_and_filter(self)
+        self._databases = Databases(self)
+        self._invites = Invites(self)
+        self._migrations = Migrations(self)
+        self._records = Records(self)
+        self._table = Table(self)
+        self._users = Users(self)
+        self._workspaces = Workspaces(self)
+
     def get_config(self) -> dict:
         """
         Get the configuration
         """
         return {
             "apiKey": self.api_key,
             "apiKeyLocation": self.api_key_location,
@@ -743,118 +756,83 @@
             expect_codes=[200, 400, 403, 404, 500],
         )
 
         if result.status_code == 400:
             raise BadRequestException(result.status_code, result.json()["message"])
         return result.json()
 
-    # --------------------------------------------------- #
-    #
-    # Namespace: CORE
-    #
-    # --------------------------------------------------- #
-
     def authentication(self) -> Authentication:
         """
         Authentication Namespace
-        scope: core
         :return Authentication
         """
-        if "authentication" not in self.namespaces:
-            self.namespaces["authentication"] = Authentication(self)
-        return self.namespaces["authentication"]
+        return self._authentication
 
     def databases(self) -> Databases:
         """
         Databases Namespace
-        scope: core
         :return Databases
         """
-        if "databases" not in self.namespaces:
-            self.namespaces["databases"] = Databases(self)
-        return self.namespaces["databases"]
+        return self._databases
 
     def invites(self) -> Invites:
         """
         Invites Namespace
-        scope: core
         :return Invites
         """
-        if "invites" not in self.namespaces:
-            self.namespaces["invites"] = Invites(self)
-        return self.namespaces["invites"]
+        return self._invites
 
     def users(self) -> Users:
         """
         Users Namespace
-        scope: core
         :return Users
         """
-        if "users" not in self.namespaces:
-            self.namespaces["users"] = Users(self)
-        return self.namespaces["users"]
+        return self._users
 
     def workspaces(self) -> Workspaces:
         """
         Workspaces Namespace
-        scope: core
         :return Workspaces
         """
-        if "workspaces" not in self.namespaces:
-            self.namespaces["workspaces"] = Workspaces(self)
-        return self.namespaces["workspaces"]
-
-    # --------------------------------------------------- #
-    #
-    # Namespace: WORKSPACE
-    #
-    # --------------------------------------------------- #
+        return self._workspaces
 
     def branch(self) -> Branch:
         """
         Branch Namespace
-        scope: workspace
         :return Branch
         """
-        if "branch" not in self.namespaces:
-            self.namespaces["branch"] = Branch(self)
-        return self.namespaces["branch"]
+        return self._branch
 
     def migrations(self) -> Migrations:
         """
         Migrations Namespace
-        scope: workspace
         :return Migrations
         """
-        if "migrations" not in self.namespaces:
-            self.namespaces["migrations"] = Migrations(self)
-        return self.namespaces["migrations"]
+        return self._migrations
 
     def records(self) -> Records:
         """
         Records Namespace
-        scope: workspace
         :return Records
         """
-        if "records" not in self.namespaces:
-            self.namespaces["records"] = Records(self)
-        return self.namespaces["records"]
+        return self._records
 
     def search_and_filter(self) -> Search_and_filter:
         """
         Search_and_Filter Namespace
-        scope: workspace
         :return Search_and_filter
         """
-        if "search_and_filter" not in self.namespaces:
-            self.namespaces["search_and_filter"] = Search_and_filter(self)
-        return self.namespaces["search_and_filter"]
+        return self._search_and_filter
+
+    def data(self) -> Search_and_filter:
+        """
+        Shorter alias for Search_and_Filter
+        :return Search_and_filter
+        """
+        return self._search_and_filter
 
     def table(self) -> Table:
         """
         Table Namespace
-        scope: workspace
         :return Table
         """
-        if "table" not in self.namespaces:
-            self.namespaces["table"] = Table(self)
-        return self.namespaces["table"]
+        return self._table
```

### Comparing `xata-0.8.0/xata/errors.py` & `xata-0.9.0/xata/errors.py`

 * *Files identical despite different names*

### Comparing `xata-0.8.0/xata/helpers.py` & `xata-0.9.0/xata/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
 
 import logging
 import time
-from datetime import datetime
+from datetime import datetime, timezone
 from threading import Lock, Thread
 
 from .client import XataClient
 
 DEFAULT_THREAD_POOL_SIZE = 4
 DEFAULT_BATCH_SIZE = 25
 DEFAULT_FLUSH_INTERVAL = 5
@@ -269,7 +269,20 @@
 
         def size(self) -> int:
             """
             Get total size of stored records
             """
             with self.lock:
                 return sum([len(self.store[n]["records"]) for n in self.store.keys()])
+
+
+def to_rfc339(dt: datetime, tz=timezone.utc) -> str:
+    """
+    Format a datetime object to an RFC3339 compliant string
+    :link https://xata.io/docs/concepts/data-model#datetime
+    :link https://datatracker.ietf.org/doc/html/rfc3339
+
+    :param dt: datetime instance to convert
+    :param tz: timezone to convert in, default: UTC
+    :return str
+    """
+    return dt.replace(tzinfo=tz).isoformat()
```

### Comparing `xata-0.8.0/xata/namespace.py` & `xata-0.9.0/xata/namespace.py`

 * *Files identical despite different names*

### Comparing `xata-0.8.0/xata/namespaces/__init__.py` & `xata-0.9.0/xata/namespaces/__init__.py`

 * *Files identical despite different names*

### Comparing `xata-0.8.0/xata/namespaces/core/__init__.py` & `xata-0.9.0/xata/namespaces/core/__init__.py`

 * *Files identical despite different names*

### Comparing `xata-0.8.0/xata/namespaces/core/authentication.py` & `xata-0.9.0/xata/namespaces/core/authentication.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,25 +17,23 @@
 # under the License.
 #
 
 # ------------------------------------------------------- #
 # Authentication
 # Authentication and API Key management.
 # Specification: core:v1.0
-# Base URL: https://api.xata.io
 # ------------------------------------------------------- #
 
 from requests import Response
 
 from xata.namespace import Namespace
 
 
 class Authentication(Namespace):
 
-    base_url = "https://api.xata.io"
     scope = "core"
 
     def getUserAPIKeys(
         self,
     ) -> Response:
         """
         Retrieve a list of existing user API keys
```

### Comparing `xata-0.8.0/xata/namespaces/core/databases.py` & `xata-0.9.0/xata/namespaces/core/databases.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,25 +17,23 @@
 # under the License.
 #
 
 # ------------------------------------------------------- #
 # Databases
 # Workspace databases management.
 # Specification: core:v1.0
-# Base URL: https://api.xata.io
 # ------------------------------------------------------- #
 
 from requests import Response
 
 from xata.namespace import Namespace
 
 
 class Databases(Namespace):
 
-    base_url = "https://api.xata.io"
     scope = "core"
 
     def getDatabaseList(self, workspace_id: str = None) -> Response:
         """
         List all databases available in your Workspace.
 
         Path: /workspaces/{workspace_id}/dbs
```

### Comparing `xata-0.8.0/xata/namespaces/core/invites.py` & `xata-0.9.0/xata/namespaces/core/invites.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,25 +17,23 @@
 # under the License.
 #
 
 # ------------------------------------------------------- #
 # Invites
 # Manage user invites.
 # Specification: core:v1.0
-# Base URL: https://api.xata.io
 # ------------------------------------------------------- #
 
 from requests import Response
 
 from xata.namespace import Namespace
 
 
 class Invites(Namespace):
 
-    base_url = "https://api.xata.io"
     scope = "core"
 
     def inviteWorkspaceMember(self, payload: dict, workspace_id: str = None) -> Response:
         """
         Invite some user to join the workspace with the given role
 
         Path: /workspaces/{workspace_id}/invites
```

### Comparing `xata-0.8.0/xata/namespaces/core/users.py` & `xata-0.9.0/xata/namespaces/core/users.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,25 +17,23 @@
 # under the License.
 #
 
 # ------------------------------------------------------- #
 # Users
 # Users management
 # Specification: core:v1.0
-# Base URL: https://api.xata.io
 # ------------------------------------------------------- #
 
 from requests import Response
 
 from xata.namespace import Namespace
 
 
 class Users(Namespace):
 
-    base_url = "https://api.xata.io"
     scope = "core"
 
     def getUser(
         self,
     ) -> Response:
         """
         Return details of the user making the request
```

### Comparing `xata-0.8.0/xata/namespaces/core/workspaces.py` & `xata-0.9.0/xata/namespaces/core/workspaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,25 +17,23 @@
 # under the License.
 #
 
 # ------------------------------------------------------- #
 # Workspaces
 # Workspaces management
 # Specification: core:v1.0
-# Base URL: https://api.xata.io
 # ------------------------------------------------------- #
 
 from requests import Response
 
 from xata.namespace import Namespace
 
 
 class Workspaces(Namespace):
 
-    base_url = "https://api.xata.io"
     scope = "core"
 
     def getWorkspacesList(
         self,
     ) -> Response:
         """
         Retrieve the list of workspaces the user belongs to
```

### Comparing `xata-0.8.0/xata/namespaces/workspace/__init__.py` & `xata-0.9.0/xata/namespaces/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `xata-0.8.0/xata/namespaces/workspace/branch.py` & `xata-0.9.0/xata/namespaces/workspace/branch.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,25 +17,23 @@
 # under the License.
 #
 
 # ------------------------------------------------------- #
 # Branch
 # Branch management.
 # Specification: workspace:v1.0
-# Base URL: https://{workspaceId}.{regionId}.xata.sh
 # ------------------------------------------------------- #
 
 from requests import Response
 
 from xata.namespace import Namespace
 
 
 class Branch(Namespace):
 
-    base_url = "https://{workspaceId}.{regionId}.xata.sh"
     scope = "workspace"
 
     def getBranchList(self, db_name: str) -> Response:
         """
         List all available Branches
 
         Path: /dbs/{db_name}
@@ -74,21 +72,15 @@
 
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}"
         return self.request("GET", url_path)
 
-    def createBranch(
-        self,
-        payload: dict,
-        db_name: str = None,
-        branch_name: str = None,
-        _from: str = None,
-    ) -> Response:
+    def createBranch(self, payload: dict, db_name: str = None, branch_name: str = None, _from: str = None) -> Response:
         """
         Create Database branch
 
         Path: /db/{db_branch_name}
         Method: PUT
         Response status codes:
         - 201: Created
```

### Comparing `xata-0.8.0/xata/namespaces/workspace/migrations.py` & `xata-0.9.0/xata/namespaces/workspace/migrations.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,25 +17,23 @@
 # under the License.
 #
 
 # ------------------------------------------------------- #
 # Migrations
 # Branch schema migrations and history.
 # Specification: workspace:v1.0
-# Base URL: https://{workspaceId}.{regionId}.xata.sh
 # ------------------------------------------------------- #
 
 from requests import Response
 
 from xata.namespace import Namespace
 
 
 class Migrations(Namespace):
 
-    base_url = "https://{workspaceId}.{regionId}.xata.sh"
     scope = "workspace"
 
     def getBranchMigrationHistory(self, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
         """
         Get branch migration history [deprecated]
 
         Path: /db/{db_branch_name}/migrations
```

### Comparing `xata-0.8.0/xata/namespaces/workspace/records.py` & `xata-0.9.0/xata/namespaces/workspace/records.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,25 +17,23 @@
 # under the License.
 #
 
 # ------------------------------------------------------- #
 # Records
 # Record access API.
 # Specification: workspace:v1.0
-# Base URL: https://{workspaceId}.{regionId}.xata.sh
 # ------------------------------------------------------- #
 
 from requests import Response
 
 from xata.namespace import Namespace
 
 
 class Records(Namespace):
 
-    base_url = "https://{workspaceId}.{regionId}.xata.sh"
     scope = "workspace"
 
     def branchTransaction(self, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
         """
         Execute a transaction on a branch
 
         Path: /db/{db_branch_name}/transaction
@@ -56,20 +54,15 @@
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/transaction"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def insertRecord(
-        self,
-        table_name: str,
-        payload: dict,
-        db_name: str = None,
-        branch_name: str = None,
-        columns: list = None,
+        self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None, columns: list = None
     ) -> Response:
         """
         Insert a new Record into the Table
 
         Path: /db/{db_branch_name}/tables/{table_name}/data
         Method: POST
         Response status codes:
@@ -91,20 +84,15 @@
         url_path = f"/db/{db_branch_name}/tables/{table_name}/data"
         if columns is not None:
             url_path += "?columns=%s" % ",".join(columns)
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def getRecord(
-        self,
-        table_name: str,
-        record_id: str,
-        db_name: str = None,
-        branch_name: str = None,
-        columns: list = None,
+        self, table_name: str, record_id: str, db_name: str = None, branch_name: str = None, columns: list = None
     ) -> Response:
         """
         Retrieve record by ID
 
         Path: /db/{db_branch_name}/tables/{table_name}/data/{record_id}
         Method: GET
         Response status codes:
@@ -223,20 +211,15 @@
             query_params.append(f"ifVersion={ifVersion}")
         if query_params:
             url_path += "?" + "&".join(query_params)
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def deleteRecord(
-        self,
-        table_name: str,
-        record_id: str,
-        db_name: str = None,
-        branch_name: str = None,
-        columns: list = None,
+        self, table_name: str, record_id: str, db_name: str = None, branch_name: str = None, columns: list = None
     ) -> Response:
         """
         Delete record from table
 
         Path: /db/{db_branch_name}/tables/{table_name}/data/{record_id}
         Method: DELETE
         Response status codes:
@@ -303,20 +286,15 @@
             query_params.append(f"ifVersion={ifVersion}")
         if query_params:
             url_path += "?" + "&".join(query_params)
         headers = {"content-type": "application/json"}
         return self.request("PATCH", url_path, headers, payload)
 
     def bulkInsertTableRecords(
-        self,
-        table_name: str,
-        payload: dict,
-        db_name: str = None,
-        branch_name: str = None,
-        columns: list = None,
+        self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None, columns: list = None
     ) -> Response:
         """
         Bulk insert records
 
         Path: /db/{db_branch_name}/tables/{table_name}/bulk
         Method: POST
         Response status codes:
```

### Comparing `xata-0.8.0/xata/namespaces/workspace/search_and_filter.py` & `xata-0.9.0/xata/namespaces/workspace/search_and_filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,34 +17,26 @@
 # under the License.
 #
 
 # ------------------------------------------------------- #
 # Search_and_filter
 # APIs for searching, querying, filtering, and aggregating records.
 # Specification: workspace:v1.0
-# Base URL: https://{workspaceId}.{regionId}.xata.sh
 # ------------------------------------------------------- #
 
 from requests import Response
 
 from xata.namespace import Namespace
 
 
 class Search_and_filter(Namespace):
 
-    base_url = "https://{workspaceId}.{regionId}.xata.sh"
     scope = "workspace"
 
-    def queryTable(
-        self,
-        table_name: str,
-        payload: dict,
-        db_name: str = None,
-        branch_name: str = None,
-    ) -> Response:
+    def queryTable(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
         """
         The Query Table API can be used to retrieve all records in a table.  The API support
         filtering, sorting, selecting a subset of columns, and pagination.  The overall structure
         of the request looks like this:  ```json // POST
         /db/<dbname>:<branch>/tables/<table>/query {   "columns": [...],   "filter": {     "$all":
         [...],     "$any": [...]     ...   },   "sort": {     "multiple": [...]     ...   },
         "page": {     ...   } } ```  For usage, see also the [API Guide](https://xata.io/docs/api-
@@ -155,15 +147,21 @@
         example of using the `$includesAll` operator:  ```json {   "filter": {
         "settings.labels": {       "$includesAll": [{ "$contains": "label" }]     }   } } ```  The
         above matches if all array values contain the string "label".  ### Sorting  Sorting by one
         element:  ```json POST /db/demo:main/tables/table/query {   "sort": {     "index": "asc"
         } } ```  or descendently:  ```json POST /db/demo:main/tables/table/query {   "sort": {
         "index": "desc"   } } ```  Sorting by multiple fields:  ```json POST
         /db/demo:main/tables/table/query {   "sort": [     {       "index": "desc"     },     {
-        "createdAt": "desc"     }   ] } ```  ### Pagination  We offer cursor pagination and offset
+        "createdAt": "desc"     }   ] } ```  It is also possible to sort results randomly:
+        ```json POST /db/demo:main/tables/table/query {   "sort": {     "*": "random"   } } ```
+        Note that a random sort does not apply to a specific column, hence the special column name
+        `"*"`.  A random sort can be combined with an ascending or descending sort on a specific
+        column:  ```json POST /db/demo:main/tables/table/query {   "sort": [     {       "name":
+        "desc"     },     {       "*": "random"     }   ] } ```  This will sort on the `name`
+        column, breaking ties randomly.  ### Pagination  We offer cursor pagination and offset
         pagination.  For queries that are expected to return more than 1000 records, cursor
         pagination is needed in order to retrieve all of their results.  The offset pagination
         method is limited to 1000 records.  Example of size + offset pagination:  ```json POST
         /db/demo:main/tables/table/query {   "page": {     "size": 100,     "offset": 200   } }
         ```  The `page.size` parameter represents the maximum number of records returned by this
         query.  It has a default value of 20 and a maximum value of 200. The `page.offset`
         parameter represents the number of matching records to skip.  It has a default value of 0
@@ -251,21 +249,15 @@
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/search"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
-    def searchTable(
-        self,
-        table_name: str,
-        payload: dict,
-        db_name: str = None,
-        branch_name: str = None,
-    ) -> Response:
+    def searchTable(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
         """
         Run a free text search operation in a particular table.  The endpoint accepts a `query`
         parameter that is used for the free text search and a set of structured filters (via the
         `filter` parameter) that are applied before the search.  The `filter` parameter uses the
         same syntax as the [query endpoint](/api-reference/db/db_branch_name/tables/table_name/)
         with the following exceptions: * filters `$contains`, `$startsWith`, `$endsWith` don't
         work on columns of type `text` * filtering on columns of type `multiple` is currently
@@ -289,19 +281,15 @@
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/search"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
     def vectorSearchTable(
-        self,
-        table_name: str,
-        payload: dict,
-        db_name: str = None,
-        branch_name: str = None,
+        self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None
     ) -> Response:
         """
         This endpoint can be used to perform vector-based similarity searches in a table.  It can
         be used for implementing semantic search and product recommendation.  To use this
         endpoint, you need a column of type vector.  The input vector must have the same dimension
         as the vector column.
 
@@ -364,21 +352,15 @@
         url_path = f"/db/{db_branch_name}/tables/{table_name}/ask"
         headers = {
             "content-type": "application/json",
             "accept": response_content_type,
         }
         return self.request("POST", url_path, headers, payload)
 
-    def summarizeTable(
-        self,
-        table_name: str,
-        payload: dict,
-        db_name: str = None,
-        branch_name: str = None,
-    ) -> Response:
+    def summarizeTable(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
         """
         This endpoint allows you to (optionally) define groups, and then to run calculations on
         the values in each group.  This is most helpful when  you'd like to understand the data
         you have in your database.  A group is a combination of unique values.  If you create a
         group for  `sold_by`, `product_name`, we will return one row for every combination  of
         `sold_by` and `product_name` you have in your database.  When you  want to calculate
         statistics, you define these groups and ask Xata to  calculate data on each group.  **Some
@@ -427,21 +409,15 @@
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/summarize"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
-    def aggregateTable(
-        self,
-        table_name: str,
-        payload: dict,
-        db_name: str = None,
-        branch_name: str = None,
-    ) -> Response:
+    def aggregateTable(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
         """
         This endpoint allows you to run aggregations (analytics) on the data from one table.
         While the summary endpoint is served from a transactional store and the results are
         strongly  consistent, the aggregate endpoint is served from our columnar store and the
         results are  only eventually consistent.  On the other hand, the aggregate endpoint uses a
         store that is more appropiate for analytics, makes use of approximative algorithms  (e.g
         for cardinality), and is generally faster and can do more complex aggregations.  For
```

### Comparing `xata-0.8.0/xata/namespaces/workspace/table.py` & `xata-0.9.0/xata/namespaces/workspace/table.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,25 +17,23 @@
 # under the License.
 #
 
 # ------------------------------------------------------- #
 # Table
 # Table management.
 # Specification: workspace:v1.0
-# Base URL: https://{workspaceId}.{regionId}.xata.sh
 # ------------------------------------------------------- #
 
 from requests import Response
 
 from xata.namespace import Namespace
 
 
 class Table(Namespace):
 
-    base_url = "https://{workspaceId}.{regionId}.xata.sh"
     scope = "workspace"
 
     def createTable(self, table_name: str, db_name: str = None, branch_name: str = None) -> Response:
         """
         Creates a new table with the given name.  Returns 422 if a table with the same name
         already exists.
 
@@ -81,21 +79,15 @@
 
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}"
         return self.request("DELETE", url_path)
 
-    def updateTable(
-        self,
-        table_name: str,
-        payload: dict,
-        db_name: str = None,
-        branch_name: str = None,
-    ) -> Response:
+    def updateTable(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
         """
         Update table.  Currently there is only one update operation supported: renaming the table
         by providing a new name.  In the example below, we rename a table from “users” to
         “people”:  ```json // PATCH /db/test:main/tables/users  {   "name": "people" } ```
 
         Path: /db/{db_branch_name}/tables/{table_name}
         Method: PATCH
@@ -139,21 +131,15 @@
 
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/schema"
         return self.request("GET", url_path)
 
-    def setTableSchema(
-        self,
-        table_name: str,
-        payload: dict,
-        db_name: str = None,
-        branch_name: str = None,
-    ) -> Response:
+    def setTableSchema(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
         """
         Update table schema
 
         Path: /db/{db_branch_name}/tables/{table_name}/schema
         Method: PUT
         Response status codes:
         - 200: Schema migration response with ID and migration status.
@@ -198,21 +184,15 @@
 
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/columns"
         return self.request("GET", url_path)
 
-    def addTableColumn(
-        self,
-        table_name: str,
-        payload: dict,
-        db_name: str = None,
-        branch_name: str = None,
-    ) -> Response:
+    def addTableColumn(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> Response:
         """
         Adds a new column to the table.  The body of the request should contain the column
         definition.  In the column definition, the 'name' field should contain the full path
         separated by dots.  If the parent objects do not exists, they will be automatically
         created.  For example, passing `"name": "address.city"` will auto-create the `address`
         object if it doesn't exist.
 
@@ -233,21 +213,15 @@
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/columns"
         headers = {"content-type": "application/json"}
         return self.request("POST", url_path, headers, payload)
 
-    def getColumn(
-        self,
-        table_name: str,
-        column_name: str,
-        db_name: str = None,
-        branch_name: str = None,
-    ) -> Response:
+    def getColumn(self, table_name: str, column_name: str, db_name: str = None, branch_name: str = None) -> Response:
         """
         Get the definition of a single column.  To refer to sub-objects, the column name can
         contain dots.  For example `address.country`.
 
         Path: /db/{db_branch_name}/tables/{table_name}/columns/{column_name}
         Method: GET
         Response status codes:
@@ -265,21 +239,15 @@
 
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/columns/{column_name}"
         return self.request("GET", url_path)
 
-    def deleteColumn(
-        self,
-        table_name: str,
-        column_name: str,
-        db_name: str = None,
-        branch_name: str = None,
-    ) -> Response:
+    def deleteColumn(self, table_name: str, column_name: str, db_name: str = None, branch_name: str = None) -> Response:
         """
         Deletes the specified column.  To refer to sub-objects, the column name can contain dots.
         For example `address.country`.
 
         Path: /db/{db_branch_name}/tables/{table_name}/columns/{column_name}
         Method: DELETE
         Response status codes:
@@ -297,20 +265,15 @@
         :return Response
         """
         db_branch_name = self.client.get_db_branch_name(db_name, branch_name)
         url_path = f"/db/{db_branch_name}/tables/{table_name}/columns/{column_name}"
         return self.request("DELETE", url_path)
 
     def updateColumn(
-        self,
-        table_name: str,
-        column_name: str,
-        payload: dict,
-        db_name: str = None,
-        branch_name: str = None,
+        self, table_name: str, column_name: str, payload: dict, db_name: str = None, branch_name: str = None
     ) -> Response:
         """
         Update column with partial data.  Can be used for renaming the column by providing a new
         "name" field.  To refer to sub-objects, the column name can contain dots.  For example
         `address.country`.
 
         Path: /db/{db_branch_name}/tables/{table_name}/columns/{column_name}
```

### Comparing `xata-0.8.0/PKG-INFO` & `xata-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xata
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python client for Xata.io
 License: Apache-2.0
 Author: Xata
 Author-email: support@xata.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

