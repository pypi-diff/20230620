# Comparing `tmp/pgx-0.8.1.tar.gz` & `tmp/pgx-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgx-0.8.1.tar", last modified: Mon Jun 12 09:53:37 2023, max compression
+gzip compressed data, was "pgx-0.9.0.tar", last modified: Tue Jun 13 10:49:52 2023, max compression
```

## Comparing `pgx-0.8.1.tar` & `pgx-0.9.0.tar`

### file list

```diff
@@ -1,151 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:37.369275 pgx-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 09:53:24.000000 pgx-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-06-12 09:53:37.369275 pgx-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14805 2023-06-12 09:53:24.000000 pgx-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:37.345275 pgx-0.8.1/pgx/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:37.349275 pgx-0.8.1/pgx/_mahjong/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_mahjong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_mahjong/_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_mahjong/_hand.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_mahjong/_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_mahjong/_meld.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_mahjong/_shanten.py
--rw-r--r--   0 runner    (1001) docker     (123)    16845 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_mahjong/_yaku.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:37.349275 pgx-0.8.1/pgx/_mahjong/cache/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_mahjong/cache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:37.349275 pgx-0.8.1/pgx/_src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/api_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:37.353275 pgx-0.8.1/pgx/_src/assets/
--rw-r--r--   0 runner    (1001) docker     (123)  2657333 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/assets/between.npy
--rw-r--r--   0 runner    (1001) docker     (123)    91982 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/assets/can_move.npy
--rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/chess_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:37.357275 pgx-0.8.1/pgx/_src/dwg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/animalshogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/gardner_chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/hex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:37.357275 pgx-0.8.1/pgx/_src/dwg/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:37.357275 pgx-0.8.1/pgx/_src/dwg/images/chess/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/chess/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/chess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/chess/bBishop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/chess/bKing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/chess/bKnight.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/chess/bPawn.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/chess/bQueen.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/chess/bRook.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/chess/wBishop.svg
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/chess/wKing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/chess/wKnight.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/chess/wPawn.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/chess/wQueen.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/chess/wRook.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:37.361275 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/
--rw-r--r--   0 runner    (1001) docker     (123)    45499 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/1p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45511 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/2p.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/3p.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/4p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/5p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/6p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/7p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15152 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/8p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/9p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/b.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/gd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/oya.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/rd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/leduc_holdem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/dwg/tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/gardner_chess_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/shogi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23844 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/_src/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/animal_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    17854 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)    38409 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    31606 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/connect_four.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:37.361275 pgx-0.8.1/pgx/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/experimental/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/experimental/gym.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/experimental/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/experimental/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)    20306 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/gardner_chess.py
--rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/hex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/leduc_holdem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:37.365275 pgx-0.8.1/pgx/minatar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/minatar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/minatar/asterix.py
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/minatar/breakout.py
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/minatar/freeway.py
--rw-r--r--   0 runner    (1001) docker     (123)    25161 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/minatar/seaquest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/minatar/space_invaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/minatar/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)    20357 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    21398 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/tic_tac_toe.py
--rw-r--r--   0 runner    (1001) docker     (123)    14399 2023-06-12 09:53:24.000000 pgx-0.8.1/pgx/v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:37.345275 pgx-0.8.1/pgx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-06-12 09:53:37.000000 pgx-0.8.1/pgx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-06-12 09:53:37.000000 pgx-0.8.1/pgx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 09:53:37.000000 pgx-0.8.1/pgx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-12 09:53:37.000000 pgx-0.8.1/pgx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 09:53:37.000000 pgx-0.8.1/pgx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-12 09:53:24.000000 pgx-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 09:53:37.369275 pgx-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-12 09:53:24.000000 pgx-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:37.369275 pgx-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/minatar_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_animal_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_asterix.py
--rw-r--r--   0 runner    (1001) docker     (123)    17919 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_breakout.py
--rw-r--r--   0 runner    (1001) docker     (123)    75241 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    46618 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_freeway.py
--rw-r--r--   0 runner    (1001) docker     (123)    41511 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_gardner_chess.py
--rw-r--r--   0 runner    (1001) docker     (123)    39841 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_go.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_hex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_leduc_holdem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_seaquest.py
--rw-r--r--   0 runner    (1001) docker     (123)    17459 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_space_invaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    22440 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-06-12 09:53:24.000000 pgx-0.8.1/tests/test_tic_tac_toe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:49:52.200594 pgx-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 10:49:41.000000 pgx-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15750 2023-06-13 10:49:52.200594 pgx-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15294 2023-06-13 10:49:41.000000 pgx-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:49:52.184594 pgx-0.9.0/pgx/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:49:52.188594 pgx-0.9.0/pgx/_mahjong/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_mahjong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_mahjong/_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_mahjong/_hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_mahjong/_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_mahjong/_meld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_mahjong/_shanten.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16845 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_mahjong/_yaku.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:49:52.188594 pgx-0.9.0/pgx/_mahjong/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_mahjong/cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:49:52.188594 pgx-0.9.0/pgx/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/api_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:49:52.192594 pgx-0.9.0/pgx/_src/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)  2657333 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/assets/between.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    91982 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/assets/can_move.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/chess_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:49:52.192594 pgx-0.9.0/pgx/_src/dwg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/animalshogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/gardner_chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/hex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:49:52.192594 pgx-0.9.0/pgx/_src/dwg/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:49:52.196594 pgx-0.9.0/pgx/_src/dwg/images/chess/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/chess/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/chess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/chess/bBishop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/chess/bKing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/chess/bKnight.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/chess/bPawn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/chess/bQueen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/chess/bRook.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/chess/wBishop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/chess/wKing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/chess/wKnight.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/chess/wPawn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/chess/wQueen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/chess/wRook.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:49:52.196594 pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/
+-rw-r--r--   0 runner    (1001) docker     (123)    45499 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/1p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45511 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/2p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/3p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/4p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/5p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/6p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/7p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15152 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/8p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/9p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/gd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/oya.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/rd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/dwg/tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/gardner_chess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/shogi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24056 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/_src/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/animal_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38409 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31606 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/connect_four.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:49:52.196594 pgx-0.9.0/pgx/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/experimental/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/experimental/gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/experimental/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/experimental/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20306 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/gardner_chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20357 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21396 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/tic_tac_toe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15958 2023-06-13 10:49:41.000000 pgx-0.9.0/pgx/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:49:52.188594 pgx-0.9.0/pgx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15750 2023-06-13 10:49:52.000000 pgx-0.9.0/pgx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-06-13 10:49:52.000000 pgx-0.9.0/pgx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 10:49:52.000000 pgx-0.9.0/pgx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-13 10:49:52.000000 pgx-0.9.0/pgx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-13 10:49:52.000000 pgx-0.9.0/pgx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-13 10:49:41.000000 pgx-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 10:49:52.200594 pgx-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-13 10:49:41.000000 pgx-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 10:49:52.200594 pgx-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 10:49:41.000000 pgx-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-06-13 10:49:41.000000 pgx-0.9.0/tests/test_animal_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17919 2023-06-13 10:49:41.000000 pgx-0.9.0/tests/test_backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-13 10:49:41.000000 pgx-0.9.0/tests/test_baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75241 2023-06-13 10:49:41.000000 pgx-0.9.0/tests/test_bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46618 2023-06-13 10:49:41.000000 pgx-0.9.0/tests/test_chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-06-13 10:49:41.000000 pgx-0.9.0/tests/test_connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41511 2023-06-13 10:49:41.000000 pgx-0.9.0/tests/test_gardner_chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39841 2023-06-13 10:49:41.000000 pgx-0.9.0/tests/test_go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-13 10:49:41.000000 pgx-0.9.0/tests/test_hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-06-13 10:49:41.000000 pgx-0.9.0/tests/test_kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-13 10:49:41.000000 pgx-0.9.0/tests/test_leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-06-13 10:49:41.000000 pgx-0.9.0/tests/test_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-13 10:49:41.000000 pgx-0.9.0/tests/test_othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-13 10:49:41.000000 pgx-0.9.0/tests/test_play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17459 2023-06-13 10:49:41.000000 pgx-0.9.0/tests/test_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22440 2023-06-13 10:49:41.000000 pgx-0.9.0/tests/test_sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-06-13 10:49:41.000000 pgx-0.9.0/tests/test_tic_tac_toe.py
```

### Comparing `pgx-0.8.1/LICENSE` & `pgx-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/PKG-INFO` & `pgx-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgx
-Version: 0.8.1
+Version: 0.9.0
 Summary: GPU/TPU-accelerated parallel game simulators for reinforcement learning (RL)
 Home-page: https://github.com/sotetsuk/pgx
 Author: Sotetsu KOYAMADA
 Author-email: sotetsu.koyamada@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -40,14 +40,22 @@
 
 ## Installation
 
 ```sh
 pip install pgx
 ```
 
+Note that the [MinAtar](https://github.com/kenjyoung/MinAtar) suite is provided as a separate extension for Pgx ([`pgx-minatar`](https://github.com/sotetsuk/pgx-minatar)). Therefore, please run the following command additionaly to use the MinAtar suite in Pgx:
+
+```sh
+pip install pgx-minatar
+```
+
+Pgx is provided under the Apache 2.0 License, but the original MinAtar suite follows the GPL 3.0 License. Therefore, please note that the separated MinAtar extension for Pgx also adheres to the GPL 3.0 License.
+
 ## Usage
 
 
 Note that all `step` functions in Pgx environments are **JAX-native.**, i.e., they are all *JIT-able*.
 
 <a href="https://colab.research.google.com/github/sotetsuk/pgx/blob/main/colab/pgx_hello_world.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
 
@@ -109,32 +117,32 @@
 
 ```py
 >>> env.version
 ```
 
 | Game/EnvId | Visualization | Version | Five-word description |
 |:---:|:---:|:---:|:---:|
-|<a href="https://en.wikipedia.org/wiki/2048_(video_game)">2048</a> <br> `"2048"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/2048_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/2048_light.gif" width="60px">| `beta` | *Merge tiles to create 2048.* |
+|<a href="https://en.wikipedia.org/wiki/2048_(video_game)">2048</a> <br> `"2048"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/2048_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/2048_light.gif" width="60px">| `v0` | *Merge tiles to create 2048.* |
 |<a href="https://en.wikipedia.org/wiki/D%C5%8Dbutsu_sh%C5%8Dgi">Animal Shogi</a><br>`"animal_shogi"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/animal_shogi_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/animal_shogi_light.gif" width="60px">|  `v0` | *Animal-themed child-friendly shogi.* |
-|<a href="https://en.wikipedia.org/wiki/Backgammon">Backgammon</a><br>`"backgammon"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/backgammon_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/backgammon_light.gif" width="60px">| `beta` | *Luck aids bearing off checkers.* |
+|<a href="https://en.wikipedia.org/wiki/Backgammon">Backgammon</a><br>`"backgammon"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/backgammon_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/backgammon_light.gif" width="60px">| `v0` | *Luck aids bearing off checkers.* |
 |<a href="https://en.wikipedia.org/wiki/Chess">Chess</a><br>`"chess"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_light.gif" width="60px">| `v0` | *Checkmate opponent's king to win.* |
 |<a href="https://en.wikipedia.org/wiki/Connect_Four">Connect Four</a><br>`"connect_four"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/connect_four_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/connect_four_light.gif" width="60px">| `v0` | *Connect discs, win with four.* |
 |<a href="https://en.wikipedia.org/wiki/Minichess">Gardner Chess</a><br>`"gardner_chess"`|<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/gardner_chess_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/gardner_chess_light.gif" width="60px">| `v0` | *5x5 chess variant, excluding castling.* |
 |<a href="https://en.wikipedia.org/wiki/Go_(game)">Go</a><br>`"go_9x9"` `"go_19x19"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_light.gif" width="60px">| `v0` | *Strategically place stones, claim territory.* |
 |<a href="https://en.wikipedia.org/wiki/Hex_(board_game)">Hex</a><br>`"hex"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/hex_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/hex_light.gif" width="60px">| `v0` | *Connect opposite sides, block opponent.* |
-|<a href="https://en.wikipedia.org/wiki/Kuhn_poker">Kuhn Poker</a><br>`"kuhn_poker"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/kuhn_poker_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/kuhn_poker_light.gif" width="60px">| `beta` | *Three-card betting and bluffing game.* |
-|<a href="https://arxiv.org/abs/1207.1411">Leduc hold'em</a><br>`"leduc_holdem"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/leduc_holdem_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/leduc_holdem_light.gif" width="60px">| `beta` | *Two-suit, limited deck poker.* |
-|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Asterix</a><br>`"minatar-asterix"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-asterix.gif" width="50px">| `beta` | *Avoid enemies, collect treasure, survive.* |
-|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Breakout</a><br>`"minatar-breakout"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-breakout.gif" width="50px">| `beta` | *Paddle, ball, bricks, bounce, clear.* |
-|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Freeway</a><br>`"minatar-freeway"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-freeway.gif" width="50px">| `beta` | *Dodging cars, climbing up freeway.* |
-|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Seaquest</a><br>`"minatar-seaquest"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-seaquest.gif" width="50px">| `beta` | *Underwater submarine rescue and combat.* |
-|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/SpaceInvaders</a><br>`"minatar-space_invaders"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-space_invaders.gif" width="50px">| `beta` | *Alien shooter game, dodge bullets.* |
+|<a href="https://en.wikipedia.org/wiki/Kuhn_poker">Kuhn Poker</a><br>`"kuhn_poker"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/kuhn_poker_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/kuhn_poker_light.gif" width="60px">| `v0` | *Three-card betting and bluffing game.* |
+|<a href="https://arxiv.org/abs/1207.1411">Leduc hold'em</a><br>`"leduc_holdem"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/leduc_holdem_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/leduc_holdem_light.gif" width="60px">| `v0` | *Two-suit, limited deck poker.* |
+|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Asterix</a><br>`"minatar-asterix"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-asterix.gif" width="50px">| `v0` | *Avoid enemies, collect treasure, survive.* |
+|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Breakout</a><br>`"minatar-breakout"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-breakout.gif" width="50px">| `v0` | *Paddle, ball, bricks, bounce, clear.* |
+|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Freeway</a><br>`"minatar-freeway"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-freeway.gif" width="50px">| `v0` | *Dodging cars, climbing up freeway.* |
+|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Seaquest</a><br>`"minatar-seaquest"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-seaquest.gif" width="50px">| `v0` | *Underwater submarine rescue and combat.* |
+|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/SpaceInvaders</a><br>`"minatar-space_invaders"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-space_invaders.gif" width="50px">| `v0` | *Alien shooter game, dodge bullets.* |
 |<a href="https://en.wikipedia.org/wiki/Reversi">Othello</a><br>`"othello"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/othello_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/othello_light.gif" width="60px">| `v0` | *Flip and conquer opponent's pieces.* |
 |<a href="https://en.wikipedia.org/wiki/Shogi">Shogi</a><br>`"shogi"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_light.gif" width="60px"> | `v0` | *Japanese chess with captured pieces.* |
-|<a href="https://sugorokuya.jp/p/suzume-jong">Sparrow Mahjong</a><br>`"sparrow_mahjong"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/sparrow_mahjong_dark.svg" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/sparrow_mahjong_light.svg" width="60px">|  `beta` | *A simplified, children-friendly Mahjong.* |
+|<a href="https://sugorokuya.jp/p/suzume-jong">Sparrow Mahjong</a><br>`"sparrow_mahjong"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/sparrow_mahjong_dark.svg" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/sparrow_mahjong_light.svg" width="60px">|  `v0` | *A simplified, children-friendly Mahjong.* |
 |<a href="https://en.wikipedia.org/wiki/Tic-tac-toe">Tic-tac-toe</a><br>`"tic_tac_toe"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/tic_tac_toe_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/tic_tac_toe_light.gif" width="60px">| `v0` | *Three in a row wins.* |
 
 - <a href="https://en.wikipedia.org/wiki/Contract_bridge">Bridge Bidding</a> and <a href="https://en.wikipedia.org/wiki/Japanese_mahjong">Mahjong</a> environments are under development 🚧
 - Five-word descriptions were generated by [ChatGPT](https://chat.openai.com/) 🤖
 
 
 ## See also
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pgx Version: 0.8.1 Summary: GPU/TPU-accelerated
+Metadata-Version: 2.1 Name: pgx Version: 0.9.0 Summary: GPU/TPU-accelerated
 parallel game simulators for reinforcement learning (RL) Home-page: https://
 github.com/sotetsuk/pgx Author: Sotetsu KOYAMADA Author-email:
 sotetsu.koyamada@gmail.com Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown License-
 File: LICENSE [![ci](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml/
 badge.svg)](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml)
@@ -22,55 +22,61 @@
 github.com/google/jax)-native physics engine, provides extremely high-speed
 parallel simulation for RL in *continuous* state space. Then, what about RL in
 *discrete* state spaces like Chess, Shogi, and Go? **Pgx** provides a wide
 variety of JAX-native game simulators! Highlighted features include: - â¡
 **Super fast** in parallel execution on accelerators - ð² **Various game
 support** including **Backgammon**, **Chess**, **Shogi**, and **Go** - ð¼ï¸
 **Beautiful visualization** in SVG format ## Installation ```sh pip install pgx
-``` ## Usage Note that all `step` functions in Pgx environments are **JAX-
-native.**, i.e., they are all *JIT-able*. [Open_In_Colab] ```py import jax
-import pgx env = pgx.make("go_19x19") init = jax.jit(jax.vmap(env.init)) #
-vectorize and JIT-compile step = jax.jit(jax.vmap(env.step)) batch_size = 1024
-keys = jax.random.split(jax.random.PRNGKey(42), batch_size) state = init(keys)
-# vectorized states while not (state.terminated | state.truncated).all():
-action = model(state.current_player, state.observation,
-state.legal_action_mask) state = step(state, action) # state.reward (2,) ```
-Pgx is a library that focuses on faster implementations rather than just the
-API itself. However, the API itself is also sufficiently general. For example,
-all environments in Pgx can be converted to the AEC API of [PettingZoo](https:/
-/github.com/Farama-Foundation/PettingZoo), and you can run Pgx environments
-through the PettingZoo API. You can see the demonstration in Google Colab:
-[Open_In_Colab]  ## Supported games | Backgammon | Chess | Shogi | Go | |:---:
-|:---:|:---:|:---:| |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/backgammon_dark.gif#gh-dark-mode-only][https://
-raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
-backgammon_light.gif#gh-light-mode-only]|[https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-dark-mode-only][https://
-raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_light.gif#gh-
-light-mode-only]|[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/shogi_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/shogi_light.gif#gh-light-mode-only]|[https://
-raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_dark.gif#gh-
+``` Note that the [MinAtar](https://github.com/kenjyoung/MinAtar) suite is
+provided as a separate extension for Pgx ([`pgx-minatar`](https://github.com/
+sotetsuk/pgx-minatar)). Therefore, please run the following command additionaly
+to use the MinAtar suite in Pgx: ```sh pip install pgx-minatar ``` Pgx is
+provided under the Apache 2.0 License, but the original MinAtar suite follows
+the GPL 3.0 License. Therefore, please note that the separated MinAtar
+extension for Pgx also adheres to the GPL 3.0 License. ## Usage Note that all
+`step` functions in Pgx environments are **JAX-native.**, i.e., they are all
+*JIT-able*. [Open_In_Colab] ```py import jax import pgx env = pgx.make
+("go_19x19") init = jax.jit(jax.vmap(env.init)) # vectorize and JIT-compile
+step = jax.jit(jax.vmap(env.step)) batch_size = 1024 keys = jax.random.split
+(jax.random.PRNGKey(42), batch_size) state = init(keys) # vectorized states
+while not (state.terminated | state.truncated).all(): action = model
+(state.current_player, state.observation, state.legal_action_mask) state = step
+(state, action) # state.reward (2,) ``` Pgx is a library that focuses on faster
+implementations rather than just the API itself. However, the API itself is
+also sufficiently general. For example, all environments in Pgx can be
+converted to the AEC API of [PettingZoo](https://github.com/Farama-Foundation/
+PettingZoo), and you can run Pgx environments through the PettingZoo API. You
+can see the demonstration in Google Colab: [Open_In_Colab]  ## Supported games
+| Backgammon | Chess | Shogi | Go | |:---:|:---:|:---:|:---:| |[https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/backgammon_dark.gif#gh-
 dark-mode-only][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/go-19x19_light.gif#gh-light-mode-only]| Use `pgx.available_envs() -
-> Tuple[EnvId]` to see the list of currently available games. Given an ``, you
-can create the environment via ```py >>> env = pgx.make() ``` You can check the
-current version of each environment by ```py >>> env.version ``` | Game/EnvId |
-Visualization | Version | Five-word description | |:---:|:---:|:---:|:---:
-| |2048
+assets/backgammon_light.gif#gh-light-mode-only]|[https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-dark-
+mode-only][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
+chess_light.gif#gh-light-mode-only]|[https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/shogi_dark.gif#gh-dark-mode-only][https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_light.gif#gh-
+light-mode-only]|[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
+assets/go-19x19_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/go-19x19_light.gif#gh-light-mode-only]| Use
+`pgx.available_envs() -> Tuple[EnvId]` to see the list of currently available
+games. Given an ``, you can create the environment via ```py >>> env = pgx.make
+() ``` You can check the current version of each environment by ```py >>>
+env.version ``` | Game/EnvId | Visualization | Version | Five-word description
+| |:---:|:---:|:---:|:---:| |2048
 `"2048"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 2048_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
-2048_light.gif]| `beta` | *Merge tiles to create 2048.* | |Animal_Shogi
+2048_light.gif]| `v0` | *Merge tiles to create 2048.* | |Animal_Shogi
 `"animal_shogi"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/animal_shogi_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
 main/docs/assets/animal_shogi_light.gif]| `v0` | *Animal-themed child-friendly
 shogi.* | |Backgammon
 `"backgammon"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/backgammon_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
-main/docs/assets/backgammon_light.gif]| `beta` | *Luck aids bearing off
+main/docs/assets/backgammon_light.gif]| `v0` | *Luck aids bearing off
 checkers.* | |Chess
 `"chess"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 chess_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/chess_light.gif]| `v0` | *Checkmate opponent's king to win.* | |Connect
 Four
 `"connect_four"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/connect_four_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
@@ -85,46 +91,46 @@
 main/docs/assets/go-19x19_light.gif]| `v0` | *Strategically place stones, claim
 territory.* | |Hex
 `"hex"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 hex_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 hex_light.gif]| `v0` | *Connect opposite sides, block opponent.* | |Kuhn_Poker
 `"kuhn_poker"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/kuhn_poker_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
-main/docs/assets/kuhn_poker_light.gif]| `beta` | *Three-card betting and
-bluffing game.* | |Leduc_hold'em
+main/docs/assets/kuhn_poker_light.gif]| `v0` | *Three-card betting and bluffing
+game.* | |Leduc_hold'em
 `"leduc_holdem"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/leduc_holdem_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
-main/docs/assets/leduc_holdem_light.gif]| `beta` | *Two-suit, limited deck
+main/docs/assets/leduc_holdem_light.gif]| `v0` | *Two-suit, limited deck
 poker.* | |MinAtar/Asterix
 `"minatar-asterix"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/minatar-asterix.gif]| `beta` | *Avoid enemies, collect treasure,
-survive.* | |MinAtar/Breakout
+assets/minatar-asterix.gif]| `v0` | *Avoid enemies, collect treasure, survive.*
+| |MinAtar/Breakout
 `"minatar-breakout"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/
-docs/assets/minatar-breakout.gif]| `beta` | *Paddle, ball, bricks, bounce,
+docs/assets/minatar-breakout.gif]| `v0` | *Paddle, ball, bricks, bounce,
 clear.* | |MinAtar/Freeway
 `"minatar-freeway"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/minatar-freeway.gif]| `beta` | *Dodging cars, climbing up freeway.* |
+assets/minatar-freeway.gif]| `v0` | *Dodging cars, climbing up freeway.* |
 |MinAtar/Seaquest
 `"minatar-seaquest"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/
-docs/assets/minatar-seaquest.gif]| `beta` | *Underwater submarine rescue and
+docs/assets/minatar-seaquest.gif]| `v0` | *Underwater submarine rescue and
 combat.* | |MinAtar/SpaceInvaders
 `"minatar-space_invaders"` |[https://raw.githubusercontent.com/sotetsuk/pgx/
-main/docs/assets/minatar-space_invaders.gif]| `beta` | *Alien shooter game,
-dodge bullets.* | |Othello
+main/docs/assets/minatar-space_invaders.gif]| `v0` | *Alien shooter game, dodge
+bullets.* | |Othello
 `"othello"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 othello_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/othello_light.gif]| `v0` | *Flip and conquer opponent's pieces.* |
 |Shogi
 `"shogi"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 shogi_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/shogi_light.gif] | `v0` | *Japanese chess with captured pieces.* |
 |Sparrow_Mahjong
 `"sparrow_mahjong"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/sparrow_mahjong_dark.svg][https://raw.githubusercontent.com/sotetsuk/
-pgx/main/docs/assets/sparrow_mahjong_light.svg]| `beta` | *A simplified,
+pgx/main/docs/assets/sparrow_mahjong_light.svg]| `v0` | *A simplified,
 children-friendly Mahjong.* | |Tic-tac-toe
 `"tic_tac_toe"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/tic_tac_toe_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
 main/docs/assets/tic_tac_toe_light.gif]| `v0` | *Three in a row wins.* | -
 Bridge_Bidding and Mahjong environments are under development ð§ - Five-word
 descriptions were generated by [ChatGPT](https://chat.openai.com/) ð¤ ## See
 also Pgx is intended to complement these **JAX-native environments** with
```

### Comparing `pgx-0.8.1/README.md` & `pgx-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,22 @@
 
 ## Installation
 
 ```sh
 pip install pgx
 ```
 
+Note that the [MinAtar](https://github.com/kenjyoung/MinAtar) suite is provided as a separate extension for Pgx ([`pgx-minatar`](https://github.com/sotetsuk/pgx-minatar)). Therefore, please run the following command additionaly to use the MinAtar suite in Pgx:
+
+```sh
+pip install pgx-minatar
+```
+
+Pgx is provided under the Apache 2.0 License, but the original MinAtar suite follows the GPL 3.0 License. Therefore, please note that the separated MinAtar extension for Pgx also adheres to the GPL 3.0 License.
+
 ## Usage
 
 
 Note that all `step` functions in Pgx environments are **JAX-native.**, i.e., they are all *JIT-able*.
 
 <a href="https://colab.research.google.com/github/sotetsuk/pgx/blob/main/colab/pgx_hello_world.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
 
@@ -96,32 +104,32 @@
 
 ```py
 >>> env.version
 ```
 
 | Game/EnvId | Visualization | Version | Five-word description |
 |:---:|:---:|:---:|:---:|
-|<a href="https://en.wikipedia.org/wiki/2048_(video_game)">2048</a> <br> `"2048"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/2048_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/2048_light.gif" width="60px">| `beta` | *Merge tiles to create 2048.* |
+|<a href="https://en.wikipedia.org/wiki/2048_(video_game)">2048</a> <br> `"2048"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/2048_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/2048_light.gif" width="60px">| `v0` | *Merge tiles to create 2048.* |
 |<a href="https://en.wikipedia.org/wiki/D%C5%8Dbutsu_sh%C5%8Dgi">Animal Shogi</a><br>`"animal_shogi"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/animal_shogi_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/animal_shogi_light.gif" width="60px">|  `v0` | *Animal-themed child-friendly shogi.* |
-|<a href="https://en.wikipedia.org/wiki/Backgammon">Backgammon</a><br>`"backgammon"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/backgammon_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/backgammon_light.gif" width="60px">| `beta` | *Luck aids bearing off checkers.* |
+|<a href="https://en.wikipedia.org/wiki/Backgammon">Backgammon</a><br>`"backgammon"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/backgammon_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/backgammon_light.gif" width="60px">| `v0` | *Luck aids bearing off checkers.* |
 |<a href="https://en.wikipedia.org/wiki/Chess">Chess</a><br>`"chess"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_light.gif" width="60px">| `v0` | *Checkmate opponent's king to win.* |
 |<a href="https://en.wikipedia.org/wiki/Connect_Four">Connect Four</a><br>`"connect_four"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/connect_four_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/connect_four_light.gif" width="60px">| `v0` | *Connect discs, win with four.* |
 |<a href="https://en.wikipedia.org/wiki/Minichess">Gardner Chess</a><br>`"gardner_chess"`|<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/gardner_chess_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/gardner_chess_light.gif" width="60px">| `v0` | *5x5 chess variant, excluding castling.* |
 |<a href="https://en.wikipedia.org/wiki/Go_(game)">Go</a><br>`"go_9x9"` `"go_19x19"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_light.gif" width="60px">| `v0` | *Strategically place stones, claim territory.* |
 |<a href="https://en.wikipedia.org/wiki/Hex_(board_game)">Hex</a><br>`"hex"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/hex_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/hex_light.gif" width="60px">| `v0` | *Connect opposite sides, block opponent.* |
-|<a href="https://en.wikipedia.org/wiki/Kuhn_poker">Kuhn Poker</a><br>`"kuhn_poker"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/kuhn_poker_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/kuhn_poker_light.gif" width="60px">| `beta` | *Three-card betting and bluffing game.* |
-|<a href="https://arxiv.org/abs/1207.1411">Leduc hold'em</a><br>`"leduc_holdem"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/leduc_holdem_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/leduc_holdem_light.gif" width="60px">| `beta` | *Two-suit, limited deck poker.* |
-|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Asterix</a><br>`"minatar-asterix"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-asterix.gif" width="50px">| `beta` | *Avoid enemies, collect treasure, survive.* |
-|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Breakout</a><br>`"minatar-breakout"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-breakout.gif" width="50px">| `beta` | *Paddle, ball, bricks, bounce, clear.* |
-|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Freeway</a><br>`"minatar-freeway"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-freeway.gif" width="50px">| `beta` | *Dodging cars, climbing up freeway.* |
-|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Seaquest</a><br>`"minatar-seaquest"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-seaquest.gif" width="50px">| `beta` | *Underwater submarine rescue and combat.* |
-|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/SpaceInvaders</a><br>`"minatar-space_invaders"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-space_invaders.gif" width="50px">| `beta` | *Alien shooter game, dodge bullets.* |
+|<a href="https://en.wikipedia.org/wiki/Kuhn_poker">Kuhn Poker</a><br>`"kuhn_poker"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/kuhn_poker_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/kuhn_poker_light.gif" width="60px">| `v0` | *Three-card betting and bluffing game.* |
+|<a href="https://arxiv.org/abs/1207.1411">Leduc hold'em</a><br>`"leduc_holdem"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/leduc_holdem_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/leduc_holdem_light.gif" width="60px">| `v0` | *Two-suit, limited deck poker.* |
+|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Asterix</a><br>`"minatar-asterix"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-asterix.gif" width="50px">| `v0` | *Avoid enemies, collect treasure, survive.* |
+|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Breakout</a><br>`"minatar-breakout"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-breakout.gif" width="50px">| `v0` | *Paddle, ball, bricks, bounce, clear.* |
+|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Freeway</a><br>`"minatar-freeway"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-freeway.gif" width="50px">| `v0` | *Dodging cars, climbing up freeway.* |
+|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Seaquest</a><br>`"minatar-seaquest"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-seaquest.gif" width="50px">| `v0` | *Underwater submarine rescue and combat.* |
+|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/SpaceInvaders</a><br>`"minatar-space_invaders"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-space_invaders.gif" width="50px">| `v0` | *Alien shooter game, dodge bullets.* |
 |<a href="https://en.wikipedia.org/wiki/Reversi">Othello</a><br>`"othello"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/othello_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/othello_light.gif" width="60px">| `v0` | *Flip and conquer opponent's pieces.* |
 |<a href="https://en.wikipedia.org/wiki/Shogi">Shogi</a><br>`"shogi"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_light.gif" width="60px"> | `v0` | *Japanese chess with captured pieces.* |
-|<a href="https://sugorokuya.jp/p/suzume-jong">Sparrow Mahjong</a><br>`"sparrow_mahjong"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/sparrow_mahjong_dark.svg" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/sparrow_mahjong_light.svg" width="60px">|  `beta` | *A simplified, children-friendly Mahjong.* |
+|<a href="https://sugorokuya.jp/p/suzume-jong">Sparrow Mahjong</a><br>`"sparrow_mahjong"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/sparrow_mahjong_dark.svg" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/sparrow_mahjong_light.svg" width="60px">|  `v0` | *A simplified, children-friendly Mahjong.* |
 |<a href="https://en.wikipedia.org/wiki/Tic-tac-toe">Tic-tac-toe</a><br>`"tic_tac_toe"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/tic_tac_toe_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/tic_tac_toe_light.gif" width="60px">| `v0` | *Three in a row wins.* |
 
 - <a href="https://en.wikipedia.org/wiki/Contract_bridge">Bridge Bidding</a> and <a href="https://en.wikipedia.org/wiki/Japanese_mahjong">Mahjong</a> environments are under development 🚧
 - Five-word descriptions were generated by [ChatGPT](https://chat.openai.com/) 🤖
 
 
 ## See also
```

#### html2text {}

```diff
@@ -16,55 +16,61 @@
 github.com/google/jax)-native physics engine, provides extremely high-speed
 parallel simulation for RL in *continuous* state space. Then, what about RL in
 *discrete* state spaces like Chess, Shogi, and Go? **Pgx** provides a wide
 variety of JAX-native game simulators! Highlighted features include: - â¡
 **Super fast** in parallel execution on accelerators - ð² **Various game
 support** including **Backgammon**, **Chess**, **Shogi**, and **Go** - ð¼ï¸
 **Beautiful visualization** in SVG format ## Installation ```sh pip install pgx
-``` ## Usage Note that all `step` functions in Pgx environments are **JAX-
-native.**, i.e., they are all *JIT-able*. [Open_In_Colab] ```py import jax
-import pgx env = pgx.make("go_19x19") init = jax.jit(jax.vmap(env.init)) #
-vectorize and JIT-compile step = jax.jit(jax.vmap(env.step)) batch_size = 1024
-keys = jax.random.split(jax.random.PRNGKey(42), batch_size) state = init(keys)
-# vectorized states while not (state.terminated | state.truncated).all():
-action = model(state.current_player, state.observation,
-state.legal_action_mask) state = step(state, action) # state.reward (2,) ```
-Pgx is a library that focuses on faster implementations rather than just the
-API itself. However, the API itself is also sufficiently general. For example,
-all environments in Pgx can be converted to the AEC API of [PettingZoo](https:/
-/github.com/Farama-Foundation/PettingZoo), and you can run Pgx environments
-through the PettingZoo API. You can see the demonstration in Google Colab:
-[Open_In_Colab]  ## Supported games | Backgammon | Chess | Shogi | Go | |:---:
-|:---:|:---:|:---:| |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/backgammon_dark.gif#gh-dark-mode-only][https://
-raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
-backgammon_light.gif#gh-light-mode-only]|[https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-dark-mode-only][https://
-raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_light.gif#gh-
-light-mode-only]|[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/shogi_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/shogi_light.gif#gh-light-mode-only]|[https://
-raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_dark.gif#gh-
+``` Note that the [MinAtar](https://github.com/kenjyoung/MinAtar) suite is
+provided as a separate extension for Pgx ([`pgx-minatar`](https://github.com/
+sotetsuk/pgx-minatar)). Therefore, please run the following command additionaly
+to use the MinAtar suite in Pgx: ```sh pip install pgx-minatar ``` Pgx is
+provided under the Apache 2.0 License, but the original MinAtar suite follows
+the GPL 3.0 License. Therefore, please note that the separated MinAtar
+extension for Pgx also adheres to the GPL 3.0 License. ## Usage Note that all
+`step` functions in Pgx environments are **JAX-native.**, i.e., they are all
+*JIT-able*. [Open_In_Colab] ```py import jax import pgx env = pgx.make
+("go_19x19") init = jax.jit(jax.vmap(env.init)) # vectorize and JIT-compile
+step = jax.jit(jax.vmap(env.step)) batch_size = 1024 keys = jax.random.split
+(jax.random.PRNGKey(42), batch_size) state = init(keys) # vectorized states
+while not (state.terminated | state.truncated).all(): action = model
+(state.current_player, state.observation, state.legal_action_mask) state = step
+(state, action) # state.reward (2,) ``` Pgx is a library that focuses on faster
+implementations rather than just the API itself. However, the API itself is
+also sufficiently general. For example, all environments in Pgx can be
+converted to the AEC API of [PettingZoo](https://github.com/Farama-Foundation/
+PettingZoo), and you can run Pgx environments through the PettingZoo API. You
+can see the demonstration in Google Colab: [Open_In_Colab]  ## Supported games
+| Backgammon | Chess | Shogi | Go | |:---:|:---:|:---:|:---:| |[https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/backgammon_dark.gif#gh-
 dark-mode-only][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/go-19x19_light.gif#gh-light-mode-only]| Use `pgx.available_envs() -
-> Tuple[EnvId]` to see the list of currently available games. Given an ``, you
-can create the environment via ```py >>> env = pgx.make() ``` You can check the
-current version of each environment by ```py >>> env.version ``` | Game/EnvId |
-Visualization | Version | Five-word description | |:---:|:---:|:---:|:---:
-| |2048
+assets/backgammon_light.gif#gh-light-mode-only]|[https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-dark-
+mode-only][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
+chess_light.gif#gh-light-mode-only]|[https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/shogi_dark.gif#gh-dark-mode-only][https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_light.gif#gh-
+light-mode-only]|[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
+assets/go-19x19_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/go-19x19_light.gif#gh-light-mode-only]| Use
+`pgx.available_envs() -> Tuple[EnvId]` to see the list of currently available
+games. Given an ``, you can create the environment via ```py >>> env = pgx.make
+() ``` You can check the current version of each environment by ```py >>>
+env.version ``` | Game/EnvId | Visualization | Version | Five-word description
+| |:---:|:---:|:---:|:---:| |2048
 `"2048"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 2048_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
-2048_light.gif]| `beta` | *Merge tiles to create 2048.* | |Animal_Shogi
+2048_light.gif]| `v0` | *Merge tiles to create 2048.* | |Animal_Shogi
 `"animal_shogi"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/animal_shogi_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
 main/docs/assets/animal_shogi_light.gif]| `v0` | *Animal-themed child-friendly
 shogi.* | |Backgammon
 `"backgammon"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/backgammon_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
-main/docs/assets/backgammon_light.gif]| `beta` | *Luck aids bearing off
+main/docs/assets/backgammon_light.gif]| `v0` | *Luck aids bearing off
 checkers.* | |Chess
 `"chess"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 chess_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/chess_light.gif]| `v0` | *Checkmate opponent's king to win.* | |Connect
 Four
 `"connect_four"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/connect_four_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
@@ -79,46 +85,46 @@
 main/docs/assets/go-19x19_light.gif]| `v0` | *Strategically place stones, claim
 territory.* | |Hex
 `"hex"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 hex_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 hex_light.gif]| `v0` | *Connect opposite sides, block opponent.* | |Kuhn_Poker
 `"kuhn_poker"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/kuhn_poker_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
-main/docs/assets/kuhn_poker_light.gif]| `beta` | *Three-card betting and
-bluffing game.* | |Leduc_hold'em
+main/docs/assets/kuhn_poker_light.gif]| `v0` | *Three-card betting and bluffing
+game.* | |Leduc_hold'em
 `"leduc_holdem"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/leduc_holdem_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
-main/docs/assets/leduc_holdem_light.gif]| `beta` | *Two-suit, limited deck
+main/docs/assets/leduc_holdem_light.gif]| `v0` | *Two-suit, limited deck
 poker.* | |MinAtar/Asterix
 `"minatar-asterix"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/minatar-asterix.gif]| `beta` | *Avoid enemies, collect treasure,
-survive.* | |MinAtar/Breakout
+assets/minatar-asterix.gif]| `v0` | *Avoid enemies, collect treasure, survive.*
+| |MinAtar/Breakout
 `"minatar-breakout"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/
-docs/assets/minatar-breakout.gif]| `beta` | *Paddle, ball, bricks, bounce,
+docs/assets/minatar-breakout.gif]| `v0` | *Paddle, ball, bricks, bounce,
 clear.* | |MinAtar/Freeway
 `"minatar-freeway"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/minatar-freeway.gif]| `beta` | *Dodging cars, climbing up freeway.* |
+assets/minatar-freeway.gif]| `v0` | *Dodging cars, climbing up freeway.* |
 |MinAtar/Seaquest
 `"minatar-seaquest"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/
-docs/assets/minatar-seaquest.gif]| `beta` | *Underwater submarine rescue and
+docs/assets/minatar-seaquest.gif]| `v0` | *Underwater submarine rescue and
 combat.* | |MinAtar/SpaceInvaders
 `"minatar-space_invaders"` |[https://raw.githubusercontent.com/sotetsuk/pgx/
-main/docs/assets/minatar-space_invaders.gif]| `beta` | *Alien shooter game,
-dodge bullets.* | |Othello
+main/docs/assets/minatar-space_invaders.gif]| `v0` | *Alien shooter game, dodge
+bullets.* | |Othello
 `"othello"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 othello_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/othello_light.gif]| `v0` | *Flip and conquer opponent's pieces.* |
 |Shogi
 `"shogi"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 shogi_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/shogi_light.gif] | `v0` | *Japanese chess with captured pieces.* |
 |Sparrow_Mahjong
 `"sparrow_mahjong"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/sparrow_mahjong_dark.svg][https://raw.githubusercontent.com/sotetsuk/
-pgx/main/docs/assets/sparrow_mahjong_light.svg]| `beta` | *A simplified,
+pgx/main/docs/assets/sparrow_mahjong_light.svg]| `v0` | *A simplified,
 children-friendly Mahjong.* | |Tic-tac-toe
 `"tic_tac_toe"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/tic_tac_toe_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
 main/docs/assets/tic_tac_toe_light.gif]| `v0` | *Three in a row wins.* | -
 Bridge_Bidding and Mahjong environments are under development ð§ - Five-word
 descriptions were generated by [ChatGPT](https://chat.openai.com/) ð¤ ## See
 also Pgx is intended to complement these **JAX-native environments** with
```

### Comparing `pgx-0.8.1/pgx/_mahjong/_hand.py` & `pgx-0.9.0/pgx/_mahjong/_hand.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_mahjong/_mahjong.py` & `pgx-0.9.0/pgx/_mahjong/_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_mahjong/_meld.py` & `pgx-0.9.0/pgx/_mahjong/_meld.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_mahjong/_shanten.py` & `pgx-0.9.0/pgx/_mahjong/_shanten.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_mahjong/_yaku.py` & `pgx-0.9.0/pgx/_mahjong/_yaku.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/api_test.py` & `pgx-0.9.0/pgx/_src/api_test.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/assets/between.npy` & `pgx-0.9.0/pgx/_src/assets/between.npy`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/assets/can_move.npy` & `pgx-0.9.0/pgx/_src/assets/can_move.npy`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/chess_utils.py` & `pgx-0.9.0/pgx/_src/chess_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/animalshogi.py` & `pgx-0.9.0/pgx/_src/dwg/animalshogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/backgammon.py` & `pgx-0.9.0/pgx/_src/dwg/backgammon.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/bridge_bidding.py` & `pgx-0.9.0/pgx/_src/dwg/bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/chess.py` & `pgx-0.9.0/pgx/_src/dwg/chess.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/connect_four.py` & `pgx-0.9.0/pgx/_src/dwg/connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/gardner_chess.py` & `pgx-0.9.0/pgx/_src/dwg/gardner_chess.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/go.py` & `pgx-0.9.0/pgx/_src/dwg/go.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/hex.py` & `pgx-0.9.0/pgx/_src/dwg/hex.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/chess/LICENSE` & `pgx-0.9.0/pgx/_src/dwg/images/chess/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/chess/bBishop.svg` & `pgx-0.9.0/pgx/_src/dwg/images/chess/bBishop.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/chess/bKing.svg` & `pgx-0.9.0/pgx/_src/dwg/images/chess/bKing.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/chess/bKnight.svg` & `pgx-0.9.0/pgx/_src/dwg/images/chess/bKnight.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/chess/bPawn.svg` & `pgx-0.9.0/pgx/_src/dwg/images/chess/bPawn.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/chess/bQueen.svg` & `pgx-0.9.0/pgx/_src/dwg/images/chess/bQueen.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/chess/bRook.svg` & `pgx-0.9.0/pgx/_src/dwg/images/chess/bRook.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/chess/wBishop.svg` & `pgx-0.9.0/pgx/_src/dwg/images/chess/wBishop.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/chess/wKing.svg` & `pgx-0.9.0/pgx/_src/dwg/images/chess/wKing.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/chess/wKnight.svg` & `pgx-0.9.0/pgx/_src/dwg/images/chess/wKnight.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/chess/wPawn.svg` & `pgx-0.9.0/pgx/_src/dwg/images/chess/wPawn.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/chess/wQueen.svg` & `pgx-0.9.0/pgx/_src/dwg/images/chess/wQueen.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/chess/wRook.svg` & `pgx-0.9.0/pgx/_src/dwg/images/chess/wRook.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/1p.svg` & `pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/1p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg` & `pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/2p.svg` & `pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/2p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg` & `pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/3p.svg` & `pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/3p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg` & `pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/4p.svg` & `pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/4p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg` & `pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/5p.svg` & `pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/5p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg` & `pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/6p.svg` & `pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/6p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg` & `pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/7p.svg` & `pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/7p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg` & `pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/8p.svg` & `pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/8p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg` & `pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/9p.svg` & `pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/9p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg` & `pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/b.svg` & `pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/b.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/gd.svg` & `pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/gd.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/oya.svg` & `pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/oya.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/images/sparrow_mahjong/rd.svg` & `pgx-0.9.0/pgx/_src/dwg/images/sparrow_mahjong/rd.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/kuhn_poker.py` & `pgx-0.9.0/pgx/_src/dwg/kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/leduc_holdem.py` & `pgx-0.9.0/pgx/_src/dwg/leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/othello.py` & `pgx-0.9.0/pgx/_src/dwg/othello.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/play2048.py` & `pgx-0.9.0/pgx/_src/dwg/play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/shogi.py` & `pgx-0.9.0/pgx/_src/dwg/shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/sparrow_mahjong.py` & `pgx-0.9.0/pgx/_src/dwg/sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/dwg/tictactoe.py` & `pgx-0.9.0/pgx/_src/dwg/tictactoe.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/gardner_chess_utils.py` & `pgx-0.9.0/pgx/_src/gardner_chess_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/shogi_utils.py` & `pgx-0.9.0/pgx/_src/shogi_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/struct.py` & `pgx-0.9.0/pgx/_src/struct.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/_src/visualizer.py` & `pgx-0.9.0/pgx/_src/visualizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -649,33 +649,39 @@
             assert False
 
     def _get_nth_state(self, states: State, i):
         return jax.tree_util.tree_map(lambda x: x[i], states)
 
 
 def save_svg(
-    states: State,
+    state: State,
     filename: Union[str, Path],
     *,
     color_theme: Optional[Literal["light", "dark"]] = None,
     scale: Optional[float] = None,
 ) -> None:
     assert str(filename).endswith(".svg")
-    v = Visualizer(color_theme=color_theme, scale=scale)
-    v.get_dwg(states=states).saveas(filename)
+    if state.env_id.startswith("minatar"):
+        state.save_svg(filename=filename)
+    else:
+        v = Visualizer(color_theme=color_theme, scale=scale)
+        v.get_dwg(states=state).saveas(filename)
 
 
 def save_svg_animation(
     states: Sequence[State],
     filename: Union[str, Path],
     *,
     color_theme: Optional[Literal["light", "dark"]] = None,
     scale: Optional[float] = None,
     frame_duration_seconds: Optional[float] = None,
 ) -> None:
+    assert not states[0].env_id.startswith(
+        "minatar"
+    ), "MinAtar does not support svg animation."
     assert str(filename).endswith(".svg")
     v = Visualizer(color_theme=color_theme, scale=scale)
 
     if frame_duration_seconds is None:
         frame_duration_seconds = global_config.frame_duration_seconds
 
     frame_groups = []
```

### Comparing `pgx-0.8.1/pgx/animal_shogi.py` & `pgx-0.9.0/pgx/animal_shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/backgammon.py` & `pgx-0.9.0/pgx/backgammon.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
     @property
     def id(self) -> v1.EnvId:
         return "backgammon"
 
     @property
     def version(self) -> str:
-        return "beta"
+        return "v0"
 
     @property
     def num_players(self) -> int:
         return 2
 
     @property
     def _illegal_action_penalty(self) -> float:
```

### Comparing `pgx-0.8.1/pgx/baseline.py` & `pgx-0.9.0/pgx/baseline.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/bridge_bidding.py` & `pgx-0.9.0/pgx/bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/chess.py` & `pgx-0.9.0/pgx/chess.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/connect_four.py` & `pgx-0.9.0/pgx/connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/experimental/bridge_bidding.py` & `pgx-0.9.0/pgx/experimental/bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/experimental/gym.py` & `pgx-0.9.0/pgx/experimental/gym.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/experimental/visualize.py` & `pgx-0.9.0/pgx/experimental/visualize.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/gardner_chess.py` & `pgx-0.9.0/pgx/gardner_chess.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/go.py` & `pgx-0.9.0/pgx/go.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/hex.py` & `pgx-0.9.0/pgx/hex.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/kuhn_poker.py` & `pgx-0.9.0/pgx/kuhn_poker.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
     @property
     def id(self) -> v1.EnvId:
         return "kuhn_poker"
 
     @property
     def version(self) -> str:
-        return "beta"
+        return "v0"
 
     @property
     def num_players(self) -> int:
         return 2
 
 
 def _init(rng: jax.random.KeyArray) -> State:
```

### Comparing `pgx-0.8.1/pgx/leduc_holdem.py` & `pgx-0.9.0/pgx/leduc_holdem.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
     @property
     def id(self) -> v1.EnvId:
         return "leduc_holdem"
 
     @property
     def version(self) -> str:
-        return "beta"
+        return "v0"
 
     @property
     def num_players(self) -> int:
         return 2
 
 
 def _init(rng: jax.random.KeyArray) -> State:
```

### Comparing `pgx-0.8.1/pgx/othello.py` & `pgx-0.9.0/pgx/othello.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/play2048.py` & `pgx-0.9.0/pgx/play2048.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
     @property
     def id(self) -> v1.EnvId:
         return "2048"
 
     @property
     def version(self) -> str:
-        return "beta"
+        return "v0"
 
     @property
     def num_players(self) -> int:
         return 1
 
 
 def _init(rng: jax.random.KeyArray) -> State:
```

### Comparing `pgx-0.8.1/pgx/shogi.py` & `pgx-0.9.0/pgx/shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/sparrow_mahjong.py` & `pgx-0.9.0/pgx/sparrow_mahjong.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
 
     @property
     def id(self) -> v1.EnvId:
         return "sparrow_mahjong"
 
     @property
     def version(self) -> str:
-        return "beta"
+        return "v0"
 
     @property
     def num_players(self) -> int:
         return 3
 
 
 def _init(rng: jax.random.KeyArray):
```

### Comparing `pgx-0.8.1/pgx/tic_tac_toe.py` & `pgx-0.9.0/pgx/tic_tac_toe.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/pgx/v1.py` & `pgx-0.9.0/pgx/v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import abc
+import sys
 from typing import Literal, Optional, Tuple, get_args
 
 import jax
 import jax.numpy as jnp
 
 from pgx._src.struct import dataclass
 
@@ -383,33 +384,66 @@
 
         return KuhnPoker()
     elif env_id == "leduc_holdem":
         from pgx.leduc_holdem import LeducHoldem
 
         return LeducHoldem()
     elif env_id == "minatar-asterix":
-        from pgx.minatar.asterix import MinAtarAsterix
+        try:
+            from pgx_minatar.asterix import MinAtarAsterix  # type: ignore
+
+            return MinAtarAsterix()
+        except ModuleNotFoundError:
+            print(
+                '"minatar-asterix" environment is provided as a separate plugin of Pgx.\nPlease run `$ pip install pgx-minatar` to use this environment in Pgx.',
+                file=sys.stderr,
+            )
 
-        return MinAtarAsterix()
     elif env_id == "minatar-breakout":
-        from pgx.minatar.breakout import MinAtarBreakout
+        try:
+            from pgx_minatar.breakout import MinAtarBreakout  # type: ignore
 
-        return MinAtarBreakout()
+            return MinAtarBreakout()
+        except ModuleNotFoundError:
+            print(
+                '"minatar-breakout" environment is provided as a separate plugin of Pgx.\nPlease run `$ pip install pgx-minatar` to use this environment in Pgx.',
+                file=sys.stderr,
+            )
     elif env_id == "minatar-freeway":
-        from pgx.minatar.freeway import MinAtarFreeway
+        try:
+            from pgx_minatar.freeway import MinAtarFreeway  # type: ignore
 
-        return MinAtarFreeway()
+            return MinAtarFreeway()
+        except ModuleNotFoundError:
+            print(
+                '"minatar-freeway" environment is provided as a separate plugin of Pgx.\nPlease run `$ pip install pgx-minatar` to use this environment in Pgx.',
+                file=sys.stderr,
+            )
     elif env_id == "minatar-seaquest":
-        from pgx.minatar.seaquest import MinAtarSeaquest
+        try:
+            from pgx_minatar.seaquest import MinAtarSeaquest  # type: ignore
 
-        return MinAtarSeaquest()
+            return MinAtarSeaquest()
+        except ModuleNotFoundError:
+            print(
+                '"minatar-seaquest" environment is provided as a separate plugin of Pgx.\nPlease run `$ pip install pgx-minatar` to use this environment in Pgx.',
+                file=sys.stderr,
+            )
     elif env_id == "minatar-space_invaders":
-        from pgx.minatar.space_invaders import MinAtarSpaceInvaders
-
-        return MinAtarSpaceInvaders()
+        try:
+            from pgx_minatar.space_invaders import (  # type: ignore
+                MinAtarSpaceInvaders,
+            )
+
+            return MinAtarSpaceInvaders()
+        except ModuleNotFoundError:
+            print(
+                '"minatar-space_invaders" environment is provided as a separate plugin of Pgx.\nPlease run `$ pip install pgx-minatar` to use this environment in Pgx.',
+                file=sys.stderr,
+            )
     elif env_id == "othello":
         from pgx.othello import Othello
 
         return Othello()
     elif env_id == "shogi":
         from pgx.shogi import Shogi
```

### Comparing `pgx-0.8.1/pgx.egg-info/PKG-INFO` & `pgx-0.9.0/pgx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgx
-Version: 0.8.1
+Version: 0.9.0
 Summary: GPU/TPU-accelerated parallel game simulators for reinforcement learning (RL)
 Home-page: https://github.com/sotetsuk/pgx
 Author: Sotetsu KOYAMADA
 Author-email: sotetsu.koyamada@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -40,14 +40,22 @@
 
 ## Installation
 
 ```sh
 pip install pgx
 ```
 
+Note that the [MinAtar](https://github.com/kenjyoung/MinAtar) suite is provided as a separate extension for Pgx ([`pgx-minatar`](https://github.com/sotetsuk/pgx-minatar)). Therefore, please run the following command additionaly to use the MinAtar suite in Pgx:
+
+```sh
+pip install pgx-minatar
+```
+
+Pgx is provided under the Apache 2.0 License, but the original MinAtar suite follows the GPL 3.0 License. Therefore, please note that the separated MinAtar extension for Pgx also adheres to the GPL 3.0 License.
+
 ## Usage
 
 
 Note that all `step` functions in Pgx environments are **JAX-native.**, i.e., they are all *JIT-able*.
 
 <a href="https://colab.research.google.com/github/sotetsuk/pgx/blob/main/colab/pgx_hello_world.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
 
@@ -109,32 +117,32 @@
 
 ```py
 >>> env.version
 ```
 
 | Game/EnvId | Visualization | Version | Five-word description |
 |:---:|:---:|:---:|:---:|
-|<a href="https://en.wikipedia.org/wiki/2048_(video_game)">2048</a> <br> `"2048"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/2048_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/2048_light.gif" width="60px">| `beta` | *Merge tiles to create 2048.* |
+|<a href="https://en.wikipedia.org/wiki/2048_(video_game)">2048</a> <br> `"2048"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/2048_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/2048_light.gif" width="60px">| `v0` | *Merge tiles to create 2048.* |
 |<a href="https://en.wikipedia.org/wiki/D%C5%8Dbutsu_sh%C5%8Dgi">Animal Shogi</a><br>`"animal_shogi"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/animal_shogi_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/animal_shogi_light.gif" width="60px">|  `v0` | *Animal-themed child-friendly shogi.* |
-|<a href="https://en.wikipedia.org/wiki/Backgammon">Backgammon</a><br>`"backgammon"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/backgammon_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/backgammon_light.gif" width="60px">| `beta` | *Luck aids bearing off checkers.* |
+|<a href="https://en.wikipedia.org/wiki/Backgammon">Backgammon</a><br>`"backgammon"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/backgammon_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/backgammon_light.gif" width="60px">| `v0` | *Luck aids bearing off checkers.* |
 |<a href="https://en.wikipedia.org/wiki/Chess">Chess</a><br>`"chess"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_light.gif" width="60px">| `v0` | *Checkmate opponent's king to win.* |
 |<a href="https://en.wikipedia.org/wiki/Connect_Four">Connect Four</a><br>`"connect_four"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/connect_four_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/connect_four_light.gif" width="60px">| `v0` | *Connect discs, win with four.* |
 |<a href="https://en.wikipedia.org/wiki/Minichess">Gardner Chess</a><br>`"gardner_chess"`|<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/gardner_chess_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/gardner_chess_light.gif" width="60px">| `v0` | *5x5 chess variant, excluding castling.* |
 |<a href="https://en.wikipedia.org/wiki/Go_(game)">Go</a><br>`"go_9x9"` `"go_19x19"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_light.gif" width="60px">| `v0` | *Strategically place stones, claim territory.* |
 |<a href="https://en.wikipedia.org/wiki/Hex_(board_game)">Hex</a><br>`"hex"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/hex_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/hex_light.gif" width="60px">| `v0` | *Connect opposite sides, block opponent.* |
-|<a href="https://en.wikipedia.org/wiki/Kuhn_poker">Kuhn Poker</a><br>`"kuhn_poker"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/kuhn_poker_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/kuhn_poker_light.gif" width="60px">| `beta` | *Three-card betting and bluffing game.* |
-|<a href="https://arxiv.org/abs/1207.1411">Leduc hold'em</a><br>`"leduc_holdem"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/leduc_holdem_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/leduc_holdem_light.gif" width="60px">| `beta` | *Two-suit, limited deck poker.* |
-|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Asterix</a><br>`"minatar-asterix"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-asterix.gif" width="50px">| `beta` | *Avoid enemies, collect treasure, survive.* |
-|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Breakout</a><br>`"minatar-breakout"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-breakout.gif" width="50px">| `beta` | *Paddle, ball, bricks, bounce, clear.* |
-|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Freeway</a><br>`"minatar-freeway"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-freeway.gif" width="50px">| `beta` | *Dodging cars, climbing up freeway.* |
-|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Seaquest</a><br>`"minatar-seaquest"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-seaquest.gif" width="50px">| `beta` | *Underwater submarine rescue and combat.* |
-|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/SpaceInvaders</a><br>`"minatar-space_invaders"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-space_invaders.gif" width="50px">| `beta` | *Alien shooter game, dodge bullets.* |
+|<a href="https://en.wikipedia.org/wiki/Kuhn_poker">Kuhn Poker</a><br>`"kuhn_poker"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/kuhn_poker_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/kuhn_poker_light.gif" width="60px">| `v0` | *Three-card betting and bluffing game.* |
+|<a href="https://arxiv.org/abs/1207.1411">Leduc hold'em</a><br>`"leduc_holdem"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/leduc_holdem_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/leduc_holdem_light.gif" width="60px">| `v0` | *Two-suit, limited deck poker.* |
+|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Asterix</a><br>`"minatar-asterix"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-asterix.gif" width="50px">| `v0` | *Avoid enemies, collect treasure, survive.* |
+|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Breakout</a><br>`"minatar-breakout"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-breakout.gif" width="50px">| `v0` | *Paddle, ball, bricks, bounce, clear.* |
+|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Freeway</a><br>`"minatar-freeway"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-freeway.gif" width="50px">| `v0` | *Dodging cars, climbing up freeway.* |
+|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/Seaquest</a><br>`"minatar-seaquest"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-seaquest.gif" width="50px">| `v0` | *Underwater submarine rescue and combat.* |
+|<a href="https://github.com/kenjyoung/MinAtar">MinAtar/SpaceInvaders</a><br>`"minatar-space_invaders"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/minatar-space_invaders.gif" width="50px">| `v0` | *Alien shooter game, dodge bullets.* |
 |<a href="https://en.wikipedia.org/wiki/Reversi">Othello</a><br>`"othello"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/othello_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/othello_light.gif" width="60px">| `v0` | *Flip and conquer opponent's pieces.* |
 |<a href="https://en.wikipedia.org/wiki/Shogi">Shogi</a><br>`"shogi"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_light.gif" width="60px"> | `v0` | *Japanese chess with captured pieces.* |
-|<a href="https://sugorokuya.jp/p/suzume-jong">Sparrow Mahjong</a><br>`"sparrow_mahjong"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/sparrow_mahjong_dark.svg" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/sparrow_mahjong_light.svg" width="60px">|  `beta` | *A simplified, children-friendly Mahjong.* |
+|<a href="https://sugorokuya.jp/p/suzume-jong">Sparrow Mahjong</a><br>`"sparrow_mahjong"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/sparrow_mahjong_dark.svg" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/sparrow_mahjong_light.svg" width="60px">|  `v0` | *A simplified, children-friendly Mahjong.* |
 |<a href="https://en.wikipedia.org/wiki/Tic-tac-toe">Tic-tac-toe</a><br>`"tic_tac_toe"` |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/tic_tac_toe_dark.gif" width="60px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/tic_tac_toe_light.gif" width="60px">| `v0` | *Three in a row wins.* |
 
 - <a href="https://en.wikipedia.org/wiki/Contract_bridge">Bridge Bidding</a> and <a href="https://en.wikipedia.org/wiki/Japanese_mahjong">Mahjong</a> environments are under development 🚧
 - Five-word descriptions were generated by [ChatGPT](https://chat.openai.com/) 🤖
 
 
 ## See also
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pgx Version: 0.8.1 Summary: GPU/TPU-accelerated
+Metadata-Version: 2.1 Name: pgx Version: 0.9.0 Summary: GPU/TPU-accelerated
 parallel game simulators for reinforcement learning (RL) Home-page: https://
 github.com/sotetsuk/pgx Author: Sotetsu KOYAMADA Author-email:
 sotetsu.koyamada@gmail.com Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown License-
 File: LICENSE [![ci](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml/
 badge.svg)](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml)
@@ -22,55 +22,61 @@
 github.com/google/jax)-native physics engine, provides extremely high-speed
 parallel simulation for RL in *continuous* state space. Then, what about RL in
 *discrete* state spaces like Chess, Shogi, and Go? **Pgx** provides a wide
 variety of JAX-native game simulators! Highlighted features include: - â¡
 **Super fast** in parallel execution on accelerators - ð² **Various game
 support** including **Backgammon**, **Chess**, **Shogi**, and **Go** - ð¼ï¸
 **Beautiful visualization** in SVG format ## Installation ```sh pip install pgx
-``` ## Usage Note that all `step` functions in Pgx environments are **JAX-
-native.**, i.e., they are all *JIT-able*. [Open_In_Colab] ```py import jax
-import pgx env = pgx.make("go_19x19") init = jax.jit(jax.vmap(env.init)) #
-vectorize and JIT-compile step = jax.jit(jax.vmap(env.step)) batch_size = 1024
-keys = jax.random.split(jax.random.PRNGKey(42), batch_size) state = init(keys)
-# vectorized states while not (state.terminated | state.truncated).all():
-action = model(state.current_player, state.observation,
-state.legal_action_mask) state = step(state, action) # state.reward (2,) ```
-Pgx is a library that focuses on faster implementations rather than just the
-API itself. However, the API itself is also sufficiently general. For example,
-all environments in Pgx can be converted to the AEC API of [PettingZoo](https:/
-/github.com/Farama-Foundation/PettingZoo), and you can run Pgx environments
-through the PettingZoo API. You can see the demonstration in Google Colab:
-[Open_In_Colab]  ## Supported games | Backgammon | Chess | Shogi | Go | |:---:
-|:---:|:---:|:---:| |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/backgammon_dark.gif#gh-dark-mode-only][https://
-raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
-backgammon_light.gif#gh-light-mode-only]|[https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-dark-mode-only][https://
-raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_light.gif#gh-
-light-mode-only]|[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/shogi_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/shogi_light.gif#gh-light-mode-only]|[https://
-raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_dark.gif#gh-
+``` Note that the [MinAtar](https://github.com/kenjyoung/MinAtar) suite is
+provided as a separate extension for Pgx ([`pgx-minatar`](https://github.com/
+sotetsuk/pgx-minatar)). Therefore, please run the following command additionaly
+to use the MinAtar suite in Pgx: ```sh pip install pgx-minatar ``` Pgx is
+provided under the Apache 2.0 License, but the original MinAtar suite follows
+the GPL 3.0 License. Therefore, please note that the separated MinAtar
+extension for Pgx also adheres to the GPL 3.0 License. ## Usage Note that all
+`step` functions in Pgx environments are **JAX-native.**, i.e., they are all
+*JIT-able*. [Open_In_Colab] ```py import jax import pgx env = pgx.make
+("go_19x19") init = jax.jit(jax.vmap(env.init)) # vectorize and JIT-compile
+step = jax.jit(jax.vmap(env.step)) batch_size = 1024 keys = jax.random.split
+(jax.random.PRNGKey(42), batch_size) state = init(keys) # vectorized states
+while not (state.terminated | state.truncated).all(): action = model
+(state.current_player, state.observation, state.legal_action_mask) state = step
+(state, action) # state.reward (2,) ``` Pgx is a library that focuses on faster
+implementations rather than just the API itself. However, the API itself is
+also sufficiently general. For example, all environments in Pgx can be
+converted to the AEC API of [PettingZoo](https://github.com/Farama-Foundation/
+PettingZoo), and you can run Pgx environments through the PettingZoo API. You
+can see the demonstration in Google Colab: [Open_In_Colab]  ## Supported games
+| Backgammon | Chess | Shogi | Go | |:---:|:---:|:---:|:---:| |[https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/backgammon_dark.gif#gh-
 dark-mode-only][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/go-19x19_light.gif#gh-light-mode-only]| Use `pgx.available_envs() -
-> Tuple[EnvId]` to see the list of currently available games. Given an ``, you
-can create the environment via ```py >>> env = pgx.make() ``` You can check the
-current version of each environment by ```py >>> env.version ``` | Game/EnvId |
-Visualization | Version | Five-word description | |:---:|:---:|:---:|:---:
-| |2048
+assets/backgammon_light.gif#gh-light-mode-only]|[https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-dark-
+mode-only][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
+chess_light.gif#gh-light-mode-only]|[https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/shogi_dark.gif#gh-dark-mode-only][https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_light.gif#gh-
+light-mode-only]|[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
+assets/go-19x19_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/go-19x19_light.gif#gh-light-mode-only]| Use
+`pgx.available_envs() -> Tuple[EnvId]` to see the list of currently available
+games. Given an ``, you can create the environment via ```py >>> env = pgx.make
+() ``` You can check the current version of each environment by ```py >>>
+env.version ``` | Game/EnvId | Visualization | Version | Five-word description
+| |:---:|:---:|:---:|:---:| |2048
 `"2048"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 2048_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
-2048_light.gif]| `beta` | *Merge tiles to create 2048.* | |Animal_Shogi
+2048_light.gif]| `v0` | *Merge tiles to create 2048.* | |Animal_Shogi
 `"animal_shogi"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/animal_shogi_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
 main/docs/assets/animal_shogi_light.gif]| `v0` | *Animal-themed child-friendly
 shogi.* | |Backgammon
 `"backgammon"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/backgammon_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
-main/docs/assets/backgammon_light.gif]| `beta` | *Luck aids bearing off
+main/docs/assets/backgammon_light.gif]| `v0` | *Luck aids bearing off
 checkers.* | |Chess
 `"chess"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 chess_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/chess_light.gif]| `v0` | *Checkmate opponent's king to win.* | |Connect
 Four
 `"connect_four"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/connect_four_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
@@ -85,46 +91,46 @@
 main/docs/assets/go-19x19_light.gif]| `v0` | *Strategically place stones, claim
 territory.* | |Hex
 `"hex"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 hex_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 hex_light.gif]| `v0` | *Connect opposite sides, block opponent.* | |Kuhn_Poker
 `"kuhn_poker"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/kuhn_poker_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
-main/docs/assets/kuhn_poker_light.gif]| `beta` | *Three-card betting and
-bluffing game.* | |Leduc_hold'em
+main/docs/assets/kuhn_poker_light.gif]| `v0` | *Three-card betting and bluffing
+game.* | |Leduc_hold'em
 `"leduc_holdem"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/leduc_holdem_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
-main/docs/assets/leduc_holdem_light.gif]| `beta` | *Two-suit, limited deck
+main/docs/assets/leduc_holdem_light.gif]| `v0` | *Two-suit, limited deck
 poker.* | |MinAtar/Asterix
 `"minatar-asterix"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/minatar-asterix.gif]| `beta` | *Avoid enemies, collect treasure,
-survive.* | |MinAtar/Breakout
+assets/minatar-asterix.gif]| `v0` | *Avoid enemies, collect treasure, survive.*
+| |MinAtar/Breakout
 `"minatar-breakout"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/
-docs/assets/minatar-breakout.gif]| `beta` | *Paddle, ball, bricks, bounce,
+docs/assets/minatar-breakout.gif]| `v0` | *Paddle, ball, bricks, bounce,
 clear.* | |MinAtar/Freeway
 `"minatar-freeway"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/minatar-freeway.gif]| `beta` | *Dodging cars, climbing up freeway.* |
+assets/minatar-freeway.gif]| `v0` | *Dodging cars, climbing up freeway.* |
 |MinAtar/Seaquest
 `"minatar-seaquest"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/
-docs/assets/minatar-seaquest.gif]| `beta` | *Underwater submarine rescue and
+docs/assets/minatar-seaquest.gif]| `v0` | *Underwater submarine rescue and
 combat.* | |MinAtar/SpaceInvaders
 `"minatar-space_invaders"` |[https://raw.githubusercontent.com/sotetsuk/pgx/
-main/docs/assets/minatar-space_invaders.gif]| `beta` | *Alien shooter game,
-dodge bullets.* | |Othello
+main/docs/assets/minatar-space_invaders.gif]| `v0` | *Alien shooter game, dodge
+bullets.* | |Othello
 `"othello"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 othello_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/othello_light.gif]| `v0` | *Flip and conquer opponent's pieces.* |
 |Shogi
 `"shogi"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 shogi_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/shogi_light.gif] | `v0` | *Japanese chess with captured pieces.* |
 |Sparrow_Mahjong
 `"sparrow_mahjong"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/sparrow_mahjong_dark.svg][https://raw.githubusercontent.com/sotetsuk/
-pgx/main/docs/assets/sparrow_mahjong_light.svg]| `beta` | *A simplified,
+pgx/main/docs/assets/sparrow_mahjong_light.svg]| `v0` | *A simplified,
 children-friendly Mahjong.* | |Tic-tac-toe
 `"tic_tac_toe"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/tic_tac_toe_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
 main/docs/assets/tic_tac_toe_light.gif]| `v0` | *Three in a row wins.* | -
 Bridge_Bidding and Mahjong environments are under development ð§ - Five-word
 descriptions were generated by [ChatGPT](https://chat.openai.com/) ð¤ ## See
 also Pgx is intended to complement these **JAX-native environments** with
```

### Comparing `pgx-0.8.1/pgx.egg-info/SOURCES.txt` & `pgx-0.9.0/pgx.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -98,38 +98,25 @@
 pgx/_src/dwg/images/sparrow_mahjong/oya.svg
 pgx/_src/dwg/images/sparrow_mahjong/rd.svg
 pgx/experimental/__init__.py
 pgx/experimental/bridge_bidding.py
 pgx/experimental/gym.py
 pgx/experimental/utils.py
 pgx/experimental/visualize.py
-pgx/minatar/__init__.py
-pgx/minatar/asterix.py
-pgx/minatar/breakout.py
-pgx/minatar/freeway.py
-pgx/minatar/seaquest.py
-pgx/minatar/space_invaders.py
-pgx/minatar/utils.py
 tests/__init__.py
-tests/minatar_utils.py
 tests/test_animal_shogi.py
-tests/test_asterix.py
 tests/test_backgammon.py
 tests/test_baseline.py
-tests/test_breakout.py
 tests/test_bridge_bidding.py
 tests/test_chess.py
 tests/test_connect_four.py
-tests/test_freeway.py
 tests/test_gardner_chess.py
 tests/test_go.py
 tests/test_hex.py
 tests/test_kuhn_poker.py
 tests/test_leduc_holdem.py
 tests/test_mahjong.py
 tests/test_othello.py
 tests/test_play2048.py
-tests/test_seaquest.py
 tests/test_shogi.py
-tests/test_space_invaders.py
 tests/test_sparrow_mahjong.py
 tests/test_tic_tac_toe.py
```

### Comparing `pgx-0.8.1/pyproject.toml` & `pgx-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/setup.py` & `pgx-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/tests/test_animal_shogi.py` & `pgx-0.9.0/tests/test_animal_shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/tests/test_backgammon.py` & `pgx-0.9.0/tests/test_backgammon.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/tests/test_baseline.py` & `pgx-0.9.0/tests/test_baseline.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/tests/test_bridge_bidding.py` & `pgx-0.9.0/tests/test_bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/tests/test_chess.py` & `pgx-0.9.0/tests/test_chess.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/tests/test_connect_four.py` & `pgx-0.9.0/tests/test_connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/tests/test_gardner_chess.py` & `pgx-0.9.0/tests/test_gardner_chess.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/tests/test_go.py` & `pgx-0.9.0/tests/test_go.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/tests/test_hex.py` & `pgx-0.9.0/tests/test_hex.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/tests/test_kuhn_poker.py` & `pgx-0.9.0/tests/test_kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/tests/test_leduc_holdem.py` & `pgx-0.9.0/tests/test_leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/tests/test_mahjong.py` & `pgx-0.9.0/tests/test_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/tests/test_othello.py` & `pgx-0.9.0/tests/test_othello.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/tests/test_play2048.py` & `pgx-0.9.0/tests/test_play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/tests/test_shogi.py` & `pgx-0.9.0/tests/test_shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/tests/test_sparrow_mahjong.py` & `pgx-0.9.0/tests/test_sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.8.1/tests/test_tic_tac_toe.py` & `pgx-0.9.0/tests/test_tic_tac_toe.py`

 * *Files identical despite different names*

