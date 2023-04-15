# Comparing `tmp/arlq-1.0.5.tar.gz` & `tmp/arlq-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arlq-1.0.5.tar", last modified: Sat Apr 15 11:41:40 2023, max compression
+gzip compressed data, was "arlq-1.0.6.tar", last modified: Sat Apr 15 13:02:16 2023, max compression
```

## Comparing `arlq-1.0.5.tar` & `arlq-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-15 11:41:40.152169 arlq-1.0.5/
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1305 2023-04-14 17:26:18.000000 arlq-1.0.5/LICENSE
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1046 2023-04-15 11:41:40.152169 arlq-1.0.5/PKG-INFO
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     4375 2023-04-15 10:32:33.000000 arlq-1.0.5/README.md
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-15 11:41:40.152169 arlq-1.0.5/arlq/
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       57 2023-04-14 17:26:18.000000 arlq-1.0.5/arlq/__init__.py
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       22 2023-04-15 11:38:24.000000 arlq-1.0.5/arlq/_version.py
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)    19670 2023-04-15 11:38:00.000000 arlq-1.0.5/arlq/arlq.py
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-15 11:41:40.152169 arlq-1.0.5/arlq.egg-info/
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1046 2023-04-15 11:41:40.000000 arlq-1.0.5/arlq.egg-info/PKG-INFO
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      253 2023-04-15 11:41:40.000000 arlq-1.0.5/arlq.egg-info/SOURCES.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        1 2023-04-15 11:41:40.000000 arlq-1.0.5/arlq.egg-info/dependency_links.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       36 2023-04-15 11:41:40.000000 arlq-1.0.5/arlq.egg-info/entry_points.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       43 2023-04-15 11:41:40.000000 arlq-1.0.5/arlq.egg-info/requires.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        5 2023-04-15 11:41:40.000000 arlq-1.0.5/arlq.egg-info/top_level.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      836 2023-04-15 11:41:40.152169 arlq-1.0.5/setup.cfg
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       38 2023-04-14 17:26:18.000000 arlq-1.0.5/setup.py
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-15 13:02:16.401621 arlq-1.0.6/
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1305 2023-04-14 17:26:18.000000 arlq-1.0.6/LICENSE
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1046 2023-04-15 13:02:16.401621 arlq-1.0.6/PKG-INFO
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     4375 2023-04-15 10:32:33.000000 arlq-1.0.6/README.md
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-15 13:02:16.397621 arlq-1.0.6/arlq/
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       57 2023-04-14 17:26:18.000000 arlq-1.0.6/arlq/__init__.py
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       22 2023-04-15 12:49:29.000000 arlq-1.0.6/arlq/_version.py
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)    19706 2023-04-15 12:56:17.000000 arlq-1.0.6/arlq/arlq.py
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-15 13:02:16.401621 arlq-1.0.6/arlq.egg-info/
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1046 2023-04-15 13:02:16.000000 arlq-1.0.6/arlq.egg-info/PKG-INFO
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      253 2023-04-15 13:02:16.000000 arlq-1.0.6/arlq.egg-info/SOURCES.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        1 2023-04-15 13:02:16.000000 arlq-1.0.6/arlq.egg-info/dependency_links.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       36 2023-04-15 13:02:16.000000 arlq-1.0.6/arlq.egg-info/entry_points.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       43 2023-04-15 13:02:16.000000 arlq-1.0.6/arlq.egg-info/requires.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        5 2023-04-15 13:02:16.000000 arlq-1.0.6/arlq.egg-info/top_level.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      836 2023-04-15 13:02:16.401621 arlq-1.0.6/setup.cfg
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       38 2023-04-14 17:26:18.000000 arlq-1.0.6/setup.py
```

### Comparing `arlq-1.0.5/LICENSE` & `arlq-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `arlq-1.0.5/PKG-INFO` & `arlq-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arlq
-Version: 1.0.5
+Version: 1.0.6
 Summary: ARQL, another rogue-like quest game.
 Home-page: https://github.com/tos-kamiya/arlq
 Author: Toshihiro Kamiya
 Author-email: kamiya@mbj.nifty.com
 License: BSD 2-Clause License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `arlq-1.0.5/README.md` & `arlq-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `arlq-1.0.5/arlq/arlq.py` & `arlq-1.0.6/arlq/arlq.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,26 +294,27 @@
                 stdscr.addstr(m.y, m.x, ch, curses.color_pair(3) | attr)
         elif isinstance(o, Treasure):
             t = o
             if CHAR_TREASURE in encountered_types:
                 stdscr.addstr(t.y, t.x, CHAR_TREASURE, curses.color_pair(4) | curses.A_BOLD)
 
     if show_entities:
+        attr = curses.A_DIM
         for o in objects:
             if isinstance(o, Monster):
                 m = o
                 if torched[m.y][m.x] != 0:
                     continue
 
                 ch = m.kind.char
-                stdscr.addstr(m.y, m.x, ch)
+                stdscr.addstr(m.y, m.x, ch, attr)
             elif isinstance(o, Treasure):
                 t = o
                 if CHAR_TREASURE not in encountered_types:
-                    stdscr.addstr(t.y, t.x, CHAR_TREASURE)
+                    stdscr.addstr(t.y, t.x, CHAR_TREASURE, attr)
 
 
 def player_attack_by_level(player: Player) -> int:
     if player.item == ITEM_SWORD:
         return player.level * 3
     elif player.item == ITEM_POISONED:
         return (player.level + 2) // 3
@@ -345,15 +346,15 @@
     buf = []
     buf.append("HRS: %d" % hours)
     buf.append(level_str)
     if beatable is not None:
         buf.append("> %s" % beatable.char)
     buf.append("FOOD: %d" % player.food)
     buf.append(item_str)
-    buf.append("/ Press [Q] to exit")
+    buf.append("/ [Q] to exit")
     stdscr.addstr(FIELD_HEIGHT, 0, "  ".join(buf))
 
     if message:
         stdscr.addstr(FIELD_HEIGHT + 1, 0, message)
 
 
 def key_to_dir(key: int) -> Optional[Point]:
@@ -587,15 +588,15 @@
     curses.cbreak()
     curses.curs_set(0)
 
     curses.start_color()
     curses.use_default_colors()
     curses.init_pair(1, curses.COLOR_GREEN, -1)  # wall
     curses.init_pair(2, curses.COLOR_BLUE, -1)  # player
-    curses.init_pair(3, curses.COLOR_RED, -1)  # monster
+    curses.init_pair(3, curses.COLOR_WHITE, -1)  # monster
     curses.init_pair(4, curses.COLOR_YELLOW, -1)  # treasure
 
     try:
         curses.wrapper(curses_main)
     except TerminalSizeSmall as e:
         sys.exit("Error: Terminal size too small. Minimum size is: %d x %d" % (FIELD_WIDTH, FIELD_HEIGHT + 2))
     finally:
```

### Comparing `arlq-1.0.5/arlq.egg-info/PKG-INFO` & `arlq-1.0.6/arlq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arlq
-Version: 1.0.5
+Version: 1.0.6
 Summary: ARQL, another rogue-like quest game.
 Home-page: https://github.com/tos-kamiya/arlq
 Author: Toshihiro Kamiya
 Author-email: kamiya@mbj.nifty.com
 License: BSD 2-Clause License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `arlq-1.0.5/setup.cfg` & `arlq-1.0.6/setup.cfg`

 * *Files identical despite different names*

