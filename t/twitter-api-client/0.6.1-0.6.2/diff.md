# Comparing `tmp/twitter-api-client-0.6.1.tar.gz` & `tmp/twitter-api-client-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.6.1.tar", last modified: Thu Apr 13 01:52:02 2023, max compression
+gzip compressed data, was "twitter-api-client-0.6.2.tar", last modified: Sat Apr 15 00:46:23 2023, max compression
```

## Comparing `twitter-api-client-0.6.1.tar` & `twitter-api-client-0.6.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-13 01:52:02.526536 twitter-api-client-0.6.1/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-07 23:06:22.000000 twitter-api-client-0.6.1/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)     6125 2023-04-13 01:52:02.526536 twitter-api-client-0.6.1/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-04-13 01:52:02.526536 twitter-api-client-0.6.1/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)     7094 2023-04-13 01:51:56.000000 twitter-api-client-0.6.1/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-13 01:52:02.523536 twitter-api-client-0.6.1/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-07 23:06:22.000000 twitter-api-client-0.6.1/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    22979 2023-04-10 18:34:38.000000 twitter-api-client-0.6.1/twitter/account.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-13 01:52:02.525536 twitter-api-client-0.6.1/twitter/config/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-07 23:06:22.000000 twitter-api-client-0.6.1/twitter/config/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)      909 2023-04-07 23:06:22.000000 twitter-api-client-0.6.1/twitter/config/log.py
--rw-r--r--   0 x         (1000) x         (1000)   148071 2023-04-07 23:06:22.000000 twitter-api-client-0.6.1/twitter/config/operations.py
--rw-r--r--   0 x         (1000) x         (1000)     5858 2023-04-07 23:06:22.000000 twitter-api-client-0.6.1/twitter/config/settings.py
--rw-r--r--   0 x         (1000) x         (1000)     2456 2023-04-10 18:10:09.000000 twitter-api-client-0.6.1/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     5242 2023-04-10 19:10:29.000000 twitter-api-client-0.6.1/twitter/login.py
--rw-r--r--   0 x         (1000) x         (1000)    12761 2023-04-13 00:22:22.000000 twitter-api-client-0.6.1/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     5105 2023-04-12 03:42:43.000000 twitter-api-client-0.6.1/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     2235 2023-04-07 23:06:22.000000 twitter-api-client-0.6.1/twitter/utils.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-13 01:52:02.526536 twitter-api-client-0.6.1/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)     6125 2023-04-13 01:52:02.000000 twitter-api-client-0.6.1/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      461 2023-04-13 01:52:02.000000 twitter-api-client-0.6.1/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-04-13 01:52:02.000000 twitter-api-client-0.6.1/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       82 2023-04-13 01:52:02.000000 twitter-api-client-0.6.1/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-04-13 01:52:02.000000 twitter-api-client-0.6.1/twitter_api_client.egg-info/top_level.txt
+drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-04-15 00:46:23.662479 twitter-api-client-0.6.2/
+-rw-rw-r--   0 x         (1000) x         (1000)     1075 2023-04-14 02:53:18.000000 twitter-api-client-0.6.2/LICENSE
+-rw-rw-r--   0 x         (1000) x         (1000)     6238 2023-04-15 00:46:23.662479 twitter-api-client-0.6.2/PKG-INFO
+-rw-rw-r--   0 x         (1000) x         (1000)       38 2023-04-15 00:46:23.662479 twitter-api-client-0.6.2/setup.cfg
+-rw-rw-r--   0 x         (1000) x         (1000)     7220 2023-04-15 00:40:05.000000 twitter-api-client-0.6.2/setup.py
+drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-04-15 00:46:23.662479 twitter-api-client-0.6.2/twitter/
+-rw-rw-r--   0 x         (1000) x         (1000)        0 2023-04-14 02:53:18.000000 twitter-api-client-0.6.2/twitter/__init__.py
+-rw-rw-r--   0 x         (1000) x         (1000)    26558 2023-04-15 00:35:53.000000 twitter-api-client-0.6.2/twitter/account.py
+drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-04-15 00:46:23.662479 twitter-api-client-0.6.2/twitter/config/
+-rw-rw-r--   0 x         (1000) x         (1000)        0 2023-04-14 02:53:18.000000 twitter-api-client-0.6.2/twitter/config/__init__.py
+-rw-rw-r--   0 x         (1000) x         (1000)      909 2023-04-14 02:53:18.000000 twitter-api-client-0.6.2/twitter/config/log.py
+-rw-rw-r--   0 x         (1000) x         (1000)   147862 2023-04-14 21:16:39.000000 twitter-api-client-0.6.2/twitter/config/operations.py
+-rw-rw-r--   0 x         (1000) x         (1000)     5858 2023-04-14 02:53:18.000000 twitter-api-client-0.6.2/twitter/config/settings.py
+-rw-rw-r--   0 x         (1000) x         (1000)     2539 2023-04-14 21:53:11.000000 twitter-api-client-0.6.2/twitter/constants.py
+-rw-rw-r--   0 x         (1000) x         (1000)     5242 2023-04-14 02:53:18.000000 twitter-api-client-0.6.2/twitter/login.py
+-rw-rw-r--   0 x         (1000) x         (1000)    12761 2023-04-14 02:53:18.000000 twitter-api-client-0.6.2/twitter/scraper.py
+-rw-rw-r--   0 x         (1000) x         (1000)     5105 2023-04-14 02:53:18.000000 twitter-api-client-0.6.2/twitter/search.py
+-rw-rw-r--   0 x         (1000) x         (1000)     2235 2023-04-14 02:53:18.000000 twitter-api-client-0.6.2/twitter/utils.py
+drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-04-15 00:46:23.662479 twitter-api-client-0.6.2/twitter_api_client.egg-info/
+-rw-rw-r--   0 x         (1000) x         (1000)     6238 2023-04-15 00:46:23.000000 twitter-api-client-0.6.2/twitter_api_client.egg-info/PKG-INFO
+-rw-rw-r--   0 x         (1000) x         (1000)      461 2023-04-15 00:46:23.000000 twitter-api-client-0.6.2/twitter_api_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 x         (1000) x         (1000)        1 2023-04-15 00:46:23.000000 twitter-api-client-0.6.2/twitter_api_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 x         (1000) x         (1000)       82 2023-04-15 00:46:23.000000 twitter-api-client-0.6.2/twitter_api_client.egg-info/requires.txt
+-rw-rw-r--   0 x         (1000) x         (1000)        8 2023-04-15 00:46:23.000000 twitter-api-client-0.6.2/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.6.1/LICENSE` & `twitter-api-client-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.1/PKG-INFO` & `twitter-api-client-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.6.1
+Version: 0.6.2
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
@@ -91,14 +91,18 @@
 
  # refresh all pinned lists in this order
  account.update_pinned_lists([543, 432, 321])
 
  # unpin all lists
  account.update_pinned_lists([])
 
+ # get timelines
+ timeline = account.home_timeline()
+ latest_timeline = account.home_latest_timeline(limit=100)
+
  # example configuration
  account.update_settings({
      "address_book_live_sync_enabled": False,
      "allow_ads_personalization": False,
      "allow_authenticated_periscope_requests": True,
      "allow_dm_groups_from": "following",
      "allow_dms_from": "following",
```

### Comparing `twitter-api-client-0.6.1/setup.py` & `twitter-api-client-0.6.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.6.1",
+    version="0.6.2",
     python_requires=">=3.11.0",
     description="Twitter API",
     long_description=dedent('''
     Complete implementation of the undocumented Twitter API
     
     Includes tools to **scrape**, **automate**, and **search** twitter
     
@@ -97,14 +97,18 @@
     
     # refresh all pinned lists in this order
     account.update_pinned_lists([543, 432, 321])
     
     # unpin all lists
     account.update_pinned_lists([])
     
+    # get timelines
+    timeline = account.home_timeline()
+    latest_timeline = account.home_latest_timeline(limit=100)
+    
     # example configuration
     account.update_settings({
         "address_book_live_sync_enabled": False,
         "allow_ads_personalization": False,
         "allow_authenticated_periscope_requests": True,
         "allow_dm_groups_from": "following",
         "allow_dms_from": "following",
```

### Comparing `twitter-api-client-0.6.1/twitter/account.py` & `twitter-api-client-0.6.2/twitter/account.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from datetime import datetime
 from functools import wraps, partial
 from pathlib import Path
 from urllib.parse import urlencode
 from uuid import uuid1, getnode
 
 import orjson
-from requests import Response
+from requests import Response, Session
 from tqdm import tqdm
 
 from .config.log import log_config
 from .config.operations import operations
 from .config.settings import *
 from .constants import *
 from .login import login
@@ -39,14 +39,17 @@
     asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
 else:
     asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
 
 logging.config.dictConfig(log_config)
 logger = logging.getLogger(__name__)
 
+ID = 'ID'
+DUP_LIMIT = 5
+
 
 def log(fn=None, *, level: int = logging.DEBUG, info: list = None) -> callable:
     if fn is None:
         return partial(log, level=level, info=info)
 
     @wraps(fn)
     def wrapper(*args, **kwargs):
@@ -58,17 +61,26 @@
 
         limits = {k: v for k, v in r.headers.items() if 'x-rate-limit' in k}
         current_time = int(time.time())
         wait = int(r.headers.get('x-rate-limit-reset', current_time)) - current_time
         logger.log(level, f'{wait // 60} minutes until rate-limit reset. {limits = }')
 
         try:
+            data = {}
             if 200 <= r.status_code < 300:
-                typenames = find_key(r.json(), '__typename')
+                if 'json' in r.headers.get('content-type', ''):
+                    data = r.json()
+                    if data.get('errors'):
+                        logger.log(level, f'[{ERROR}error{RESET}] ({fn.__name__}) {args_info} {r.status_code} {r.text}')
+                        return r
+
+                typenames = find_key(data, '__typename')
+                logger.log(level, f'{typenames = }')
                 errors = ','.join([t for t in typenames if re.search('fail|error', t, flags=re.I)])
+
                 if errors:
                     message = f'[{ERROR}error{RESET}] {r.status_code} ({BOLD}{fn.__name__}{RESET}) {args_info} {WARN}{errors}{RESET}'
                 else:
                     message = f'[{SUCCESS}success{RESET}] {r.status_code} ({BOLD}{fn.__name__}{RESET}) {args_info}'
 
                 if info:
                     for k in info:
@@ -327,14 +339,87 @@
         return self.gql(Operation.Account.CreateBookmark, {'tweet_id': tweet_id})
 
     @log(info=['json'])
     def unbookmark(self, tweet_id: int) -> Response:
         return self.gql(Operation.Account.DeleteBookmark, {'tweet_id': tweet_id})
 
     @log(info=['json'])
+    def home_timeline(self):
+        return self.gql(Operation.Account.HomeTimeline, {})
+
+    def home_latest_timeline(self, limit: int = 100):
+        r = self.gql(Operation.Account.HomeLatestTimeline, {})
+        data = r.json() | {ID: self.session.cookies.get('username')}
+        return self.paginate(self.session, data, Operation.Account.HomeTimeline, limit)
+
+    # todo: a lot of duplicated code here, will need to refactor
+    def paginate(self, session: Session, data: dict, operation: tuple, limit: int):
+
+        def get_cursor(data):
+            # inefficient, but need to deal with arbitrary schema
+            entries = find_key(data, 'entries')
+            if entries:
+                for entry in entries.pop():
+                    if entry.get('entryId', '').startswith('cursor-bottom'):
+                        content = entry['content']
+                        if itemContent := content.get('itemContent'):
+                            return itemContent['value']  # v2 cursor
+                        return content['value']  # v1 cursor
+
+        all_data = []
+        try:
+            name, key = operation
+            params = deepcopy(operations[name])
+            ids = set()
+            counts = []
+            # params['variables'][key] = data[ID]
+            cursor = get_cursor(data)
+            while 1:
+                params['variables']['cursor'] = cursor
+
+                r = self.gql(operation, params['variables'])
+                _data = r.json()
+
+                if csrf := r.cookies.get("ct0"):
+                    session.headers.update({"x-csrf-token": csrf.value})
+                session.cookies.update(r.cookies)
+
+                path = Path(f'data/raw/{data[ID]}')
+                path.mkdir(parents=True, exist_ok=True)
+                (path / f'{time.time_ns()}_{name}.json').write_text(
+                    orjson.dumps(_data, option=orjson.OPT_INDENT_2).decode(),
+                    encoding='utf-8'
+                )
+
+                all_data.append(_data)
+                cursor = get_cursor(_data)
+                logger.debug(f'{cursor = }')
+                ids |= set(find_key(_data, 'rest_id'))
+                logger.debug(f'({data[ID]})\t{len(ids)} unique results')
+                counts.append(len(ids))
+
+                success_message = f'[{SUCCESS}success{RESET}] done pagination'
+                # followers/following have "0|"
+                if not cursor or cursor.startswith('0|'):
+                    logger.debug(f'{success_message}\tlast cursor: {cursor}')
+                    break
+                if len(ids) >= limit:
+                    logger.debug(f'{success_message}\tsurpassed limit of {limit} results')
+                    break
+                # did last 5 requests return duplicate data?
+                if len(counts) > DUP_LIMIT and len(set(counts[-1:-DUP_LIMIT:-1])) == 1:
+                    logger.debug(f'{success_message}\tpast {DUP_LIMIT} requests returned duplicate data')
+                    break
+
+        except Exception as e:
+            logger.debug(f'[{ERROR}error{RESET}] paginate falied: {e}')
+        # save_data(all_data, name)
+        return all_data
+
+    @log(info=['json'])
     def create_list(self, name: str, description: str, private: bool) -> Response:
         variables = {
             "isPrivate": private,
             "name": name,
             "description": description,
         }
         return self.gql(Operation.Account.CreateList, variables)
```

### Comparing `twitter-api-client-0.6.1/twitter/config/log.py` & `twitter-api-client-0.6.2/twitter/config/log.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.1/twitter/config/operations.py` & `twitter-api-client-0.6.2/twitter/config/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1437,47 +1437,43 @@
             "interactive_text_enabled": True,
             "responsive_web_text_conversations_enabled": True,
             "longform_notetweets_richtext_consumption_enabled": True,
             "responsive_web_enhance_cards_enabled": True
         }
     },
     "HomeTimeline": {
-        "queryId": "u5XGoPEa9-Hb30zpGz3Yrg",
-        "variables": {
-            "count": 1000,
-            "includePromotedContent": True,
-            "latestControlAvailable": True,
-            "requestContext": "launch",
-            "withCommunity": True,
-            "withSuperFollowsUserFields": True,
-            "withDownvotePerspective": False,
-            "withReactionsMetadata": False,
-            "withReactionsPerspective": False,
-            "withSuperFollowsTweetFields": True
+        'queryId': 'HCosKfLNW1AcOo3la3mMgg',
+        'variables': {
+            'count': 1000,
+            'includePromotedContent': True,
+            'latestControlAvailable': True,
+            'requestContext': 'launch',
+            'withCommunity': True,
+            # 'seenTweetIds': [],
         },
-        "features": {
-            "responsive_web_twitter_blue_verified_badge_is_enabled": True,
-            "responsive_web_graphql_exclude_directive_enabled": True,
-            "verified_phone_label_enabled": True,
-            "responsive_web_graphql_timeline_navigation_enabled": True,
-            "responsive_web_graphql_skip_user_profile_image_extensions_enabled": True,
-            "tweetypie_unmention_optimization_enabled": True,
-            "vibe_api_enabled": True,
-            "responsive_web_edit_tweet_api_enabled": True,
-            "graphql_is_translatable_rweb_tweet_is_translatable_enabled": True,
-            "view_counts_everywhere_api_enabled": True,
-            "longform_notetweets_consumption_enabled": True,
-            "tweet_awards_web_tipping_enabled": True,
-            "freedom_of_speech_not_reach_fetch_enabled": True,
-            "standardized_nudges_misinfo": True,
-            "tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled": True,
-            "interactive_text_enabled": True,
-            "responsive_web_text_conversations_enabled": True,
-            "longform_notetweets_richtext_consumption_enabled": True,
-            "responsive_web_enhance_cards_enabled": True
+        'features': {
+            'blue_business_profile_image_shape_enabled': True,
+            'responsive_web_graphql_exclude_directive_enabled': True,
+            'verified_phone_label_enabled': False,
+            'responsive_web_graphql_timeline_navigation_enabled': True,
+            'responsive_web_graphql_skip_user_profile_image_extensions_enabled': False,
+            'tweetypie_unmention_optimization_enabled': True,
+            'vibe_api_enabled': True,
+            'responsive_web_edit_tweet_api_enabled': True,
+            'graphql_is_translatable_rweb_tweet_is_translatable_enabled': True,
+            'view_counts_everywhere_api_enabled': True,
+            'longform_notetweets_consumption_enabled': True,
+            'tweet_awards_web_tipping_enabled': False,
+            'freedom_of_speech_not_reach_fetch_enabled': False,
+            'standardized_nudges_misinfo': True,
+            'tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled': False,
+            'interactive_text_enabled': True,
+            'responsive_web_text_conversations_enabled': False,
+            'longform_notetweets_rich_text_read_enabled': True,
+            'responsive_web_enhance_cards_enabled': False,
         }
     },
     "ImmersiveMedia": {
         "queryId": "7P_Y2m7_NkEnge7eCeW-cw",
         "variables": {},
         "features": {
             "responsive_web_twitter_blue_verified_badge_is_enabled": True,
```

### Comparing `twitter-api-client-0.6.1/twitter/config/settings.py` & `twitter-api-client-0.6.2/twitter/config/settings.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.1/twitter/constants.py` & `twitter-api-client-0.6.2/twitter/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,17 @@
         UserByScreenName = Value('screen_name')
         UserByRestId = Value('userId')
         # batch-user
         UsersByRestIds = Value('userIds')
 
     # @member
     class Account(Enum):
+        # user
+        HomeTimeline = Value()
+        HomeLatestTimeline = Value()
         # tweet
         CreateTweet = Value()
         CreateScheduledTweet = Value()
         DeleteScheduledTweet = Value()
         FetchScheduledTweets = Value()
         DeleteTweet = Value()
         FavoriteTweet = Value()
```

### Comparing `twitter-api-client-0.6.1/twitter/login.py` & `twitter-api-client-0.6.2/twitter/login.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.1/twitter/scraper.py` & `twitter-api-client-0.6.2/twitter/scraper.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.1/twitter/search.py` & `twitter-api-client-0.6.2/twitter/search.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.1/twitter/utils.py` & `twitter-api-client-0.6.2/twitter/utils.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.1/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.6.2/twitter_api_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.6.1
+Version: 0.6.2
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
@@ -91,14 +91,18 @@
 
  # refresh all pinned lists in this order
  account.update_pinned_lists([543, 432, 321])
 
  # unpin all lists
  account.update_pinned_lists([])
 
+ # get timelines
+ timeline = account.home_timeline()
+ latest_timeline = account.home_latest_timeline(limit=100)
+
  # example configuration
  account.update_settings({
      "address_book_live_sync_enabled": False,
      "allow_ads_personalization": False,
      "allow_authenticated_periscope_requests": True,
      "allow_dm_groups_from": "following",
      "allow_dms_from": "following",
```

