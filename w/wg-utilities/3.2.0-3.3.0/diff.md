# Comparing `tmp/wg_utilities-3.2.0.tar.gz` & `tmp/wg_utilities-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wg_utilities-3.2.0.tar", max compression
+gzip compressed data, was "wg_utilities-3.3.0.tar", max compression
```

## Comparing `wg_utilities-3.2.0.tar` & `wg_utilities-3.3.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1069 2023-04-13 23:08:24.073689 wg_utilities-3.2.0/LICENSE
--rw-r--r--   0        0        0     1520 2023-04-13 23:08:24.073689 wg_utilities-3.2.0/README.md
--rw-r--r--   0        0        0     4825 2023-04-13 23:08:24.077689 wg_utilities-3.2.0/pyproject.toml
--rw-r--r--   0        0        0      280 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/__init__.py
--rw-r--r--   0        0        0      140 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/api/__init__.py
--rw-r--r--   0        0        0     7384 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/api/temp_auth_server.py
--rw-r--r--   0        0        0      560 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/clients/__init__.py
--rw-r--r--   0        0        0     5081 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/clients/_google.py
--rw-r--r--   0        0        0    10359 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/clients/_spotify_types.py
--rw-r--r--   0        0        0    24778 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/clients/google_calendar.py
--rw-r--r--   0        0        0    56600 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/clients/google_drive.py
--rw-r--r--   0        0        0     7261 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/clients/google_fit.py
--rw-r--r--   0        0        0    14184 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/clients/google_photos.py
--rw-r--r--   0        0        0    16312 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/clients/monzo.py
--rw-r--r--   0        0        0    25465 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/clients/oauth_client.py
--rw-r--r--   0        0        0    49911 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/clients/spotify.py
--rw-r--r--   0        0        0    21546 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/clients/truelayer.py
--rw-r--r--   0        0        0      126 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/devices/__init__.py
--rw-r--r--   0        0        0      119 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/devices/dht22/__init__.py
--rwxr-xr-x   0        0        0     6642 2023-04-13 23:08:24.145691 wg_utilities-3.2.0/wg_utilities/devices/dht22/dht22_lib.py
--rw-r--r--   0        0        0     1129 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/devices/epd/__init__.py
--rw-r--r--   0        0        0     7042 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/devices/epd/epd7in5_v2.py
--rw-r--r--   0        0        0     6041 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/devices/epd/epdconfig.py
--rw-r--r--   0        0        0      138 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/devices/yamaha_yas_209/__init__.py
--rw-r--r--   0        0        0    36374 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py
--rw-r--r--   0        0        0     5401 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/exceptions/__init__.py
--rw-r--r--   0        0        0      803 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/functions/__init__.py
--rw-r--r--   0        0        0     4595 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/functions/_functions.py
--rw-r--r--   0        0        0     1287 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/functions/datetime_helpers.py
--rw-r--r--   0        0        0     2024 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/functions/file_management.py
--rw-r--r--   0        0        0     8877 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/functions/json.py
--rw-r--r--   0        0        0     1386 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/functions/processes.py
--rw-r--r--   0        0        0     1106 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/functions/string_manipulation.py
--rw-r--r--   0        0        0     1586 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/functions/xml.py
--rw-r--r--   0        0        0     7258 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/loggers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/py.typed
--rw-r--r--   0        0        0      167 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/testing/__init__.py
--rw-r--r--   0        0        0     5257 2023-04-13 23:08:24.149691 wg_utilities-3.2.0/wg_utilities/testing/_custom_mocks.py
--rw-r--r--   0        0        0     3336 1970-01-01 00:00:00.000000 wg_utilities-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-15 20:24:04.024161 wg_utilities-3.3.0/LICENSE
+-rw-r--r--   0        0        0     2297 2023-04-15 20:24:04.024161 wg_utilities-3.3.0/README.md
+-rw-r--r--   0        0        0     4825 2023-04-15 20:24:04.028161 wg_utilities-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0      280 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/__init__.py
+-rw-r--r--   0        0        0      140 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/api/__init__.py
+-rw-r--r--   0        0        0     7384 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/api/temp_auth_server.py
+-rw-r--r--   0        0        0      560 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/clients/__init__.py
+-rw-r--r--   0        0        0     4305 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/clients/_google.py
+-rw-r--r--   0        0        0    10390 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/clients/_spotify_types.py
+-rw-r--r--   0        0        0    24119 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/clients/google_calendar.py
+-rw-r--r--   0        0        0    56745 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/clients/google_drive.py
+-rw-r--r--   0        0        0     7441 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/clients/google_fit.py
+-rw-r--r--   0        0        0    13531 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/clients/google_photos.py
+-rw-r--r--   0        0        0    15632 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/clients/monzo.py
+-rw-r--r--   0        0        0    26324 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/clients/oauth_client.py
+-rw-r--r--   0        0        0    49179 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/clients/spotify.py
+-rw-r--r--   0        0        0    21707 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/clients/truelayer.py
+-rw-r--r--   0        0        0      126 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/devices/__init__.py
+-rw-r--r--   0        0        0      119 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/devices/dht22/__init__.py
+-rwxr-xr-x   0        0        0     6642 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/devices/dht22/dht22_lib.py
+-rw-r--r--   0        0        0     1129 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/devices/epd/__init__.py
+-rw-r--r--   0        0        0     7042 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/devices/epd/epd7in5_v2.py
+-rw-r--r--   0        0        0     6041 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/devices/epd/epdconfig.py
+-rw-r--r--   0        0        0      138 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/devices/yamaha_yas_209/__init__.py
+-rw-r--r--   0        0        0    36374 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py
+-rw-r--r--   0        0        0     5401 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/exceptions/__init__.py
+-rw-r--r--   0        0        0      803 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/functions/__init__.py
+-rw-r--r--   0        0        0     4595 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/functions/_functions.py
+-rw-r--r--   0        0        0     1287 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/functions/datetime_helpers.py
+-rw-r--r--   0        0        0     2024 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/functions/file_management.py
+-rw-r--r--   0        0        0     8877 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/functions/json.py
+-rw-r--r--   0        0        0     1386 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/functions/processes.py
+-rw-r--r--   0        0        0     1106 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/functions/string_manipulation.py
+-rw-r--r--   0        0        0     1586 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/functions/xml.py
+-rw-r--r--   0        0        0     7258 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/loggers/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/py.typed
+-rw-r--r--   0        0        0      167 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/testing/__init__.py
+-rw-r--r--   0        0        0     5257 2023-04-15 20:24:04.096162 wg_utilities-3.3.0/wg_utilities/testing/_custom_mocks.py
+-rw-r--r--   0        0        0     4113 1970-01-01 00:00:00.000000 wg_utilities-3.3.0/PKG-INFO
```

### Comparing `wg_utilities-3.2.0/LICENSE` & `wg_utilities-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.2.0/pyproject.toml` & `wg_utilities-3.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wg-utilities"
-version = "3.2.0"
+version = "3.3.0"
 description = "Loads of useful stuff for the things I do :)"
 
 authors = ["Will Garside <worgarside@gmail.com>"]
 include = ["wg_utilities/py.typed"]
 license = "MIT"
 maintainers = ["Will Garside <worgarside@gmail.com>"]
 packages = [{ include = "wg_utilities" }]
```

### Comparing `wg_utilities-3.2.0/wg_utilities/api/temp_auth_server.py` & `wg_utilities-3.3.0/wg_utilities/api/temp_auth_server.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.2.0/wg_utilities/clients/__init__.py` & `wg_utilities-3.3.0/wg_utilities/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.2.0/wg_utilities/clients/_google.py` & `wg_utilities-3.3.0/wg_utilities/clients/_google.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Generic Google Client - having one client for all APIs is way too big."""
 from __future__ import annotations
 
 from collections.abc import Callable, Iterable, Mapping
 from copy import deepcopy
 from json import dumps
 from logging import DEBUG, getLogger
-from pathlib import Path
 from typing import TYPE_CHECKING, Any, Generic, Literal, TypeAlias, TypedDict, TypeVar
 
 from requests import Response, get
 
 from wg_utilities.clients.oauth_client import OAuthClient, StrBytIntFlt
 from wg_utilities.loggers import add_stream_handler
 
@@ -70,43 +69,20 @@
 class GoogleClient(
     Generic[GetJsonResponseGoogleClient], OAuthClient[GetJsonResponseGoogleClient]
 ):
     """Custom client for interacting with the Google APIs."""
 
     ACCESS_TOKEN_ENDPOINT = "https://oauth2.googleapis.com/token"
     AUTH_LINK_BASE = "https://accounts.google.com/o/oauth2/v2/auth"
+    BASE_URL: str
 
     DEFAULT_PARAMS: dict[StrBytIntFlt, StrBytIntFlt | Iterable[StrBytIntFlt] | None] = {
         "pageSize": "50",
     }
 
-    def __init__(
-        self,
-        *,
-        client_id: str,
-        client_secret: str,
-        base_url: str,
-        log_requests: bool = False,
-        creds_cache_path: Path | None = None,
-        scopes: list[str] | None = None,
-        oauth_login_redirect_host: str = "localhost",
-    ):
-        """Initialise the client."""
-        super().__init__(
-            base_url=base_url,
-            access_token_endpoint=self.ACCESS_TOKEN_ENDPOINT,
-            auth_link_base=self.AUTH_LINK_BASE,
-            client_id=client_id,
-            client_secret=client_secret,
-            log_requests=log_requests,
-            creds_cache_path=creds_cache_path,
-            scopes=scopes,
-            oauth_login_redirect_host=oauth_login_redirect_host,
-        )
-
     def get_items(
         self,
         url: str,
         *,
         list_key: Literal["albums", "drives", "files", "items", "point"] = "items",
         params: dict[
             StrBytIntFlt,
```

### Comparing `wg_utilities-3.2.0/wg_utilities/clients/_spotify_types.py` & `wg_utilities-3.3.0/wg_utilities/clients/_spotify_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,15 @@
         "SINGLE",
         "ALBUM",
         "COMPILATION",
     ]
     artists: list[ArtistSummaryJson]
     available_markets: list[str]
     images: list[Image]
+    is_playable: bool | None
     release_date: str | date
     release_date_precision: str
     total_tracks: int
     restrictions: NotRequired[dict[str, str]]
     type: Literal["album"]
 
 
@@ -251,15 +252,15 @@
     available_markets: list[None]
     disc_number: int
     duration_ms: int
     episode: NotRequired[bool]
     explicit: bool
     external_ids: dict[None, None]
     is_local: Literal[True]
-    is_playable: NotRequired[str]
+    is_playable: NotRequired[bool]
     linked_from: NotRequired[_LinkedFromInTrack]
     popularity: int
     preview_url: None
     track_number: int
     type: Literal["track"]
 
 
@@ -271,15 +272,15 @@
     available_markets: list[str]
     disc_number: int
     duration_ms: int
     episode: NotRequired[bool]
     explicit: bool
     external_ids: NotRequired[dict[str, str]]
     is_local: Literal[False]
-    is_playable: NotRequired[str]
+    is_playable: NotRequired[bool]
     linked_from: NotRequired[_LinkedFromInTrack]
     popularity: int
     preview_url: str
     restrictions: NotRequired[
         dict[Literal["reason"], Literal["explicit", "market", "product"]]
     ]
     track: NotRequired[bool]
```

### Comparing `wg_utilities-3.2.0/wg_utilities/clients/google_calendar.py` & `wg_utilities-3.3.0/wg_utilities/clients/google_calendar.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from __future__ import annotations
 
 from collections.abc import Callable, Iterable, Mapping, Set
 from datetime import date as date_
 from datetime import datetime as datetime_
 from datetime import timedelta, tzinfo
 from enum import Enum
-from pathlib import Path
 from typing import Any, Literal, TypeAlias, TypedDict, TypeVar
 
 from pydantic import Field, root_validator, validator
 from pytz import UTC, timezone
 from requests import delete
 from tzlocal import get_localzone
 
@@ -585,40 +584,20 @@
 
     BASE_URL = "https://www.googleapis.com/calendar/v3"
 
     DEFAULT_PARAMS: dict[StrBytIntFlt, StrBytIntFlt | Iterable[StrBytIntFlt] | None] = {
         "maxResults": "250",
     }
 
-    DEFAULT_SCOPE = [
+    DEFAULT_SCOPES = [
         "https://www.googleapis.com/auth/calendar",
         "https://www.googleapis.com/auth/calendar.events",
     ]
 
-    def __init__(
-        self,
-        client_id: str,
-        client_secret: str,
-        *,
-        scopes: list[str] | None = None,
-        log_requests: bool = False,
-        creds_cache_path: Path | None = None,
-        oauth_login_redirect_host: str = "localhost",
-    ):
-        super().__init__(
-            base_url=self.BASE_URL,
-            client_id=client_id,
-            client_secret=client_secret,
-            scopes=scopes or self.DEFAULT_SCOPE,
-            log_requests=log_requests,
-            creds_cache_path=creds_cache_path,
-            oauth_login_redirect_host=oauth_login_redirect_host,
-        )
-
-        self._primary_calendar: Calendar
+    _primary_calendar: Calendar
 
     def create_event(
         self,
         summary: str,
         start_datetime: datetime_ | date_,
         end_datetime: datetime_ | date_,
         tz: str | None = None,
```

### Comparing `wg_utilities-3.2.0/wg_utilities/clients/google_drive.py` & `wg_utilities-3.3.0/wg_utilities/clients/google_drive.py`

 * *Files 0% similar despite different names*

```diff
@@ -1452,44 +1452,46 @@
     Args:
         scopes (list): a list of scopes the client can be given
         creds_cache_path (str): file path for where to cache credentials
     """
 
     BASE_URL = "https://www.googleapis.com/drive/v3"
 
-    DEFAULT_SCOPE = [
+    DEFAULT_SCOPES = [
         "https://www.googleapis.com/auth/drive",
         "https://www.googleapis.com/auth/drive.file",
         "https://www.googleapis.com/auth/drive.readonly",
         "https://www.googleapis.com/auth/drive.metadata.readonly",
         "https://www.googleapis.com/auth/drive.appdata",
         "https://www.googleapis.com/auth/drive.metadata",
         "https://www.googleapis.com/auth/drive.photos.readonly",
     ]
 
     def __init__(
         self,
+        *,
         client_id: str,
         client_secret: str,
-        *,
-        scopes: list[str] | None = None,
         log_requests: bool = False,
         creds_cache_path: Path | None = None,
+        scopes: list[str] | None = None,
+        oauth_login_redirect_host: str = "localhost",
         # pylint: disable=line-too-long
         item_metadata_retrieval: ItemMetadataRetrieval = ItemMetadataRetrieval.ON_FIRST_REQUEST,
-        oauth_login_redirect_host: str = "localhost",
+        headless_auth_link_callback: Callable[[str], None] | None = None,
     ):
         super().__init__(
-            base_url=self.BASE_URL,
             client_id=client_id,
             client_secret=client_secret,
-            scopes=scopes or self.DEFAULT_SCOPE,
             log_requests=log_requests,
             creds_cache_path=creds_cache_path,
+            scopes=scopes or self.DEFAULT_SCOPES,
             oauth_login_redirect_host=oauth_login_redirect_host,
+            base_url=self.BASE_URL,
+            headless_auth_link_callback=headless_auth_link_callback,
         )
 
         self._my_drive: Drive
         self.item_metadata_retrieval = item_metadata_retrieval
 
     @property
     def my_drive(self) -> Drive:
```

### Comparing `wg_utilities-3.2.0/wg_utilities/clients/google_fit.py` & `wg_utilities-3.3.0/wg_utilities/clients/google_fit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Custom client for interacting with Google's Fit API."""
 from __future__ import annotations
 
+from collections.abc import Callable
 from datetime import datetime
 from pathlib import Path
 from typing import Any, Literal, TypedDict
 
 from wg_utilities.clients._google import GoogleClient
 from wg_utilities.functions.datetime_helpers import DatetimeFixedUnit as DFUnit
 from wg_utilities.functions.datetime_helpers import utcnow
@@ -191,30 +192,32 @@
         "https://www.googleapis.com/auth/fitness.body.read",
         "https://www.googleapis.com/auth/fitness.location.read",
         "https://www.googleapis.com/auth/fitness.nutrition.read",
     ]
 
     def __init__(
         self,
+        *,
         client_id: str,
         client_secret: str,
-        *,
-        scopes: list[str] | None = None,
         log_requests: bool = False,
         creds_cache_path: Path | None = None,
+        scopes: list[str] | None = None,
         oauth_login_redirect_host: str = "localhost",
+        headless_auth_link_callback: Callable[[str], None] | None = None,
     ):
         super().__init__(
-            base_url=self.BASE_URL,
             client_id=client_id,
             client_secret=client_secret,
-            scopes=scopes or self.DEFAULT_SCOPES,
             log_requests=log_requests,
             creds_cache_path=creds_cache_path,
+            scopes=scopes or self.DEFAULT_SCOPES,
             oauth_login_redirect_host=oauth_login_redirect_host,
+            base_url=self.BASE_URL,
+            headless_auth_link_callback=headless_auth_link_callback,
         )
 
         self.data_sources: dict[str, DataSource] = {}
 
     def get_data_source(self, data_source_id: str) -> DataSource:
         """Get a data source based on its UID.
```

### Comparing `wg_utilities-3.2.0/wg_utilities/clients/google_photos.py` & `wg_utilities-3.3.0/wg_utilities/clients/google_photos.py`

 * *Files 2% similar despite different names*

```diff
@@ -345,38 +345,18 @@
     DEFAULT_SCOPES = [
         "https://www.googleapis.com/auth/photoslibrary.readonly",
         "https://www.googleapis.com/auth/photoslibrary.appendonly",
         "https://www.googleapis.com/auth/photoslibrary.readonly.appcreateddata",
         "https://www.googleapis.com/auth/photoslibrary.edit.appcreateddata",
     ]
 
-    def __init__(
-        self,
-        client_id: str,
-        client_secret: str,
-        *,
-        scopes: list[str] | None = None,
-        log_requests: bool = False,
-        creds_cache_path: Path | None = None,
-        oauth_login_redirect_host: str = "localhost",
-    ):
-        super().__init__(
-            base_url=self.BASE_URL,
-            client_id=client_id,
-            client_secret=client_secret,
-            scopes=scopes or self.DEFAULT_SCOPES,
-            log_requests=log_requests,
-            creds_cache_path=creds_cache_path,
-            oauth_login_redirect_host=oauth_login_redirect_host,
-        )
-
-        self._albums: list[Album]
-        # Only really used to check if all album metadata has been fetched, not
-        # available to the user (would still require caching all albums).
-        self._album_count: int
+    _albums: list[Album]
+    # Only really used to check if all album metadata has been fetched, not
+    # available to the user (would still require caching all albums).
+    _album_count: int
 
     def get_album_by_id(self, album_id: str) -> Album:
         """Get an album by its ID.
 
         Args:
             album_id (str): the ID of the album to fetch
```

### Comparing `wg_utilities-3.2.0/wg_utilities/clients/monzo.py` & `wg_utilities-3.3.0/wg_utilities/clients/monzo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # pylint: disable=too-few-public-methods
 """Custom client for interacting with Monzo's API."""
 from __future__ import annotations
 
 from collections.abc import Iterable
 from datetime import datetime, timedelta
 from logging import DEBUG, getLogger
-from pathlib import Path
 from typing import Any, Literal, TypedDict, final
 
 from pydantic import Field
 from requests import put
 
 from wg_utilities.clients.oauth_client import (
     BaseModelWithConfig,
@@ -424,35 +423,15 @@
     AUTH_LINK_BASE = "https://auth.monzo.com"
     BASE_URL = "https://api.monzo.com"
 
     DEFAULT_PARAMS: dict[
         StrBytIntFlt, StrBytIntFlt | Iterable[StrBytIntFlt] | None
     ] = {}
 
-    def __init__(
-        self,
-        *,
-        client_id: str,
-        client_secret: str,
-        log_requests: bool = False,
-        creds_cache_path: Path | None = None,
-        oauth_login_redirect_host: str = "localhost",
-    ):
-        super().__init__(
-            base_url=self.BASE_URL,
-            access_token_endpoint=self.ACCESS_TOKEN_ENDPOINT,
-            auth_link_base=self.AUTH_LINK_BASE,
-            client_id=client_id,
-            client_secret=client_secret,
-            log_requests=log_requests,
-            creds_cache_path=creds_cache_path,
-            oauth_login_redirect_host=oauth_login_redirect_host,
-        )
-
-        self._current_account: Account
+    _current_account: Account
 
     def deposit_into_pot(
         self, pot: Pot, amount_pence: int, dedupe_id: str | None = None
     ) -> None:
         """Move money from the user's account into one of their pots.
 
         Args:
```

### Comparing `wg_utilities-3.2.0/wg_utilities/clients/oauth_client.py` & `wg_utilities-3.3.0/wg_utilities/clients/oauth_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -215,45 +215,53 @@
 
 class OAuthClient(Generic[GetJsonResponse]):
     """Custom client for interacting with OAuth APIs.
 
     Includes all necessary/basic authentication functionality
     """
 
+    ACCESS_TOKEN_ENDPOINT: str
+    AUTH_LINK_BASE: str
+    BASE_URL: str
+
     ACCESS_TOKEN_EXPIRY_THRESHOLD = 150
 
     DEFAULT_CACHE_DIR = getenv("WG_UTILITIES_CREDS_CACHE_DIR")
-
     DEFAULT_PARAMS: dict[
         StrBytIntFlt, StrBytIntFlt | Iterable[StrBytIntFlt] | None
     ] = {}
+    DEFAULT_SCOPES: list[str] = []
+
+    HEADLESS_MODE = getenv("WG_UTILITIES_HEADLESS_MODE", "0") == "1"
 
     def __init__(
         self,
         *,
-        base_url: str,
-        access_token_endpoint: str,
-        auth_link_base: str,
         client_id: str | None = None,
         client_secret: str | None = None,
         log_requests: bool = False,
         creds_cache_path: Path | None = None,
         scopes: list[str] | None = None,
         oauth_login_redirect_host: str = "localhost",
+        access_token_endpoint: str | None = None,
+        auth_link_base: str | None = None,
+        base_url: str | None = None,
+        headless_auth_link_callback: Callable[[str], None] | None = None,
     ):
         self._client_id = client_id
         self._client_secret = client_secret
-        self.base_url = base_url
-        self.access_token_endpoint = access_token_endpoint
-        self.auth_link_base = auth_link_base
+        self.base_url = base_url or self.BASE_URL
+        self.access_token_endpoint = access_token_endpoint or self.ACCESS_TOKEN_ENDPOINT
+        self.auth_link_base = auth_link_base or self.AUTH_LINK_BASE
         self.log_requests = log_requests
         self._creds_cache_path = creds_cache_path
         self.oauth_login_redirect_host = oauth_login_redirect_host
+        self.headless_auth_link_callback = headless_auth_link_callback
 
-        self.scopes = scopes or []
+        self.scopes = scopes or self.DEFAULT_SCOPES
 
         self._credentials: OAuthCredentials
         self._temp_auth_server: TempAuthServer
 
         if self._creds_cache_path:
             self._load_local_credentials()
 
@@ -572,31 +580,40 @@
         state_token = "".join(choice(ascii_letters) for _ in range(32))
 
         self.temp_auth_server.start_server()
 
         # pylint: disable=line-too-long
         redirect_uri = f"http://{self.oauth_login_redirect_host}:{self.temp_auth_server.port}/get_auth_code"
 
-        auth_link = (
-            self.auth_link_base
-            + "?"
-            + urlencode(
-                {
-                    "client_id": self._client_id,
-                    "redirect_uri": redirect_uri,
-                    "response_type": "code",
-                    "state": state_token,
-                    "scope": " ".join(self.scopes),
-                    "access_type": "offline",
-                    "prompt": "consent",
-                }
-            )
-        )
-        LOGGER.debug("Opening %s", auth_link)
-        open_browser(auth_link)
+        auth_link_params = {
+            "client_id": self._client_id,
+            "redirect_uri": redirect_uri,
+            "response_type": "code",
+            "state": state_token,
+            "access_type": "offline",
+            "prompt": "consent",
+        }
+
+        if self.scopes:
+            auth_link_params["scope"] = " ".join(self.scopes)
+
+        auth_link = self.auth_link_base + "?" + urlencode(auth_link_params)
+
+        if self.HEADLESS_MODE:
+            if self.headless_auth_link_callback is None:
+                LOGGER.warning(
+                    "Headless mode is enabled, but no headless auth link callback "
+                    "has been set. The auth link will not be opened."
+                )
+                LOGGER.debug("Auth link: %s", auth_link)
+            else:
+                LOGGER.info("Sending auth link to callback")
+                self.headless_auth_link_callback(auth_link)
+        else:
+            open_browser(auth_link)
 
         request_args = self.temp_auth_server.wait_for_request(
             "/get_auth_code", kill_on_request=True
         )
 
         if state_token != request_args.get("state"):
             raise ValueError(
```

### Comparing `wg_utilities-3.2.0/wg_utilities/clients/spotify.py` & `wg_utilities-3.3.0/wg_utilities/clients/spotify.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from builtins import type as type_
 from collections.abc import Callable, Iterable, Iterator, Mapping, Sequence, Set
 from datetime import date, datetime, timedelta
 from enum import Enum
 from http import HTTPStatus
 from json import dumps
 from logging import DEBUG, getLogger
-from pathlib import Path
 from re import sub
 from typing import (
     Any,
     ClassVar,
     Generic,
     Literal,
     TypeAlias,
@@ -132,17 +131,18 @@
         log_requests (bool): flag for choosing if to log all requests made
         creds_cache_path (str): path at which to save cached credentials
     """
 
     AUTH_LINK_BASE = "https://accounts.spotify.com/authorize"
     ACCESS_TOKEN_ENDPOINT = "https://accounts.spotify.com/api/token"
     BASE_URL = "https://api.spotify.com/v1"
+
     DATETIME_FORMAT = "%Y-%m-%dT%H:%M:%SZ"
 
-    ALL_SCOPES = [
+    DEFAULT_SCOPES = [
         "ugc-image-upload",
         "user-read-recently-played",
         "user-top-read",
         "user-read-playback-position",
         "user-read-playback-state",
         "user-modify-playback-state",
         "user-read-currently-playing",
@@ -165,37 +165,15 @@
         "artist",
         "playlist",
         "track",
         # "show",
         # "episode",
     )
 
-    def __init__(
-        self,
-        *,
-        client_id: str,
-        client_secret: str,
-        log_requests: bool = False,
-        creds_cache_path: Path | None = None,
-        scopes: list[str] | None = None,
-        oauth_login_redirect_host: str = "localhost",
-    ):
-        super().__init__(
-            base_url=self.BASE_URL,
-            access_token_endpoint=self.ACCESS_TOKEN_ENDPOINT,
-            auth_link_base=self.AUTH_LINK_BASE,
-            client_id=client_id,
-            client_secret=client_secret,
-            log_requests=log_requests,
-            creds_cache_path=creds_cache_path,
-            scopes=scopes or self.ALL_SCOPES,
-            oauth_login_redirect_host=oauth_login_redirect_host,
-        )
-
-        self._current_user: User
+    _current_user: User
 
     def add_tracks_to_playlist(
         self,
         tracks: Iterable[Track],
         playlist: Playlist,
         *,
         log_responses: bool = False,
@@ -780,14 +758,15 @@
     )
     artists_json: list[ArtistSummaryJson] = Field(alias="artists")
     available_markets: list[str]
     copyrights: list[dict[str, str]] | None
     external_ids: dict[str, str] | None
     genres: list[str] | None
     images: list[Image]
+    is_playable: bool | None
     label: str | None
     popularity: int | None
     release_date_precision: Literal["year", "month", "day"] | None
     release_date: date
     restrictions: dict[str, str] | None
     total_tracks: int
     tracks_json: PaginatedResponseTracks = Field(
@@ -948,15 +927,15 @@
     available_markets: list[str]
     disc_number: int
     duration_ms: int
     episode: bool | None
     explicit: bool
     external_ids: dict[str, str] | None
     is_local: bool
-    is_playable: str | None
+    is_playable: bool | None
     linked_from: TrackFullJson | None
     popularity: int | None
     preview_url: str | None
     restrictions: str | None
     track: bool | None
     track_number: int
     type: Literal["track"]
```

### Comparing `wg_utilities-3.2.0/wg_utilities/clients/truelayer.py` & `wg_utilities-3.3.0/wg_utilities/clients/truelayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pylint: disable=too-few-public-methods
 """Custom client for interacting with TrueLayer's API."""
 from __future__ import annotations
 
-from collections.abc import Iterable
+from collections.abc import Callable, Iterable
 from datetime import date, datetime, timedelta
 from enum import Enum, auto
 from logging import DEBUG, getLogger
 from os.path import sep
 from pathlib import Path
 from typing import Any, ClassVar, Literal, TypeAlias, TypedDict, TypeVar
 
@@ -520,15 +520,15 @@
 class TrueLayerClient(OAuthClient[dict[Literal["results"], list[TrueLayerEntityJson]]]):
     """Custom client for interacting with TrueLayer's APIs."""
 
     AUTH_LINK_BASE = "https://auth.truelayer.com/"
     ACCESS_TOKEN_ENDPOINT = "https://auth.truelayer.com/connect/token"
     BASE_URL = "https://api.truelayer.com"
 
-    ALL_SCOPES = [
+    DEFAULT_SCOPES = [
         "info",
         "accounts",
         "balance",
         "cards",
         "transactions",
         "direct_debits",
         "standing_orders",
@@ -540,14 +540,15 @@
         *,
         client_id: str,
         client_secret: str,
         log_requests: bool = False,
         creds_cache_path: Path | None = None,
         scopes: list[str] | None = None,
         oauth_login_redirect_host: str = "localhost",
+        headless_auth_link_callback: Callable[[str], None] | None = None,
         bank: Bank,
     ):
         super().__init__(
             base_url=self.BASE_URL,
             access_token_endpoint=self.ACCESS_TOKEN_ENDPOINT,
             auth_link_base=self.AUTH_LINK_BASE,
             client_id=client_id,
@@ -562,16 +563,17 @@
                         "oauth_credentials",
                         type(self).__name__,
                         client_id,
                         f"{bank.name.lower()}.json",
                     ]
                 )
             ),
-            scopes=scopes or self.ALL_SCOPES,
+            scopes=scopes or self.DEFAULT_SCOPES,
             oauth_login_redirect_host=oauth_login_redirect_host,
+            headless_auth_link_callback=headless_auth_link_callback,
         )
 
         self.bank = bank
 
     def _get_entity_by_id(
         self,
         entity_id: str,
```

### Comparing `wg_utilities-3.2.0/wg_utilities/devices/dht22/dht22_lib.py` & `wg_utilities-3.3.0/wg_utilities/devices/dht22/dht22_lib.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.2.0/wg_utilities/devices/epd/__init__.py` & `wg_utilities-3.3.0/wg_utilities/devices/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.2.0/wg_utilities/devices/epd/epd7in5_v2.py` & `wg_utilities-3.3.0/wg_utilities/devices/epd/epd7in5_v2.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.2.0/wg_utilities/devices/epd/epdconfig.py` & `wg_utilities-3.3.0/wg_utilities/devices/epd/epdconfig.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.2.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py` & `wg_utilities-3.3.0/wg_utilities/devices/yamaha_yas_209/yamaha_yas_209.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.2.0/wg_utilities/exceptions/__init__.py` & `wg_utilities-3.3.0/wg_utilities/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.2.0/wg_utilities/functions/__init__.py` & `wg_utilities-3.3.0/wg_utilities/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.2.0/wg_utilities/functions/_functions.py` & `wg_utilities-3.3.0/wg_utilities/functions/_functions.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.2.0/wg_utilities/functions/datetime_helpers.py` & `wg_utilities-3.3.0/wg_utilities/functions/datetime_helpers.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.2.0/wg_utilities/functions/file_management.py` & `wg_utilities-3.3.0/wg_utilities/functions/file_management.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.2.0/wg_utilities/functions/json.py` & `wg_utilities-3.3.0/wg_utilities/functions/json.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.2.0/wg_utilities/functions/processes.py` & `wg_utilities-3.3.0/wg_utilities/functions/processes.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.2.0/wg_utilities/functions/string_manipulation.py` & `wg_utilities-3.3.0/wg_utilities/functions/string_manipulation.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.2.0/wg_utilities/functions/xml.py` & `wg_utilities-3.3.0/wg_utilities/functions/xml.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.2.0/wg_utilities/loggers/__init__.py` & `wg_utilities-3.3.0/wg_utilities/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `wg_utilities-3.2.0/wg_utilities/testing/_custom_mocks.py` & `wg_utilities-3.3.0/wg_utilities/testing/_custom_mocks.py`

 * *Files identical despite different names*

