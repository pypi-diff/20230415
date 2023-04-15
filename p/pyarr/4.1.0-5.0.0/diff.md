# Comparing `tmp/pyarr-4.1.0.tar.gz` & `tmp/pyarr-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyarr-4.1.0.tar", last modified: Tue Jun 28 13:04:42 2022, max compression
+gzip compressed data, was "pyarr-5.0.0.tar", max compression
```

## Comparing `pyarr-4.1.0.tar` & `pyarr-5.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1056 2022-06-28 13:04:11.245759 pyarr-4.1.0/LICENSE
--rw-r--r--   0        0        0     1351 2022-06-28 13:04:11.245759 pyarr-4.1.0/README.md
--rw-r--r--   0        0        0      249 2022-06-28 13:04:11.245759 pyarr-4.1.0/pyarr/__init__.py
--rw-r--r--   0        0        0    26203 2022-06-28 13:04:11.245759 pyarr-4.1.0/pyarr/base.py
--rw-r--r--   0        0        0      126 2022-06-28 13:04:11.245759 pyarr-4.1.0/pyarr/const.py
--rw-r--r--   0        0        0      709 2022-06-28 13:04:11.245759 pyarr-4.1.0/pyarr/exceptions.py
--rw-r--r--   0        0        0    28089 2022-06-28 13:04:11.245759 pyarr-4.1.0/pyarr/lidarr.py
--rw-r--r--   0        0        0        0 2022-06-28 13:04:11.245759 pyarr-4.1.0/pyarr/models/__init__.py
--rw-r--r--   0        0        0      139 2022-06-28 13:04:11.245759 pyarr-4.1.0/pyarr/models/common.py
--rw-r--r--   0        0        0     1137 2022-06-28 13:04:11.245759 pyarr-4.1.0/pyarr/models/lidarr.py
--rw-r--r--   0        0        0      806 2022-06-28 13:04:11.245759 pyarr-4.1.0/pyarr/models/radarr.py
--rw-r--r--   0        0        0     1204 2022-06-28 13:04:11.245759 pyarr-4.1.0/pyarr/models/readarr.py
--rw-r--r--   0        0        0      967 2022-06-28 13:04:11.245759 pyarr-4.1.0/pyarr/models/sonarr.py
--rw-r--r--   0        0        0        0 2022-06-28 13:04:11.245759 pyarr-4.1.0/pyarr/py.typed
--rw-r--r--   0        0        0    18288 2022-06-28 13:04:11.245759 pyarr-4.1.0/pyarr/radarr.py
--rw-r--r--   0        0        0    23297 2022-06-28 13:04:11.245759 pyarr-4.1.0/pyarr/readarr.py
--rw-r--r--   0        0        0     7849 2022-06-28 13:04:11.245759 pyarr-4.1.0/pyarr/request_handler.py
--rw-r--r--   0        0        0    18065 2022-06-28 13:04:11.245759 pyarr-4.1.0/pyarr/sonarr.py
--rw-r--r--   0        0        0     2565 2022-06-28 13:04:11.245759 pyarr-4.1.0/pyproject.toml
--rw-r--r--   0        0        0     2193 2022-06-28 13:04:42.661019 pyarr-4.1.0/setup.py
--rw-r--r--   0        0        0     2357 2022-06-28 13:04:42.661395 pyarr-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-04-15 19:14:27.549990 pyarr-5.0.0/LICENSE
+-rw-r--r--   0        0        0     6550 2023-04-15 19:14:27.549990 pyarr-5.0.0/README.md
+-rw-r--r--   0        0        0      249 2023-04-15 19:14:27.549990 pyarr-5.0.0/pyarr/__init__.py
+-rw-r--r--   0        0        0    30979 2023-04-15 19:14:27.549990 pyarr-5.0.0/pyarr/base.py
+-rw-r--r--   0        0        0      101 2023-04-15 19:14:27.549990 pyarr-5.0.0/pyarr/const.py
+-rw-r--r--   0        0        0      878 2023-04-15 19:14:27.549990 pyarr-5.0.0/pyarr/exceptions.py
+-rw-r--r--   0        0        0    26726 2023-04-15 19:14:27.549990 pyarr-5.0.0/pyarr/lidarr.py
+-rw-r--r--   0        0        0        0 2023-04-15 19:14:27.549990 pyarr-5.0.0/pyarr/models/__init__.py
+-rw-r--r--   0        0        0     2387 2023-04-15 19:14:27.549990 pyarr-5.0.0/pyarr/models/common.py
+-rw-r--r--   0        0        0      974 2023-04-15 19:14:27.549990 pyarr-5.0.0/pyarr/models/lidarr.py
+-rw-r--r--   0        0        0     1758 2023-04-15 19:14:27.549990 pyarr-5.0.0/pyarr/models/radarr.py
+-rw-r--r--   0        0        0     1833 2023-04-15 19:14:27.549990 pyarr-5.0.0/pyarr/models/readarr.py
+-rw-r--r--   0        0        0     2057 2023-04-15 19:14:27.549990 pyarr-5.0.0/pyarr/models/sonarr.py
+-rw-r--r--   0        0        0        0 2023-04-15 19:14:27.549990 pyarr-5.0.0/pyarr/py.typed
+-rw-r--r--   0        0        0    20044 2023-04-15 19:14:27.553990 pyarr-5.0.0/pyarr/radarr.py
+-rw-r--r--   0        0        0    31128 2023-04-15 19:14:27.553990 pyarr-5.0.0/pyarr/readarr.py
+-rw-r--r--   0        0        0     8163 2023-04-15 19:14:27.553990 pyarr-5.0.0/pyarr/request_handler.py
+-rw-r--r--   0        0        0    27253 2023-04-15 19:14:27.553990 pyarr-5.0.0/pyarr/sonarr.py
+-rw-r--r--   0        0        0      300 2023-04-15 19:14:27.553990 pyarr-5.0.0/pyarr/types.py
+-rw-r--r--   0        0        0     3092 2023-04-15 19:14:27.553990 pyarr-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7854 1970-01-01 00:00:00.000000 pyarr-5.0.0/PKG-INFO
```

### Comparing `pyarr-4.1.0/LICENSE` & `pyarr-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyarr-4.1.0/pyarr/base.py` & `pyarr-5.0.0/pyarr/sonarr.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,813 +1,771 @@
 from datetime import datetime
 from typing import Any, Optional, Union
+from warnings import warn
 
 from requests import Response
 
-from .const import PAGE, PAGE_SIZE
-from .request_handler import RequestHandler
+from pyarr.exceptions import PyarrMissingArgument
+from pyarr.types import JsonArray, JsonObject
 
+from .base import BaseArrAPI
+from .models.common import PyarrHistorySortKey, PyarrSortDirection
+from .models.sonarr import SonarrCommands, SonarrSortKey
 
-class BaseArrAPI(RequestHandler):
-    """Base functions in all Arr API's"""
 
-    def __init__(self, host_url: str, api_key: str, ver_uri: str = "/"):
-        """Initialise the instance connection
+class SonarrAPI(BaseArrAPI):
+    """API wrapper for Sonarr endpoints."""
 
-        Args:
-            host_url (str): URL to Arr instance
-            api_key (str): API key for Arr instance
-            ver_uri (str, optional): API Version. Defaults to "/".
-        """
-
-        self.ver_uri = ver_uri
-        super().__init__(host_url, api_key)
-
-    def assert_return(
-        self,
-        path: str,
-        ver_uri: str,
-        typearg: type,
-        params: Optional[dict[str, Any]] = None,
-    ) -> Any:
-        """Helper function to add assert to enforce typing responses
+    def __init__(self, host_url: str, api_key: str, ver_uri: str = "/v3"):
+        """Initialize the Sonarr API.
 
         Args:
-            path (str): Path on API
-            ver_uri (str): API Version
-            typearg (type): Python Type
-            params (Union[dict[str, Any], None], optional): Any required params. Defaults to None.
-
-        Returns:
-            Any: Any
+            host_url (str): URL for Sonarr
+            api_key (str): API key for Sonarr
+            ver_uri (str): Version URI for Radarr. Defaults to None (empty string).
         """
-        if params is None:
-            response = self._get(path, ver_uri)
-        else:
-            response = self._get(path, ver_uri, params=params)
-        assert isinstance(response, typearg)
-        return response
 
-    # CALENDAR
+        super().__init__(host_url, api_key, ver_uri)
 
-    # GET /calendar/
-    def get_calendar(
+    # POST /rootfolder
+    def add_root_folder(
         self,
-        start_date: Optional[str] = None,
-        end_date: Optional[str] = None,
-        unmonitored: bool = True,
-    ) -> list[dict[str, Any]]:
-        """Gets upcoming releases by monitored, if start/end are not
-        supplied, today and tomorrow will be returned
+        directory: str,
+    ) -> JsonObject:
+        """Adds a new root folder
 
         Args:
-            start_date (Optional[str], optional): ISO8601 start datetime. Defaults to None.
-            end_date (Optional[str], optional): ISO8601 end datetime. Defaults to None.
-            unmonitored (bool, optional): Include unmonitored movies. Defaults to True.
-
-        Returns:
-            list[dict[str, Any]]: List of dictionaries with items
-        """
-        params: dict[str, Any] = {}
-        if start_date:
-            params["start"] = datetime.strptime(start_date, "%Y-%m-%d").strftime(
-                "%Y-%m-%d"
-            )
-        if end_date:
-            params["end"] = datetime.strptime(end_date, "%Y-%m-%d").strftime("%Y-%m-%d")
-        params["unmonitored"] = unmonitored
-
-        return self.assert_return("calendar", self.ver_uri, list, params)
-
-    # SYSTEM
-
-    # GET /system/status
-    def get_system_status(self) -> list[dict[str, Any]]:
-        """Gets system status
+            directory (str): The directory path
 
         Returns:
-           list[dict[str, Any]]: List of dictionaries with items
+            JsonObject: Dictionary containing path details
         """
-        return self.assert_return("system/status", self.ver_uri, list)
+        return self._post("rootfolder", self.ver_uri, data={"path": directory})
 
-    # GET /health
-    def get_health(self) -> list[dict[str, Any]]:
-        """Get health information
+    ## COMMAND
 
-        Returns:
-            list[dict[str, Any]]: List of dictionaries with items
-        """
-        return self.assert_return("health", self.ver_uri, list)
-
-    # GET /metadata
-    def get_metadata(self) -> list[dict[str, Any]]:
-        """Get all metadata consumer settings
-
-        Returns:
-             list[dict[str, Any]]: List of dictionaries with items
-        """
-        return self.assert_return("metadata", self.ver_uri, list)
-
-    # GET /update
-    def get_update(self) -> list[dict[str, Any]]:
-        """Will return a list of recent updated
-
-        Returns:
-             list[dict[str, Any]]: List of dictionaries with items
-        """
-        return self.assert_return("update", self.ver_uri, list)
-
-    # GET /rootfolder
-    def get_root_folder(self) -> list[dict[str, Any]]:
-        """Get list of root folders, free space and any unmappedFolders
-
-        Returns:
-             list[dict[str, Any]]: List of dictionaries with items
-        """
-        return self.assert_return("rootfolder", self.ver_uri, list)
-
-    # DELETE /rootfolder
-    def del_root_folder(
-        self, id_: int
-    ) -> Union[
-        Response, dict[str, Any], dict[Any, Any]
-    ]:  # sourcery skip: class-extract-method
-        """Delete root folder with specified id
+    # POST /command
+    # TODO: Add more logic to ensure correct kwargs for a command
+    def post_command(
+        self, name: SonarrCommands, **kwargs: Optional[dict[str, Union[int, list[int]]]]
+    ) -> JsonObject:
+        """Performs any of the predetermined Sonarr command routines
 
         Args:
-            id_ (int): Root folder id from database
-
-        Returns:
-            Response: HTTP Response
-        """
-        params = {"id": id_}
-        return self._delete("rootfolder", self.ver_uri, params=params)
-
-    # GET /diskspace
-    def get_disk_space(self) -> list[dict[str, Any]]:
-        """Query disk usage information
-            System > Status
-
-        Returns:
-            list[dict[str, Any]]: List of dictionaries with items
-        """
-        return self.assert_return("diskspace", self.ver_uri, list)
-
-    # GET /system/backup
-    def get_backup(self) -> list[dict[str, Any]]:
-        """Returns the list of available backups
-
-        Returns:
-            list[dict[str, Any]]: List of dictionaries with items
-        """
-        return self.assert_return("system/backup", self.ver_uri, list)
-
-    # LOGS
-
-    # GET /log
-    def get_log(
-        self,
-        page: int = PAGE,
-        page_size: int = PAGE_SIZE,
-        sort_key: str = "time",
-        sort_dir: str = "desc",
-        filter_key: Optional[str] = None,
-        filter_value: str = "All",
-    ) -> list[dict[str, Any]]:
-        """Gets logs from instance
-
-        Args:
-            page (int, optional): Specifiy page to return. Defaults to PAGE.
-            page_size (int, optional): Number of items per page. Defaults to PAGE_SIZE.
-            sort_key (str, optional): Field to sort by. Defaults to "time".
-            sort_dir (str, optional): Direction to sort. Defaults to "desc".
-            filter_key (Optional[str], optional): Key to filter by. Defaults to None.
-            filter_value (str, optional): Value of the filter. Defaults to "All".
-
-        Returns:
-            list[dict[str, Any]]: List of dictionaries with items
-        """
-        params = {
-            "page": page,
-            "pageSize": page_size,
-            "sortKey": sort_key,
-            "sortDir": sort_dir,
-            "filterKey": filter_key,
-            "filterValue": filter_value,
-        }
-        return self.assert_return("log", self.ver_uri, list, params)
-
-    # GET /history
-    # TODO: check the ID on this method may need to move to specific APIs
-    def get_history(
-        self,
-        sort_key: str = "date",
-        page: int = PAGE,
-        page_size: int = PAGE_SIZE,
-        sort_dir: str = "desc",
-        id_: Optional[int] = None,
-    ) -> list[dict[str, Any]]:
-        """Gets history (grabs/failures/completed)
+            name (SonarrCommands): Command that should be executed
+            **kwargs: Additional parameters for specific commands.
 
-        Args:
-            sort_key (str, optional): Field to sort by. Defaults to "date".
-            page (int, optional): Page number to return. Defaults to PAGE.
-            page_size (int, optional): Number of items per page. Defaults to PAGE_SIZE.
-            sort_dir (str, optional): Direction to sort the items. Defaults to "desc".
-            id_ (Optional[int], optional): Filter to a specific episode ID. Defaults to None.
+        Note:
+            For available commands and required `**kwargs` see the `SonarrCommands` model
 
         Returns:
-           list[dict[str, Any]]: List of dictionaries with items
+            JsonObject: Dictionary containing job
         """
-        params = {
-            "sortKey": sort_key,
-            "page": page,
-            "pageSize": page_size,
-            "sortDir": sort_dir,
+        data: dict[str, Any] = {
+            "name": name,
         }
-        if id_:
-            params["episodeId"] = id_
-        return self.assert_return("history", self.ver_uri, list, params)
+        if kwargs:
+            data |= kwargs
+        return self._post("command", self.ver_uri, data=data)
 
-    # BLOCKLIST
+    ## EPISODE
 
-    # GET /blocklist
-    def get_blocklist(
-        self,
-        page: int = PAGE,
-        page_size: int = PAGE_SIZE,
-        sort_direction: str = "descending",
-        sort_key: str = "date",
-    ) -> list[dict[str, Any]]:
-        """Returns blocked releases.
-
-        Args:
-            page (int, optional): Page to be returned. Defaults to PAGE.
-            page_size (int, optional): Number of results per page. Defaults to PAGE_SIZE.
-            sort_direction (str, optional): Direction to sort items. Defaults to "descending".
-            sort_key (str, optional): Field to sort by. Defaults to "date".
-
-        Returns:
-            list[dict[str, Any]]: List of dictionaries with items
-        """
-        params = {
-            "page": page,
-            "pageSize": page_size,
-            "sortDirection": sort_direction,
-            "sortKey": sort_key,
-        }
-        return self.assert_return("blocklist", self.ver_uri, list, params)
-
-    # DELETE /blocklist
-    def del_blocklist(
-        self, id_: int
-    ) -> Union[Response, dict[str, Any], dict[Any, Any]]:
-        """Removes a specific release (the id provided) from the blocklist
+    # GET /episode
+    def get_episode(self, id_: int, series: bool = False) -> JsonObject:
+        """Get episodes by ID or series
 
         Args:
-            id_ (int): Blocklist ID from database
+            id_ (int): ID for Episode or Series.
+            series (bool, optional): Set to true if the ID is for a Series. Defaults to false.
 
         Returns:
-            Response: HTTP Response
+            JsonArray: List of dictionaries with items
         """
-        params = {"id": id_}
-        return self._delete("blocklist", self.ver_uri, params=params)
+        return self._get(
+            f"episode{'' if series else f'/{id_}'}",
+            self.ver_uri,
+            params={"seriesId": id_} if series else None,
+        )
 
-    # DELETE /blocklist/bulk
-    def del_blocklist_bulk(
-        self, data: dict[str, Any]
-    ) -> Union[Response, dict[str, Any], dict[Any, Any]]:
-        """Delete blocked releases in bulk
+    # GET /episode
+    def get_episodes_by_series_id(self, id_: int) -> JsonArray:
+        # sourcery skip: class-extract-method
+        """Gets all episodes from a given series ID
 
         Args:
-            data (dict[str, Any]): Blocklists that should be deleted
+            id_ (int): Database id for series
+
+        Note:
+            This method is deprecated and will be removed in a
+            future release. Please use get_episode()
 
         Returns:
-            Response: HTTP Response
+            JsonArray: List of dictionaries with items
         """
-        return self._delete("blocklist/bulk", self.ver_uri, data=data)
-
-    # PROFILES
+        warn(
+            "This method is deprecated and will be removed in a future release. Please use get_episode()",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        params = {"seriesId": id_}
+        return self._get("episode", self.ver_uri, params)
 
-    # GET /qualityprofile/{id}
-    def get_quality_profile(self, id_: Optional[int] = None) -> list[dict[str, Any]]:
-        """Gets all quality profiles or specific one with id_
+    # GET /episode/{id}
+    def get_episode_by_episode_id(self, id_: int) -> JsonObject:
+        """Gets a specific episode by database id
 
         Args:
-            id_ (Optional[int], optional): Quality profile id from database. Defaults to None.
-
-        Returns:
-            list[dict[str, Any]]: List of dictionaries with items
-        """
-        path = f"qualityprofile/{id_}" if id_ else "qualityprofile"
-        return self.assert_return(path, self.ver_uri, list)
-
-    # PUT /qualityprofile/{id}
-    def upd_quality_profile(self, id_: int, data: dict[str, Any]) -> dict[str, Any]:
-        """Update the quality profile data
+            id_ (int): Database id for episode
 
         Note:
-            To be used in conjunction with get_quality_profile()
-
-        Args:
-            id_ (int): Profile ID to Update
-            data (dict[str, Any]): All parameters to update
+            This method is deprecated and will be removed in a
+            future release. Please use get_episode()
 
         Returns:
-            dict[str, Any]: Dictionary of updated record
+            JsonArray: List of dictionaries with items
         """
-        return self._put(f"qualityprofile/{id_}", self.ver_uri, data=data)
+        warn(
+            "This method is deprecated and will be removed in a future release. Please use get_episode()",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return self._get(f"episode/{id_}", self.ver_uri)
 
-    # DELETE /qualityprofile
-    def del_quality_profile(
-        self, id_: int
-    ) -> Union[Response, dict[str, Any], dict[Any, Any]]:
-        """Removes a specific quality profile from the blocklist
+    # PUT /episode
+    def upd_episode(self, id_: int, data: JsonObject) -> JsonObject:
+        """Update the given episodes, currently only monitored is supported
 
         Args:
-            id_ (int): Quality profile ID from database
+            id_ (int): ID of the Episode to be updated
+            data (dict[str, Any]): Parameters to update the episode
 
-        Returns:
-            Response: HTTP Response
-        """
-        params = {"id": id_}
-        return self._delete("qualityprofile", self.ver_uri, params=params)
+        Example:
+            ::
 
-    # GET /qualitydefinition/{id}
-    def get_quality_definition(self, id_: Optional[int] = None) -> list[dict[str, Any]]:
-        """Gets all quality definitions or specific one by ID
-
-        Args:
-            id_ (Optional[int], optional): Import list database id. Defaults to None.
+                payload = {"monitored": True}
+                sonarr.upd_episode(1, payload)
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            JsonObject: Dictionary with updated record
         """
-        path = f"qualitydefinition/{id_}" if id_ else "qualitydefinition"
-        return self.assert_return(path, self.ver_uri, list)
+        return self._put(f"episode/{id_}", self.ver_uri, data=data)
 
-    # PUT /qualitydefinition/{id}
-    def upd_quality_definition(self, id_: int, data: dict[str, Any]) -> dict[str, Any]:
-        """Update the quality definitions.
-
-        Note:
-            To be used in conjunction with get_quality_definition()
+    # PUT /episode/monitor
+    def upd_episode_monitor(
+        self, episode_ids: list[int], monitored: bool = True
+    ) -> JsonArray:
+        """Update episode monitored status
 
         Args:
-            id_ (int): ID of definition to update
-            data (dict[str, Any]): All parameters to update
+            episode_ids (list[int]): All episode IDs to be updated
+            monitored (bool, optional): True or False. Defaults to True.
 
         Returns:
-            dict[str, Any]: Dictionary of updated record
+            JsonArray: list of dictionaries containing updated records
         """
-        return self._put(f"qualitydefinition/{id_}", self.ver_uri, data=data)
+        return self._put(
+            "episode/monitor",
+            self.ver_uri,
+            data={"episodeIds": episode_ids, "monitored": monitored},
+        )
 
-    # INDEXER
+    ## EPISODE FILE
 
-    # GET /indexer/{id}
-    def get_indexer(self, id_: Optional[int] = None) -> list[dict[str, Any]]:
-        """Get all indexers or specific by id
+    # GET /episodefile
+    def get_episode_files_by_series_id(self, id_: int) -> JsonArray:
+        """Returns all episode file information for series id specified
 
         Args:
-            id_ (Optional[int], optional): Database if of indexer to return. Defaults to None.
+            id_ (int): Database id of series
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            JsonArray: List of dictionaries with items
         """
-        path = f"indexer/{id_}" if id_ else "indexer"
-        return self.assert_return(path, self.ver_uri, list)
+        warn(
+            "This method is deprecated and will be removed in a future release. Please use get_episode_file()",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        params = {"seriesId": id_}
+        return self._get("episodefile", self.ver_uri, params)
 
-    # PUT /indexer/{id}
-    def upd_indexer(self, id_: int, data: dict[str, Any]) -> dict[str, Any]:
-        """Edit a Indexer by database id
-
-        Note:
-            To be used in conjunction with get_indexer()
+    # GET /episodefile/{id}
+    def get_episode_file(self, id_: int, series: bool = False) -> JsonObject:
+        """Returns episode file information for specified id
 
         Args:
-            id_ (int): Indexer database id
-            data (dict[str, Any]): Data to be updated within Indexer
+            id_ (int): Database id of episode file
+            series (bool, optional): Set to true if the ID is for a Series. Defaults to false.
 
         Returns:
-            dict[str, Any]: Dictionary of updated record
+            JsonObject: Dictionary with data
         """
-        return self._put(f"indexer/{id_}", self.ver_uri, data=data)
+        return self._get(
+            f"episodefile{'' if series else f'/{id_}'}",
+            self.ver_uri,
+            params={"seriesId": id_} if series else None,
+        )
 
-    # DELETE /indexer
-    def del_indexer(self, id_: int) -> Union[Response, dict[str, Any], dict[Any, Any]]:
-        """Removes a specific indexer from the blocklist
+    # DELETE /episodefile/{id}
+    def del_episode_file(self, id_: int) -> Union[Response, JsonObject, dict[Any, Any]]:
+        """Deletes the episode file with corresponding id
 
         Args:
-            id_ (int): indexer id from database
+            id_ (int): Database id for episode file
 
         Returns:
             Response: HTTP Response
         """
-        params = {"id": id_}
-        return self._delete("indexer", self.ver_uri, params=params)
-
-    # QUEUE
+        return self._delete(f"episodefile/{id_}", self.ver_uri)
 
-    # DELETE /queue/{id}
-    def del_queue(
-        self, id_: int, remove_from_client: bool = True, blacklist: bool = True
-    ) -> Union[Response, dict[str, Any], dict[Any, Any]]:
-        """Remove an item from the queue and blacklist it
+    # PUT /episodefile/{id}
+    def upd_episode_file_quality(self, id_: int, data: JsonObject) -> JsonObject:
+        """Updates the quality of the episode file and returns the episode file
 
         Args:
-            id_ (int): ID of the item to be removed
-            remove_from_client (bool, optional): Remove the item from the client. Defaults to True.
-            blacklist (bool, optional): Add the item to the blacklist. Defaults to True.
+            id_ (int): Database id for episode file
+            data (JsonObject): data with quality::
+
+                {
+                    "quality": {
+                        "quality": {
+                        "id": 8
+                        },
+                        "revision": {
+                        "version": 1,
+                        "real": 0
+                        }
+                    },
+                }
 
         Returns:
-            Response: HTTP Response
+            JsonObject: Dictionary with updated record
         """
-        params = {"removeFromClient": remove_from_client, "blacklist": blacklist}
-        return self._delete(f"queue/{id_}", self.ver_uri, params=params)
+        return self._put(f"episodefile/{id_}", self.ver_uri, data=data)
 
-    # GET /system/task/{id}
-    def get_task(self, id_: Optional[int] = None) -> list[dict[str, Any]]:
-        """Return a list of tasks, or specify a task ID to return single task
+    # GET /wanted/missing
+    def get_wanted(
+        self,
+        page: Optional[int] = None,
+        page_size: Optional[int] = None,
+        sort_key: Optional[SonarrSortKey] = None,
+        sort_dir: Optional[PyarrSortDirection] = None,
+        include_series: Optional[bool] = None,
+    ) -> JsonObject:
+        """Gets missing episode (episodes without files)
+
+        Args:
+            page (Optional[int], optional): Page number to return. Defaults to None.
+            page_size (Optional[int], optional): Number of items per page. Defaults to None.
+            sort_key (Optional[SonarrSortKey], optional): series.title or airDateUtc. Defaults to None.
+            sort_dir (Optional[PyarrSortDirection], optional): Direction to sort the items. Defaults to None.
+            include_series (Optional[bool], optional): Include the whole series. Defaults to None
+
+        Returns:
+            JsonObject: Dictionary with items
+        """
+        params: dict[str, Union[int, SonarrSortKey, PyarrSortDirection, bool]] = {}
+        if page:
+            params["page"] = page
+        if page_size:
+            params["pageSize"] = page_size
+        if sort_key and sort_dir:
+            params["sortKey"] = sort_key
+            params["sortDirection"] = sort_dir
+        elif sort_key or sort_dir:
+            raise PyarrMissingArgument("sort_key and sort_dir  must be used together")
+        if include_series:
+            params["includeSeries"] = include_series
 
-        Args:
-            id_ (Optional[int], optional):  ID for task. Defaults to None.
+        return self._get("wanted/missing", self.ver_uri, params)
 
-        Returns:
-            list[dict[str, Any]]: List of dictionaries with items
-        """
-        path = f"system/task/{id_}" if id_ else "system/task"
-        return self.assert_return(path, self.ver_uri, list)
+    ## QUEUE
 
-    # GET /remotepathmapping
-    def get_remote_path_mapping(
-        self, id_: Optional[int] = None
-    ) -> list[dict[str, Any]]:
-        """Get remote path mappings for downloads Directory
+    # GET /queue
+    def get_queue(
+        self,
+        page: Optional[int] = None,
+        page_size: Optional[int] = None,
+        sort_key: Optional[SonarrSortKey] = None,
+        sort_dir: Optional[PyarrSortDirection] = None,
+        include_unknown_series_items: Optional[bool] = None,
+        include_series: Optional[bool] = None,
+        include_episode: Optional[bool] = None,
+    ) -> JsonObject:
+        """Gets currently downloading info
+
+        Args:
+            page (Optional[int], optional): Page number to return. Defaults to None.
+            page_size (Optional[int], optional): Number of items per page. Defaults to None.
+            sort_key (Optional[SonarrSortKey], optional): Field to sort by. Defaults to None.
+            sort_dir (Optional[PyarrSortDirection], optional): Direction to sort the items. Defaults to None.
+            include_unknown_series_items (Optional[bool], optional): Include unknown series items. Defaults to None.
+            include_series (Optional[bool], optional): Include series. Defaults to None.
+            include_episode (Optional[bool], optional): Include episodes. Defaults to None.
+
+        Returns:
+            JsonObject: Dictionary with queue items
+        """
+        params: dict[str, Union[int, bool, SonarrSortKey, PyarrSortDirection]] = {}
+
+        if page:
+            params["page"] = page
+        if page_size:
+            params["pageSize"] = page_size
+        if sort_key and sort_dir:
+            params["sortKey"] = sort_key
+            params["sortDirection"] = sort_dir
+        elif sort_key or sort_dir:
+            raise PyarrMissingArgument("sort_key and sort_dir  must be used together")
+        if include_unknown_series_items is not None:
+            params["includeUnknownSeriesItems"] = include_unknown_series_items
+        if include_series is not None:
+            params["includeSeries"] = include_series
+        if include_episode is not None:
+            params["includeEpisode"] = include_episode
+
+        return self._get("queue", self.ver_uri, params)
+
+    ## PARSE
+
+    def get_parse_title_path(
+        self, title: Optional[str] = None, path: Optional[str] = None
+    ) -> JsonObject:
+        """Returns the result of parsing a title or path. series and episodes will be
+        returned only if the parsing matches to a specific series and one or more
+        episodes. series and episodes will be formatted the same as Series and Episode
+        responses.
 
         Args:
-            id_ (Optional[int], optional): ID for specific record. Defaults to None.
-
-        Returns:
-            list[dict[str, Any]]: List of dictionaries with items
-        """
-        _path = "" if isinstance(id_, str) or id_ is None else f"/{id_}"
-        return self.assert_return(f"remotepathmapping{_path}", self.ver_uri, list)
+            title (Optional[str], optional): Title of series or episode. Defaults to None.
+            path (Optional[str], optional): file path of series or episode. Defaults to None.
 
-    # CONFIG
-
-    # GET /config/ui
-    def get_config_ui(self) -> dict[str, Any]:
-        """Query Radarr for UI configuration
+        Raises:
+            PyarrMissingArgument: If no argument is passed, error
 
         Returns:
-            dict[str, Any]: List of dictionaries with items
+            JsonObject: Dictionary with items
         """
-        return self.assert_return("config/ui", self.ver_uri, dict)
+        if title is None and path is None:
+            raise PyarrMissingArgument("A title or path must be specified")
+        params = {}
+        if title is not None:
+            params["title"] = title
+        if path is not None:
+            params["path"] = path
+        return self._get("parse", self.ver_uri, params)
 
-    # PUT /config/ui
-    def upd_config_ui(self, data: dict[str, Any]) -> dict[str, Any]:
-        """Edit one or many UI settings and save to to the database
+    # GET /parse
+    def get_parsed_title(self, title: str) -> JsonObject:
+        """Returns the result of parsing a title. series and episodes will be
+        returned only if the parsing matches to a specific series and one or more
+        episodes. series and episodes will be formatted the same as Series and Episode
+        responses.
 
         Args:
-            data (dict[str, Any]): Data to be Updated.
-
-        Returns:
-            dict[str, Any]: Dictionary with items
-        """
-        return self._put("config/ui", self.ver_uri, data=data)
-
-    # GET /config/host
-    def get_config_host(self) -> dict[str, Any]:
-        """Get General/Host settings.
+            title (str): Title of series / episode
 
         Returns:
-            dict[str, Any]: Dictionaries with items
+            JsonObject: List of dictionaries with items
         """
-        return self.assert_return("config/host", self.ver_uri, dict)
+        warn(
+            "This method is deprecated and will be removed in a future release. Please use get_parse_title_path()",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return self._get("parse", self.ver_uri, {"title": title})
 
-    # PUT /config/host
-    def upd_config_host(self, data: dict[str, Any]) -> dict[str, Any]:
-        """Edit General/Host settings.
+    # GET /parse
+    def get_parsed_path(self, file_path: str) -> JsonObject:
+        """Returns the result of parsing a file path. series and episodes will be
+        returned only if the parsing matches to a specific series and one or more
+        episodes. series and episodes will be formatted the same as Series and Episode
+        responses.
 
         Args:
-            data (dict[str, Any]): data to be updated
+            file_path (str): file path of series / episode
 
         Returns:
-            dict[str, Any]: Dictionaries with items
+            JsonObject: List of dictionaries with items
         """
-        return self._put("config/host", self.ver_uri, data=data)
+        warn(
+            "This method is deprecated and will be removed in a future release. Please use get_parse_title_path()",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return self._get("parse", self.ver_uri, {"path": file_path})
 
-    # GET /config/naming
-    def get_config_naming(self) -> dict[str, Any]:
-        """Get Settings for file and folder naming.
+    ## RELEASE
 
-        Returns:
-            dict[str, Any]: Dictionary with items
-        """
-        return self.assert_return("config/naming", self.ver_uri, dict)
-
-    # PUT /config/naming
-    def upd_config_naming(self, data: dict[str, Any]) -> dict[str, Any]:
-        """Edit Settings for file and folder naming.
+    # GET /release
+    def get_releases(self, id_: Optional[int] = None) -> JsonArray:
+        """Query indexers for latest releases.
 
         Args:
-            data (dict[str, Any]): data to be updated
+            id_ (int): Database id for episode to check
 
         Returns:
-            dict[str, Any]: Dictionary with items
+            JsonArray: List of dictionaries with items
         """
-        return self._put("config/naming", self.ver_uri, data=data)
+        return self._get("release", self.ver_uri, {"episodeId": id_} if id_ else None)
 
-    # GET /config/mediamanagement
-    def get_media_management(self) -> dict[str, Any]:
-        """Get media management configuration
-
-        Returns:
-            dict[str, Any]: Dictionary with items
-        """
-        return self.assert_return("config/mediamanagement", self.ver_uri, dict)
-
-    # PUT /config/mediamanagement
-    def upd_media_management(self, data: dict[str, Any]) -> dict[str, Any]:
-        """Get media management configuration
-
-        Note:
-            Recommended to use with get_media_management()
+    # POST /release
+    def download_release(self, guid: str, indexer_id: int) -> JsonObject:
+        """Adds a previously searched release to the download client, if the release is
+         still in Sonarr's search cache (30 minute cache). If the release is not found
+         in the cache Sonarr will return a 404.
 
         Args:
-            data (dict[str, Any]): data to be updated
+            guid (str): Recently searched result guid
+            indexer_id (int): Database id of indexer to use
 
         Returns:
-            dict[str, Any]: Dictionary with items
+            JsonObject: Dictionary with download release details
         """
-        return self._put("config/mediamanagement", self.ver_uri, data=data)
-
-    # NOTIFICATIONS
+        data = {"guid": guid, "indexerId": indexer_id}
+        return self._post("release", self.ver_uri, data=data)
 
-    # GET /notification
-    def get_notification(self, id_: Optional[int] = None) -> list[dict[str, Any]]:
-        """Get a list of all notification services, or single by ID
+    # POST /release/push
+    # TODO: find response
+    def push_release(
+        self, title: str, download_url: str, protocol: str, publish_date: datetime
+    ) -> Any:
+        """If the title is wanted, Sonarr will grab it.
 
         Args:
-            id_ (Optional[int], optional): Notification ID. Defaults to None.
+            title (str): Release name
+            download_url (str): .torrent file URL
+            protocol (str): "Usenet" or "Torrent
+            publish_date (datetime): ISO8601 date
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            JSON: Array
         """
-        _path = "" if isinstance(id_, str) or id_ is None else f"/{id_}"
-        return self.assert_return(f"notification{_path}", self.ver_uri, list)
-
-    # GET /notification/schema
-    def get_notification_schema(self) -> list[dict[str, Any]]:
-        """Get possible notification connections
-
-        Returns:
-            list[dict[str, Any]]: List of dictionaries with items
-        """
-        return self.assert_return("notification/schema", self.ver_uri, list)
+        data = {
+            "title": title,
+            "downloadUrl": download_url,
+            "protocol": protocol,
+            "publishDate": publish_date.isoformat(),
+        }
+        return self._post("release/push", self.ver_uri, data=data)
 
-    # PUT /notification/{id}
-    def upd_notification(self, id_: int, data: dict[str, Any]) -> dict[str, Any]:
-        """Edit notification by database id
+    ## SERIES
+    # GET /series and /series/{id}
+    def get_series(
+        self, id_: Optional[int] = None, tvdb: Optional[bool] = False
+    ) -> Union[JsonArray, JsonObject]:
+        """Returns all series in your collection or the series with the matching
+        series ID if one is found.
 
         Args:
-            id_ (int): Database id of notification
-            data (dict[str, Any]): data that requires updating
+            id_ (Optional[int], optional): Database id for series. Defaults to None.
+            tvdb (Optional[bool], optional): Set to true if ID is tvdb. Defaults to False
 
         Returns:
-            dict[str, Any]: Dictionary of updated record
+            Union[JsonArray, JsonObject]: List of dictionaries with items, or a
+            dictionary with single item
         """
-        return self._put(f"notification/{id_}", self.ver_uri, data=data)
+        if id_ and tvdb:
+            path = f"series?tvdbId={id_}"
+        else:
+            path = f"series{f'/{id_}' if id_ else ''}"
+        return self._get(path, self.ver_uri)
 
-    # DELETE /notification/{id}
-    def del_notification(
-        self, id_: int
-    ) -> Union[Response, dict[str, Any], dict[Any, Any]]:
-        """Delete a notification by its database id
+    # POST /series
+    def add_series(
+        self,
+        series: JsonObject,
+        quality_profile_id: int,
+        language_profile_id: int,
+        root_dir: str,
+        season_folder: bool = True,
+        monitored: bool = True,
+        ignore_episodes_with_files: bool = False,
+        ignore_episodes_without_files: bool = False,
+        search_for_missing_episodes: bool = False,
+    ) -> JsonObject:
+        """Adds a new series to your collection
+
+        Note:
+            if you do not add the required params, then the series wont function. some of these without the others can
+            indeed make a "series". But it wont function properly in nzbdrone.
 
         Args:
-            id_ (int): Database id of notification.
+            series (JsonObject): A series object from `lookup()`
+            quality_profile_id (int): Database id for quality profile
+            language_profile_id (int): Database id for language profile
+            root_dir (str): Root folder location, full path will be created from this
+            season_folder (bool, optional): Create a folder for each season. Defaults to True.
+            monitored (bool, optional): Monitor this series. Defaults to True.
+            ignore_episodes_with_files (bool, optional): Ignore any episodes with existing files. Defaults to False.
+            ignore_episodes_without_files (bool, optional): Ignore any episodes without existing files. Defaults to False.
+            search_for_missing_episodes (bool, optional): Search for missing episodes to download. Defaults to False.
+
+        Returns:
+            JsonObject: Dictionary of added record
+        """
+        if not monitored and series.get("seasons"):
+            for season in series["seasons"]:
+                season["monitored"] = False
+
+        series["rootFolderPath"] = root_dir
+        series["qualityProfileId"] = quality_profile_id
+        series["languageProfileId"] = language_profile_id
+        series["seasonFolder"] = season_folder
+        series["monitored"] = monitored
+        series["addOptions"] = {
+            "ignoreEpisodesWithFiles": ignore_episodes_with_files,
+            "ignoreEpisodesWithoutFiles": ignore_episodes_without_files,
+            "searchForMissingEpisodes": search_for_missing_episodes,
+        }
 
-        Returns:
-            Response: HTTP Response
-        """
-        return self._delete(f"notification/{id_}", self.ver_uri)
+        response: dict[str, Any] = self._post("series", self.ver_uri, data=series)
+        for item in response:
+            if "errorMessage" in item:
+                raise Exception(item)
+            else:
+                continue
 
-    # TAGS
+        return response
 
-    # GET /tag/{id}
-    def get_tag(self, id_: Optional[int] = None) -> list[dict[str, Any]]:
-        """Returns all tags or specific tag by database id
+    # PUT /series
+    def upd_series(self, data: JsonObject) -> JsonObject:
+        """Update an existing series
 
         Args:
-            id_ (Optional[int], optional): Database id for tag. Defaults to None.
+            data (JsonObject): contains data obtained by get_series()
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            JsonObject: Dictionary or updated record
         """
-        path = f"tag/{id_}" if id_ else "tag"
-        return self.assert_return(path, self.ver_uri, list)
+        return self._put("series", self.ver_uri, data=data)
 
-    # GET /tag/detail/{id}
-    def get_tag_detail(
-        self, id_: Optional[int] = None
-    ) -> Union[list[dict[str, Any]], dict[str, Any]]:
-        """Returns all tags or specific tag by database id with detailed information
+    # DELETE /series/{id}
+    def del_series(
+        self, id_: int, delete_files: bool = False
+    ) -> Union[Response, JsonObject, dict[Any, Any]]:
+        """Delete the series with the given ID
 
         Args:
-            id_ (Optional[int], optional): Database id for tag. Defaults to None.
+            id_ (int): Database ID for series
+            delete_files (bool, optional): If true series folder and files will be deleted. Defaults to False.
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            dict: Blank dictionary
         """
-        path = f"tag/detail/{id_}" if id_ else "tag/detail"
-        return self.assert_return(path, self.ver_uri, list if id_ is None else dict)
+        # File deletion does not work
+        params = {"deleteFiles": delete_files}
+        return self._delete(f"series/{id_}", self.ver_uri, params=params)
 
-    # POST /tag
-    def create_tag(self, label: str) -> dict[str, Any]:
-        """Adds a new tag
+    # GET /series/lookup
+    def lookup_series(
+        self, term: Optional[str] = None, id_: Optional[int] = None
+    ) -> JsonArray:
+        """Searches for new shows on TheTVDB.com utilizing sonarr.tv's caching and augmentation proxy.
 
         Args:
-            label (str): Tag name / label
+            term (Optional[str], optional): Series' Name
+            id_ (Optional[int], optional): TVDB ID for series
 
         Returns:
-            dict[str, Any]: Dictionary of new record
+            JsonArray: List of dictionaries with items
         """
-        data = {"label": label}
-        return self._post("tag", self.ver_uri, data=data)
+        if term is None and id_ is None:
+            raise PyarrMissingArgument("A term or TVDB id must be included")
+
+        return self._get("series/lookup", self.ver_uri, {"term": term or f"tvdb:{id_}"})
 
-    # PUT /tag/{id}
-    def upd_tag(self, id_: int, label: str) -> dict[str, Any]:
-        """Update an existing tag
+    # GET /series/lookup
+    def lookup_series_by_tvdb_id(self, id_: int) -> JsonArray:
+        """Searches for new shows on TheTVDB.com utilizing sonarr.tv's caching and augmentation proxy.
 
         Note:
-            You should perform a get_tag() and submit the full body with changes
+            This method is deprecated and will be removed in a future release. Please use lookup_series()
 
         Args:
-            id_ (int): Database id of tag
-            label (str): tag name / label
+            id_ (int): TVDB ID
 
         Returns:
-            dict[str, Any]: Dictionary of updated items
+            JsonArray: List of dictionaries with items
         """
-        data = {"id": id_, "label": label}
-        return self._put(f"tag/{id_}", self.ver_uri, data=data)
+        warn(
+            "This method is deprecated and will be removed in a future release. Please use lookup_series()",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        params = {"term": f"tvdb:{id_}"}
+        return self._get("series/lookup", self.ver_uri, params)
 
-    # DELETE /tag/{id}
-    def del_tag(self, id_: int) -> Union[Response, dict[str, Any], dict[Any, Any]]:
-        """Delete the tag with the given ID
+    # GET /history
+    # Overrides base get history for ID
+    def get_history(
+        self,
+        page: Optional[int] = None,
+        page_size: Optional[int] = None,
+        sort_key: Optional[PyarrHistorySortKey] = None,
+        sort_dir: Optional[PyarrSortDirection] = None,
+        id_: Optional[int] = None,
+    ) -> JsonObject:
+        """Gets history (grabs/failures/completed)
 
         Args:
-            id_ (int): Database id of tag
+            page (Optional[int], optional): Page number to return. Defaults to None.
+            page_size (Optional[int], optional): Number of items per page. Defaults to None.
+            sort_key (Optional[PyarrHistorySortKey], optional): Field to sort by. Defaults to None.
+            sort_dir (Optional[PyarrSortDirection], optional): Direction to sort the items. Defaults to None.
+            id_ (Optional[int], optional): Filter to a specific episode ID. Defaults to None.
 
         Returns:
-            Response: HTTP Response
+           JsonObject: Dictionary with items
         """
-        return self._delete(f"tag/{id_}", self.ver_uri)
+        params: dict[str, Union[int, PyarrHistorySortKey, PyarrSortDirection]] = {}
 
-    # DOWNLOAD CLIENT
+        if page:
+            params["page"] = page
 
-    # GET /downloadclient/{id}
-    def get_download_client(self, id_: Optional[int] = None) -> list[dict[str, Any]]:
-        """Get a list of all the download clients or a single client by its database id
+        if page_size:
+            params["pageSize"] = page_size
 
-        Args:
-            id_ (Optional[int], optional): Download client database id. Defaults to None.
+        if sort_key and sort_dir:
+            params["sortKey"] = sort_key
+            params["sortDirection"] = sort_dir
+        elif sort_key or sort_dir:
+            raise PyarrMissingArgument("sort_key and sort_dir  must be used together")
 
-        Returns:
-            list[dict[str, Any]]: List of dictionaries with items
-        """
-        path = f"downloadclient/{id_}" if id_ else "downloadclient"
-        return self.assert_return(path, self.ver_uri, list)
+        if id_:
+            params["episodeId"] = id_
 
-    # GET /downloadclient/schema
-    def get_download_client_schema(
-        self, implementation_: Optional[str] = None
-    ) -> list[dict[str, Any]]:
-        """Gets the schemas for the different download Clients
+        return self._get("history", self.ver_uri, params)
+
+    # GET /languageprofile/{id}
+    def get_language_profile(
+        self, id_: Optional[int] = None
+    ) -> Union[JsonArray, dict[Any, Any]]:
+        """Gets all language profiles or specific one with id
 
         Args:
-            implementation_ (Optional[str], optional): Client implementation name. Defaults to None.
+            id_ (Optional[int], optional): Language profile id from database. Defaults to None.
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            Union[JsonArray, dict[Any, Any]]: List of dictionaries with items
         """
-        response = self.assert_return("downloadclient/schema", self.ver_uri, list)
-        if implementation_:
-            return [
-                schema
-                for schema in response
-                if schema["implementation"] == implementation_
-            ]
 
-        return response
+        path = f"languageprofile{f'/{id_}' if id_ else ''}"
+        return self._get(path, self.ver_uri)
 
-    # POST /downloadclient/
-    def add_download_client(self, data: dict[str, Any]) -> dict[str, Any]:
-        """Add a download client based on the schema information supplied
+    # PUT /languageprofile/{id}
+    def upd_language_profile(self, id_: int, data: JsonObject) -> JsonObject:
+        """Update the language profile data
 
         Note:
-            Recommended to be used in conjunction with get_download_client_schema()
+            To be used in conjunction with get_language_profile()
 
         Args:
-            data (dict[str, Any]): dictionary with download client schema and settings
+            id_ (int): Profile ID to Update
+            data (JsonObject): All parameters to update
 
         Returns:
-            dict[str, Any]: dictionary of added item
+            JsonObject: Dictionary of updated record
         """
-        return self._post("downloadclient", self.ver_uri, data=data)
-
-    # PUT /downloadclient/{id}
-    def upd_download_client(self, id_: int, data: dict[str, Any]) -> dict[str, Any]:
-        """Edit a downloadclient by database id
-
-        Args:
-            id_ (int): Download client database id
-            data (dict[str, Any]): data to be updated within download client
 
-        Returns:
-            dict[str, Any]: dictionary of updated item
-        """
-        return self._put(f"downloadclient/{id_}", self.ver_uri, data=data)
+        return self._put(f"languageprofile/{id_}", self.ver_uri, data=data)
 
-    # DELETE /downloadclient/{id}
-    def del_download_client(
+    # DELETE /languageprofile
+    def del_language_profile(
         self, id_: int
-    ) -> Union[Response, dict[str, Any], dict[Any, Any]]:
-        """Delete a download client by database id
+    ) -> Union[Response, JsonObject, dict[Any, Any]]:
+        """Removes a specific language profile from the blocklist
 
         Args:
-            id_ (int): download client database id
+            id_ (int): Profile ID from database
 
         Returns:
             Response: HTTP Response
         """
-        return self._delete(f"downloadclient/{id_}", self.ver_uri)
-
-    # IMPORT LIST
+        return self._delete(f"languageprofile/{id_}", self.ver_uri)
 
-    # GET /importlist
-    def get_import_list(self, id_: Optional[int] = None) -> list[dict[str, Any]]:
-        """Query for all lists or a single list by its database id
+    # GET /languageprofile/schema/{id}
+    def get_language_profile_schema(
+        self, id_: Optional[int] = None
+    ) -> Union[JsonArray, dict[Any, Any]]:
+        """Gets all language profile schemas or specific one with id
 
         Args:
-            id_ (Optional[int], optional): Import list database id. Defaults to None.
+            id_ (Optional[int], optional): Language profile schema id from database. Defaults to None.
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            Union[JsonArray, dict[Any, Any]]: List of dictionaries with items
         """
-        path = f"importlist/{id_}" if id_ else "importlist"
-        return self.assert_return(path, self.ver_uri, list)
 
-    # POST /importlist/
-    def add_import_list(self) -> Any:
-        """This is not implemented yet
+        path = f"languageprofile/schema{f'/{id_}' if id_ else ''}"
+        return self._get(path, self.ver_uri)
 
-        Raises:
-            NotImplementedError: Error
-        """
-        raise NotImplementedError()
-
-    # PUT /importlist/{id}
-    def upd_import_list(self, id_: int, data: dict[str, Any]) -> dict[str, Any]:
-        """Edit an importlist
+    # POST /qualityprofile
+    def add_quality_profile(
+        self, name: str, upgrades_allowed: bool, cutoff: int, items: list
+    ) -> JsonObject:
+        """Add new quality profile
 
         Args:
-            id_ (int): Import list database id
-            data (dict[str, Any]): data to be updated within the import list
+            name (str): Name of the profile
+            upgrades_allowed (bool): Are upgrades in quality allowed?
+            cutoff (int): ID of quality definition to cutoff at. Must be an allowed definition ID.
+            items (list): Add a list of items (from `get_quality_definition()`)
 
         Returns:
-            dict[str, Any]: Dictionary of updated data
+            JsonObject: An object containing the profile
         """
-        return self._put(f"importlist/{id_}", self.ver_uri, data=data)
-
-    # DELETE /importlist/{id}
-    def del_import_list(
-        self, id_: int
-    ) -> Union[Response, dict[str, Any], dict[Any, Any]]:
-        """Delete an import list
+        data = {
+            "name": name,
+            "upgradeAllowed": upgrades_allowed,
+            "cutoff": cutoff,
+            "items": items,
+        }
+        return self._post("qualityprofile", self.ver_uri, data=data)
 
-        Args:
-            id_ (int): Import list database id
+    # GET /manualimport
+    def get_manual_import(
+        self,
+        folder: str,
+        download_id: Optional[str] = None,
+        series_id: Optional[int] = None,
+        filter_existing_files: Optional[bool] = None,
+        replace_existing_files: Optional[bool] = None,
+    ) -> JsonArray:
+        """Gets a manual import list
+
+        Args:
+            downloadId (str): Download IDs
+            series_id (int, optional): Series Database ID. Defaults to None.
+            folder (Optional[str], optional): folder name. Defaults to None.
+            filterExistingFiles (bool, optional): filter files. Defaults to True.
+            replaceExistingFiles (bool, optional): replace files. Defaults to True.
+
+        Returns:
+            JsonArray: List of dictionaries with items
+        """
+        params: dict[str, Union[str, int, bool]] = {"folder": folder}
+        if download_id:
+            params["downloadId"] = download_id
+        if series_id:
+            params["seriesId"] = series_id
+        if filter_existing_files:
+            params["filterExistingFiles"] = filter_existing_files
+        if replace_existing_files:
+            params["replaceExistingFiles"] = replace_existing_files
+
+        return self._get("manualimport", self.ver_uri, params=params)
+
+    # PUT /manualimport
+    def upd_manual_import(self, data: JsonObject) -> JsonObject:
+        """Update a manual import
 
-        Returns:
-            Response: HTTP Response
-        """
-        return self._delete(f"importlist/{id_}", self.ver_uri)
+        Note:
+            To be used in conjunction with get_manual_import()
 
-    # GET /config/downloadclient
-    def get_config_download_client(self) -> dict[str, Any]:
-        """Gets download client page configuration
+        Args:
+            data (JsonObject): Data containing changes
 
         Returns:
-            dict[str, Any]: Dictionary of configuration
-        """
-        return self.assert_return("config/downloadclient", self.ver_uri, dict)
-
-    # POST /notifications
-    def add_notifications(self) -> Any:
-        """This is not implemented yet
-
-        Raises:
-            NotImplementedError: Error
+            JsonObject: Dictionary of updated record
         """
-        raise NotImplementedError()
+        return self._put("manualimport", self.ver_uri, data=data)
```

### Comparing `pyarr-4.1.0/pyarr/lidarr.py` & `pyarr-5.0.0/pyarr/lidarr.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Any, Optional, Union
 
 from requests import Response
 
+from pyarr.types import JsonArray, JsonObject
+
 from .base import BaseArrAPI
-from .const import PAGE, PAGE_SIZE
-from .exceptions import PyarrError, PyarrMissingProfile
+from .exceptions import PyarrMissingArgument, PyarrMissingProfile
 from .models.common import PyarrSortDirection
-from .models.lidarr import LidarrArtistMonitor, LidarrSortKeys
+from .models.lidarr import LidarrArtistMonitor, LidarrCommand, LidarrSortKey
 
 
 class LidarrAPI(BaseArrAPI):
     """API wrapper for Lidarr endpoints.
 
     Args:
         RequestAPI (:obj:`str`): provides connection to API endpoint
@@ -28,96 +29,125 @@
         super().__init__(host_url, api_key, ver_uri)
 
     # POST /rootfolder
     def add_root_folder(
         self,
         name: str,
         path: str,
-        defaultTags: list[int],
-        qualityProfile: int,
-        metadataProfile: int,
-    ) -> dict[str, Any]:
-        """Adds a root folder
+        default_quality_profile_id: int,
+        default_metadata_profile_id: int,
+        default_tags: list[int] = None,
+    ) -> JsonObject:
+        """Add a new location to store files
 
         Args:
             name (str): Name for this root folder
             path (str): Location the files should be stored
-            defaultTags (list[int]): List of default tag IDs
-            qualityProfile (int): Default quality profile ID
-            metadataProfile (int): Default metadata profile ID
+            default_quality_profile_id (int): Default quality profile ID
+            default_metadata_profile_id (int): Default metadata profile ID
+            default_tags (list[int]): List of default tag IDs
 
         Returns:
-            dict[str, Any]: Dictonary with added record
+            JsonObject: Dictonary with added record
         """
         folder_json = {
-            "defaultTags": defaultTags,
-            "defaultQualityProfileId": qualityProfile,
-            "defaultMetadataProfileId": metadataProfile,
+            "defaultTags": default_tags or [],
+            "defaultQualityProfileId": default_quality_profile_id,
+            "defaultMetadataProfileId": default_metadata_profile_id,
             "name": name,
             "path": path,
         }
 
         return self._post("rootfolder", self.ver_uri, data=folder_json)
 
-    def lookup(self, term: str) -> list[dict[str, Any]]:
+    def lookup(self, term: str) -> JsonArray:
         """Search for an artist / album / song
 
         Args:
-            term (str): Search term
+            term (str): Search term, can also use MusicBrainz IDs::
+
+                lidarr.lookup(term="lidarr:cc197bad-dc9c-440d-a5b5-d52ba2e14234")
+
+        Returns:
+            JsonArray: List of dictionaries with items
+        """
+        return self._get("search", self.ver_uri, params={"term": term})
+
+    def lookup_artist(self, term: str) -> JsonArray:
+        """Search for an Artist to add to the database
+
+        Args:
+            term (str): Search term, can also use MusicBrainz IDs::
+
+                lidarr.lookup(term="lidarr:cc197bad-dc9c-440d-a5b5-d52ba2e14234")
+
+        Returns:
+            JsonArray: List of dictionaries with items
+        """
+
+        return self._get("artist/lookup", self.ver_uri, params={"term": term})
+
+    def lookup_album(self, term: str) -> JsonArray:
+        """Search for an Album to add to the database
+
+        Args:
+            term (str): Search term, can also use MusicBrainz IDs::
+
+                lidarr.lookup(term="lidarr:1dc4c347-a1db-32aa-b14f-bc9cc507b843")
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            JsonArray: List of dictionaries with items
         """
-        return self.assert_return("search", self.ver_uri, list, params={"term": term})
+        return self._get("album/lookup", self.ver_uri, params={"term": term})
 
-    def get_artist(self, id_: Union[str, int, None] = None) -> list[dict[str, Any]]:
+    def get_artist(self, id_: Optional[Union[str, int]] = None) -> JsonArray:
         """Get an artist by ID or get all artists
 
         Args:
-            id_ (Union[str, int, None], optional): Artist ID. Defaults to None.
+            id_ (Optional[Union[str, int]], optional): Artist ID. Defaults to None.
+
+        Note:
+            Include a string to search by MusicBrainz id.
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            JsonArray: List of dictionaries with items
         """
 
         _path = "" if isinstance(id_, str) or id_ is None else f"/{id_}"
-        return self.assert_return(
+        return self._get(
             f"artist{_path}",
             self.ver_uri,
-            list,
             params={"mbId": id_} if isinstance(id_, str) else None,
         )
 
-    def _artist_json(
+    def add_artist(
         self,
-        term: str,
+        artist: JsonObject,
         root_dir: str,
         quality_profile_id: Optional[int] = None,
         metadata_profile_id: Optional[int] = None,
         monitored: bool = True,
-        artist_monitor: LidarrArtistMonitor = LidarrArtistMonitor.ALL_ALBUMS,
+        artist_monitor: LidarrArtistMonitor = "all",
         artist_search_for_missing_albums: bool = False,
-    ) -> dict[str, Any]:
-        """Method to help build the JSON for adding an artist
+    ) -> JsonObject:
+        """Adds an artist from the lookup result
 
         Args:
-            term (str): Search term for artist
-            root_dir (str): Root directory for music
-            quality_profile_id (Optional[int], optional): Quality profile Id. Defaults to None.
+            artist (JsonObject): Artist record from lookup()
+            root_dir (str): Directory for music to be stored
+            quality_profile_id (Optional[int], optional): Quality profile ID. Defaults to None.
             metadata_profile_id (Optional[int], optional): Metadata profile ID. Defaults to None.
-            monitored (bool, optional): Should this be monitored. Defaults to True.
-            artist_monitor (LidarrArtistMonitor, optional): Should the artist be monitored. Defaults to LidarrArtistMonitor.ALL_ALBUMS.
-            artist_search_for_missing_albums (bool, optional): Should we search for missing albums. Defaults to False.
-
-        Raises:
-            PyarrMissingProfile: Raised when quality or metadata profile are missing
+            monitored (bool, optional): Monitor the artist. Defaults to True.
+            artist_monitor (LidarrArtistMonitor, optional): Monitor the artist. Defaults to "all".
+            artist_search_for_missing_albums (bool, optional): Search for missing albums by this artist. Defaults to False.
 
         Returns:
-            dict[str, Any]: Dictionary with artist information
+            JsonObject: Dictonary with added record
         """
+
         if quality_profile_id is None:
             try:
                 quality_profile_id = self.get_quality_profile()[0]["id"]
             except IndexError as exception:
                 raise PyarrMissingProfile(
                     "There is no Quality Profile setup"
                 ) from exception
@@ -125,157 +155,106 @@
             try:
                 metadata_profile_id = self.get_metadata_profile()[0]["id"]
             except IndexError as exception:
                 raise PyarrMissingProfile(
                     "There is no Metadata Profile setup"
                 ) from exception
 
-        artist = self.lookup_artist(term)[0]
         artist["id"] = 0
         artist["metadataProfileId"] = metadata_profile_id
         artist["qualityProfileId"] = quality_profile_id
         artist["rootFolderPath"] = root_dir
         artist["addOptions"] = {
             "monitor": artist_monitor,
             "searchForMissingAlbums": artist_search_for_missing_albums,
         }
         artist["monitored"] = monitored
 
-        return artist
-
-    def add_artist(
-        self,
-        search_term: str,
-        root_dir: str,
-        quality_profile_id: Optional[int] = None,
-        metadata_profile_id: Optional[int] = None,
-        monitored: bool = True,
-        artist_monitor: LidarrArtistMonitor = LidarrArtistMonitor.ALL_ALBUMS,
-        artist_search_for_missing_albums: bool = False,
-    ) -> dict[str, Any]:
-        """Adds an artist based on a search term, must be artist name or album/single
-        by lidarr guid
-
-        Args:
-            search_term (str): Artist name or album/single
-            root_dir (str): Directory for music to be stored
-            quality_profile_id (Optional[int], optional): Quality profile ID. Defaults to None.
-            metadata_profile_id (Optional[int], optional): Metadata profile ID. Defaults to None.
-            monitored (bool, optional): Monitor the artist. Defaults to True.
-            artist_monitor (LidarrArtistMonitor, optional): Monitor the artist. Defaults to LidarrArtistMonitor.ALL_ALBUMS.
-            artist_search_for_missing_albums (bool, optional): Search for missing albums by this artist. Defaults to False.
-
-        Returns:
-            dict[str, Any]: Dictonary with added record
-        """
+        return self._post("artist", self.ver_uri, data=artist)
 
-        artist_json = self._artist_json(
-            search_term,
-            root_dir,
-            quality_profile_id,
-            metadata_profile_id,
-            monitored,
-            artist_monitor,
-            artist_search_for_missing_albums,
-        )
-        return self._post("artist", self.ver_uri, data=artist_json)
-
-    def upd_artist(self, data: dict[str, Any]) -> dict[str, Any]:
+    def upd_artist(self, data: JsonObject) -> JsonObject:
         """Update an existing artist
 
+        note:
+
         Args:
-            data (dict[str, Any]): Data for the artist record
+            data (JsonObject): Dictionary containing an object obtained from get_artist()
 
         Returns:
-            dict[str, Any]: Dictionary of updated record
+            JsonObject: Dictionary of updated record
         """
         return self._put("artist", self.ver_uri, data=data)
 
-    def delete_artist(
-        self, id_: int
-    ) -> Union[Response, dict[str, Any], dict[Any, Any]]:
+    def delete_artist(self, id_: int) -> Union[Response, JsonObject, dict[Any, Any]]:
         """Delete an artist with the provided ID
 
         Args:
             id_ (int): Artist ID to be deleted
 
         Returns:
-            Response: 200 / 401
+            Response: HTTP Response
         """
         return self._delete(f"artist/{id_}", self.ver_uri)
 
-    def lookup_artist(self, term: str) -> list[dict[str, Any]]:
-        """Search for an Artist to add to the database
-
-        Args:
-            term (str): Search term to use for lookup
-
-        Returns:
-            list[dict[str, Any]]: List of dictionaries with items
-        """
-
-        return self.assert_return(
-            "artist/lookup", self.ver_uri, list, params={"term": term}
-        )
-
     def get_album(
         self,
         albumIds: Union[int, list[int], None] = None,
         artistId: Optional[int] = None,
         foreignAlbumId: Optional[int] = None,
         allArtistAlbums: bool = False,
-    ) -> list[dict[str, Any]]:
+    ) -> JsonArray:
         """Get a specific album by ID, or get all albums
 
         Args:
             albumIds (Union[int, list[int], None], optional): Database album IDs. Defaults to None.
             artistId (Optional[int], optional): Database artist IDs. Defaults to None.
             foreignAlbumId (Optional[int], optional): Foreign album id. Defaults to None.
             allArtistAlbums (bool, optional): Get all artists albums. Defaults to False.
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            JsonArray: List of dictionaries with items
         """
-        params: dict[str, Any] = {"includeAllArtistAlbums": str(allArtistAlbums)}
+        params: dict[str, Any] = {"includeAllArtistAlbums": allArtistAlbums}
 
         if isinstance(albumIds, list):
             params["albumids"] = albumIds
         if artistId is not None:
             params["artistId"] = artistId
         if foreignAlbumId is not None:
             params["foreignAlbumId"] = foreignAlbumId
         _path = "" if isinstance(albumIds, list) or albumIds is None else f"/{albumIds}"
-        return self.assert_return(f"album{_path}", self.ver_uri, list, params=params)
+        return self._get(
+            f"album{_path}",
+            self.ver_uri,
+            params=params,
+        )
 
-    def _album_json(
+    def add_album(
         self,
-        term: str,
+        album: JsonObject,
         root_dir: str,
         quality_profile_id: Optional[int] = None,
         metadata_profile_id: Optional[int] = None,
         monitored: bool = True,
-        artist_monitor: LidarrArtistMonitor = LidarrArtistMonitor.ALL_ALBUMS,
+        artist_monitor: LidarrArtistMonitor = "all",
         artist_search_for_missing_albums: bool = False,
-    ) -> dict[str, Any]:
-        """Method to help build the JSON for adding an album
+    ) -> JsonObject:
+        """Adds an album to Lidarr
 
         Args:
-            term (str): Search term for the album
-            root_dir (str): Director to store the album.
+            album (JsonObject): Album record from `lookup()`
+            root_dir (str): Location to store music
             quality_profile_id (Optional[int], optional): Quality profile ID. Defaults to None.
             metadata_profile_id (Optional[int], optional): Metadata profile ID. Defaults to None.
-            monitored (bool, optional): Monitor the albums. Defaults to True.
-            artist_monitor (LidarrArtistMonitor, optional): Monitor the artist. Defaults to LidarrArtistMonitor.ALL_ALBUMS.
-            artist_search_for_missing_albums (bool, optional): Search for missing albums by the artist. Defaults to False.
-
-        Raises:
-            PyarrMissingProfile: Error if there are no quality or metadata profiles that match
+            monitored (bool, optional): Should the album be monitored. Defaults to True.
+            artist_monitor (LidarrArtistMonitor, optional): What level to monitor the artist. Defaults to "all".
+            artist_search_for_missing_albums (bool, optional): Search for any missing albums by this artist. Defaults to False.
 
         Returns:
-            dict[str, Any]: Dictionary with album data
+            JsonObject: Dictionary with added record
         """
         if quality_profile_id is None:
             try:
                 quality_profile_id = self.get_quality_profile()[0]["id"]
             except IndexError as exception:
                 raise PyarrMissingProfile(
                     "There is no Quality Profile setup"
@@ -284,257 +263,226 @@
             try:
                 metadata_profile_id = self.get_metadata_profile()[0]["id"]
             except IndexError as exception:
                 raise PyarrMissingProfile(
                     "There is no Metadata Profile setup"
                 ) from exception
 
-        artist = self.lookup_artist(term)[0]
-        artist["id"] = 0
-        artist["metadataProfileId"] = metadata_profile_id
-        artist["qualityProfileId"] = quality_profile_id
-        artist["rootFolderPath"] = root_dir
-        artist["addOptions"] = {
+        album["id"] = 0
+        album["artist"]["metadataProfileId"] = metadata_profile_id
+        album["artist"]["qualityProfileId"] = quality_profile_id
+        album["artist"]["rootFolderPath"] = root_dir
+        album["artist"]["addOptions"] = {
             "monitor": artist_monitor,
             "searchForMissingAlbums": artist_search_for_missing_albums,
         }
-        artist["monitored"] = monitored
-
-        return artist
-
-    def add_album(
-        self,
-        search_term: str,
-        root_dir: str,
-        quality_profile_id: Optional[int] = None,
-        metadata_profile_id: Optional[int] = None,
-        monitored: bool = True,
-        artist_monitor: LidarrArtistMonitor = LidarrArtistMonitor.ALL_ALBUMS,
-        artist_search_for_missing_albums: bool = False,
-    ) -> dict[str, Any]:
-        """Adds an album to Lidarr
-
-        Args:
-            search_term (str): Name of the album to search for
-            root_dir (str): Location to store music
-            quality_profile_id (Optional[int], optional): Quality profile ID. Defaults to None.
-            metadata_profile_id (Optional[int], optional): Metadata profile ID. Defaults to None.
-            monitored (bool, optional): Should the album be monitored. Defaults to True.
-            artist_monitor (LidarrArtistMonitor, optional): What level to monitor the artist. Defaults to LidarrArtistMonitor.ALL_ALBUMS.
-            artist_search_for_missing_albums (bool, optional): Search for any missing albums by this artist. Defaults to False.
+        album["monitored"] = monitored
+        return self._post("album", self.ver_uri, data=album)
 
-        Returns:
-            dict[str, Any]: Dictionary with added record
-        """
-        album_json = self._album_json(
-            search_term,
-            root_dir,
-            quality_profile_id,
-            metadata_profile_id,
-            monitored,
-            artist_monitor,
-            artist_search_for_missing_albums,
-        )
-        return self._post("album", self.ver_uri, data=album_json)
-
-    def upd_album(self, data: dict[str, Any]) -> dict[str, Any]:
+    def upd_album(self, data: JsonObject) -> JsonObject:
         """Update an album
 
         Args:
-            data (dict[str, Any]): data to update albums
+            data (JsonObject): data to update albums
 
         Note:
             To be used in conjunction with get_album()
 
         Returns:
-            dict[str, Any]: Dictionary of updated record
+            JsonObject: Dictionary of updated record
         """
         return self._put("album", self.ver_uri, data=data)
 
-    def delete_album(self, id_: int) -> Union[Response, dict[str, Any], dict[Any, Any]]:
+    def delete_album(self, id_: int) -> Union[Response, JsonObject, dict[Any, Any]]:
         """Delete an album with the provided ID
 
         Args:
             id_ (int): Album ID to be deleted
 
         Returns:
             Response: 200 / 401
         """
         return self._delete(f"album/{id_}", self.ver_uri)
 
-    def lookup_album(self, term: str) -> list[dict[str, Any]]:
-        """Search for an Album to add to the database
+    # POST /command
+    def post_command(self, name: LidarrCommand) -> JsonObject:
+        """Send a command to Lidarr
 
         Args:
-            term (str): Search term to use for lookup
+            name (LidarrCommand): Command to be run against Lidarr
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            JsonObject: dictionary of executed command information
         """
-        return self.assert_return(
-            "album/lookup", self.ver_uri, list, params={"term": term}
-        )
-
-    # POST /command
-    def post_command(self) -> Any:
-        """This function is not implemented
-
-        Raises:
-            NotImplementedError: Error
-        """
-        raise NotImplementedError("This feature is not implemented yet.")
+        return self._post("command", self.ver_uri, data={"name": name})
 
     # GET /wanted
     def get_wanted(
         self,
         id_: Optional[int] = None,
-        sort_key: LidarrSortKeys = LidarrSortKeys.TITLE,
-        page: int = PAGE,
-        page_size: int = PAGE_SIZE,
-        sort_dir: PyarrSortDirection = PyarrSortDirection.ASC,
+        page: Optional[int] = None,
+        page_size: Optional[int] = None,
+        sort_key: Optional[LidarrSortKey] = None,
+        sort_dir: Optional[PyarrSortDirection] = None,
         missing: bool = True,
-    ) -> dict[str, Any]:
+    ) -> JsonObject:
         """Get wanted albums that are missing or not meeting cutoff
 
         Args:
             id_ (int | None, optional): Specific album ID to return. Defaults to None.
-            sort_key (LidarrSortKeys, optional): id, title, ratings, or quality". (Others do not apply). Defaults to LidarrSortKeys.TITLE.
-            page (int, optional): Page number to return. Defaults to 1.
-            page_size (int, optional): Number of items per page. Defaults to 10.
-            sort_dir (PyarrSortDirection, optional): Sort ascending or descending. Defaults to PyarrSortDirection.ASC.
+            page (Optional[int], optional): Page number to return. Defaults to None.
+            page_size (Optional[int], optional): Number of items per page. Defaults to None.
+            sort_key (Optional[LidarrSortKey], optional): Column to sort by. Defaults to None.
+            sort_dir (Optional[PyarrSortDirection], optional): Direction to sort the items. Defaults to None.
             missing (bool, optional): Search for missing (True) or cutoff not met (False). Defaults to True.
 
         Returns:
-            dict[str, Any]: List of dictionaries with items
+            JsonObject: List of dictionaries with items
         """
-        params = {
-            "sortKey": sort_key.value,
-            "page": page,
-            "pageSize": page_size,
-        }
+        params: dict[str, Union[int, LidarrSortKey, PyarrSortDirection, bool]] = {}
+        if page:
+            params["page"] = page
+        if page_size:
+            params["pageSize"] = page_size
+        if sort_key and sort_dir:
+            params["sortKey"] = sort_key
+            params["sortDirection"] = sort_dir
+        elif sort_key or sort_dir:
+            raise PyarrMissingArgument("sort_key and sort_dir  must be used together")
+
         _path = "missing" if missing else "cutoff"
-        return self.assert_return(
+        return self._get(
             f"wanted/{_path}{'' if id_ is None else f'/{id_}'}",
             self.ver_uri,
-            dict,
             params=params,
         )
 
     # GET /parse
     # TODO: Confirm response type
-    def get_parse(self, title: str) -> list[dict[str, Any]]:
+    def get_parse(self, title: str) -> JsonArray:
         """Return the music / artist with a matching filename
 
         Args:
             title (str): file
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            JsonArray: List of dictionaries with items
         """
-        return self.assert_return("parse", self.ver_uri, list, params={"title": title})
+        return self._get("parse", self.ver_uri, params={"title": title})
 
     # GET /track
     def get_tracks(
         self,
         artistId: Optional[int] = None,
         albumId: Optional[int] = None,
         albumReleaseId: Optional[int] = None,
-        trackIds: Union[int, list[int], None] = None,
-    ) -> list[dict[str, Any]]:
+        trackIds: Optional[Union[int, list[int]]] = None,
+    ) -> JsonArray:
         """Get tracks based on provided IDs
 
         Args:
             artistId (Optional[int], optional): Artist ID. Defaults to None.
             albumId (Optional[int], optional): Album ID. Defaults to None.
             albumReleaseId (Optional[int], optional): Album Release ID. Defaults to None.
-            trackIds (Union[int, list[int], None], optional): Track IDs. Defaults to None.
+            trackIds (Optional[Union[int, list[int]]], optional): Track IDs. Defaults to None.
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            JsonArray: List of dictionaries with items
         """
         params: dict[str, Any] = {}
         if artistId is not None:
             params["artistId"] = artistId
         if albumId is not None:
             params["albumId"] = albumId
         if albumReleaseId is not None:
             params["albumReleaseId"] = albumReleaseId
         if isinstance(trackIds, list):
             params["trackIds"] = trackIds
-        return self.assert_return(
+
+        if (
+            artistId is None
+            and albumId is None
+            and albumReleaseId is None
+            and trackIds is None
+        ):
+            raise PyarrMissingArgument(
+                "One of artistId, albumId, albumReleaseId or trackIds must be provided"
+            )
+
+        return self._get(
             f"track{f'/{trackIds}' if isinstance(trackIds, int) else ''}",
             self.ver_uri,
-            list,
             params=params,
         )
 
     # GET /trackfile/
     def get_track_file(
         self,
         artistId: Optional[int] = None,
         albumId: Optional[int] = None,
         trackFileIds: Union[int, list[int], None] = None,
-        unmapped: bool = False,
-    ) -> list[dict[str, Any]]:
+        unmapped: Optional[bool] = None,
+    ) -> JsonArray:
         """Get track files based on IDs, or get all unmapped files
 
         Args:
             artistId (Optional[int], optional): Artist database ID. Defaults to None.
             albumId (Optional[int], optional): Album database ID. Defaults to None.
             trackFileIds (Union[int, list[int], None], optional): Specific file IDs. Defaults to None.
-            unmapped (bool, optional): Get all unmapped filterExistingFiles. Defaults to False.
+            unmapped (Optional[bool], optional): Get all unmapped filterExistingFiles. Defaults to None.
 
         Raises:
             PyarrError: Where no IDs or unmapped params provided
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            JsonArray: List of dictionaries with items
         """
         if (
             artistId is None
             and albumId is None
             and trackFileIds is None
-            and not unmapped
+            and unmapped is None
         ):
-            raise PyarrError(
-                "BadRequest: artistId, albumId, trackFileIds or unmapped must be provided"
+            raise PyarrMissingArgument(
+                "artistId, albumId, trackFileIds or unmapped must be provided"
             )
-        params: dict[str, Any] = {"unmapped": str(unmapped)}
+        params: dict[str, Any] = {}
         if artistId is not None:
             params["artistId"] = artistId
         if albumId is not None:
             params["albumId"] = albumId
         if isinstance(trackFileIds, list):
             params["trackFileIds"] = trackFileIds
-        return self.assert_return(
+        if unmapped is not None:
+            params["unmapped"] = unmapped
+        return self._get(
             f"trackfile{f'/{trackFileIds}' if isinstance(trackFileIds, int) else ''}",
             self.ver_uri,
-            list,
             params=params,
         )
 
     # PUT /trackfile/{id_}
-    def upd_track_file(self, data: dict[str, Any]) -> dict[str, Any]:
+    def upd_track_file(self, data: JsonObject) -> JsonObject:
         """Update an existing track file
 
         Note:
             To be used in conjunction with get_track_file()
 
         Args:
-            data (dict[str, Any]): Updated data for track files
+            data (JsonObject): Updated data for track files
 
         Returns:
-            dict[str, Any]: Dictionary of updated record
+            JsonObject: Dictionary of updated record
         """
         return self._put("trackfile", self.ver_uri, data=data)
 
     # DEL /trackfile/{ids_}
     def delete_track_file(
         self, ids_: Union[int, list[int]]
-    ) -> Union[Response, dict[str, Any], dict[Any, Any]]:
+    ) -> Union[Response, JsonObject, dict[Any, Any]]:
         """Delete track files. Use integer for one file or list for mass deletion.
 
         Args:
             ids_ (Union[int, list[int]]): Single ID or list of IDs for files to delete
 
         Returns:
             Response: 200 / 401
@@ -542,241 +490,270 @@
         return self._delete(
             f"trackfile/{'bulk' if isinstance(ids_, list) else f'{ids_}'}",
             self.ver_uri,
             data={"trackFileIds": ids_} if isinstance(ids_, list) else None,
         )
 
     # GET /metadataprofile/{id}
-    def get_metadata_profile(self, id_: Optional[int] = None) -> list[dict[str, Any]]:
-        """Gets all metadata profiles or specific one with id_
+    def get_metadata_profile(self, id_: Optional[int] = None) -> JsonArray:
+        """Gets all metadata profiles or specific one with id
 
         Args:
             id_ (Optional[int], optional): Metadata profile id from database. Defaults to None.
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            JsonArray: List of dictionaries with items
         """
-        _path = f"/{id_}" if id_ else ""
-        response = self._get(f"metadataprofile{_path}", self.ver_uri)
-        assert isinstance(response, list)
-        return response
-
-    # POST /metadataprofile
-    def add_metadata_profile(self) -> Any:
-        """This function is not implemented
+        return self._get(
+            f"metadataprofile{f'/{id_}' if id_ else ''}",
+            self.ver_uri,
+        )
 
-        Raises:
-            NotImplementedError: Error
-        """
-        raise NotImplementedError("This feature is not implemented yet.")
+    # TODO: POST /metadataprofile
 
     # PUT /metadataprofile
-    def upd_metadata_profile(self, data: dict[str, Any]) -> dict[str, Any]:
+    def upd_metadata_profile(self, data: JsonObject) -> JsonObject:
         """Update a metadata profile
 
         Args:
-            data (dict[str, Any]): Data containing metadata profile and changes
+            data (JsonObject): Data containing metadata profile and changes
 
         Returns:
-            dict[str, Any]: Dictionary of updated record
+            JsonObject: Dictionary of updated record
         """
         return self._put("metadataprofile", self.ver_uri, data=data)
 
     # GET /config/metadataProvider
-    def get_metadata_provider(self) -> list[dict[str, Any]]:
+    def get_metadata_provider(self) -> JsonObject:
         """Get metadata provider config (settings/metadata)
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            JsonObject: Dictionary with data
         """
-        return self.assert_return("config/metadataProvider", self.ver_uri, list)
+        return self._get("config/metadataProvider", self.ver_uri)
 
     # PUT /config/metadataprovider
-    def upd_metadata_provider(self, data: dict[str, Any]) -> dict[str, Any]:
+    def upd_metadata_provider(self, data: JsonObject) -> JsonObject:
         """Update metadata provider by providing json data update
 
         Note:
             To be used in conjunction with get_metadata_provider()
 
         Args:
-            data (dict[str, Any]): Configuration data
+            data (JsonObject): Configuration data
 
         Returns:
-            dict[str, Any]: Dictionary of updated record
+            JsonObject: Dictionary of updated record
         """
         return self._put("config/metadataProvider", self.ver_uri, data=data)
 
     # GET /queue
     def get_queue(
         self,
-        page: int = PAGE,
-        page_size: int = PAGE_SIZE,
-        sort_key: LidarrSortKeys = LidarrSortKeys.TIMELEFT,
-        unknown_artists: bool = False,
-        include_artist: bool = False,
-        include_album: bool = False,
-    ) -> dict[str, Any]:
+        page: Optional[int] = None,
+        page_size: Optional[int] = None,
+        sort_key: Optional[LidarrSortKey] = None,
+        sort_dir: Optional[PyarrSortDirection] = None,
+        unknown_artists: Optional[bool] = None,
+        include_artist: Optional[bool] = None,
+        include_album: Optional[bool] = None,
+    ) -> JsonObject:
         """Get the queue of download_release
 
         Args:
-            page (int, optional): Which page to load. Defaults to PAGE.
-            page_size (int, optional): Number of items per page. Defaults to PAGE_SIZE.
-            sort_key (LidarrSortKeys, optional): Key to sort by. Defaults to LidarrSortKeys.TIMELEFT.
-            unknown_artists (bool, optional): Include unknown artists. Defaults to False.
-            include_artist (bool, optional): Include Artists. Defaults to False.
-            include_album (bool, optional): Include albums. Defaults to False.
-
-        Returns:
-            dict[str, Any]: List of dictionaries with items
-        """
-        params = {
-            "page": page,
-            "pageSize": page_size,
-            "sortKey": sort_key,
-            "unknownArtists": unknown_artists,
-            "includeAlbum": include_album,
-            "includeArtist": include_artist,
-        }
+            page (Optional[int], optional): Page number to return. Defaults to None.
+            page_size (Optional[int], optional): Number of items per page. Defaults to None.
+            sort_key (Optional[LidarrSortKey], optional): Column to sort by. Defaults to None.
+            sort_dir (Optional[PyarrSortDirection], optional): Direction to sort the items. Defaults to None.
+            unknown_artists (Optional[bool], optional): Include unknown artists. Defaults to None.
+            include_artist (Optional[bool], optional): Include Artists. Defaults to None.
+            include_album (Optional[bool], optional): Include albums. Defaults to None.
+
+        Returns:
+            JsonObject: List of dictionaries with items
+        """
+        params: dict[str, Union[int, str, PyarrSortDirection, LidarrSortKey]] = {}
+        if page:
+            params["page"] = page
+        if page_size:
+            params["pageSize"] = page_size
+        if sort_key and sort_dir:
+            params["sortKey"] = sort_key
+            params["sortDirection"] = sort_dir
+        elif sort_key or sort_dir:
+            raise PyarrMissingArgument("sort_key and sort_dir  must be used together")
+
+        if unknown_artists:
+            params["unknownArtists"] = unknown_artists
+        if include_album:
+            params["includeAlbum"] = include_album
+        if include_artist:
+            params["includeArtist"] = include_artist
 
-        return self.assert_return("queue", self.ver_uri, dict, params=params)
+        return self._get("queue", self.ver_uri, params=params)
 
     # GET /queue/details
     def get_queue_details(
         self,
         artistId: Optional[int] = None,
         albumIds: Union[list[int], None] = None,
-        include_artist: bool = False,
-        include_album: bool = True,
-    ) -> list[dict[str, Any]]:
+        include_artist: Optional[bool] = None,
+        include_album: Optional[bool] = None,
+    ) -> JsonArray:
         """Get queue details for artist or album
 
         Args:
             artistId (Optional[int], optional): Artist database ID. Defaults to None.
             albumIds (Union[list[int], None], optional): Album database ID. Defaults to None.
-            include_artist (bool, optional): Include the artist. Defaults to False.
-            include_album (bool, optional): Include the album. Defaults to True.
+            include_artist (Optional[bool], optional): Include the artist. Defaults to None.
+            include_album (Optional[bool], optional): Include the album. Defaults to None.
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            JsonArray: List of dictionaries with items
         """
 
-        params: dict[str, Any] = {
-            "includeArtist": include_artist,
-            "includeAlbum": include_album,
-        }
-        if artistId is not None:
+        params: dict[str, Any] = {}
+        if include_artist:
+            params["includeArtist"] = include_artist
+        if include_album:
+            params["includeAlbum"] = include_album
+        if artistId:
             params["artistId"] = artistId
-        if albumIds is not None:
+        if albumIds:
             params["albumIds"] = albumIds
 
-        return self.assert_return("queue/details", self.ver_uri, list, params=params)
+        return self._get("queue/details", self.ver_uri, params=params)
 
     # GET /release
     def get_release(
         self, artistId: Optional[int] = None, albumId: Optional[int] = None
-    ) -> list[dict[str, Any]]:
+    ) -> JsonArray:
         """Search indexers for specified fields.
 
         Args:
             artistId (Optional[int], optional): Artist ID from DB. Defaults to None.
             albumId (Optional[int], optional): Album IT from Database. Defaults to None.
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            JsonArray: List of dictionaries with items
         """
         params = {}
-        if artistId is not None:
+        if artistId:
             params["artistId"] = artistId
-        if albumId is not None:
-            params["artistId"] = albumId
-        return self.assert_return("release", self.ver_uri, list, params=params)
+        if albumId:
+            params["albumId"] = albumId
+        return self._get("release", self.ver_uri, params=params)
 
     # GET /rename
-    def get_rename(
-        self, artistId: int, albumId: Optional[int] = None
-    ) -> list[dict[str, Any]]:
+    def get_rename(self, artistId: int, albumId: Optional[int] = None) -> JsonArray:
         """Get files matching specified id that are not properly renamed yet.
 
         Args:
             artistId (int): Database ID for Artists
             albumId (Optional[int], optional): Album ID. Defaults to None.
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            JsonArray: List of dictionaries with items
         """
         params = {"artistId": artistId}
-        if albumId is not None:
+        if albumId:
             params["albumId"] = albumId
-        return self.assert_return(
+        return self._get(
             "rename",
             self.ver_uri,
-            list,
             params=params,
         )
 
     # GET /manualimport
     def get_manual_import(
         self,
-        downloadId: str,
-        artistId: int = 0,
-        folder: Optional[str] = None,
-        filterExistingFiles: bool = True,
-        replaceExistingFiles: bool = True,
-    ) -> list[dict[str, Any]]:
+        folder: str,
+        downloadId: Optional[str] = None,
+        artistId: Optional[int] = None,
+        filterExistingFiles: Optional[bool] = None,
+        replaceExistingFiles: Optional[bool] = None,
+    ) -> JsonArray:
         """Gets a manual import list
 
         Args:
             downloadId (str): Download IDs
             artistId (int, optional): Artist Database ID. Defaults to 0.
             folder (Optional[str], optional): folder name. Defaults to None.
             filterExistingFiles (bool, optional): filter files. Defaults to True.
             replaceExistingFiles (bool, optional): replace files. Defaults to True.
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            JsonArray: List of dictionaries with items
         """
-        params = {
-            "artistId": artistId,
-            "downloadId": downloadId,
-            "filterExistingFiles": str(filterExistingFiles),
-            "folder": folder if folder is not None else "",
-            "replaceExistingFiles": str(replaceExistingFiles),
-        }
-        return self.assert_return("manualimport", self.ver_uri, list, params=params)
+        params: dict[str, Union[str, int, bool]] = {"folder": folder}
+        if downloadId:
+            params["downloadId"] = downloadId
+        if artistId:
+            params["artistId"] = artistId
+        if filterExistingFiles:
+            params["filterExistingFiles"] = filterExistingFiles
+        if replaceExistingFiles:
+            params["replaceExistingFiles"] = replaceExistingFiles
+
+        return self._get("manualimport", self.ver_uri, params=params)
 
     # PUT /manualimport
-    def upd_manual_import(self, data: dict[str, Any]) -> dict[str, Any]:
+    def upd_manual_import(self, data: JsonObject) -> JsonObject:
         """Update a manual import
 
         Note:
             To be used in conjunction with get_manual_import()
 
         Args:
-            data (dict[str, Any]): Data containing changes
+            data (JsonObject): Data containing changes
 
         Returns:
-            dict[str, Any]: Dictionary of updated record
+            JsonObject: Dictionary of updated record
         """
         return self._put("manualimport", self.ver_uri, data=data)
 
     # GET /retag
     def get_retag(
-        self, artistId: int, albumId: Optional[int] = None
-    ) -> list[dict[str, Any]]:
+        self, artistId: Optional[int] = None, albumId: Optional[int] = None
+    ) -> JsonArray:
         """Get Retag
 
         Args:
             artistId (int): ID for the  artist
             albumId Optional[int], optional): ID foir the album. Defaults to None.
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            JsonArray: List of dictionaries with items
         """
-        params = {"artistId": artistId}
-        if albumId is not None:
+        params = {}
+        if artistId:
+            params["artistId"] = artistId
+        if albumId:
             params["albumId"] = albumId
-        return self.assert_return(
+        return self._get(
             "retag",
             self.ver_uri,
-            list,
             params=params,
         )
+
+    # POST /qualityprofile
+    def add_quality_profile(
+        self, name: str, upgrades_allowed: bool, cutoff: int, items: list
+    ) -> JsonObject:
+        """Add new quality profile
+
+        Args:
+            name (str): Name of the profile
+            upgrades_allowed (bool): Are upgrades in quality allowed?
+            cutoff (int): ID of quality definition to cutoff at. Must be an allowed definition ID.
+            items (list): Add a list of items (from `get_quality_definition()`)
+
+        Returns:
+            JsonObject: An object containing the profile
+        """
+        data = {
+            "name": name,
+            "upgradeAllowed": upgrades_allowed,
+            "cutoff": cutoff,
+            "items": items,
+        }
+        return self._post("qualityprofile", self.ver_uri, data=data)
```

### Comparing `pyarr-4.1.0/pyarr/readarr.py` & `pyarr-5.0.0/pyarr/radarr.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,606 +1,611 @@
 from typing import Any, Optional, Union
+from warnings import warn
 
 from requests import Response
 
+from pyarr.types import JsonArray, JsonObject
+
 from .base import BaseArrAPI
-from .const import PAGE, PAGE_SIZE
-from .exceptions import PyarrMissingProfile
+from .exceptions import PyarrMissingArgument
 from .models.common import PyarrSortDirection
-from .models.readarr import (
-    ReadarrAuthorMonitor,
-    ReadarrBookTypes,
-    ReadarrCommands,
-    ReadarrSortKeys,
+from .models.radarr import (
+    RadarrAvailabilityType,
+    RadarrCommands,
+    RadarrEventType,
+    RadarrMonitorType,
+    RadarrSortKey,
 )
 
 
-class ReadarrAPI(BaseArrAPI):
-    """API wrapper for Readarr endpoints."""
+class RadarrAPI(BaseArrAPI):
+    """API wrapper for Radarr endpoints.
+
+    Args:
+        RequestAPI (:obj:`str`): provides connection to API endpoint
+    """
 
     def __init__(self, host_url: str, api_key: str):
-        """Initialise Readarr API
+        """Initialize the Radarr API.
 
         Args:
-            host_url (str): URL for Readarr
-            api_key (str): API key for Readarr
+            host_url (str): URL for Radarr
+            api_key (str): API key for Radarr
         """
 
-        ver_uri = "/v1"
+        ver_uri = "/v3"
         super().__init__(host_url, api_key, ver_uri)
 
-    def _book_json(
+    ## CONFIG
+    # POST /rootfolder
+    def add_root_folder(
         self,
-        db_id: str,
-        book_id_type: ReadarrBookTypes,
-        root_dir: str,
-        quality_profile_id: Optional[int] = None,
-        metadata_profile_id: Optional[int] = None,
-        monitored: bool = True,
-        search_for_new_book: bool = False,
-        author_monitor: ReadarrAuthorMonitor = ReadarrAuthorMonitor.ALL,
-        author_search_for_missing_books: bool = False,
-    ) -> dict[str, Any]:
-        """Constructs the JSON required to add a new book to Readarr
-
-        Args:
-            db_id (str): Book ID from Goodreads, ISBN or ASIN
-            book_id_type (ReadarrBookTypes): Type of book ID
-            root_dir (str): Root directory for books
-            quality_profile_id (Optional[int], optional): Quality profile ID. Defaults to None.
-            metadata_profile_id (Optional[int], optional): Metadata profile ID. Defaults to None.
-            monitored (bool, optional): Monitor for book. Defaults to True.
-            search_for_new_book (bool, optional): Search for new book on adding. Defaults to False.
-            author_monitor (ReadarrAuthorMonitor, optional): Monitor the author. Defaults to ReadarrAuthorMonitor.ALL.
-            author_search_for_missing_books (bool, optional): Search for other missing books by author. Defaults to False.
-
-        Raises:
-            PyarrMissingProfile: Error if Metadata or Quality profile ID are incorrect
-
-        Returns:
-            dict[str, Any]: Dictionary of generated record
-        """
-        if quality_profile_id is None:
-            try:
-                quality_profile_id = self.get_quality_profile()[0]["id"]
-            except IndexError as exception:
-                raise PyarrMissingProfile(
-                    "There is no Quality Profile setup"
-                ) from exception
-        if metadata_profile_id is None:
-            try:
-                metadata_profile_id = self.get_metadata_profile()[0]["id"]
-            except IndexError as exception:
-                raise PyarrMissingProfile(
-                    "There is no Metadata Profile setup"
-                ) from exception
-        book = self.lookup_book(f"{book_id_type}:{db_id}")[0]
-
-        book["author"]["metadataProfileId"] = metadata_profile_id
-        book["author"]["qualityProfileId"] = quality_profile_id
-        book["author"]["rootFolderPath"] = root_dir
-        book["author"]["addOptions"] = {
-            "monitor": author_monitor,
-            "searchForMissingBooks": author_search_for_missing_books,
-        }
-        book["monitored"] = monitored
-        book["author"]["manualAdd"] = True
-        book["addOptions"] = {"searchForNewBook": search_for_new_book}
+        directory: str,
+    ) -> JsonObject:
+        """Adds a new root folder
 
-        return book
+        Args:
+            directory (str): The directory path
+
+        Returns:
+            JsonObject: Dictionary containing path details
+        """
+        return self._post("rootfolder", self.ver_uri, data={"path": directory})
+
+    ## MOVIE
+
+    # GET /movie
+    def get_movie(
+        self, id_: Optional[int] = None, tmdb: bool = False
+    ) -> Union[JsonArray, JsonObject]:  # sourcery skip: class-extract-method
+        """Returns all movies in the database, movie based on the Radarr ID or TMDB id.
+
+        Note:
+            IMDB is not supported at this time
 
-    def _author_json(
+        Args:
+            id_ (Optional[int], optional): Radarr ID or TMDB ID of Movies. Defaults to None.
+            tmdb (bool): Use TMDB Id. Defaults to False
+
+        Returns:
+            Union[JsonArray, JsonObject]: List or Dictionary with items
+        """
+        params = {}
+        if tmdb:
+            params["tmdbid"] = id_
+
+        return self._get(
+            f"movie{'' if id_ is None or tmdb else f'/{id_}'}",
+            self.ver_uri,
+            params=params,
+        )
+
+    # POST /movie
+    def add_movie(
         self,
-        term: str,
+        movie: JsonObject,
         root_dir: str,
-        quality_profile_id: Optional[int] = None,
-        metadata_profile_id: Optional[int] = None,
+        quality_profile_id: int,
         monitored: bool = True,
-        author_monitor: ReadarrAuthorMonitor = ReadarrAuthorMonitor.NONE,
-        search_for_missing_books: bool = False,
-    ) -> dict[str, Any]:
-        """Constructs the JSON required to add a new book to Readarr
-
-        Args:
-            term (str): Search term
-            root_dir (str): Root directory for books
-            quality_profile_id (Optional[int], optional): Quality profile ID. Defaults to None.
-            metadata_profile_id (Optional[int], optional): Metadata profile ID. Defaults to None.
-            monitored (bool, optional): Monitor this author. Defaults to True.
-            author_monitor (ReadarrAuthorMonitor, optional): Monitor the author. Defaults to ReadarrAuthorMonitor.NONE.
-            search_for_missing_books (bool, optional): Search for missing books by the author. Defaults to False.
-
-        Raises:
-            PyarrMissingProfile: Error if Metadata or Quality profile ID are incorrect
-
-        Returns:
-            dict[str, Any]: Dictionary of author data
-        """
-        if quality_profile_id is None:
-            try:
-                quality_profile_id = self.get_quality_profile()[0]["id"]
-            except IndexError as exception:
-                raise PyarrMissingProfile(
-                    "There is no Quality Profile setup"
-                ) from exception
-        if metadata_profile_id is None:
-            try:
-                metadata_profile_id = self.get_metadata_profile()[0]["id"]
-            except IndexError as exception:
-                raise PyarrMissingProfile(
-                    "There is no Metadata Profile setup"
-                ) from exception
-
-        author = self.lookup_author(term)[0]
-
-        author["metadataProfileId"] = metadata_profile_id
-        author["qualityProfileId"] = quality_profile_id
-        author["rootFolderPath"] = root_dir
-        author["addOptions"] = {
-            "monitor": author_monitor,
-            "searchForMissingBooks": search_for_missing_books,
+        search_for_movie: bool = True,
+        monitor: RadarrMonitorType = "movieOnly",
+        minimum_availability: RadarrAvailabilityType = "announced",
+        tags: list[int] = [],
+    ) -> JsonObject:
+        """Adds a movie to the database
+
+        Args:
+            movie (JsonObject): Movie record from `lookup_movie()`
+            root_dir (str): Location of the root DIR
+            quality_profile_id (int): ID of the quality profile the movie will use
+            monitored (bool, optional): Should the movie be monitored. Defaults to True.
+            search_for_movie (bool, optional): Should we search for the movie. Defaults to True.
+            monitor (RadarrMonitorType, optional): Monitor movie or collection. Defaults to "movieOnly".
+            minimum_availability (RadarrAvailabilityType, optional): Availability of movie. Defaults to "announced"
+            tags (list[int], optional): List of tag id's. Defaults to [].
+
+        Returns:
+            JsonObject: Dictonary with added record
+        """
+        movie["rootFolderPath"] = root_dir
+        movie["qualityProfileId"] = quality_profile_id
+        movie["monitored"] = monitored
+        movie["minimumAvailability"] = minimum_availability
+        movie["addOptions"] = {
+            "monitor": monitor,
+            "searchForMovie": search_for_movie,
         }
-        author["monitored"] = monitored
+        movie["tags"] = tags
 
-        return author
+        return self._post("movie", self.ver_uri, data=movie)
 
-    # COMMAND
+    # PUT /movie
+    def upd_movie(
+        self,
+        data: JsonObject,
+        move_files: Optional[bool] = None,
+    ) -> JsonObject:
+        """Updates a movie in the database.
+
+        Args:
+            data (JsonObject): Dictionary containing an object obtained from get_movie()
+            move_files (Optional[bool], optional): Have radarr move files when updating. Defaults to None.
+
+        Returns:
+            JsonObject: Dictionary with updated record
+        """
+        params = {}
+        if move_files is not None:
+            params["moveFiles"] = move_files
+        print(type(data))
+        return self._put(
+            "movie",
+            self.ver_uri,
+            data=data,
+            params=params,
+        )
 
-    # GET /command/:id
-    def get_command(self, id_: Optional[int] = None) -> list[dict[str, Any]]:
-        """Queries the status of a previously started command, or all currently started commands.
+    # GET /movie/{id}
+    def get_movie_by_movie_id(self, id_: int) -> JsonObject:
+        """Get a movie by the Radarr database ID
 
         Args:
-            id_ (Optional[int], optional): Database ID of the command. Defaults to None.
+            id_ (int): Database Id of movie to return
+
+        Note:
+            This method is deprecated and will be removed in a
+            future release. Please use get_movie()
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            JsonArray: List of dictionaries with items
         """
-        path = f"command/{id_}" if id_ else "command"
-        return self.assert_return(path, self.ver_uri, list)
+        warn(
+            "This method is deprecated and will be removed in a future release. Please use get_movie()",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return self._get(f"movie/{id_}", self.ver_uri)
 
-    # POST /command
-    # TODO: confirm return type & Kwargs
-    def post_command(self, name: ReadarrCommands, **kwargs) -> Any:
-        """Performs any of the predetermined Readarr command routines
+    # DELETE /movie/{id}
+    def del_movie(
+        self,
+        id_: Union[int, list],
+        delete_files: Optional[bool] = None,
+        add_exclusion: Optional[bool] = None,
+    ) -> Union[Response, JsonObject, dict[Any, Any]]:
+        """Delete a single movie or multiple movies by database id.
 
         Args:
-            name (ReadarrCommands): Command name that should be executed
-            **kwargs: Additional parameters for specific commands
+            id_ (Union[int, list]): Int with single movie Id or list with multiple IDs to delete.
+            delete_files (bool, optional): Delete movie files when deleting movies. Defaults to None.
+            add_exclusion (bool, optional): Add deleted movies to List Exclusions. Defaults to None.
 
         Returns:
-            _type_: _description_
+            Response: HTTP Response
         """
-        data = {
-            "name": name,
-            **kwargs,
-        }
-        return self._post("command", self.ver_uri, data=data)
-
-    ## WANTED (MISSING)
-
-    # GET /wanted/missing
-    def get_missing(
-        self,
-        sort_key: ReadarrSortKeys = ReadarrSortKeys.BOOK_ID,
-        page: int = PAGE,
-        page_size: int = PAGE_SIZE,
-        sort_dir: PyarrSortDirection = PyarrSortDirection.ASC,
-    ) -> dict[str, Any]:
-        """Gets missing episode (episodes without files)
-
-        Args:
-            sort_key (ReadarrSortKeys, optional): id, title, ratings, bookid, or quality. (Others do not apply). Defaults to ReadarrSortKeys.BOOK_ID.
-            page (int, optional): Page number to return. Defaults to PAGE.
-            page_size (int, optional): Number of items per page. Defaults to PAGE_SIZE.
-            sort_dir (PyarrSortDirection, optional): Direction to sort the items. Defaults to PyarrSortDirection.ASC.
-
-        Returns:
-            dict[str, Any]: List of dictionaries with items
-        """
-        params = {
-            "sortKey": sort_key,
-            "page": page,
-            "pageSize": page_size,
-            "sortDir": sort_dir,
-        }
-        return self.assert_return("wanted/missing", self.ver_uri, dict, params)
+        params: dict[str, Union[str, list[int], int]] = {}
+        if isinstance(id_, list):
+            params["movieIds"] = id_
+        if delete_files:
+            params["deleteFiles"] = delete_files
+
+        if add_exclusion:
+            params["addImportExclusion"] = add_exclusion
+
+            print(params)
+        return self._delete(
+            "movie/editor" if isinstance(id_, list) else f"movie/{id_}",
+            self.ver_uri,
+            params=None if isinstance(id_, list) else params,
+            data=params if isinstance(id_, list) else None,
+        )
 
-    # GET /wanted/cutoff
-    def get_cutoff(
-        self,
-        sort_key: ReadarrSortKeys = ReadarrSortKeys.BOOK_ID,
-        page: int = PAGE,
-        page_size: int = PAGE_SIZE,
-        sort_dir: PyarrSortDirection = PyarrSortDirection.DESC,
-        monitored: bool = True,
-    ) -> dict[str, Any]:
-        """Get wanted items where the cutoff is unmet
+    # GET /movie/lookup
+    def lookup_movie(self, term: str) -> JsonArray:
+        """Search for a movie to add to the database (Uses TMDB for search results)
 
         Args:
-            sort_key (ReadarrSortKeys, optional): id, title, ratings, bookid, or quality". (others do not apply). Defaults to ReadarrSortKeys.BOOK_ID.
-            page (int, optional): Page number to return. Defaults to PAGE.
-            page_size (int, optional):  Number of items per page. Defaults to PAGE_SIZE.
-            sort_dir (PyarrSortDirection, optional): Direction to sort. Defaults to PyarrSortDirection.DESC.
-            monitored (bool, optional): Search for monitored only. Defaults to True.
+            term (str): Search term to use for lookup, can also do IMDB & TMDB IDs::
+
+                radarr.lookup_movie(term="imdb:123456")
+                radarr.lookup_movie(term="tmdb:123456")
 
         Returns:
-            dict[str, Any]: List of dictionaries with items
+            JsonArray: List of dictionaries with items
         """
-        params = {
-            "sortKey": sort_key,
-            "page": page,
-            "pageSize": page_size,
-            "sortDir": sort_dir,
-            "monitored": monitored,
-        }
-        return self.assert_return("wanted/cutoff", self.ver_uri, dict, params)
-
-    ## QUEUE
-
-    # GET /queue
-    def get_queue(
-        self,
-        page: int = PAGE,
-        page_size: int = PAGE_SIZE,
-        sort_dir: PyarrSortDirection = PyarrSortDirection.ASC,
-        sort_key: ReadarrSortKeys = ReadarrSortKeys.TIMELEFT,
-        unknown_authors: bool = False,
-        include_author: bool = False,
-        include_book: bool = False,
-    ) -> dict[str, Any]:
-        """Get current download information
-
-        Args:
-            page (int, optional): Page number. Defaults to PAGE.
-            page_size (int, optional): Number of items per page. Defaults to PAGE_SIZE.
-            sort_dir (PyarrSortDirection, optional): Direction to sort. Defaults to PyarrSortDirection.ASC.
-            sort_key (ReadarrSortKeys, optional): Field to sort by. Defaults to ReadarrSortKeys.TIMELEFT.
-            unknown_authors (bool, optional): Include items with an unknown author. Defaults to False.
-            include_author (bool, optional): Include the author. Defaults to False.
-            include_book (bool, optional): Include the book. Defaults to False.
-
-        Returns:
-            dict[str, Any]: List of dictionaries with items
-        """
-        params = {
-            "sortKey": sort_key,
-            "page": page,
-            "pageSize": page_size,
-            "sortDirection": sort_dir,
-            "includeUnknownAuthorItems": unknown_authors,
-            "includeAuthor": include_author,
-            "includeBook": include_book,
-        }
-        return self.assert_return("queue", self.ver_uri, dict, params)
+        params = {"term": term}
+        return self._get("movie/lookup", self.ver_uri, params)
 
-    # GET /metadataprofile/{id}
-    def get_metadata_profile(self, id_: Optional[int] = None) -> list[dict[str, Any]]:
-        """Gets all metadata profiles or specific one with ID
+    # GET /movie/lookup
+    def lookup_movie_by_tmdb_id(self, id_: int) -> JsonArray:
+        """Search for movie by TMDB ID
 
         Args:
-            id_ (Optional[int], optional): Metadata profile id from database. Defaults to None.
+            id_ (str): TMDB ID
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            JsonArray: List of dictionaries with items
         """
-        path = f"metadataprofile/{id_}" if id_ else "metadataprofile"
-        return self.assert_return(path, self.ver_uri, list)
+        warn(
+            "This method is deprecated and will be removed in a future release. use lookup_movie(term='tmdb:123456')",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        params = {"term": f"tmdb:{id_}"}
+        return self._get("movie/lookup", self.ver_uri, params)
 
-    # GET /delayprofile/{id}
-    def get_delay_profile(self, id_: Optional[int] = None) -> list[dict[str, Any]]:
-        """Gets all delay profiles or specific one with ID
+    # GET /movie/lookup
+    def lookup_movie_by_imdb_id(self, id_: str) -> JsonArray:
+        """Search for movie by IMDB ID
 
         Args:
-            id_ (Optional[int], optional): Metadata profile ID from database. Defaults to None.
+            id_ (str): IMDB ID
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            JsonArray: List of dictionaries with items
         """
-        path = f"delayprofile/{id_}" if id_ else "delayprofile"
-        return self.assert_return(path, self.ver_uri, list)
+        warn(
+            "This method is deprecated and will be removed in a future release. use lookup_movie(term='imdb:123456')",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        params = {"term": f"imdb:{id_}"}
+        return self._get("movie/lookup", self.ver_uri, params)
 
-    # GET /releaseprofile/{id}
-    def get_release_profile(self, id_: Optional[int] = None) -> list[dict[str, Any]]:
-        """Gets all release profiles or specific one with ID
+    # PUT /movie/editor
+    def upd_movies(self, data: JsonObject) -> JsonArray:
+        """The Updates operation allows to edit properties of multiple movies at once
 
         Args:
-            id_ (Optional[int], optional): Release profile ID from database. Defaults to None.
+            data (JsonObject): Updated movie information::
+
+                {"movieIds":[28],"tags":[3],"applyTags":"add"}
+                {"movieIds":[28],"monitored":true}
+                {"movieIds":[28],"qualityProfileId":1}
+                {"movieIds":[28],"minimumAvailability":"inCinemas"}
+                {"movieIds":[28],"rootFolderPath":"/defaults/"}
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            JsonArray: Dictionary containing updated record
         """
-        path = f"releaseprofile/{id_}" if id_ else "releaseprofile"
-        return self.assert_return(path, self.ver_uri, list)
 
-    ## BOOKS
+        return self._put("movie/editor", self.ver_uri, data=data)
 
-    # GET /book and /book/{id}
-    def get_book(self, id_: Optional[int] = None) -> list[dict[str, Any]]:
-        """Returns all books in your collection or the book with the matching
-        book ID if one is found.
+    # DELETE /movie/editor
+    def del_movies(
+        self, data: JsonObject
+    ) -> Union[Response, JsonObject, dict[Any, Any]]:
+        """The delete operation allows mass deletion of movies (and optionally files)
 
         Args:
-            id_ (Optional[int], optional): Database id for book. Defaults to None.
+            data (JsonObject): dictionary of movies to be deleted::
+
+                {
+                    "movieIds": [
+                        0
+                    ],
+                    "deleteFIles": true,
+                    "addImportExclusion": true
+                }
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            Response: HTTP Response
         """
-        path = f"book/{id_}" if id_ else "book"
-        return self.assert_return(path, self.ver_uri, list)
+        warn(
+            "This method is deprecated and will be removed in a future release. Please use del_movie().",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        return self._delete("movie/editor", self.ver_uri, data=data)
 
-    # GET /book/lookup
-    def lookup_book(self, term: str) -> list[dict[str, Any]]:
-        """Searches for new books using a term, goodreads ID, isbn or asin.
+    # POST /movie/import
+    def import_movies(self, data: JsonArray) -> JsonArray:
+        """The movie import endpoint is used by the bulk import view in Radarr UI. It allows movies to be bulk added to the Radarr database.
 
         Args:
-            term (str): Search term::
-
-                goodreads:656
-                isbn:067003469X
-                asin:B00JCDK5ME
+            data (JsonObject): dictionary of all movies to be imported
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            JsonArray: List of dictionaries with items
         """
-        return self.assert_return("book/lookup", self.ver_uri, list, {"term": term})
+        return self._post("movie/import", self.ver_uri, data=data)
 
-    # POST /book
-    def add_book(
-        self,
-        db_id: str,
-        book_id_type: ReadarrBookTypes,
-        root_dir: str,
-        quality_profile_id: Optional[int] = None,
-        metadata_profile_id: Optional[int] = None,
-        monitored: bool = True,
-        search_for_new_book: bool = False,
-        author_monitor: ReadarrAuthorMonitor = ReadarrAuthorMonitor.ALL,
-        author_search_for_missing_books: bool = False,
-    ) -> dict[str, Any]:
-        """Adds a new book and  its associated author (if not already added)
-
-        Args:
-            db_id (int): goodreads, isbn, asin ID for the book
-            book_id_type (str): goodreads / isbn / asin
-            root_dir (str): Directory for book to be stored
-            quality_profile_id (int, optional): quality profile id. Defaults to 1.
-            metadata_profile_id (int, optional): metadata profile id. Defaults to 0.
-            monitored (bool, optional): should the book be monitored. Defaults to True.
-            search_for_new_book (bool, optional): search for the book to download now. Defaults to False.
-            author_monitor (str, optional): monitor the author for new books. Defaults to "all".
-            author_search_for_missing_books (bool, optional): search for missing books from this author. Defaults to False.
-
-        Returns:
-            dict[str, Any]: Dictionary of added record
-        """
-
-        book_json = self._book_json(
-            db_id,
-            book_id_type,
-            root_dir,
-            quality_profile_id,
-            metadata_profile_id,
-            monitored,
-            search_for_new_book,
-            author_monitor,
-            author_search_for_missing_books,
-        )
-        return self._post("book", self.ver_uri, data=book_json)
+    ## MOVIEFILE
 
-    # PUT /book/{id}
-    def upd_book(self, id_: int, data: dict[str, Any]) -> dict[str, Any]:
-        """Update the given book, currently only monitored is changed, all other modifications are ignored.
+    # GET /moviefile
+    # TODO: merge this with get_movie_file
+    def get_movie_files_by_movie_id(self, id_: int) -> JsonArray:
+        """Get a movie file object by Movie database ID.
 
-        Note:
-            To be used in conjunction with get_book()
+        Args:
+            id_ (int): Movie database ID
+
+        Returns:
+            JsonArray: List of dictionaries with items
+        """
+
+        params = {"movieId": id_}
+        return self._get("moviefile", self.ver_uri, params)
+
+    # GET /moviefile
+    def get_movie_file(self, id_: Union[int, list]) -> JsonArray:
+        """Get movie file by database ID
 
         Args:
-            id_ (int): Book database ID to update
-            data (dict[str, Any]): All parameters to update book
+            id_ (int, list): Movie file ID, or multiple in a list
 
         Returns:
-            dict[str, Any]: Dictionary with updated record
+            JsonArray: List of dictionaries with items
         """
-        return self._put(f"book/{id_}", self.ver_uri, data=data)
+        if not isinstance(id_, list):
+            return self._get(f"moviefile/{id_}", self.ver_uri)
+        params = [("movieFileIds", file) for file in id_]
+        return self._get("moviefile", self.ver_uri, params=params)
 
-    # DELETE /book/{id}
-    def del_book(
-        self, id_: int, delete_files: bool = False, import_list_exclusion: bool = True
-    ) -> Union[Response, dict[str, Any], dict[Any, Any]]:
-        """Delete the book with the given ID
+    # DELETE /moviefile/{id}
+    def del_movie_file(
+        self, id_: Union[int, list]
+    ) -> Union[Response, JsonObject, dict[Any, Any]]:
+        """Allows for deletion of a moviefile by its database ID.
 
         Args:
-            id_ (int): Database ID for book
-            delete_files (bool, optional): If true book folder and files will be deleted. Defaults to False.
-            import_list_exclusion (bool, optional): Add an exclusion so book doesn't get re-added. Defaults to True.
+            id_ (Union[int, list]): Movie file ID
 
         Returns:
             Response: HTTP Response
         """
-        params = {
-            "deleteFiles": delete_files,
-            "addImportListExclusion": import_list_exclusion,
-        }
-        return self._delete(f"book/{id_}", self.ver_uri, params=params)
 
-    # AUTHOR
+        if isinstance(id_, list):
+            data = {"movieFileIds": id_}
+        return self._delete(
+            "moviefile/bulk" if isinstance(id_, list) else f"moviefile/{id_}",
+            self.ver_uri,
+            data=data if isinstance(id_, list) else None,
+        )
 
-    # GET /author and /author/{id}
-    def get_author(self, id_: Optional[int] = None) -> list[dict[str, Any]]:
-        """Returns all authors in your collection or the author with the matching ID if one is found.
+    # GET /history/movie
+    def get_movie_history(
+        self, id_: int, event_type: Optional[RadarrEventType] = None
+    ) -> JsonArray:
+        """Get history for a given movie in database by its database ID
 
         Args:
-            id_ (Optional[int], optional): Database ID for author. Defaults to None.
+            id_ (int): Database ID of movie
+            event_type (Optional[RadarrEventType], optional): History event type to retrieve. Defaults to None.
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            JsonArray: List of dictionaries with items
         """
-        path = f"author/{id_}" if id_ else "author"
-        return self.assert_return(path, self.ver_uri, list)
+        params: dict[str, Union[int, str, RadarrEventType]] = {"movieId": id_}
+        if event_type:
+            params["eventType"] = event_type
+        return self._get("history/movie", self.ver_uri, params)
+
+    ## BLOCKLIST
 
-    # GET /author/lookup/
-    def lookup_author(self, term: str) -> list[dict[str, Any]]:
-        """Searches for new authors using a term
+    # GET /blocklist/movie
+    def get_blocklist_by_movie_id(
+        self,
+        id_: int,
+    ) -> JsonArray:
+        """Retrieves blocklisted releases that are tied to a given movie in the database.
 
         Args:
-            term (str): Author name or book
+            id_ (int): Movie id from Database
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            JsonArray: List of dictionaries with items
         """
-        params = {"term": term}
-        return self.assert_return("author/lookup", self.ver_uri, list, params)
+        params = {"movieId": id_}
+        return self._get("blocklist/movie", self.ver_uri, params)
+
+    ## QUEUE
 
-    # POST /author/
-    def add_author(
+    # GET /queue
+    def get_queue(
         self,
-        search_term: str,
-        root_dir: str,
-        quality_profile_id: Optional[int] = None,
-        metadata_profile_id: Optional[int] = None,
-        monitored: bool = True,
-        author_monitor: ReadarrAuthorMonitor = ReadarrAuthorMonitor.NONE,
-        author_search_for_missing_books: bool = False,
-    ) -> dict[str, Any]:
-        """Adds an authorbased on search term, must be author name or book by goodreads / isbn / asin ID
-
-        Args:
-            search_term (str): Author name or Author book by ID
-            root_dir (str): Directory for book to be stored
-            quality_profile_id (int, optional): Quality profile id. Defaults to 1.
-            metadata_profile_id (int, optional): Metadata profile id. Defaults to 0.
-            monitored (bool, optional): Should the author be monitored. Defaults to True.
-            author_monitor (ReadarrAuthorMonitor, optional): What level  should the author be monitored. Defaults to "ReadarrAuthorMonitor.NONE".
-            author_search_for_missing_books (bool, optional): Search for any missing books by the author. Defaults to False.
-
-        Returns:
-            dict[str, Any]: Dictonary of added record
-        """
-        author_json = self._author_json(
-            search_term,
-            root_dir,
-            quality_profile_id,
-            metadata_profile_id,
-            monitored,
-            author_monitor,
-            author_search_for_missing_books,
-        )
-        return self._post("author", self.ver_uri, data=author_json)
+        page: Optional[int] = None,
+        page_size: Optional[int] = None,
+        sort_dir: Optional[PyarrSortDirection] = None,
+        sort_key: Optional[RadarrSortKey] = None,
+        include_unknown_movie_items: Optional[bool] = None,
+    ) -> JsonObject:
+        """Return a list of items in the queue
+
+        Args:
+            page (Optional[int], optional): Page to be returned. Defaults to None.
+            page_size (Optional[int], optional): Number of results per page. Defaults to None.
+            sort_direction (Optional[PyarrSortDirection], optional): Direction to sort. Defaults to None.
+            sort_key (Optional[RadarrSortKey], optional): Field to sort. Defaults to None.
+            include_unknown_movie_items (Optional[bool], optional): Include unknown movie items. Defaults to None.
+
+        Returns:
+            JsonObject: List of dictionaries with items
+        """
+        params: dict[str, Union[int, PyarrSortDirection, RadarrSortKey, bool]] = {}
+
+        if page:
+            params["page"] = page
+        if page_size:
+            params["pageSize"] = page_size
+        if sort_key and sort_dir:
+            params["sortKey"] = sort_key
+            params["sortDirection"] = sort_dir
+        elif sort_key or sort_dir:
+            raise PyarrMissingArgument("sort_key and sort_dir  must be used together")
+        if include_unknown_movie_items is not None:
+            params["includeUnknownMovieItems"] = include_unknown_movie_items
 
-    # PUT /author/{id}
-    def upd_author(self, id_: int, data: dict[str, Any]) -> dict[str, Any]:
-        """Update the given author, currently only monitored is changed, all other modifications are ignored.
+        return self._get("queue", self.ver_uri, params)
 
-        Note:
-            To be used in conjunction with get_author()
+    # GET /queue/details
+    def get_queue_details(
+        self,
+        id_: Optional[int] = None,
+        include_movie: Optional[bool] = None,
+    ) -> JsonArray:
+        """Get details of all items in queue
 
         Args:
-            id_ (int): Author database ID to update
-            data (dict[str, Any]): All parameters to update author
+            id_ (Optional[int], optional): select specific item by id. Defaults to None
+            include_movie (Optional[bool], optional): Include movie object if linked. Defaults to None.
 
         Returns:
-            dict[str, Any]: Dictionary with updated record
+            JsonArray: List of dictionaries with items
         """
-        return self._put(f"author/{id_}", self.ver_uri, data=data)
+        params = {}
+        if id_:
+            params["movieId"] = id_
+        if include_movie is not None:
+            params["includeMovie"] = include_movie
+
+        return self._get("queue/details", self.ver_uri, params)
 
-    # DELETE /author/{id}
-    def del_author(
-        self, id_: int, delete_files: bool = False, import_list_exclusion: bool = True
-    ) -> Union[Response, dict[str, Any], dict[Any, Any]]:
-        """Delete the author with the given ID
+    # GET /queue/status
+    def get_queue_status(self) -> JsonObject:
+        """Queue item status
+
+        Returns:
+            JsonArray: List of dictionaries with items
+        """
+        return self._get("queue/status", self.ver_uri)
+
+    # DELETE /queue/bulk
+    def del_queue_bulk(
+        self,
+        id_: list[int],
+        remove_from_client: Optional[bool] = None,
+        blocklist: Optional[bool] = None,
+    ) -> Union[Response, JsonObject, dict[Any, Any]]:
+        """Remove multiple items from queue by their IDs
 
         Args:
-            id_ (int): Database ID for author
-            delete_files (bool, optional): If true author folder and files will be deleted. Defaults to False.
-            import_list_exclusion (bool, optional): Add an exclusion so author doesn't get re-added. Defaults to True.
+            id_ (list[int]): Dictionary of IDs to be removed::
+            remove_from_client (bool, optional): Remove the items from the client. Defaults to True.
+            blocklist (bool, optional): Add the items to the blocklist. Defaults to True.
 
         Returns:
             Response: HTTP Response
         """
-        params = {
-            "deleteFiles": delete_files,
-            "addImportListExclusion": import_list_exclusion,
-        }
-        return self._delete(f"author/{id_}", self.ver_uri, params=params)
+        data = {"ids": id_}
+        params = {"removeFromClient": remove_from_client, "blocklist": blocklist}
+        return self._delete("queue/bulk", self.ver_uri, params=params, data=data)
 
-    ## LOG
+    # POST /queue/grab/{id}
+    def force_grab_queue_item(self, id_: int) -> JsonObject:
+        """Perform a Radarr "force grab" on a pending queue item by its ID.
 
-    # GET /log/file
-    def get_log_file(self) -> list[dict[str, Any]]:
-        """Get log file
+        Args:
+            id_ (int): Queue item ID from database.
 
         Returns:
-            list[dict[str, Any]]: List of dictionaries with items
+            JsonObject: Dictionary with record
         """
-        return self.assert_return("log/file", self.ver_uri, list)
+        return self._post(f"queue/grab/{id_}", self.ver_uri)
 
-    # CONFIG
+    ## COMMAND
 
-    # POST /rootFolder/
-    def add_root_folder(
-        self,
-        name: str,
-        directory: str,
-        is_calibre_lib: bool = False,
-        calibre_host: str = "localhost",
-        calibre_port: int = 8080,
-        use_ssl: bool = False,
-        output_profile: str = "default",
-        default_tags: Union[list, None] = None,
-        default_quality_profile_id: int = 1,
-        default_metadata_profile_id: int = 1,
-    ) -> dict[str, Any]:
-        """Add a new root directory to the Readarr Server
-
-        Args:
-            name (str): Friendly Name for folder
-            directory (str): Directory to use e.g. /books/
-            is_calibre_lib (bool, optional): Use Calibre Content Server. Defaults to False.
-            calibre_host (str, optional): Calibre Content Server address. Defaults to "localhost".
-            calibre_port (int, optional): Calibre Content Server port. Defaults to 8080.
-            use_ssl (bool, optional): Calibre Content Server SSL. Defaults to False.
-            output_profile (str, optional): Books to monitor. Defaults to "default".
-            default_tags (Union[list, None], optional): List of tags to apply. Defaults to None.
-            default_quality_profile_id (int, optional): Quality Profile. Defaults to 1.
-            default_metadata_profile_id (int, optional): Metadata Profile. Defaults to 1.
-
-        Returns:
-            dict[str, Any]: Dictionary of added record
-        """
-        folder_json = {
-            "isCalibreLibrary": is_calibre_lib,
-            "host": calibre_host,
-            "port": calibre_port,
-            "useSsl": use_ssl,
-            "outputProfile": output_profile,
-            "defaultTags": default_tags or [],
-            "defaultQualityProfileId": default_quality_profile_id,
-            "defaultMetadataProfileId": default_metadata_profile_id,
+    # POST /command
+    def post_command(
+        self, name: RadarrCommands, **kwargs: Optional[dict[str, Union[int, list[int]]]]
+    ) -> JsonObject:
+        """Performs any of the predetermined Radarr command routines.
+
+        Args:
+            name (RadarrCommands): Command that should be executed
+            **kwargs: Additional parameters for specific commands. See note.
+
+        Note:
+            For available commands and required `**kwargs` see the `RadarrCommands` model
+
+
+        Returns:
+            JsonObject: Dictionary containing job
+        """
+        data: dict[str, Any] = {
             "name": name,
-            "path": directory,
         }
-        return self._post("rootFolder", self.ver_uri, data=folder_json)
+        if kwargs:
+            data |= kwargs
+        return self._post("command", self.ver_uri, data=data)
+
+    ## CUSTOM FILTERS
+
+    # GET /customfilter
+    def get_custom_filter(self) -> JsonArray:
+        """Query Radarr for custom filters
+
+        Returns:
+            JsonArray: List of dictionaries with items
+        """
+        return self._get("customfilter", self.ver_uri)
+
+    # POST /qualityprofile
+    def add_quality_profile(
+        self, name: str, upgrades_allowed: bool, cutoff: int, items: list
+    ) -> JsonObject:
+        """Add new quality profile
 
-    # GET /config/metadataProvider
-    def get_metadata_provider(self) -> dict[str, Any]:
-        """Get metadata provider from settings/metadata
+        Args:
+            name (str): Name of the profile
+            upgrades_allowed (bool): Are upgrades in quality allowed?
+            cutoff (int): ID of quality definition to cutoff at. Must be an allowed definition ID.
+            items (list): Add a list of items (from `get_quality_definition()`)
 
         Returns:
-            dict[str, Any]: Dictionary of record
+            JsonObject: An object containing the profile
         """
-        return self.assert_return("config/metadataProvider", self.ver_uri, dict)
+        data = {
+            "name": name,
+            "upgradeAllowed": upgrades_allowed,
+            "cutoff": cutoff,
+            "items": items,
+        }
+        return self._post("qualityprofile", self.ver_uri, data=data)
 
-    # PUT /config/metadataProvider
-    def upd_metadata_provider(self, data: dict[str, Any]) -> dict[str, Any]:
-        """Update the metadata provider data.
+    # GET /manualimport
+    def get_manual_import(
+        self,
+        folder: str,
+        download_id: Optional[str] = None,
+        movie_id: Optional[int] = None,
+        filter_existing_files: Optional[bool] = None,
+        replace_existing_files: Optional[bool] = None,
+    ) -> JsonArray:
+        """Gets a manual import list
+
+        Args:
+            downloadId (str): Download IDs
+            movieId (int, optional): Movie Database ID. Defaults to None.
+            folder (Optional[str], optional): folder name. Defaults to None.
+            filterExistingFiles (bool, optional): filter files. Defaults to True.
+            replaceExistingFiles (bool, optional): replace files. Defaults to True.
+
+        Returns:
+            JsonArray: List of dictionaries with items
+        """
+        params: dict[str, Union[str, int, bool]] = {"folder": folder}
+        if download_id:
+            params["downloadId"] = download_id
+        if movie_id:
+            params["movieId"] = movie_id
+        if filter_existing_files:
+            params["filterExistingFiles"] = filter_existing_files
+        if replace_existing_files:
+            params["replaceExistingFiles"] = replace_existing_files
+
+        return self._get("manualimport", self.ver_uri, params=params)
+
+    # PUT /manualimport
+    def upd_manual_import(self, data: JsonObject) -> JsonObject:
+        """Update a manual import
 
         Note:
-            To be used in conjunction with get_metadata_provider()
+            To be used in conjunction with get_manual_import()
 
         Args:
-            data (dict[str, Any]): All parameters to update
+            data (JsonObject): Data containing changes
 
         Returns:
-            dict[str, Any]: Dictionary of updated record
+            JsonObject: Dictionary of updated record
         """
-        return self._put("config/metadataProvider", self.ver_uri, data=data)
+        return self._put("manualimport", self.ver_uri, data=data)
```

### Comparing `pyarr-4.1.0/pyarr/request_handler.py` & `pyarr-5.0.0/pyarr/request_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-from typing import Any, Union
+from typing import Any, Optional, Union
 
 import requests
 from requests import Response
 from requests.auth import HTTPBasicAuth
 
 from .exceptions import (
     PyarrAccessRestricted,
     PyarrBadGateway,
+    PyarrBadRequest,
     PyarrConnectionError,
     PyarrMethodNotAllowed,
     PyarrResourceNotFound,
     PyarrUnauthorizedError,
 )
+from .types import _ReturnType
 
 
 class RequestHandler:
     """Base class for API Wrappers"""
 
     def __init__(
         self,
@@ -24,15 +26,15 @@
     ):
         """Constructor for connection to Arr API
 
         Args:
             host_url (str): Host URL to Arr api
             api_key (str): API Key for Arr api
         """
-        self.host_url = host_url
+        self.host_url = host_url.rstrip("/")
         self.api_key = api_key
         self.session: requests.Session = requests.Session()
         self.auth: Union[HTTPBasicAuth, None] = None
 
     def _request_url(self, path: str, ver_uri: str) -> str:
         """Builds the URL for the request to use.
 
@@ -58,16 +60,16 @@
         """
         return HTTPBasicAuth(username, password)
 
     def _get(
         self,
         path: str,
         ver_uri: str = "",
-        params: Union[dict[int, list[int]], dict, None] = None,
-    ) -> Union[list[dict], dict[str, Any]]:
+        params: Union[dict[str, Any], list[tuple[str, Any]], None] = None,
+    ) -> _ReturnType:
         """Wrapper on any get requests
 
         Args:
             path (str): Path to API endpoint e.g. /api/manualimport
             params (dict, optional): URL Parameters to send with the request. Defaults to None.
 
         Returns:
@@ -82,27 +84,23 @@
                 auth=self.auth,
             )
         except requests.Timeout as exception:
             raise PyarrConnectionError(
                 "Timeout occurred while connecting to API."
             ) from exception
         response = _process_response(res)
-        if isinstance(response, dict):
-            assert isinstance(response, dict)
-        else:
-            assert isinstance(response, list)
-        return response
+        return self._return(res, dict if isinstance(response, dict) else list)
 
     def _post(
         self,
         path: str,
         ver_uri: str = "",
         params: Union[dict, None] = None,
         data: Union[list[dict], dict, None] = None,
-    ) -> dict[str, Any]:
+    ) -> _ReturnType:
         """Wrapper on any post requests
 
         Args:
             path (str): Path to API endpoint e.g. /api/manualimport
             params (dict, optional): URL Parameters to send with the request. Defaults to None.
             data (dict, optional): Payload to send with request. Defaults to None.
 
@@ -114,31 +112,34 @@
             res = self.session.post(
                 self._request_url(path, ver_uri),
                 headers=headers,
                 params=params,
                 json=data,
                 auth=self.auth,
             )
+
         except requests.Timeout as exception:
             raise PyarrConnectionError(
                 "Timeout occurred while connecting to API."
             ) from exception
-        return self._return(res, dict)
+        response = _process_response(res)
+        return self._return(res, dict if isinstance(response, dict) else list)
 
     def _put(
         self,
         path: str,
-        ver_uri: str = "",
-        params: Union[dict, None] = None,
-        data: Union[dict, None] = None,
-    ) -> dict[str, Any]:
+        ver_uri: str,
+        params: Optional[dict] = None,
+        data: Optional[Union[dict[str, Any], list[dict[str, Any]]]] = None,
+    ) -> _ReturnType:
         """Wrapper on any put requests
 
         Args:
             path (str): Path to API endpoint e.g. /api/manualimport
+            ver_uri (str): API Version
             params (dict, optional): URL Parameters to send with the request. Defaults to None.
             data (dict, optional): Payload to send with request. Defaults to None.
 
         Returns:
             Object: Response object from requests
         """
         headers = {"X-Api-Key": self.api_key}
@@ -150,15 +151,17 @@
                 json=data,
                 auth=self.auth,
             )
         except requests.Timeout as exception:
             raise PyarrConnectionError(
                 "Timeout occurred while connecting to API."
             ) from exception
-        return self._return(res, dict)
+
+        response = _process_response(res)
+        return self._return(res, dict if isinstance(response, dict) else list)
 
     def _delete(
         self,
         path: str,
         ver_uri: str = "",
         params: Union[dict, None] = None,
         data: Union[dict, None] = None,
@@ -221,14 +224,17 @@
         PyarrAccessRestricted: Invalid Permissions
         PyarrResourceNotFound: Incorrect Resource
         PyarrBadGateway: Bad Gateway
 
     Returns:
         JSON: Array
     """
+    if res.status_code == 400:
+        raise PyarrBadRequest(f"Bad Request, possibly a bug. {str(res.content)}")
+
     if res.status_code == 401:
         raise PyarrUnauthorizedError(
             "Unauthorized. Please ensure valid API Key is used.", {}
         )
     if res.status_code == 403:
         raise PyarrAccessRestricted(
             "Access restricted. Please ensure API Key has correct permissions", {}
```

### Comparing `pyarr-4.1.0/pyproject.toml` & `pyarr-5.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyarr"
-version = "4.1.0"
+version = "5.0.0"
 description = "Synchronous Sonarr, Radarr, Lidarr and Readarr API's for Python"
 authors = ["Steven Marks <marksie1988@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["sonarr", "radarr", "readarr", "lidarr", "api", "wrapper", "plex"]
 homepage = "https://github.com/totaldebug/pyarr"
 repository = "https://github.com/totaldebug/pyarr"
@@ -14,52 +14,67 @@
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 packages = [
     {include = "pyarr"},
     {include = "pyarr/py.typed"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-requests = "^2.21.0"
-types-requests = "^2.25.11"
-
-[tool.poetry.dev-dependencies]
-black = {version = "^22.3", allow-prereleases = true}
-flake8 = "^3.8.4"
-isort = "^5.10.0"
+requests = "^2.28.2"
+types-requests = "^2.28.11.17"
+overrides = "^7.3.1"
+
+[tool.poetry.group.dev.dependencies]
+black = {version = "^22.12.0", allow-prereleases = true}
+flake8 = "^3.9.2"
+isort = "^5.12.0"
 mypy = "^0.910"
-pre-commit = "^2.15.0"
+pre-commit = "^2.21.0"
 interrogate = "^1.5.0"
-Sphinx = "^4.3.2"
-sphinx-argparse = "^0.3.1"
+Sphinx = "^4.5.0"
+sphinx-argparse = "^0.3.2"
 sphinx-autobuild = "^2021.3.14"
-sphinx-rtd-theme = "^1.0.0"
+sphinx-rtd-theme = "^1.2.0"
+pytest = "^7.2.2"
+pytest-cov = "^3.0.0"
+pylint = "^2.17.1"
+responses = "^0.21.0"
+autoflake = "^1.7.8"
+ipykernel = "^6.22.0"
+sphinx-toolbox = "^3.4.0"
+enum-tools = "^0.9.0.post1"
+pytest-rerunfailures = "^11.1.2"
+nox = "^2022.11.21"
+toml = "^0.10.2"
 
 [tool.black]
 line-length = 88
 target_version = ['py39']
 include = '\.pyi?$'
 exclude = '''
 
 (
   /(
       \.eggs         # exclude a few common directories in the
     | \.git          # root of the project
     | \.hg
     | \.mypy_cache
     | \.tox
+    | \.nox
     | \.venv
+    | \.cache
     | _build
     | buck-out
     | build
     | dist
   )/
 )
 '''
@@ -80,30 +95,37 @@
 known_first_party = [
     "pyarr",
     "tests",
 ]
 forced_separate = [
     "tests",
 ]
+skip = [".cache", ".nox"]
 combine_as_imports = true
 
+[tool.autoflake]
+check = true
+remove-unused-variables = true
+remove-all-unused-imports = true
+remove-duplicate-keys = true
+
 [tool.interrogate]
 ignore-init-method = true
 ignore-init-module = false
 ignore-magic = false
 ignore-semiprivate = false
 ignore-private = false
 ignore-property-decorators = false
 ignore-module = true
 ignore-nested-functions = false
 ignore-nested-classes = true
 ignore-setters = false
 fail-under = 100
-exclude = ["setup.py", "sphinx-docs", "build", ".devcontainer"]
+exclude = ["setup.py", "sphinx-docs", "build", ".devcontainer", ".nox", ".cache"]
 ignore-regex = ["^get$", "^mock_.*", ".*BaseClass.*"]
 verbose = 0
 quiet = false
 color = true
 
 [build-system]
-requires = ["poetry>=0.12"]
+requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.masonry.api"
```

