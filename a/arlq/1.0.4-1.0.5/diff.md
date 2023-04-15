# Comparing `tmp/arlq-1.0.4.tar.gz` & `tmp/arlq-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arlq-1.0.4.tar", last modified: Sat Apr 15 09:42:59 2023, max compression
+gzip compressed data, was "arlq-1.0.5.tar", last modified: Sat Apr 15 11:41:40 2023, max compression
```

## Comparing `arlq-1.0.4.tar` & `arlq-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-15 09:42:59.184526 arlq-1.0.4/
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1305 2023-04-14 17:26:18.000000 arlq-1.0.4/LICENSE
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1046 2023-04-15 09:42:59.184526 arlq-1.0.4/PKG-INFO
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     4375 2023-04-15 09:27:53.000000 arlq-1.0.4/README.md
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-15 09:42:59.184526 arlq-1.0.4/arlq/
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       57 2023-04-14 17:26:18.000000 arlq-1.0.4/arlq/__init__.py
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       22 2023-04-15 09:00:02.000000 arlq-1.0.4/arlq/_version.py
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)    19597 2023-04-15 09:28:26.000000 arlq-1.0.4/arlq/arlq.py
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-15 09:42:59.184526 arlq-1.0.4/arlq.egg-info/
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1046 2023-04-15 09:42:59.000000 arlq-1.0.4/arlq.egg-info/PKG-INFO
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      253 2023-04-15 09:42:59.000000 arlq-1.0.4/arlq.egg-info/SOURCES.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        1 2023-04-15 09:42:59.000000 arlq-1.0.4/arlq.egg-info/dependency_links.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       36 2023-04-15 09:42:59.000000 arlq-1.0.4/arlq.egg-info/entry_points.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       43 2023-04-15 09:42:59.000000 arlq-1.0.4/arlq.egg-info/requires.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        5 2023-04-15 09:42:59.000000 arlq-1.0.4/arlq.egg-info/top_level.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      836 2023-04-15 09:42:59.184526 arlq-1.0.4/setup.cfg
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       38 2023-04-14 17:26:18.000000 arlq-1.0.4/setup.py
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-15 11:41:40.152169 arlq-1.0.5/
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1305 2023-04-14 17:26:18.000000 arlq-1.0.5/LICENSE
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1046 2023-04-15 11:41:40.152169 arlq-1.0.5/PKG-INFO
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     4375 2023-04-15 10:32:33.000000 arlq-1.0.5/README.md
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-15 11:41:40.152169 arlq-1.0.5/arlq/
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       57 2023-04-14 17:26:18.000000 arlq-1.0.5/arlq/__init__.py
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       22 2023-04-15 11:38:24.000000 arlq-1.0.5/arlq/_version.py
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)    19670 2023-04-15 11:38:00.000000 arlq-1.0.5/arlq/arlq.py
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-15 11:41:40.152169 arlq-1.0.5/arlq.egg-info/
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1046 2023-04-15 11:41:40.000000 arlq-1.0.5/arlq.egg-info/PKG-INFO
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      253 2023-04-15 11:41:40.000000 arlq-1.0.5/arlq.egg-info/SOURCES.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        1 2023-04-15 11:41:40.000000 arlq-1.0.5/arlq.egg-info/dependency_links.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       36 2023-04-15 11:41:40.000000 arlq-1.0.5/arlq.egg-info/entry_points.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       43 2023-04-15 11:41:40.000000 arlq-1.0.5/arlq.egg-info/requires.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        5 2023-04-15 11:41:40.000000 arlq-1.0.5/arlq.egg-info/top_level.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      836 2023-04-15 11:41:40.152169 arlq-1.0.5/setup.cfg
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       38 2023-04-14 17:26:18.000000 arlq-1.0.5/setup.py
```

### Comparing `arlq-1.0.4/LICENSE` & `arlq-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `arlq-1.0.4/PKG-INFO` & `arlq-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arlq
-Version: 1.0.4
+Version: 1.0.5
 Summary: ARQL, another rogue-like quest game.
 Home-page: https://github.com/tos-kamiya/arlq
 Author: Toshihiro Kamiya
 Author-email: kamiya@mbj.nifty.com
 License: BSD 2-Clause License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `arlq-1.0.4/README.md` & `arlq-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `arlq-1.0.4/arlq/arlq.py` & `arlq-1.0.5/arlq/arlq.py`

 * *Files 2% similar despite different names*

```diff
@@ -437,22 +437,24 @@
             player.item = ""
         return message
 
     stdscr.keypad(True)
 
     message: Optional[str] = None
     hours: int = -1
-    while True:
+    game_ends = False
+    while not game_ends:
         hours += 1
 
         # Starvation check
         player.food -= 1
         if player.food <= 0:
             message = ">> Starved to Death. <<"
-            break  # end game
+            game_ends = True
+            break
 
         # Show the field
         update_torched(torched, player, torch_radius)
         temp_message = consume_player_item(player)
         stdscr.clear()
         draw_stage(stdscr, objects, field, torched, encountered_types, show_entities=args.debug_show_entities)
         draw_status_bar(stdscr, player, hours, message=message or temp_message)
@@ -485,15 +487,16 @@
 
         # Actions & events (combats, state changes, etc)
         for enc_obj_i, enc_obj in enc_obj_infos:
             if isinstance(enc_obj, Treasure):
                 if CHAR_DRAGON in encountered_types:
                     encountered_types.add(CHAR_TREASURE)
                     message = ">> Won the Treasure! <<"
-                    break  # end game
+                    game_ends = True
+                    break
             elif isinstance(enc_obj, Monster):
                 m = enc_obj
                 encountered_types.add(m.kind.char)
                 player_attack = player_attack_by_level(player)
 
                 if player_attack < m.kind.level:
                     if m.kind.item == ITEM_RANDOM_TRANSPORT:
```

### Comparing `arlq-1.0.4/arlq.egg-info/PKG-INFO` & `arlq-1.0.5/arlq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arlq
-Version: 1.0.4
+Version: 1.0.5
 Summary: ARQL, another rogue-like quest game.
 Home-page: https://github.com/tos-kamiya/arlq
 Author: Toshihiro Kamiya
 Author-email: kamiya@mbj.nifty.com
 License: BSD 2-Clause License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `arlq-1.0.4/setup.cfg` & `arlq-1.0.5/setup.cfg`

 * *Files identical despite different names*

