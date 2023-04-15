# Comparing `tmp/arlq-1.0.2.tar.gz` & `tmp/arlq-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arlq-1.0.2.tar", last modified: Fri Apr 14 18:06:10 2023, max compression
+gzip compressed data, was "arlq-1.0.4.tar", last modified: Sat Apr 15 09:42:59 2023, max compression
```

## Comparing `arlq-1.0.2.tar` & `arlq-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-14 18:06:10.966935 arlq-1.0.2/
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1305 2023-04-14 17:26:18.000000 arlq-1.0.2/LICENSE
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1046 2023-04-14 18:06:10.966935 arlq-1.0.2/PKG-INFO
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     4216 2023-04-14 17:16:04.000000 arlq-1.0.2/README.md
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-14 18:06:10.966935 arlq-1.0.2/arlq/
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       57 2023-04-14 17:26:18.000000 arlq-1.0.2/arlq/__init__.py
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       22 2023-04-14 18:05:06.000000 arlq-1.0.2/arlq/_version.py
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)    17399 2023-04-14 18:00:27.000000 arlq-1.0.2/arlq/arlq.py
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-14 18:06:10.966935 arlq-1.0.2/arlq.egg-info/
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1046 2023-04-14 18:06:10.000000 arlq-1.0.2/arlq.egg-info/PKG-INFO
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      253 2023-04-14 18:06:10.000000 arlq-1.0.2/arlq.egg-info/SOURCES.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        1 2023-04-14 18:06:10.000000 arlq-1.0.2/arlq.egg-info/dependency_links.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       36 2023-04-14 18:06:10.000000 arlq-1.0.2/arlq.egg-info/entry_points.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       43 2023-04-14 18:06:10.000000 arlq-1.0.2/arlq.egg-info/requires.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        5 2023-04-14 18:06:10.000000 arlq-1.0.2/arlq.egg-info/top_level.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      836 2023-04-14 18:06:10.966935 arlq-1.0.2/setup.cfg
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       38 2023-04-14 17:26:18.000000 arlq-1.0.2/setup.py
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-15 09:42:59.184526 arlq-1.0.4/
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1305 2023-04-14 17:26:18.000000 arlq-1.0.4/LICENSE
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1046 2023-04-15 09:42:59.184526 arlq-1.0.4/PKG-INFO
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     4375 2023-04-15 09:27:53.000000 arlq-1.0.4/README.md
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-15 09:42:59.184526 arlq-1.0.4/arlq/
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       57 2023-04-14 17:26:18.000000 arlq-1.0.4/arlq/__init__.py
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       22 2023-04-15 09:00:02.000000 arlq-1.0.4/arlq/_version.py
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)    19597 2023-04-15 09:28:26.000000 arlq-1.0.4/arlq/arlq.py
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-15 09:42:59.184526 arlq-1.0.4/arlq.egg-info/
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1046 2023-04-15 09:42:59.000000 arlq-1.0.4/arlq.egg-info/PKG-INFO
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      253 2023-04-15 09:42:59.000000 arlq-1.0.4/arlq.egg-info/SOURCES.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        1 2023-04-15 09:42:59.000000 arlq-1.0.4/arlq.egg-info/dependency_links.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       36 2023-04-15 09:42:59.000000 arlq-1.0.4/arlq.egg-info/entry_points.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       43 2023-04-15 09:42:59.000000 arlq-1.0.4/arlq.egg-info/requires.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        5 2023-04-15 09:42:59.000000 arlq-1.0.4/arlq.egg-info/top_level.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      836 2023-04-15 09:42:59.184526 arlq-1.0.4/setup.cfg
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       38 2023-04-14 17:26:18.000000 arlq-1.0.4/setup.py
```

### Comparing `arlq-1.0.2/LICENSE` & `arlq-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `arlq-1.0.2/PKG-INFO` & `arlq-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arlq
-Version: 1.0.2
+Version: 1.0.4
 Summary: ARQL, another rogue-like quest game.
 Home-page: https://github.com/tos-kamiya/arlq
 Author: Toshihiro Kamiya
 Author-email: kamiya@mbj.nifty.com
 License: BSD 2-Clause License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `arlq-1.0.2/README.md` & `arlq-1.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 |Monster Display, Name | Description |
 |---|---|
 |a Amoeba|Weak enough for the player to defeat from the start. Good for leveling up.|
 |b Bison|Second weakest. Gives lots of food. Hunt a Bison when you're hungry!|
 |c Chimera|Fairly strong. Carries a sword that you can obtain when defeated. With the sword, your attack power triples in the next battle.|
 |d Komodo Dragon|Strong. If defeated, provides a lot of food, but being poisoned, your attack power will be reduced to one-third in the next battle.|
 |f Fairy|Not a foe. Follows you when you come in contact. Gives you a small blessing.|
+|g Gorgon|A monster that petrifies you instantly just by making eye contact. Without a fairy companion, your body will be petrified for 48 hours! Be careful!|
 |A Rare Amoeba|A rare Amoeba that boosts your level significantly!|
 |B Rare Bison|So delicious that you'll probably eat much more than a regular Bison|
 |C Rare Chimera|In addition to the sword, it possesses clairvoyance.|
 |D Dragon|Strong. Defeating the Dragon reveals the treasure chest ("T") location. Even if you don't defeat it, you'll be able to recognize the chest.|
 |E Elemental|Not a foe. Teleports the player to a random location in the dungeon. Offers extra services for high-level players.|
 
 ## License
```

### Comparing `arlq-1.0.2/arlq/arlq.py` & `arlq-1.0.4/arlq/arlq.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from typing import Dict, List, Optional, Set, Tuple
 
 import argparse
 import curses
 import math
-import platform
 import random
 import sys
 
 try:
     from ._version import __version__
 except:
-    __version__ = '(unknown)'
+    __version__ = "(unknown)"
 
 ROOM_WIDTH = 5
 ROOM_HEIGHT = 4
 ROOM_NUM_X = 12
 ROOM_NUM_Y = 4
 FIELD_WIDTH = (ROOM_WIDTH + 1) * ROOM_NUM_X + 1
 FIELD_HEIGHT = (ROOM_HEIGHT + 1) * ROOM_NUM_Y + 1
@@ -24,28 +23,30 @@
 FOOD_BISON = 40
 FOOD_SPECIAL_BISON = 80
 FOOD_AMOEBA = 8
 FOOD_CHIMERA = 8
 FOOD_COMODO_DRAGON = 30
 FOOD_DRAGON = 10
 FOOD_ELEMENTAL = 0
+FOOD_GORGON = -48
 
-ITEM_BISON_MEAT = 'Bison Meat'
-ITEM_SWORD = 'Sword'
-ITEM_POISONED = 'Poisoned'
-ITEM_RANDOM_TRANSPORT = 'Random Trans.'
-ITEM_SPECIAL_EXP = 'Special Exp.'
-ITEM_SPECIAL_BISON_MEAT = 'Bison Meat++'
-ITEM_SWORD_AND_CLAIRVOYANCE = 'Sword & Eye'
-ITEM_TREASURE_POINTER = 'Treasure Ptr.'
+ITEM_BISON_MEAT = "Bison Meat"
+ITEM_SWORD = "Sword"
+ITEM_POISONED = "Poisoned"
+ITEM_RANDOM_TRANSPORT = "Random Trans."
+ITEM_SPECIAL_EXP = "Special Exp."
+ITEM_SPECIAL_BISON_MEAT = "Bison Meat++"
+ITEM_SWORD_AND_CLAIRVOYANCE = "Sword & Eye"
+ITEM_TREASURE_POINTER = "Treasure Ptr."
+ITEM_STONED = "Stoned"
 
-COMPANION_FAIRY = 'Fairy'
+COMPANION_FAIRY = "Fairy"
 
-CHAR_DRAGON = 'D'
-CHAR_TREASURE = 'T'
+CHAR_DRAGON = "D"
+CHAR_TREASURE = "T"
 
 
 Point = Tuple[int, int]
 Edge = Tuple[Point, Point]
 
 
 def gen_maze(width: int, height: int) -> List[Edge]:
@@ -140,67 +141,73 @@
 class Monster(Entity):
     def __init__(self, x, y, kind):
         super().__init__(x, y)
         self.kind = kind
 
 
 class MonsterKind:
-    def __init__(self, char, level, feed, item = '', companion = ''):
+    def __init__(self, char, level, feed, item="", companion=""):
         self.char = char
         self.level = level
         self.item = item
         self.feed = feed
         self.companion = companion
 
 
 # Combine monster_data and item_data into a single dict
 MONSTER_KINDS: List[MonsterKind] = [
-    MonsterKind('a', 1, FOOD_AMOEBA),  # Amoeba
-    MonsterKind('b', 3, FOOD_BISON, item=ITEM_BISON_MEAT),  # Bison
-    MonsterKind('c', 6, FOOD_CHIMERA, item=ITEM_SWORD),  # Chimera
-    MonsterKind('d', 15, FOOD_COMODO_DRAGON, item=ITEM_POISONED),  # Comodo Dragon
+    MonsterKind("a", 1, FOOD_AMOEBA),  # Amoeba
+    MonsterKind("b", 3, FOOD_BISON, item=ITEM_BISON_MEAT),  # Bison
+    MonsterKind("c", 6, FOOD_CHIMERA, item=ITEM_SWORD),  # Chimera
+    MonsterKind("d", 15, FOOD_COMODO_DRAGON, item=ITEM_POISONED),  # Comodo Dragon
     MonsterKind(CHAR_DRAGON, 15, FOOD_DRAGON, item=ITEM_TREASURE_POINTER),  # Dragon
-    MonsterKind('E', 20, FOOD_ELEMENTAL, item=ITEM_RANDOM_TRANSPORT),  # Elemental
-    MonsterKind('f', 0, 0, companion=COMPANION_FAIRY),  # Fairy
+    MonsterKind("E", 20, FOOD_ELEMENTAL, item=ITEM_RANDOM_TRANSPORT),  # Elemental
+    MonsterKind("f", 0, 0, companion=COMPANION_FAIRY),  # Fairy
+    MonsterKind("g", 0, FOOD_GORGON, item=ITEM_STONED),  # Gorgon
 ]
 
 RARE_MONSTER_KINDS: List[MonsterKind] = [
-    MonsterKind('A', 1, FOOD_AMOEBA, item=ITEM_SPECIAL_EXP),  # Amoeba rare
-    MonsterKind('B', 3, FOOD_SPECIAL_BISON, item=ITEM_SPECIAL_BISON_MEAT),  # Bison rare
-    MonsterKind('C', 6, FOOD_CHIMERA, item=ITEM_SWORD_AND_CLAIRVOYANCE),  # Chimera rare
+    MonsterKind("A", 1, FOOD_AMOEBA, item=ITEM_SPECIAL_EXP),  # Amoeba rare
+    MonsterKind("B", 3, FOOD_SPECIAL_BISON, item=ITEM_SPECIAL_BISON_MEAT),  # Bison rare
+    MonsterKind("C", 6, FOOD_CHIMERA, item=ITEM_SWORD_AND_CLAIRVOYANCE),  # Chimera rare
 ]
 
 MONSTER_KIND_POPULATION: Dict[str, int] = {
-    'a': 20,
-    'b': 4,
-    'c': 4,
-    'd': 4,
-    'D': 1,
-    'E': 2,
-    'f': 1,
+    "a": 20,
+    "b": 4,
+    "c": 4,
+    "d": 4,
+    "D": 1,
+    "E": 2,
+    "f": 1,
+    "g": 1,
 }
 
 
 def find_random_place(objects: List[Entity], field: List[List[str]], distance: int) -> Point:
     places = [(o.x, o.y) for o in objects]
     while True:
         x = random.randint(1, FIELD_WIDTH - 2)
         y = random.randint(1, FIELD_HEIGHT - 2)
-        if field[y][x] == ' ' and field[y][x + 1] == ' ' and not any(abs(p[0] - x) <= distance and abs(p[1] - y) <= distance for p in places):
+        if (
+            field[y][x] == " "
+            and field[y][x + 1] == " "
+            and not any(abs(p[0] - x) <= distance and abs(p[1] - y) <= distance for p in places)
+        ):
             return x, y
 
 
 def spawn_monsters(objects: List[Entity], field: List[List[str]]) -> None:
     """
     Spawn monsters in the game by finding random places on the field.
-    
+
     Args:
     - objects: a list of objects in the game
     - field: the game field
-    
+
     This function modifies the objects list by adding newly spawned monsters.
     """
 
     for kind in MONSTER_KINDS:
         for _ in range(MONSTER_KIND_POPULATION[kind.char]):
             x, y = find_random_place(objects, field, 2)
             m = Monster(x, y, kind)
@@ -209,81 +216,105 @@
     x, y = find_random_place(objects, field, 2)
     m = Monster(x, y, kind)
     objects.append(m)
 
 
 def create_field() -> List[List[str]]:
     # Create field filled with spaces
-    field = [[' ' for _ in range(FIELD_WIDTH)] for _ in range(FIELD_HEIGHT)]
+    field = [[" " for _ in range(FIELD_WIDTH)] for _ in range(FIELD_HEIGHT)]
 
     # Create walls
     for ry in range(ROOM_NUM_Y + 1):
         y = ry * (ROOM_HEIGHT + 1)
         for x in range(0, FIELD_WIDTH):
-            field[y][x] = '#'
+            field[y][x] = "#"
     for rx in range(ROOM_NUM_X + 1):
         x = rx * (ROOM_WIDTH + 1)
         for y in range(0, FIELD_HEIGHT):
-            field[y][x] = '#'
+            field[y][x] = "#"
 
     # Create corridors
     edges = gen_maze(ROOM_NUM_X, ROOM_NUM_Y)
     for edge in edges:
         (x1, y1), (x2, y2) = sorted(edge)
         assert x1 <= x2
         assert y1 <= y2
         d = random.randrange(3) + 1  # 1, 2, 3
         if y1 == y2:
             for y in range(ROOM_HEIGHT - 2):
-                field[y1 * (ROOM_HEIGHT + 1) + d + y][x2 * (ROOM_WIDTH + 1)] = ' '
+                field[y1 * (ROOM_HEIGHT + 1) + d + y][x2 * (ROOM_WIDTH + 1)] = " "
         else:
             assert x1 == x2
             for x in range(ROOM_WIDTH - 2):
-                field[y2 * (ROOM_HEIGHT + 1)][x1 * (ROOM_WIDTH + 1) + d + x] = ' '
+                field[y2 * (ROOM_HEIGHT + 1)][x1 * (ROOM_WIDTH + 1) + d + x] = " "
 
     return field
 
 
-def draw_stage(stdscr: curses.window, objects: List[Entity], field: List[List[str]], torched: List[List[int]], encountered_types: Set[str], no_hide: Optional[bool] = False) -> None:
-    hide_on = not no_hide
-    for y, row in enumerate(field):
-        for x, cell in enumerate(row):
-            if (hide_on or cell == ' ') and torched[y][x] == 0:
-                stdscr.addstr(y, x, '.', curses.A_DIM)
-            else:
-                if cell == '#':
-                    stdscr.addstr(y, x, '#', curses.color_pair(1))
-                else:
-                    assert cell == ' '
-                    stdscr.addstr(y, x, ' ')
-
+def draw_stage(
+    stdscr: curses.window,
+    objects: List[Entity],
+    field: List[List[str]],
+    torched: List[List[int]],
+    encountered_types: Set[str],
+    show_entities: Optional[bool] = False,
+) -> None:
+    player, px, py = None, None, None
     for o in objects:
         if isinstance(o, Player):
             player = o
-            stdscr.addstr(player.y, player.x, '@', curses.color_pair(2) | curses.A_BOLD)
-            if player.companion:
-                stdscr.addstr(player.y, player.x + 1, "'", curses.color_pair(2) | curses.A_BOLD)
+            px, py = player.x, player.y
+    assert player is not None and px is not None and py is not None
+
+    if player.companion:
+        stdscr.addstr(py, px + 1, "'", curses.color_pair(2) | curses.A_BOLD)
+
+    for y, row in enumerate(field):
+        for x, cell in enumerate(row):
+            if (not show_entities or cell == " ") and torched[y][x] == 0:
+                stdscr.addstr(y, x, ".", curses.A_DIM)
+            elif cell == "#":
+                stdscr.addstr(y, x, "#", curses.color_pair(1))
+
+    stdscr.addstr(py, px, "@", curses.color_pair(2) | curses.A_BOLD)
 
     for o in objects:
         if isinstance(o, Monster):
             m = o
-            if hide_on and torched[m.y][m.x] == 0:
+            if torched[m.y][m.x] == 0:
                 continue
 
             ch = m.kind.char
-            if hide_on and m.kind.char not in encountered_types:
-                stdscr.addstr(m.y, m.x, '?', curses.color_pair(3))
+            if m.kind.char not in encountered_types:
+                if show_entities:
+                    stdscr.addstr(m.y, m.x, ch)
+                else:
+                    stdscr.addstr(m.y, m.x, "?", curses.color_pair(3))
             else:
-                attr = curses.A_BOLD if 'A' <= ch <= 'Z' else 0
+                attr = curses.A_BOLD if "A" <= ch <= "Z" else 0
                 stdscr.addstr(m.y, m.x, ch, curses.color_pair(3) | attr)
         elif isinstance(o, Treasure):
             t = o
             if CHAR_TREASURE in encountered_types:
                 stdscr.addstr(t.y, t.x, CHAR_TREASURE, curses.color_pair(4) | curses.A_BOLD)
 
+    if show_entities:
+        for o in objects:
+            if isinstance(o, Monster):
+                m = o
+                if torched[m.y][m.x] != 0:
+                    continue
+
+                ch = m.kind.char
+                stdscr.addstr(m.y, m.x, ch)
+            elif isinstance(o, Treasure):
+                t = o
+                if CHAR_TREASURE not in encountered_types:
+                    stdscr.addstr(t.y, t.x, CHAR_TREASURE)
+
 
 def player_attack_by_level(player: Player) -> int:
     if player.item == ITEM_SWORD:
         return player.level * 3
     elif player.item == ITEM_POISONED:
         return (player.level + 2) // 3
     else:
@@ -314,44 +345,44 @@
     buf = []
     buf.append("HRS: %d" % hours)
     buf.append(level_str)
     if beatable is not None:
         buf.append("> %s" % beatable.char)
     buf.append("FOOD: %d" % player.food)
     buf.append(item_str)
-    buf.append('/ Press [Q] to exit')
+    buf.append("/ Press [Q] to exit")
     stdscr.addstr(FIELD_HEIGHT, 0, "  ".join(buf))
 
     if message:
         stdscr.addstr(FIELD_HEIGHT + 1, 0, message)
 
 
 def key_to_dir(key: int) -> Optional[Point]:
     dx, dy = 0, 0
-    if key in [ord('w'), curses.KEY_UP]:
+    if key in [ord("w"), curses.KEY_UP]:
         dy = -1
-    elif key in [ord('a'), curses.KEY_LEFT]:
+    elif key in [ord("a"), curses.KEY_LEFT]:
         dx = -1
-    elif key in [ord('s'), curses.KEY_DOWN]:
+    elif key in [ord("s"), curses.KEY_DOWN]:
         dy = 1
-    elif key in [ord('d'), curses.KEY_RIGHT]:
+    elif key in [ord("d"), curses.KEY_RIGHT]:
         dx = 1
     else:
         return None
     return dx, dy
 
 
 def update_torched(torched: List[List[int]], player: Player, torch_radius: int) -> None:
     if player.companion == COMPANION_FAIRY:
         torch_radius += 1
 
     for dy in range(-torch_radius, torch_radius + 1):
         y = player.y + dy
         if 0 <= y < FIELD_HEIGHT:
-            w = int(math.sqrt((torch_radius*1.2)**2 - dy**2) + 0.5)
+            w = int(math.sqrt((torch_radius * 1.2) ** 2 - dy**2) + 0.5)
             for dx in range(-w, w + 1):
                 x = player.x + dx
                 if 0 <= x < FIELD_WIDTH:
                     torched[y][x] = 1
 
 
 args_box: List[argparse.Namespace] = []
@@ -384,27 +415,30 @@
     if args.large_torch:
         torch_radius = 5
     elif args.small_torch:
         torch_radius = 3
 
     def consume_player_item(player: Player) -> str:
         item = player.item
-        message = ''
+        message = ""
         if item in [ITEM_BISON_MEAT, ITEM_SPECIAL_BISON_MEAT]:
             message = "-- Stuffed."
-            player.item = ''
+            player.item = ""
         elif item == ITEM_TREASURE_POINTER:
             message = "-- Sparkle."
-            player.item = ''
+            player.item = ""
         elif item == ITEM_SPECIAL_EXP:
             message = "-- Special Exp."
-            player.item = ''
+            player.item = ""
         elif item == ITEM_SWORD_AND_CLAIRVOYANCE:
             message = "-- Clairvoyance."
             player.item = ITEM_SWORD
+        elif item == ITEM_STONED:
+            message = "-- Stoned."
+            player.item = ""
         return message
 
     stdscr.keypad(True)
 
     message: Optional[str] = None
     hours: int = -1
     while True:
@@ -416,121 +450,135 @@
             message = ">> Starved to Death. <<"
             break  # end game
 
         # Show the field
         update_torched(torched, player, torch_radius)
         temp_message = consume_player_item(player)
         stdscr.clear()
-        draw_stage(stdscr, objects, field, torched, encountered_types, no_hide=args.debug_no_hide)
+        draw_stage(stdscr, objects, field, torched, encountered_types, show_entities=args.debug_show_entities)
         draw_status_bar(stdscr, player, hours, message=message or temp_message)
         stdscr.refresh()
 
         # Move player
         while True:
             key = stdscr.getch()
             d = key_to_dir(key)
             if d is None:
                 return
 
             dx, dy = d
             new_x, new_y = player.x + dx, player.y + dy
-            if field[new_y][new_x] == ' ':  # if the cell is not a wall
+            if field[new_y][new_x] == " ":  # if the cell is not a wall
                 player.x, player.y = new_x, new_y
                 break
 
         # Find encountered object
-        enc_obj: Optional[Entity] = None
-        enc_obj_i: int = -1
-        for enc_obj_i, o in enumerate(objects):
-            if (not isinstance(o, Player)) and o.x == player.x and o.y == player.y:
-                enc_obj = o
-                break
-        if enc_obj is None:
-            continue  # while True
-
-        if isinstance(enc_obj, Treasure):
-            if CHAR_DRAGON in encountered_types:
-                encountered_types.add(CHAR_TREASURE)
-                message = ">> Won the Treasure! <<"
-                break  # end game
-        elif isinstance(enc_obj, Monster):
-            m = enc_obj
-            encountered_types.add(m.kind.char)
-            player_attak = player_attack_by_level(player)
-
-            if player_attak < m.kind.level:
-                # respawn
-                player.x, player.y = find_random_place(objects, field, 2)
-                player.item = ''
-                player.item_taken_from = ''
-                player.food = min(player.food, FOOD_INIT)
-            else:
-                if m.kind.item == ITEM_RANDOM_TRANSPORT:
-                    pass
-                elif m.kind.item == ITEM_SPECIAL_EXP:
-                    player.level += 7
-                else:
-                    player.level += 1
-
-                if m.kind.item == ITEM_SWORD_AND_CLAIRVOYANCE:
-                    update_torched(torched, player, torch_radius * 4)
-
-                if m.kind.item == ITEM_TREASURE_POINTER:
+        enc_obj_infos: List[Tuple[int, Entity]] = []
+        sur_obj_infos: List[Tuple[int, Entity]] = []
+        for i, o in enumerate(objects):
+            if not isinstance(o, Player):
+                dx = abs(o.x - player.x)
+                dy = abs(o.y - player.y)
+                if dx == 0 and dy == 0:
+                    enc_obj_infos.append((i, o))
+                elif dx <= 1 and dy <= 1:
+                    sur_obj_infos.append((i, o))
+
+        # Actions & events (combats, state changes, etc)
+        for enc_obj_i, enc_obj in enc_obj_infos:
+            if isinstance(enc_obj, Treasure):
+                if CHAR_DRAGON in encountered_types:
                     encountered_types.add(CHAR_TREASURE)
-
-                player.food = min(FOOD_MAX, player.food + m.kind.feed)
-
-                if m.kind.companion:
-                    player.companion = m.kind.companion
-
-                if m.kind.item == ITEM_RANDOM_TRANSPORT:
-                    player.x, player.y = find_random_place(objects, field, 2)
-                    m.x, m.y = player.x + 1, player.y
+                    message = ">> Won the Treasure! <<"
+                    break  # end game
+            elif isinstance(enc_obj, Monster):
+                m = enc_obj
+                encountered_types.add(m.kind.char)
+                player_attack = player_attack_by_level(player)
+
+                if player_attack < m.kind.level:
+                    if m.kind.item == ITEM_RANDOM_TRANSPORT:
+                        player.x, player.y = find_random_place(objects, field, 2)
+                    else:
+                        # respawn
+                        player.x, player.y = find_random_place(objects, field, 2)
+                        player.item = ""
+                        player.item_taken_from = ""
+                        player.food = min(player.food, FOOD_INIT)
                 else:
-                    del objects[enc_obj_i]
-                    player.item = m.kind.item
-                    player.item_taken_from = m.kind.char
+                    if m.kind.item == ITEM_RANDOM_TRANSPORT:
+                        pass  # do not change player level
+                    elif m.kind.item == ITEM_SPECIAL_EXP:
+                        player.level += 7
+                    else:
+                        player.level += 1
+
+                    if m.kind.item == ITEM_SWORD_AND_CLAIRVOYANCE:
+                        update_torched(torched, player, torch_radius * 4)
+
+                    if m.kind.item == ITEM_TREASURE_POINTER:
+                        encountered_types.add(CHAR_TREASURE)
+
+                    if m.kind.item == ITEM_STONED:
+                        if player.companion == COMPANION_FAIRY:
+                            player.companion = ''
+                        else:
+                            hours += -m.kind.feed
+                            player.food += m.kind.feed
+                            if player.food < 1:
+                                player.food = 1
+                    else:
+                        player.food = min(FOOD_MAX, player.food + m.kind.feed)
+
+                    if m.kind.companion:
+                        player.companion = m.kind.companion
+
+                    if m.kind.item == ITEM_RANDOM_TRANSPORT:
+                        player.x, player.y = find_random_place(objects, field, 2)
+                        m.x, m.y = player.x + 1, player.y
+                    else:
+                        del objects[enc_obj_i]
+                        player.item = m.kind.item
+                        player.item_taken_from = m.kind.char
+
+        for sur_obj_i, sur_obj in sur_obj_infos:
+            if isinstance(sur_obj, Treasure):
+                if CHAR_DRAGON in encountered_types:
+                    encountered_types.add(CHAR_TREASURE)
 
     update_torched(torched, player, torch_radius)
 
     temp_message = consume_player_item(player)
     stdscr.clear()
-    draw_stage(stdscr, objects, field, torched, encountered_types, no_hide=args.debug_no_hide)
+    draw_stage(stdscr, objects, field, torched, encountered_types, show_entities=args.debug_show_entities)
     draw_status_bar(stdscr, player, hours, message=message or temp_message)
     stdscr.refresh()
 
     while True:
         key = stdscr.getch()
-        if key == ord('q'):
+        if key == ord("q"):
             break
+        elif key == ord("r"):
+            stdscr.clear()
+            draw_stage(stdscr, objects, field, torched, encountered_types, show_entities=True)
+            draw_status_bar(stdscr, player, hours, message=message or temp_message)
+            stdscr.refresh()
 
 
 def main():
     parser = argparse.ArgumentParser(
-        description='A Rogue-Like game.',
+        description="A Rogue-Like game.",
     )
 
-    parser.add_argument('--version', action='version', version='%(prog)s ' + __version__)
+    parser.add_argument("--version", action="version", version="%(prog)s " + __version__)
 
     g = parser.add_mutually_exclusive_group()
-    g.add_argument(
-        '-l', '--large-torch',
-        action='store_true',
-        help='Large torch.'
-    )
-    g.add_argument(
-        '-s', '--small-torch',
-        action='store_true',
-        help='Small torch.'
-    )
-    g.add_argument(
-        '--debug-no-hide',
-        action='store_true',
-        help='Debug option.'
-    )
+    g.add_argument("-l", "--large-torch", action="store_true", help="Large torch.")
+    g.add_argument("-s", "--small-torch", action="store_true", help="Small torch.")
+    g.add_argument("--debug-show-entities", action="store_true", help="Debug option.")
 
     args = parser.parse_args()
     args_box.append(args)
 
     curses.initscr()
     curses.noecho()
     curses.cbreak()
```

### Comparing `arlq-1.0.2/arlq.egg-info/PKG-INFO` & `arlq-1.0.4/arlq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arlq
-Version: 1.0.2
+Version: 1.0.4
 Summary: ARQL, another rogue-like quest game.
 Home-page: https://github.com/tos-kamiya/arlq
 Author: Toshihiro Kamiya
 Author-email: kamiya@mbj.nifty.com
 License: BSD 2-Clause License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `arlq-1.0.2/setup.cfg` & `arlq-1.0.4/setup.cfg`

 * *Files identical despite different names*

