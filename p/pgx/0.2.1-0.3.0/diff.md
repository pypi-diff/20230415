# Comparing `tmp/pgx-0.2.1.tar.gz` & `tmp/pgx-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgx-0.2.1.tar", last modified: Wed Mar 29 02:28:14 2023, max compression
+gzip compressed data, was "pgx-0.3.0.tar", last modified: Sat Apr 15 18:29:16 2023, max compression
```

## Comparing `pgx-0.2.1.tar` & `pgx-0.3.0.tar`

### file list

```diff
@@ -1,132 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 02:28:14.959416 pgx-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-29 02:28:03.000000 pgx-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-29 02:28:14.959416 pgx-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9078 2023-03-29 02:28:03.000000 pgx-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 02:28:14.935416 pgx-0.2.1/pgx/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32646 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_animal_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    33481 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123) 11106175 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    48097 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_chess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 02:28:14.943416 pgx-0.2.1/pgx/_dwg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/animalshogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/hex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 02:28:14.943416 pgx-0.2.1/pgx/_dwg/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 02:28:14.947416 pgx-0.2.1/pgx/_dwg/images/chess/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/chess/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/chess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/chess/bBishop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/chess/bKing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/chess/bKnight.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/chess/bPawn.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/chess/bQueen.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/chess/bRook.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/chess/wBishop.svg
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/chess/wKing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/chess/wKnight.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/chess/wPawn.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/chess/wQueen.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/chess/wRook.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 02:28:14.951417 pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/
--rw-r--r--   0 runner    (1001) docker     (123)    45499 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/1p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45511 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/1pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/2p.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/2pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/3p.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/3pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/4p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/4pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/5p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/5pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/6p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/6pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/7p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/7pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15152 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/8p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/8pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/9p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/9pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/b.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/gd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/oya.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/rd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/leduc_holdem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_dwg/tictactoe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 02:28:14.951417 pgx-0.2.1/pgx/_flax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_flax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15107 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_flax/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_flax/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_shogi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    23399 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18240 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 02:28:14.951417 pgx-0.2.1/pgx/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/experimental/gym.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/experimental/pettingzoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/experimental/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/experimental/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/experimental/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18192 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/hex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/leduc_holdem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 02:28:14.955417 pgx-0.2.1/pgx/minatar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/minatar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12372 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/minatar/asterix.py
--rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/minatar/breakout.py
--rw-r--r--   0 runner    (1001) docker     (123)     8394 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/minatar/freeway.py
--rw-r--r--   0 runner    (1001) docker     (123)    25832 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/minatar/seaquest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/minatar/space_invaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/minatar/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)    20566 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    21142 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-03-29 02:28:03.000000 pgx-0.2.1/pgx/tic_tac_toe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 02:28:14.939416 pgx-0.2.1/pgx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-29 02:28:14.000000 pgx-0.2.1/pgx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-03-29 02:28:14.000000 pgx-0.2.1/pgx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 02:28:14.000000 pgx-0.2.1/pgx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-29 02:28:14.000000 pgx-0.2.1/pgx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-29 02:28:14.000000 pgx-0.2.1/pgx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-03-29 02:28:03.000000 pgx-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 02:28:14.959416 pgx-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-03-29 02:28:03.000000 pgx-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 02:28:14.959416 pgx-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 02:28:03.000000 pgx-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-03-29 02:28:03.000000 pgx-0.2.1/tests/minatar_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17650 2023-03-29 02:28:03.000000 pgx-0.2.1/tests/test_animal_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-03-29 02:28:03.000000 pgx-0.2.1/tests/test_asterix.py
--rw-r--r--   0 runner    (1001) docker     (123)    17435 2023-03-29 02:28:03.000000 pgx-0.2.1/tests/test_backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-03-29 02:28:03.000000 pgx-0.2.1/tests/test_breakout.py
--rw-r--r--   0 runner    (1001) docker     (123)    50826 2023-03-29 02:28:03.000000 pgx-0.2.1/tests/test_bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    15568 2023-03-29 02:28:03.000000 pgx-0.2.1/tests/test_chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-03-29 02:28:03.000000 pgx-0.2.1/tests/test_connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-03-29 02:28:03.000000 pgx-0.2.1/tests/test_freeway.py
--rw-r--r--   0 runner    (1001) docker     (123)    39629 2023-03-29 02:28:03.000000 pgx-0.2.1/tests/test_go.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-03-29 02:28:03.000000 pgx-0.2.1/tests/test_hex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-03-29 02:28:03.000000 pgx-0.2.1/tests/test_kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-03-29 02:28:03.000000 pgx-0.2.1/tests/test_leduc_holdem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-03-29 02:28:03.000000 pgx-0.2.1/tests/test_othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-03-29 02:28:03.000000 pgx-0.2.1/tests/test_play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-03-29 02:28:03.000000 pgx-0.2.1/tests/test_seaquest.py
--rw-r--r--   0 runner    (1001) docker     (123)    17534 2023-03-29 02:28:03.000000 pgx-0.2.1/tests/test_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-03-29 02:28:03.000000 pgx-0.2.1/tests/test_space_invaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    22436 2023-03-29 02:28:03.000000 pgx-0.2.1/tests/test_sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-03-29 02:28:03.000000 pgx-0.2.1/tests/test_tic_tac_toe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:16.267836 pgx-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-15 18:29:07.000000 pgx-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-15 18:29:16.267836 pgx-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9565 2023-04-15 18:29:07.000000 pgx-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:16.255836 pgx-0.3.0/pgx/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123) 11106175 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25378 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_chess_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:16.259836 pgx-0.3.0/pgx/_dwg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/animalshogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/hex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:16.259836 pgx-0.3.0/pgx/_dwg/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:16.259836 pgx-0.3.0/pgx/_dwg/images/chess/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/chess/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/chess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/chess/bBishop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/chess/bKing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/chess/bKnight.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/chess/bPawn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/chess/bQueen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/chess/bRook.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/chess/wBishop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/chess/wKing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/chess/wKnight.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/chess/wPawn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/chess/wQueen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/chess/wRook.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:16.263836 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/
+-rw-r--r--   0 runner    (1001) docker     (123)    45499 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/1p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45511 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/1pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/2p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/2pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/3p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/3pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/4p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/4pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/5p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/5pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/6p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/6pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/7p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/7pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15152 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/8p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/8pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/9p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/9pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/gd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/oya.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/rd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_dwg/tictactoe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:16.263836 pgx-0.3.0/pgx/_flax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_flax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15107 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_flax/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_flax/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_shogi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23850 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/animal_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18240 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43936 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28856 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:16.263836 pgx-0.3.0/pgx/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/experimental/gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/experimental/pettingzoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/experimental/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/experimental/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/experimental/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18192 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/leduc_holdem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:16.263836 pgx-0.3.0/pgx/minatar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/minatar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12372 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/minatar/asterix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/minatar/breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8394 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/minatar/freeway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25832 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/minatar/seaquest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/minatar/space_invaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/minatar/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20566 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21142 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-15 18:29:07.000000 pgx-0.3.0/pgx/tic_tac_toe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:16.255836 pgx-0.3.0/pgx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-15 18:29:16.000000 pgx-0.3.0/pgx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-15 18:29:16.000000 pgx-0.3.0/pgx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 18:29:16.000000 pgx-0.3.0/pgx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-15 18:29:16.000000 pgx-0.3.0/pgx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-15 18:29:16.000000 pgx-0.3.0/pgx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-15 18:29:07.000000 pgx-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 18:29:16.267836 pgx-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-15 18:29:07.000000 pgx-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:16.267836 pgx-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/minatar_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_animal_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_asterix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17435 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61039 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29734 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_freeway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39629 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_seaquest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17534 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_space_invaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22436 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-04-15 18:29:07.000000 pgx-0.3.0/tests/test_tic_tac_toe.py
```

### Comparing `pgx-0.2.1/LICENSE` & `pgx-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/README.md` & `pgx-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -85,484 +85,514 @@
 00000540: 542d 6162 6c65 2a0a 2d20 2a2a 5375 7065  T-able*.- **Supe
 00000550: 7220 6661 7374 2a2a 2069 6e20 7061 7261  r fast** in para
 00000560: 6c6c 656c 2065 7865 6375 7469 6f6e 206f  llel execution o
 00000570: 6e20 6163 6365 6c65 7261 746f 7273 0a2d  n accelerators.-
 00000580: 202a 2a56 6172 696f 7573 2067 616d 6520   **Various game 
 00000590: 7375 7070 6f72 742a 2a20 696e 636c 7564  support** includ
 000005a0: 696e 6720 2a2a 4261 636b 6761 6d6d 6f6e  ing **Backgammon
-000005b0: 2a2a 2c20 2a2a 5368 6f67 692a 2a2c 2061  **, **Shogi**, a
-000005c0: 6e64 202a 2a47 6f2a 2a0a 2d20 2a2a 4265  nd **Go**.- **Be
-000005d0: 6175 7469 6675 6c20 7669 7375 616c 697a  autiful visualiz
-000005e0: 6174 696f 6e2a 2a20 696e 2053 5647 2066  ation** in SVG f
-000005f0: 6f72 6d61 740a 0a0a 2323 2049 6e73 7461  ormat...## Insta
-00000600: 6c6c 0a0a 6060 6073 680a 7069 7020 696e  ll..```sh.pip in
-00000610: 7374 616c 6c20 7067 780a 6060 600a 0a23  stall pgx.```..#
-00000620: 2320 5573 6167 650a 0a60 6060 7079 0a69  # Usage..```py.i
-00000630: 6d70 6f72 7420 6a61 780a 696d 706f 7274  mport jax.import
-00000640: 2070 6778 0a0a 656e 7620 3d20 7067 782e   pgx..env = pgx.
-00000650: 6d61 6b65 2822 676f 2d31 3978 3139 2229  make("go-19x19")
-00000660: 0a69 6e69 7420 3d20 6a61 782e 6a69 7428  .init = jax.jit(
-00000670: 6a61 782e 766d 6170 2865 6e76 2e69 6e69  jax.vmap(env.ini
-00000680: 7429 2920 2023 2076 6563 746f 7269 7a65  t))  # vectorize
-00000690: 2061 6e64 204a 4954 2d63 6f6d 7069 6c65   and JIT-compile
-000006a0: 0a73 7465 7020 3d20 6a61 782e 6a69 7428  .step = jax.jit(
-000006b0: 6a61 782e 766d 6170 2865 6e76 2e73 7465  jax.vmap(env.ste
-000006c0: 7029 290a 0a62 6174 6368 5f73 697a 6520  p))..batch_size 
-000006d0: 3d20 3130 3234 0a6b 6579 7320 3d20 6a61  = 1024.keys = ja
-000006e0: 782e 7261 6e64 6f6d 2e73 706c 6974 286a  x.random.split(j
-000006f0: 6178 2e72 616e 646f 6d2e 5052 4e47 4b65  ax.random.PRNGKe
-00000700: 7928 3432 292c 2062 6174 6368 5f73 697a  y(42), batch_siz
-00000710: 6529 0a73 7461 7465 203d 2069 6e69 7428  e).state = init(
-00000720: 6b65 7973 2920 2023 2076 6563 746f 7269  keys)  # vectori
-00000730: 7a65 6420 7374 6174 6573 0a77 6869 6c65  zed states.while
-00000740: 206e 6f74 2073 7461 7465 2e74 6572 6d69   not state.termi
-00000750: 6e61 7465 642e 616c 6c28 293a 0a20 2020  nated.all():.   
-00000760: 2061 6374 696f 6e20 3d20 6d6f 6465 6c28   action = model(
-00000770: 7374 6174 652e 6375 7272 656e 745f 706c  state.current_pl
-00000780: 6179 6572 2c20 7374 6174 652e 6f62 7365  ayer, state.obse
-00000790: 7276 6174 696f 6e2c 2073 7461 7465 2e6c  rvation, state.l
-000007a0: 6567 616c 5f61 6374 696f 6e5f 6d61 736b  egal_action_mask
-000007b0: 290a 2020 2020 7374 6174 6520 3d20 7374  ).    state = st
-000007c0: 6570 2873 7461 7465 2c20 6163 7469 6f6e  ep(state, action
-000007d0: 2920 2023 2073 7461 7465 2e72 6577 6172  )  # state.rewar
-000007e0: 6420 2832 2c29 0a60 6060 0a0a 3c21 2d2d  d (2,).```..<!--
-000007f0: 2d0a 2323 2320 4c69 6d69 7461 7469 6f6e  -.### Limitation
-00000800: 7320 2866 6f72 2074 6865 2073 696d 706c  s (for the simpl
-00000810: 6963 6974 7929 0a2a 2044 6f65 7320 2a2a  icity).* Does **
-00000820: 4e4f 542a 2a20 7375 7070 6f72 7420 6167  NOT** support ag
-00000830: 656e 7420 6465 6174 6820 616e 6420 6372  ent death and cr
-00000840: 6561 7469 6f6e 2c20 7768 6963 6820 6479  eation, which dy
-00000850: 6e6d 6963 616c 6c79 2063 6861 6e67 6573  nmically changes
-00000860: 2074 6865 2061 7272 6179 2073 697a 652e   the array size.
-00000870: 2049 7420 646f 6573 206e 6f74 2077 656c   It does not wel
-00000880: 6c20 7375 6974 2074 6f20 4750 552d 6163  l suit to GPU-ac
-00000890: 6365 6c65 7261 7465 6420 636f 6d70 7574  celerated comput
-000008a0: 6174 696f 6e2e 0a2a 2044 6f65 7320 2a2a  ation..* Does **
-000008b0: 4e4f 542a 2a20 7375 7070 6f72 7420 4368  NOT** support Ch
-000008c0: 616e 6365 2070 6c61 7965 7220 284e 6174  ance player (Nat
-000008d0: 7572 6520 706c 6179 6572 2920 7769 7468  ure player) with
-000008e0: 2061 6374 696f 6e20 7365 6c65 6374 696f   action selectio
-000008f0: 6e2e 0a2a 2044 6f65 7320 2a2a 4e4f 542a  n..* Does **NOT*
-00000900: 2a20 7375 7070 6f72 7420 4f70 656e 4149  * support OpenAI
-00000910: 2047 796d 2041 5049 2e0a 2020 2020 2a20   Gym API..    * 
-00000920: 4f70 656e 4149 2047 796d 2069 7320 666f  OpenAI Gym is fo
-00000930: 7220 7369 6e67 6c65 2d61 6765 6e74 2065  r single-agent e
-00000940: 6e76 6972 6f6e 6d65 6e74 2e20 4d6f 7374  nvironment. Most
-00000950: 206f 6620 5067 7820 656e 7669 726f 6e6d   of Pgx environm
-00000960: 656e 7473 2061 7265 206d 756c 7469 2d70  ents are multi-p
-00000970: 6c61 7965 7220 6761 6d65 732e 204a 7573  layer games. Jus
-00000980: 7420 6465 6669 6e69 6e67 206f 7070 6f6e  t defining oppon
-00000990: 656e 7473 2069 7320 6e6f 7420 656e 6f75  ents is not enou
-000009a0: 6768 2066 6f72 2063 6f6e 7665 7274 696e  gh for convertin
-000009b0: 6720 6d75 6c74 692d 6167 656e 7420 656e  g multi-agent en
-000009c0: 7669 726f 6e65 6d6e 7473 2074 6f20 4f70  vironemnts to Op
-000009d0: 656e 4149 2047 796d 2065 6e76 6972 6f6e  enAI Gym environ
-000009e0: 6d65 6e74 2e20 452e 672e 2c20 696e 2074  ment. E.g., in t
-000009f0: 6865 2067 616d 6520 6f66 2067 6f2c 2074  he game of go, t
-00000a00: 6865 206e 6578 7420 7374 6174 6520 7327  he next state s'
-00000a10: 2069 7320 6465 6669 6e65 6420 6173 2074   is defined as t
-00000a20: 6865 2073 7461 7465 206a 7573 7420 6166  he state just af
-00000a30: 7465 7220 706c 6163 696e 6720 6120 7374  ter placing a st
-00000a40: 6f6e 6520 696e 2041 6c68 6147 6f20 7061  one in AlhaGo pa
-00000a50: 7065 722e 2048 6f77 6576 6572 2c20 7327  per. However, s'
-00000a60: 2062 6563 6f6d 6573 2074 6865 2073 7461   becomes the sta
-00000a70: 7465 2061 6674 6572 2074 6865 206f 7070  te after the opp
-00000a80: 6f6e 656e 7473 2720 706c 6179 2e20 5468  onents' play. Th
-00000a90: 6973 2063 6861 6e67 6573 2074 6865 2064  is changes the d
-00000aa0: 6566 696e 6974 696f 6e20 6f66 2056 2873  efinition of V(s
-00000ab0: 2729 2e0a 2a20 446f 6573 202a 2a4e 4f54  ')..* Does **NOT
-00000ac0: 2a2a 2073 7570 706f 7274 2050 6574 7469  ** support Petti
-00000ad0: 6e67 5a6f 6f20 4150 492e 0a20 2020 202a  ngZoo API..    *
-00000ae0: 2050 6574 7469 6e67 5a6f 6f20 6973 202a   PettingZoo is *
-00000af0: 4779 6d20 666f 7220 6d75 6c74 692d 6167  Gym for multi-ag
-00000b00: 656e 7420 524c 2a2e 2041 7320 6661 7220  ent RL*. As far 
-00000b10: 6173 2077 6520 6b6e 6f77 2c20 5065 7474  as we know, Pett
-00000b20: 696e 675a 6f6f 2064 6f65 7320 6e6f 7420  ingZoo does not 
-00000b30: 7375 7070 6f72 7420 7665 6374 6f72 697a  support vectoriz
-00000b40: 6564 2065 6e76 6972 6f6e 6d65 6e74 7320  ed environments 
-00000b50: 286c 696b 6520 5665 6374 6f72 456e 7620  (like VectorEnv 
-00000b60: 696e 204f 7065 6e41 4920 4779 6d29 2e20  in OpenAI Gym). 
-00000b70: 4173 2050 6778 2773 206d 6169 6e20 6665  As Pgx's main fe
-00000b80: 6174 7572 6520 6973 2068 6967 686c 7920  ature is highly 
-00000b90: 7665 6374 6f72 697a 6564 2065 6e76 6972  vectorized envir
-00000ba0: 6f6e 6d65 6e74 2076 6961 2047 5055 2f54  onment via GPU/T
-00000bb0: 5055 2073 7570 706f 7274 2c20 5765 2064  PU support, We d
-00000bc0: 6f20 6e6f 7420 6375 7272 656e 746c 7920  o not currently 
-00000bd0: 7375 7070 6f72 7420 5065 7474 696e 675a  support PettingZ
-00000be0: 6f6f 2041 5049 2e20 0a0a 2323 2320 6073  oo API. ..### `s
-00000bf0: 6b69 705f 6368 616e 6365 600a 2a20 5765  kip_chance`.* We
-00000c00: 2070 7265 7061 7265 2073 6b69 705f 6368   prepare skip_ch
-00000c10: 616e 6365 3d54 7275 6520 6f70 7469 6f6e  ance=True option
-00000c20: 2066 6f72 2073 6f6d 6520 656e 7669 726f   for some enviro
-00000c30: 6e6d 656e 7473 2e20 5468 6973 206d 616b  nments. This mak
-00000c40: 6573 2069 7420 706f 7373 6962 6c65 2074  es it possible t
-00000c50: 6f20 636f 6e73 6964 6572 2076 616c 7565  o consider value
-00000c60: 2066 756e 6374 696f 6e20 666f 7220 2270   function for "p
-00000c70: 6f73 742d 6465 6369 7369 6f6e 2073 7461  ost-decision sta
-00000c80: 7465 7322 2028 5365 6520 416c 676f 524c  tes" (See AlgoRL
-00000c90: 2062 6f6f 6b29 2e20 486f 7765 7665 722c   book). However,
-00000ca0: 2077 6520 646f 206e 6f74 2061 6c6c 6f77   we do not allow
-00000cb0: 2063 6861 6e63 6520 6167 656e 7420 746f   chance agent to
-00000cc0: 2063 686f 6f73 6520 6163 7469 6f6e 206c   choose action l
-00000cd0: 696b 6520 4f70 656e 5370 6965 6c2e 2054  ike OpenSpiel. T
-00000ce0: 6869 7320 6973 2062 6563 6175 7365 2074  his is because t
-00000cf0: 6865 2061 6374 696f 6e20 7370 6163 6520  he action space 
-00000d00: 6f66 2063 6861 6e63 6520 6167 656e 7420  of chance agent 
-00000d10: 616e 6420 7573 7561 6c20 6167 656e 7420  and usual agent 
-00000d20: 6172 6520 6469 6666 6572 656e 742e 2054  are different. T
-00000d30: 6875 732c 2077 6865 6e20 7468 6520 6368  hus, when the ch
-00000d40: 616e 6365 2070 6c61 7965 7220 6973 2063  ance player is c
-00000d50: 686f 7365 6e20 2860 6375 7272 656e 745f  hosen (`current_
-00000d60: 706c 6179 6572 3d2d 3160 292c 2060 6163  player=-1`), `ac
-00000d70: 7469 6f6e 3d2d 3160 206d 7573 7420 6265  tion=-1` must be
-00000d80: 2072 6574 7572 6e65 6420 746f 2073 7465   returned to ste
-00000d90: 7020 6675 6e63 7469 6f6e 2e20 5573 6520  p function. Use 
-00000da0: 6073 6875 6666 6c65 6020 746f 206d 616b  `shuffle` to mak
-00000db0: 6520 6073 7465 7060 2073 746f 6368 6173  e `step` stochas
-00000dc0: 7469 632e 0a0a 2323 2320 7472 756e 6361  tic...### trunca
-00000dd0: 7461 7469 6f6e 2061 6e64 2061 7574 6f5f  tation and auto_
-00000de0: 7265 7365 740a 2a20 7375 7070 6f72 7465  reset.* supporte
-00000df0: 6420 6279 2060 6d61 6b65 2865 6e76 5f69  d by `make(env_i
-00000e00: 643d 222e 2e2e 222c 2061 7574 6f5f 7265  d="...", auto_re
-00000e10: 7365 743d 5472 7565 2c20 6d61 785f 6570  set=True, max_ep
-00000e20: 6973 6f64 655f 6c65 6e67 7468 3d36 3429  isode_length=64)
-00000e30: 600a 2a20 6061 7574 6f5f 7265 7365 7460  `.* `auto_reset`
-00000e40: 2077 696c 6c20 7265 706c 6163 6520 7468   will replace th
-00000e50: 6520 7465 726d 696e 616c 2073 7461 7465  e terminal state
-00000e60: 2062 7920 696e 6974 6961 6c20 7374 6174   by initial stat
-00000e70: 6520 2862 7574 2060 6973 5f74 6572 6d69  e (but `is_termi
-00000e80: 6e61 6c3d 5472 7565 6020 6973 2073 6574  nal=True` is set
-00000e90: 290a 2a20 6069 735f 7472 756e 6361 7465  ).* `is_truncate
-00000ea0: 643d 5472 7565 6020 6973 2061 6c73 6f20  d=True` is also 
-00000eb0: 7365 7420 746f 2073 7461 7465 0a2d 2d2d  set to state.---
-00000ec0: 3e0a 0a23 2320 5375 7070 6f72 7465 6420  >..## Supported 
-00000ed0: 6761 6d65 7320 616e 6420 726f 6164 206d  games and road m
-00000ee0: 6170 0a0a 3e20 3a77 6172 6e69 6e67 3a20  ap..> :warning: 
-00000ef0: 5067 7820 6973 2063 7572 7265 6e74 6c79  Pgx is currently
-00000f00: 2069 6e20 7468 6520 6265 7461 2076 6572   in the beta ver
-00000f10: 7369 6f6e 2e20 5468 6572 6566 6f72 652c  sion. Therefore,
-00000f20: 2041 5049 2069 7320 7375 626a 6563 7420   API is subject 
-00000f30: 746f 2063 6861 6e67 6520 7769 7468 6f75  to change withou
-00000f40: 7420 6e6f 7469 6365 2e20 5765 2061 696d  t notice. We aim
-00000f50: 2074 6f20 7265 6c65 6173 6520 7631 2e30   to release v1.0
-00000f60: 2e30 2069 6e20 4170 7269 6c20 3230 3233  .0 in April 2023
-00000f70: 2e20 4f70 696e 696f 6e73 2061 6e64 2063  . Opinions and c
-00000f80: 6f6d 6d65 6e74 7320 6172 6520 6d6f 7265  omments are more
-00000f90: 2074 6861 6e20 7765 6c63 6f6d 6521 0a0a   than welcome!..
-00000fa0: 5573 6520 6070 6778 2e61 7661 696c 6162  Use `pgx.availab
-00000fb0: 6c65 5f67 616d 6573 2829 6020 746f 2073  le_games()` to s
-00000fc0: 6565 2074 6865 206c 6973 7420 6f66 2063  ee the list of c
-00000fd0: 7572 7265 6e74 6c79 2061 7661 696c 6162  urrently availab
-00000fe0: 6c65 2067 616d 6573 2e0a 0a3c 6469 7620  le games...<div 
-00000ff0: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
-00001000: 3c69 6d67 2073 7263 3d22 6669 672f 7376  <img src="fig/sv
-00001010: 6773 2f32 3034 385f 6461 726b 2e73 7667  gs/2048_dark.svg
-00001020: 2367 682d 6461 726b 2d6d 6f64 652d 6f6e  #gh-dark-mode-on
-00001030: 6c79 2220 6865 6967 6874 3d22 3132 3070  ly" height="120p
-00001040: 7822 3e0a 3c69 6d67 2073 7263 3d22 6669  x">.<img src="fi
-00001050: 672f 7376 6773 2f62 6163 6b67 616d 6d6f  g/svgs/backgammo
-00001060: 6e5f 6461 726b 2e73 7667 2367 682d 6461  n_dark.svg#gh-da
-00001070: 726b 2d6d 6f64 652d 6f6e 6c79 2220 6865  rk-mode-only" he
-00001080: 6967 6874 3d22 3132 3070 7822 3e0a 3c69  ight="120px">.<i
-00001090: 6d67 2073 7263 3d22 6669 672f 7376 6773  mg src="fig/svgs
-000010a0: 2f67 6f2d 3978 395f 6461 726b 2e73 7667  /go-9x9_dark.svg
-000010b0: 2367 682d 6461 726b 2d6d 6f64 652d 6f6e  #gh-dark-mode-on
-000010c0: 6c79 2220 6865 6967 6874 3d22 3132 3070  ly" height="120p
-000010d0: 7822 3e0a 3c69 6d67 2073 7263 3d22 6669  x">.<img src="fi
-000010e0: 672f 7376 6773 2f6b 7568 6e5f 706f 6b65  g/svgs/kuhn_poke
-000010f0: 725f 6461 726b 2e73 7667 2367 682d 6461  r_dark.svg#gh-da
-00001100: 726b 2d6d 6f64 652d 6f6e 6c79 2220 6865  rk-mode-only" he
-00001110: 6967 6874 3d22 3132 3070 7822 3e0a 3c69  ight="120px">.<i
-00001120: 6d67 2073 7263 3d22 6669 672f 7376 6773  mg src="fig/svgs
-00001130: 2f73 686f 6769 5f64 6172 6b2e 7376 6723  /shogi_dark.svg#
-00001140: 6768 2d64 6172 6b2d 6d6f 6465 2d6f 6e6c  gh-dark-mode-onl
-00001150: 7922 2068 6569 6768 743d 2231 3230 7078  y" height="120px
-00001160: 223e 0a3c 2f64 6976 3e0a 0a3c 6469 7620  ">.</div>..<div 
-00001170: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
-00001180: 3c69 6d67 2073 7263 3d22 6669 672f 7376  <img src="fig/sv
-00001190: 6773 2f32 3034 385f 6c69 6768 742e 7376  gs/2048_light.sv
-000011a0: 6723 6768 2d6c 6967 6874 2d6d 6f64 652d  g#gh-light-mode-
-000011b0: 6f6e 6c79 2220 6865 6967 6874 3d22 3132  only" height="12
-000011c0: 3070 7822 3e0a 3c69 6d67 2073 7263 3d22  0px">.<img src="
-000011d0: 6669 672f 7376 6773 2f62 6163 6b67 616d  fig/svgs/backgam
-000011e0: 6d6f 6e5f 6c69 6768 742e 7376 6723 6768  mon_light.svg#gh
-000011f0: 2d6c 6967 6874 2d6d 6f64 652d 6f6e 6c79  -light-mode-only
-00001200: 2220 6865 6967 6874 3d22 3132 3070 7822  " height="120px"
-00001210: 3e0a 3c69 6d67 2073 7263 3d22 6669 672f  >.<img src="fig/
-00001220: 7376 6773 2f67 6f2d 3978 395f 6c69 6768  svgs/go-9x9_ligh
-00001230: 742e 7376 6723 6768 2d6c 6967 6874 2d6d  t.svg#gh-light-m
-00001240: 6f64 652d 6f6e 6c79 2220 6865 6967 6874  ode-only" height
-00001250: 3d22 3132 3070 7822 3e0a 3c69 6d67 2073  ="120px">.<img s
-00001260: 7263 3d22 6669 672f 7376 6773 2f6b 7568  rc="fig/svgs/kuh
-00001270: 6e5f 706f 6b65 725f 6c69 6768 742e 7376  n_poker_light.sv
-00001280: 6723 6768 2d6c 6967 6874 2d6d 6f64 652d  g#gh-light-mode-
-00001290: 6f6e 6c79 2220 6865 6967 6874 3d22 3132  only" height="12
-000012a0: 3070 7822 3e0a 3c69 6d67 2073 7263 3d22  0px">.<img src="
-000012b0: 6669 672f 7376 6773 2f73 686f 6769 5f6c  fig/svgs/shogi_l
-000012c0: 6967 6874 2e73 7667 2367 682d 6c69 6768  ight.svg#gh-ligh
-000012d0: 742d 6d6f 6465 2d6f 6e6c 7922 2068 6569  t-mode-only" hei
-000012e0: 6768 743d 2231 3230 7078 223e 0a3c 2f64  ght="120px">.</d
-000012f0: 6976 3e0a 0a3c 6469 7620 616c 6967 6e3d  iv>..<div align=
-00001300: 2263 656e 7465 7222 3e0a 3c74 6162 6c65  "center">.<table
-00001310: 3e0a 3c74 723e 0a20 203c 7468 3e47 616d  >.<tr>.  <th>Gam
-00001320: 653c 2f74 683e 0a20 203c 7468 3e45 6e76  e</th>.  <th>Env
-00001330: 6972 6f6e 6d65 6e74 3c2f 7468 3e0a 2020  ironment</th>.  
-00001340: 3c74 683e 5669 7375 616c 697a 6174 696f  <th>Visualizatio
-00001350: 6e3c 2f74 683e 0a3c 2f74 723e 0a3c 7472  n</th>.</tr>.<tr
-00001360: 3e0a 203c 7464 3e3c 6120 6872 6566 3d22  >. <td><a href="
-00001370: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
-00001380: 6564 6961 2e6f 7267 2f77 696b 692f 3230  edia.org/wiki/20
-00001390: 3438 5f28 7669 6465 6f5f 6761 6d65 2922  48_(video_game)"
-000013a0: 3e32 3034 383c 2f61 3e3c 2f74 643e 0a20  >2048</a></td>. 
-000013b0: 3c74 643e 3a77 6869 7465 5f63 6865 636b  <td>:white_check
-000013c0: 5f6d 6172 6b3a 3c2f 7464 3e0a 203c 7464  _mark:</td>. <td
-000013d0: 3e3a 7768 6974 655f 6368 6563 6b5f 6d61  >:white_check_ma
-000013e0: 726b 3a3c 2f74 643e 0a3c 2f74 723e 0a3c  rk:</td>.</tr>.<
-000013f0: 7472 3e0a 203c 7464 3e20 3c61 2068 7265  tr>. <td> <a hre
-00001400: 663d 2268 7474 7073 3a2f 2f65 6e2e 7769  f="https://en.wi
-00001410: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
-00001420: 2f44 2543 3525 3844 6275 7473 755f 7368  /D%C5%8Dbutsu_sh
-00001430: 2543 3525 3844 6769 223e 416e 696d 616c  %C5%8Dgi">Animal
-00001440: 2053 686f 6769 3c2f 613e 203c 2f74 643e   Shogi</a> </td>
-00001450: 0a20 3c74 643e 3a63 6f6e 7374 7275 6374  . <td>:construct
-00001460: 696f 6e3a 3c2f 7464 3e0a 203c 7464 3e3a  ion:</td>. <td>:
-00001470: 7768 6974 655f 6368 6563 6b5f 6d61 726b  white_check_mark
-00001480: 3a3c 2f74 643e 0a3c 2f74 723e 0a3c 7472  :</td>.</tr>.<tr
-00001490: 3e0a 203c 7464 3e3c 6120 6872 6566 3d22  >. <td><a href="
-000014a0: 6874 7470 733a 2f2f 656e 2e77 696b 6970  https://en.wikip
-000014b0: 6564 6961 2e6f 7267 2f77 696b 692f 4261  edia.org/wiki/Ba
-000014c0: 636b 6761 6d6d 6f6e 223e 4261 636b 6761  ckgammon">Backga
-000014d0: 6d6d 6f6e 3c2f 613e 3c2f 7464 3e0a 203c  mmon</a></td>. <
-000014e0: 7464 3e3a 7768 6974 655f 6368 6563 6b5f  td>:white_check_
-000014f0: 6d61 726b 3a3c 2f74 643e 0a20 3c74 643e  mark:</td>. <td>
-00001500: 3a77 6869 7465 5f63 6865 636b 5f6d 6172  :white_check_mar
-00001510: 6b3a 3c2f 7464 3e0a 3c2f 7472 3e0a 3c74  k:</td>.</tr>.<t
-00001520: 723e 0a20 3c74 643e 3c61 2068 7265 663d  r>. <td><a href=
-00001530: 2268 7474 7073 3a2f 2f65 6e2e 7769 6b69  "https://en.wiki
-00001540: 7065 6469 612e 6f72 672f 7769 6b69 2f43  pedia.org/wiki/C
-00001550: 6f6e 7472 6163 745f 6272 6964 6765 223e  ontract_bridge">
-00001560: 4272 6964 6765 2042 6964 6469 6e67 3c2f  Bridge Bidding</
-00001570: 613e 3c2f 7464 3e0a 203c 7464 3e3a 636f  a></td>. <td>:co
-00001580: 6e73 7472 7563 7469 6f6e 3a3c 2f74 643e  nstruction:</td>
-00001590: 0a20 3c74 643e 3a77 6869 7465 5f63 6865  . <td>:white_che
-000015a0: 636b 5f6d 6172 6b3a 3c2f 7464 3e0a 3c2f  ck_mark:</td>.</
-000015b0: 7472 3e0a 3c74 723e 0a20 3c74 643e 3c61  tr>.<tr>. <td><a
-000015c0: 2068 7265 663d 2268 7474 7073 3a2f 2f65   href="https://e
-000015d0: 6e2e 7769 6b69 7065 6469 612e 6f72 672f  n.wikipedia.org/
-000015e0: 7769 6b69 2f43 6865 7373 223e 4368 6573  wiki/Chess">Ches
-000015f0: 733c 2f61 3e3c 2f74 643e 0a20 3c74 643e  s</a></td>. <td>
-00001600: 3a63 6f6e 7374 7275 6374 696f 6e3a 3c2f  :construction:</
-00001610: 7464 3e0a 203c 7464 3e3a 7768 6974 655f  td>. <td>:white_
-00001620: 6368 6563 6b5f 6d61 726b 3a3c 2f74 643e  check_mark:</td>
-00001630: 0a3c 2f74 723e 0a3c 7472 3e0a 203c 7464  .</tr>.<tr>. <td
-00001640: 3e3c 6120 6872 6566 3d22 6874 7470 733a  ><a href="https:
-00001650: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
-00001660: 7267 2f77 696b 692f 436f 6e6e 6563 745f  rg/wiki/Connect_
-00001670: 466f 7572 223e 436f 6e6e 6563 7420 466f  Four">Connect Fo
-00001680: 7572 3c2f 613e 3c2f 7464 3e0a 203c 7464  ur</a></td>. <td
-00001690: 3e3a 7768 6974 655f 6368 6563 6b5f 6d61  >:white_check_ma
-000016a0: 726b 3a3c 2f74 643e 0a20 3c74 643e 3a77  rk:</td>. <td>:w
-000016b0: 6869 7465 5f63 6865 636b 5f6d 6172 6b3a  hite_check_mark:
-000016c0: 3c2f 7464 3e0a 3c2f 7472 3e0a 3c74 723e  </td>.</tr>.<tr>
-000016d0: 0a20 3c74 643e 3c61 2068 7265 663d 2268  . <td><a href="h
-000016e0: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
-000016f0: 6469 612e 6f72 672f 7769 6b69 2f47 6f5f  dia.org/wiki/Go_
-00001700: 2867 616d 6529 223e 476f 3c2f 613e 3c2f  (game)">Go</a></
-00001710: 7464 3e0a 203c 7464 3e3a 7768 6974 655f  td>. <td>:white_
-00001720: 6368 6563 6b5f 6d61 726b 3a3c 2f74 643e  check_mark:</td>
-00001730: 0a20 3c74 643e 3a77 6869 7465 5f63 6865  . <td>:white_che
-00001740: 636b 5f6d 6172 6b3a 3c2f 7464 3e0a 3c2f  ck_mark:</td>.</
-00001750: 7472 3e0a 3c74 723e 0a20 3c74 643e 3c61  tr>.<tr>. <td><a
-00001760: 2068 7265 663d 2268 7474 7073 3a2f 2f65   href="https://e
-00001770: 6e2e 7769 6b69 7065 6469 612e 6f72 672f  n.wikipedia.org/
-00001780: 7769 6b69 2f48 6578 5f28 626f 6172 645f  wiki/Hex_(board_
-00001790: 6761 6d65 2922 3e48 6578 3c2f 613e 3c2f  game)">Hex</a></
-000017a0: 7464 3e0a 203c 7464 3e3a 7768 6974 655f  td>. <td>:white_
-000017b0: 6368 6563 6b5f 6d61 726b 3a3c 2f74 643e  check_mark:</td>
-000017c0: 0a20 3c74 643e 3a77 6869 7465 5f63 6865  . <td>:white_che
-000017d0: 636b 5f6d 6172 6b3a 3c2f 7464 3e0a 3c2f  ck_mark:</td>.</
-000017e0: 7472 3e0a 3c74 723e 0a20 3c74 643e 3c61  tr>.<tr>. <td><a
-000017f0: 2068 7265 663d 2268 7474 7073 3a2f 2f65   href="https://e
-00001800: 6e2e 7769 6b69 7065 6469 612e 6f72 672f  n.wikipedia.org/
-00001810: 7769 6b69 2f4b 7568 6e5f 706f 6b65 7222  wiki/Kuhn_poker"
-00001820: 3e4b 7568 6e20 506f 6b65 723c 2f61 3e3c  >Kuhn Poker</a><
-00001830: 2f74 643e 0a20 3c74 643e 3a77 6869 7465  /td>. <td>:white
-00001840: 5f63 6865 636b 5f6d 6172 6b3a 3c2f 7464  _check_mark:</td
-00001850: 3e0a 203c 7464 3e3a 7768 6974 655f 6368  >. <td>:white_ch
-00001860: 6563 6b5f 6d61 726b 3a3c 2f74 643e 0a3c  eck_mark:</td>.<
-00001870: 2f74 723e 0a3c 7472 3e0a 203c 7464 3e3c  /tr>.<tr>. <td><
-00001880: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00001890: 6172 7869 762e 6f72 672f 6162 732f 3132  arxiv.org/abs/12
-000018a0: 3037 2e31 3431 3122 3e4c 6564 7563 2068  07.1411">Leduc h
-000018b0: 6f6c 6427 656d 3c2f 613e 3c2f 7464 3e0a  old'em</a></td>.
-000018c0: 203c 7464 3e3a 7768 6974 655f 6368 6563   <td>:white_chec
-000018d0: 6b5f 6d61 726b 3a3c 2f74 643e 0a20 3c74  k_mark:</td>. <t
-000018e0: 643e 3a77 6869 7465 5f63 6865 636b 5f6d  d>:white_check_m
-000018f0: 6172 6b3a 3c2f 7464 3e0a 3c2f 7472 3e0a  ark:</td>.</tr>.
-00001900: 3c74 723e 0a20 3c74 643e 3c61 2068 7265  <tr>. <td><a hre
-00001910: 663d 2268 7474 7073 3a2f 2f65 6e2e 7769  f="https://en.wi
-00001920: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
-00001930: 2f4a 6170 616e 6573 655f 6d61 686a 6f6e  /Japanese_mahjon
-00001940: 6722 3e4d 6168 6a6f 6e67 3c2f 613e 3c2f  g">Mahjong</a></
-00001950: 7464 3e0a 203c 7464 3e3a 636f 6e73 7472  td>. <td>:constr
-00001960: 7563 7469 6f6e 3a3c 2f74 643e 0a20 3c74  uction:</td>. <t
-00001970: 643e 3a63 6f6e 7374 7275 6374 696f 6e3a  d>:construction:
-00001980: 3c2f 7464 3e0a 3c2f 7472 3e0a 3c74 723e  </td>.</tr>.<tr>
-00001990: 0a20 3c74 643e 3c61 2068 7265 663d 2268  . <td><a href="h
-000019a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000019b0: 6d2f 6b65 6e6a 796f 756e 672f 4d69 6e41  m/kenjyoung/MinA
-000019c0: 7461 7222 3e4d 696e 4174 6172 2f41 7374  tar">MinAtar/Ast
-000019d0: 6572 6978 3c2f 613e 3c2f 7464 3e0a 203c  erix</a></td>. <
-000019e0: 7464 3e3a 7768 6974 655f 6368 6563 6b5f  td>:white_check_
-000019f0: 6d61 726b 3a3c 2f74 643e 0a20 3c74 643e  mark:</td>. <td>
-00001a00: 3a77 6869 7465 5f63 6865 636b 5f6d 6172  :white_check_mar
-00001a10: 6b3a 3c2f 7464 3e0a 3c2f 7472 3e0a 3c74  k:</td>.</tr>.<t
-00001a20: 723e 0a20 3c74 643e 3c61 2068 7265 663d  r>. <td><a href=
-00001a30: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-00001a40: 636f 6d2f 6b65 6e6a 796f 756e 672f 4d69  com/kenjyoung/Mi
-00001a50: 6e41 7461 7222 3e4d 696e 4174 6172 2f42  nAtar">MinAtar/B
-00001a60: 7265 616b 6f75 743c 2f61 3e3c 2f74 643e  reakout</a></td>
-00001a70: 0a20 3c74 643e 3a77 6869 7465 5f63 6865  . <td>:white_che
-00001a80: 636b 5f6d 6172 6b3a 3c2f 7464 3e0a 203c  ck_mark:</td>. <
-00001a90: 7464 3e3a 7768 6974 655f 6368 6563 6b5f  td>:white_check_
-00001aa0: 6d61 726b 3a3c 2f74 643e 0a3c 2f74 723e  mark:</td>.</tr>
-00001ab0: 0a3c 7472 3e0a 203c 7464 3e3c 6120 6872  .<tr>. <td><a hr
-00001ac0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-00001ad0: 7562 2e63 6f6d 2f6b 656e 6a79 6f75 6e67  ub.com/kenjyoung
-00001ae0: 2f4d 696e 4174 6172 223e 4d69 6e41 7461  /MinAtar">MinAta
-00001af0: 722f 4672 6565 7761 793c 2f61 3e3c 2f74  r/Freeway</a></t
-00001b00: 643e 0a20 3c74 643e 3a77 6869 7465 5f63  d>. <td>:white_c
-00001b10: 6865 636b 5f6d 6172 6b3a 3c2f 7464 3e0a  heck_mark:</td>.
-00001b20: 203c 7464 3e3a 7768 6974 655f 6368 6563   <td>:white_chec
-00001b30: 6b5f 6d61 726b 3a3c 2f74 643e 0a3c 2f74  k_mark:</td>.</t
-00001b40: 723e 0a3c 7472 3e0a 203c 7464 3e3c 6120  r>.<tr>. <td><a 
-00001b50: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00001b60: 7468 7562 2e63 6f6d 2f6b 656e 6a79 6f75  thub.com/kenjyou
-00001b70: 6e67 2f4d 696e 4174 6172 223e 4d69 6e41  ng/MinAtar">MinA
-00001b80: 7461 722f 5365 6171 7565 7374 3c2f 613e  tar/Seaquest</a>
-00001b90: 3c2f 7464 3e0a 203c 7464 3e3a 7768 6974  </td>. <td>:whit
-00001ba0: 655f 6368 6563 6b5f 6d61 726b 3a3c 2f74  e_check_mark:</t
-00001bb0: 643e 0a20 3c74 643e 3a77 6869 7465 5f63  d>. <td>:white_c
-00001bc0: 6865 636b 5f6d 6172 6b3a 3c2f 7464 3e0a  heck_mark:</td>.
-00001bd0: 3c2f 7472 3e0a 3c74 723e 0a20 3c74 643e  </tr>.<tr>. <td>
-00001be0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00001bf0: 2f67 6974 6875 622e 636f 6d2f 6b65 6e6a  /github.com/kenj
-00001c00: 796f 756e 672f 4d69 6e41 7461 7222 3e4d  young/MinAtar">M
-00001c10: 696e 4174 6172 2f53 7061 6365 496e 7661  inAtar/SpaceInva
-00001c20: 6465 7273 3c2f 613e 3c2f 7464 3e0a 203c  ders</a></td>. <
-00001c30: 7464 3e3a 7768 6974 655f 6368 6563 6b5f  td>:white_check_
-00001c40: 6d61 726b 3a3c 2f74 643e 0a20 3c74 643e  mark:</td>. <td>
-00001c50: 3a77 6869 7465 5f63 6865 636b 5f6d 6172  :white_check_mar
-00001c60: 6b3a 3c2f 7464 3e0a 3c2f 7472 3e0a 3c74  k:</td>.</tr>.<t
-00001c70: 723e 0a20 3c74 643e 3c61 2068 7265 663d  r>. <td><a href=
-00001c80: 2268 7474 7073 3a2f 2f65 6e2e 7769 6b69  "https://en.wiki
-00001c90: 7065 6469 612e 6f72 672f 7769 6b69 2f52  pedia.org/wiki/R
-00001ca0: 6576 6572 7369 223e 4f74 6865 6c6c 6f3c  eversi">Othello<
-00001cb0: 2f61 3e3c 2f74 643e 0a20 3c74 643e 3a77  /a></td>. <td>:w
-00001cc0: 6869 7465 5f63 6865 636b 5f6d 6172 6b3a  hite_check_mark:
-00001cd0: 3c2f 7464 3e0a 203c 7464 3e3a 7768 6974  </td>. <td>:whit
-00001ce0: 655f 6368 6563 6b5f 6d61 726b 3a3c 2f74  e_check_mark:</t
-00001cf0: 643e 0a3c 2f74 723e 0a3c 7472 3e0a 203c  d>.</tr>.<tr>. <
-00001d00: 7464 3e3c 6120 6872 6566 3d22 6874 7470  td><a href="http
-00001d10: 733a 2f2f 656e 2e77 696b 6970 6564 6961  s://en.wikipedia
-00001d20: 2e6f 7267 2f77 696b 692f 5368 6f67 6922  .org/wiki/Shogi"
-00001d30: 3e53 686f 6769 3c2f 613e 3c2f 7464 3e0a  >Shogi</a></td>.
-00001d40: 203c 7464 3e3a 7768 6974 655f 6368 6563   <td>:white_chec
-00001d50: 6b5f 6d61 726b 3a3c 2f74 643e 0a20 3c74  k_mark:</td>. <t
-00001d60: 643e 3a77 6869 7465 5f63 6865 636b 5f6d  d>:white_check_m
-00001d70: 6172 6b3a 3c2f 7464 3e0a 3c2f 7472 3e0a  ark:</td>.</tr>.
-00001d80: 3c74 723e 0a20 3c74 643e 3c61 2068 7265  <tr>. <td><a hre
-00001d90: 663d 2268 7474 7073 3a2f 2f73 7567 6f72  f="https://sugor
-00001da0: 6f6b 7579 612e 6a70 2f70 2f73 757a 756d  okuya.jp/p/suzum
-00001db0: 652d 6a6f 6e67 223e 5370 6172 726f 7720  e-jong">Sparrow 
-00001dc0: 4d61 686a 6f6e 673c 2f61 3e3c 2f74 643e  Mahjong</a></td>
-00001dd0: 0a20 3c74 643e 3a77 6869 7465 5f63 6865  . <td>:white_che
-00001de0: 636b 5f6d 6172 6b3a 3c2f 7464 3e0a 203c  ck_mark:</td>. <
-00001df0: 7464 3e3a 7768 6974 655f 6368 6563 6b5f  td>:white_check_
-00001e00: 6d61 726b 3a3c 2f74 643e 0a3c 2f74 723e  mark:</td>.</tr>
-00001e10: 0a3c 7472 3e0a 203c 7464 3e3c 6120 6872  .<tr>. <td><a hr
-00001e20: 6566 3d22 6874 7470 733a 2f2f 656e 2e77  ef="https://en.w
-00001e30: 696b 6970 6564 6961 2e6f 7267 2f77 696b  ikipedia.org/wik
-00001e40: 692f 5469 632d 7461 632d 746f 6522 3e54  i/Tic-tac-toe">T
-00001e50: 6963 2d74 6163 2d74 6f65 3c2f 613e 3c2f  ic-tac-toe</a></
-00001e60: 7464 3e0a 203c 7464 3e3a 7768 6974 655f  td>. <td>:white_
-00001e70: 6368 6563 6b5f 6d61 726b 3a3c 2f74 643e  check_mark:</td>
-00001e80: 0a20 3c74 643e 3a77 6869 7465 5f63 6865  . <td>:white_che
-00001e90: 636b 5f6d 6172 6b3a 3c2f 7464 3e0a 3c2f  ck_mark:</td>.</
-00001ea0: 7472 3e0a 3c2f 7461 626c 653e 0a3c 2f64  tr>.</table>.</d
-00001eb0: 6976 3e0a 0a23 2320 5365 6520 616c 736f  iv>..## See also
-00001ec0: 0a0a 5067 7820 6973 2069 6e74 656e 6465  ..Pgx is intende
-00001ed0: 6420 746f 2063 6f6d 706c 656d 656e 7420  d to complement 
-00001ee0: 7468 6573 6520 2a2a 4a41 582d 6e61 7469  these **JAX-nati
-00001ef0: 7665 2065 6e76 6972 6f6e 6d65 6e74 732a  ve environments*
-00001f00: 2a20 7769 7468 2028 636c 6173 7369 6329  * with (classic)
-00001f10: 2062 6f61 7264 2067 616d 6520 7375 6974   board game suit
-00001f20: 733a 0a0a 2d20 5b52 6f62 6572 7454 4c61  s:..- [RobertTLa
-00001f30: 6e67 652f 6779 6d6e 6178 5d28 6874 7470  nge/gymnax](http
-00001f40: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f52  s://github.com/R
-00001f50: 6f62 6572 7454 4c61 6e67 652f 6779 6d6e  obertTLange/gymn
-00001f60: 6178 293a 2043 6c61 7373 6963 2063 6f6e  ax): Classic con
-00001f70: 7472 6f6c 2c20 6273 7569 7465 2c20 6574  trol, bsuite, et
-00001f80: 632e 0a2d 205b 676f 6f67 6c65 2f62 7261  c..- [google/bra
-00001f90: 785d 2868 7474 7073 3a2f 2f67 6974 6875  x](https://githu
-00001fa0: 622e 636f 6d2f 676f 6f67 6c65 2f62 7261  b.com/google/bra
-00001fb0: 7829 3a20 5269 6769 6462 6f64 7920 7068  x): Rigidbody ph
-00001fc0: 7973 6963 7320 7369 6d75 6c61 7469 6f6e  ysics simulation
-00001fd0: 0a2d 205b 696e 7374 6164 6565 7061 692f  .- [instadeepai/
-00001fe0: 6a75 6d61 6e6a 695d 2868 7474 7073 3a2f  jumanji](https:/
-00001ff0: 2f67 6974 6875 622e 636f 6d2f 696e 7374  /github.com/inst
-00002000: 6164 6565 7061 692f 6a75 6d61 6e6a 6929  adeepai/jumanji)
-00002010: 3a20 496e 6475 7374 7279 2d64 7269 7665  : Industry-drive
-00002020: 6e20 656e 7669 726f 6e6d 656e 7473 2028  n environments (
-00002030: 652e 672e 2c20 5472 6176 656c 6c69 6e67  e.g., Travelling
-00002040: 2053 616c 6573 6d61 6e20 5072 6f62 6c65   Salesman Proble
-00002050: 6d29 0a0a 436f 6d62 696e 696e 6720 5067  m)..Combining Pg
-00002060: 7820 7769 7468 2074 6865 7365 202a 2a4a  x with these **J
-00002070: 4158 2d6e 6174 6976 6520 616c 676f 7269  AX-native algori
-00002080: 7468 6d73 2f69 6d70 6c65 6d65 6e74 6174  thms/implementat
-00002090: 696f 6e73 2a2a 206d 6967 6874 2062 6520  ions** might be 
-000020a0: 616e 2069 6e74 6572 6573 7469 6e67 2064  an interesting d
-000020b0: 6972 6563 7469 6f6e 3a0a 0a2d 205b 416e  irection:..- [An
-000020c0: 616b 696e 2066 7261 6d65 776f 726b 5d28  akin framework](
-000020d0: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
-000020e0: 672f 6162 732f 3231 3034 2e30 3632 3732  g/abs/2104.06272
-000020f0: 293a 2048 6967 686c 7920 6566 6669 6369  ): Highly effici
-00002100: 656e 7420 524c 2066 7261 6d65 776f 726b  ent RL framework
-00002110: 2074 6861 7420 776f 726b 7320 7769 7468   that works with
-00002120: 204a 4158 2d6e 6174 6976 6520 656e 7669   JAX-native envi
-00002130: 726f 6e6d 656e 7473 206f 6e20 5450 5573  ronments on TPUs
-00002140: 0a2d 205b 6465 6570 6d69 6e64 2f6d 6374  .- [deepmind/mct
-00002150: 785d 2868 7474 7073 3a2f 2f67 6974 6875  x](https://githu
-00002160: 622e 636f 6d2f 6465 6570 6d69 6e64 2f6d  b.com/deepmind/m
-00002170: 6374 7829 3a20 4a41 582d 6e61 7469 7665  ctx): JAX-native
-00002180: 204d 4354 5320 696d 706c 656d 656e 7461   MCTS implementa
-00002190: 7469 6f6e 732c 2069 6e63 6c75 6469 6e67  tions, including
-000021a0: 2041 6c70 6861 5a65 726f 2061 6e64 204d   AlphaZero and M
-000021b0: 755a 6572 6f0a 2d20 5b64 6565 706d 696e  uZero.- [deepmin
-000021c0: 642f 726c 6178 5d28 6874 7470 733a 2f2f  d/rlax](https://
-000021d0: 6769 7468 7562 2e63 6f6d 2f64 6565 706d  github.com/deepm
-000021e0: 696e 642f 726c 6178 293a 204a 4158 2d6e  ind/rlax): JAX-n
-000021f0: 6174 6976 6520 524c 2063 6f6d 706f 6e65  ative RL compone
-00002200: 6e74 730a 2d20 5b67 6f6f 676c 652f 6576  nts.- [google/ev
-00002210: 6f6a 6178 5d28 6874 7470 733a 2f2f 6769  ojax](https://gi
-00002220: 7468 7562 2e63 6f6d 2f67 6f6f 676c 652f  thub.com/google/
-00002230: 6576 6f6a 6178 293a 2048 6172 6477 6172  evojax): Hardwar
-00002240: 652d 4163 6365 6c65 7261 7465 6420 6e65  e-Accelerated ne
-00002250: 7572 6f65 766f 6c75 7469 6f6e 0a2d 205b  uroevolution.- [
-00002260: 526f 6265 7274 544c 616e 6765 2f65 766f  RobertTLange/evo
-00002270: 7361 785d 2868 7474 7073 3a2f 2f67 6974  sax](https://git
-00002280: 6875 622e 636f 6d2f 526f 6265 7274 544c  hub.com/RobertTL
-00002290: 616e 6765 2f65 766f 7361 7829 3a20 4a41  ange/evosax): JA
-000022a0: 582d 6e61 7469 7665 2065 766f 6c75 7469  X-native evoluti
-000022b0: 6f6e 2073 7472 6174 6567 7920 2845 5329  on strategy (ES)
-000022c0: 2069 6d70 6c65 6d65 6e74 6174 696f 6e73   implementations
-000022d0: 0a2d 205b 6164 6170 7469 7665 2d69 6e74  .- [adaptive-int
-000022e0: 656c 6c69 6765 6e74 2d72 6f62 6f74 6963  elligent-robotic
-000022f0: 732f 5144 6178 5d28 6874 7470 733a 2f2f  s/QDax](https://
-00002300: 6769 7468 7562 2e63 6f6d 2f61 6461 7074  github.com/adapt
-00002310: 6976 652d 696e 7465 6c6c 6967 656e 742d  ive-intelligent-
-00002320: 726f 626f 7469 6373 2f51 4461 7829 3a20  robotics/QDax): 
-00002330: 4a41 582d 6e61 7469 7665 2051 7561 6c69  JAX-native Quali
-00002340: 7479 2d44 6976 6572 7369 7479 2028 5144  ty-Diversity (QD
-00002350: 2920 616c 676f 7269 7468 6d73 0a0a 0a23  ) algorithms...#
-00002360: 2320 4c49 4345 4e53 450a 0a41 7061 6368  # LICENSE..Apach
-00002370: 652d 322e 300a                           e-2.0.
+000005b0: 2a2a 2c20 2a2a 4368 6573 732a 2a2c 202a  **, **Chess**, *
+000005c0: 2a53 686f 6769 2a2a 2c20 616e 6420 2a2a  *Shogi**, and **
+000005d0: 476f 2a2a 0a2d 202a 2a42 6561 7574 6966  Go**.- **Beautif
+000005e0: 756c 2076 6973 7561 6c69 7a61 7469 6f6e  ul visualization
+000005f0: 2a2a 2069 6e20 5356 4720 666f 726d 6174  ** in SVG format
+00000600: 0a0a 0a23 2320 496e 7374 616c 6c0a 0a60  ...## Install..`
+00000610: 6060 7368 0a70 6970 2069 6e73 7461 6c6c  ``sh.pip install
+00000620: 2070 6778 0a60 6060 0a0a 2323 2055 7361   pgx.```..## Usa
+00000630: 6765 0a3c 6120 6872 6566 3d22 6874 7470  ge.<a href="http
+00000640: 733a 2f2f 636f 6c61 622e 7265 7365 6172  s://colab.resear
+00000650: 6368 2e67 6f6f 676c 652e 636f 6d2f 6769  ch.google.com/gi
+00000660: 7468 7562 2f73 6f74 6574 7375 6b2f 7067  thub/sotetsuk/pg
+00000670: 782f 626c 6f62 2f6d 6169 6e2f 636f 6c61  x/blob/main/cola
+00000680: 622f 7067 785f 6865 6c6c 6f5f 776f 726c  b/pgx_hello_worl
+00000690: 642e 6970 796e 6222 3e3c 696d 6720 7372  d.ipynb"><img sr
+000006a0: 633d 2268 7474 7073 3a2f 2f63 6f6c 6162  c="https://colab
+000006b0: 2e72 6573 6561 7263 682e 676f 6f67 6c65  .research.google
+000006c0: 2e63 6f6d 2f61 7373 6574 732f 636f 6c61  .com/assets/cola
+000006d0: 622d 6261 6467 652e 7376 6722 2061 6c74  b-badge.svg" alt
+000006e0: 3d22 4f70 656e 2049 6e20 436f 6c61 6222  ="Open In Colab"
+000006f0: 2f3e 3c2f 613e 0a0a 6060 6070 790a 696d  /></a>..```py.im
+00000700: 706f 7274 206a 6178 0a69 6d70 6f72 7420  port jax.import 
+00000710: 7067 780a 0a65 6e76 203d 2070 6778 2e6d  pgx..env = pgx.m
+00000720: 616b 6528 2267 6f2d 3139 7831 3922 290a  ake("go-19x19").
+00000730: 696e 6974 203d 206a 6178 2e6a 6974 286a  init = jax.jit(j
+00000740: 6178 2e76 6d61 7028 656e 762e 696e 6974  ax.vmap(env.init
+00000750: 2929 2020 2320 7665 6374 6f72 697a 6520  ))  # vectorize 
+00000760: 616e 6420 4a49 542d 636f 6d70 696c 650a  and JIT-compile.
+00000770: 7374 6570 203d 206a 6178 2e6a 6974 286a  step = jax.jit(j
+00000780: 6178 2e76 6d61 7028 656e 762e 7374 6570  ax.vmap(env.step
+00000790: 2929 0a0a 6261 7463 685f 7369 7a65 203d  ))..batch_size =
+000007a0: 2031 3032 340a 6b65 7973 203d 206a 6178   1024.keys = jax
+000007b0: 2e72 616e 646f 6d2e 7370 6c69 7428 6a61  .random.split(ja
+000007c0: 782e 7261 6e64 6f6d 2e50 524e 474b 6579  x.random.PRNGKey
+000007d0: 2834 3229 2c20 6261 7463 685f 7369 7a65  (42), batch_size
+000007e0: 290a 7374 6174 6520 3d20 696e 6974 286b  ).state = init(k
+000007f0: 6579 7329 2020 2320 7665 6374 6f72 697a  eys)  # vectoriz
+00000800: 6564 2073 7461 7465 730a 7768 696c 6520  ed states.while 
+00000810: 6e6f 7420 7374 6174 652e 7465 726d 696e  not state.termin
+00000820: 6174 6564 2e61 6c6c 2829 3a0a 2020 2020  ated.all():.    
+00000830: 6163 7469 6f6e 203d 206d 6f64 656c 2873  action = model(s
+00000840: 7461 7465 2e63 7572 7265 6e74 5f70 6c61  tate.current_pla
+00000850: 7965 722c 2073 7461 7465 2e6f 6273 6572  yer, state.obser
+00000860: 7661 7469 6f6e 2c20 7374 6174 652e 6c65  vation, state.le
+00000870: 6761 6c5f 6163 7469 6f6e 5f6d 6173 6b29  gal_action_mask)
+00000880: 0a20 2020 2073 7461 7465 203d 2073 7465  .    state = ste
+00000890: 7028 7374 6174 652c 2061 6374 696f 6e29  p(state, action)
+000008a0: 2020 2320 7374 6174 652e 7265 7761 7264    # state.reward
+000008b0: 2028 322c 290a 6060 600a 0a3c 212d 2d2d   (2,).```..<!---
+000008c0: 0a23 2323 204c 696d 6974 6174 696f 6e73  .### Limitations
+000008d0: 2028 666f 7220 7468 6520 7369 6d70 6c69   (for the simpli
+000008e0: 6369 7479 290a 2a20 446f 6573 202a 2a4e  city).* Does **N
+000008f0: 4f54 2a2a 2073 7570 706f 7274 2061 6765  OT** support age
+00000900: 6e74 2064 6561 7468 2061 6e64 2063 7265  nt death and cre
+00000910: 6174 696f 6e2c 2077 6869 6368 2064 796e  ation, which dyn
+00000920: 6d69 6361 6c6c 7920 6368 616e 6765 7320  mically changes 
+00000930: 7468 6520 6172 7261 7920 7369 7a65 2e20  the array size. 
+00000940: 4974 2064 6f65 7320 6e6f 7420 7765 6c6c  It does not well
+00000950: 2073 7569 7420 746f 2047 5055 2d61 6363   suit to GPU-acc
+00000960: 656c 6572 6174 6564 2063 6f6d 7075 7461  elerated computa
+00000970: 7469 6f6e 2e0a 2a20 446f 6573 202a 2a4e  tion..* Does **N
+00000980: 4f54 2a2a 2073 7570 706f 7274 2043 6861  OT** support Cha
+00000990: 6e63 6520 706c 6179 6572 2028 4e61 7475  nce player (Natu
+000009a0: 7265 2070 6c61 7965 7229 2077 6974 6820  re player) with 
+000009b0: 6163 7469 6f6e 2073 656c 6563 7469 6f6e  action selection
+000009c0: 2e0a 2a20 446f 6573 202a 2a4e 4f54 2a2a  ..* Does **NOT**
+000009d0: 2073 7570 706f 7274 204f 7065 6e41 4920   support OpenAI 
+000009e0: 4779 6d20 4150 492e 0a20 2020 202a 204f  Gym API..    * O
+000009f0: 7065 6e41 4920 4779 6d20 6973 2066 6f72  penAI Gym is for
+00000a00: 2073 696e 676c 652d 6167 656e 7420 656e   single-agent en
+00000a10: 7669 726f 6e6d 656e 742e 204d 6f73 7420  vironment. Most 
+00000a20: 6f66 2050 6778 2065 6e76 6972 6f6e 6d65  of Pgx environme
+00000a30: 6e74 7320 6172 6520 6d75 6c74 692d 706c  nts are multi-pl
+00000a40: 6179 6572 2067 616d 6573 2e20 4a75 7374  ayer games. Just
+00000a50: 2064 6566 696e 696e 6720 6f70 706f 6e65   defining oppone
+00000a60: 6e74 7320 6973 206e 6f74 2065 6e6f 7567  nts is not enoug
+00000a70: 6820 666f 7220 636f 6e76 6572 7469 6e67  h for converting
+00000a80: 206d 756c 7469 2d61 6765 6e74 2065 6e76   multi-agent env
+00000a90: 6972 6f6e 656d 6e74 7320 746f 204f 7065  ironemnts to Ope
+00000aa0: 6e41 4920 4779 6d20 656e 7669 726f 6e6d  nAI Gym environm
+00000ab0: 656e 742e 2045 2e67 2e2c 2069 6e20 7468  ent. E.g., in th
+00000ac0: 6520 6761 6d65 206f 6620 676f 2c20 7468  e game of go, th
+00000ad0: 6520 6e65 7874 2073 7461 7465 2073 2720  e next state s' 
+00000ae0: 6973 2064 6566 696e 6564 2061 7320 7468  is defined as th
+00000af0: 6520 7374 6174 6520 6a75 7374 2061 6674  e state just aft
+00000b00: 6572 2070 6c61 6369 6e67 2061 2073 746f  er placing a sto
+00000b10: 6e65 2069 6e20 416c 6861 476f 2070 6170  ne in AlhaGo pap
+00000b20: 6572 2e20 486f 7765 7665 722c 2073 2720  er. However, s' 
+00000b30: 6265 636f 6d65 7320 7468 6520 7374 6174  becomes the stat
+00000b40: 6520 6166 7465 7220 7468 6520 6f70 706f  e after the oppo
+00000b50: 6e65 6e74 7327 2070 6c61 792e 2054 6869  nents' play. Thi
+00000b60: 7320 6368 616e 6765 7320 7468 6520 6465  s changes the de
+00000b70: 6669 6e69 7469 6f6e 206f 6620 5628 7327  finition of V(s'
+00000b80: 292e 0a2a 2044 6f65 7320 2a2a 4e4f 542a  )..* Does **NOT*
+00000b90: 2a20 7375 7070 6f72 7420 5065 7474 696e  * support Pettin
+00000ba0: 675a 6f6f 2041 5049 2e0a 2020 2020 2a20  gZoo API..    * 
+00000bb0: 5065 7474 696e 675a 6f6f 2069 7320 2a47  PettingZoo is *G
+00000bc0: 796d 2066 6f72 206d 756c 7469 2d61 6765  ym for multi-age
+00000bd0: 6e74 2052 4c2a 2e20 4173 2066 6172 2061  nt RL*. As far a
+00000be0: 7320 7765 206b 6e6f 772c 2050 6574 7469  s we know, Petti
+00000bf0: 6e67 5a6f 6f20 646f 6573 206e 6f74 2073  ngZoo does not s
+00000c00: 7570 706f 7274 2076 6563 746f 7269 7a65  upport vectorize
+00000c10: 6420 656e 7669 726f 6e6d 656e 7473 2028  d environments (
+00000c20: 6c69 6b65 2056 6563 746f 7245 6e76 2069  like VectorEnv i
+00000c30: 6e20 4f70 656e 4149 2047 796d 292e 2041  n OpenAI Gym). A
+00000c40: 7320 5067 7827 7320 6d61 696e 2066 6561  s Pgx's main fea
+00000c50: 7475 7265 2069 7320 6869 6768 6c79 2076  ture is highly v
+00000c60: 6563 746f 7269 7a65 6420 656e 7669 726f  ectorized enviro
+00000c70: 6e6d 656e 7420 7669 6120 4750 552f 5450  nment via GPU/TP
+00000c80: 5520 7375 7070 6f72 742c 2057 6520 646f  U support, We do
+00000c90: 206e 6f74 2063 7572 7265 6e74 6c79 2073   not currently s
+00000ca0: 7570 706f 7274 2050 6574 7469 6e67 5a6f  upport PettingZo
+00000cb0: 6f20 4150 492e 200a 0a23 2323 2060 736b  o API. ..### `sk
+00000cc0: 6970 5f63 6861 6e63 6560 0a2a 2057 6520  ip_chance`.* We 
+00000cd0: 7072 6570 6172 6520 736b 6970 5f63 6861  prepare skip_cha
+00000ce0: 6e63 653d 5472 7565 206f 7074 696f 6e20  nce=True option 
+00000cf0: 666f 7220 736f 6d65 2065 6e76 6972 6f6e  for some environ
+00000d00: 6d65 6e74 732e 2054 6869 7320 6d61 6b65  ments. This make
+00000d10: 7320 6974 2070 6f73 7369 626c 6520 746f  s it possible to
+00000d20: 2063 6f6e 7369 6465 7220 7661 6c75 6520   consider value 
+00000d30: 6675 6e63 7469 6f6e 2066 6f72 2022 706f  function for "po
+00000d40: 7374 2d64 6563 6973 696f 6e20 7374 6174  st-decision stat
+00000d50: 6573 2220 2853 6565 2041 6c67 6f52 4c20  es" (See AlgoRL 
+00000d60: 626f 6f6b 292e 2048 6f77 6576 6572 2c20  book). However, 
+00000d70: 7765 2064 6f20 6e6f 7420 616c 6c6f 7720  we do not allow 
+00000d80: 6368 616e 6365 2061 6765 6e74 2074 6f20  chance agent to 
+00000d90: 6368 6f6f 7365 2061 6374 696f 6e20 6c69  choose action li
+00000da0: 6b65 204f 7065 6e53 7069 656c 2e20 5468  ke OpenSpiel. Th
+00000db0: 6973 2069 7320 6265 6361 7573 6520 7468  is is because th
+00000dc0: 6520 6163 7469 6f6e 2073 7061 6365 206f  e action space o
+00000dd0: 6620 6368 616e 6365 2061 6765 6e74 2061  f chance agent a
+00000de0: 6e64 2075 7375 616c 2061 6765 6e74 2061  nd usual agent a
+00000df0: 7265 2064 6966 6665 7265 6e74 2e20 5468  re different. Th
+00000e00: 7573 2c20 7768 656e 2074 6865 2063 6861  us, when the cha
+00000e10: 6e63 6520 706c 6179 6572 2069 7320 6368  nce player is ch
+00000e20: 6f73 656e 2028 6063 7572 7265 6e74 5f70  osen (`current_p
+00000e30: 6c61 7965 723d 2d31 6029 2c20 6061 6374  layer=-1`), `act
+00000e40: 696f 6e3d 2d31 6020 6d75 7374 2062 6520  ion=-1` must be 
+00000e50: 7265 7475 726e 6564 2074 6f20 7374 6570  returned to step
+00000e60: 2066 756e 6374 696f 6e2e 2055 7365 2060   function. Use `
+00000e70: 7368 7566 666c 6560 2074 6f20 6d61 6b65  shuffle` to make
+00000e80: 2060 7374 6570 6020 7374 6f63 6861 7374   `step` stochast
+00000e90: 6963 2e0a 0a23 2323 2074 7275 6e63 6174  ic...### truncat
+00000ea0: 6174 696f 6e20 616e 6420 6175 746f 5f72  ation and auto_r
+00000eb0: 6573 6574 0a2a 2073 7570 706f 7274 6564  eset.* supported
+00000ec0: 2062 7920 606d 616b 6528 656e 765f 6964   by `make(env_id
+00000ed0: 3d22 2e2e 2e22 2c20 6175 746f 5f72 6573  ="...", auto_res
+00000ee0: 6574 3d54 7275 652c 206d 6178 5f65 7069  et=True, max_epi
+00000ef0: 736f 6465 5f6c 656e 6774 683d 3634 2960  sode_length=64)`
+00000f00: 0a2a 2060 6175 746f 5f72 6573 6574 6020  .* `auto_reset` 
+00000f10: 7769 6c6c 2072 6570 6c61 6365 2074 6865  will replace the
+00000f20: 2074 6572 6d69 6e61 6c20 7374 6174 6520   terminal state 
+00000f30: 6279 2069 6e69 7469 616c 2073 7461 7465  by initial state
+00000f40: 2028 6275 7420 6069 735f 7465 726d 696e   (but `is_termin
+00000f50: 616c 3d54 7275 6560 2069 7320 7365 7429  al=True` is set)
+00000f60: 0a2a 2060 6973 5f74 7275 6e63 6174 6564  .* `is_truncated
+00000f70: 3d54 7275 6560 2069 7320 616c 736f 2073  =True` is also s
+00000f80: 6574 2074 6f20 7374 6174 650a 2d2d 2d3e  et to state.--->
+00000f90: 0a0a 2323 2053 7570 706f 7274 6564 2067  ..## Supported g
+00000fa0: 616d 6573 2061 6e64 2072 6f61 6420 6d61  ames and road ma
+00000fb0: 700a 0a3e 203a 7761 726e 696e 673a 2050  p..> :warning: P
+00000fc0: 6778 2069 7320 6375 7272 656e 746c 7920  gx is currently 
+00000fd0: 696e 2074 6865 2062 6574 6120 7665 7273  in the beta vers
+00000fe0: 696f 6e2e 2054 6865 7265 666f 7265 2c20  ion. Therefore, 
+00000ff0: 4150 4920 6973 2073 7562 6a65 6374 2074  API is subject t
+00001000: 6f20 6368 616e 6765 2077 6974 686f 7574  o change without
+00001010: 206e 6f74 6963 652e 2057 6520 6169 6d20   notice. We aim 
+00001020: 746f 2072 656c 6561 7365 2076 312e 302e  to release v1.0.
+00001030: 3020 696e 2041 7072 696c 2032 3032 332e  0 in April 2023.
+00001040: 204f 7069 6e69 6f6e 7320 616e 6420 636f   Opinions and co
+00001050: 6d6d 656e 7473 2061 7265 206d 6f72 6520  mments are more 
+00001060: 7468 616e 2077 656c 636f 6d65 210a 0a55  than welcome!..U
+00001070: 7365 2060 7067 782e 6176 6169 6c61 626c  se `pgx.availabl
+00001080: 655f 6761 6d65 7328 2960 2074 6f20 7365  e_games()` to se
+00001090: 6520 7468 6520 6c69 7374 206f 6620 6375  e the list of cu
+000010a0: 7272 656e 746c 7920 6176 6169 6c61 626c  rrently availabl
+000010b0: 6520 6761 6d65 732e 0a0a 3c64 6976 2061  e games...<div a
+000010c0: 6c69 676e 3d22 6365 6e74 6572 223e 0a3c  lign="center">.<
+000010d0: 696d 6720 7372 633d 2266 6967 2f73 7667  img src="fig/svg
+000010e0: 732f 3230 3438 5f64 6172 6b2e 706e 6723  s/2048_dark.png#
+000010f0: 6768 2d64 6172 6b2d 6d6f 6465 2d6f 6e6c  gh-dark-mode-onl
+00001100: 7922 2068 6569 6768 743d 2231 3230 7078  y" height="120px
+00001110: 223e 0a3c 696d 6720 7372 633d 2266 6967  ">.<img src="fig
+00001120: 2f73 7667 732f 6261 636b 6761 6d6d 6f6e  /svgs/backgammon
+00001130: 5f64 6172 6b2e 706e 6723 6768 2d64 6172  _dark.png#gh-dar
+00001140: 6b2d 6d6f 6465 2d6f 6e6c 7922 2068 6569  k-mode-only" hei
+00001150: 6768 743d 2231 3230 7078 223e 0a3c 696d  ght="120px">.<im
+00001160: 6720 7372 633d 2266 6967 2f73 7667 732f  g src="fig/svgs/
+00001170: 676f 2d39 7839 5f64 6172 6b2e 706e 6723  go-9x9_dark.png#
+00001180: 6768 2d64 6172 6b2d 6d6f 6465 2d6f 6e6c  gh-dark-mode-onl
+00001190: 7922 2068 6569 6768 743d 2231 3230 7078  y" height="120px
+000011a0: 223e 0a3c 696d 6720 7372 633d 2266 6967  ">.<img src="fig
+000011b0: 2f73 7667 732f 6b75 686e 5f70 6f6b 6572  /svgs/kuhn_poker
+000011c0: 5f64 6172 6b2e 706e 6723 6768 2d64 6172  _dark.png#gh-dar
+000011d0: 6b2d 6d6f 6465 2d6f 6e6c 7922 2068 6569  k-mode-only" hei
+000011e0: 6768 743d 2231 3230 7078 223e 0a3c 696d  ght="120px">.<im
+000011f0: 6720 7372 633d 2266 6967 2f73 7667 732f  g src="fig/svgs/
+00001200: 7368 6f67 695f 6461 726b 2e70 6e67 2367  shogi_dark.png#g
+00001210: 682d 6461 726b 2d6d 6f64 652d 6f6e 6c79  h-dark-mode-only
+00001220: 2220 6865 6967 6874 3d22 3132 3070 7822  " height="120px"
+00001230: 3e0a 3c2f 6469 763e 0a0a 3c64 6976 2061  >.</div>..<div a
+00001240: 6c69 676e 3d22 6365 6e74 6572 223e 0a3c  lign="center">.<
+00001250: 696d 6720 7372 633d 2266 6967 2f73 7667  img src="fig/svg
+00001260: 732f 3230 3438 5f6c 6967 6874 2e70 6e67  s/2048_light.png
+00001270: 2367 682d 6c69 6768 742d 6d6f 6465 2d6f  #gh-light-mode-o
+00001280: 6e6c 7922 2068 6569 6768 743d 2231 3230  nly" height="120
+00001290: 7078 223e 0a3c 696d 6720 7372 633d 2266  px">.<img src="f
+000012a0: 6967 2f73 7667 732f 6261 636b 6761 6d6d  ig/svgs/backgamm
+000012b0: 6f6e 5f6c 6967 6874 2e70 6e67 2367 682d  on_light.png#gh-
+000012c0: 6c69 6768 742d 6d6f 6465 2d6f 6e6c 7922  light-mode-only"
+000012d0: 2068 6569 6768 743d 2231 3230 7078 223e   height="120px">
+000012e0: 0a3c 696d 6720 7372 633d 2266 6967 2f73  .<img src="fig/s
+000012f0: 7667 732f 676f 2d39 7839 5f6c 6967 6874  vgs/go-9x9_light
+00001300: 2e70 6e67 2367 682d 6c69 6768 742d 6d6f  .png#gh-light-mo
+00001310: 6465 2d6f 6e6c 7922 2068 6569 6768 743d  de-only" height=
+00001320: 2231 3230 7078 223e 0a3c 696d 6720 7372  "120px">.<img sr
+00001330: 633d 2266 6967 2f73 7667 732f 6b75 686e  c="fig/svgs/kuhn
+00001340: 5f70 6f6b 6572 5f6c 6967 6874 2e70 6e67  _poker_light.png
+00001350: 2367 682d 6c69 6768 742d 6d6f 6465 2d6f  #gh-light-mode-o
+00001360: 6e6c 7922 2068 6569 6768 743d 2231 3230  nly" height="120
+00001370: 7078 223e 0a3c 696d 6720 7372 633d 2266  px">.<img src="f
+00001380: 6967 2f73 7667 732f 7368 6f67 695f 6c69  ig/svgs/shogi_li
+00001390: 6768 742e 706e 6723 6768 2d6c 6967 6874  ght.png#gh-light
+000013a0: 2d6d 6f64 652d 6f6e 6c79 2220 6865 6967  -mode-only" heig
+000013b0: 6874 3d22 3132 3070 7822 3e0a 3c2f 6469  ht="120px">.</di
+000013c0: 763e 0a0a 3c64 6976 2061 6c69 676e 3d22  v>..<div align="
+000013d0: 6365 6e74 6572 223e 0a3c 7461 626c 653e  center">.<table>
+000013e0: 0a3c 7472 3e0a 2020 3c74 683e 4761 6d65  .<tr>.  <th>Game
+000013f0: 3c2f 7468 3e0a 2020 3c74 683e 456e 7669  </th>.  <th>Envi
+00001400: 726f 6e6d 656e 743c 2f74 683e 0a20 203c  ronment</th>.  <
+00001410: 7468 3e56 6973 7561 6c69 7a61 7469 6f6e  th>Visualization
+00001420: 3c2f 7468 3e0a 3c2f 7472 3e0a 3c74 723e  </th>.</tr>.<tr>
+00001430: 0a20 3c74 643e 3c61 2068 7265 663d 2268  . <td><a href="h
+00001440: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
+00001450: 6469 612e 6f72 672f 7769 6b69 2f32 3034  dia.org/wiki/204
+00001460: 385f 2876 6964 656f 5f67 616d 6529 223e  8_(video_game)">
+00001470: 3230 3438 3c2f 613e 3c2f 7464 3e0a 203c  2048</a></td>. <
+00001480: 7464 3e3a 7768 6974 655f 6368 6563 6b5f  td>:white_check_
+00001490: 6d61 726b 3a3c 2f74 643e 0a20 3c74 643e  mark:</td>. <td>
+000014a0: 3a77 6869 7465 5f63 6865 636b 5f6d 6172  :white_check_mar
+000014b0: 6b3a 3c2f 7464 3e0a 3c2f 7472 3e0a 3c74  k:</td>.</tr>.<t
+000014c0: 723e 0a20 3c74 643e 203c 6120 6872 6566  r>. <td> <a href
+000014d0: 3d22 6874 7470 733a 2f2f 656e 2e77 696b  ="https://en.wik
+000014e0: 6970 6564 6961 2e6f 7267 2f77 696b 692f  ipedia.org/wiki/
+000014f0: 4425 4335 2538 4462 7574 7375 5f73 6825  D%C5%8Dbutsu_sh%
+00001500: 4335 2538 4467 6922 3e41 6e69 6d61 6c20  C5%8Dgi">Animal 
+00001510: 5368 6f67 693c 2f61 3e20 3c2f 7464 3e0a  Shogi</a> </td>.
+00001520: 203c 7464 3e3a 7768 6974 655f 6368 6563   <td>:white_chec
+00001530: 6b5f 6d61 726b 3a3c 2f74 643e 0a20 3c74  k_mark:</td>. <t
+00001540: 643e 3a77 6869 7465 5f63 6865 636b 5f6d  d>:white_check_m
+00001550: 6172 6b3a 3c2f 7464 3e0a 3c2f 7472 3e0a  ark:</td>.</tr>.
+00001560: 3c74 723e 0a20 3c74 643e 3c61 2068 7265  <tr>. <td><a hre
+00001570: 663d 2268 7474 7073 3a2f 2f65 6e2e 7769  f="https://en.wi
+00001580: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
+00001590: 2f42 6163 6b67 616d 6d6f 6e22 3e42 6163  /Backgammon">Bac
+000015a0: 6b67 616d 6d6f 6e3c 2f61 3e3c 2f74 643e  kgammon</a></td>
+000015b0: 0a20 3c74 643e 3a77 6869 7465 5f63 6865  . <td>:white_che
+000015c0: 636b 5f6d 6172 6b3a 3c2f 7464 3e0a 203c  ck_mark:</td>. <
+000015d0: 7464 3e3a 7768 6974 655f 6368 6563 6b5f  td>:white_check_
+000015e0: 6d61 726b 3a3c 2f74 643e 0a3c 2f74 723e  mark:</td>.</tr>
+000015f0: 0a3c 7472 3e0a 203c 7464 3e3c 6120 6872  .<tr>. <td><a hr
+00001600: 6566 3d22 6874 7470 733a 2f2f 656e 2e77  ef="https://en.w
+00001610: 696b 6970 6564 6961 2e6f 7267 2f77 696b  ikipedia.org/wik
+00001620: 692f 436f 6e74 7261 6374 5f62 7269 6467  i/Contract_bridg
+00001630: 6522 3e42 7269 6467 6520 4269 6464 696e  e">Bridge Biddin
+00001640: 673c 2f61 3e3c 2f74 643e 0a20 3c74 643e  g</a></td>. <td>
+00001650: 3a63 6f6e 7374 7275 6374 696f 6e3a 3c2f  :construction:</
+00001660: 7464 3e0a 203c 7464 3e3a 7768 6974 655f  td>. <td>:white_
+00001670: 6368 6563 6b5f 6d61 726b 3a3c 2f74 643e  check_mark:</td>
+00001680: 0a3c 2f74 723e 0a3c 7472 3e0a 203c 7464  .</tr>.<tr>. <td
+00001690: 3e3c 6120 6872 6566 3d22 6874 7470 733a  ><a href="https:
+000016a0: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
+000016b0: 7267 2f77 696b 692f 4368 6573 7322 3e43  rg/wiki/Chess">C
+000016c0: 6865 7373 3c2f 613e 3c2f 7464 3e0a 203c  hess</a></td>. <
+000016d0: 7464 3e3a 7768 6974 655f 6368 6563 6b5f  td>:white_check_
+000016e0: 6d61 726b 3a3c 2f74 643e 0a20 3c74 643e  mark:</td>. <td>
+000016f0: 3a77 6869 7465 5f63 6865 636b 5f6d 6172  :white_check_mar
+00001700: 6b3a 3c2f 7464 3e0a 3c2f 7472 3e0a 3c74  k:</td>.</tr>.<t
+00001710: 723e 0a20 3c74 643e 3c61 2068 7265 663d  r>. <td><a href=
+00001720: 2268 7474 7073 3a2f 2f65 6e2e 7769 6b69  "https://en.wiki
+00001730: 7065 6469 612e 6f72 672f 7769 6b69 2f43  pedia.org/wiki/C
+00001740: 6f6e 6e65 6374 5f46 6f75 7222 3e43 6f6e  onnect_Four">Con
+00001750: 6e65 6374 2046 6f75 723c 2f61 3e3c 2f74  nect Four</a></t
+00001760: 643e 0a20 3c74 643e 3a77 6869 7465 5f63  d>. <td>:white_c
+00001770: 6865 636b 5f6d 6172 6b3a 3c2f 7464 3e0a  heck_mark:</td>.
+00001780: 203c 7464 3e3a 7768 6974 655f 6368 6563   <td>:white_chec
+00001790: 6b5f 6d61 726b 3a3c 2f74 643e 0a3c 2f74  k_mark:</td>.</t
+000017a0: 723e 0a3c 7472 3e0a 203c 7464 3e3c 6120  r>.<tr>. <td><a 
+000017b0: 6872 6566 3d22 6874 7470 733a 2f2f 656e  href="https://en
+000017c0: 2e77 696b 6970 6564 6961 2e6f 7267 2f77  .wikipedia.org/w
+000017d0: 696b 692f 476f 5f28 6761 6d65 2922 3e47  iki/Go_(game)">G
+000017e0: 6f3c 2f61 3e3c 2f74 643e 0a20 3c74 643e  o</a></td>. <td>
+000017f0: 3a77 6869 7465 5f63 6865 636b 5f6d 6172  :white_check_mar
+00001800: 6b3a 3c2f 7464 3e0a 203c 7464 3e3a 7768  k:</td>. <td>:wh
+00001810: 6974 655f 6368 6563 6b5f 6d61 726b 3a3c  ite_check_mark:<
+00001820: 2f74 643e 0a3c 2f74 723e 0a3c 7472 3e0a  /td>.</tr>.<tr>.
+00001830: 203c 7464 3e3c 6120 6872 6566 3d22 6874   <td><a href="ht
+00001840: 7470 733a 2f2f 656e 2e77 696b 6970 6564  tps://en.wikiped
+00001850: 6961 2e6f 7267 2f77 696b 692f 4865 785f  ia.org/wiki/Hex_
+00001860: 2862 6f61 7264 5f67 616d 6529 223e 4865  (board_game)">He
+00001870: 783c 2f61 3e3c 2f74 643e 0a20 3c74 643e  x</a></td>. <td>
+00001880: 3a77 6869 7465 5f63 6865 636b 5f6d 6172  :white_check_mar
+00001890: 6b3a 3c2f 7464 3e0a 203c 7464 3e3a 7768  k:</td>. <td>:wh
+000018a0: 6974 655f 6368 6563 6b5f 6d61 726b 3a3c  ite_check_mark:<
+000018b0: 2f74 643e 0a3c 2f74 723e 0a3c 7472 3e0a  /td>.</tr>.<tr>.
+000018c0: 203c 7464 3e3c 6120 6872 6566 3d22 6874   <td><a href="ht
+000018d0: 7470 733a 2f2f 656e 2e77 696b 6970 6564  tps://en.wikiped
+000018e0: 6961 2e6f 7267 2f77 696b 692f 4b75 686e  ia.org/wiki/Kuhn
+000018f0: 5f70 6f6b 6572 223e 4b75 686e 2050 6f6b  _poker">Kuhn Pok
+00001900: 6572 3c2f 613e 3c2f 7464 3e0a 203c 7464  er</a></td>. <td
+00001910: 3e3a 7768 6974 655f 6368 6563 6b5f 6d61  >:white_check_ma
+00001920: 726b 3a3c 2f74 643e 0a20 3c74 643e 3a77  rk:</td>. <td>:w
+00001930: 6869 7465 5f63 6865 636b 5f6d 6172 6b3a  hite_check_mark:
+00001940: 3c2f 7464 3e0a 3c2f 7472 3e0a 3c74 723e  </td>.</tr>.<tr>
+00001950: 0a20 3c74 643e 3c61 2068 7265 663d 2268  . <td><a href="h
+00001960: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
+00001970: 2f61 6273 2f31 3230 372e 3134 3131 223e  /abs/1207.1411">
+00001980: 4c65 6475 6320 686f 6c64 2765 6d3c 2f61  Leduc hold'em</a
+00001990: 3e3c 2f74 643e 0a20 3c74 643e 3a77 6869  ></td>. <td>:whi
+000019a0: 7465 5f63 6865 636b 5f6d 6172 6b3a 3c2f  te_check_mark:</
+000019b0: 7464 3e0a 203c 7464 3e3a 7768 6974 655f  td>. <td>:white_
+000019c0: 6368 6563 6b5f 6d61 726b 3a3c 2f74 643e  check_mark:</td>
+000019d0: 0a3c 2f74 723e 0a3c 7472 3e0a 203c 7464  .</tr>.<tr>. <td
+000019e0: 3e3c 6120 6872 6566 3d22 6874 7470 733a  ><a href="https:
+000019f0: 2f2f 656e 2e77 696b 6970 6564 6961 2e6f  //en.wikipedia.o
+00001a00: 7267 2f77 696b 692f 4a61 7061 6e65 7365  rg/wiki/Japanese
+00001a10: 5f6d 6168 6a6f 6e67 223e 4d61 686a 6f6e  _mahjong">Mahjon
+00001a20: 673c 2f61 3e3c 2f74 643e 0a20 3c74 643e  g</a></td>. <td>
+00001a30: 3a63 6f6e 7374 7275 6374 696f 6e3a 3c2f  :construction:</
+00001a40: 7464 3e0a 203c 7464 3e3a 636f 6e73 7472  td>. <td>:constr
+00001a50: 7563 7469 6f6e 3a3c 2f74 643e 0a3c 2f74  uction:</td>.</t
+00001a60: 723e 0a3c 7472 3e0a 203c 7464 3e3c 6120  r>.<tr>. <td><a 
+00001a70: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
+00001a80: 7468 7562 2e63 6f6d 2f6b 656e 6a79 6f75  thub.com/kenjyou
+00001a90: 6e67 2f4d 696e 4174 6172 223e 4d69 6e41  ng/MinAtar">MinA
+00001aa0: 7461 722f 4173 7465 7269 783c 2f61 3e3c  tar/Asterix</a><
+00001ab0: 2f74 643e 0a20 3c74 643e 3a77 6869 7465  /td>. <td>:white
+00001ac0: 5f63 6865 636b 5f6d 6172 6b3a 3c2f 7464  _check_mark:</td
+00001ad0: 3e0a 203c 7464 3e3a 7768 6974 655f 6368  >. <td>:white_ch
+00001ae0: 6563 6b5f 6d61 726b 3a3c 2f74 643e 0a3c  eck_mark:</td>.<
+00001af0: 2f74 723e 0a3c 7472 3e0a 203c 7464 3e3c  /tr>.<tr>. <td><
+00001b00: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00001b10: 6769 7468 7562 2e63 6f6d 2f6b 656e 6a79  github.com/kenjy
+00001b20: 6f75 6e67 2f4d 696e 4174 6172 223e 4d69  oung/MinAtar">Mi
+00001b30: 6e41 7461 722f 4272 6561 6b6f 7574 3c2f  nAtar/Breakout</
+00001b40: 613e 3c2f 7464 3e0a 203c 7464 3e3a 7768  a></td>. <td>:wh
+00001b50: 6974 655f 6368 6563 6b5f 6d61 726b 3a3c  ite_check_mark:<
+00001b60: 2f74 643e 0a20 3c74 643e 3a77 6869 7465  /td>. <td>:white
+00001b70: 5f63 6865 636b 5f6d 6172 6b3a 3c2f 7464  _check_mark:</td
+00001b80: 3e0a 3c2f 7472 3e0a 3c74 723e 0a20 3c74  >.</tr>.<tr>. <t
+00001b90: 643e 3c61 2068 7265 663d 2268 7474 7073  d><a href="https
+00001ba0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6b65  ://github.com/ke
+00001bb0: 6e6a 796f 756e 672f 4d69 6e41 7461 7222  njyoung/MinAtar"
+00001bc0: 3e4d 696e 4174 6172 2f46 7265 6577 6179  >MinAtar/Freeway
+00001bd0: 3c2f 613e 3c2f 7464 3e0a 203c 7464 3e3a  </a></td>. <td>:
+00001be0: 7768 6974 655f 6368 6563 6b5f 6d61 726b  white_check_mark
+00001bf0: 3a3c 2f74 643e 0a20 3c74 643e 3a77 6869  :</td>. <td>:whi
+00001c00: 7465 5f63 6865 636b 5f6d 6172 6b3a 3c2f  te_check_mark:</
+00001c10: 7464 3e0a 3c2f 7472 3e0a 3c74 723e 0a20  td>.</tr>.<tr>. 
+00001c20: 3c74 643e 3c61 2068 7265 663d 2268 7474  <td><a href="htt
+00001c30: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001c40: 6b65 6e6a 796f 756e 672f 4d69 6e41 7461  kenjyoung/MinAta
+00001c50: 7222 3e4d 696e 4174 6172 2f53 6561 7175  r">MinAtar/Seaqu
+00001c60: 6573 743c 2f61 3e3c 2f74 643e 0a20 3c74  est</a></td>. <t
+00001c70: 643e 3a77 6869 7465 5f63 6865 636b 5f6d  d>:white_check_m
+00001c80: 6172 6b3a 3c2f 7464 3e0a 203c 7464 3e3a  ark:</td>. <td>:
+00001c90: 7768 6974 655f 6368 6563 6b5f 6d61 726b  white_check_mark
+00001ca0: 3a3c 2f74 643e 0a3c 2f74 723e 0a3c 7472  :</td>.</tr>.<tr
+00001cb0: 3e0a 203c 7464 3e3c 6120 6872 6566 3d22  >. <td><a href="
+00001cc0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001cd0: 6f6d 2f6b 656e 6a79 6f75 6e67 2f4d 696e  om/kenjyoung/Min
+00001ce0: 4174 6172 223e 4d69 6e41 7461 722f 5370  Atar">MinAtar/Sp
+00001cf0: 6163 6549 6e76 6164 6572 733c 2f61 3e3c  aceInvaders</a><
+00001d00: 2f74 643e 0a20 3c74 643e 3a77 6869 7465  /td>. <td>:white
+00001d10: 5f63 6865 636b 5f6d 6172 6b3a 3c2f 7464  _check_mark:</td
+00001d20: 3e0a 203c 7464 3e3a 7768 6974 655f 6368  >. <td>:white_ch
+00001d30: 6563 6b5f 6d61 726b 3a3c 2f74 643e 0a3c  eck_mark:</td>.<
+00001d40: 2f74 723e 0a3c 7472 3e0a 203c 7464 3e3c  /tr>.<tr>. <td><
+00001d50: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00001d60: 656e 2e77 696b 6970 6564 6961 2e6f 7267  en.wikipedia.org
+00001d70: 2f77 696b 692f 5265 7665 7273 6922 3e4f  /wiki/Reversi">O
+00001d80: 7468 656c 6c6f 3c2f 613e 3c2f 7464 3e0a  thello</a></td>.
+00001d90: 203c 7464 3e3a 7768 6974 655f 6368 6563   <td>:white_chec
+00001da0: 6b5f 6d61 726b 3a3c 2f74 643e 0a20 3c74  k_mark:</td>. <t
+00001db0: 643e 3a77 6869 7465 5f63 6865 636b 5f6d  d>:white_check_m
+00001dc0: 6172 6b3a 3c2f 7464 3e0a 3c2f 7472 3e0a  ark:</td>.</tr>.
+00001dd0: 3c74 723e 0a20 3c74 643e 3c61 2068 7265  <tr>. <td><a hre
+00001de0: 663d 2268 7474 7073 3a2f 2f65 6e2e 7769  f="https://en.wi
+00001df0: 6b69 7065 6469 612e 6f72 672f 7769 6b69  kipedia.org/wiki
+00001e00: 2f53 686f 6769 223e 5368 6f67 693c 2f61  /Shogi">Shogi</a
+00001e10: 3e3c 2f74 643e 0a20 3c74 643e 3a77 6869  ></td>. <td>:whi
+00001e20: 7465 5f63 6865 636b 5f6d 6172 6b3a 3c2f  te_check_mark:</
+00001e30: 7464 3e0a 203c 7464 3e3a 7768 6974 655f  td>. <td>:white_
+00001e40: 6368 6563 6b5f 6d61 726b 3a3c 2f74 643e  check_mark:</td>
+00001e50: 0a3c 2f74 723e 0a3c 7472 3e0a 203c 7464  .</tr>.<tr>. <td
+00001e60: 3e3c 6120 6872 6566 3d22 6874 7470 733a  ><a href="https:
+00001e70: 2f2f 7375 676f 726f 6b75 7961 2e6a 702f  //sugorokuya.jp/
+00001e80: 702f 7375 7a75 6d65 2d6a 6f6e 6722 3e53  p/suzume-jong">S
+00001e90: 7061 7272 6f77 204d 6168 6a6f 6e67 3c2f  parrow Mahjong</
+00001ea0: 613e 3c2f 7464 3e0a 203c 7464 3e3a 7768  a></td>. <td>:wh
+00001eb0: 6974 655f 6368 6563 6b5f 6d61 726b 3a3c  ite_check_mark:<
+00001ec0: 2f74 643e 0a20 3c74 643e 3a77 6869 7465  /td>. <td>:white
+00001ed0: 5f63 6865 636b 5f6d 6172 6b3a 3c2f 7464  _check_mark:</td
+00001ee0: 3e0a 3c2f 7472 3e0a 3c74 723e 0a20 3c74  >.</tr>.<tr>. <t
+00001ef0: 643e 3c61 2068 7265 663d 2268 7474 7073  d><a href="https
+00001f00: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
+00001f10: 6f72 672f 7769 6b69 2f54 6963 2d74 6163  org/wiki/Tic-tac
+00001f20: 2d74 6f65 223e 5469 632d 7461 632d 746f  -toe">Tic-tac-to
+00001f30: 653c 2f61 3e3c 2f74 643e 0a20 3c74 643e  e</a></td>. <td>
+00001f40: 3a77 6869 7465 5f63 6865 636b 5f6d 6172  :white_check_mar
+00001f50: 6b3a 3c2f 7464 3e0a 203c 7464 3e3a 7768  k:</td>. <td>:wh
+00001f60: 6974 655f 6368 6563 6b5f 6d61 726b 3a3c  ite_check_mark:<
+00001f70: 2f74 643e 0a3c 2f74 723e 0a3c 2f74 6162  /td>.</tr>.</tab
+00001f80: 6c65 3e0a 3c2f 6469 763e 0a0a 2323 2053  le>.</div>..## S
+00001f90: 6565 2061 6c73 6f0a 0a50 6778 2069 7320  ee also..Pgx is 
+00001fa0: 696e 7465 6e64 6564 2074 6f20 636f 6d70  intended to comp
+00001fb0: 6c65 6d65 6e74 2074 6865 7365 202a 2a4a  lement these **J
+00001fc0: 4158 2d6e 6174 6976 6520 656e 7669 726f  AX-native enviro
+00001fd0: 6e6d 656e 7473 2a2a 2077 6974 6820 2863  nments** with (c
+00001fe0: 6c61 7373 6963 2920 626f 6172 6420 6761  lassic) board ga
+00001ff0: 6d65 2073 7569 7473 3a0a 0a2d 205b 526f  me suits:..- [Ro
+00002000: 6265 7274 544c 616e 6765 2f67 796d 6e61  bertTLange/gymna
+00002010: 785d 2868 7474 7073 3a2f 2f67 6974 6875  x](https://githu
+00002020: 622e 636f 6d2f 526f 6265 7274 544c 616e  b.com/RobertTLan
+00002030: 6765 2f67 796d 6e61 7829 3a20 4a41 5820  ge/gymnax): JAX 
+00002040: 696d 706c 656d 656e 7461 7469 6f6e 206f  implementation o
+00002050: 6620 706f 7075 6c61 7220 524c 2065 6e76  f popular RL env
+00002060: 6972 6f6e 6d65 6e74 7320 285b 636c 6173  ironments ([clas
+00002070: 7369 6320 636f 6e74 726f 6c5d 2868 7474  sic control](htt
+00002080: 7073 3a2f 2f67 796d 6e61 7369 756d 2e66  ps://gymnasium.f
+00002090: 6172 616d 612e 6f72 672f 656e 7669 726f  arama.org/enviro
+000020a0: 6e6d 656e 7473 2f63 6c61 7373 6963 5f63  nments/classic_c
+000020b0: 6f6e 7472 6f6c 292c 205b 6273 7569 7465  ontrol), [bsuite
+000020c0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000020d0: 2e63 6f6d 2f64 6565 706d 696e 642f 6273  .com/deepmind/bs
+000020e0: 7569 7465 292c 204d 696e 4174 6172 2c20  uite), MinAtar, 
+000020f0: 6574 6329 2061 6e64 206d 6574 6120 524c  etc) and meta RL
+00002100: 2074 6173 6b73 0a2d 205b 676f 6f67 6c65   tasks.- [google
+00002110: 2f62 7261 785d 2868 7474 7073 3a2f 2f67  /brax](https://g
+00002120: 6974 6875 622e 636f 6d2f 676f 6f67 6c65  ithub.com/google
+00002130: 2f62 7261 7829 3a20 5269 6769 6462 6f64  /brax): Rigidbod
+00002140: 7920 7068 7973 6963 7320 7369 6d75 6c61  y physics simula
+00002150: 7469 6f6e 2069 6e20 4a41 5820 616e 6420  tion in JAX and 
+00002160: 636f 6e74 696e 756f 7573 2d73 7061 6365  continuous-space
+00002170: 2052 4c20 7461 736b 7320 2861 6e74 2c20   RL tasks (ant, 
+00002180: 6665 7463 682c 2068 756d 616e 6f69 642c  fetch, humanoid,
+00002190: 2065 7463 290a 2d20 5b69 6e73 7461 6465   etc).- [instade
+000021a0: 6570 6169 2f6a 756d 616e 6a69 5d28 6874  epai/jumanji](ht
+000021b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000021c0: 2f69 6e73 7461 6465 6570 6169 2f6a 756d  /instadeepai/jum
+000021d0: 616e 6a69 293a 2041 2073 7569 7465 206f  anji): A suite o
+000021e0: 6620 6469 7665 7273 6520 616e 6420 6368  f diverse and ch
+000021f0: 616c 6c65 6e67 696e 670a 2020 2020 524c  allenging.    RL
+00002200: 2065 6e76 6972 6f6e 6d65 6e74 7320 696e   environments in
+00002210: 204a 4158 2028 6269 6e2d 7061 636b 696e   JAX (bin-packin
+00002220: 672c 2072 6f75 7469 6e67 2070 726f 626c  g, routing probl
+00002230: 656d 732c 2065 7463 290a 0a43 6f6d 6269  ems, etc)..Combi
+00002240: 6e69 6e67 2050 6778 2077 6974 6820 7468  ning Pgx with th
+00002250: 6573 6520 2a2a 4a41 582d 6e61 7469 7665  ese **JAX-native
+00002260: 2061 6c67 6f72 6974 686d 732f 696d 706c   algorithms/impl
+00002270: 656d 656e 7461 7469 6f6e 732a 2a20 6d69  ementations** mi
+00002280: 6768 7420 6265 2061 6e20 696e 7465 7265  ght be an intere
+00002290: 7374 696e 6720 6469 7265 6374 696f 6e3a  sting direction:
+000022a0: 0a0a 2d20 5b41 6e61 6b69 6e20 6672 616d  ..- [Anakin fram
+000022b0: 6577 6f72 6b5d 2868 7474 7073 3a2f 2f61  ework](https://a
+000022c0: 7278 6976 2e6f 7267 2f61 6273 2f32 3130  rxiv.org/abs/210
+000022d0: 342e 3036 3237 3229 3a20 4869 6768 6c79  4.06272): Highly
+000022e0: 2065 6666 6963 6965 6e74 2052 4c20 6672   efficient RL fr
+000022f0: 616d 6577 6f72 6b20 7468 6174 2077 6f72  amework that wor
+00002300: 6b73 2077 6974 6820 4a41 582d 6e61 7469  ks with JAX-nati
+00002310: 7665 2065 6e76 6972 6f6e 6d65 6e74 7320  ve environments 
+00002320: 6f6e 2054 5055 730a 2d20 5b64 6565 706d  on TPUs.- [deepm
+00002330: 696e 642f 6d63 7478 5d28 6874 7470 733a  ind/mctx](https:
+00002340: 2f2f 6769 7468 7562 2e63 6f6d 2f64 6565  //github.com/dee
+00002350: 706d 696e 642f 6d63 7478 293a 204a 4158  pmind/mctx): JAX
+00002360: 2d6e 6174 6976 6520 4d43 5453 2069 6d70  -native MCTS imp
+00002370: 6c65 6d65 6e74 6174 696f 6e73 2c20 696e  lementations, in
+00002380: 636c 7564 696e 6720 416c 7068 615a 6572  cluding AlphaZer
+00002390: 6f20 616e 6420 4d75 5a65 726f 0a2d 205b  o and MuZero.- [
+000023a0: 6465 6570 6d69 6e64 2f72 6c61 785d 2868  deepmind/rlax](h
+000023b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000023c0: 6d2f 6465 6570 6d69 6e64 2f72 6c61 7829  m/deepmind/rlax)
+000023d0: 3a20 4a41 582d 6e61 7469 7665 2052 4c20  : JAX-native RL 
+000023e0: 636f 6d70 6f6e 656e 7473 0a2d 205b 676f  components.- [go
+000023f0: 6f67 6c65 2f65 766f 6a61 785d 2868 7474  ogle/evojax](htt
+00002400: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00002410: 676f 6f67 6c65 2f65 766f 6a61 7829 3a20  google/evojax): 
+00002420: 4861 7264 7761 7265 2d41 6363 656c 6572  Hardware-Acceler
+00002430: 6174 6564 206e 6575 726f 6576 6f6c 7574  ated neuroevolut
+00002440: 696f 6e0a 2d20 5b52 6f62 6572 7454 4c61  ion.- [RobertTLa
+00002450: 6e67 652f 6576 6f73 6178 5d28 6874 7470  nge/evosax](http
+00002460: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f52  s://github.com/R
+00002470: 6f62 6572 7454 4c61 6e67 652f 6576 6f73  obertTLange/evos
+00002480: 6178 293a 204a 4158 2d6e 6174 6976 6520  ax): JAX-native 
+00002490: 6576 6f6c 7574 696f 6e20 7374 7261 7465  evolution strate
+000024a0: 6779 2028 4553 2920 696d 706c 656d 656e  gy (ES) implemen
+000024b0: 7461 7469 6f6e 730a 2d20 5b61 6461 7074  tations.- [adapt
+000024c0: 6976 652d 696e 7465 6c6c 6967 656e 742d  ive-intelligent-
+000024d0: 726f 626f 7469 6373 2f51 4461 785d 2868  robotics/QDax](h
+000024e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000024f0: 6d2f 6164 6170 7469 7665 2d69 6e74 656c  m/adaptive-intel
+00002500: 6c69 6765 6e74 2d72 6f62 6f74 6963 732f  ligent-robotics/
+00002510: 5144 6178 293a 204a 4158 2d6e 6174 6976  QDax): JAX-nativ
+00002520: 6520 5175 616c 6974 792d 4469 7665 7273  e Quality-Divers
+00002530: 6974 7920 2851 4429 2061 6c67 6f72 6974  ity (QD) algorit
+00002540: 686d 730a 0a0a 2323 204c 4943 454e 5345  hms...## LICENSE
+00002550: 0a0a 4170 6163 6865 2d32 2e30 0a         ..Apache-2.0.
```

### Comparing `pgx-0.2.1/pgx/_cache.py` & `pgx-0.3.0/pgx/_cache.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/animalshogi.py` & `pgx-0.3.0/pgx/_dwg/backgammon.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,165 +1,194 @@
-from pgx._animal_shogi import JaxAnimalShogiState as AnimalShogiState
+from pgx.backgammon import State as BackgammonState
+from pgx.backgammon import _get_abs_board
 
 
-def _make_animalshogi_dwg(dwg, state: AnimalShogiState, config: dict):
-    BOARD_WIDTH = 3
+def _make_backgammon_dwg(dwg, state: BackgammonState, config):
+    board = _get_abs_board(state)
+    BOARD_WIDTH = config["BOARD_WIDTH"]
     BOARD_HEIGHT = config["BOARD_HEIGHT"]
     GRID_SIZE = config["GRID_SIZE"]
     color_set = config["COLOR_SET"]
-    MOVE = {
-        "P": [(0, -1)],
-        "R": [(1, 0), (0, 1), (-1, 0), (0, -1)],
-        "B": [(1, 1), (-1, 1), (-1, -1), (1, -1)],
-        "K": [
-            (1, 0),
-            (0, 1),
-            (-1, 0),
-            (0, -1),
-            (1, 1),
-            (-1, 1),
-            (-1, -1),
-            (1, -1),
-        ],
-        "G": [(1, 0), (0, 1), (-1, 0), (0, -1), (-1, -1), (1, -1)],
-    }
-
     # background
     dwg.add(
         dwg.rect(
             (0, 0),
             (
-                (BOARD_WIDTH + 2) * GRID_SIZE,
-                (BOARD_HEIGHT + 1) * GRID_SIZE,
+                (BOARD_WIDTH + 6) * GRID_SIZE,
+                (BOARD_HEIGHT + 3) * GRID_SIZE,
             ),
             fill=color_set.background_color,
         )
     )
 
     # board
     # grid
     board_g = dwg.g()
-    hlines = board_g.add(dwg.g(id="hlines", stroke=color_set.grid_color))
-    for y in range(1, BOARD_HEIGHT):
-        hlines.add(
-            dwg.line(
-                start=(0, GRID_SIZE * y),
-                end=(
-                    GRID_SIZE * BOARD_WIDTH,
-                    GRID_SIZE * y,
-                ),
-            )
-        )
-    vlines = board_g.add(dwg.g(id="vline", stroke=color_set.grid_color))
-    for x in range(1, BOARD_WIDTH):
-        vlines.add(
-            dwg.line(
-                start=(GRID_SIZE * x, 0),
-                end=(
-                    GRID_SIZE * x,
-                    GRID_SIZE * BOARD_HEIGHT,
-                ),
+    for i in range(24):
+        p1 = (i * GRID_SIZE, 0)
+        p2 = ((i + 1) * GRID_SIZE, 0)
+        p3 = ((i + 0.5) * GRID_SIZE, 6 * GRID_SIZE)
+        if 6 <= i < 12:
+            p1 = ((i + 1) * GRID_SIZE, 0)
+            p2 = ((i + 2) * GRID_SIZE, 0)
+            p3 = ((i + 1.5) * GRID_SIZE, 6 * GRID_SIZE)
+        elif 12 <= i < 18:
+            p1 = ((i - 12) * GRID_SIZE, 14 * GRID_SIZE)
+            p2 = ((i + 1 - 12) * GRID_SIZE, 14 * GRID_SIZE)
+            p3 = ((i + 0.5 - 12) * GRID_SIZE, 8 * GRID_SIZE)
+        elif 18 <= i:
+            p1 = ((i + 1 - 12) * GRID_SIZE, 14 * GRID_SIZE)
+            p2 = ((i + 2 - 12) * GRID_SIZE, 14 * GRID_SIZE)
+            p3 = ((i + 1.5 - 12) * GRID_SIZE, 8 * GRID_SIZE)
+
+        fill_color = color_set.p1_color if i % 2 == 0 else color_set.text_color
+
+        board_g.add(
+            dwg.polygon(
+                points=[p1, p2, p3],
+                stroke=color_set.text_color,
+                fill=fill_color,
             )
         )
     board_g.add(
         dwg.rect(
             (0, 0),
             (
-                BOARD_WIDTH * GRID_SIZE,
-                BOARD_HEIGHT * GRID_SIZE,
+                13 * GRID_SIZE,
+                14 * GRID_SIZE,
             ),
+            stroke=color_set.grid_color,
             fill="none",
+        )
+    )
+    board_g.add(
+        dwg.rect(
+            (6 * GRID_SIZE, 0),
+            (
+                1 * GRID_SIZE,
+                14 * GRID_SIZE,
+            ),
             stroke=color_set.grid_color,
+            fill="none",
         )
     )
 
     # pieces
-    p1_pieces_g = dwg.g()
-    p2_pieces_g = dwg.g()
-    for i, piece_pos, piece_type in zip(
-        range(10),
-        state.board[1:11],
-        ["P", "R", "B", "K", "G", "P", "R", "B", "K", "G"],
-    ):
-        for xy, is_set in enumerate(piece_pos):
-            if is_set == 1:
-                if i < 5:
-                    pieces_g = p1_pieces_g
-                    x = 2 - xy // BOARD_HEIGHT  # AnimalShogiStateは右上原点
-                    y = xy % BOARD_HEIGHT
-                    fill_color = color_set.p1_color
-                    stroke = color_set.p1_outline
-                else:
-                    pieces_g = p2_pieces_g
-                    x = xy // BOARD_HEIGHT
-                    y = 3 - xy % BOARD_HEIGHT
-                    fill_color = color_set.p2_color
-                    stroke = color_set.p2_outline
-
-                pieces_g.add(
-                    dwg.rect(
-                        insert=(
-                            (x + 0.1) * GRID_SIZE,
-                            (y + 0.1) * GRID_SIZE,
-                        ),
-                        size=(
-                            0.8 * GRID_SIZE,
-                            0.8 * GRID_SIZE,
-                        ),
-                        rx="3px",
-                        ry="3px",
-                        stroke=stroke,
-                        fill=fill_color,
-                    )
+    for i, piece in enumerate(board[:24]):
+        fill_color = color_set.p2_color
+        if piece < 0:  # 白
+            piece = -piece
+            fill_color = color_set.p1_color
+
+        x = (12 - i) + 0.5
+        y = 13.5
+        diff = -1
+        if 6 <= i < 12:
+            x = (12 - i) - 0.5
+            y = 13.5
+        elif 12 <= i < 18:
+            x = i - 12 + 0.5
+            y = 0.5
+            diff = 1
+        elif 18 <= i:
+            x = i - 12 + 1.5
+            y = 0.5
+            diff = 1
+        for n in range(piece):
+            board_g.add(
+                dwg.circle(
+                    center=(x * GRID_SIZE, (y + n * diff) * GRID_SIZE),
+                    r=0.5 * GRID_SIZE,
+                    stroke=color_set.grid_color,
+                    fill=fill_color,
                 )
-                pieces_g.add(
-                    dwg.text(
-                        text=piece_type,
-                        insert=(
-                            (x + 0.27) * GRID_SIZE,
-                            (y + 0.72) * GRID_SIZE,
-                        ),
-                        fill=stroke,
-                        font_size="46px",
-                        font_family="Courier",
-                    )
+            )
+
+    # bar
+    for i, piece in enumerate(board[24:26]):  # 24:黒, 25:白
+        fill_color = color_set.p2_color
+        delta = 1
+        offset = 0.5
+        if i == 1:
+            piece = -piece
+            fill_color = color_set.p1_color
+            delta = -1
+            offset = -0.5
+        for n in range(piece):
+            board_g.add(
+                dwg.circle(
+                    center=(
+                        6.5 * GRID_SIZE,
+                        (7 + offset + n * delta) * GRID_SIZE,
+                    ),
+                    r=0.5 * GRID_SIZE,
+                    stroke=color_set.grid_color,
+                    fill=fill_color,
                 )
-                # 移動可能方向
-                for _x, _y in MOVE[piece_type]:
-                    pieces_g.add(
-                        dwg.circle(
-                            center=(
-                                (x + 0.5 + _x * 0.35) * GRID_SIZE,
-                                (y + 0.5 + _y * 0.35) * GRID_SIZE,
-                            ),
-                            r=GRID_SIZE * 0.01,
-                            stroke=stroke,
-                            fill=stroke,
-                        )
-                    )
-    # hand
-    for i, piece_num, piece_type in zip(
-        range(6), state.hand, ["P", "R", "B", "P", "R", "B"]
-    ):
-        _g = p1_pieces_g if i < 3 else p2_pieces_g
-        _g.add(
-            dwg.text(
-                text=f"{piece_type}:{piece_num}",
-                insert=(
-                    3.1 * GRID_SIZE,
-                    (3.3 + (i % 3) * 0.3) * GRID_SIZE,
-                ),
-                fill=color_set.p1_outline,
-                font_size="20px",
-                font_family="Courier",
             )
+
+    # off
+    board_g.add(
+        dwg.rect(
+            (13 * GRID_SIZE, 0),
+            (
+                4 * GRID_SIZE,
+                2 * GRID_SIZE,
+            ),
+            stroke=color_set.grid_color,
+            fill=color_set.background_color,
+        )
+    )
+    board_g.add(
+        dwg.circle(
+            center=(14 * GRID_SIZE, 1 * GRID_SIZE),
+            r=0.5 * GRID_SIZE,
+            stroke=color_set.grid_color,
+            fill=color_set.p2_color,
+        )
+    )
+    board_g.add(
+        dwg.text(
+            text=f"×{board[26]}",  # 26:黒
+            insert=(
+                14.6 * GRID_SIZE,
+                1.4 * GRID_SIZE,
+            ),
+            fill=color_set.grid_color,
+            font_size="34px",
+            font_family="serif",
         )
+    )
 
-    board_g.add(p1_pieces_g)
-    p2_pieces_g.rotate(
-        angle=180,
-        center=(GRID_SIZE * BOARD_WIDTH / 2, GRID_SIZE * BOARD_HEIGHT / 2),
+    board_g.add(
+        dwg.rect(
+            (13 * GRID_SIZE, 12 * GRID_SIZE),
+            (
+                4 * GRID_SIZE,
+                2 * GRID_SIZE,
+            ),
+            stroke=color_set.grid_color,
+            fill=color_set.background_color,
+        )
+    )
+    board_g.add(
+        dwg.circle(
+            center=(14 * GRID_SIZE, 13 * GRID_SIZE),
+            r=0.5 * GRID_SIZE,
+            stroke=color_set.grid_color,
+            fill=color_set.p1_color,
+        )
+    )
+    board_g.add(
+        dwg.text(
+            text=f"×{-board[27]}",  # 27:白
+            insert=(
+                14.6 * GRID_SIZE,
+                13.4 * GRID_SIZE,
+            ),
+            fill=color_set.grid_color,
+            font_size="34px",
+            font_family="serif",
+        )
     )
-    board_g.add(p2_pieces_g)
-    board_g.translate(GRID_SIZE / 2, 0)
 
     return board_g
```

### Comparing `pgx-0.2.1/pgx/_dwg/bridge_bidding.py` & `pgx-0.3.0/pgx/_dwg/bridge_bidding.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import numpy as np
 
-from pgx._bridge_bidding import State as BridgeBiddingState
+from pgx.bridge_bidding import State as BridgeBiddingState
 
 
 def _make_bridge_dwg(dwg, state: BridgeBiddingState, config):
     NUM_CARD_TYPE = 13
     # fmt: off
     TO_CARD = ["A", "2", "3", "4", "5", "6", "7", "8", "9", "10", "J", "Q", "K"]
-    SUITS = ["\u2660", "\u2665", "\u2666", "\u2663", "N"]  # ♠♡♢♣
+    SUITS = ["\u2660", "\u2665", "\u2666", "\u2663"]  # ♠♡♢♣
+    DENOMINATIONS = ["\u2663", "\u2666", "\u2665", "\u2660", "N"]  # ♣♢♡♠
     ACT = ["P", "X", "XX"]
     # fmt:on
     color_set = config["COLOR_SET"]
 
     # board
     board_g = dwg.g()
 
     # hand
     x_offset = [235, 480, 235, -10]
     y_offset = [10, 190, 370, 190]
     area_width = 230
     area_height = 150
-    for i in range(4):  # player0,1,2,3
+    for i in range(4):  # N, E, S, W
         hand = sorted(state.hand[i * NUM_CARD_TYPE : (i + 1) * NUM_CARD_TYPE])
         assert len(hand) == NUM_CARD_TYPE
         # player
         pos = np.array(["North", "East", "South", "West"], dtype=object)
         pos[state.dealer] = pos[state.dealer] + "(Dealer)"
         newline_offset = 0
         over_offset = 0
@@ -169,15 +170,15 @@
                 fill=color_set.grid_color,
                 font_size="20px",
                 font_family="Courier",
                 font_weight="bold",
             )
         )
 
-        # val
+        # vul
         if (state.vul_NS and i % 2 == 0) or (state.vul_EW and i % 2 == 1):
             board_g.add(
                 dwg.text(
                     text="Vul.",
                     insert=(
                         x_offset[i] + area_width + over_offset - 50,
                         y_offset[i],
@@ -205,15 +206,15 @@
             stroke_width="5px",
         )
     )
     for i, act in enumerate(state.bidding_history):
         if act == -1:
             break
         act_str = (
-            str(act // 5 + 1) + SUITS[act % 5]
+            str(act // 5 + 1) + DENOMINATIONS[(act % 5)]
             if 0 <= act < 35
             else ACT[act - 35]
         )
         color = (
             "orangered"
             if act % 5 == 1 or act % 5 == 2
             else color_set.text_color
```

### Comparing `pgx-0.2.1/pgx/_dwg/chess.py` & `pgx-0.3.0/pgx/_dwg/chess.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import base64
 import os
 
-from pgx._chess import ChessState
+from pgx.chess import State as ChessState
+from pgx.chess import _flip
 
 
 def _make_chess_dwg(dwg, state: ChessState, config):
     def _set_piece(_x, _y, _type, _dwg, _dwg_g, grid_size):
         PATH = {
             "P": "images/chess/bPawn.svg",
             "N": "images/chess/bKnight.svg",
@@ -37,26 +38,27 @@
 
     GRID_SIZE = config["GRID_SIZE"]
     BOARD_WIDTH = 8
     BOARD_HEIGHT = 8
 
     NUM_TO_CHAR = ["a", "b", "c", "d", "e", "f", "g", "h"]
     PIECES = [
-        "P",
-        "N",
-        "B",
-        "R",
-        "Q",
-        "K",
+        "",
         "wP",
         "wN",
         "wB",
         "wR",
         "wQ",
         "wK",
+        "P",
+        "N",
+        "B",
+        "R",
+        "Q",
+        "K",
     ]  # k"N"ight
     color_set = config["COLOR_SET"]
 
     # background
     dwg.add(
         dwg.rect(
             (0, 0),
@@ -125,31 +127,35 @@
                     (8.35) * GRID_SIZE,
                 ),
                 font_size="20px",
                 font_family="Serif",
             )
         )
 
+    if state.turn == 1:
+        state = _flip(state)
     # pieces
     pieces_g = dwg.g()
-    for i, piece_pos, piece_type in zip(
-        range(12),
-        state.board[1:13],
-        PIECES,
-    ):
-        for xy, is_set in enumerate(piece_pos):
-            if is_set == 1:
-                x = xy // BOARD_HEIGHT  # ChessStateは左下原点
-                y = 7 - xy % BOARD_HEIGHT
-                pieces_g = _set_piece(
-                    x * GRID_SIZE,
-                    y * GRID_SIZE,
-                    piece_type,
-                    dwg,
-                    pieces_g,
-                    GRID_SIZE,
-                )
+    for i in range(64):
+        pi = int(state.board[i].item())
+        if pi == 0:
+            continue
+        if pi < 0:
+            pi *= -1
+            pi += 6
+        piece_type = PIECES[pi]
+        xy = i
+        x = xy // BOARD_HEIGHT  # ChessStateは左下原点
+        y = 7 - xy % BOARD_HEIGHT
+        pieces_g = _set_piece(
+            x * GRID_SIZE,
+            y * GRID_SIZE,
+            piece_type,
+            dwg,
+            pieces_g,
+            GRID_SIZE,
+        )
 
     board_g.add(pieces_g)
     board_g.translate(10, 0)
 
     return board_g
```

### Comparing `pgx-0.2.1/pgx/_dwg/connect_four.py` & `pgx-0.3.0/pgx/_dwg/connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/go.py` & `pgx-0.3.0/pgx/_dwg/go.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/chess/LICENSE` & `pgx-0.3.0/pgx/_dwg/images/chess/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/chess/bBishop.svg` & `pgx-0.3.0/pgx/_dwg/images/chess/bBishop.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/chess/bKing.svg` & `pgx-0.3.0/pgx/_dwg/images/chess/bKing.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/chess/bKnight.svg` & `pgx-0.3.0/pgx/_dwg/images/chess/bKnight.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/chess/bPawn.svg` & `pgx-0.3.0/pgx/_dwg/images/chess/bPawn.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/chess/bQueen.svg` & `pgx-0.3.0/pgx/_dwg/images/chess/bQueen.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/chess/bRook.svg` & `pgx-0.3.0/pgx/_dwg/images/chess/bRook.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/chess/wBishop.svg` & `pgx-0.3.0/pgx/_dwg/images/chess/wBishop.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/chess/wKing.svg` & `pgx-0.3.0/pgx/_dwg/images/chess/wKing.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/chess/wKnight.svg` & `pgx-0.3.0/pgx/_dwg/images/chess/wKnight.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/chess/wPawn.svg` & `pgx-0.3.0/pgx/_dwg/images/chess/wPawn.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/chess/wQueen.svg` & `pgx-0.3.0/pgx/_dwg/images/chess/wQueen.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/chess/wRook.svg` & `pgx-0.3.0/pgx/_dwg/images/chess/wRook.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/1p.svg` & `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/1p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/1pr.svg` & `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/1pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/2p.svg` & `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/2p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/2pr.svg` & `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/2pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/3p.svg` & `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/3p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/3pr.svg` & `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/3pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/4p.svg` & `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/4p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/4pr.svg` & `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/4pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/5p.svg` & `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/5p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/5pr.svg` & `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/5pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/6p.svg` & `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/6p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/6pr.svg` & `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/6pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/7p.svg` & `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/7p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/7pr.svg` & `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/7pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/8p.svg` & `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/8p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/8pr.svg` & `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/8pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/9p.svg` & `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/9p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/9pr.svg` & `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/9pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/b.svg` & `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/b.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/gd.svg` & `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/gd.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/oya.svg` & `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/oya.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/images/sparrow_mahjong/rd.svg` & `pgx-0.3.0/pgx/_dwg/images/sparrow_mahjong/rd.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/kuhn_poker.py` & `pgx-0.3.0/pgx/_dwg/kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/leduc_holdem.py` & `pgx-0.3.0/pgx/_dwg/leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/othello.py` & `pgx-0.3.0/pgx/_dwg/othello.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             (0, 0),
             (
                 BOARD_SIZE * GRID_SIZE,
                 BOARD_SIZE * GRID_SIZE,
             ),
             fill="none",
             stroke=color_set.grid_color,
-            stroke_width="20px",
+            stroke_width="10px",
             rx="3px",
             ry="3px",
         )
     )
     board_g.add(
         dwg.rect(
             (0, 0),
```

### Comparing `pgx-0.2.1/pgx/_dwg/play2048.py` & `pgx-0.3.0/pgx/_dwg/play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/shogi.py` & `pgx-0.3.0/pgx/_dwg/shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/sparrow_mahjong.py` & `pgx-0.3.0/pgx/_dwg/sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_dwg/tictactoe.py` & `pgx-0.3.0/pgx/_dwg/tictactoe.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_flax/serialization.py` & `pgx-0.3.0/pgx/_flax/serialization.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_flax/struct.py` & `pgx-0.3.0/pgx/_flax/struct.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_shogi_utils.py` & `pgx-0.3.0/pgx/_shogi_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_test.py` & `pgx-0.3.0/pgx/_test.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/_visualizer.py` & `pgx-0.3.0/pgx/_visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,16 @@
         try:
             SIZE = len(states.current_player)
             WIDTH = math.ceil(math.sqrt(SIZE - 0.1))
             if SIZE - (WIDTH - 1) ** 2 >= WIDTH:
                 HEIGHT = WIDTH
             else:
                 HEIGHT = WIDTH - 1
+            if SIZE == 1:
+                states = self._get_nth_state(states, 0)
         except TypeError:
             SIZE = 1
             WIDTH = 1
             HEIGHT = 1
 
         self._set_config_by_state(states)
         assert self._make_dwg_group is not None
@@ -232,31 +234,31 @@
             self.config["BOARD_HEIGHT"] = 14
             self._make_dwg_group = _make_backgammon_dwg
             if (
                 self.config["COLOR_THEME"] is None
                 and self.config["COLOR_THEME"] == "dark"
             ) or self.config["COLOR_THEME"] == "dark":
                 self.config["COLOR_SET"] = ColorSet(
-                    "gray",
-                    "black",
                     "black",
-                    "dimgray",
+                    "darkgray",
+                    "white",
+                    "white",
                     "#1e1e1e",
-                    "gainsboro",
-                    "",
+                    "silver",
+                    "dimgray",
                 )
             else:
                 self.config["COLOR_SET"] = ColorSet(
                     "white",
                     "black",
                     "lightgray",
                     "white",
                     "white",
                     "black",
-                    "",
+                    "gray",
                 )
         elif isinstance(_state, BridgeBiddingState):
             self.config["GRID_SIZE"] = 50
             self.config["BOARD_WIDTH"] = 14
             self.config["BOARD_HEIGHT"] = 10
             self._make_dwg_group = _make_bridge_dwg
             if (
@@ -317,19 +319,19 @@
             self._make_dwg_group = _make_connect_four_dwg
             if (
                 self.config["COLOR_THEME"] is None
                 and self.config["COLOR_THEME"] == "dark"
             ) or self.config["COLOR_THEME"] == "dark":
                 self.config["COLOR_SET"] = ColorSet(
                     "black",
-                    "lightgray",
+                    "darkgray",
+                    "white",
                     "white",
-                    "lightgray",
                     "#1e1e1e",
-                    "lightgray",
+                    "silver",
                     "gray",
                 )
             else:
                 self.config["COLOR_SET"] = ColorSet(
                     "black",
                     "white",
                     "black",
@@ -348,47 +350,61 @@
                 self.config["BOARD_HEIGHT"] = int(_state.size)
             self._make_dwg_group = _make_go_dwg
             if (
                 self.config["COLOR_THEME"] is None
                 and self.config["COLOR_THEME"] == "dark"
             ) or self.config["COLOR_THEME"] == "dark":
                 self.config["COLOR_SET"] = ColorSet(
-                    "black", "gray", "white", "white", "#1e1e1e", "white", ""
+                    "black",
+                    "darkgray",
+                    "white",
+                    "white",
+                    "#1e1e1e",
+                    "silver",
+                    "",
                 )
             else:
                 self.config["COLOR_SET"] = ColorSet(
                     "black",
                     "white",
                     "black",
                     "black",
                     "white",
                     "black",
                     "",
                 )
         elif isinstance(_state, HexState):
+            import jax.numpy as jnp
+
+            from pgx._dwg.hex import four_dig
+
             self.config["GRID_SIZE"] = 30
             try:
-                self.config["BOARD_WIDTH"] = int(_state.size[0] * 1.3)
-                self.config["BOARD_HEIGHT"] = int(_state.size[0] * 0.8)
+                self.config["BOARD_WIDTH"] = four_dig(_state.size[0] * 1.5)
+                self.config["BOARD_HEIGHT"] = four_dig(
+                    _state.size[0] * jnp.sqrt(3) / 2
+                )
             except IndexError:
-                self.config["BOARD_WIDTH"] = int(_state.size * 1.3)
-                self.config["BOARD_HEIGHT"] = int(_state.size * 0.8)
+                self.config["BOARD_WIDTH"] = four_dig(_state.size * 1.5)
+                self.config["BOARD_HEIGHT"] = four_dig(
+                    _state.size * jnp.sqrt(3) / 2
+                )
             self._make_dwg_group = _make_hex_dwg
             if (
                 self.config["COLOR_THEME"] is None
                 and self.config["COLOR_THEME"] == "dark"
             ) or self.config["COLOR_THEME"] == "dark":
                 self.config["COLOR_SET"] = ColorSet(
                     "black",
+                    "darkgray",
                     "white",
                     "white",
-                    "black",
                     "#1e1e1e",
-                    "white",
-                    "dimgray",
+                    "gray",
+                    "#333333",
                 )
             else:
                 self.config["COLOR_SET"] = ColorSet(
                     "black",
                     "white",
                     "black",
                     "black",
@@ -459,19 +475,19 @@
             self._make_dwg_group = _make_othello_dwg
             if (
                 self.config["COLOR_THEME"] is None
                 and self.config["COLOR_THEME"] == "dark"
             ) or self.config["COLOR_THEME"] == "dark":
                 self.config["COLOR_SET"] = ColorSet(
                     "black",
-                    "lightgray",
+                    "darkgray",
+                    "white",
                     "white",
-                    "lightgray",
                     "#1e1e1e",
-                    "lightgray",
+                    "silver",
                     "",
                 )
             else:
                 self.config["COLOR_SET"] = ColorSet(
                     "black",
                     "white",
                     "black",
@@ -603,14 +619,15 @@
             return ChessState(
                 turn=_states.turn[_i],  # type:ignore
                 board=_states.board[_i],
             )
         elif isinstance(_states, BridgeBiddingState):
             return BridgeBiddingState(  # type:ignore
                 turn=_states.turn[_i],
+                dealer=_states.dealer[_i],
                 current_player=_states.current_player[_i],
                 hand=_states.hand[_i],
                 bidding_history=_states.bidding_history[_i],
                 vul_NS=_states.vul_NS[_i],
                 vul_EW=_states.vul_EW[_i],
             )
         elif isinstance(_states, GoState):
```

### Comparing `pgx-0.2.1/pgx/backgammon.py` & `pgx-0.3.0/pgx/backgammon.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/connect_four.py` & `pgx-0.3.0/pgx/connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/core.py` & `pgx-0.3.0/pgx/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,17 +30,18 @@
 # We do not explicitly include version in EnvId for three reasons:
 # (1) In game domain, performance measure is not the score in environment but
 #     the comparison to other agents (i.e., environment version is less important),
 # (2) we do not provide older versions (as with OpenAI Gym), and
 # (3) it is tedious to remember and write version numbers.
 EnvId = Literal[
     "2048",
-    # "animal_shogi",
+    "animal_shogi",
     "backgammon",
-    # "bridge_bidding",
+    "bridge_bidding",
+    "chess",
     "connect_four",
     "go-9x9",
     "go-19x19",
     "hex",
     "kuhn_poker",
     "leduc_holdem",
     # "mahjong",
@@ -203,24 +204,36 @@
         return state.replace(reward=reward, terminated=TRUE)  # type: ignore
 
 
 def available_games() -> Tuple[EnvId, ...]:
     return get_args(EnvId)
 
 
-def make(env_id: EnvId):
+def make(env_id: EnvId):  # noqa: C901
     if env_id == "2048":
         from pgx.play2048 import Play2048
 
         return Play2048()
-    if env_id == "backgammon":
+    elif env_id == "animal_shogi":
+        from pgx.animal_shogi import AnimalShogi
+
+        return AnimalShogi()
+    elif env_id == "backgammon":
         from pgx.backgammon import Backgammon
 
         return Backgammon()
-    if env_id == "connect_four":
+    elif env_id == "bridge_bidding":
+        from pgx.bridge_bidding import BridgeBidding
+
+        return BridgeBidding()
+    elif env_id == "chess":
+        from pgx.chess import Chess
+
+        return Chess()
+    elif env_id == "connect_four":
         from pgx.connect_four import ConnectFour
 
         return ConnectFour()
     elif env_id == "go-9x9":
         from pgx.go import Go
 
         return Go(size=9, komi=7.5)
```

### Comparing `pgx-0.2.1/pgx/experimental/gym.py` & `pgx-0.3.0/pgx/experimental/gym.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/experimental/pettingzoo.py` & `pgx-0.3.0/pgx/experimental/pettingzoo.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/experimental/visualize.py` & `pgx-0.3.0/pgx/experimental/visualize.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/experimental/wrappers.py` & `pgx-0.3.0/pgx/experimental/wrappers.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/go.py` & `pgx-0.3.0/pgx/go.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/hex.py` & `pgx-0.3.0/pgx/hex.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/kuhn_poker.py` & `pgx-0.3.0/pgx/kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/leduc_holdem.py` & `pgx-0.3.0/pgx/leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/minatar/asterix.py` & `pgx-0.3.0/pgx/minatar/asterix.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/minatar/breakout.py` & `pgx-0.3.0/pgx/minatar/breakout.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/minatar/freeway.py` & `pgx-0.3.0/pgx/minatar/freeway.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/minatar/seaquest.py` & `pgx-0.3.0/pgx/minatar/seaquest.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/minatar/space_invaders.py` & `pgx-0.3.0/pgx/minatar/space_invaders.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/minatar/utils.py` & `pgx-0.3.0/pgx/minatar/utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/othello.py` & `pgx-0.3.0/pgx/othello.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/play2048.py` & `pgx-0.3.0/pgx/play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/shogi.py` & `pgx-0.3.0/pgx/shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/sparrow_mahjong.py` & `pgx-0.3.0/pgx/sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx/tic_tac_toe.py` & `pgx-0.3.0/pgx/tic_tac_toe.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/pgx.egg-info/SOURCES.txt` & `pgx-0.3.0/pgx.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 pgx/__init__.py
-pgx/_animal_shogi.py
-pgx/_bridge_bidding.py
 pgx/_cache.py
-pgx/_chess.py
+pgx/_chess_utils.py
 pgx/_shogi_utils.py
 pgx/_test.py
 pgx/_visualizer.py
+pgx/animal_shogi.py
 pgx/backgammon.py
+pgx/bridge_bidding.py
+pgx/chess.py
 pgx/connect_four.py
 pgx/core.py
 pgx/go.py
 pgx/hex.py
 pgx/kuhn_poker.py
 pgx/leduc_holdem.py
 pgx/othello.py
```

### Comparing `pgx-0.2.1/setup.py` & `pgx-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="pgx",
-    version="0.2.1",
+    version="0.3.0",
     long_description_content_type="text/markdown",
     description="",
     url="",
     author="Sotetsu KOYAMADA",
     author_email="sotetsu.koyamada@gmail.com",
     keywords="",
     packages=find_packages(),
```

### Comparing `pgx-0.2.1/tests/minatar_utils.py` & `pgx-0.3.0/tests/minatar_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/tests/test_asterix.py` & `pgx-0.3.0/tests/test_asterix.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/tests/test_backgammon.py` & `pgx-0.3.0/tests/test_backgammon.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/tests/test_breakout.py` & `pgx-0.3.0/tests/test_breakout.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/tests/test_bridge_bidding.py` & `pgx-0.3.0/tests/test_bridge_bidding.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 import csv
 from typing import Tuple
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 
-from pgx._bridge_bidding import (
+from pgx.bridge_bidding import (
+    BridgeBidding,
     State,
     _calc_score,
     _calculate_dds_tricks,
     _contract,
+    _init_by_key,
     _key_to_hand,
     _load_sample_hash,
     _pbn_to_key,
     _player_position,
     _shuffle_players,
     _state_to_key,
     _state_to_pbn,
     _to_binary,
     _value_to_dds_tricks,
     duplicate,
     init,
-    init_by_key,
-    step,
 )
 
+env = BridgeBidding()
+init_by_key = jax.jit(env.init)
+step = jax.jit(env.step)
+observe = jax.jit(env.observe)
+
 
 def test_shuffle_players():
     key = jax.random.PRNGKey(0)
     for i in range(100):
         key, subkey = jax.random.split(key)
         shuffled_players = _shuffle_players(subkey)
         assert (shuffled_players[0] - shuffled_players[2]) % 2
@@ -81,30 +86,31 @@
     #  1C 2S  X  P
     #   P XX  P 5H
     #  5S  P 6C  X
     #  XX  P 7C  P
     #   P  P
     key = jax.random.PRNGKey(0)
     HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES = _load_sample_hash()
-    state = init_by_key(HASH_TABLE_SAMPLE_KEYS[0], key)
+    state = _init_by_key(HASH_TABLE_SAMPLE_KEYS[0], key)
+    # state = init_by_key(HASH_TABLE_SAMPLE_KEYS[0], key)
     state = state.replace(
         dealer=jnp.int8(1),
         current_player=jnp.int8(3),
         shuffled_players=jnp.array([0, 3, 1, 2], dtype=jnp.int8),
         vul_NS=jnp.bool_(0),
         vul_EW=jnp.bool_(0),
     )
     bidding_history = jnp.full(319, -1, dtype=jnp.int8)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = legal_action_mask.at[36].set(False)
     legal_action_mask = legal_action_mask.at[37].set(False)
     first_denomination_NS = jnp.full(5, -1, dtype=jnp.int8)
     first_denomination_EW = jnp.full(5, -1, dtype=jnp.int8)
 
-    state = step(state, 35, HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES)
+    state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P
 
     assert state.turn == 1
@@ -119,15 +125,15 @@
     assert not state.call_x
     assert not state.call_xx
     assert jnp.all(state.first_denomination_NS == first_denomination_NS)
     assert jnp.all(state.first_denomination_EW == first_denomination_EW)
     assert state.pass_num == 1
     assert jnp.all(state.reward == np.zeros(4))
 
-    state = step(state, 35, HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES)
+    state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P
 
     assert state.turn == 2
@@ -142,15 +148,15 @@
     assert not state.call_x
     assert not state.call_xx
     assert jnp.all(state.first_denomination_NS == first_denomination_NS)
     assert jnp.all(state.first_denomination_EW == first_denomination_EW)
     assert state.pass_num == 2
     assert jnp.all(state.reward == jnp.zeros(4))
 
-    state = step(state, 35, HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES)
+    state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
 
     assert state.turn == 3
@@ -165,15 +171,15 @@
     assert not state.call_x
     assert not state.call_xx
     assert jnp.all(state.first_denomination_NS == first_denomination_NS)
     assert jnp.all(state.first_denomination_EW == first_denomination_EW)
     assert state.pass_num == 3
     assert jnp.all(state.reward == jnp.zeros(4))
 
-    state = step(state, 0, HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES)
+    state = step(state, 0)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C
     first_denomination_NS = jnp.array([0, -1, -1, -1, -1])
@@ -193,15 +199,15 @@
     assert not state.call_x
     assert not state.call_xx
     assert jnp.all(state.first_denomination_NS == first_denomination_NS)
     assert jnp.all(state.first_denomination_EW == first_denomination_EW)
     assert state.pass_num == 0
     assert jnp.all(state.reward == jnp.zeros(4))
 
-    state = step(state, 8, HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES)
+    state = step(state, 8)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S
     first_denomination_NS = jnp.array([0, -1, -1, -1, -1])
@@ -223,15 +229,15 @@
     assert not state.call_x
     assert not state.call_xx
     assert jnp.all(state.first_denomination_NS == first_denomination_NS)
     assert jnp.all(state.first_denomination_EW == first_denomination_EW)
     assert state.pass_num == 0
     assert jnp.all(state.reward == jnp.zeros(4))
 
-    state = step(state, 36, HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES)
+    state = step(state, 36)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X
     first_denomination_NS = jnp.array([0, -1, -1, -1, -1])
@@ -254,15 +260,15 @@
     assert state.call_x
     assert not state.call_xx
     assert jnp.all(state.first_denomination_NS == first_denomination_NS)
     assert jnp.all(state.first_denomination_EW == first_denomination_EW)
     assert state.pass_num == 0
     assert jnp.all(state.reward == jnp.zeros(4))
 
-    state = step(state, 35, HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES)
+    state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     first_denomination_NS = jnp.array([0, -1, -1, -1, -1])
@@ -286,15 +292,15 @@
     assert state.call_x
     assert not state.call_xx
     assert jnp.all(state.first_denomination_NS == first_denomination_NS)
     assert jnp.all(state.first_denomination_EW == first_denomination_EW)
     assert state.pass_num == 1
     assert jnp.all(state.reward == jnp.zeros(4))
 
-    state = step(state, 35, HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES)
+    state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P
@@ -319,15 +325,15 @@
     assert state.call_x
     assert not state.call_xx
     assert jnp.all(state.first_denomination_NS == first_denomination_NS)
     assert jnp.all(state.first_denomination_EW == first_denomination_EW)
     assert state.pass_num == 2
     assert jnp.all(state.reward == jnp.zeros(4))
 
-    state = step(state, 37, HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES)
+    state = step(state, 37)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX
@@ -352,15 +358,15 @@
     assert state.call_x
     assert state.call_xx
     assert jnp.all(state.first_denomination_NS == first_denomination_NS)
     assert jnp.all(state.first_denomination_EW == first_denomination_EW)
     assert state.pass_num == 0
     assert jnp.all(state.reward == jnp.zeros(4))
 
-    state = step(state, 35, HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES)
+    state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P
@@ -385,15 +391,15 @@
     assert state.call_x
     assert state.call_xx
     assert jnp.all(state.first_denomination_NS == first_denomination_NS)
     assert jnp.all(state.first_denomination_EW == first_denomination_EW)
     assert state.pass_num == 1
     assert jnp.all(state.reward == jnp.zeros(4))
 
-    state = step(state, 22, HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES)
+    state = step(state, 22)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
@@ -418,15 +424,15 @@
     assert not state.call_x
     assert not state.call_xx
     assert jnp.all(state.first_denomination_NS == first_denomination_NS)
     assert jnp.all(state.first_denomination_EW == first_denomination_EW)
     assert state.pass_num == 0
     assert jnp.all(state.reward == jnp.zeros(4))
 
-    state = step(state, 23, HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES)
+    state = step(state, 23)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
@@ -452,15 +458,15 @@
     assert not state.call_x
     assert not state.call_xx
     assert jnp.all(state.first_denomination_NS == first_denomination_NS)
     assert jnp.all(state.first_denomination_EW == first_denomination_EW)
     assert state.pass_num == 0
     assert jnp.all(state.reward == jnp.zeros(4))
 
-    state = step(state, 35, HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES)
+    state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
@@ -486,15 +492,15 @@
     assert not state.call_x
     assert not state.call_xx
     assert jnp.all(state.first_denomination_NS == first_denomination_NS)
     assert jnp.all(state.first_denomination_EW == first_denomination_EW)
     assert state.pass_num == 1
     assert jnp.all(state.reward == jnp.zeros(4))
 
-    state = step(state, 25, HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES)
+    state = step(state, 25)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
@@ -520,15 +526,15 @@
     assert not state.call_x
     assert not state.call_xx
     assert jnp.all(state.first_denomination_NS == first_denomination_NS)
     assert jnp.all(state.first_denomination_EW == first_denomination_EW)
     assert state.pass_num == 0
     assert jnp.all(state.reward == jnp.zeros(4))
 
-    state = step(state, 36, HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES)
+    state = step(state, 36)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
@@ -554,15 +560,15 @@
     assert state.call_x
     assert not state.call_xx
     assert np.all(state.first_denomination_NS == first_denomination_NS)
     assert np.all(state.first_denomination_EW == first_denomination_EW)
     assert state.pass_num == 0
     assert np.all(state.reward == np.zeros(4))
 
-    state = step(state, 37, HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES)
+    state = step(state, 37)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
@@ -589,15 +595,15 @@
     assert state.call_x
     assert state.call_xx
     assert jnp.all(state.first_denomination_NS == first_denomination_NS)
     assert jnp.all(state.first_denomination_EW == first_denomination_EW)
     assert state.pass_num == 0
     assert jnp.all(state.reward == jnp.zeros(4))
 
-    state = step(state, 35, HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES)
+    state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
@@ -624,15 +630,15 @@
     assert state.call_x
     assert state.call_xx
     assert jnp.all(state.first_denomination_NS == first_denomination_NS)
     assert jnp.all(state.first_denomination_EW == first_denomination_EW)
     assert state.pass_num == 1
     assert jnp.all(state.reward == jnp.zeros(4))
 
-    state = step(state, 30, HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES)
+    state = step(state, 30)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
@@ -659,15 +665,15 @@
     assert not state.call_x
     assert not state.call_xx
     assert jnp.all(state.first_denomination_NS == first_denomination_NS)
     assert jnp.all(state.first_denomination_EW == first_denomination_EW)
     assert state.pass_num == 0
     assert jnp.all(state.reward == jnp.zeros(4))
 
-    state = step(state, 35, HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES)
+    state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
@@ -694,15 +700,15 @@
     assert not state.call_x
     assert not state.call_xx
     assert jnp.all(state.first_denomination_NS == first_denomination_NS)
     assert jnp.all(state.first_denomination_EW == first_denomination_EW)
     assert state.pass_num == 1
     assert jnp.all(state.reward == jnp.zeros(4))
 
-    state = step(state, 35, HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES)
+    state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
@@ -730,42 +736,41 @@
     assert not state.call_x
     assert not state.call_xx
     assert jnp.all(state.first_denomination_NS == first_denomination_NS)
     assert jnp.all(state.first_denomination_EW == first_denomination_EW)
     assert state.pass_num == 2
     assert jnp.all(state.reward == jnp.zeros(4))
 
-    state = step(state, 35, HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES)
+    state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #  1C 2S  X  P
     #   P XX  P 5H
     #  5S  P 6C  X
     #  XX  P 7C  P
     #   P  P
     # Passが3回続いたので終了
     assert state.terminated == True
-    assert state.current_player == -1
     first_denomination_NS = jnp.array([0, -1, -1, 0, -1])
     first_denomination_EW = jnp.array([-1, -1, 2, 3, -1])
 
     assert state.turn == 20
-    assert _player_position(state.current_player, state) == -1
     assert state.terminated
     bidding_history = bidding_history.at[20].set(35)
     assert jnp.all(state.bidding_history == bidding_history)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = jnp.where(
         jnp.arange(38) < 31, False, state.legal_action_mask
     )
-    legal_action_mask = legal_action_mask.at[36].set(True)
-    legal_action_mask = legal_action_mask.at[37].set(False)
+    legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
+    # legal_action_mask = legal_action_mask.at[36].set(True)
+    # legal_action_mask = legal_action_mask.at[37].set(False)s
     assert jnp.all(state.legal_action_mask == legal_action_mask)
     assert state.last_bid == 30
     assert _player_position(state.last_bidder, state) == 2
     assert not state.call_x
     assert not state.call_xx
     assert jnp.all(state.first_denomination_NS == first_denomination_NS)
     assert jnp.all(state.first_denomination_EW == first_denomination_EW)
@@ -793,45 +798,36 @@
     else:
         return int(state.last_bid) + 1
 
 
 def test_max_action():
     key = jax.random.PRNGKey(0)
     HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES = _load_sample_hash()
-    state = init(key)
+    state = _init_by_key(HASH_TABLE_SAMPLE_KEYS[0], key)
 
     for i in range(319):
         if i < 318:
-            state = step(
-                state,
-                max_action_length_agent(state),
-                HASH_TABLE_SAMPLE_KEYS,
-                HASH_TABLE_SAMPLE_VALUES,
-            )
+            state = step(state, max_action_length_agent(state))
             assert not state.terminated
         else:
-            state = step(
-                state,
-                max_action_length_agent(state),
-                HASH_TABLE_SAMPLE_KEYS,
-                HASH_TABLE_SAMPLE_VALUES,
-            )
+            state = step(state, max_action_length_agent(state))
             assert state.terminated
 
 
 def test_pass_out():
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #   P
     key = jax.random.PRNGKey(0)
     HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES = _load_sample_hash()
-    state = init_by_key(HASH_TABLE_SAMPLE_KEYS[1], key)
+    state = _init_by_key(HASH_TABLE_SAMPLE_KEYS[0], key)
+    # state = init_by_key(HASH_TABLE_SAMPLE_KEYS[1], key)
     state = state.replace(
         dealer=jnp.int8(1),
         current_player=jnp.int8(3),
         shuffled_players=jnp.array([0, 3, 1, 2], dtype=jnp.int8),
         vul_NS=jnp.bool_(0),
         vul_EW=jnp.bool_(0),
     )
@@ -839,15 +835,15 @@
     bidding_history = jnp.full(319, -1, dtype=jnp.int8)
     legal_action_mask = jnp.ones(38, dtype=jnp.bool_)
     legal_action_mask = legal_action_mask.at[36].set(False)
     legal_action_mask = legal_action_mask.at[37].set(False)
     first_denomination_NS = jnp.full(5, -1, dtype=jnp.int8)
     first_denomination_EW = jnp.full(5, -1, dtype=jnp.int8)
 
-    state = step(state, 35, HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES)
+    state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P
 
     assert state.turn == 1
@@ -862,15 +858,15 @@
     assert not state.call_x
     assert not state.call_xx
     assert jnp.all(state.first_denomination_NS == first_denomination_NS)
     assert jnp.all(state.first_denomination_EW == first_denomination_EW)
     assert state.pass_num == 1
     assert jnp.all(state.reward == jnp.zeros(4))
 
-    state = step(state, 35, HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES)
+    state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P
 
     assert state.turn == 2
@@ -885,15 +881,15 @@
     assert not state.call_x
     assert not state.call_xx
     assert jnp.all(state.first_denomination_NS == first_denomination_NS)
     assert jnp.all(state.first_denomination_EW == first_denomination_EW)
     assert state.pass_num == 2
     assert jnp.all(state.reward == jnp.zeros(4))
 
-    state = step(state, 35, HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES)
+    state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
 
     assert state.turn == 3
@@ -908,38 +904,458 @@
     assert not state.call_x
     assert not state.call_xx
     assert jnp.all(state.first_denomination_NS == first_denomination_NS)
     assert jnp.all(state.first_denomination_EW == first_denomination_EW)
     assert state.pass_num == 3
     assert jnp.all(state.reward == jnp.zeros(4))
 
-    state = step(state, 35, HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES)
+    state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
     #   P
 
     assert state.terminated == True
-    assert state.current_player == -1
     assert state.turn == 3
     bidding_history = bidding_history.at[3].set(35)
     assert jnp.all(state.bidding_history == bidding_history)
-    assert jnp.all(state.legal_action_mask == legal_action_mask)
+    assert jnp.all(state.legal_action_mask == jnp.ones(38, dtype=jnp.bool_))
     assert state.last_bid == -1
     assert _player_position(state.last_bidder, state) == -1
     assert not state.call_x
     assert not state.call_xx
     assert jnp.all(state.first_denomination_NS == first_denomination_NS)
     assert jnp.all(state.first_denomination_EW == first_denomination_EW)
     assert state.pass_num == 4
     assert jnp.all(state.reward == jnp.zeros(4))
 
 
+def test_observe():
+    # test init_obs
+    # hand
+    # hand: N:J92.J76.K72.9432 AKQ6.84.J863.T65 87543.KQ9532..K7 T.AT.AQT954.AQJ8
+    player0_hand = (
+        jnp.zeros(52, dtype=jnp.bool_)
+        .at[jnp.array([1, 8, 10, 18, 19, 23, 27, 32, 38, 40, 41, 42, 47])]
+        .set(True)
+    )
+    player1_hand = (
+        jnp.zeros(52, dtype=jnp.bool_)
+        .at[jnp.array([2, 3, 4, 6, 7, 14, 15, 17, 21, 24, 25, 45, 51])]
+        .set(True)
+    )
+    player2_hand = (
+        jnp.zeros(52, dtype=jnp.bool_)
+        .at[jnp.array([9, 13, 22, 26, 29, 30, 34, 35, 37, 39, 46, 49, 50])]
+        .set(True)
+    )
+    player3_hand = (
+        jnp.zeros(52, dtype=jnp.bool_)
+        .at[jnp.array([0, 5, 11, 12, 16, 20, 28, 31, 33, 36, 43, 44, 48])]
+        .set(True)
+    )
+    key = jax.random.PRNGKey(0)
+    HASH_TABLE_SAMPLE_KEYS, HASH_TABLE_SAMPLE_VALUES = _load_sample_hash()
+    state = _init_by_key(HASH_TABLE_SAMPLE_KEYS[0], key)
+    state = state.replace(
+        dealer=jnp.int8(1),
+        current_player=jnp.int8(3),
+        shuffled_players=jnp.array([0, 3, 1, 2], dtype=jnp.int8),
+        vul_NS=jnp.bool_(0),
+        vul_EW=jnp.bool_(0),
+    )
+
+    init_obs = jnp.concatenate((jnp.zeros(426, dtype=jnp.bool_), player0_hand))
+    obs = observe(state, 0)
+    print(_state_to_pbn(state))
+    assert jnp.all(obs == init_obs)
+
+    init_obs = jnp.concatenate((jnp.zeros(426, dtype=jnp.bool_), player1_hand))
+    obs = observe(state, 1)
+    assert jnp.all(obs == init_obs)
+
+    init_obs = jnp.concatenate((jnp.zeros(426, dtype=jnp.bool_), player2_hand))
+    obs = observe(state, 2)
+    assert jnp.all(obs == init_obs)
+
+    init_obs = jnp.concatenate((jnp.zeros(426, dtype=jnp.bool_), player3_hand))
+    obs = observe(state, 3)
+    assert jnp.all(obs == init_obs)
+
+    # vul
+    state = state.replace(
+        dealer=jnp.int8(1),
+        current_player=jnp.int8(3),
+        shuffled_players=jnp.array([0, 3, 1, 2], dtype=jnp.int8),
+        vul_NS=jnp.bool_(1),
+        vul_EW=jnp.bool_(0),
+    )
+    init_obs = (
+        jnp.concatenate((jnp.zeros(426, dtype=jnp.bool_), player0_hand))
+        .at[0]
+        .set(True)
+    )
+    obs = observe(state, 0)
+    assert jnp.all(obs == init_obs)
+
+    state = state.replace(
+        dealer=jnp.int8(1),
+        current_player=jnp.int8(3),
+        shuffled_players=jnp.array([0, 3, 1, 2], dtype=jnp.int8),
+        vul_NS=jnp.bool_(0),
+        vul_EW=jnp.bool_(1),
+    )
+    init_obs = (
+        jnp.concatenate((jnp.zeros(426, dtype=jnp.bool_), player0_hand))
+        .at[1]
+        .set(True)
+    )
+    obs = observe(state, 0)
+
+    assert jnp.all(obs == init_obs)
+
+    state = state.replace(
+        dealer=jnp.int8(1),
+        current_player=jnp.int8(3),
+        shuffled_players=jnp.array([0, 3, 1, 2], dtype=jnp.int8),
+        vul_NS=jnp.bool_(1),
+        vul_EW=jnp.bool_(1),
+    )
+    init_obs = (
+        jnp.concatenate((jnp.zeros(426, dtype=jnp.bool_), player0_hand))
+        .at[0]
+        .set(True)
+        .at[1]
+        .set(True)
+    )
+    obs = observe(state, 0)
+    assert jnp.all(obs == init_obs)
+
+    # bid_history
+    #
+    #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
+    #   0  3  1  2
+    #   N  E  S  W
+    #  -----------
+    #      P  P  P
+    #  1C 2S  X  P
+    #   P XX  P 5H
+    #  5S  P 6C  X
+    #  XX  P 7C  P
+    #   P  P
+    #
+
+    vul_history = jnp.zeros(426, dtype=jnp.bool_)
+
+    state = state.replace(
+        dealer=jnp.int8(1),
+        current_player=jnp.int8(3),
+        shuffled_players=jnp.array([0, 3, 1, 2], dtype=jnp.int8),
+        vul_NS=jnp.bool_(0),
+        vul_EW=jnp.bool_(0),
+    )
+
+    state = step(state, 35)
+    #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
+    #   0  3  1  2
+    #   N  E  S  W
+    #  -----------
+    #      P  ?
+
+    vul_history = vul_history.at[3].set(True)
+    obs = observe(state, state.current_player)
+    correct_obs = jnp.concatenate((vul_history, player1_hand))
+    assert jnp.all(obs == correct_obs)
+
+    state = step(state, 35)
+    #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
+    #   0  3  1  2
+    #   N  E  S  W
+    #  -----------
+    #      P  P  ?
+
+    vul_history = vul_history.at[4].set(True)
+    obs = observe(state, state.current_player)
+    correct_obs = jnp.concatenate((vul_history, player2_hand))
+    assert jnp.all(obs == correct_obs)
+
+    state = step(state, 35)
+    #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
+    #   0  3  1  2
+    #   N  E  S  W
+    #  -----------
+    #      P  P  P
+    #   ?
+
+    vul_history = vul_history.at[5].set(True)
+    obs = observe(state, state.current_player)
+    correct_obs = jnp.concatenate((vul_history, player0_hand))
+    assert jnp.all(obs == correct_obs)
+
+    state = step(state, 0)
+    #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
+    #   0  3  1  2
+    #   N  E  S  W
+    #  -----------
+    #      P  P  P
+    #  1C  ?
+
+    vul_history = vul_history.at[6].set(True)
+    obs = observe(state, state.current_player)
+    correct_obs = jnp.concatenate((vul_history, player3_hand))
+    assert jnp.all(obs == correct_obs)
+
+    state = step(state, 8)
+    #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
+    #   0  3  1  2
+    #   N  E  S  W
+    #  -----------
+    #      P  P  P
+    #  1C 2S  ?
+
+    vul_history = vul_history.at[49].set(True)
+    obs = observe(state, state.current_player)
+    correct_obs = jnp.concatenate((vul_history, player1_hand))
+    assert jnp.all(obs == correct_obs)
+
+    state = step(state, 36)
+    #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
+    #   0  3  1  2
+    #   N  E  S  W
+    #  -----------
+    #      P  P  P
+    #  1C 2S  X  ?
+
+    vul_history = vul_history.at[2 + 144 + 35 * 2 + 8].set(True)
+    obs = observe(state, state.current_player)
+    correct_obs = jnp.concatenate((vul_history, player2_hand))
+    assert jnp.all(obs == correct_obs)
+
+    state = step(state, 35)
+    #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
+    #   0  3  1  2
+    #   N  E  S  W
+    #  -----------
+    #      P  P  P
+    #  1C 2S  X  P
+    #   ?
+
+    obs = observe(state, state.current_player)
+    correct_obs = jnp.concatenate((vul_history, player0_hand))
+    assert jnp.all(obs == correct_obs)
+
+    state = step(state, 35)
+    #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
+    #   0  3  1  2
+    #   N  E  S  W
+    #  -----------
+    #      P  P  P
+    #  1C 2S  X  P
+    #   P  ?
+
+    obs = observe(state, state.current_player)
+    correct_obs = jnp.concatenate((vul_history, player3_hand))
+    assert jnp.all(obs == correct_obs)
+
+    state = step(state, 37)
+    #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
+    #   0  3  1  2
+    #   N  E  S  W
+    #  -----------
+    #      P  P  P
+    #  1C 2S  X  P
+    #   P XX  ?
+
+    vul_history = vul_history.at[2 + 284 + 35 + 8].set(True)
+    obs = observe(state, state.current_player)
+    correct_obs = jnp.concatenate((vul_history, player1_hand))
+    assert jnp.all(obs == correct_obs)
+
+    state = step(state, 35)
+    #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
+    #   0  3  1  2
+    #   N  E  S  W
+    #  -----------
+    #      P  P  P
+    #  1C 2S  X  P
+    #   P XX  P  ?
+
+    obs = observe(state, state.current_player)
+    correct_obs = jnp.concatenate((vul_history, player2_hand))
+    assert jnp.all(obs == correct_obs)
+
+    state = step(state, 22)
+    #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
+    #   0  3  1  2
+    #   N  E  S  W
+    #  -----------
+    #      P  P  P
+    #  1C 2S  X  P
+    #   P XX  P 5H
+    #   ?
+
+    vul_history = vul_history.at[2 + 4 + 35 * 3 + 22].set(True)
+    obs = observe(state, state.current_player)
+    correct_obs = jnp.concatenate((vul_history, player0_hand))
+    assert jnp.all(obs == correct_obs)
+
+    state = step(state, 23)
+    #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
+    #   0  3  1  2
+    #   N  E  S  W
+    #  -----------
+    #      P  P  P
+    #  1C 2S  X  P
+    #   P XX  P 5H
+    #  5S  ?
+
+    vul_history = vul_history.at[2 + 4 + 35 * 0 + 23].set(True)
+    obs = observe(state, state.current_player)
+    correct_obs = jnp.concatenate((vul_history, player3_hand))
+    assert jnp.all(obs == correct_obs)
+
+    state = step(state, 35)
+    #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
+    #   0  3  1  2
+    #   N  E  S  W
+    #  -----------
+    #      P  P  P
+    #  1C 2S  X  P
+    #   P XX  P 5H
+    #  5S  P  ?
+
+    obs = observe(state, state.current_player)
+    correct_obs = jnp.concatenate((vul_history, player1_hand))
+    assert jnp.all(obs == correct_obs)
+
+    state = step(state, 25)
+    #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
+    #   0  3  1  2
+    #   N  E  S  W
+    #  -----------
+    #      P  P  P
+    #  1C 2S  X  P
+    #   P XX  P 5H
+    #  5S  P 6C  ?
+
+    vul_history = vul_history.at[2 + 4 + 35 * 2 + 25].set(True)
+    obs = observe(state, state.current_player)
+    correct_obs = jnp.concatenate((vul_history, player2_hand))
+    assert jnp.all(obs == correct_obs)
+
+    state = step(state, 36)
+    #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
+    #   0  3  1  2
+    #   N  E  S  W
+    #  -----------
+    #      P  P  P
+    #  1C 2S  X  P
+    #   P XX  P 5H
+    #  5S  P 6C  X
+    #   ?
+
+    vul_history = vul_history.at[2 + 144 + 35 * 3 + 25].set(True)
+    obs = observe(state, state.current_player)
+    correct_obs = jnp.concatenate((vul_history, player0_hand))
+    assert jnp.all(obs == correct_obs)
+
+    state = step(state, 37)
+    #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
+    #   0  3  1  2
+    #   N  E  S  W
+    #  -----------
+    #      P  P  P
+    #  1C 2S  X  P
+    #   P XX  P 5H
+    #  5S  P 6C  X
+    #  XX  ?
+
+    vul_history = vul_history.at[2 + 284 + 35 * 0 + 25].set(True)
+    obs = observe(state, state.current_player)
+    correct_obs = jnp.concatenate((vul_history, player3_hand))
+    assert jnp.all(obs == correct_obs)
+
+    state = step(state, 35)
+    #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
+    #   0  3  1  2
+    #   N  E  S  W
+    #  -----------
+    #      P  P  P
+    #  1C 2S  X  P
+    #   P XX  P 5H
+    #  5S  P 6C  X
+    #  XX  P  ?
+
+    obs = observe(state, state.current_player)
+    correct_obs = jnp.concatenate((vul_history, player1_hand))
+    assert jnp.all(obs == correct_obs)
+
+    state = step(state, 30)
+    #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
+    #   0  3  1  2
+    #   N  E  S  W
+    #  -----------
+    #      P  P  P
+    #  1C 2S  X  P
+    #   P XX  P 5H
+    #  5S  P 6C  X
+    #  XX  P 7C  ?
+
+    vul_history = vul_history.at[2 + 4 + 35 * 2 + 30].set(True)
+    obs = observe(state, state.current_player)
+    correct_obs = jnp.concatenate((vul_history, player2_hand))
+    assert jnp.all(obs == correct_obs)
+
+    state = step(state, 35)
+    #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
+    #   0  3  1  2
+    #   N  E  S  W
+    #  -----------
+    #      P  P  P
+    #  1C 2S  X  P
+    #   P XX  P 5H
+    #  5S  P 6C  X
+    #  XX  P 7C  P
+    #   ?
+
+    obs = observe(state, state.current_player)
+    correct_obs = jnp.concatenate((vul_history, player0_hand))
+    assert jnp.all(obs == correct_obs)
+
+    state = step(state, 35)
+    #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
+    #   0  3  1  2
+    #   N  E  S  W
+    #  -----------
+    #      P  P  P
+    #  1C 2S  X  P
+    #   P XX  P 5H
+    #  5S  P 6C  X
+    #  XX  P 7C  P
+    #   P  ?
+
+    obs = observe(state, state.current_player)
+    correct_obs = jnp.concatenate((vul_history, player3_hand))
+    assert jnp.all(obs == correct_obs)
+
+    state = step(state, 35)
+    #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
+    #   0  3  1  2
+    #   N  E  S  W
+    #  -----------
+    #      P  P  P
+    #  1C 2S  X  P
+    #   P XX  P 5H
+    #  5S  P 6C  X
+    #  XX  P 7C  P
+    #   P  P
+
+
 def test_calc_score():
     # http://web2.acbl.org/documentLibrary/play/InstantScorer.pdf
     #
     # SCORE_TABLE[n][taken_trick_num - bid_level - 6][m]
     # n =   0: 1 minor
     #       1: 1 major
     #       2: 1 NT
@@ -1308,14 +1724,21 @@
            13,  9, 13],
             dtype=jnp.int8,
         )
     )
     # fmt: on
 
 
+def test_api():
+    import pgx
+
+    env = pgx.make("bridge_bidding")
+    pgx.api_test(env, 10)
+
+
 def to_value(sample: list) -> jnp.ndarray:
     """Convert sample to value
     >>> sample = ['0', '1', '0', '4', '0', '13', '12', '13', '9', '13', '0', '1', '0', '4', '0', '13', '12', '13', '9', '13']
     >>> to_value(sample)
     Array([  4160, 904605,   4160, 904605], dtype=int32)
     """
     jnp_sample = jnp.array([int(s) for s in sample], dtype=np.int8).reshape(
```

### Comparing `pgx-0.2.1/tests/test_connect_four.py` & `pgx-0.3.0/tests/test_connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/tests/test_freeway.py` & `pgx-0.3.0/tests/test_freeway.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/tests/test_go.py` & `pgx-0.3.0/tests/test_go.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/tests/test_hex.py` & `pgx-0.3.0/tests/test_hex.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/tests/test_kuhn_poker.py` & `pgx-0.3.0/tests/test_kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/tests/test_leduc_holdem.py` & `pgx-0.3.0/tests/test_leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/tests/test_othello.py` & `pgx-0.3.0/tests/test_othello.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/tests/test_play2048.py` & `pgx-0.3.0/tests/test_play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/tests/test_seaquest.py` & `pgx-0.3.0/tests/test_seaquest.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/tests/test_shogi.py` & `pgx-0.3.0/tests/test_shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/tests/test_space_invaders.py` & `pgx-0.3.0/tests/test_space_invaders.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/tests/test_sparrow_mahjong.py` & `pgx-0.3.0/tests/test_sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.2.1/tests/test_tic_tac_toe.py` & `pgx-0.3.0/tests/test_tic_tac_toe.py`

 * *Files identical despite different names*

