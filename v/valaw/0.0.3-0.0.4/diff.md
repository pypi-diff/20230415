# Comparing `tmp/valaw-0.0.3.tar.gz` & `tmp/valaw-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valaw-0.0.3.tar", last modified: Sat Apr  8 23:19:37 2023, max compression
+gzip compressed data, was "valaw-0.0.4.tar", last modified: Sat Apr 15 04:08:19 2023, max compression
```

## Comparing `valaw-0.0.3.tar` & `valaw-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 23:19:37.254421 valaw-0.0.3/
--rw-rw-rw-   0        0        0     1090 2023-04-04 04:45:45.000000 valaw-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1383 2023-04-08 23:19:37.251030 valaw-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      725 2023-04-06 23:58:20.000000 valaw-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-08 23:19:37.254421 valaw-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1118 2023-04-08 23:18:41.000000 valaw-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-08 23:19:37.157648 valaw-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-08 23:19:37.197668 valaw-0.0.3/src/valaw/
--rw-rw-rw-   0        0        0       73 2023-04-04 05:08:42.000000 valaw-0.0.3/src/valaw/__init__.py
--rw-rw-rw-   0        0        0    11240 2023-04-08 23:17:11.000000 valaw-0.0.3/src/valaw/client.py
-drwxrwxrwx   0        0        0        0 2023-04-08 23:19:37.246770 valaw-0.0.3/src/valaw.egg-info/
--rw-rw-rw-   0        0        0     1383 2023-04-08 23:19:37.000000 valaw-0.0.3/src/valaw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-04-08 23:19:37.000000 valaw-0.0.3/src/valaw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 23:19:37.000000 valaw-0.0.3/src/valaw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-04-08 23:19:37.000000 valaw-0.0.3/src/valaw.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-08 23:19:37.000000 valaw-0.0.3/src/valaw.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 04:08:19.275044 valaw-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2023-04-13 23:03:00.000000 valaw-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1895 2023-04-15 04:08:19.275044 valaw-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1212 2023-04-15 03:19:54.000000 valaw-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-15 04:08:19.276044 valaw-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1143 2023-04-15 03:57:53.000000 valaw-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 04:08:19.256621 valaw-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 04:08:19.262786 valaw-0.0.4/src/valaw/
+-rw-rw-rw-   0        0        0       73 2023-04-13 23:03:00.000000 valaw-0.0.4/src/valaw/__init__.py
+-rw-rw-rw-   0        0        0    13440 2023-04-15 03:43:20.000000 valaw-0.0.4/src/valaw/client.py
+drwxrwxrwx   0        0        0        0 2023-04-15 04:08:19.274044 valaw-0.0.4/src/valaw.egg-info/
+-rw-rw-rw-   0        0        0     1895 2023-04-15 04:08:19.000000 valaw-0.0.4/src/valaw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-04-15 04:08:19.000000 valaw-0.0.4/src/valaw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 04:08:19.000000 valaw-0.0.4/src/valaw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-04-15 04:08:19.000000 valaw-0.0.4/src/valaw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-15 04:08:19.000000 valaw-0.0.4/src/valaw.egg-info/top_level.txt
```

### Comparing `valaw-0.0.3/LICENSE` & `valaw-0.0.4/LICENSE`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `valaw-0.0.3/setup.py` & `valaw-0.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from setuptools import setup, find_namespace_packages
 
 with open("README.md", "r") as readme:
     long_desc = readme.read()
 
 setup(
     name="valaw",
-    version="0.0.3",
+    version="0.0.4",
     author="Jet612",
     description="An asynchronous API wrapper for VALORANT's API",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     url="https://github.com/Jet612/valaw",
     project_urls={
-        "Documentation": "https://github.com/Jet612/valaw/tree/main/docs",
+        "Documentation": "https://valaw.readthedocs.io",
         "Issue Tracker": "https://github.com/Jet612/valaw/issues",
         "Chat/Support": "https://discord.gg/mVXpvunBbF",
     },
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Development Status :: 4 - Beta",
+        "Intended Audience :: Developers"
     ],
     package_dir={"": "src"},
     packages=find_namespace_packages(where="src"),
     include_package_data=True,
     python_requires=">=3.8",
     install_requires=[
                     'aiohttp==3.8.3',
-                    'setuptools==65.5.0'
+                    'setuptools==67.6.0'
                     ]
 )
```

### Comparing `valaw-0.0.3/src/valaw/client.py` & `valaw-0.0.4/src/valaw/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -35,27 +35,28 @@
         # Checking if the arguments are valid
         if cluster.lower() not in clusters:
             raise Exceptions.InvalidCluster(f"Invalid cluster, valid clusters are: {clusters}.")
         
         self.token = token
         self.cluster = cluster
 
-        # Subclasses
-        self.account = Account(token, cluster)
-        self.content = Content(token, cluster)
-        self.match = Match(token, cluster)
-
         # Beta/Development message
         print("valaw: This library is still in development, please report any bugs to https://github.com/Jet612/valaw/issues.")
 
-class Account:
-    def __init__(self, token: str, cluster: str):
-        self.token = token
+    def change_cluster(self, cluster: str):
+        """Change the cluster."""
+
+        if cluster.lower() not in clusters:
+            raise Exceptions.InvalidCluster(f"Invalid cluster, valid clusters are: {clusters}.")
         self.cluster = cluster
 
+    ##################
+    ### ACCOUNT-V1 ###
+    ##################
+
     async def GET_getByPuuid(self, puuid: str, cluster: str = None) -> dict:
         """Get account by PUUID."""
 
         if cluster != None:
             if cluster.lower() not in clusters:
                 raise Exceptions.InvalidCluster(f"Invalid cluster, valid clusters are: {clusters}.")
         else:
@@ -129,18 +130,17 @@
                 "Accept-Charset": "application/x-www-form-urlencoded; charset=UTF-8",
                 "Origin": "https://developer.riotgames.com",
                 "X-Riot-Token": self.token
             }
             async with session.get(f"https://{cluster}.api.riotgames.com/riot/account/v1/active-shards/by-game/val/by-puuid/{puuid}", headers=headers) as resp:
                 return await verify_content(resp)
 
-class Content:
-    def __init__(self, token: str, cluster: str):
-        self.token = token
-        self.cluster = cluster
+    ######################
+    ### VAL-CONTENT-V1 ###
+    ######################
 
     async def GET_getContent(self, region: str, locale: str = "") -> dict:
         """Get content optionally filtered by locale. A locale is recommended to be used for faster response times."""
 
         if region.lower() not in regions:
             raise Exceptions.InvalidRegion(f"Invalid region, valid regions are: {regions}.")
 
@@ -155,19 +155,18 @@
                 "Accept-Language": "en-US,en;q=0.9",
                 "Accept-Charset": "application/x-www-form-urlencoded; charset=UTF-8",
                 "Origin": "https://developer.riotgames.com",
                 "X-Riot-Token": self.token
             }
             async with session.get(f"https://{region}.api.riotgames.com/val/content/v1/contents{locale}", headers=headers) as resp:
                 return await verify_content(resp)
-            
-class Match:
-    def __init__(self, token: str, cluster: str):
-        self.token = token
-        self.cluster = cluster
+
+    ####################
+    ### VAL-MATCH-V1 ###
+    #################### 
 
     async def GET_getMatch(self, matchId: str, region: str) -> dict:
         """Get match by id."""
 
         if region.lower() not in regions:
             raise Exceptions.InvalidRegion(f"Invalid region, valid regions are: {regions}.")
 
@@ -223,8 +222,53 @@
                 "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36",
                 "Accept-Language": "en-US,en;q=0.9",
                 "Accept-Charset": "application/x-www-form-urlencoded; charset=UTF-8",
                 "Origin": "https://developer.riotgames.com",
                 "X-Riot-Token": self.token
             }
             async with session.get(f"https://{region}.api.riotgames.com/val/match/v1/recent-matches/by-queue/{queue}", headers=headers) as resp:
+                return await verify_content(resp)
+    
+    #####################
+    ### VAL-RANKED-V1 ###
+    #####################
+
+    async def GET_getLeaderboard(self, actId: str, region: str, size: int = 200, startIndex: int = 0) -> dict:
+        """Get leaderboard for the competitive queue"""
+
+        if region.lower() not in regions:
+            raise Exceptions.InvalidRegion(f"Invalid region, valid regions are: {regions}.")
+        
+        if size > 200 or size < 1:
+            raise ValueError(f"Invalid size, valid values: 1 to 200.")
+        
+        async with aiohttp.ClientSession() as session:
+            headers = {
+                "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36",
+                "Accept-Language": "en-US,en;q=0.9",
+                "Accept-Charset": "application/x-www-form-urlencoded; charset=UTF-8",
+                "Origin": "https://developer.riotgames.com",
+                "X-Riot-Token": self.token
+            }
+            async with session.get(f"https://{region}.api.riotgames.com/val/ranked/v1/leaderboards/by-act/{actId}?size={size}&startIndex={startIndex}", headers=headers) as resp:
+                return await verify_content(resp)
+
+    #####################
+    ### VAL-STATUS-V1 ###
+    #####################
+
+    async def GET_getPlatformData(self, region: str) -> dict:
+        """Get VALORANT status for the given platform."""
+
+        if region.lower() not in regions:
+            raise Exceptions.InvalidRegion(f"Invalid region, valid regions are: {regions}.")
+
+        async with aiohttp.ClientSession() as session:
+            headers = {
+                "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36",
+                "Accept-Language": "en-US,en;q=0.9",
+                "Accept-Charset": "application/x-www-form-urlencoded; charset=UTF-8",
+                "Origin": "https://developer.riotgames.com",
+                "X-Riot-Token": self.token
+            }
+            async with session.get(f"https://{region}.api.riotgames.com/val/status/v1/platform-data", headers=headers) as resp:
                 return await verify_content(resp)
```

