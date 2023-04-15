# Comparing `tmp/databricks_sql_connector-2.4.1.tar.gz` & `tmp/databricks_sql_connector-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_sql_connector-2.4.1.tar", max compression
+gzip compressed data, was "databricks_sql_connector-2.5.0.tar", max compression
```

## Comparing `databricks_sql_connector-2.4.1.tar` & `databricks_sql_connector-2.5.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     3741 2023-03-21 20:28:36.475587 databricks_sql_connector-2.4.1/CHANGELOG.md
--rw-r--r--   0        0        0    11346 2023-03-21 20:28:36.475587 databricks_sql_connector-2.4.1/LICENSE
--rw-r--r--   0        0        0     2723 2023-03-21 20:28:36.475587 databricks_sql_connector-2.4.1/README.md
--rw-r--r--   0        0        0     1416 2023-03-21 20:29:02.907926 databricks_sql_connector-2.4.1/pyproject.toml
--rw-r--r--   0        0        0      295 2023-03-21 20:28:36.479587 databricks_sql_connector-2.4.1/src/databricks/__init__.py
--rw-r--r--   0        0        0     1269 2023-03-21 20:28:36.479587 databricks_sql_connector-2.4.1/src/databricks/sql/__init__.py
--rw-r--r--   0        0        0        0 2023-03-21 20:28:36.479587 databricks_sql_connector-2.4.1/src/databricks/sql/auth/__init__.py
--rw-r--r--   0        0        0     3616 2023-03-21 20:28:36.479587 databricks_sql_connector-2.4.1/src/databricks/sql/auth/auth.py
--rw-r--r--   0        0        0     4711 2023-03-21 20:28:36.479587 databricks_sql_connector-2.4.1/src/databricks/sql/auth/authenticators.py
--rw-r--r--   0        0        0     9717 2023-03-21 20:28:36.479587 databricks_sql_connector-2.4.1/src/databricks/sql/auth/oauth.py
--rw-r--r--   0        0        0     1201 2023-03-21 20:28:36.479587 databricks_sql_connector-2.4.1/src/databricks/sql/auth/oauth_http_handler.py
--rw-r--r--   0        0        0      872 2023-03-21 20:28:36.479587 databricks_sql_connector-2.4.1/src/databricks/sql/auth/thrift_http_client.py
--rw-r--r--   0        0        0    36862 2023-03-21 20:28:36.479587 databricks_sql_connector-2.4.1/src/databricks/sql/client.py
--rw-r--r--   0        0        0     2423 2023-03-21 20:28:36.479587 databricks_sql_connector-2.4.1/src/databricks/sql/exc.py
--rw-r--r--   0        0        0        0 2023-03-21 20:28:36.479587 databricks_sql_connector-2.4.1/src/databricks/sql/experimental/__init__.py
--rw-r--r--   0        0        0     2236 2023-03-21 20:28:36.479587 databricks_sql_connector-2.4.1/src/databricks/sql/experimental/oauth_persistence.py
--rwxr-xr-x   0        0        0     8062 2023-03-21 20:28:36.479587 databricks_sql_connector-2.4.1/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote
--rw-r--r--   0        0        0   136849 2023-03-21 20:28:36.479587 databricks_sql_connector-2.4.1/src/databricks/sql/thrift_api/TCLIService/TCLIService.py
--rw-r--r--   0        0        0       49 2023-03-21 20:28:36.479587 databricks_sql_connector-2.4.1/src/databricks/sql/thrift_api/TCLIService/__init__.py
--rw-r--r--   0        0        0     1307 2023-03-21 20:28:36.479587 databricks_sql_connector-2.4.1/src/databricks/sql/thrift_api/TCLIService/constants.py
--rw-r--r--   0        0        0  2077276 2023-03-21 20:28:36.483587 databricks_sql_connector-2.4.1/src/databricks/sql/thrift_api/TCLIService/ttypes.py
--rw-r--r--   0        0        0        0 2023-03-21 20:28:36.487587 databricks_sql_connector-2.4.1/src/databricks/sql/thrift_api/__init__.py
--rw-r--r--   0        0        0    41055 2023-03-21 20:28:36.487587 databricks_sql_connector-2.4.1/src/databricks/sql/thrift_backend.py
--rw-r--r--   0        0        0     6771 2023-03-21 20:28:36.487587 databricks_sql_connector-2.4.1/src/databricks/sql/types.py
--rw-r--r--   0        0        0     6646 2023-03-21 20:28:36.487587 databricks_sql_connector-2.4.1/src/databricks/sql/utils.py
--rw-r--r--   0        0        0       60 2023-03-21 20:28:36.487587 databricks_sql_connector-2.4.1/src/databricks/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     9813 2023-03-21 20:28:36.487587 databricks_sql_connector-2.4.1/src/databricks/sqlalchemy/dialect/__init__.py
--rw-r--r--   0        0        0      494 2023-03-21 20:28:36.487587 databricks_sql_connector-2.4.1/src/databricks/sqlalchemy/dialect/base.py
--rw-r--r--   0        0        0      792 2023-03-21 20:28:36.487587 databricks_sql_connector-2.4.1/src/databricks/sqlalchemy/dialect/compiler.py
--rw-r--r--   0        0        0     4106 1970-01-01 00:00:00.000000 databricks_sql_connector-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0     3935 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0    11346 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/LICENSE
+-rw-r--r--   0        0        0     2723 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/README.md
+-rw-r--r--   0        0        0     1416 2023-04-15 04:18:18.493806 databricks_sql_connector-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0      295 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/src/databricks/__init__.py
+-rw-r--r--   0        0        0     1269 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/src/databricks/sql/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/src/databricks/sql/auth/__init__.py
+-rw-r--r--   0        0        0     3894 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/src/databricks/sql/auth/auth.py
+-rw-r--r--   0        0        0     5493 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/src/databricks/sql/auth/authenticators.py
+-rw-r--r--   0        0        0     9717 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/src/databricks/sql/auth/oauth.py
+-rw-r--r--   0        0        0     1201 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/src/databricks/sql/auth/oauth_http_handler.py
+-rw-r--r--   0        0        0     1269 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/src/databricks/sql/auth/thrift_http_client.py
+-rw-r--r--   0        0        0    36862 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/src/databricks/sql/client.py
+-rw-r--r--   0        0        0     2423 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/src/databricks/sql/exc.py
+-rw-r--r--   0        0        0        0 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/src/databricks/sql/experimental/__init__.py
+-rw-r--r--   0        0        0     2236 2023-04-15 04:17:53.229556 databricks_sql_connector-2.5.0/src/databricks/sql/experimental/oauth_persistence.py
+-rwxr-xr-x   0        0        0     8062 2023-04-15 04:17:53.233556 databricks_sql_connector-2.5.0/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote
+-rw-r--r--   0        0        0   136849 2023-04-15 04:17:53.233556 databricks_sql_connector-2.5.0/src/databricks/sql/thrift_api/TCLIService/TCLIService.py
+-rw-r--r--   0        0        0       49 2023-04-15 04:17:53.233556 databricks_sql_connector-2.5.0/src/databricks/sql/thrift_api/TCLIService/__init__.py
+-rw-r--r--   0        0        0     1307 2023-04-15 04:17:53.233556 databricks_sql_connector-2.5.0/src/databricks/sql/thrift_api/TCLIService/constants.py
+-rw-r--r--   0        0        0  2077276 2023-04-15 04:17:53.237556 databricks_sql_connector-2.5.0/src/databricks/sql/thrift_api/TCLIService/ttypes.py
+-rw-r--r--   0        0        0        0 2023-04-15 04:17:53.237556 databricks_sql_connector-2.5.0/src/databricks/sql/thrift_api/__init__.py
+-rw-r--r--   0        0        0    41140 2023-04-15 04:17:53.237556 databricks_sql_connector-2.5.0/src/databricks/sql/thrift_backend.py
+-rw-r--r--   0        0        0     6771 2023-04-15 04:17:53.237556 databricks_sql_connector-2.5.0/src/databricks/sql/types.py
+-rw-r--r--   0        0        0     6646 2023-04-15 04:17:53.237556 databricks_sql_connector-2.5.0/src/databricks/sql/utils.py
+-rw-r--r--   0        0        0       60 2023-04-15 04:17:53.237556 databricks_sql_connector-2.5.0/src/databricks/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     9813 2023-04-15 04:17:53.237556 databricks_sql_connector-2.5.0/src/databricks/sqlalchemy/dialect/__init__.py
+-rw-r--r--   0        0        0      494 2023-04-15 04:17:53.237556 databricks_sql_connector-2.5.0/src/databricks/sqlalchemy/dialect/base.py
+-rw-r--r--   0        0        0      792 2023-04-15 04:17:53.237556 databricks_sql_connector-2.5.0/src/databricks/sqlalchemy/dialect/compiler.py
+-rw-r--r--   0        0        0     4106 1970-01-01 00:00:00.000000 databricks_sql_connector-2.5.0/PKG-INFO
```

### Comparing `databricks_sql_connector-2.4.1/CHANGELOG.md` & `databricks_sql_connector-2.5.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # Release History
 
-## 2.4.x (Unreleased)
+## 2.5.x (Unreleased)
+
+## 2.5.0 (2023-04-14)
+- Add support for External Auth providers
+- Fix: Python HTTP proxies were broken
+- Other: All Thrift requests that timeout during connection will be automatically retried
 
 ## 2.4.1 (2023-03-21)
 
 - Less strict numpy and pyarrow dependencies
 - Update examples in README to use security best practices
 - Update docstring for client.execute() for clarity
```

### Comparing `databricks_sql_connector-2.4.1/LICENSE` & `databricks_sql_connector-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.4.1/README.md` & `databricks_sql_connector-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.4.1/pyproject.toml` & `databricks_sql_connector-2.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databricks-sql-connector"
-version = "2.4.1"
+version = "2.5.0"
 description = "Databricks SQL Connector for Python"
 authors = ["Databricks <databricks-sql-connector-maintainers@databricks.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "databricks", from = "src"}]
 include = ["CHANGELOG.md"]
```

### Comparing `databricks_sql_connector-2.4.1/src/databricks/sql/__init__.py` & `databricks_sql_connector-2.5.0/src/databricks/sql/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 NUMBER = DBAPITypeObject(
     "boolean", "tinyint", "smallint", "int", "bigint", "float", "double", "decimal"
 )
 DATETIME = DBAPITypeObject("timestamp")
 DATE = DBAPITypeObject("date")
 ROWID = DBAPITypeObject()
 
-__version__ = "2.4.1"
+__version__ = "2.5.0"
 USER_AGENT_NAME = "PyDatabricksSqlConnector"
 
 # These two functions are pyhive legacy
 Date = datetime.date
 Timestamp = datetime.datetime
```

### Comparing `databricks_sql_connector-2.4.1/src/databricks/sql/auth/auth.py` & `databricks_sql_connector-2.5.0/src/databricks/sql/auth/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from enum import Enum
 from typing import List
 
 from databricks.sql.auth.authenticators import (
     AuthProvider,
     AccessTokenAuthProvider,
     BasicAuthProvider,
+    ExternalAuthProvider,
     DatabricksOAuthProvider,
 )
 from databricks.sql.experimental.oauth_persistence import OAuthPersistence
 
 
 class AuthType(Enum):
     DATABRICKS_OAUTH = "databricks-oauth"
@@ -26,29 +27,33 @@
         auth_type: str = None,
         oauth_scopes: List[str] = None,
         oauth_client_id: str = None,
         oauth_redirect_port_range: List[int] = None,
         use_cert_as_auth: str = None,
         tls_client_cert_file: str = None,
         oauth_persistence=None,
+        credentials_provider=None,
     ):
         self.hostname = hostname
         self.username = username
         self.password = password
         self.access_token = access_token
         self.auth_type = auth_type
         self.oauth_scopes = oauth_scopes
         self.oauth_client_id = oauth_client_id
         self.oauth_redirect_port_range = oauth_redirect_port_range
         self.use_cert_as_auth = use_cert_as_auth
         self.tls_client_cert_file = tls_client_cert_file
         self.oauth_persistence = oauth_persistence
+        self.credentials_provider = credentials_provider
 
 
 def get_auth_provider(cfg: ClientContext):
+    if cfg.credentials_provider:
+        return ExternalAuthProvider(cfg.credentials_provider)
     if cfg.auth_type == AuthType.DATABRICKS_OAUTH.value:
         assert cfg.oauth_redirect_port_range is not None
         assert cfg.oauth_client_id is not None
         assert cfg.oauth_scopes is not None
 
         return DatabricksOAuthProvider(
             cfg.hostname,
@@ -90,9 +95,10 @@
         tls_client_cert_file=kwargs.get("_tls_client_cert_file"),
         oauth_scopes=PYSQL_OAUTH_SCOPES,
         oauth_client_id=kwargs.get("oauth_client_id") or PYSQL_OAUTH_CLIENT_ID,
         oauth_redirect_port_range=[kwargs["oauth_redirect_port"]]
         if kwargs.get("oauth_client_id") and kwargs.get("oauth_redirect_port")
         else PYSQL_OAUTH_REDIRECT_PORT_RANGE,
         oauth_persistence=kwargs.get("experimental_oauth_persistence"),
+        credentials_provider=kwargs.get("credentials_provider"),
     )
     return get_auth_provider(cfg)
```

### Comparing `databricks_sql_connector-2.4.1/src/databricks/sql/auth/authenticators.py` & `databricks_sql_connector-2.5.0/src/databricks/sql/auth/authenticators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,40 @@
+import abc
 import base64
 import logging
-from typing import Dict, List
+from typing import Callable, Dict, List
 
 from databricks.sql.auth.oauth import OAuthManager
 
 # Private API: this is an evolving interface and it will change in the future.
 # Please must not depend on it in your applications.
 from databricks.sql.experimental.oauth_persistence import OAuthToken, OAuthPersistence
 
 
 class AuthProvider:
     def add_headers(self, request_headers: Dict[str, str]):
         pass
 
 
+HeaderFactory = Callable[[], Dict[str, str]]
+
+# In order to keep compatibility with SDK
+class CredentialsProvider(abc.ABC):
+    """CredentialsProvider is the protocol (call-side interface)
+    for authenticating requests to Databricks REST APIs"""
+
+    @abc.abstractmethod
+    def auth_type(self) -> str:
+        ...
+
+    @abc.abstractmethod
+    def __call__(self, *args, **kwargs) -> HeaderFactory:
+        ...
+
+
 # Private API: this is an evolving interface and it will change in the future.
 # Please must not depend on it in your applications.
 class AccessTokenAuthProvider(AuthProvider):
     def __init__(self, access_token: str):
         self.__authorization_header_value = "Bearer {}".format(access_token)
 
     def add_headers(self, request_headers: Dict[str, str]):
@@ -116,7 +133,17 @@
 
                 if self._oauth_persistence:
                     token = OAuthToken(self._access_token, self._refresh_token)
                     self._oauth_persistence.persist(self._hostname, token)
         except Exception as e:
             logging.error(f"unexpected error in oauth token update", e, exc_info=True)
             raise e
+
+
+class ExternalAuthProvider(AuthProvider):
+    def __init__(self, credentials_provider: CredentialsProvider) -> None:
+        self._header_factory = credentials_provider()
+
+    def add_headers(self, request_headers: Dict[str, str]):
+        headers = self._header_factory()
+        for k, v in headers.items():
+            request_headers[k] = v
```

### Comparing `databricks_sql_connector-2.4.1/src/databricks/sql/auth/oauth.py` & `databricks_sql_connector-2.5.0/src/databricks/sql/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.4.1/src/databricks/sql/auth/oauth_http_handler.py` & `databricks_sql_connector-2.5.0/src/databricks/sql/auth/oauth_http_handler.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.4.1/src/databricks/sql/client.py` & `databricks_sql_connector-2.5.0/src/databricks/sql/client.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.4.1/src/databricks/sql/exc.py` & `databricks_sql_connector-2.5.0/src/databricks/sql/exc.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.4.1/src/databricks/sql/experimental/oauth_persistence.py` & `databricks_sql_connector-2.5.0/src/databricks/sql/experimental/oauth_persistence.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.4.1/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote` & `databricks_sql_connector-2.5.0/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.4.1/src/databricks/sql/thrift_api/TCLIService/TCLIService.py` & `databricks_sql_connector-2.5.0/src/databricks/sql/thrift_api/TCLIService/TCLIService.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.4.1/src/databricks/sql/thrift_api/TCLIService/constants.py` & `databricks_sql_connector-2.5.0/src/databricks/sql/thrift_api/TCLIService/constants.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.4.1/src/databricks/sql/thrift_api/TCLIService/ttypes.py` & `databricks_sql_connector-2.5.0/src/databricks/sql/thrift_api/TCLIService/ttypes.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.4.1/src/databricks/sql/thrift_backend.py` & `databricks_sql_connector-2.5.0/src/databricks/sql/thrift_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,35 +318,35 @@
                 logger.debug("Sending request: {}".format(request))
                 response = method(request)
                 logger.debug("Received response: {}".format(response))
                 return response
             except OSError as err:
                 error = err
                 error_message = str(err)
+                # fmt: off
+                # The built-in errno package encapsulates OSError codes, which are OS-specific.
+                # log.info for errors we believe are not unusual or unexpected. log.warn for
+                # for others like EEXIST, EBADF, ERANGE which are not expected in this context.
+                #
+                # I manually tested this retry behaviour using mitmweb and confirmed that 
+                # GetOperationStatus requests are retried when I forced network connection
+                # interruptions / timeouts / reconnects. See #24 for more info.
+                                        # | Debian | Darwin |
+                info_errs = [           # |--------|--------|         
+                    errno.ESHUTDOWN,    # |   32   |   32   |
+                    errno.EAFNOSUPPORT, # |   97   |   47   |
+                    errno.ECONNRESET,   # |   104  |   54   |
+                    errno.ETIMEDOUT,    # |   110  |   60   |
+                ]
 
                 gos_name = TCLIServiceClient.GetOperationStatus.__name__
-                if method.__name__ == gos_name:
+                # retry on timeout. Happens a lot in Azure and it is safe as data has not been sent to server yet
+                if method.__name__ == gos_name or err.errno == errno.ETIMEDOUT:
                     retry_delay = bound_retry_delay(attempt, self._retry_delay_default)
 
-                    # fmt: off
-                    # The built-in errno package encapsulates OSError codes, which are OS-specific.
-                    # log.info for errors we believe are not unusual or unexpected. log.warn for
-                    # for others like EEXIST, EBADF, ERANGE which are not expected in this context.
-                    #
-                    # I manually tested this retry behaviour using mitmweb and confirmed that 
-                    # GetOperationStatus requests are retried when I forced network connection
-                    # interruptions / timeouts / reconnects. See #24 for more info.
-                                            # | Debian | Darwin |
-                    info_errs = [           # |--------|--------|         
-                        errno.ESHUTDOWN,    # |   32   |   32   |
-                        errno.EAFNOSUPPORT, # |   97   |   47   |
-                        errno.ECONNRESET,   # |   104  |   54   |
-                        errno.ETIMEDOUT,    # |   110  |   60   |
-                    ]
-
                     # fmt: on
                     log_string = f"{gos_name} failed with code {err.errno} and will attempt to retry"
                     if err.errno in info_errs:
                         logger.info(log_string)
                     else:
                         logger.warning(log_string)
             except Exception as err:
```

### Comparing `databricks_sql_connector-2.4.1/src/databricks/sql/types.py` & `databricks_sql_connector-2.5.0/src/databricks/sql/types.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.4.1/src/databricks/sql/utils.py` & `databricks_sql_connector-2.5.0/src/databricks/sql/utils.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.4.1/src/databricks/sqlalchemy/dialect/__init__.py` & `databricks_sql_connector-2.5.0/src/databricks/sqlalchemy/dialect/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.4.1/src/databricks/sqlalchemy/dialect/compiler.py` & `databricks_sql_connector-2.5.0/src/databricks/sqlalchemy/dialect/compiler.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.4.1/PKG-INFO` & `databricks_sql_connector-2.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-sql-connector
-Version: 2.4.1
+Version: 2.5.0
 Summary: Databricks SQL Connector for Python
 License: Apache-2.0
 Author: Databricks
 Author-email: databricks-sql-connector-maintainers@databricks.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

