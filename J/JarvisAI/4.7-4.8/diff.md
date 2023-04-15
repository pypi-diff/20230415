# Comparing `tmp/JarvisAI-4.7.tar.gz` & `tmp/JarvisAI-4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JarvisAI-4.7.tar", last modified: Sun Apr  9 20:50:25 2023, max compression
+gzip compressed data, was "JarvisAI-4.8.tar", last modified: Sat Apr 15 05:39:49 2023, max compression
```

## Comparing `JarvisAI-4.7.tar` & `JarvisAI-4.8.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 20:50:25.057886 JarvisAI-4.7/
-drwxrwxrwx   0        0        0        0 2023-04-09 20:50:24.716306 JarvisAI-4.7/JarvisAI/
--rw-rw-rw-   0        0        0    10957 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 20:50:24.799123 JarvisAI-4.7/JarvisAI/brain/
--rw-rw-rw-   0        0        0        0 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/brain/__init__.py
--rw-rw-rw-   0        0        0      931 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/brain/auth.py
--rw-rw-rw-   0        0        0     3401 2023-04-09 20:49:35.000000 JarvisAI-4.7/JarvisAI/brain/chatbot_premium.py
--rw-rw-rw-   0        0        0     1505 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/brain/intent_classification.py
--rw-rw-rw-   0        0        0      919 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/brain/ner.py
-drwxrwxrwx   0        0        0        0 2023-04-09 20:50:25.019455 JarvisAI-4.7/JarvisAI/features/
--rw-rw-rw-   0        0        0        0 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/__init__.py
--rw-rw-rw-   0        0        0     1135 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/click_photo.py
--rw-rw-rw-   0        0        0     1280 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/covid_cases.py
--rw-rw-rw-   0        0        0      333 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/date_time.py
--rw-rw-rw-   0        0        0      363 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/games.py
--rw-rw-rw-   0        0        0      310 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/greet.py
--rw-rw-rw-   0        0        0      186 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/iambored.py
--rw-rw-rw-   0        0        0     1068 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/internet_speed_test.py
--rw-rw-rw-   0        0        0      364 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/joke.py
--rw-rw-rw-   0        0        0      867 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/news.py
--rw-rw-rw-   0        0        0      333 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/places_near_me.py
--rw-rw-rw-   0        0        0      625 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/screenshot.py
--rw-rw-rw-   0        0        0      895 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/send_email.py
--rw-rw-rw-   0        0        0      615 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/tell_me_about.py
--rw-rw-rw-   0        0        0     3923 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/volume_controller.py
--rw-rw-rw-   0        0        0      983 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/weather.py
--rw-rw-rw-   0        0        0      535 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/website_open.py
--rw-rw-rw-   0        0        0      449 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/whatsapp_message.py
--rw-rw-rw-   0        0        0      245 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/youtube_play.py
--rw-rw-rw-   0        0        0      492 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features/youtube_video_downloader.py
--rw-rw-rw-   0        0        0     3215 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/features_manager.py
-drwxrwxrwx   0        0        0        0 2023-04-09 20:50:25.026483 JarvisAI-4.7/JarvisAI/utils/
--rw-rw-rw-   0        0        0        0 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/utils/__init__.py
--rw-rw-rw-   0        0        0     3670 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/utils/input_output.py
-drwxrwxrwx   0        0        0        0 2023-04-09 20:50:25.045450 JarvisAI-4.7/JarvisAI/utils/speech_to_text/
--rw-rw-rw-   0        0        0        0 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/utils/speech_to_text/__init__.py
--rw-rw-rw-   0        0        0     2277 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/utils/speech_to_text/speech_to_text.py
--rw-rw-rw-   0        0        0      715 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/utils/speech_to_text/speech_to_text_whisper.py
-drwxrwxrwx   0        0        0        0 2023-04-09 20:50:25.055973 JarvisAI-4.7/JarvisAI/utils/text_to_speech/
--rw-rw-rw-   0        0        0        0 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/utils/text_to_speech/__init__.py
--rw-rw-rw-   0        0        0     3268 2023-04-03 21:49:40.000000 JarvisAI-4.7/JarvisAI/utils/text_to_speech/text_to_speech.py
-drwxrwxrwx   0        0        0        0 2023-04-09 20:50:24.743871 JarvisAI-4.7/JarvisAI.egg-info/
--rw-rw-rw-   0        0        0    12183 2023-04-09 20:50:24.000000 JarvisAI-4.7/JarvisAI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1350 2023-04-09 20:50:24.000000 JarvisAI-4.7/JarvisAI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 20:50:24.000000 JarvisAI-4.7/JarvisAI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      354 2023-04-09 20:50:24.000000 JarvisAI-4.7/JarvisAI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-09 20:50:24.000000 JarvisAI-4.7/JarvisAI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-04-03 21:49:40.000000 JarvisAI-4.7/License.txt
--rw-rw-rw-   0        0        0       45 2023-04-03 21:49:40.000000 JarvisAI-4.7/MANIFEST.in
--rw-rw-rw-   0        0        0    12183 2023-04-09 20:50:25.057886 JarvisAI-4.7/PKG-INFO
--rw-rw-rw-   0        0        0    11271 2023-04-07 06:33:15.000000 JarvisAI-4.7/README.md
--rw-rw-rw-   0        0        0       42 2023-04-09 20:50:25.058902 JarvisAI-4.7/setup.cfg
--rw-rw-rw-   0        0        0     1856 2023-04-09 20:50:12.000000 JarvisAI-4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 05:39:49.202029 JarvisAI-4.8/
+drwxrwxrwx   0        0        0        0 2023-04-15 05:39:49.165558 JarvisAI-4.8/JarvisAI/
+-rw-rw-rw-   0        0        0    12349 2023-04-15 04:47:12.000000 JarvisAI-4.8/JarvisAI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 05:39:49.186798 JarvisAI-4.8/JarvisAI/brain/
+-rw-rw-rw-   0        0        0        0 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/brain/__init__.py
+-rw-rw-rw-   0        0        0      931 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/brain/auth.py
+-rw-rw-rw-   0        0        0     3762 2023-04-15 04:52:26.000000 JarvisAI-4.8/JarvisAI/brain/chatbot_premium.py
+-rw-rw-rw-   0        0        0     2304 2023-04-15 05:00:05.000000 JarvisAI-4.8/JarvisAI/brain/intent_classification.py
+-rw-rw-rw-   0        0        0      919 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/brain/ner.py
+drwxrwxrwx   0        0        0        0 2023-04-15 05:39:49.196935 JarvisAI-4.8/JarvisAI/features/
+-rw-rw-rw-   0        0        0        0 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/features/__init__.py
+-rw-rw-rw-   0        0        0     1135 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/features/click_photo.py
+-rw-rw-rw-   0        0        0     1280 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/features/covid_cases.py
+-rw-rw-rw-   0        0        0      333 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/features/date_time.py
+-rw-rw-rw-   0        0        0      363 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/features/games.py
+-rw-rw-rw-   0        0        0      310 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/features/greet.py
+-rw-rw-rw-   0        0        0      186 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/features/iambored.py
+-rw-rw-rw-   0        0        0     1068 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/features/internet_speed_test.py
+-rw-rw-rw-   0        0        0      364 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/features/joke.py
+-rw-rw-rw-   0        0        0      867 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/features/news.py
+-rw-rw-rw-   0        0        0      333 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/features/places_near_me.py
+-rw-rw-rw-   0        0        0      625 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/features/screenshot.py
+-rw-rw-rw-   0        0        0      895 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/features/send_email.py
+-rw-rw-rw-   0        0        0     1620 2023-04-15 05:30:29.000000 JarvisAI-4.8/JarvisAI/features/tell_me_about.py
+-rw-rw-rw-   0        0        0     3923 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/features/volume_controller.py
+-rw-rw-rw-   0        0        0      983 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/features/weather.py
+-rw-rw-rw-   0        0        0      535 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/features/website_open.py
+-rw-rw-rw-   0        0        0      449 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/features/whatsapp_message.py
+-rw-rw-rw-   0        0        0      245 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/features/youtube_play.py
+-rw-rw-rw-   0        0        0      492 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/features/youtube_video_downloader.py
+-rw-rw-rw-   0        0        0     3215 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/features_manager.py
+drwxrwxrwx   0        0        0        0 2023-04-15 05:39:49.197936 JarvisAI-4.8/JarvisAI/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/utils/__init__.py
+-rw-rw-rw-   0        0        0     3670 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/utils/input_output.py
+drwxrwxrwx   0        0        0        0 2023-04-15 05:39:49.198936 JarvisAI-4.8/JarvisAI/utils/speech_to_text/
+-rw-rw-rw-   0        0        0        0 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/utils/speech_to_text/__init__.py
+-rw-rw-rw-   0        0        0     2277 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/utils/speech_to_text/speech_to_text.py
+-rw-rw-rw-   0        0        0      715 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/utils/speech_to_text/speech_to_text_whisper.py
+drwxrwxrwx   0        0        0        0 2023-04-15 05:39:49.199936 JarvisAI-4.8/JarvisAI/utils/text_to_speech/
+-rw-rw-rw-   0        0        0        0 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/utils/text_to_speech/__init__.py
+-rw-rw-rw-   0        0        0     3268 2023-04-03 21:49:40.000000 JarvisAI-4.8/JarvisAI/utils/text_to_speech/text_to_speech.py
+drwxrwxrwx   0        0        0        0 2023-04-15 05:39:49.184807 JarvisAI-4.8/JarvisAI.egg-info/
+-rw-rw-rw-   0        0        0    12669 2023-04-15 05:39:49.000000 JarvisAI-4.8/JarvisAI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1350 2023-04-15 05:39:49.000000 JarvisAI-4.8/JarvisAI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 05:39:49.000000 JarvisAI-4.8/JarvisAI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      354 2023-04-15 05:39:49.000000 JarvisAI-4.8/JarvisAI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-15 05:39:49.000000 JarvisAI-4.8/JarvisAI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-04-03 21:49:40.000000 JarvisAI-4.8/License.txt
+-rw-rw-rw-   0        0        0       45 2023-04-03 21:49:40.000000 JarvisAI-4.8/MANIFEST.in
+-rw-rw-rw-   0        0        0    12669 2023-04-15 05:39:49.201034 JarvisAI-4.8/PKG-INFO
+-rw-rw-rw-   0        0        0    11757 2023-04-15 05:39:46.000000 JarvisAI-4.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-15 05:39:49.202029 JarvisAI-4.8/setup.cfg
+-rw-rw-rw-   0        0        0     1856 2023-04-14 13:00:28.000000 JarvisAI-4.8/setup.py
```

### Comparing `JarvisAI-4.7/JarvisAI/__init__.py` & `JarvisAI-4.8/JarvisAI/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,32 +14,56 @@
     from JarvisAI.brain import intent_classification
     from JarvisAI.brain import ner
     from JarvisAI.features_manager import action_map
     from JarvisAI.brain.auth import verify_user
 
 
 def action_handler(intent, query, api_key):
+    intent = intent.replace("_", " ")
     if intent in action_map:
         logging.info(f"Intent {intent} matched. Calling action {action_map[intent]}")
         entities = ner.perform_ner(query=query)
-        return action_map[intent](query=query, intent=intent, entities=entities, input_output_fun=input_output,
-                                  api_key=api_key)
+        try:
+            ans = action_map[intent](query=query, intent=intent, entities=entities, input_output_fun=input_output,
+                                     api_key=api_key)
+            if ans == "Entity not found":
+                intent = "others"
+                print(
+                    "Entity not found, calling action for intent 'others'. If you are not upgraded to our premium plan, "
+                    "please upgrade to use this feature.")
+                ans = action_map[intent](query=query, intent=intent, entities=entities, input_output_fun=input_output,
+                                         api_key=api_key)
+                return ans
+            return ans
+        except Exception as e:
+            ans = action_map[intent](query=query, intent=intent, entities=entities, input_output_fun=input_output,
+                                     api_key=api_key)
+            if ans == "Entity not found":
+                intent = "others"
+                print(
+                    "Entity not found, calling action for intent 'others'. If you are not upgraded to our premium plan, "
+                    "please upgrade to use this feature.")
+                ans = action_map[intent](query=query, intent=intent, entities=entities, input_output_fun=input_output,
+                                         api_key=api_key)
+                return ans
+            return ans
     else:
         logging.info(f"Intent {intent} not found in action map.")
         return "Sorry, I don't know how to handle this intent."
 
 
 # function to add new actions to the actions_map dictionary
 def add_action(intent: str, action: object):
     """Add a new action to the action map.
     @param intent: (String) The intent to be mapped to the action.
     @param action: (Object) The function to call when the intent is matched.
     @return: (String) The message to be displayed to the user.
     """
     try:
+        intent = intent.replace("_", " ")
         action_map[intent] = action
 
         if not os.path.exists('actions.json'):
             url = "https://raw.githubusercontent.com/Dipeshpal/Jarvis_AI/master/JarvisAI/JarvisAI/actions.json"
             data = requests.get(url).json()
             with open('actions.json', 'w') as f:
                 json.dump(data, f)
@@ -156,32 +180,32 @@
                       f"{available_output_mechanisms}"
         except Exception as e:
             logging.exception(f"An error occurred while handling output. Error: {e}")
             self.handle_output(f"An error occurred while handling output. Error: {e}")
 
     def take_action(self, intent, query):
         try:
-            if not os.path.exists('actions.json'):
-                # TODO: Add a default actions.json file
-                logging.error("actions.json file not found.")
-                return "actions.json file not found."
-
-            # load the JSON file containing the list of available actions and their respective commands
-            with open('actions.json', 'r') as f:
-                actions = json.load(f)
+            # if not os.path.exists('actions.json'):
+            #     # TODO: Add a default actions.json file
+            #     logging.error("actions.json file not found.")
+            #     return "actions.json file not found."
+            #
+            # # load the JSON file containing the list of available actions and their respective commands
+            # with open('actions.json', 'r') as f:
+            #     actions = json.load(f)
 
             # check if the intent matches any of the available actions
-            for action in actions:
-                if action['intent'] == intent:
-                    # if the intent matches, do the action
-                    try:
-                        return action_handler(intent, query, self.api_key)
-                    except Exception as e:
-                        logging.exception(f"An error occurred while performing action. Error: {e}")
-                        self.handle_output(f"An error occurred while performing action. Error: {e}")
+            # for action in actions:
+            # intent, _ = intent_classification.classify_intent(secret_key=self.api_key, text=query)
+            # if the intent matches, do the action
+            try:
+                return action_handler(intent, query, self.api_key)
+            except Exception as e:
+                logging.exception(f"An error occurred while performing action. Error: {e}")
+                self.handle_output(f"An error occurred while performing action. Error: {e}")
 
             print(f"Intent {intent} not found in actions.json.")
             # if no action is matched, return a default message
             return "Sorry, I don't know how to handle this intent."
         except Exception as e:
             logging.exception(f"An error occurred while taking action. Error: {e}")
             return f"An error occurred while taking action. Error: {e}"
@@ -196,18 +220,18 @@
                     continue
                 if query == 'exit':
                     self.handle_output("Exiting...")
                     break
                 else:
                     # NOTE: The query is passed to the intent classification function to get the intent
                     intent, _ = intent_classification.classify_intent(secret_key=self.api_key, text=query)
-                    print(f"Intent: {intent}")
-                    intent = intent.replace("_", " ")
+                    # print(f"Intent: {intent}")
+                    # intent = intent.replace("_", " ")
                     # PATCH BELOW for date and time if-else
-                    if 'time' in intent:
+                    if 'time' in intent.replace("_", " "):
                         print(f"Intent: date / {intent}")
                     else:
                         print(f"Intent: {intent}")
                     logging.debug(f"Input: {query}, Intent: {intent}")
                     response = self.take_action(intent, query)
                     self.handle_output(response)
             except Exception as e:
@@ -226,9 +250,9 @@
         return command + ' Executed'
 
 
     jarvis = JarvisAI(input_mechanism='text', output_mechanism='text',
                       google_speech_api_key=None, backend_tts_api='pyttsx3',
                       use_whisper_asr=False, display_logs=False,
                       api_key='527557f2-0b67-4500-8ca0-03766ade589a')
-    # add_action("general", custom_function)
+    add_action("general", custom_function)
     jarvis.start()
```

### Comparing `JarvisAI-4.7/JarvisAI/brain/auth.py` & `JarvisAI-4.8/JarvisAI/brain/auth.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.7/JarvisAI/brain/chatbot_premium.py` & `JarvisAI-4.8/JarvisAI/brain/chatbot_premium.py`

 * *Files 7% similar despite different names*

```diff
@@ -84,32 +84,43 @@
 def search_all(query, advance_search=False):
     combined = search_google_description(query) + "\n" + search_wiki(query)
     if advance_search:
         combined += "\n" + ' '.join(search_google(query))
     return combined
 
 
+def try_to_get_response(*args, **kwargs):
+    api_key = kwargs.get("api_key")
+    query = kwargs.get('query')
+    context = search_all(query, advance_search=False)
+    headers = {
+        'accept': 'application/json',
+        'content-type': 'application/x-www-form-urlencoded',
+    }
+    params = {
+        'secret_key': api_key,
+        'text': query,
+        'context': context,
+    }
+    response = requests.post('https://www.jarvisai.in/chatbot_premium_api', params=params, headers=headers)
+    if response.status_code == 200:
+        return response.json()['data']
+    else:
+        return response.json().get("message", "Server is facing some issues. Please try again later.")
+
+
 def premium_chat(*args, **kwargs):
-    try:
-        api_key = kwargs.get("api_key")
-        query = kwargs.get('query')
-        context = search_all(query, advance_search=False)
-        headers = {
-            'accept': 'application/json',
-            'content-type': 'application/x-www-form-urlencoded',
-        }
-        params = {
-            'secret_key': api_key,
-            'text': query,
-            'context': context,
-        }
-        response = requests.post('https://www.jarvisai.in/chatbot_premium_api', params=params, headers=headers)
-        if response.status_code == 200:
-            return response.json()['data']
-        else:
-            return response.json().get("message", "Server is facing some issues. Please try again later.")
-    except Exception as e:
-        return f"An error occurred while performing premium_chat, connect with developer. Error: {e}"
+    # try 3 times to call try_to_get_response(*args, **kwargs) function and if it fails then return error message
+    for i in range(3):
+        try:
+            return try_to_get_response(*args, **kwargs)
+        except Exception as e:
+            pass
+    return "Server is facing some issues. Please try again later."
+    # try:
+    #     try_to_get_response(*args, **kwargs)
+    # except Exception as e:
+    #     return f"An error occurred while performing premium_chat, connect with developer. Error: {e}"
 
 
 if __name__ == "__main__":
     print(premium_chat(query="who is naredra modi", api_key='ae44cc6e-0d5c-45c1-b8a3-fe412469510f'))
```

### Comparing `JarvisAI-4.7/JarvisAI/brain/intent_classification.py` & `JarvisAI-4.8/JarvisAI/brain/intent_classification.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,30 +14,46 @@
     """
     try:
         if not os.path.exists('actions.json'):
             return None
         else:
             with open('actions.json', 'r') as f:
                 actions = json.load(f)
+            # Below is sample actions.json file
+            # [
+            #   {
+            #     "intent": "greet and hello hi kind of things",
+            #     "example": []
+            #   },
+            #   {
+            #     "intent": "goodbye",
+            #     "example": ['bye', 'goodbye', 'see you later']
+            #   }
+            # ]
+            # if text in example then return intent
             for action in actions:
                 if text in action['example']:
                     return action['intent']
+                if action['intent'] in text:
+                    return action['intent']
+                if action['example'] == "":
+                    continue
     except Exception as e:
-        return e
+        return None
 
 
-def classify_intent(secret_key, text):
+def try_to_classify_intent(secret_key, text):
     """Classify the intent of a text string using the Wit.ai API.
 
-    Args:
-        text (str): The text string to classify.
+       Args:
+           text (str): The text string to classify.
 
-    Returns:
-        str: The intent of the text string.
-    """
+       Returns:
+           str: The intent of the text string.
+       """
     try:
         intent = check_local_intent(text)
         if intent is not None:
             return intent, 1.0
     except Exception as e:
         pass
 
@@ -47,10 +63,17 @@
         data = response.json()
         if data['status'] == 'success':
             return data['data'][0], data['data'][1]
     except Exception as e:
         return e, None
 
 
+def classify_intent(secret_key, text):
+    for i in range(3):
+        try:
+            return try_to_classify_intent(secret_key, text)
+        except Exception as e:
+            pass
+
 if __name__ == "__main__":
-    intent, _ = classify_intent('527557f2-0b67-4500-8ca0-03766ade589a', "what is the time")
+    intent, _ = classify_intent('99f605ce-5bf9-4e80-93a3-f367df65aa27', "custom function")
     print(intent, _)
```

### Comparing `JarvisAI-4.7/JarvisAI/brain/ner.py` & `JarvisAI-4.8/JarvisAI/brain/ner.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.7/JarvisAI/features/click_photo.py` & `JarvisAI-4.8/JarvisAI/features/click_photo.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.7/JarvisAI/features/covid_cases.py` & `JarvisAI-4.8/JarvisAI/features/covid_cases.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.7/JarvisAI/features/internet_speed_test.py` & `JarvisAI-4.8/JarvisAI/features/internet_speed_test.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.7/JarvisAI/features/news.py` & `JarvisAI-4.8/JarvisAI/features/news.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.7/JarvisAI/features/screenshot.py` & `JarvisAI-4.8/JarvisAI/features/screenshot.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.7/JarvisAI/features/send_email.py` & `JarvisAI-4.8/JarvisAI/features/send_email.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.7/JarvisAI/features/volume_controller.py` & `JarvisAI-4.8/JarvisAI/features/volume_controller.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.7/JarvisAI/features/weather.py` & `JarvisAI-4.8/JarvisAI/features/weather.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.7/JarvisAI/features/website_open.py` & `JarvisAI-4.8/JarvisAI/features/website_open.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.7/JarvisAI/features_manager.py` & `JarvisAI-4.8/JarvisAI/features_manager.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.7/JarvisAI/utils/input_output.py` & `JarvisAI-4.8/JarvisAI/utils/input_output.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.7/JarvisAI/utils/speech_to_text/speech_to_text.py` & `JarvisAI-4.8/JarvisAI/utils/speech_to_text/speech_to_text.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.7/JarvisAI/utils/speech_to_text/speech_to_text_whisper.py` & `JarvisAI-4.8/JarvisAI/utils/speech_to_text/speech_to_text_whisper.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.7/JarvisAI/utils/text_to_speech/text_to_speech.py` & `JarvisAI-4.8/JarvisAI/utils/text_to_speech/text_to_speech.py`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.7/JarvisAI.egg-info/PKG-INFO` & `JarvisAI-4.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: JarvisAI
-Version: 4.7
-Summary: JarvisAI is python library to build your own AI virtual assistant with natural language processing.
-Home-page: https://github.com/Dipeshpal/Jarvis_AI
-Author: Dipesh
-Author-email: dipeshpal17@gmail.com
-License: UNKNOWN
-Project-URL: Official Website, https://jarvisai.in
-Project-URL: Documentation, https://github.com/Dipeshpal/Jarvis_AI
-Project-URL: Donate, https://www.buymeacoffee.com/dipeshpal
-Project-URL: Say Thanks!, https://youtube.com/techportofficial
-Project-URL: Source, https://github.com/Dipeshpal/Jarvis_AI
-Project-URL: Contact, https://www.dipeshpal.in/social
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: License.txt
-
 [![Header](https://i.postimg.cc/mDCdt9Jn/Mixing-Panel-Photocentric-EDM-Youtube-Channel-Art-1.png "Header")](http://jarvis-ai-api.herokuapp.com/)    
     
     
 ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)    
     
 # Hello, folks! <img src="https://raw.githubusercontent.com/MartinHeinz/MartinHeinz/master/wave.gif" width="30px">    
  This project is created only for those who are interested in building a Virtual Assistant. Generally, it took lots of time to write code from scratch to build a Virtual Assistant. So, I have built a Library called "JarvisAI", which gives you easy functionality to build your own Virtual Assistant.    
@@ -57,14 +35,19 @@
 
 **Check out our plan: https://jarvisai.in/dashboard**
 
 
 ## YouTube Tutorial-  
   
 Click on the image below to watch the tutorial on YouTube-  
+
+**Tutorial Latest-**
+
+[![JarvisAI Tutorial 1](https://img.youtube.com/vi/hPE-kdRmYf8/0.jpg)](https://www.youtube.com/watch?v=hPE-kdRmYf8)  
+
   
 **Tutorial 1-**  
   
 [![JarvisAI Tutorial 1](https://img.youtube.com/vi/p2hdqB11S-8/0.jpg)](https://www.youtube.com/watch?v=p2hdqB11S-8)  
   
 **Tutorial 2-**  
   
@@ -137,42 +120,61 @@
 * [Optional Step] You might need to Install [Microsoft Visual C++ Redistributable for Visual Studio 2022](https://visualstudio.microsoft.com/downloads/#microsoft-visual-c-redistributable-for-visual-studio-2022)  
   
 ### 4.2. Code You Need-  
    
    You need only this piece of code-
 	
 	
-	def custom_function(*args, **kwargs):
+    import JarvisAI
+
+    def custom_function(*args, **kwargs):
         command = kwargs.get('query')
         entities = kwargs.get('entities')
         print(entities)
         # write your code here to do something with the command
         # perform some tasks # return is optional
         return command + ' Executed'
-
-
-    jarvis = JarvisAI.Jarvis(input_mechanism='voice', output_mechanism='both',
-                    google_speech_api_key=None, backend_tts_api='pyttsx3',
-                    use_whisper_asr=False, display_logs=False,
-                    api_key='527557f2-0b67-4500-8ca0-03766ade589a')
-    # add_action("general", custom_function)  # OPTIONAL
-    jarvis.start()
-	
+    
+    
+    jarvis = JarvisAI.JarvisAI(input_mechanism='text', output_mechanism='text',
+                           google_speech_api_key=None, backend_tts_api='pyttsx3',
+                           use_whisper_asr=False, display_logs=False,
+                           api_key='99f605ce-5bf9-4e80-93a3-f367df65aa27')
+    JarvisAI.add_action('custom_function', custom_function)
+    jarvis.start()	
   
    
  ### 4.3. **What's now?**    
     
  It will start your AI, it will ask you to give input and accordingly it will produce output.      
    You can configure  `input_mechanism` and  `output_mechanism` parameter for voice input/output or text input/output.    
     
    ### 4.4. Let's understand the Parameters-    
+    
+For text input-
+    
+    input_mechanism='text'
+
+For voice input-
+    
+    input_mechanism='voice'
+
+For text output-
+    
+    output_mechanism='text'
+    
+For voice output-
+    
+    output_mechanism='voice'
+
+For voice and text output-
+    
+    output_mechanism='both'
      
-  ```bash :param input_method: (object) method to get input from user <allowed values: [InputsMethods.text_input, InputsMethods.voice_input_google_api, InputsMethods.voice_input_deepspeech_streaming]> :param output_method: (object) method to give output to user <allowed values: [OutputMethods.text_output, OutputMethods.voice_output] :param backend_tts_api: (str) [Default 'pyttsx3'] backend tts api to use <allowed values: ['pyttsx3', 'gtts']> :param api_key: (str) [Default ''] api key to use JarvisAI get it from http://jarvis-ai-api.herokuapp.com :param detect_wake_word: (bool) [Default True] detect wake word or not <allowed values: [True, False]> :param wake_word_detection_method: (object) [Default None] method to detect wake word <allowed values: [InputsMethods.voice_input_google_api, InputsMethods.voice_input_deepspeech_streaming] :param bot_name: (str) [Default 'Jarvis'] name of the bot :param display_intent: (bool) [Default True] display intent or not <allowed values: [True, False]> :param google_speech_recognition_input_lang: (str) [Default 'en'] language of the input Check supported languages here: https://cloud.google.com/speech-to-text/docs/languages :param google_speech_recognition_key: (str) [Default None] api key to use Google Speech API :param google_speech_recognition_duration_listening: (int) [Default 5] duration of the listening    
- READ MORE: Google Speech API (Pricing and Key) at: https://cloud.google.com/speech-to-text  
-```   
+
 ## 5. What it can do (Features it supports)-    
     
 1. Currently, it supports only english language    
 2. Supports voice and text input/output.    
 3. Supports AI based voice input (using whisper asr) and by using google api voice input.    
 4. All intellectual task is process in JarvisAI server so there is no load on your system.    
 5. Lightweight and able to understand natural language (commands)    
@@ -210,18 +212,18 @@
  22. others  / Unknown Intent (Premium Feature)
 
   
 ### 5.2. Supported Input/Output Methods (Which option do I need to choose?)-    
 
 You can set below parameter while creating object of JarvisAI-
 
-    jarvis = JarvisAI.Jarvis(input_mechanism='voice', output_mechanism='both',  
-                    google_speech_api_key=None, backend_tts_api='pyttsx3',  
-                    use_whisper_asr=False, display_logs=False,  
-                    api_key='527557f2-0b67-4500-8ca0-03766ade589a')
+    jarvis = JarvisAI.JarvisAI(input_mechanism='text', output_mechanism='text',
+                           google_speech_api_key=None, backend_tts_api='pyttsx3',
+                           use_whisper_asr=False, display_logs=False,
+                           api_key='99f605ce-5bf9-4e80-93a3-f367df65aa27')
     
 1. **For text input-**'    
     
 		input_mechanism='text'
        
 2. **For voice input-**    
    
@@ -229,55 +231,98 @@
     
 3. **For text output-**    
     
 	    output_mechanism='text'
     
 4. **For voice output-**    
 
-	    output_mechanism='text'
+	    output_mechanism='voice'
 
 5. **For voice and text output-**    
 
 	    output_mechanism='both'
        
 ## 6. Future/Request Features-    
 
  **WIP**    
  **You tell me**    
-    at dipeshpal17@gmail.com or my social media.
+    at info@jarvisai.in or my www.dipeshpal.in/social
     
  ## 7. Contribute-    
- **Instructions Coming Soon**    
+  
+  1. Clone this repo.
+  2. Create your file in JarvisAI/JarvisAI/features/<your_file.py>
+  3. Write entry function like this-
+  
+  	
+	def some_func(*args, **kwargs):
+	    query = kwargs.get("query")
+	    entities = kwargs.get("entities")
+	    li = ['EVENT', 'FAC', 'GPE', 'LANGUAGE', 'LAW', 'LOC', 'MONEY', 'NORP', 'ORDINAL', 'ORG',
+		  'PERCENT', 'PERSON', 'PRODUCT', 'TIME', 'WORK_OF_ART']
+	    topic = [entity[0] for entity in entities if entity[1] in li][0]
+	    return "This Code Done"
+	
+  - query is the text that is recognized by your microphone
+  
+  - entities Named Entity Recognition is a technique of natural language processing that is used for the categorization of the data
+  
+  - Example-
+	
+	query: who is Narendra Modi
+
+	entities: [('Narendra Modi', 'PERSON')]
+	
+	topic: Narendra Modi
+ 
+ 	So, now you got the topic from query and now you can play with the topic.
+ 
+  4. Your function can return someting text or perform something. Return text will be automatically print / spoken by your system.
+  5. In JarvisAI/JarvisAI/features_manager.py , import and add your function like this
+ 	
+	try:
+    		from features.your_file import some_func
+	except Exception as e:
+		from .features.your_file import some_func
+	
+	action_map = {
+		.....
+		....
+		'your_intent': some_func
+	}
+	
+  6. That's it now raise pull request. I'll verify your code. If working, ethical and all terms are followed, I'll approve.
+  7. You will become contributer.
+
  ## 8. Contact me-    
  - [Instagram](https://www.instagram.com/dipesh_pal17)    
         
 - [YouTube](https://www.youtube.com/dipeshpal17)    
         
     
     
 ## 9. Donate-    
  
 Consider donating to JarvisAI to support our mission of keeping our servers running 24/7. Your contribution will enable us to continue doing great things and providing valuable services. Every little bit helps!
 
-[Click Here to support](https://www.instamojo.com/@techport/?ref=preview)    
+
+[Click Here to support](https://www.instamojo.com/@techport/)    
     
 **_Feel free to use my code, don't forget to mention credit. All the contributors will get credits in this repo._**    
  **_Mention below line for credits-_**    
  ***Credits-***    
  - [https://jarvisai.in](https://jarvisai.in)    
         
 - [https://github.com/Dipeshpal/Jarvis_AI](https://github.com/Dipeshpal/Jarvis_AI)    
         
 - [https://www.youtube.com/dipeshpal17](https://www.youtube.com/dipeshpal17)    
         
-- [https://www.instagram.com/dipesh_pal17](https://www.instagram.com/dipesh_pal17/)    
+- [https://www.instagram.com/dipesh_pal17](https://www.instagram.com/_dipeshpal_)
         
     
 ## 10. Thank me on-    
- - Follow me on Instagram:  [https://www.instagram.com/dipesh_pal17](https://www.instagram.com/dipesh_pal17/)    
+ - Follow me on Instagram: [https://www.instagram.com/dipesh_pal17](https://www.instagram.com/_dipeshpal_)  
         
 - Subscribe me on YouTube:  [https://www.youtube.com/dipeshpal17](https://www.youtube.com/dipeshpal17)    
     
 ## License    
  [MIT](https://choosealicense.com/licenses/mit/)
-
-
```

### Comparing `JarvisAI-4.7/JarvisAI.egg-info/SOURCES.txt` & `JarvisAI-4.8/JarvisAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.7/License.txt` & `JarvisAI-4.8/License.txt`

 * *Files identical despite different names*

### Comparing `JarvisAI-4.7/PKG-INFO` & `JarvisAI-4.8/JarvisAI.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JarvisAI
-Version: 4.7
+Version: 4.8
 Summary: JarvisAI is python library to build your own AI virtual assistant with natural language processing.
 Home-page: https://github.com/Dipeshpal/Jarvis_AI
 Author: Dipesh
 Author-email: dipeshpal17@gmail.com
 License: UNKNOWN
 Project-URL: Official Website, https://jarvisai.in
 Project-URL: Documentation, https://github.com/Dipeshpal/Jarvis_AI
@@ -57,14 +57,19 @@
 
 **Check out our plan: https://jarvisai.in/dashboard**
 
 
 ## YouTube Tutorial-  
   
 Click on the image below to watch the tutorial on YouTube-  
+
+**Tutorial Latest-**
+
+[![JarvisAI Tutorial 1](https://img.youtube.com/vi/hPE-kdRmYf8/0.jpg)](https://www.youtube.com/watch?v=hPE-kdRmYf8)  
+
   
 **Tutorial 1-**  
   
 [![JarvisAI Tutorial 1](https://img.youtube.com/vi/p2hdqB11S-8/0.jpg)](https://www.youtube.com/watch?v=p2hdqB11S-8)  
   
 **Tutorial 2-**  
   
@@ -137,42 +142,61 @@
 * [Optional Step] You might need to Install [Microsoft Visual C++ Redistributable for Visual Studio 2022](https://visualstudio.microsoft.com/downloads/#microsoft-visual-c-redistributable-for-visual-studio-2022)  
   
 ### 4.2. Code You Need-  
    
    You need only this piece of code-
 	
 	
-	def custom_function(*args, **kwargs):
+    import JarvisAI
+
+    def custom_function(*args, **kwargs):
         command = kwargs.get('query')
         entities = kwargs.get('entities')
         print(entities)
         # write your code here to do something with the command
         # perform some tasks # return is optional
         return command + ' Executed'
-
-
-    jarvis = JarvisAI.Jarvis(input_mechanism='voice', output_mechanism='both',
-                    google_speech_api_key=None, backend_tts_api='pyttsx3',
-                    use_whisper_asr=False, display_logs=False,
-                    api_key='527557f2-0b67-4500-8ca0-03766ade589a')
-    # add_action("general", custom_function)  # OPTIONAL
-    jarvis.start()
-	
+    
+    
+    jarvis = JarvisAI.JarvisAI(input_mechanism='text', output_mechanism='text',
+                           google_speech_api_key=None, backend_tts_api='pyttsx3',
+                           use_whisper_asr=False, display_logs=False,
+                           api_key='99f605ce-5bf9-4e80-93a3-f367df65aa27')
+    JarvisAI.add_action('custom_function', custom_function)
+    jarvis.start()	
   
    
  ### 4.3. **What's now?**    
     
  It will start your AI, it will ask you to give input and accordingly it will produce output.      
    You can configure  `input_mechanism` and  `output_mechanism` parameter for voice input/output or text input/output.    
     
    ### 4.4. Let's understand the Parameters-    
+    
+For text input-
+    
+    input_mechanism='text'
+
+For voice input-
+    
+    input_mechanism='voice'
+
+For text output-
+    
+    output_mechanism='text'
+    
+For voice output-
+    
+    output_mechanism='voice'
+
+For voice and text output-
+    
+    output_mechanism='both'
      
-  ```bash :param input_method: (object) method to get input from user <allowed values: [InputsMethods.text_input, InputsMethods.voice_input_google_api, InputsMethods.voice_input_deepspeech_streaming]> :param output_method: (object) method to give output to user <allowed values: [OutputMethods.text_output, OutputMethods.voice_output] :param backend_tts_api: (str) [Default 'pyttsx3'] backend tts api to use <allowed values: ['pyttsx3', 'gtts']> :param api_key: (str) [Default ''] api key to use JarvisAI get it from http://jarvis-ai-api.herokuapp.com :param detect_wake_word: (bool) [Default True] detect wake word or not <allowed values: [True, False]> :param wake_word_detection_method: (object) [Default None] method to detect wake word <allowed values: [InputsMethods.voice_input_google_api, InputsMethods.voice_input_deepspeech_streaming] :param bot_name: (str) [Default 'Jarvis'] name of the bot :param display_intent: (bool) [Default True] display intent or not <allowed values: [True, False]> :param google_speech_recognition_input_lang: (str) [Default 'en'] language of the input Check supported languages here: https://cloud.google.com/speech-to-text/docs/languages :param google_speech_recognition_key: (str) [Default None] api key to use Google Speech API :param google_speech_recognition_duration_listening: (int) [Default 5] duration of the listening    
- READ MORE: Google Speech API (Pricing and Key) at: https://cloud.google.com/speech-to-text  
-```   
+
 ## 5. What it can do (Features it supports)-    
     
 1. Currently, it supports only english language    
 2. Supports voice and text input/output.    
 3. Supports AI based voice input (using whisper asr) and by using google api voice input.    
 4. All intellectual task is process in JarvisAI server so there is no load on your system.    
 5. Lightweight and able to understand natural language (commands)    
@@ -210,18 +234,18 @@
  22. others  / Unknown Intent (Premium Feature)
 
   
 ### 5.2. Supported Input/Output Methods (Which option do I need to choose?)-    
 
 You can set below parameter while creating object of JarvisAI-
 
-    jarvis = JarvisAI.Jarvis(input_mechanism='voice', output_mechanism='both',  
-                    google_speech_api_key=None, backend_tts_api='pyttsx3',  
-                    use_whisper_asr=False, display_logs=False,  
-                    api_key='527557f2-0b67-4500-8ca0-03766ade589a')
+    jarvis = JarvisAI.JarvisAI(input_mechanism='text', output_mechanism='text',
+                           google_speech_api_key=None, backend_tts_api='pyttsx3',
+                           use_whisper_asr=False, display_logs=False,
+                           api_key='99f605ce-5bf9-4e80-93a3-f367df65aa27')
     
 1. **For text input-**'    
     
 		input_mechanism='text'
        
 2. **For voice input-**    
    
@@ -229,55 +253,100 @@
     
 3. **For text output-**    
     
 	    output_mechanism='text'
     
 4. **For voice output-**    
 
-	    output_mechanism='text'
+	    output_mechanism='voice'
 
 5. **For voice and text output-**    
 
 	    output_mechanism='both'
        
 ## 6. Future/Request Features-    
 
  **WIP**    
  **You tell me**    
-    at dipeshpal17@gmail.com or my social media.
+    at info@jarvisai.in or my www.dipeshpal.in/social
     
  ## 7. Contribute-    
- **Instructions Coming Soon**    
+  
+  1. Clone this repo.
+  2. Create your file in JarvisAI/JarvisAI/features/<your_file.py>
+  3. Write entry function like this-
+  
+  	
+	def some_func(*args, **kwargs):
+	    query = kwargs.get("query")
+	    entities = kwargs.get("entities")
+	    li = ['EVENT', 'FAC', 'GPE', 'LANGUAGE', 'LAW', 'LOC', 'MONEY', 'NORP', 'ORDINAL', 'ORG',
+		  'PERCENT', 'PERSON', 'PRODUCT', 'TIME', 'WORK_OF_ART']
+	    topic = [entity[0] for entity in entities if entity[1] in li][0]
+	    return "This Code Done"
+	
+  - query is the text that is recognized by your microphone
+  
+  - entities Named Entity Recognition is a technique of natural language processing that is used for the categorization of the data
+  
+  - Example-
+	
+	query: who is Narendra Modi
+
+	entities: [('Narendra Modi', 'PERSON')]
+	
+	topic: Narendra Modi
+ 
+ 	So, now you got the topic from query and now you can play with the topic.
+ 
+  4. Your function can return someting text or perform something. Return text will be automatically print / spoken by your system.
+  5. In JarvisAI/JarvisAI/features_manager.py , import and add your function like this
+ 	
+	try:
+    		from features.your_file import some_func
+	except Exception as e:
+		from .features.your_file import some_func
+	
+	action_map = {
+		.....
+		....
+		'your_intent': some_func
+	}
+	
+  6. That's it now raise pull request. I'll verify your code. If working, ethical and all terms are followed, I'll approve.
+  7. You will become contributer.
+
  ## 8. Contact me-    
  - [Instagram](https://www.instagram.com/dipesh_pal17)    
         
 - [YouTube](https://www.youtube.com/dipeshpal17)    
         
     
     
 ## 9. Donate-    
  
 Consider donating to JarvisAI to support our mission of keeping our servers running 24/7. Your contribution will enable us to continue doing great things and providing valuable services. Every little bit helps!
 
-[Click Here to support](https://www.instamojo.com/@techport/?ref=preview)    
+
+[Click Here to support](https://www.instamojo.com/@techport/)    
     
 **_Feel free to use my code, don't forget to mention credit. All the contributors will get credits in this repo._**    
  **_Mention below line for credits-_**    
  ***Credits-***    
  - [https://jarvisai.in](https://jarvisai.in)    
         
 - [https://github.com/Dipeshpal/Jarvis_AI](https://github.com/Dipeshpal/Jarvis_AI)    
         
 - [https://www.youtube.com/dipeshpal17](https://www.youtube.com/dipeshpal17)    
         
-- [https://www.instagram.com/dipesh_pal17](https://www.instagram.com/dipesh_pal17/)    
+- [https://www.instagram.com/dipesh_pal17](https://www.instagram.com/_dipeshpal_)
         
     
 ## 10. Thank me on-    
- - Follow me on Instagram:  [https://www.instagram.com/dipesh_pal17](https://www.instagram.com/dipesh_pal17/)    
+ - Follow me on Instagram: [https://www.instagram.com/dipesh_pal17](https://www.instagram.com/_dipeshpal_)  
         
 - Subscribe me on YouTube:  [https://www.youtube.com/dipeshpal17](https://www.youtube.com/dipeshpal17)    
     
 ## License    
  [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `JarvisAI-4.7/README.md` & `JarvisAI-4.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: JarvisAI
+Version: 4.8
+Summary: JarvisAI is python library to build your own AI virtual assistant with natural language processing.
+Home-page: https://github.com/Dipeshpal/Jarvis_AI
+Author: Dipesh
+Author-email: dipeshpal17@gmail.com
+License: UNKNOWN
+Project-URL: Official Website, https://jarvisai.in
+Project-URL: Documentation, https://github.com/Dipeshpal/Jarvis_AI
+Project-URL: Donate, https://www.buymeacoffee.com/dipeshpal
+Project-URL: Say Thanks!, https://youtube.com/techportofficial
+Project-URL: Source, https://github.com/Dipeshpal/Jarvis_AI
+Project-URL: Contact, https://www.dipeshpal.in/social
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: License.txt
+
 [![Header](https://i.postimg.cc/mDCdt9Jn/Mixing-Panel-Photocentric-EDM-Youtube-Channel-Art-1.png "Header")](http://jarvis-ai-api.herokuapp.com/)    
     
     
 ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)    
     
 # Hello, folks! <img src="https://raw.githubusercontent.com/MartinHeinz/MartinHeinz/master/wave.gif" width="30px">    
  This project is created only for those who are interested in building a Virtual Assistant. Generally, it took lots of time to write code from scratch to build a Virtual Assistant. So, I have built a Library called "JarvisAI", which gives you easy functionality to build your own Virtual Assistant.    
@@ -35,14 +57,19 @@
 
 **Check out our plan: https://jarvisai.in/dashboard**
 
 
 ## YouTube Tutorial-  
   
 Click on the image below to watch the tutorial on YouTube-  
+
+**Tutorial Latest-**
+
+[![JarvisAI Tutorial 1](https://img.youtube.com/vi/hPE-kdRmYf8/0.jpg)](https://www.youtube.com/watch?v=hPE-kdRmYf8)  
+
   
 **Tutorial 1-**  
   
 [![JarvisAI Tutorial 1](https://img.youtube.com/vi/p2hdqB11S-8/0.jpg)](https://www.youtube.com/watch?v=p2hdqB11S-8)  
   
 **Tutorial 2-**  
   
@@ -115,42 +142,61 @@
 * [Optional Step] You might need to Install [Microsoft Visual C++ Redistributable for Visual Studio 2022](https://visualstudio.microsoft.com/downloads/#microsoft-visual-c-redistributable-for-visual-studio-2022)  
   
 ### 4.2. Code You Need-  
    
    You need only this piece of code-
 	
 	
-	def custom_function(*args, **kwargs):
+    import JarvisAI
+
+    def custom_function(*args, **kwargs):
         command = kwargs.get('query')
         entities = kwargs.get('entities')
         print(entities)
         # write your code here to do something with the command
         # perform some tasks # return is optional
         return command + ' Executed'
-
-
-    jarvis = JarvisAI.Jarvis(input_mechanism='voice', output_mechanism='both',
-                    google_speech_api_key=None, backend_tts_api='pyttsx3',
-                    use_whisper_asr=False, display_logs=False,
-                    api_key='527557f2-0b67-4500-8ca0-03766ade589a')
-    # add_action("general", custom_function)  # OPTIONAL
-    jarvis.start()
-	
+    
+    
+    jarvis = JarvisAI.JarvisAI(input_mechanism='text', output_mechanism='text',
+                           google_speech_api_key=None, backend_tts_api='pyttsx3',
+                           use_whisper_asr=False, display_logs=False,
+                           api_key='99f605ce-5bf9-4e80-93a3-f367df65aa27')
+    JarvisAI.add_action('custom_function', custom_function)
+    jarvis.start()	
   
    
  ### 4.3. **What's now?**    
     
  It will start your AI, it will ask you to give input and accordingly it will produce output.      
    You can configure  `input_mechanism` and  `output_mechanism` parameter for voice input/output or text input/output.    
     
    ### 4.4. Let's understand the Parameters-    
+    
+For text input-
+    
+    input_mechanism='text'
+
+For voice input-
+    
+    input_mechanism='voice'
+
+For text output-
+    
+    output_mechanism='text'
+    
+For voice output-
+    
+    output_mechanism='voice'
+
+For voice and text output-
+    
+    output_mechanism='both'
      
-  ```bash :param input_method: (object) method to get input from user <allowed values: [InputsMethods.text_input, InputsMethods.voice_input_google_api, InputsMethods.voice_input_deepspeech_streaming]> :param output_method: (object) method to give output to user <allowed values: [OutputMethods.text_output, OutputMethods.voice_output] :param backend_tts_api: (str) [Default 'pyttsx3'] backend tts api to use <allowed values: ['pyttsx3', 'gtts']> :param api_key: (str) [Default ''] api key to use JarvisAI get it from http://jarvis-ai-api.herokuapp.com :param detect_wake_word: (bool) [Default True] detect wake word or not <allowed values: [True, False]> :param wake_word_detection_method: (object) [Default None] method to detect wake word <allowed values: [InputsMethods.voice_input_google_api, InputsMethods.voice_input_deepspeech_streaming] :param bot_name: (str) [Default 'Jarvis'] name of the bot :param display_intent: (bool) [Default True] display intent or not <allowed values: [True, False]> :param google_speech_recognition_input_lang: (str) [Default 'en'] language of the input Check supported languages here: https://cloud.google.com/speech-to-text/docs/languages :param google_speech_recognition_key: (str) [Default None] api key to use Google Speech API :param google_speech_recognition_duration_listening: (int) [Default 5] duration of the listening    
- READ MORE: Google Speech API (Pricing and Key) at: https://cloud.google.com/speech-to-text  
-```   
+
 ## 5. What it can do (Features it supports)-    
     
 1. Currently, it supports only english language    
 2. Supports voice and text input/output.    
 3. Supports AI based voice input (using whisper asr) and by using google api voice input.    
 4. All intellectual task is process in JarvisAI server so there is no load on your system.    
 5. Lightweight and able to understand natural language (commands)    
@@ -188,18 +234,18 @@
  22. others  / Unknown Intent (Premium Feature)
 
   
 ### 5.2. Supported Input/Output Methods (Which option do I need to choose?)-    
 
 You can set below parameter while creating object of JarvisAI-
 
-    jarvis = JarvisAI.Jarvis(input_mechanism='voice', output_mechanism='both',  
-                    google_speech_api_key=None, backend_tts_api='pyttsx3',  
-                    use_whisper_asr=False, display_logs=False,  
-                    api_key='527557f2-0b67-4500-8ca0-03766ade589a')
+    jarvis = JarvisAI.JarvisAI(input_mechanism='text', output_mechanism='text',
+                           google_speech_api_key=None, backend_tts_api='pyttsx3',
+                           use_whisper_asr=False, display_logs=False,
+                           api_key='99f605ce-5bf9-4e80-93a3-f367df65aa27')
     
 1. **For text input-**'    
     
 		input_mechanism='text'
        
 2. **For voice input-**    
    
@@ -207,53 +253,100 @@
     
 3. **For text output-**    
     
 	    output_mechanism='text'
     
 4. **For voice output-**    
 
-	    output_mechanism='text'
+	    output_mechanism='voice'
 
 5. **For voice and text output-**    
 
 	    output_mechanism='both'
        
 ## 6. Future/Request Features-    
 
  **WIP**    
  **You tell me**    
-    at dipeshpal17@gmail.com or my social media.
+    at info@jarvisai.in or my www.dipeshpal.in/social
     
  ## 7. Contribute-    
- **Instructions Coming Soon**    
+  
+  1. Clone this repo.
+  2. Create your file in JarvisAI/JarvisAI/features/<your_file.py>
+  3. Write entry function like this-
+  
+  	
+	def some_func(*args, **kwargs):
+	    query = kwargs.get("query")
+	    entities = kwargs.get("entities")
+	    li = ['EVENT', 'FAC', 'GPE', 'LANGUAGE', 'LAW', 'LOC', 'MONEY', 'NORP', 'ORDINAL', 'ORG',
+		  'PERCENT', 'PERSON', 'PRODUCT', 'TIME', 'WORK_OF_ART']
+	    topic = [entity[0] for entity in entities if entity[1] in li][0]
+	    return "This Code Done"
+	
+  - query is the text that is recognized by your microphone
+  
+  - entities Named Entity Recognition is a technique of natural language processing that is used for the categorization of the data
+  
+  - Example-
+	
+	query: who is Narendra Modi
+
+	entities: [('Narendra Modi', 'PERSON')]
+	
+	topic: Narendra Modi
+ 
+ 	So, now you got the topic from query and now you can play with the topic.
+ 
+  4. Your function can return someting text or perform something. Return text will be automatically print / spoken by your system.
+  5. In JarvisAI/JarvisAI/features_manager.py , import and add your function like this
+ 	
+	try:
+    		from features.your_file import some_func
+	except Exception as e:
+		from .features.your_file import some_func
+	
+	action_map = {
+		.....
+		....
+		'your_intent': some_func
+	}
+	
+  6. That's it now raise pull request. I'll verify your code. If working, ethical and all terms are followed, I'll approve.
+  7. You will become contributer.
+
  ## 8. Contact me-    
  - [Instagram](https://www.instagram.com/dipesh_pal17)    
         
 - [YouTube](https://www.youtube.com/dipeshpal17)    
         
     
     
 ## 9. Donate-    
  
 Consider donating to JarvisAI to support our mission of keeping our servers running 24/7. Your contribution will enable us to continue doing great things and providing valuable services. Every little bit helps!
 
-[Click Here to support](https://www.instamojo.com/@techport/?ref=preview)    
+
+[Click Here to support](https://www.instamojo.com/@techport/)    
     
 **_Feel free to use my code, don't forget to mention credit. All the contributors will get credits in this repo._**    
  **_Mention below line for credits-_**    
  ***Credits-***    
  - [https://jarvisai.in](https://jarvisai.in)    
         
 - [https://github.com/Dipeshpal/Jarvis_AI](https://github.com/Dipeshpal/Jarvis_AI)    
         
 - [https://www.youtube.com/dipeshpal17](https://www.youtube.com/dipeshpal17)    
         
-- [https://www.instagram.com/dipesh_pal17](https://www.instagram.com/dipesh_pal17/)    
+- [https://www.instagram.com/dipesh_pal17](https://www.instagram.com/_dipeshpal_)
         
     
 ## 10. Thank me on-    
- - Follow me on Instagram:  [https://www.instagram.com/dipesh_pal17](https://www.instagram.com/dipesh_pal17/)    
+ - Follow me on Instagram: [https://www.instagram.com/dipesh_pal17](https://www.instagram.com/_dipeshpal_)  
         
 - Subscribe me on YouTube:  [https://www.youtube.com/dipeshpal17](https://www.youtube.com/dipeshpal17)    
     
 ## License    
  [MIT](https://choosealicense.com/licenses/mit/)
+
+
```

### Comparing `JarvisAI-4.7/setup.py` & `JarvisAI-4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_namespace_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="JarvisAI",
-    version="4.7",
+    version="4.8",
     author="Dipesh",
     author_email="dipeshpal17@gmail.com",
     description="JarvisAI is python library to build your own AI virtual assistant with natural language processing.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Dipeshpal/Jarvis_AI",
     include_package_data=True,
```

