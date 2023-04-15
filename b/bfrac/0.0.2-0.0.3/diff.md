# Comparing `tmp/bfrac-0.0.2.tar.gz` & `tmp/bfrac-0.0.3.tar.gz`

## Comparing `bfrac-0.0.2.tar` & `bfrac-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bfrac-0.0.2/example_config.ini
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 bfrac-0.0.2/bfrac/__about__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 bfrac-0.0.2/bfrac/__init__.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 bfrac-0.0.2/bfrac/app_config.py
--rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 bfrac-0.0.2/bfrac/riot_api_caller.py
--rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 bfrac-0.0.2/bfrac/riot_api_helper.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 bfrac-0.0.2/tests/context.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 bfrac-0.0.2/tests/simple_test.py
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 bfrac-0.0.2/tests/tester.ipynb
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 bfrac-0.0.2/.gitignore
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 bfrac-0.0.2/LICENSE
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 bfrac-0.0.2/README.md
--rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 bfrac-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 bfrac-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bfrac-0.0.3/example_config.ini
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 bfrac-0.0.3/bfrac/__about__.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 bfrac-0.0.3/bfrac/__init__.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 bfrac-0.0.3/bfrac/app_config.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 bfrac-0.0.3/bfrac/match_info_object.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 bfrac-0.0.3/bfrac/query_context.py
+-rw-r--r--   0        0        0    10302 2020-02-02 00:00:00.000000 bfrac-0.0.3/bfrac/riot_api_caller.py
+-rw-r--r--   0        0        0     4726 2020-02-02 00:00:00.000000 bfrac-0.0.3/bfrac/riot_api_helper.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 bfrac-0.0.3/tests/context.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 bfrac-0.0.3/tests/simple_test.py
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 bfrac-0.0.3/tests/tester.ipynb
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 bfrac-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 bfrac-0.0.3/LICENSE
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 bfrac-0.0.3/README.md
+-rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 bfrac-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 bfrac-0.0.3/PKG-INFO
```

### Comparing `bfrac-0.0.2/bfrac/app_config.py` & `bfrac-0.0.3/bfrac/app_config.py`

 * *Files identical despite different names*

### Comparing `bfrac-0.0.2/bfrac/riot_api_helper.py` & `bfrac-0.0.3/bfrac/riot_api_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 class RiotAPIHelper:
     """
     Helper class containing static methods for calling common riot api endpoints.
     """
-    lol_servers = ["br1", "eun1", "euw1", "jp1", "kr", "la1", "la2", "na1", "oc1", "ph2", "ru", "sg2", "th2", "tr1",
+    LOL_SERVERS = ["br1", "eun1", "euw1", "jp1", "kr", "la1", "la2", "na1", "oc1", "ph2", "ru", "sg2", "th2", "tr1",
                    "tw2", "vn2"]
-    lol_continents = ["americas", "asia", "europe", "sea"]
+    LOL_CONTINENTS = ["americas", "asia", "europe", "sea"]
+    LOL_SERVER_TO_CONTINENT = {"br1": "americas", "eun1": "europe", "euw1": "europe", "jp1": "asia", "kr": "asia",
+                               "la1": "americas", "la2": "americas", "na1": "americas", "oc1": "sea", "ph2": "sea",
+                               "ru": "europe", "sg2": "sea", "th2": "sea", "tr1": "europe", "tw2": "sea", "vn2": "sea"}
 
     """
     The AMERICAS routing value serves NA, BR, LAN and LAS.
     The ASIA routing value serves KR and JP.
     The EUROPE routing value serves EUNE, EUW, TR and RU.
     The SEA routing value serves OCE, PH2, SG2, TH2, TW2 and VN2.
     """
@@ -30,16 +33,16 @@
         return f"https://{in_region_continent}.api.riotgames.com/lol/match/v5/matches/{in_match_id}"
 
     @staticmethod
     def url_match_timeline(in_region_continent, in_match_id):
         return f"https://{in_region_continent}.api.riotgames.com/lol/match/v5/matches/{in_match_id}/timeline"
 
     @staticmethod
-    def get_summoner_by_name(in_riot_api_caller, in_region, in_summoner_name):
-        url = RiotAPIHelper.url_summoner_by_name(in_region, in_summoner_name)
+    def get_summoner_by_name(in_riot_api_caller, in_region_server, in_summoner_name):
+        url = RiotAPIHelper.url_summoner_by_name(in_region_server, in_summoner_name)
         return in_riot_api_caller.call_riot_api(url, {})
 
     @staticmethod
     def get_matches_list(in_riot_api_caller, in_region_continent, in_summoner_puuid, in_count,
                          in_type="", in_queue=None, in_start_time=0, in_end_time=0, in_start=0):
         """
```

### Comparing `bfrac-0.0.2/tests/tester.ipynb` & `bfrac-0.0.3/tests/tester.ipynb`

 * *Files identical despite different names*

### Comparing `bfrac-0.0.2/.gitignore` & `bfrac-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `bfrac-0.0.2/LICENSE` & `bfrac-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bfrac-0.0.2/pyproject.toml` & `bfrac-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bfrac-0.0.2/PKG-INFO` & `bfrac-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfrac
-Version: 0.0.2
+Version: 0.0.3
 Summary: Beginner Friendly Riot API Caller is a simple wrapper for RiotAPI with rate maintenance built in.
 Project-URL: Documentation, https://github.com/deamonpog/bfrac#readme
 Project-URL: Issues, https://github.com/deamonpog/bfrac/issues
 Project-URL: Source, https://github.com/deamonpog/bfrac
 Author-email: deamonpog <pog666@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

