# Comparing `tmp/chessmaker-0.1.2.tar.gz` & `tmp/chessmaker-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chessmaker-0.1.2.tar", last modified: Thu Apr 13 00:44:40 2023, max compression
+gzip compressed data, was "chessmaker-0.2.tar", max compression
```

## Comparing `chessmaker-0.1.2.tar` & `chessmaker-0.2.tar`

### file list

```diff
@@ -1,63 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 00:44:40.208286 chessmaker-0.1.2/
--rw-rw-rw-   0        0        0    35184 2023-04-05 10:50:17.000000 chessmaker-0.1.2/LICENSE
--rw-rw-rw-   0        0        0    43007 2023-04-13 00:44:40.207286 chessmaker-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1618 2023-04-13 00:44:26.000000 chessmaker-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 00:44:40.144287 chessmaker-0.1.2/chessmaker/
--rw-rw-rw-   0        0        0      159 2023-04-12 23:23:56.000000 chessmaker-0.1.2/chessmaker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 00:44:40.156288 chessmaker-0.1.2/chessmaker/chess/
--rw-rw-rw-   0        0        0      198 2023-04-12 23:20:16.000000 chessmaker-0.1.2/chessmaker/chess/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 00:44:40.167287 chessmaker-0.1.2/chessmaker/chess/base/
--rw-rw-rw-   0        0        0      686 2023-04-12 23:23:13.000000 chessmaker-0.1.2/chessmaker/chess/base/__init__.py
--rw-rw-rw-   0        0        0     6797 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/base/board.py
--rw-rw-rw-   0        0        0     1095 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/base/game.py
--rw-rw-rw-   0        0        0      275 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/base/move_option.py
--rw-rw-rw-   0        0        0     3472 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/base/piece.py
--rw-rw-rw-   0        0        0      583 2023-04-12 22:32:25.000000 chessmaker-0.1.2/chessmaker/chess/base/player.py
--rw-rw-rw-   0        0        0      241 2023-04-12 22:32:25.000000 chessmaker-0.1.2/chessmaker/chess/base/position.py
--rw-rw-rw-   0        0        0      708 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/base/rule.py
--rw-rw-rw-   0        0        0     2023 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/base/square.py
--rw-rw-rw-   0        0        0     4049 2023-04-13 00:44:26.000000 chessmaker-0.1.2/chessmaker/chess/game_factory.py
-drwxrwxrwx   0        0        0        0 2023-04-13 00:44:40.178287 chessmaker-0.1.2/chessmaker/chess/pieces/
--rw-rw-rw-   0        0        0      607 2023-04-12 23:23:13.000000 chessmaker-0.1.2/chessmaker/chess/pieces/__init__.py
--rw-rw-rw-   0        0        0      659 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/pieces/bishop.py
--rw-rw-rw-   0        0        0     6570 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/pieces/king.py
--rw-rw-rw-   0        0        0      887 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/pieces/knight.py
-drwxrwxrwx   0        0        0        0 2023-04-13 00:44:40.185287 chessmaker-0.1.2/chessmaker/chess/pieces/knook/
--rw-rw-rw-   0        0        0      191 2023-04-12 23:23:13.000000 chessmaker-0.1.2/chessmaker/chess/pieces/knook/__init__.py
--rw-rw-rw-   0        0        0      975 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/pieces/knook/knook.py
--rw-rw-rw-   0        0        0       30 2023-04-12 22:32:25.000000 chessmaker-0.1.2/chessmaker/chess/pieces/knook/knookable.py
--rw-rw-rw-   0        0        0     1055 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/pieces/knook/knookable_knight.py
--rw-rw-rw-   0        0        0     1155 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/pieces/knook/knookable_rook.py
--rw-rw-rw-   0        0        0     1528 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/pieces/knook/merge_to_knook.py
--rw-rw-rw-   0        0        0     5542 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/pieces/pawn.py
--rw-rw-rw-   0        0        0     2458 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/pieces/piece_utils.py
--rw-rw-rw-   0        0        0      792 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/pieces/queen.py
--rw-rw-rw-   0        0        0     1064 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/pieces/rook.py
-drwxrwxrwx   0        0        0        0 2023-04-13 00:44:40.188286 chessmaker-0.1.2/chessmaker/chess/results/
--rw-rw-rw-   0        0        0       44 2023-04-12 23:20:15.000000 chessmaker-0.1.2/chessmaker/chess/results/__init__.py
--rw-rw-rw-   0        0        0     2428 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/results/simple_result.py
-drwxrwxrwx   0        0        0        0 2023-04-13 00:44:40.197287 chessmaker-0.1.2/chessmaker/chess/rules/
--rw-rw-rw-   0        0        0      256 2023-04-13 00:44:26.000000 chessmaker-0.1.2/chessmaker/chess/rules/__init__.py
--rw-rw-rw-   0        0        0     3540 2023-04-13 00:00:02.000000 chessmaker-0.1.2/chessmaker/chess/rules/beta_decay.py
--rw-rw-rw-   0        0        0     1929 2023-04-13 00:44:26.000000 chessmaker-0.1.2/chessmaker/chess/rules/forced_en_passant.py
--rw-rw-rw-   0        0        0     3387 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/rules/il_vaticano.py
--rw-rw-rw-   0        0        0     2695 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/rules/knight_boosting.py
--rw-rw-rw-   0        0        0     1685 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/rules/omnipotent_f6_pawn.py
--rw-rw-rw-   0        0        0     2254 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/chess/rules/siberian_swipe.py
-drwxrwxrwx   0        0        0        0 2023-04-13 00:44:40.199286 chessmaker-0.1.2/chessmaker/clients/
--rw-rw-rw-   0        0        0       52 2023-04-12 23:20:16.000000 chessmaker-0.1.2/chessmaker/clients/__init__.py
--rw-rw-rw-   0        0        0    13709 2023-04-13 00:44:26.000000 chessmaker-0.1.2/chessmaker/clients/pywebio_ui.py
--rw-rw-rw-   0        0        0      278 2023-04-12 22:32:25.000000 chessmaker-0.1.2/chessmaker/cloneable.py
-drwxrwxrwx   0        0        0        0 2023-04-13 00:44:40.205286 chessmaker-0.1.2/chessmaker/events/
--rw-rw-rw-   0        0        0      132 2023-04-12 23:20:16.000000 chessmaker-0.1.2/chessmaker/events/__init__.py
--rw-rw-rw-   0        0        0      385 2023-04-12 22:32:25.000000 chessmaker-0.1.2/chessmaker/events/event.py
--rw-rw-rw-   0        0        0      147 2023-04-12 22:32:25.000000 chessmaker-0.1.2/chessmaker/events/event_priority.py
--rw-rw-rw-   0        0        0     3203 2023-04-12 22:57:13.000000 chessmaker-0.1.2/chessmaker/events/event_publisher.py
-drwxrwxrwx   0        0        0        0 2023-04-13 00:44:40.152287 chessmaker-0.1.2/chessmaker.egg-info/
--rw-rw-rw-   0        0        0    43007 2023-04-13 00:44:40.000000 chessmaker-0.1.2/chessmaker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1698 2023-04-13 00:44:40.000000 chessmaker-0.1.2/chessmaker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 00:44:40.000000 chessmaker-0.1.2/chessmaker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-04-13 00:44:40.000000 chessmaker-0.1.2/chessmaker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-13 00:44:40.000000 chessmaker-0.1.2/chessmaker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1253 2023-04-13 00:40:55.000000 chessmaker-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 00:44:40.208286 chessmaker-0.1.2/setup.cfg
+-rw-r--r--   0        0        0      159 2023-04-12 23:23:56.894161 chessmaker-0.2/chessmaker/__init__.py
+-rw-r--r--   0        0        0      240 2023-04-13 13:53:22.478241 chessmaker-0.2/chessmaker/chess/__init__.py
+-rw-r--r--   0        0        0      688 2023-04-15 12:04:05.533044 chessmaker-0.2/chessmaker/chess/base/__init__.py
+-rw-r--r--   0        0        0     6833 2023-04-13 19:53:48.828413 chessmaker-0.2/chessmaker/chess/base/board.py
+-rw-r--r--   0        0        0     1095 2023-04-12 22:57:13.177726 chessmaker-0.2/chessmaker/chess/base/game.py
+-rw-r--r--   0        0        0      275 2023-04-13 19:53:48.822414 chessmaker-0.2/chessmaker/chess/base/move_option.py
+-rw-r--r--   0        0        0     3515 2023-04-15 12:04:05.524045 chessmaker-0.2/chessmaker/chess/base/piece.py
+-rw-r--r--   0        0        0      583 2023-04-12 22:32:25.286163 chessmaker-0.2/chessmaker/chess/base/player.py
+-rw-r--r--   0        0        0      241 2023-04-12 22:32:25.006418 chessmaker-0.2/chessmaker/chess/base/position.py
+-rw-r--r--   0        0        0      708 2023-04-12 22:57:13.193723 chessmaker-0.2/chessmaker/chess/base/rule.py
+-rw-r--r--   0        0        0     2187 2023-04-13 19:53:48.815413 chessmaker-0.2/chessmaker/chess/base/square.py
+-rw-r--r--   0        0        0     5299 2023-04-14 16:36:39.857090 chessmaker-0.2/chessmaker/chess/game_factory.py
+-rw-r--r--   0        0        0     2460 2023-04-15 15:01:42.502293 chessmaker-0.2/chessmaker/chess/piece_utils.py
+-rw-r--r--   0        0        0      319 2023-04-13 13:47:46.308045 chessmaker-0.2/chessmaker/chess/pieces/__init__.py
+-rw-r--r--   0        0        0      652 2023-04-13 13:46:31.618457 chessmaker-0.2/chessmaker/chess/pieces/bishop.py
+-rw-r--r--   0        0        0     6790 2023-04-14 01:55:25.122905 chessmaker-0.2/chessmaker/chess/pieces/king.py
+-rw-r--r--   0        0        0      880 2023-04-13 13:46:31.589457 chessmaker-0.2/chessmaker/chess/pieces/knight.py
+-rw-r--r--   0        0        0      191 2023-04-12 23:23:13.134441 chessmaker-0.2/chessmaker/chess/pieces/knook/__init__.py
+-rw-r--r--   0        0        0      968 2023-04-15 14:44:35.264730 chessmaker-0.2/chessmaker/chess/pieces/knook/knook.py
+-rw-r--r--   0        0        0       30 2023-04-15 15:13:15.595692 chessmaker-0.2/chessmaker/chess/pieces/knook/knookable.py
+-rw-r--r--   0        0        0     1177 2023-04-15 15:59:27.992040 chessmaker-0.2/chessmaker/chess/pieces/knook/knookable_knight.py
+-rw-r--r--   0        0        0     1209 2023-04-15 15:54:03.824540 chessmaker-0.2/chessmaker/chess/pieces/knook/knookable_rook.py
+-rw-r--r--   0        0        0     1607 2023-04-15 15:26:32.334630 chessmaker-0.2/chessmaker/chess/pieces/knook/merge_to_knook.py
+-rw-r--r--   0        0        0     5453 2023-04-15 12:04:05.529045 chessmaker-0.2/chessmaker/chess/pieces/pawn.py
+-rw-r--r--   0        0        0      785 2023-04-13 13:46:31.572457 chessmaker-0.2/chessmaker/chess/pieces/queen.py
+-rw-r--r--   0        0        0     1057 2023-04-13 13:46:31.652457 chessmaker-0.2/chessmaker/chess/pieces/rook.py
+-rw-r--r--   0        0        0      332 2023-04-14 13:45:12.352119 chessmaker-0.2/chessmaker/chess/results/__init__.py
+-rw-r--r--   0        0        0      478 2023-04-14 12:39:03.945677 chessmaker-0.2/chessmaker/chess/results/capture_all_pieces_to_win.py
+-rw-r--r--   0        0        0      584 2023-04-14 12:32:41.047541 chessmaker-0.2/chessmaker/chess/results/checkmate.py
+-rw-r--r--   0        0        0      770 2023-04-14 13:40:19.292622 chessmaker-0.2/chessmaker/chess/results/double_check_to_win.py
+-rw-r--r--   0        0        0     1134 2023-04-15 02:00:39.838687 chessmaker-0.2/chessmaker/chess/results/no_captures_or_pawn_moves.py
+-rw-r--r--   0        0        0      923 2023-04-14 11:49:56.085457 chessmaker-0.2/chessmaker/chess/results/repetition.py
+-rw-r--r--   0        0        0      326 2023-04-14 11:49:56.091457 chessmaker-0.2/chessmaker/chess/results/stalemate.py
+-rw-r--r--   0        0        0      510 2023-04-15 00:31:09.011728 chessmaker-0.2/chessmaker/chess/results/standard_result.py
+-rw-r--r--   0        0        0      345 2023-04-14 13:02:43.693404 chessmaker-0.2/chessmaker/chess/rules/__init__.py
+-rw-r--r--   0        0        0     3533 2023-04-13 13:46:31.611456 chessmaker-0.2/chessmaker/chess/rules/beta_decay.py
+-rw-r--r--   0        0        0     1875 2023-04-14 14:42:06.954160 chessmaker-0.2/chessmaker/chess/rules/forced_en_passant.py
+-rw-r--r--   0        0        0     3670 2023-04-15 12:04:05.521043 chessmaker-0.2/chessmaker/chess/rules/il_vaticano.py
+-rw-r--r--   0        0        0      979 2023-04-14 12:49:09.088586 chessmaker-0.2/chessmaker/chess/rules/king_cant_move_to_c2.py
+-rw-r--r--   0        0        0     2695 2023-04-12 22:57:13.120723 chessmaker-0.2/chessmaker/chess/rules/knight_boosting.py
+-rw-r--r--   0        0        0     2461 2023-04-14 13:33:54.257799 chessmaker-0.2/chessmaker/chess/rules/la_bastarda.py
+-rw-r--r--   0        0        0     1871 2023-04-15 12:04:05.540043 chessmaker-0.2/chessmaker/chess/rules/omnipotent_f6_pawn.py
+-rw-r--r--   0        0        0     1982 2023-04-14 01:23:32.960857 chessmaker-0.2/chessmaker/chess/rules/siberian_swipe.py
+-rw-r--r--   0        0        0       64 2023-04-14 17:14:53.444902 chessmaker-0.2/chessmaker/clients/__init__.py
+-rw-r--r--   0        0        0    15728 2023-04-15 15:58:59.834041 chessmaker-0.2/chessmaker/clients/pywebio_ui.py
+-rw-r--r--   0        0        0      278 2023-04-12 22:32:25.207165 chessmaker-0.2/chessmaker/cloneable.py
+-rw-r--r--   0        0        0      132 2023-04-12 23:20:16.008216 chessmaker-0.2/chessmaker/events/__init__.py
+-rw-r--r--   0        0        0      395 2023-04-13 19:53:48.832414 chessmaker-0.2/chessmaker/events/event.py
+-rw-r--r--   0        0        0      146 2023-04-14 13:26:17.602659 chessmaker-0.2/chessmaker/events/event_priority.py
+-rw-r--r--   0        0        0     3203 2023-04-12 22:57:13.182724 chessmaker-0.2/chessmaker/events/event_publisher.py
+-rw-r--r--   0        0        0    35184 2023-04-05 10:50:17.213863 chessmaker-0.2/LICENSE
+-rw-r--r--   0        0        0     1096 2023-04-15 16:07:51.887204 chessmaker-0.2/pyproject.toml
+-rw-r--r--   0        0        0     1862 2023-04-14 14:15:04.351108 chessmaker-0.2/README.md
+-rw-r--r--   0        0        0     2958 1970-01-01 00:00:00.000000 chessmaker-0.2/PKG-INFO
```

### Comparing `chessmaker-0.1.2/LICENSE` & `chessmaker-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.2/README.md` & `chessmaker-0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # ChessMaker
 
 An easily extendible chess implementation designed
 to support any custom rule or feature.
 
+<span style="font-size:x-large;"><b>
+Play: [https://chessmaker.azurewebsites.net](https://chessmaker.azurewebsites.net)
+</b></span>
+
 **Documentation**: [https://wolfdwyc.github.io/ChessMaker](https://wolfdwyc.github.io/ChessMaker)
 
-**Source Code**: [https://github.com/WolfDWyc/ChessMaker](https://wolfdwyc.github.io/ChessMaker)
+**Source Code**: [https://github.com/WolfDWyc/ChessMaker](https://github.com/WolfDWyc/ChessMaker)
 
 ---
 
 ## What is ChessMaker?
 
 ChessMaker is a Python (3.11+) chess implementation that can be extended to support any custom rule or feature.
 It allows you to build almost any variant you can think of easily and quickly.
@@ -23,21 +27,26 @@
 * Chess960
 * Knooks
 * Forced En Passant
 * Knight Boosting
 * Siberian Swipe
 * Il Vaticano
 * Beta Decay
+* La Bastarda
 * Omnipotent F6 Pawn
+* King Cant Move to C2
+* Vertical Castling
+* Double Check to Win
+* Capture All Pieces to Win
+
 
 ## What ChessMaker isn't
 
 * A complete chess server - It doesn't support users, matchmaking, ratings, cheating detection, etc. 
 The frontend is very simple and not the focus of the project.
 * A chess engine. The design choices are not optimized for speed, and it doesn't provide any analysis or AI.
 * A compliant or standard chess implementation. It doesn't support UCI or existing chess GUIs,
 because it allows rules that wouldn't be possible with those.
 
-!!! note
-    While ChessMaker isn't a chess server, one could be built on top of it, and development of alternative clients to it is welcomed and encouraged.
+Note: While ChessMaker isn't a chess server, one could be built on top of it, and development of alternative clients to it is welcomed and encouraged.
```

### Comparing `chessmaker-0.1.2/chessmaker/chess/base/__init__.py` & `chessmaker-0.2/chessmaker/chess/base/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .board import Board, BeforeTurnChangeEvent, AfterTurnChangeEvent, AfterNewPieceEvent, BeforeAddSquareEvent, \
                     BeforeRemoveSquareEvent, AfterAddSquareEvent, AfterRemoveSquareEvent
 from .game import Game, AfterGameEndEvent
 from .piece import Piece, PieceEventTypes, AfterMoveEvent, BeforeMoveEvent, AfterGetMoveOptionsEvent, \
-                    BeforeGetMoveOptionsEvent, AfterCaptureEvent, BeforeCaptureEvent
+                    BeforeGetMoveOptionsEvent, AfterCapturedEvent, BeforeCapturedEvent
 from .player import Player
 from .position import Position
 from .rule import Rule, as_rule
 from .square import Square, BeforeAddPieceEvent, AfterRemovePieceEvent, AfterAddPieceEvent, BeforeRemovePieceEvent
 from .move_option import MoveOption
```

### Comparing `chessmaker-0.1.2/chessmaker/chess/base/board.py` & `chessmaker-0.2/chessmaker/chess/base/board.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         # Subscribe to the events of each square
         for row in self._squares:
             for square in row:
                 if square is not None:
                     # TODO: Subscribe to new squares
                     self.propagate_all(square)
-                    square.board = self
+                    square._board = self
                     if square.piece is not None:
                         self._on_after_add_piece(AfterAddPieceEvent(square, square.piece))
 
         self.subscribe(AfterAddPieceEvent, self._on_after_add_piece)
         self.subscribe(AfterMoveEvent, self._on_after_move)
 
         for rule in self.rules:
@@ -88,14 +88,15 @@
 
 
     # TODO: Implement this in a way that detects actual new pieces and not moved pieces
     def _on_after_add_piece(self, event: AfterAddPieceEvent):
         piece: Piece = event.piece
         if piece._board is None:
             piece._board = self
+            piece.on_join_board()
             self.publish(AfterNewPieceEvent(piece))
             self.propagate_all(piece)
 
     def _on_after_move(self, _: AfterMoveEvent):
         next_player = next(self.turn_iterator)
         before_turn_change_event = BeforeTurnChangeEvent(self, next_player)
         self.publish(before_turn_change_event)
```

### Comparing `chessmaker-0.1.2/chessmaker/chess/base/game.py` & `chessmaker-0.2/chessmaker/chess/base/game.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.2/chessmaker/chess/base/piece.py` & `chessmaker-0.2/chessmaker/chess/base/piece.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,43 +6,49 @@
 from chessmaker.chess.base.player import Player
 from chessmaker.cloneable import Cloneable
 from chessmaker.events import EventPublisher, Event, CancellableEvent
 
 if TYPE_CHECKING:
     from chessmaker.chess.base.board import Board
 
+
 @dataclass(frozen=True)
 class AfterGetMoveOptionsEvent(Event):
     piece: "Piece"
     move_options: Iterable[MoveOption]
 
+
 class BeforeGetMoveOptionsEvent(AfterGetMoveOptionsEvent):
     def set_move_options(self, move_options: Iterable[MoveOption]):
         self._set("move_options", move_options)
 
+
 @dataclass(frozen=True)
 class AfterMoveEvent(Event):
     piece: "Piece"
     move_option: MoveOption
 
+
 class BeforeMoveEvent(AfterMoveEvent, CancellableEvent):
     def set_move_option(self, move_option: MoveOption):
         self._set("move_option", move_option)
 
+
 @dataclass(frozen=True)
-class AfterCaptureEvent(Event):
-    capturing_piece: "Piece"
+class AfterCapturedEvent(Event):
     captured_piece: "Piece"
 
-class BeforeCaptureEvent(AfterCaptureEvent):
+
+class BeforeCapturedEvent(AfterCapturedEvent):
     pass
 
 
-PieceEventTypes = AfterGetMoveOptionsEvent | BeforeGetMoveOptionsEvent | AfterMoveEvent | BeforeMoveEvent |\
-                  AfterCaptureEvent | BeforeCaptureEvent
+PieceEventTypes = AfterGetMoveOptionsEvent | BeforeGetMoveOptionsEvent | AfterMoveEvent | BeforeMoveEvent | \
+                  AfterCapturedEvent | BeforeCapturedEvent
+
 
 class Piece(EventPublisher[PieceEventTypes], Cloneable):
     def __init__(self, player: Player):
         super().__init__()
         self._player = player
         self._board: Board = None
 
@@ -70,22 +76,25 @@
         source = self.board[self.position]
         source.piece = None
 
         destination = self.board[move_option.position]
 
         for capture_position in move_option.captures:
             capture_piece = self.board[capture_position].piece
-            self.publish(BeforeCaptureEvent(self, capture_piece))
+            capture_piece.publish(BeforeCapturedEvent(capture_piece))
             self.board[capture_position].piece = None
-            self.publish(AfterCaptureEvent(self, capture_piece))
+            capture_piece.publish(AfterCapturedEvent(capture_piece))
 
         destination.piece = self
 
         self.publish(AfterMoveEvent(self, move_option))
 
+    def on_join_board(self):
+        pass
+
     @property
     def player(self):
         return self._player
 
     @property
     def position(self):
         return self.board._get_piece_position(self)
@@ -95,15 +104,15 @@
         if self._board is None:
             raise Exception("Piece is not on the board yet")
         return self._board
 
     @classmethod
     @property
     @abstractmethod
-    def name(self):
+    def name(cls):
         raise NotImplementedError
 
     @abstractmethod
     def _get_move_options(self) -> Iterable[MoveOption]:
         raise NotImplementedError
 
     @abstractmethod
```

### Comparing `chessmaker-0.1.2/chessmaker/chess/base/player.py` & `chessmaker-0.2/chessmaker/chess/base/player.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.2/chessmaker/chess/base/rule.py` & `chessmaker-0.2/chessmaker/chess/base/rule.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.2/chessmaker/chess/base/square.py` & `chessmaker-0.2/chessmaker/chess/base/square.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,24 +27,30 @@
     pass
 
 
 class Square(EventPublisher[BeforeAddPieceEvent | AfterAddPieceEvent | BeforeRemovePieceEvent | AfterRemovePieceEvent], Cloneable):
     def __init__(self, piece: Piece | None = None):
         super().__init__()
         self._piece = piece
-        self.board: Board = None
+        self._board: Board = None
 
     @property
     def piece(self) -> Piece:
         return self._piece
 
     @property
     def position(self):
         return self.board._get_square_position(self)
 
+    @property
+    def board(self):
+        if self._board is None:
+            raise Exception("Square is not on the board yet")
+        return self._board
+
     @piece.setter
     def piece(self, piece: Piece):
         old_piece = self._piece
 
         if piece is old_piece:
             warnings.warn("Setting the same piece on the square has no effect", RuntimeWarning)
             return
```

### Comparing `chessmaker-0.1.2/chessmaker/chess/game_factory.py` & `chessmaker-0.2/chessmaker/chess/game_factory.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,94 @@
 import random
 from itertools import cycle
 from typing import Callable
 
+from chessmaker.chess import results
 from chessmaker.chess.base.board import Board
 from chessmaker.chess.base.game import Game
 from chessmaker.chess.base.piece import Piece
 from chessmaker.chess.base.player import Player
 from chessmaker.chess.base.square import Square
 from chessmaker.chess.pieces.bishop import Bishop
 from chessmaker.chess.pieces.king import King
 from chessmaker.chess.pieces.knight import Knight
 from chessmaker.chess.pieces.knook.knookable_knight import KnookableKnight
 from chessmaker.chess.pieces.knook.knookable_rook import KnookableRook
 from chessmaker.chess.pieces.pawn import Pawn
 from chessmaker.chess.pieces.queen import Queen
 from chessmaker.chess.pieces.rook import Rook
-from chessmaker.chess.results.simple_result import GetSimpleResult
-from chessmaker.chess.rules import ForcedEnPassant, KnightBoosting, OmnipotentF6Pawn, SiberianSwipe, IlVaticano, BetaDecay
+from chessmaker.chess.results import stalemate, Repetition, NoCapturesOrPawnMoves, checkmate
+from chessmaker.chess.rules import ForcedEnPassant, KnightBoosting, OmnipotentF6Pawn, SiberianSwipe, IlVaticano, \
+    BetaDecay, KingCantMoveToC2, LaBastarda
+
 
 class A:
     pass
 
+
 def create_game(
         chess960: bool = False,
         knooks: bool = False,
         forced_en_passant: bool = False,
         knight_boosting: bool = False,
         omnipotent_f6_pawn: bool = False,
         siberian_swipe: bool = False,
         il_vaticano: bool = False,
         beta_decay: bool = False,
+        la_bastarda: bool = False,
+        king_cant_move_to_c2: bool = False,
+        vertical_castling: bool = False,
+        double_check_to_win: bool = False,
+        capture_all_pieces_to_win: bool = False,
 ):
     _knight = Knight
     _rook = Rook
+    castling_directions = ((1, 0), (-1, 0))
+    if vertical_castling:
+        castling_directions = tuple(list(castling_directions) + [(0, 1), (0, -1)])
+    _king = lambda player: King(player, attackable=capture_all_pieces_to_win, castling_directions=castling_directions)
     if knooks:
         _knight = KnookableKnight
         _rook = KnookableRook
 
+    white = Player("white")
+    black = Player("black")
+    turn_iterator = cycle([white, black])
+
     def _empty_line(length: int) -> list[Square]:
         return [Square() for _ in range(length)]
 
     def _up_pawn(player: Player):
-        return Square(Pawn(player, Pawn.Direction.UP, promotions=[Bishop, _rook, Queen, _knight]))
+        return Pawn(player, Pawn.Direction.UP, promotions=[Bishop, _rook, Queen, _knight])
 
     def _down_pawn(player: Player):
-        return Square(Pawn(player, Pawn.Direction.DOWN, promotions=[Bishop, _rook, Queen, _knight]))
+        return Pawn(player, Pawn.Direction.DOWN, promotions=[Bishop, _rook, Queen, _knight])
 
-    white = Player("white")
-    black = Player("black")
-    turn_iterator = cycle([white, black])
+    def _pawn(player: Player):
+        if player == white:
+            return _up_pawn(player)
+        elif player == black:
+            return _down_pawn(player)
 
     def _piece_row() -> list[Callable[[Player], Piece]]:
 
-        pieces = [_rook, _knight, Bishop, Queen, King, Bishop, _knight, _rook]
+        pieces = [_rook, _knight, Bishop, Queen, _king, Bishop, _knight, _rook]
 
         if chess960:
             row = [None] * len(pieces)
             matched = False
             while not matched:
                 matched = True
                 row = random.sample(pieces, len(pieces))
                 first_bishop, second_bishop = [i for i, piece in enumerate(row) if piece == Bishop]
                 if first_bishop % 2 == second_bishop % 2:
                     matched = False
                     continue
 
-                king = row.index(King)
+                king = row.index(_king)
                 first_rook, second_rook = [i for i, piece in enumerate(row) if piece == _rook]
 
                 if king < first_rook < second_rook or king > first_rook > second_rook:
                     matched = False
                     continue
         else:
             row = pieces
@@ -80,38 +99,50 @@
 
     rules = []
     for enabled, rule in [
         (forced_en_passant, ForcedEnPassant()),
         (knight_boosting, KnightBoosting()),
         (siberian_swipe, SiberianSwipe()),
         (il_vaticano, IlVaticano()),
-        (omnipotent_f6_pawn, OmnipotentF6Pawn({white: lambda: _up_pawn(white).piece, black: lambda: _down_pawn(black).piece})),
-        (beta_decay, BetaDecay([_rook, Bishop,
-            lambda player: _up_pawn(player).piece if player == white else _down_pawn(player).piece,
-        ])),
+        (king_cant_move_to_c2, KingCantMoveToC2()),
+        (omnipotent_f6_pawn, OmnipotentF6Pawn(pawn=_pawn)),
+        (la_bastarda, LaBastarda(pawn=_pawn)),
+        (beta_decay, BetaDecay([_rook, Bishop, _pawn])),
     ]:
         if enabled:
             rules.append(rule)
 
-    board = Board(
-        squares=[
-            [Square(piece_row[i](black)) for i in range(8)],
-            [_down_pawn(black) for _ in range(8)],
-            _empty_line(8),
-            _empty_line(8),
-            _empty_line(8),
-            _empty_line(8),
-            [_up_pawn(white) for _ in range(8)],
-            [Square(piece_row[i](white)) for i in range(8)],
-        ],
-        players=[white, black],
-        turn_iterator=turn_iterator,
-        rules=rules,
-    )
+    result_functions = [stalemate, Repetition(3), NoCapturesOrPawnMoves(50)]
+    if capture_all_pieces_to_win:
+        result_functions.insert(0, results.capture_all_pieces_to_win)
+    else:
+        result_functions.insert(0, checkmate)
+
+    if double_check_to_win:
+        result_functions.insert(0, results.double_check_to_win)
+
+    def get_result(board: Board) -> str:
+        for result_function in result_functions:
+            result = result_function(board)
+            if result:
+                return result
 
     game = Game(
-        board=board,
-        get_result=GetSimpleResult(),
+        board=Board(
+            squares=[
+                [Square(piece_row[i](black)) for i in range(8)],
+                [Square(_pawn(black)) for _ in range(8)],
+                _empty_line(8),
+                _empty_line(8),
+                _empty_line(8),
+                _empty_line(8),
+                [Square(_pawn(white)) for _ in range(8)],
+                [Square(piece_row[i](white)) for i in range(8)],
+            ],
+            players=[white, black],
+            turn_iterator=turn_iterator,
+            rules=rules,
+        ),
+        get_result=get_result,
     )
 
     return game
-
```

### Comparing `chessmaker-0.1.2/chessmaker/chess/pieces/bishop.py` & `chessmaker-0.2/chessmaker/chess/pieces/bishop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable
 
 from chessmaker.chess.base.move_option import MoveOption
 from chessmaker.chess.base.piece import Piece
-from chessmaker.chess.pieces.piece_utils import get_diagonals_until_blocked, filter_uncapturable_positions, \
+from chessmaker.chess.piece_utils import get_diagonals_until_blocked, filter_uncapturable_positions, \
     positions_to_move_options
 
 
 class Bishop(Piece):
     @classmethod
     @property
     def name(cls):
```

### Comparing `chessmaker-0.1.2/chessmaker/chess/pieces/king.py` & `chessmaker-0.2/chessmaker/chess/pieces/king.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from chessmaker.chess.base.board import AfterNewPieceEvent
 from chessmaker.chess.base.move_option import MoveOption
 from chessmaker.chess.base.piece import Piece, PieceEventTypes, BeforeMoveEvent, BeforeGetMoveOptionsEvent
 from chessmaker.chess.base.player import Player
 from chessmaker.chess.base.position import Position
 from chessmaker.chess.base.square import Square
-from chessmaker.chess.pieces.piece_utils import filter_uncapturable_positions, is_in_board, iterate_until_blocked, \
+from chessmaker.chess.piece_utils import filter_uncapturable_positions, is_in_board, iterate_until_blocked, \
     positions_to_move_options
 from chessmaker.chess.pieces.rook import Rook
 from chessmaker.events import Event, EventPublisher, EventPriority
 
 
 @dataclass(frozen=True)
 class AfterCastleEvent(Event):
@@ -27,30 +27,36 @@
     def set_king_destination(self, king_destination: Square):
         self._set("king_destination", king_destination)
 
     def set_rook_destination(self, rook_destination: Square):
         self._set("rook_destination", rook_destination)
 
 class King(Piece, EventPublisher[PieceEventTypes | AfterCastleEvent | BeforeCastleEvent]):
-    def __init__(self, player: Player, moved: bool = False, attackable: bool = False):
+    def __init__(
+            self,
+            player: Player,
+            moved: bool = False,
+            attackable: bool = False,
+            castling_directions: tuple[tuple[int, int], ...] = ((1, 0), (-1, 0))
+    ):
         super().__init__(player)
         self._moved = moved
         self._attackable = attackable
-        self.subscribe(AfterNewPieceEvent, self.on_after_added_to_board)
+        self._castling_directions = castling_directions
         self.subscribe(BeforeMoveEvent, self._on_before_move, EventPriority.VERY_HIGH)
 
 
+
     @classmethod
     @property
     def name(cls):
         return "King"
 
-    def on_after_added_to_board(self, _: AfterNewPieceEvent):
+    def on_join_board(self):
         if not self._attackable:
-            # TODO: What if the piece switches player?
             for piece in self.board.get_pieces():
                 if piece.player == self.player:
                     piece.subscribe(BeforeGetMoveOptionsEvent, self._on_before_get_move_options)
             self.board.subscribe(AfterNewPieceEvent, self._on_after_new_piece)
 
     def _on_after_new_piece(self, event: AfterNewPieceEvent):
         if event.piece.player == self.player:
@@ -112,15 +118,15 @@
         ]
 
         positions = filter(partial(is_in_board, self.board), positions)
         positions = list(filter_uncapturable_positions(self, positions))
 
         move_options = list(positions_to_move_options(self.board, positions))
 
-        for direction in [(1, 0), (-1, 0)]:
+        for direction in self._castling_directions:
             line = list(iterate_until_blocked(self, direction))
             if len(line) > 2:
                 last_piece = self.board[line[-1]].piece
                 if (last_piece is not None and
                         last_piece.player == self.player and
                         isinstance(last_piece, Rook) and
                         not last_piece.moved and
@@ -130,26 +136,30 @@
         return move_options
     def _on_before_move(self, event: BeforeMoveEvent):
         if "castle" in event.move_option.extra:
             move_option = event.move_option
             destination = self.board[move_option.position]
 
             rook_source = self.board[Position(*move_option.extra["castle"])]
-            rook_destination = self.board[Position((self.position.x + move_option.position.x) // 2, self.position.y)]
+            rook_destination = self.board[Position(
+                (self.position.x + move_option.position.x) // 2,
+                (self.position.y + move_option.position.y) // 2,
+            )]
             rook: Rook = rook_source.piece
 
             before_castle_event = BeforeCastleEvent(self, rook, destination, rook_destination)
             self.publish(before_castle_event)
 
             before_castle_event.king_destination.piece = self
-            rook_source.piece = None
+            self.board[self.position].piece = None
             self._moved = True
 
             before_castle_event.rook_destination.piece = rook
+            rook_source.piece = None
             rook.moved = True
 
             self.publish(AfterCastleEvent(self, rook))
         self._moved = True
 
     def clone(self):
         # TODO: What if someone else clones the king?
-        return King(self.player, self._moved, attackable=True)
+        return King(self.player, self._moved, attackable=True, castling_directions=self._castling_directions)
```

### Comparing `chessmaker-0.1.2/chessmaker/chess/pieces/knight.py` & `chessmaker-0.2/chessmaker/chess/pieces/knight.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from functools import partial
 from typing import Iterable
 
 from chessmaker.chess.base.move_option import MoveOption
 from chessmaker.chess.base.piece import Piece
-from chessmaker.chess.pieces.piece_utils import filter_uncapturable_positions, is_in_board, positions_to_move_options
+from chessmaker.chess.piece_utils import filter_uncapturable_positions, is_in_board, positions_to_move_options
 
 MOVE_OFFSETS = [(1, 2), (2, 1), (2, -1), (1, -2), (-1, -2), (-2, -1), (-2, 1), (-1, 2)]
 
 
 class Knight(Piece):
     @classmethod
     @property
```

### Comparing `chessmaker-0.1.2/chessmaker/chess/pieces/knook/knook.py` & `chessmaker-0.2/chessmaker/chess/pieces/knook/knook.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from functools import partial
 from typing import Iterable
 
 from chessmaker.chess.base.move_option import MoveOption
 from chessmaker.chess.base.piece import Piece
 from chessmaker.chess.pieces import knight
-from chessmaker.chess.pieces.piece_utils import filter_uncapturable_positions, is_in_board, \
+from chessmaker.chess.piece_utils import filter_uncapturable_positions, is_in_board, \
     get_straight_until_blocked, positions_to_move_options
 
 
 class Knook(Piece):
     @classmethod
     @property
     def name(cls):
```

### Comparing `chessmaker-0.1.2/chessmaker/chess/pieces/knook/knookable_knight.py` & `chessmaker-0.2/chessmaker/chess/pieces/knook/knookable_knight.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from functools import partial
+from itertools import chain
 
-from chessmaker.chess.base.piece import AfterMoveEvent
+from chessmaker.chess.base.piece import AfterMoveEvent, PieceEventTypes
 from chessmaker.chess.pieces import knight
 from chessmaker.chess.pieces.knight import Knight
 from chessmaker.chess.pieces.knook import merge_to_knook
 from chessmaker.chess.pieces.knook.knookable import Knookable
-from chessmaker.chess.pieces.piece_utils import is_in_board
-from chessmaker.events import EventPriority
+from chessmaker.chess.piece_utils import is_in_board
+from chessmaker.events import EventPriority, EventPublisher
 
 
-class KnookableKnight(Knight, Knookable):
+class KnookableKnight(Knight, EventPublisher[PieceEventTypes | merge_to_knook.MergeToKnookEventTypes], Knookable):
     def __init__(self, player):
         super().__init__(player)
         self.subscribe(AfterMoveEvent, merge_to_knook.on_after_move, EventPriority.VERY_HIGH)
 
     def _get_move_options(self):
         positions = [self.position.offset(*offset) for offset in knight.MOVE_OFFSETS]
         positions = list(filter(partial(is_in_board, self.board), positions))
         merge_move_options = merge_to_knook.get_merge_move_options(self, positions)
 
-        return list(super()._get_move_options()) + list(merge_move_options)
+        return chain(super()._get_move_options(), merge_move_options)
 
     def clone(self):
         return KnookableKnight(self.player)
```

### Comparing `chessmaker-0.1.2/chessmaker/chess/pieces/knook/knookable_rook.py` & `chessmaker-0.2/chessmaker/chess/pieces/knook/knookable_rook.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
+from itertools import chain
 from typing import Iterable
 
 from chessmaker.chess.base.move_option import MoveOption
-from chessmaker.chess.base.piece import AfterMoveEvent
+from chessmaker.chess.base.piece import AfterMoveEvent, PieceEventTypes
 from chessmaker.chess.base.player import Player
 from chessmaker.chess.pieces.knook import merge_to_knook
 from chessmaker.chess.pieces.knook.knookable import Knookable
-from chessmaker.chess.pieces.piece_utils import filter_uncapturable_positions, get_straight_until_blocked
+from chessmaker.chess.piece_utils import get_straight_until_blocked
 from chessmaker.chess.pieces.rook import Rook
-from chessmaker.events import EventPriority
+from chessmaker.events import EventPriority, EventPublisher
 
 
-class KnookableRook(Rook, Knookable):
+class KnookableRook(Rook, EventPublisher[PieceEventTypes | merge_to_knook.MergeToKnookEventTypes], Knookable):
     def __init__(self, player: Player, moved: bool = False):
         super().__init__(player, moved)
         self.subscribe(AfterMoveEvent, merge_to_knook.on_after_move, EventPriority.VERY_HIGH)
 
     def _get_move_options(self) -> Iterable[MoveOption]:
-        positions = list(filter_uncapturable_positions(self, get_straight_until_blocked(self)))
+        positions = list(get_straight_until_blocked(self))
         merge_move_options = merge_to_knook.get_merge_move_options(self, positions)
 
-        return list(super()._get_move_options()) + list(merge_move_options)
+        return chain(super()._get_move_options(), merge_move_options)
 
     def clone(self):
         return KnookableRook(self.player, self.moved)
```

### Comparing `chessmaker-0.1.2/chessmaker/chess/pieces/knook/merge_to_knook.py` & `chessmaker-0.2/chessmaker/chess/pieces/knook/merge_to_knook.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,31 +10,33 @@
 
 
 @dataclass(frozen=True)
 class AfterMergeToKnookEvent(Event):
     piece: Piece
     knook: Knook
 
+
 class BeforeMergeToKnookEvent(AfterMergeToKnookEvent):
     def set_knook(self, knook: Knook):
         self._set("knook", knook)
 
 
+MergeToKnookEventTypes = AfterMergeToKnookEvent | BeforeMergeToKnookEvent
+
+
 def get_merge_move_options(piece: Piece, positions: Iterable[Position]) -> Iterable[MoveOption]:
     for position in positions:
         position_piece = piece.board[position].piece
 
         if position_piece is not None and position_piece.player == piece.player:
             if isinstance(position_piece, Knookable) and not isinstance(position_piece, type(piece)):
                 yield MoveOption(position, extra=dict(knook=True))
 
+
 def on_after_move(event: AfterMoveEvent):
-    if "knook" in event.move_option.extra:
+    if event.move_option.extra.get("knook"):
         piece = event.piece
         before_merge_to_knook_event = BeforeMergeToKnookEvent(piece, Knook(event.piece.player))
         event.piece.publish(before_merge_to_knook_event)
         knook = before_merge_to_knook_event.knook
         piece.board[event.move_option.position].piece = knook
         piece.publish(AfterMergeToKnookEvent(piece, knook))
-
-
-
```

### Comparing `chessmaker-0.1.2/chessmaker/chess/pieces/pawn.py` & `chessmaker-0.2/chessmaker/chess/pieces/pawn.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from dataclasses import dataclass
 from enum import Enum
 from typing import Iterable, Type
 
 from chessmaker.chess.base.board import AfterNewPieceEvent
 from chessmaker.chess.base.game import AfterTurnChangeEvent
 from chessmaker.chess.base.move_option import MoveOption
-from chessmaker.chess.base.piece import Piece, BeforeMoveEvent, AfterMoveEvent, BeforeCaptureEvent, AfterCaptureEvent
+from chessmaker.chess.base.piece import Piece, BeforeMoveEvent, AfterMoveEvent, BeforeCapturedEvent, AfterCapturedEvent
 from chessmaker.chess.base.player import Player
 from chessmaker.chess.base.position import Position
-from chessmaker.chess.pieces.piece_utils import iterate_until_blocked, is_in_board
+from chessmaker.chess.piece_utils import iterate_until_blocked, is_in_board
 from chessmaker.events import EventPriority, Event
 
 @dataclass(frozen=True)
 class AfterPromotionEvent(Event):
     pawn: "Pawn"
     promotion: Piece
 
@@ -44,19 +44,18 @@
         if promotions is None:
             promotions = []
         self.promotions = {promotion.name: promotion for promotion in promotions}
         self._direction = direction
         self._moved_turns_ago = moved_turns_ago
         self._last_position = last_position
 
-        self.subscribe(AfterNewPieceEvent, self.on_after_added_to_board)
         self.subscribe(BeforeMoveEvent, self._on_before_move, EventPriority.VERY_HIGH)
         self.subscribe(AfterMoveEvent, self._on_after_move, EventPriority.VERY_HIGH)
 
-    def on_after_added_to_board(self):
+    def on_join_board(self):
         self.board.subscribe(AfterTurnChangeEvent, self._on_turn_change)
 
     def _on_turn_change(self, _: AfterTurnChangeEvent):
         if self._moved_turns_ago != -1:
             self._moved_turns_ago += 1
 
     def _get_move_options(self) -> Iterable[MoveOption]:
```

### Comparing `chessmaker-0.1.2/chessmaker/chess/pieces/piece_utils.py` & `chessmaker-0.2/chessmaker/chess/piece_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,13 +62,14 @@
         position_piece = piece.board[position].piece
         if position_piece is not None and position_piece.player == piece.player:
             continue
         filtered_positions.append(position)
 
     return filtered_positions
 
+
 def positions_to_move_options(board: Board, positions: Iterable[Position]) -> Iterable[MoveOption]:
     for position in positions:
         if board[position].piece is None:
             yield MoveOption(position)
         else:
             yield MoveOption(position, captures={position})
```

### Comparing `chessmaker-0.1.2/chessmaker/chess/pieces/queen.py` & `chessmaker-0.2/chessmaker/chess/pieces/queen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from itertools import chain
 from typing import Iterable
 
 from chessmaker.chess.base.move_option import MoveOption
 from chessmaker.chess.base.piece import Piece
-from chessmaker.chess.pieces.piece_utils import filter_uncapturable_positions, get_straight_until_blocked \
+from chessmaker.chess.piece_utils import filter_uncapturable_positions, get_straight_until_blocked \
     , get_diagonals_until_blocked, positions_to_move_options
 
 
 class Queen(Piece):
     @classmethod
     @property
     def name(cls):
```

### Comparing `chessmaker-0.1.2/chessmaker/chess/pieces/rook.py` & `chessmaker-0.2/chessmaker/chess/pieces/rook.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Iterable
 
 from chessmaker.chess.base.move_option import MoveOption
 from chessmaker.chess.base.piece import Piece, AfterMoveEvent
 from chessmaker.chess.base.player import Player
-from chessmaker.chess.pieces.piece_utils import filter_uncapturable_positions, get_straight_until_blocked, \
+from chessmaker.chess.piece_utils import filter_uncapturable_positions, get_straight_until_blocked, \
     positions_to_move_options
 from chessmaker.events import EventPriority
 
 
 class Rook(Piece):
     def __init__(self, player: Player, moved: bool = False):
         super().__init__(player)
```

### Comparing `chessmaker-0.1.2/chessmaker/chess/rules/beta_decay.py` & `chessmaker-0.2/chessmaker/chess/rules/beta_decay.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Callable
 
 from chessmaker.chess.base.board import AfterNewPieceEvent, Board
 from chessmaker.chess.base.move_option import MoveOption
 from chessmaker.chess.base.piece import Piece, BeforeGetMoveOptionsEvent, BeforeMoveEvent, AfterMoveEvent
 from chessmaker.chess.base.player import Player
 from chessmaker.chess.base.rule import Rule
-from chessmaker.chess.pieces.piece_utils import iterate_until_blocked
+from chessmaker.chess.piece_utils import iterate_until_blocked
 from chessmaker.chess.pieces.queen import Queen
 from chessmaker.events import EventPriority
 
 sign = lambda x: x and (1, -1)[x < 0]
 
 class BetaDecay(Rule):
     def __init__(self, decay_to_pieces: list[Callable[[Player], Piece]]):
```

### Comparing `chessmaker-0.1.2/chessmaker/chess/rules/forced_en_passant.py` & `chessmaker-0.2/chessmaker/chess/rules/forced_en_passant.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,27 +20,25 @@
         board.subscribe(AfterTurnChangeEvent, self.on_turn_change)
 
     def on_turn_change(self, event: AfterTurnChangeEvent):
         for player in event.board.players:
             self.can_en_passant[player] = False
             for piece in event.board.get_player_pieces(player):
                 if isinstance(piece, Pawn):
-                    move_options = piece._get_move_options()
+                    move_options = piece.get_move_options()
                     if any(move_option.extra.get("en_passant") for move_option in move_options):
                         self.can_en_passant[player] = True
                         break
 
     def on_before_get_move_options(self, event: BeforeGetMoveOptionsEvent):
-        event_move_options = event.move_options
-        if not self.can_en_passant[event.piece.player]:
-            return
-        move_options = []
-        for move_option in event_move_options:
-            if move_option.extra.get("en_passant"):
-                move_options.append(move_option)
-        event.set_move_options(move_options)
+        if self.can_en_passant[event.piece.player]:
+            move_options = []
+            for move_option in event.move_options:
+                if move_option.extra.get("en_passant"):
+                    move_options.append(move_option)
+            event.set_move_options(move_options)
 
     def clone(self):
         return ForcedEnPassant(can_en_passant=self.can_en_passant.copy())
```

### Comparing `chessmaker-0.1.2/chessmaker/chess/rules/il_vaticano.py` & `chessmaker-0.2/chessmaker/chess/rules/il_vaticano.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from itertools import chain
 
 from chessmaker.chess.base.board import Board, AfterNewPieceEvent
 from chessmaker.chess.base.move_option import MoveOption
-from chessmaker.chess.base.piece import Piece, BeforeGetMoveOptionsEvent, BeforeMoveEvent
+from chessmaker.chess.base.piece import Piece, BeforeGetMoveOptionsEvent, BeforeMoveEvent, AfterMoveEvent, \
+    BeforeCapturedEvent, AfterCapturedEvent
 from chessmaker.chess.base.rule import Rule
 from chessmaker.chess.pieces.bishop import Bishop
-from chessmaker.chess.pieces.piece_utils import is_in_board
+from chessmaker.chess.piece_utils import is_in_board
 from chessmaker.events import EventPriority
 
 SIZE = 3
 sign = lambda x: x and (1, -1)[x < 0]
 
 class IlVaticano(Rule):
     def on_join_board(self, board: Board):
@@ -67,19 +68,22 @@
         if "il_vaticano" in event.move_option.extra:
             other_position = event.move_option.position
 
             # Iterate all positions between the two positions
             direction = (sign(other_position.x - position.x), sign(other_position.y - position.y))
             enemy_position = position.offset(*direction)
             while enemy_position != other_position:
+                enemy_piece = board[enemy_position].piece
+                enemy_piece.publish(BeforeCapturedEvent(enemy_piece))
                 board[enemy_position].piece = None
+                enemy_piece.publish(AfterCapturedEvent(enemy_piece))
                 enemy_position = enemy_position.offset(*direction)
 
             board[position].piece = board[other_position].piece
             board[other_position].piece = piece
-            piece.move(MoveOption(other_position))
+            piece.publish(AfterMoveEvent(piece, MoveOption(other_position)))
             event.set_cancelled(True)
     def clone(self):
         return IlVaticano()
```

### Comparing `chessmaker-0.1.2/chessmaker/chess/rules/knight_boosting.py` & `chessmaker-0.2/chessmaker/chess/rules/knight_boosting.py`

 * *Files identical despite different names*

### Comparing `chessmaker-0.1.2/chessmaker/chess/rules/omnipotent_f6_pawn.py` & `chessmaker-0.2/chessmaker/chess/rules/siberian_swipe.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,52 @@
-from typing import Callable
+from itertools import chain
 
-from chessmaker.chess.base.board import Board
+from chessmaker.chess.base.board import AfterNewPieceEvent, Board
 from chessmaker.chess.base.move_option import MoveOption
-from chessmaker.chess.base.piece import Piece, BeforeGetMoveOptionsEvent, BeforeMoveEvent
-from chessmaker.chess.base.player import Player
-from chessmaker.chess.base.position import Position
+from chessmaker.chess.base.piece import Piece, BeforeGetMoveOptionsEvent
 from chessmaker.chess.base.rule import Rule
+from chessmaker.chess.piece_utils import is_in_board
+from chessmaker.chess.pieces.rook import Rook
 from chessmaker.events import EventPriority
 
-F6 = Position(5, 2)
-
-class OmnipotentF6Pawn(Rule):
-    def __init__(self, player_to_pawn: dict[Player, Callable[[], Piece]]):
-        self.player_to_pawn = player_to_pawn
 
+class SiberianSwipe(Rule):
     def on_join_board(self, board: Board):
-        board.subscribe(BeforeGetMoveOptionsEvent, self.on_before_get_move_options, EventPriority.HIGH)
-        board.subscribe(BeforeMoveEvent, self.on_before_move)
+        for piece in board.get_pieces():
+            self.subscribe_to_piece(piece)
+
+        board.subscribe(AfterNewPieceEvent, self.on_new_piece)
+
+    def subscribe_to_piece(self, piece: Piece):
+        if isinstance(piece, Rook):
+            piece.subscribe(BeforeGetMoveOptionsEvent, self.on_before_get_move_options, EventPriority.HIGH)
+
+    def on_new_piece(self, event: AfterNewPieceEvent):
+        self.subscribe_to_piece(event.piece)
 
     def on_before_get_move_options(self, event: BeforeGetMoveOptionsEvent):
-        f6_piece = event.piece.board[F6].piece
+        move_options = event.move_options
+        rook: Rook = event.piece
+        board = event.piece.board
+        player = event.piece.player
+        position = event.piece.position
+        new_move_options = []
 
-        if f6_piece is not None and f6_piece.player != event.piece.player:
-            move_options = list(event.move_options)
-            move_options.append(MoveOption(F6, extra=dict(summon_pawn=True), captures={F6}))
-            event.set_move_options(move_options)
-
-    def on_before_move(self, event: BeforeMoveEvent):
-        if event.move_option.extra.get("summon_pawn"):
-            piece = self.player_to_pawn[event.piece.player]()
-            event.piece.board[F6].piece = piece
-            piece.move(MoveOption(F6))
-            event.set_move_option(MoveOption(event.piece.position))
-            event.set_cancelled(True)
+        if rook.moved:
+            return
 
-    def clone(self):
-        return OmnipotentF6Pawn(player_to_pawn=self.player_to_pawn)
+        for direction in [(0, 1), (0, -1)]:
+            enemy_position = position.offset(*direction)
+
+            while is_in_board(board, enemy_position):
+                enemy_piece = board[enemy_position].piece
 
+                if isinstance(enemy_piece, Rook) and enemy_piece.player != player:
+                    move_option = MoveOption(enemy_position, captures={enemy_position}, extra=dict(siberian_swipe=True))
+                    new_move_options.append(move_option)
 
+                enemy_position = enemy_position.offset(*direction)
 
+        event.set_move_options(chain(move_options, new_move_options))
+
+    def clone(self):
+        return SiberianSwipe()
```

### Comparing `chessmaker-0.1.2/chessmaker/clients/pywebio_ui.py` & `chessmaker-0.2/chessmaker/clients/pywebio_ui.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from copy import deepcopy
 from dataclasses import dataclass, field
+from functools import partial
 from itertools import groupby
 from typing import Callable, List, ParamSpec, TypeVar, Optional, Any
 from uuid import uuid4
 
 from pywebio import start_server, config
 from pywebio.input import input_group, actions, checkbox, radio
 from pywebio.io_ctrl import Output
@@ -33,37 +34,41 @@
 div[id='pywebio-scope-board'] .btn {width: 80px; height: 80px;}
 .pywebio {min-height:calc(100vh - 50px);}
 div[id$="-move-option"] button {color: #bdc6c8; display: inline-flex; align-item: flex-start;
  vertical-align: top; padding: 0px; line-height: 0.75; font-style: italic; font-size: 11px;
  white-space: nowrap;}
 """
 
+PIECE_URL_TEMPLATE = "https://www.chess.com/chess-themes/pieces/neo/150/{piece_color}{piece_type}.png"
+PIECE_TYPES = {"Pawn": "p", "Rook": "r", "Knight": "n", "Bishop": "b", "Queen": "q", "King": "k"}
 
+PIECE_URLS: dict[str, tuple[str, ...]] = {}
+for piece, piece_type in PIECE_TYPES.items():
+    PIECE_URLS[piece] = (
+        PIECE_URL_TEMPLATE.format(piece_color="w", piece_type=piece_type),
+        PIECE_URL_TEMPLATE.format(piece_color="b", piece_type=piece_type),
+    )
+    
 @dataclass
 class MultiplayerGame:
     game: Game
     options: list[str]
     sessions: List[ThreadBasedSession] = field(default_factory=list)
     colors: dict[str, str] = field(default_factory=dict)
+    piece_urls: dict[str, tuple[str, ...]] = field(default_factory=lambda: PIECE_URLS)
 
 
+public_games: dict[str, MultiplayerGame] = {}
 multiplayer_games: dict[str, MultiplayerGame] = {}
 
-piece_types = {
-    "Pawn": "p",
-    "Rook": "r",
-    "Knight": "n",
-    "Bishop": "b",
-    "Queen": "q",
-    "King": "k"
-}
 
 PS = ParamSpec("PS")
 RT = TypeVar("RT")
 
+
 def for_all_game_sessions(func: Callable[PS, RT]) -> Callable[PS, RT]:
     game_id = session_data.game_id
 
     def wrapper(*args, **kwargs):
         game = multiplayer_games[game_id]
         for session in game.sessions:
             func_id = str(uuid4())
@@ -86,31 +91,31 @@
             with use_scope(str(position), clear=True):
                 put_scope(str(uuid4()), square_content(board[position]))
         session_data.shown_move_options = None
         session_data.clicked_position = None
 
 
 def get_piece_url(piece: Piece):
-    piece_color = multiplayer_games[session_data.game_id].colors[piece.player.name]
-    if piece.name == "Knook":
-        if piece_color == "w":
-            return "https://i.imgur.com/UiWcdEb.png"
-        else:
-            return "https://i.imgur.com/g7xTVts.png"
+    multiplayer_game = multiplayer_games[session_data.game_id]
+    player_index = list(multiplayer_game.colors.keys()).index(piece.player.name)
+    return multiplayer_game.piece_urls[piece.name][player_index]
 
-    piece_type = piece_types[piece.name]
 
-    return f"https://www.chess.com/chess-themes/pieces/neo/150/{piece_color}{piece_type}.png"
+def move_piece(piece: Piece, move_option: MoveOption):
+    if session_data.clicked_position is None:
+        return
+    session_data.clicked_position = None
+    piece.move(move_option)
 
 
 def show_multiple_move_options(piece: Piece, move_options: List[MoveOption]):
     with popup("Choose an option"):
         for move_option in move_options:
             def on_click(_move_option=deepcopy(move_option)):
-                piece.move(_move_option)
+                move_piece(piece, _move_option)
                 close_popup()
 
             if move_option.extra:
                 text = ", ".join([f"{key.title()}: {value}" for key, value in move_option.extra.items()])
             else:
                 text = "Move"
 
@@ -132,15 +137,15 @@
 
         with use_scope(str(move_option_position), clear=True):
             with use_scope(f"{move_option_position}-move-option"):
 
                 text = ""
                 if len(position_move_options) == 1:
                     move_option = position_move_options[0]
-                    on_click = lambda _move_option=move_option: piece.move(_move_option)
+                    on_click = lambda _move_option=move_option: move_piece(piece, _move_option)
                     if move_option.extra:
                         text = list(move_option.extra.keys())[0].capitalize().replace("_", " ")
                 else:
                     on_click = lambda _move_options=position_move_options: show_multiple_move_options(piece,
                                                                                                       _move_options)
                     text = "Multiple options"
 
@@ -280,77 +285,103 @@
     multiplayer_games[game_id].sessions.append(ThreadBasedSession.get_current_session())
     game = multiplayer_games[game_id].game
 
     session_data.game = game
     session_data.game_id = game_id
     session_data.own_game = False
 
+    put_markdown("""# ChessMaker \n """).style("text-align:center")
+    put_text("Invite URL: " + eval_js("window.location.href.split('?')[0]") + "?game_id=" + session_data.game_id)
     initialize_board()
+    put_markdown("[Docs](https://wolfdwyc.github.io/ChessMaker) - [Source](https://github.com/WolfDWyc/ChessMaker)\nMade by WolfDWyc").style("text-align:center")
+
 
-def new_game(game_factory: Callable[..., Game], options: list[str], mode: str):
+def new_game(game_factory: Callable[..., Game], options: list[str], mode: str, piece_urls: dict[str, tuple[str, ...]]):
     game: Game = game_factory(**{option: True for option in options})
     game_id = str(uuid4())
 
     session_data.game = game
     session_data.game_id = game_id
 
-    multiplayer_game = MultiplayerGame(game, options, [ThreadBasedSession.get_current_session()])
+    multiplayer_game = MultiplayerGame(game, options, [ThreadBasedSession.get_current_session()], {}, piece_urls)
     colors = ['w', 'b']
     for player in game.board.players:
         multiplayer_game.colors[player.name] = colors.pop(0)
 
     multiplayer_games[game_id] = multiplayer_game
+    if mode == 'Multiplayer (Public)':
+        public_games[game_id] = multiplayer_game
 
     session_data.own_game = True
-    if mode == 'Multiplayer':
+    if mode != 'Singleplayer':
         session_data.player = game.board.current_player
     else:
         session_data.player = ""
 
-    # game.board.subscribe(AfterAddPieceEvent, for_all_game_sessions(on_after_change_piece))
-    # game.board.subscribe(AfterRemovePieceEvent, for_all_game_sessions(on_after_change_piece))
     game.board.subscribe(AfterMoveEvent, for_all_game_sessions(on_after_move))
     game.board.subscribe(AfterTurnChangeEvent, for_all_game_sessions(on_after_turn_change))
     game.subscribe(AfterGameEndEvent, for_all_game_sessions(on_game_end))
 
-    put_markdown("# Chess \n").style("text-align:center")
-    if mode == 'Multiplayer':
+    put_markdown("""# ChessMaker \n """).style("text-align:center")
+    if mode == 'Multiplayer (Private)':
         put_text("Invite URL: " + eval_js("window.location.href.split('?')[0]") + "?game_id=" + session_data.game_id)
     initialize_board()
+    put_markdown("[Docs](https://wolfdwyc.github.io/ChessMaker) - [Source](https://github.com/WolfDWyc/ChessMaker)\nMade by WolfDWyc").style("text-align:center")
 
 
 def start_pywebio_chess_server(
         game_factory: Callable[..., Game],
         supported_options: List[str] = None,
+        piece_urls: dict[str, tuple[str, ...]] = PIECE_URLS,
         remote_access: bool = False,
-        port: int = 8080,
+        port: int = 8000,
         debug: bool = False,
 ):
     if supported_options is None:
         supported_options = []
 
-    @config(title="Chess", css_style=CSS)
+    @config(
+        title="ChessMaker",
+        description="An easily extendible chess implementation designed to support any custom rule or feature.",
+        css_style=CSS
+    )
     def main():
         if get_query("game_id"):
             if get_query("game_id") not in multiplayer_games:
                 popup("Error", put_error("Game not found"))
             else:
                 join_game(get_query("game_id"))
             return
+
         form_result = input_group('New Game', [
-            radio('Mode', ['Singleplayer', 'Multiplayer'], name='mode', value='Multiplayer'),
+            radio('Mode', ['Singleplayer', 'Multiplayer (Private)', 'Multiplayer (Public)'], name='mode', value='Singleplayer'),
             checkbox('Options',
                      options=supported_options,
                      name='options'),
+            actions('Public Games', [
+                {'label': f"Join game: {', '.join(public_game.options) or 'standard'}", 'value': game_id}
+                for game_id, public_game in public_games.items()
+                ], name='public_games'),
             actions('-', [
                 {'label': 'Create ', 'value': 'create'},
             ], name='action'),
         ])
 
-        new_game(game_factory, form_result['options'], form_result['mode'])
+        if form_result['public_games'] is not None:
+            public_games.pop(form_result['public_games'])
+            join_game(form_result['public_games'])
+            return
+
+        new_game(game_factory, form_result['options'], form_result['mode'], piece_urls)
 
     start_server(main, port=port, remote_access=remote_access, debug=debug)
 
 
 if __name__ == "__main__":
-    start_pywebio_chess_server(create_game, ["chess960", "knooks", "forced_en_passant", "knight_boosting", "omnipotent_f6_pawn",
-                              "siberian_swipe", "il_vaticano", "beta_decay"], debug=True)
+    start_pywebio_chess_server(
+        create_game,
+        supported_options=["chess960", "knooks", "forced_en_passant", "knight_boosting", "omnipotent_f6_pawn",
+                           "siberian_swipe", "il_vaticano", "beta_decay", "la_bastarda", "king_cant_move_to_c2",
+                           "vertical_castling", "double_check_to_win", "capture_all_pieces_to_win"],
+        debug=True,
+        piece_urls=PIECE_URLS | {"Knook": ["https://i.imgur.com/UiWcdEb.png", "https://i.imgur.com/g7xTVts.png"]}
+    )
```

### Comparing `chessmaker-0.1.2/chessmaker/events/event_publisher.py` & `chessmaker-0.2/chessmaker/events/event_publisher.py`

 * *Files identical despite different names*

