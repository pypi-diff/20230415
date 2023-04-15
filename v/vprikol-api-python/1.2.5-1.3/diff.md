# Comparing `tmp/vprikol_api_python-1.2.5.tar.gz` & `tmp/vprikol_api_python-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vprikol_api_python-1.2.5.tar", max compression
+gzip compressed data, was "vprikol_api_python-1.3.tar", max compression
```

## Comparing `vprikol_api_python-1.2.5.tar` & `vprikol_api_python-1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       32 2023-04-03 19:07:58.939689 vprikol_api_python-1.2.5/README.md
--rw-r--r--   0        0        0      351 2023-04-03 19:07:58.939689 vprikol_api_python-1.2.5/pyproject.toml
--rw-r--r--   0        0        0       51 2023-04-03 19:07:58.939689 vprikol_api_python-1.2.5/vprikol_api/__init__.py
--rw-r--r--   0        0        0      921 2023-04-03 19:07:58.939689 vprikol_api_python-1.2.5/vprikol_api/api.py
--rw-r--r--   0        0        0     5229 2023-04-03 19:07:58.939689 vprikol_api_python-1.2.5/vprikol_api/main.py
--rw-r--r--   0        0        0     3719 2023-04-03 19:07:58.939689 vprikol_api_python-1.2.5/vprikol_api/model.py
--rw-r--r--   0        0        0      455 1970-01-01 00:00:00.000000 vprikol_api_python-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0       32 2023-04-15 14:42:42.724738 vprikol_api_python-1.3/README.md
+-rw-r--r--   0        0        0      349 2023-04-15 14:42:42.724738 vprikol_api_python-1.3/pyproject.toml
+-rw-r--r--   0        0        0       51 2023-04-15 14:42:42.724738 vprikol_api_python-1.3/vprikol_api/__init__.py
+-rw-r--r--   0        0        0      921 2023-04-15 14:42:42.724738 vprikol_api_python-1.3/vprikol_api/api.py
+-rw-r--r--   0        0        0     5567 2023-04-15 14:42:42.724738 vprikol_api_python-1.3/vprikol_api/main.py
+-rw-r--r--   0        0        0     3704 2023-04-15 14:42:42.724738 vprikol_api_python-1.3/vprikol_api/model.py
+-rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 vprikol_api_python-1.3/PKG-INFO
```

### Comparing `vprikol_api_python-1.2.5/vprikol_api/api.py` & `vprikol_api_python-1.3/vprikol_api/api.py`

 * *Files identical despite different names*

### Comparing `vprikol_api_python-1.2.5/vprikol_api/main.py` & `vprikol_api_python-1.3/vprikol_api/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,32 +22,37 @@
         result = await get(url=f'{self.base_url}ip', headers=self.headers, params={'ip': ip})
 
         if not result.success:
             raise Exception(result.error)
 
         return IpAPIResponse(**result.data)
 
-    async def get_members(self, server_id: int, fraction_id: int) -> MembersAPIResponse:
-        result = await get(url=f'{self.base_url}members', headers=self.headers, params={'server': server_id,
+    async def get_members(self, server_id: int, fraction_id: int | list[int]) -> dict[str, MembersAPIResponse]:
+        result = await get(url=f'{self.base_url}members', headers=self.headers, params={'server_id': server_id,
                                                                                         'fraction_id': fraction_id})
         if not result.success:
             raise Exception(result.error)
+        response = {}
+        for fraction_id in result.data:
+            players = []
+            if not fraction_id.isdigit():
+                continue
+            for player in result.data[fraction_id]['players']:
+                players.append({'username': player, 'id': result.data[fraction_id]['players'][player]['id'],
+                                'isOnline': result.data[fraction_id]['players'][player]['isOnline'],
+                                'isLeader': result.data[fraction_id]['players'][player]['isLeader'],
+                                'rank': result.data[fraction_id]['players'][player]['rank'],
+                                'rankLabel': result.data[fraction_id]['players'][player]['rankLabel']})
+            result.data[fraction_id]['players'] = players
+            response[fraction_id] = MembersAPIResponse(**result.data[fraction_id])
 
-        players = []
-        for player in result.data['players']:
-            players.append({'username': player, 'id': result.data['players'][player]['id'],
-                            'isOnline': result.data['players'][player]['isOnline'],
-                            'isLeader': result.data['players'][player]['isLeader'],
-                            'rank': result.data['players'][player]['rank'],
-                            'rankLabel': result.data['players'][player]['rankLabel']})
-        result.data['players'] = players
-        return MembersAPIResponse(**result.data)
+        return response
 
-    async def get_player_information(self, server_id: int, nickname: str) -> PlayerInfoRodinaAPIResponse\
-                                                                             | PlayerInfoArizonaAPIResponse\
+    async def get_player_information(self, server_id: int, nickname: str) -> PlayerInfoRodinaAPIResponse \
+                                                                             | PlayerInfoArizonaAPIResponse \
                                                                              | PlayerInfoNotFound:
         task = await post(url=f'{self.base_url}find/createTask', headers=self.headers,
                           params={'server': server_id, 'nick': nickname})
         if not task.success:
             raise Exception(task.error)
 
         task = CreatedFindTaskAPIResponse(**task.data)
```

### Comparing `vprikol_api_python-1.2.5/vprikol_api/model.py` & `vprikol_api_python-1.3/vprikol_api/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,23 +33,23 @@
     is_online: bool = Field(alias='isOnline')
     is_leader: bool = Field(alias='isLeader')
     rank: int
     rank_label: str | None = Field(alias='rankLabel')
 
 
 class MembersAPIResponse(BaseModel):
-    server: str
     fraction_label: str = Field(alias='fractionLabel')
     players: list[MembersAPIPlayer]
     total_players: int = Field(alias='totalPlayers')
     total_online: int = Field(alias='totalOnline')
     leader_nickname: str | None = Field(alias='leaderNick')
     is_leader_online: bool = Field(alias='isLeaderOnline')
 
 
+
 class ServerStatusAPIResponse(BaseModel):
     hostname: str
     payday_multiplier: int = Field(alias='paydayMultiplier')
     online_players: int = Field(alias='onlinePlayers')
     max_players: int = Field(alias='maxPlayers')
     is_closed: bool = Field(alias='isClosed')
     ip: str
```

