# Comparing `tmp/all-fives-domino-1.0.8.tar.gz` & `tmp/all-fives-domino-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "all-fives-domino-1.0.8.tar", last modified: Fri Jun  2 12:17:29 2023, max compression
+gzip compressed data, was "all-fives-domino-1.0.9.tar", last modified: Fri Jun  2 13:05:00 2023, max compression
```

## Comparing `all-fives-domino-1.0.8.tar` & `all-fives-domino-1.0.9.tar`

### file list

```diff
@@ -1,59 +1,65 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.797644 all-fives-domino-1.0.8/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-05-25 20:33:44.000000 all-fives-domino-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-25 20:33:44.000000 all-fives-domino-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      802 2023-06-02 12:17:29.797644 all-fives-domino-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      485 2023-06-02 12:17:14.000000 all-fives-domino-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.785643 all-fives-domino-1.0.8/all_fives_domino.egg-info/
--rw-r--r--   0 root         (0) root         (0)      802 2023-06-02 12:17:29.000000 all-fives-domino-1.0.8/all_fives_domino.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1371 2023-06-02 12:17:29.000000 all-fives-domino-1.0.8/all_fives_domino.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 12:17:29.000000 all-fives-domino-1.0.8/all_fives_domino.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-02 12:17:29.000000 all-fives-domino-1.0.8/all_fives_domino.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-05-25 20:33:44.000000 all-fives-domino-1.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 12:17:29.797644 all-fives-domino-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      798 2023-05-25 20:33:44.000000 all-fives-domino-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.785643 all-fives-domino-1.0.8/src/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.8/src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.785643 all-fives-domino-1.0.8/src/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      190 2023-05-25 20:34:42.000000 all-fives-domino-1.0.8/src/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.789643 all-fives-domino-1.0.8/src/main/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.8/src/main/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.789643 all-fives-domino-1.0.8/src/main/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      195 2023-05-25 20:34:42.000000 all-fives-domino-1.0.8/src/main/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.789643 all-fives-domino-1.0.8/src/main/game/
--rw-r--r--   0 root         (0) root         (0)     3981 2023-06-02 12:17:05.000000 all-fives-domino-1.0.8/src/main/game/DominoRound.py
--rw-r--r--   0 root         (0) root         (0)     2603 2023-05-26 22:06:49.000000 all-fives-domino-1.0.8/src/main/game/Piece.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.8/src/main/game/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.789643 all-fives-domino-1.0.8/src/main/game/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     5709 2023-06-02 12:17:13.000000 all-fives-domino-1.0.8/src/main/game/__pycache__/DominoRound.cpython-311.pyc
--rw-r--r--   0 root         (0) root         (0)     4585 2023-05-26 22:11:06.000000 all-fives-domino-1.0.8/src/main/game/__pycache__/Piece.cpython-311.pyc
--rw-r--r--   0 root         (0) root         (0)      200 2023-05-25 20:34:42.000000 all-fives-domino-1.0.8/src/main/game/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.789643 all-fives-domino-1.0.8/src/main/player/
--rw-r--r--   0 root         (0) root         (0)      266 2023-05-25 21:10:41.000000 all-fives-domino-1.0.8/src/main/player/Brain.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-05-26 22:06:49.000000 all-fives-domino-1.0.8/src/main/player/Hand.py
--rw-r--r--   0 root         (0) root         (0)      380 2023-05-26 22:06:49.000000 all-fives-domino-1.0.8/src/main/player/Player.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.8/src/main/player/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.793644 all-fives-domino-1.0.8/src/main/player/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     2005 2023-05-26 22:11:06.000000 all-fives-domino-1.0.8/src/main/player/__pycache__/Hand.cpython-311.pyc
--rw-r--r--   0 root         (0) root         (0)     1371 2023-05-26 22:11:06.000000 all-fives-domino-1.0.8/src/main/player/__pycache__/Player.cpython-311.pyc
--rw-r--r--   0 root         (0) root         (0)      202 2023-05-26 22:11:06.000000 all-fives-domino-1.0.8/src/main/player/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.793644 all-fives-domino-1.0.8/src/main/ui/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 12:17:05.000000 all-fives-domino-1.0.8/src/main/ui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.793644 all-fives-domino-1.0.8/src/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.8/src/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.793644 all-fives-domino-1.0.8/src/test/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      195 2023-05-25 20:34:42.000000 all-fives-domino-1.0.8/src/test/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.793644 all-fives-domino-1.0.8/src/test/game/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.8/src/test/game/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.793644 all-fives-domino-1.0.8/src/test/game/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      200 2023-05-25 20:34:42.000000 all-fives-domino-1.0.8/src/test/game/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 root         (0) root         (0)    26801 2023-05-26 22:11:06.000000 all-fives-domino-1.0.8/src/test/game/__pycache__/test_pieces.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 root         (0) root         (0)      551 2023-05-26 22:11:06.000000 all-fives-domino-1.0.8/src/test/game/__pycache__/test_round.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 root         (0) root         (0)     1411 2023-05-26 22:06:49.000000 all-fives-domino-1.0.8/src/test/game/test_pieces.py
--rw-r--r--   0 root         (0) root         (0)       94 2023-05-26 22:06:49.000000 all-fives-domino-1.0.8/src/test/game/test_round.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.797644 all-fives-domino-1.0.8/src/test/player/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 22:06:49.000000 all-fives-domino-1.0.8/src/test/player/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.797644 all-fives-domino-1.0.8/src/test/player/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      202 2023-05-26 22:11:06.000000 all-fives-domino-1.0.8/src/test/player/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 root         (0) root         (0)     8551 2023-05-27 06:34:56.000000 all-fives-domino-1.0.8/src/test/player/__pycache__/test_hand.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 root         (0) root         (0)      574 2023-05-27 06:34:49.000000 all-fives-domino-1.0.8/src/test/player/test_hand.py
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-02 12:17:16.000000 all-fives-domino-1.0.8/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:05:00.902833 all-fives-domino-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-05-25 20:33:44.000000 all-fives-domino-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-25 20:33:44.000000 all-fives-domino-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      802 2023-06-02 13:05:00.898833 all-fives-domino-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      485 2023-06-02 13:04:46.000000 all-fives-domino-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:05:00.890833 all-fives-domino-1.0.9/all_fives_domino.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      802 2023-06-02 13:05:00.000000 all-fives-domino-1.0.9/all_fives_domino.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-06-02 13:05:00.000000 all-fives-domino-1.0.9/all_fives_domino.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 13:05:00.000000 all-fives-domino-1.0.9/all_fives_domino.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-02 13:05:00.000000 all-fives-domino-1.0.9/all_fives_domino.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-05-25 20:33:44.000000 all-fives-domino-1.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 13:05:00.902833 all-fives-domino-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      798 2023-05-25 20:33:44.000000 all-fives-domino-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:05:00.890833 all-fives-domino-1.0.9/src/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.9/src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:05:00.890833 all-fives-domino-1.0.9/src/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      190 2023-05-25 20:34:42.000000 all-fives-domino-1.0.9/src/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:05:00.890833 all-fives-domino-1.0.9/src/main/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.9/src/main/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:05:00.890833 all-fives-domino-1.0.9/src/main/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      195 2023-05-25 20:34:42.000000 all-fives-domino-1.0.9/src/main/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:05:00.890833 all-fives-domino-1.0.9/src/main/game/
+-rw-r--r--   0 root         (0) root         (0)     2862 2023-06-02 13:04:37.000000 all-fives-domino-1.0.9/src/main/game/DominoRound.py
+-rw-r--r--   0 root         (0) root         (0)     3070 2023-06-02 13:04:37.000000 all-fives-domino-1.0.9/src/main/game/Piece.py
+-rw-r--r--   0 root         (0) root         (0)     1750 2023-06-02 13:04:37.000000 all-fives-domino-1.0.9/src/main/game/Scorer.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.9/src/main/game/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:05:00.894833 all-fives-domino-1.0.9/src/main/game/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     4667 2023-06-02 13:04:45.000000 all-fives-domino-1.0.9/src/main/game/__pycache__/DominoRound.cpython-311.pyc
+-rw-r--r--   0 root         (0) root         (0)     5502 2023-06-02 13:04:45.000000 all-fives-domino-1.0.9/src/main/game/__pycache__/Piece.cpython-311.pyc
+-rw-r--r--   0 root         (0) root         (0)     2853 2023-06-02 13:04:45.000000 all-fives-domino-1.0.9/src/main/game/__pycache__/Scorer.cpython-311.pyc
+-rw-r--r--   0 root         (0) root         (0)      200 2023-05-25 20:34:42.000000 all-fives-domino-1.0.9/src/main/game/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:05:00.894833 all-fives-domino-1.0.9/src/main/player/
+-rw-r--r--   0 root         (0) root         (0)      266 2023-05-25 21:10:41.000000 all-fives-domino-1.0.9/src/main/player/Brain.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-05-26 22:06:49.000000 all-fives-domino-1.0.9/src/main/player/Hand.py
+-rw-r--r--   0 root         (0) root         (0)      380 2023-05-26 22:06:49.000000 all-fives-domino-1.0.9/src/main/player/Player.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.9/src/main/player/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:05:00.894833 all-fives-domino-1.0.9/src/main/player/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     2005 2023-05-26 22:11:06.000000 all-fives-domino-1.0.9/src/main/player/__pycache__/Hand.cpython-311.pyc
+-rw-r--r--   0 root         (0) root         (0)     1371 2023-05-26 22:11:06.000000 all-fives-domino-1.0.9/src/main/player/__pycache__/Player.cpython-311.pyc
+-rw-r--r--   0 root         (0) root         (0)      202 2023-05-26 22:11:06.000000 all-fives-domino-1.0.9/src/main/player/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:05:00.894833 all-fives-domino-1.0.9/src/main/ui/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 12:17:05.000000 all-fives-domino-1.0.9/src/main/ui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:05:00.894833 all-fives-domino-1.0.9/src/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.9/src/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:05:00.894833 all-fives-domino-1.0.9/src/test/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      195 2023-05-25 20:34:42.000000 all-fives-domino-1.0.9/src/test/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:05:00.898833 all-fives-domino-1.0.9/src/test/game/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.9/src/test/game/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:05:00.898833 all-fives-domino-1.0.9/src/test/game/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      200 2023-05-25 20:34:42.000000 all-fives-domino-1.0.9/src/test/game/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 root         (0) root         (0)     3790 2023-06-02 13:04:45.000000 all-fives-domino-1.0.9/src/test/game/__pycache__/test_piece_appending.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 root         (0) root         (0)    26801 2023-05-26 22:11:06.000000 all-fives-domino-1.0.9/src/test/game/__pycache__/test_pieces.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 root         (0) root         (0)      551 2023-05-26 22:11:06.000000 all-fives-domino-1.0.9/src/test/game/__pycache__/test_round.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 root         (0) root         (0)     6130 2023-06-02 13:04:45.000000 all-fives-domino-1.0.9/src/test/game/__pycache__/test_scorer.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 root         (0) root         (0)      276 2023-06-02 13:04:37.000000 all-fives-domino-1.0.9/src/test/game/test_piece_appending.py
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-05-26 22:06:49.000000 all-fives-domino-1.0.9/src/test/game/test_pieces.py
+-rw-r--r--   0 root         (0) root         (0)       94 2023-05-26 22:06:49.000000 all-fives-domino-1.0.9/src/test/game/test_round.py
+-rw-r--r--   0 root         (0) root         (0)      490 2023-06-02 13:04:37.000000 all-fives-domino-1.0.9/src/test/game/test_scorer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:05:00.898833 all-fives-domino-1.0.9/src/test/player/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 22:06:49.000000 all-fives-domino-1.0.9/src/test/player/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 13:05:00.898833 all-fives-domino-1.0.9/src/test/player/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      202 2023-05-26 22:11:06.000000 all-fives-domino-1.0.9/src/test/player/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 root         (0) root         (0)     8551 2023-05-27 06:34:56.000000 all-fives-domino-1.0.9/src/test/player/__pycache__/test_hand.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 root         (0) root         (0)      574 2023-05-27 06:34:49.000000 all-fives-domino-1.0.9/src/test/player/test_hand.py
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-02 13:04:48.000000 all-fives-domino-1.0.9/version.txt
```

### Comparing `all-fives-domino-1.0.8/LICENSE` & `all-fives-domino-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `all-fives-domino-1.0.8/PKG-INFO` & `all-fives-domino-1.0.9/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: all-fives-domino
-Version: 1.0.8
+Version: 1.0.9
 Summary: Abstractions around cloud file interfaces (WIP)
 Home-page: https://github.com/Informanthik/all-fives-domino
 Author: Jothapunkt
 Author-email: jakob-hoefner@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 All Fives Domino
 ================
 
 Simple version of a domino variant
 
 ![image](https://img.shields.io/pypi/v/jhdata?style=flat-square)
-![image](https://img.shields.io/static/v1?label=pytest&message=12+tests&color=success&style=flat-square)
-![image](https://img.shields.io/static/v1?label=coverage&message=50%25&color=orange&style=flat-square)
+![image](https://img.shields.io/static/v1?label=pytest&message=14+tests&color=success&style=flat-square)
+![image](https://img.shields.io/static/v1?label=coverage&message=61%25&color=yellow&style=flat-square)
 
 ## Installing
 
 Install the [PyPI Package](https://pypi.org/project/all-fives-domino/):
 
     pip install all-fives-domino
```

### Comparing `all-fives-domino-1.0.8/all_fives_domino.egg-info/PKG-INFO` & `all-fives-domino-1.0.9/all_fives_domino.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: all-fives-domino
-Version: 1.0.8
+Version: 1.0.9
 Summary: Abstractions around cloud file interfaces (WIP)
 Home-page: https://github.com/Informanthik/all-fives-domino
 Author: Jothapunkt
 Author-email: jakob-hoefner@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 All Fives Domino
 ================
 
 Simple version of a domino variant
 
 ![image](https://img.shields.io/pypi/v/jhdata?style=flat-square)
-![image](https://img.shields.io/static/v1?label=pytest&message=12+tests&color=success&style=flat-square)
-![image](https://img.shields.io/static/v1?label=coverage&message=50%25&color=orange&style=flat-square)
+![image](https://img.shields.io/static/v1?label=pytest&message=14+tests&color=success&style=flat-square)
+![image](https://img.shields.io/static/v1?label=coverage&message=61%25&color=yellow&style=flat-square)
 
 ## Installing
 
 Install the [PyPI Package](https://pypi.org/project/all-fives-domino/):
 
     pip install all-fives-domino
```

### Comparing `all-fives-domino-1.0.8/all_fives_domino.egg-info/SOURCES.txt` & `all-fives-domino-1.0.9/all_fives_domino.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,31 +10,37 @@
 all_fives_domino.egg-info/top_level.txt
 src/__init__.py
 src/__pycache__/__init__.cpython-311.pyc
 src/main/__init__.py
 src/main/__pycache__/__init__.cpython-311.pyc
 src/main/game/DominoRound.py
 src/main/game/Piece.py
+src/main/game/Scorer.py
 src/main/game/__init__.py
 src/main/game/__pycache__/DominoRound.cpython-311.pyc
 src/main/game/__pycache__/Piece.cpython-311.pyc
+src/main/game/__pycache__/Scorer.cpython-311.pyc
 src/main/game/__pycache__/__init__.cpython-311.pyc
 src/main/player/Brain.py
 src/main/player/Hand.py
 src/main/player/Player.py
 src/main/player/__init__.py
 src/main/player/__pycache__/Hand.cpython-311.pyc
 src/main/player/__pycache__/Player.cpython-311.pyc
 src/main/player/__pycache__/__init__.cpython-311.pyc
 src/main/ui/__init__.py
 src/test/__init__.py
 src/test/__pycache__/__init__.cpython-311.pyc
 src/test/game/__init__.py
+src/test/game/test_piece_appending.py
 src/test/game/test_pieces.py
 src/test/game/test_round.py
+src/test/game/test_scorer.py
 src/test/game/__pycache__/__init__.cpython-311.pyc
+src/test/game/__pycache__/test_piece_appending.cpython-311-pytest-7.3.1.pyc
 src/test/game/__pycache__/test_pieces.cpython-311-pytest-7.3.1.pyc
 src/test/game/__pycache__/test_round.cpython-311-pytest-7.3.1.pyc
+src/test/game/__pycache__/test_scorer.cpython-311-pytest-7.3.1.pyc
 src/test/player/__init__.py
 src/test/player/test_hand.py
 src/test/player/__pycache__/__init__.cpython-311.pyc
 src/test/player/__pycache__/test_hand.cpython-311-pytest-7.3.1.pyc
```

### Comparing `all-fives-domino-1.0.8/setup.py` & `all-fives-domino-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `all-fives-domino-1.0.8/src/main/game/Piece.py` & `all-fives-domino-1.0.9/src/main/game/Piece.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,16 +22,34 @@
         self.linked: List[Piece] = []
         self.linked_to: Union[Piece, None] = None
         self.is_crossing = False
         self.is_double = self.sides[0] == self.sides[1]
         self.closed = False
         self.points = sum(self.sides)
 
-    def append(self, piece):
+    def append(self, piece: "Piece"):
+        piece.linked_to = self
         self.linked.append(piece)
+        if self.is_double and len(self.linked) == 2:
+            self.is_crossing = True
+
+    @property
+    def total_sides(self):
+        return 4 if self.is_crossing else 2
+
+    @property
+    def closed_sides(self):
+        sides = len(self.linked)
+        if self.linked_to is not None:
+            sides += 1
+        return sides
+
+    @property
+    def open_sides(self):
+        return self.total_sides - self.closed_sides
 
     def unlinked_side(self, other: "Piece") -> int:
         a, b = self.sides
         return b if a in other.sides else a
 
     def __str__(self):
         """Simple visual representation using die face Unicode symbols"""
```

### Comparing `all-fives-domino-1.0.8/src/main/game/__pycache__/DominoRound.cpython-311.pyc` & `all-fives-domino-1.0.9/src/main/game/__pycache__/Piece.cpython-311.pyc`

 * *Files 21% similar despite different names*

#### Python bytecode

```diff
@@ -1,779 +1,752 @@
 magic:    0xa70d0d0a
-moddate:  0xc1dd7964 (Fri Jun  2 12:17:05 2023 UTC)
-files sz: 3981
+moddate:  0xe5e87964 (Fri Jun  2 13:04:37 2023 UTC)
+files sz: 3070
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
-      0x9700640064016c006d015a016d025a026d035a030100640064026c046d
-      055a056d065a060100640064036c076d085a080100020047006404840064
-      05a6020000ab0200000000000000005a0964065300
+      0x9700640064016c006d015a016d025a02010002004700640284006403a6
+      020000ab0200000000000000005a03640484005a0464055300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('Union', 'List', 'Tuple'))
+                 4 LOAD_CONST               1 (('List', 'Union'))
                  6 IMPORT_NAME              0 (typing)
-                 8 IMPORT_FROM              1 (Union)
-                10 STORE_NAME               1 (Union)
-                12 IMPORT_FROM              2 (List)
-                14 STORE_NAME               2 (List)
-                16 IMPORT_FROM              3 (Tuple)
-                18 STORE_NAME               3 (Tuple)
-                20 POP_TOP
+                 8 IMPORT_FROM              1 (List)
+                10 STORE_NAME               1 (List)
+                12 IMPORT_FROM              2 (Union)
+                14 STORE_NAME               2 (Union)
+                16 POP_TOP
    
-     3          22 LOAD_CONST               0 (0)
-                24 LOAD_CONST               2 (('domino_set', 'Piece'))
-                26 IMPORT_NAME              4 (src.main.game.Piece)
-                28 IMPORT_FROM              5 (domino_set)
-                30 STORE_NAME               5 (domino_set)
-                32 IMPORT_FROM              6 (Piece)
-                34 STORE_NAME               6 (Piece)
-                36 POP_TOP
+     4          18 PUSH_NULL
+                20 LOAD_BUILD_CLASS
+                22 LOAD_CONST               2 (<code object Piece, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 4>)
+                24 MAKE_FUNCTION            0
+                26 LOAD_CONST               3 ('Piece')
+                28 PRECALL                  2
+                32 CALL                     2
+                42 STORE_NAME               3 (Piece)
    
-     4          38 LOAD_CONST               0 (0)
-                40 LOAD_CONST               3 (('Player',))
-                42 IMPORT_NAME              7 (src.main.player.Player)
-                44 IMPORT_FROM              8 (Player)
-                46 STORE_NAME               8 (Player)
-                48 POP_TOP
-   
-     7          50 PUSH_NULL
-                52 LOAD_BUILD_CLASS
-                54 LOAD_CONST               4 (<code object DominoRound, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py", line 7>)
-                56 MAKE_FUNCTION            0
-                58 LOAD_CONST               5 ('DominoRound')
-                60 PRECALL                  2
-                64 CALL                     2
-                74 STORE_NAME               9 (DominoRound)
-                76 LOAD_CONST               6 (None)
-                78 RETURN_VALUE
+    93          44 LOAD_CONST               4 (<code object domino_set, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 93>)
+                46 MAKE_FUNCTION            0
+                48 STORE_NAME               4 (domino_set)
+                50 LOAD_CONST               5 (None)
+                52 RETURN_VALUE
    consts
       0
-      ('Union', 'List', 'Tuple')
-      ('domino_set', 'Piece')
-      ('Player',)
+      ('List', 'Union')
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 9
+         stacksize : 4
          flags     : 0
          code
-            0x970065005a0164005a0264016402640364026404650364051900000000
-            00000000006606640684045a04640784005a05640884005a066507641564
-            0a6508640b65096604640c8405a6000000ab0000000000000000005a0a64
-            0d84005a0b6416640f650c640a6508641065036508641166021900000000
-            00000000006606641284055a0d641384005a0e641484005a0f64115300
-           7           0 RESUME                   0
+            0x970065005a0164005a0264016503640265036604640384045a04641364
+            0584045a05650664068400a6000000ab0000000000000000005a07650664
+            078400a6000000ab0000000000000000005a08650664088400a6000000ab
+            0000000000000000005a0964096400640a65036604640b84045a0a640c84
+            005a0b640d84005a0c640e84005a0d640f84005a0e641084005a0f641184
+            005a1064125300
+           4           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
-                       6 LOAD_CONST               0 ('DominoRound')
+                       6 LOAD_CONST               0 ('Piece')
                        8 STORE_NAME               2 (__qualname__)
          
-           8          10 LOAD_CONST               1 ('brain1')
-                      12 LOAD_CONST               2 ('Brain')
-                      14 LOAD_CONST               3 ('brain2')
-                      16 LOAD_CONST               2 ('Brain')
-                      18 LOAD_CONST               4 ('begins')
-                      20 LOAD_NAME                3 (Union)
-                      22 LOAD_CONST               5 (('Brain', None))
-                      24 BINARY_SUBSCR
-                      34 BUILD_TUPLE              6
-                      36 LOAD_CONST               6 (<code object __init__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py", line 8>)
-                      38 MAKE_FUNCTION            4 (annotations)
-                      40 STORE_NAME               4 (__init__)
-         
-          16          42 LOAD_CONST               7 (<code object deal_hand, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py", line 16>)
-                      44 MAKE_FUNCTION            0
-                      46 STORE_NAME               5 (deal_hand)
-         
-          22          48 LOAD_CONST               8 (<code object get_required_starting_piece, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py", line 22>)
-                      50 MAKE_FUNCTION            0
-                      52 STORE_NAME               6 (get_required_starting_piece)
-         
-          44          54 LOAD_NAME                7 (staticmethod)
-         
-          45          56 LOAD_CONST              21 ((28,))
-                      58 LOAD_CONST              10 ('piece')
-                      60 LOAD_NAME                8 (Piece)
-                      62 LOAD_CONST              11 ('return')
-                      64 LOAD_NAME                9 (int)
-                      66 BUILD_TUPLE              4
-                      68 LOAD_CONST              12 (<code object score_piece, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py", line 44>)
-                      70 MAKE_FUNCTION            5 (defaults, annotations)
-         
-          44          72 PRECALL                  0
-                      76 CALL                     0
-         
-          45          86 STORE_NAME              10 (score_piece)
-         
-          76          88 LOAD_CONST              13 (<code object score, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py", line 76>)
-                      90 MAKE_FUNCTION            0
-                      92 STORE_NAME              11 (score)
-         
-          80          94 LOAD_CONST              22 ((False,))
-                      96 LOAD_CONST              15 ('player')
-                      98 LOAD_NAME               12 (Player)
-                     100 LOAD_CONST              10 ('piece')
-                     102 LOAD_NAME                8 (Piece)
-                     104 LOAD_CONST              16 ('origin')
-                     106 LOAD_NAME                3 (Union)
-                     108 LOAD_NAME                8 (Piece)
-                     110 LOAD_CONST              17 (None)
-                     112 BUILD_TUPLE              2
-                     114 BINARY_SUBSCR
-                     124 BUILD_TUPLE              6
-                     126 LOAD_CONST              18 (<code object play, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py", line 80>)
-                     128 MAKE_FUNCTION            5 (defaults, annotations)
-                     130 STORE_NAME              13 (play)
-         
-         103         132 LOAD_CONST              19 (<code object valid_options, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py", line 103>)
-                     134 MAKE_FUNCTION            0
-                     136 STORE_NAME              14 (valid_options)
-         
-         106         138 LOAD_CONST              20 (<code object run, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py", line 106>)
-                     140 MAKE_FUNCTION            0
-                     142 STORE_NAME              15 (run)
-                     144 LOAD_CONST              17 (None)
-                     146 RETURN_VALUE
+           5          10 LOAD_CONST               1 ('a')
+                      12 LOAD_NAME                3 (int)
+                      14 LOAD_CONST               2 ('b')
+                      16 LOAD_NAME                3 (int)
+                      18 BUILD_TUPLE              4
+                      20 LOAD_CONST               3 (<code object __init__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 5>)
+                      22 MAKE_FUNCTION            4 (annotations)
+                      24 STORE_NAME               4 (__init__)
+         
+          29          26 LOAD_CONST              19 (('piece', 'Piece'))
+                      28 LOAD_CONST               5 (<code object append, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 29>)
+                      30 MAKE_FUNCTION            4 (annotations)
+                      32 STORE_NAME               5 (append)
+         
+          35          34 LOAD_NAME                6 (property)
+         
+          36          36 LOAD_CONST               6 (<code object total_sides, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 35>)
+                      38 MAKE_FUNCTION            0
+         
+          35          40 PRECALL                  0
+                      44 CALL                     0
+         
+          36          54 STORE_NAME               7 (total_sides)
+         
+          39          56 LOAD_NAME                6 (property)
+         
+          40          58 LOAD_CONST               7 (<code object closed_sides, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 39>)
+                      60 MAKE_FUNCTION            0
+         
+          39          62 PRECALL                  0
+                      66 CALL                     0
+         
+          40          76 STORE_NAME               8 (closed_sides)
+         
+          46          78 LOAD_NAME                6 (property)
+         
+          47          80 LOAD_CONST               8 (<code object open_sides, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 46>)
+                      82 MAKE_FUNCTION            0
+         
+          46          84 PRECALL                  0
+                      88 CALL                     0
+         
+          47          98 STORE_NAME               9 (open_sides)
+         
+          50         100 LOAD_CONST               9 ('other')
+                     102 LOAD_CONST               0 ('Piece')
+                     104 LOAD_CONST              10 ('return')
+                     106 LOAD_NAME                3 (int)
+                     108 BUILD_TUPLE              4
+                     110 LOAD_CONST              11 (<code object unlinked_side, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 50>)
+                     112 MAKE_FUNCTION            4 (annotations)
+                     114 STORE_NAME              10 (unlinked_side)
+         
+          54         116 LOAD_CONST              12 (<code object __str__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 54>)
+                     118 MAKE_FUNCTION            0
+                     120 STORE_NAME              11 (__str__)
+         
+          72         122 LOAD_CONST              13 (<code object __repr__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 72>)
+                     124 MAKE_FUNCTION            0
+                     126 STORE_NAME              12 (__repr__)
+         
+          76         128 LOAD_CONST              14 (<code object __hash__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 76>)
+                     130 MAKE_FUNCTION            0
+                     132 STORE_NAME              13 (__hash__)
+         
+          80         134 LOAD_CONST              15 (<code object __eq__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 80>)
+                     136 MAKE_FUNCTION            0
+                     138 STORE_NAME              14 (__eq__)
+         
+          84         140 LOAD_CONST              16 (<code object __lt__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 84>)
+                     142 MAKE_FUNCTION            0
+                     144 STORE_NAME              15 (__lt__)
+         
+          88         146 LOAD_CONST              17 (<code object __gt__, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py", line 88>)
+                     148 MAKE_FUNCTION            0
+                     150 STORE_NAME              16 (__gt__)
+                     152 LOAD_CONST              18 (None)
+                     154 RETURN_VALUE
          consts
-            'DominoRound'
-            'brain1'
-            'Brain'
-            'brain2'
-            'begins'
-            ('Brain', None)
+            'Piece'
+            'a'
+            'b'
             code
-               argcount  : 4
-               nlocals   : 4
-               stacksize : 4
+               argcount  : 3
+               nlocals   : 3
+               stacksize : 7
                flags     : 3
                code
-                  0x9700740100000000000000000000a6000000ab0000000000000000007c
-                  005f01000000000000000064007c005f0200000000000000007407000000
-                  000000000000007c017c00a6020000ab0200000000000000007c005f0400
-                  000000000000007407000000000000000000007c027c00a6020000ab0200
-                  000000000000007c005f0500000000000000007c037c016b020000000072
-                  077c006a0400000000000000006e0e7c037c026b020000000072077c006a
-                  0500000000000000006e0164007c005f06000000000000000064017c005f
-                  07000000000000000064005300
-                 8           0 RESUME                   0
-               
-                 9           2 LOAD_GLOBAL              1 (NULL + domino_set)
-                            14 PRECALL                  0
-                            18 CALL                     0
-                            28 LOAD_FAST                0 (self)
-                            30 STORE_ATTR               1 (pool)
-               
-                10          40 LOAD_CONST               0 (None)
-                            42 LOAD_FAST                0 (self)
-                            44 STORE_ATTR               2 (origin)
-               
-                11          54 LOAD_GLOBAL              7 (NULL + Player)
-                            66 LOAD_FAST                1 (brain1)
-                            68 LOAD_FAST                0 (self)
-                            70 PRECALL                  2
-                            74 CALL                     2
-                            84 LOAD_FAST                0 (self)
-                            86 STORE_ATTR               4 (player1)
-               
-                12          96 LOAD_GLOBAL              7 (NULL + Player)
-                           108 LOAD_FAST                2 (brain2)
-                           110 LOAD_FAST                0 (self)
-                           112 PRECALL                  2
-                           116 CALL                     2
+                  0x97007c0164016b000000000073127c0264016b0000000000730c7c0164
+                  026b040000000073067c0264026b04000000007216740100000000000000
+                  00000064037c019b0064047c029b0064059d05a6010000ab010000000000
+                  00000082017403000000000000000000007c017c026702a6010000ab0100
+                  000000000000007c005f02000000000000000067007c005f030000000000
+                  00000064067c005f04000000000000000064077c005f0500000000000000
+                  007c006a0200000000000000006401190000000000000000007c006a0200
+                  000000000000006408190000000000000000006b02000000007c005f0600
+                  0000000000000064077c005f070000000000000000741100000000000000
+                  0000007c006a020000000000000000a6010000ab0100000000000000007c
+                  005f09000000000000000064065300
+                 5           0 RESUME                   0
+               
+                18           2 LOAD_FAST                1 (a)
+                             4 LOAD_CONST               1 (0)
+                             6 COMPARE_OP               0 (<)
+                            12 POP_JUMP_FORWARD_IF_TRUE    18 (to 50)
+                            14 LOAD_FAST                2 (b)
+                            16 LOAD_CONST               1 (0)
+                            18 COMPARE_OP               0 (<)
+                            24 POP_JUMP_FORWARD_IF_TRUE    12 (to 50)
+                            26 LOAD_FAST                1 (a)
+                            28 LOAD_CONST               2 (6)
+                            30 COMPARE_OP               4 (>)
+                            36 POP_JUMP_FORWARD_IF_TRUE     6 (to 50)
+                            38 LOAD_FAST                2 (b)
+                            40 LOAD_CONST               2 (6)
+                            42 COMPARE_OP               4 (>)
+                            48 POP_JUMP_FORWARD_IF_FALSE    22 (to 94)
+               
+                19     >>   50 LOAD_GLOBAL              1 (NULL + ValueError)
+                            62 LOAD_CONST               3 ('Domino Piece sides can only have values 0-6, got [')
+                            64 LOAD_FAST                1 (a)
+                            66 FORMAT_VALUE             0
+                            68 LOAD_CONST               4 ('|')
+                            70 LOAD_FAST                2 (b)
+                            72 FORMAT_VALUE             0
+                            74 LOAD_CONST               5 (']')
+                            76 BUILD_STRING             5
+                            78 PRECALL                  1
+                            82 CALL                     1
+                            92 RAISE_VARARGS            1
+               
+                21     >>   94 LOAD_GLOBAL              3 (NULL + sorted)
+                           106 LOAD_FAST                1 (a)
+                           108 LOAD_FAST                2 (b)
+                           110 BUILD_LIST               2
+                           112 PRECALL                  1
+                           116 CALL                     1
                            126 LOAD_FAST                0 (self)
-                           128 STORE_ATTR               5 (player2)
+                           128 STORE_ATTR               2 (sides)
                
-                13         138 LOAD_FAST                3 (begins)
-                           140 LOAD_FAST                1 (brain1)
-                           142 COMPARE_OP               2 (==)
-                           148 POP_JUMP_FORWARD_IF_FALSE     7 (to 164)
-                           150 LOAD_FAST                0 (self)
-                           152 LOAD_ATTR                4 (player1)
-                           162 JUMP_FORWARD            14 (to 192)
-                       >>  164 LOAD_FAST                3 (begins)
-                           166 LOAD_FAST                2 (brain2)
-                           168 COMPARE_OP               2 (==)
-                           174 POP_JUMP_FORWARD_IF_FALSE     7 (to 190)
-                           176 LOAD_FAST                0 (self)
-                           178 LOAD_ATTR                5 (player2)
-                           188 JUMP_FORWARD             1 (to 192)
-                       >>  190 LOAD_CONST               0 (None)
-                       >>  192 LOAD_FAST                0 (self)
-                           194 STORE_ATTR               6 (current_player)
-               
-                14         204 LOAD_CONST               1 (False)
-                           206 LOAD_FAST                0 (self)
-                           208 STORE_ATTR               7 (has_crossing)
-                           218 LOAD_CONST               0 (None)
-                           220 RETURN_VALUE
+                22         138 BUILD_LIST               0
+                           140 LOAD_FAST                0 (self)
+                           142 STORE_ATTR               3 (linked)
+               
+                23         152 LOAD_CONST               6 (None)
+                           154 LOAD_FAST                0 (self)
+                           156 STORE_ATTR               4 (linked_to)
+               
+                24         166 LOAD_CONST               7 (False)
+                           168 LOAD_FAST                0 (self)
+                           170 STORE_ATTR               5 (is_crossing)
+               
+                25         180 LOAD_FAST                0 (self)
+                           182 LOAD_ATTR                2 (sides)
+                           192 LOAD_CONST               1 (0)
+                           194 BINARY_SUBSCR
+                           204 LOAD_FAST                0 (self)
+                           206 LOAD_ATTR                2 (sides)
+                           216 LOAD_CONST               8 (1)
+                           218 BINARY_SUBSCR
+                           228 COMPARE_OP               2 (==)
+                           234 LOAD_FAST                0 (self)
+                           236 STORE_ATTR               6 (is_double)
+               
+                26         246 LOAD_CONST               7 (False)
+                           248 LOAD_FAST                0 (self)
+                           250 STORE_ATTR               7 (closed)
+               
+                27         260 LOAD_GLOBAL             17 (NULL + sum)
+                           272 LOAD_FAST                0 (self)
+                           274 LOAD_ATTR                2 (sides)
+                           284 PRECALL                  1
+                           288 CALL                     1
+                           298 LOAD_FAST                0 (self)
+                           300 STORE_ATTR               9 (points)
+                           310 LOAD_CONST               6 (None)
+                           312 RETURN_VALUE
                consts
+                  '\n        Constructor\n\n        a: int                  -> First number on the piece\n        b: int                  -> Second number on the piece\n\n        linked: List[Piece]     -> Pieces played from this Piece\n        is_crossing: Bool       -> Whether Pieces can be appended to all four sides of this Piece\n        is_double: Bool         -> Whether both sides of the piece show the same number\n        closed: Bool            -> If a double piece is closed (face down), nothing can be appended to it\n        points: int             -> Point value of the piece, which is the combined value of both sides\n        '
+                  0
+                  6
+                  'Domino Piece sides can only have values 0-6, got ['
+                  '|'
+                  ']'
                   None
                   False
-               names      ('domino_set', 'pool', 'origin', 'Player', 'player1', 'player2', 'current_player', 'has_crossing')
-               varnames   ('self', 'brain1', 'brain2', 'begins')
+                  1
+               names      ('ValueError', 'sorted', 'sides', 'linked', 'linked_to', 'is_crossing', 'is_double', 'closed', 'sum', 'points')
+               varnames   ('self', 'a', 'b')
                freevars   ()
                cellvars   ()
-               filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py'
+               filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
                name       '__init__'
-               firstlineno 8
-               lnotab 0x020126010e012a012a014201
+               firstlineno 5
+               lnotab 0x020d30012c022c010e010e010e0142010e01
+            'piece'
             code
-               argcount  : 1
+               argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
-                  0x97007401000000000000000000006401a6010000ab0100000000000000
-                  0044005d347d017c006a010000000000000000a002000000000000000000
-                  0000000000000000000000a6000000ab00000000000000000001007c006a
-                  030000000000000000a00200000000000000000000000000000000000000
-                  00a6000000ab00000000000000000001008c3564005300
-                16           0 RESUME                   0
+                  0x97007c007c015f0000000000000000007c006a010000000000000000a0
+                  0200000000000000000000000000000000000000007c01a6010000ab0100
+                  0000000000000001007c006a030000000000000000722174090000000000
+                  00000000007c006a010000000000000000a6010000ab0100000000000000
+                  0064016b0200000000720b64027c005f0500000000000000006400530064
+                  00530064005300
+                29           0 RESUME                   0
                
-                18           2 LOAD_GLOBAL              1 (NULL + range)
-                            14 LOAD_CONST               1 (7)
-                            16 PRECALL                  1
-                            20 CALL                     1
-                            30 GET_ITER
-                       >>   32 FOR_ITER                52 (to 138)
-                            34 STORE_FAST               1 (i)
-               
-                19          36 LOAD_FAST                0 (self)
-                            38 LOAD_ATTR                1 (player1)
-                            48 LOAD_METHOD              2 (draw)
-                            70 PRECALL                  0
-                            74 CALL                     0
-                            84 POP_TOP
-               
-                20          86 LOAD_FAST                0 (self)
-                            88 LOAD_ATTR                3 (player2)
-                            98 LOAD_METHOD              2 (draw)
-                           120 PRECALL                  0
-                           124 CALL                     0
-                           134 POP_TOP
-                           136 JUMP_BACKWARD           53 (to 32)
+                30           2 LOAD_FAST                0 (self)
+                             4 LOAD_FAST                1 (piece)
+                             6 STORE_ATTR               0 (linked_to)
                
-                18     >>  138 LOAD_CONST               0 (None)
-                           140 RETURN_VALUE
+                31          16 LOAD_FAST                0 (self)
+                            18 LOAD_ATTR                1 (linked)
+                            28 LOAD_METHOD              2 (append)
+                            50 LOAD_FAST                1 (piece)
+                            52 PRECALL                  1
+                            56 CALL                     1
+                            66 POP_TOP
+               
+                32          68 LOAD_FAST                0 (self)
+                            70 LOAD_ATTR                3 (is_double)
+                            80 POP_JUMP_FORWARD_IF_FALSE    33 (to 148)
+                            82 LOAD_GLOBAL              9 (NULL + len)
+                            94 LOAD_FAST                0 (self)
+                            96 LOAD_ATTR                1 (linked)
+                           106 PRECALL                  1
+                           110 CALL                     1
+                           120 LOAD_CONST               1 (2)
+                           122 COMPARE_OP               2 (==)
+                           128 POP_JUMP_FORWARD_IF_FALSE    11 (to 152)
+               
+                33         130 LOAD_CONST               2 (True)
+                           132 LOAD_FAST                0 (self)
+                           134 STORE_ATTR               5 (is_crossing)
+                           144 LOAD_CONST               0 (None)
+                           146 RETURN_VALUE
+               
+                32     >>  148 LOAD_CONST               0 (None)
+                           150 RETURN_VALUE
+                       >>  152 LOAD_CONST               0 (None)
+                           154 RETURN_VALUE
                consts
                   None
-                  7
-               names      ('range', 'player1', 'draw', 'player2')
-               varnames   ('self', 'i')
+                  2
+                  True
+               names      ('linked_to', 'linked', 'append', 'is_double', 'len', 'is_crossing')
+               varnames   ('self', 'piece')
                freevars   ()
                cellvars   ()
-               filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py'
-               name       'deal_hand'
-               firstlineno 16
-               lnotab 0x02022201320134fe
+               filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
+               name       'append'
+               firstlineno 29
+               lnotab 0x02010e0134013e0112ff
             code
                argcount  : 1
-               nlocals   : 3
-               stacksize : 5
+               nlocals   : 1
+               stacksize : 1
                flags     : 3
-               code
-                  0x97007c006a0000000000000000008102640153007c006a000000000000
-                  000000805a640244005d4e7d017403000000000000000000007c017c01a6
-                  020000ab0200000000000000007d027c027c006a0200000000000000006a
-                  030000000000000000760072107c006a0200000000000000007c005f0000
-                  000000000000007c026302010053007c027c006a0400000000000000006a
-                  030000000000000000760072107c006a0200000000000000007c005f0000
-                  000000000000007c026302010053008c4f7c006a000000000000000000ae
-                  586401530064015300
-                22           0 RESUME                   0
-               
-                30           2 LOAD_FAST                0 (self)
-                             4 LOAD_ATTR                0 (current_player)
-                            14 POP_JUMP_FORWARD_IF_NONE     2 (to 20)
+               code 0x97007c006a000000000000000000720264016e0164025300
+                35           0 RESUME                   0
                
-                31          16 LOAD_CONST               1 (None)
-                            18 RETURN_VALUE
+                37           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (is_crossing)
+                            14 POP_JUMP_FORWARD_IF_FALSE     2 (to 20)
+                            16 LOAD_CONST               1 (4)
+                            18 JUMP_FORWARD             1 (to 22)
+                       >>   20 LOAD_CONST               2 (2)
+                       >>   22 RETURN_VALUE
+               consts
+                  None
+                  4
+                  2
+               names      ('is_crossing',)
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
+               name       'total_sides'
+               firstlineno 35
+               lnotab 0x0202
+            code
+               argcount  : 1
+               nlocals   : 2
+               stacksize : 3
+               flags     : 3
+               code
+                  0x97007401000000000000000000007c006a010000000000000000a60100
+                  00ab0100000000000000007d017c006a02000000000000000081057c0164
+                  017a0d00007d017c015300
+                39           0 RESUME                   0
+               
+                41           2 LOAD_GLOBAL              1 (NULL + len)
+                            14 LOAD_FAST                0 (self)
+                            16 LOAD_ATTR                1 (linked)
+                            26 PRECALL                  1
+                            30 CALL                     1
+                            40 STORE_FAST               1 (sides)
+               
+                42          42 LOAD_FAST                0 (self)
+                            44 LOAD_ATTR                2 (linked_to)
+                            54 POP_JUMP_FORWARD_IF_NONE     5 (to 66)
+               
+                43          56 LOAD_FAST                1 (sides)
+                            58 LOAD_CONST               1 (1)
+                            60 BINARY_OP               13 (+=)
+                            64 STORE_FAST               1 (sides)
                
-                33     >>   20 LOAD_FAST                0 (self)
-                            22 LOAD_ATTR                0 (current_player)
-                            32 POP_JUMP_FORWARD_IF_NOT_NONE    90 (to 214)
-               
-                34     >>   34 LOAD_CONST               2 ((5, 1, 2, 3, 4, 6, 0))
-                            36 GET_ITER
-                       >>   38 FOR_ITER                78 (to 196)
-                            40 STORE_FAST               1 (i)
-               
-                35          42 LOAD_GLOBAL              3 (NULL + Piece)
-                            54 LOAD_FAST                1 (i)
-                            56 LOAD_FAST                1 (i)
-                            58 PRECALL                  2
-                            62 CALL                     2
-                            72 STORE_FAST               2 (piece)
-               
-                37          74 LOAD_FAST                2 (piece)
-                            76 LOAD_FAST                0 (self)
-                            78 LOAD_ATTR                2 (player1)
-                            88 LOAD_ATTR                3 (hand)
-                            98 CONTAINS_OP              0
-                           100 POP_JUMP_FORWARD_IF_FALSE    16 (to 134)
-               
-                38         102 LOAD_FAST                0 (self)
-                           104 LOAD_ATTR                2 (player1)
-                           114 LOAD_FAST                0 (self)
-                           116 STORE_ATTR               0 (current_player)
-               
-                39         126 LOAD_FAST                2 (piece)
-                           128 SWAP                     2
-                           130 POP_TOP
-                           132 RETURN_VALUE
-               
-                40     >>  134 LOAD_FAST                2 (piece)
-                           136 LOAD_FAST                0 (self)
-                           138 LOAD_ATTR                4 (player2)
-                           148 LOAD_ATTR                3 (hand)
-                           158 CONTAINS_OP              0
-                           160 POP_JUMP_FORWARD_IF_FALSE    16 (to 194)
-               
-                41         162 LOAD_FAST                0 (self)
-                           164 LOAD_ATTR                2 (player1)
-                           174 LOAD_FAST                0 (self)
-                           176 STORE_ATTR               0 (current_player)
-               
-                42         186 LOAD_FAST                2 (piece)
-                           188 SWAP                     2
-                           190 POP_TOP
-                           192 RETURN_VALUE
-               
-                40     >>  194 JUMP_BACKWARD           79 (to 38)
-               
-                33     >>  196 LOAD_FAST                0 (self)
-                           198 LOAD_ATTR                0 (current_player)
-                           208 POP_JUMP_BACKWARD_IF_NONE    88 (to 34)
-                           210 LOAD_CONST               1 (None)
-                           212 RETURN_VALUE
-                       >>  214 LOAD_CONST               1 (None)
-                           216 RETURN_VALUE
+                44     >>   66 LOAD_FAST                1 (sides)
+                            68 RETURN_VALUE
                consts
-                  '\n        Find the piece a player is required to start with.\n\n        If no starting player is defined, the player with [5|5] begins.\n        If neither player has [5|5], the order goes [1|1], [2|2], ..., [6|6], [0|0].\n        If neither player has any double pieces, they draw a piece each until one does.\n        '
                   None
-                  (5, 1, 2, 3, 4, 6, 0)
-               names      ('current_player', 'Piece', 'player1', 'hand', 'player2')
-               varnames   ('self', 'i', 'piece')
+                  1
+               names      ('len', 'linked', 'linked_to')
+               varnames   ('self', 'sides')
                freevars   ()
                cellvars   ()
-               filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py'
-               name       'get_required_starting_piece'
-               firstlineno 22
-               lnotab 0x02080e0104020e01080120021c01180108011c01180108fe02f9
-            28
-            'piece'
+               filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
+               name       'closed_sides'
+               firstlineno 39
+               lnotab 0x020228010e010a01
+            code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 2
+               flags     : 3
+               code
+                  0x97007c006a0000000000000000007c006a0100000000000000007a0a00
+                  005300
+                46           0 RESUME                   0
+               
+                48           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (total_sides)
+                            14 LOAD_FAST                0 (self)
+                            16 LOAD_ATTR                1 (closed_sides)
+                            26 BINARY_OP               10 (-)
+                            30 RETURN_VALUE
+               consts
+                  None
+               names      ('total_sides', 'closed_sides')
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
+               name       'open_sides'
+               firstlineno 46
+               lnotab 0x0202
+            'other'
             'return'
             code
                argcount  : 2
                nlocals   : 4
-               stacksize : 7
+               stacksize : 2
                flags     : 3
                code
-                  0x97007c0164016b0000000000720f7401000000000000000000006402a6
-                  010000ab010000000000000000820164017d027c006a0100000000000000
-                  0080117c006a020000000000000000730a7c027c006a0300000000000000
-                  007a0d00007d027c006a02000000000000000073077c006a010000000000
-                  000000801f7c006a01000000000000000080477409000000000000000000
-                  007c006a020000000000000000a6010000ab01000000000000000064046b
-                  0200000000722f7c006a050000000000000000720b7c027c006a03000000
-                  00000000007a0d00007d026e1d7c027c00a0060000000000000000000000
-                  0000000000000000007c006a010000000000000000a6010000ab01000000
-                  00000000007a0d00007d027c006a07000000000000000072287409000000
-                  000000000000007c006a020000000000000000a6010000ab010000000000
-                  00000064056b020000000072107c027c006a080000000000000000640119
-                  0000000000000000007a0d00007d027c006a02000000000000000044005d
-                  1d7d037c027413000000000000000000006a0a00000000000000007c037c
-                  0164047a0a0000a6020000ab0200000000000000007a0d00007d028c1e7c
-                  025300
-                44           0 RESUME                   0
-               
-                50           2 LOAD_FAST                1 (depth)
-                             4 LOAD_CONST               1 (0)
-                             6 COMPARE_OP               0 (<)
-                            12 POP_JUMP_FORWARD_IF_FALSE    15 (to 44)
-               
-                51          14 LOAD_GLOBAL              1 (NULL + Exception)
-                            26 LOAD_CONST               2 ('Recursion too deep, some pieces linked in a loop?')
-                            28 PRECALL                  1
-                            32 CALL                     1
-                            42 RAISE_VARARGS            1
-               
-                53     >>   44 LOAD_CONST               1 (0)
-                            46 STORE_FAST               2 (score)
-               
-                56          48 LOAD_FAST                0 (piece)
-                            50 LOAD_ATTR                1 (linked_to)
-                            60 POP_JUMP_FORWARD_IF_NOT_NONE    17 (to 96)
-                            62 LOAD_FAST                0 (piece)
-                            64 LOAD_ATTR                2 (linked)
-                            74 POP_JUMP_FORWARD_IF_TRUE    10 (to 96)
-               
-                57          76 LOAD_FAST                2 (score)
-                            78 LOAD_FAST                0 (piece)
-                            80 LOAD_ATTR                3 (points)
-                            90 BINARY_OP               13 (+=)
-                            94 STORE_FAST               2 (score)
-               
-                60     >>   96 LOAD_FAST                0 (piece)
-                            98 LOAD_ATTR                2 (linked)
-                           108 POP_JUMP_FORWARD_IF_TRUE     7 (to 124)
-                           110 LOAD_FAST                0 (piece)
-                           112 LOAD_ATTR                1 (linked_to)
-                           122 POP_JUMP_FORWARD_IF_NOT_NONE    31 (to 186)
-                       >>  124 LOAD_FAST                0 (piece)
-                           126 LOAD_ATTR                1 (linked_to)
-                           136 POP_JUMP_FORWARD_IF_NOT_NONE    71 (to 280)
-                           138 LOAD_GLOBAL              9 (NULL + len)
-                           150 LOAD_FAST                0 (piece)
-                           152 LOAD_ATTR                2 (linked)
-                           162 PRECALL                  1
-                           166 CALL                     1
-                           176 LOAD_CONST               4 (1)
-                           178 COMPARE_OP               2 (==)
-                           184 POP_JUMP_FORWARD_IF_FALSE    47 (to 280)
-               
-                61     >>  186 LOAD_FAST                0 (piece)
-                           188 LOAD_ATTR                5 (is_double)
-                           198 POP_JUMP_FORWARD_IF_FALSE    11 (to 222)
-               
-                62         200 LOAD_FAST                2 (score)
-                           202 LOAD_FAST                0 (piece)
-                           204 LOAD_ATTR                3 (points)
-                           214 BINARY_OP               13 (+=)
-                           218 STORE_FAST               2 (score)
-                           220 JUMP_FORWARD            29 (to 280)
-               
-                64     >>  222 LOAD_FAST                2 (score)
-                           224 LOAD_FAST                0 (piece)
-                           226 LOAD_METHOD              6 (unlinked_side)
-                           248 LOAD_FAST                0 (piece)
-                           250 LOAD_ATTR                1 (linked_to)
-                           260 PRECALL                  1
-                           264 CALL                     1
-                           274 BINARY_OP               13 (+=)
-                           278 STORE_FAST               2 (score)
-               
-                67     >>  280 LOAD_FAST                0 (piece)
-                           282 LOAD_ATTR                7 (is_crossing)
-                           292 POP_JUMP_FORWARD_IF_FALSE    40 (to 374)
-                           294 LOAD_GLOBAL              9 (NULL + len)
-                           306 LOAD_FAST                0 (piece)
-                           308 LOAD_ATTR                2 (linked)
-                           318 PRECALL                  1
-                           322 CALL                     1
-                           332 LOAD_CONST               5 (3)
-                           334 COMPARE_OP               2 (==)
-                           340 POP_JUMP_FORWARD_IF_FALSE    16 (to 374)
-               
-                68         342 LOAD_FAST                2 (score)
-                           344 LOAD_FAST                0 (piece)
-                           346 LOAD_ATTR                8 (sides)
-                           356 LOAD_CONST               1 (0)
-                           358 BINARY_SUBSCR
-                           368 BINARY_OP               13 (+=)
-                           372 STORE_FAST               2 (score)
-               
-                71     >>  374 LOAD_FAST                0 (piece)
-                           376 LOAD_ATTR                2 (linked)
-                           386 GET_ITER
-                       >>  388 FOR_ITER                29 (to 448)
-                           390 STORE_FAST               3 (linked_piece)
-               
-                72         392 LOAD_FAST                2 (score)
-                           394 LOAD_GLOBAL             19 (NULL + Piece)
-                           406 LOAD_ATTR               10 (score_piece)
-                           416 LOAD_FAST                3 (linked_piece)
-                           418 LOAD_FAST                1 (depth)
-                           420 LOAD_CONST               4 (1)
-                           422 BINARY_OP               10 (-)
-                           426 PRECALL                  2
-                           430 CALL                     2
-                           440 BINARY_OP               13 (+=)
-                           444 STORE_FAST               2 (score)
-                           446 JUMP_BACKWARD           30 (to 388)
-               
-                74     >>  448 LOAD_FAST                2 (score)
-                           450 RETURN_VALUE
+                  0x97007c006a0000000000000000005c0200007d027d037c027c016a0000
+                  00000000000000760072027c036e017c025300
+                50           0 RESUME                   0
+               
+                51           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (sides)
+                            14 UNPACK_SEQUENCE          2
+                            18 STORE_FAST               2 (a)
+                            20 STORE_FAST               3 (b)
+               
+                52          22 LOAD_FAST                2 (a)
+                            24 LOAD_FAST                1 (other)
+                            26 LOAD_ATTR                0 (sides)
+                            36 CONTAINS_OP              0
+                            38 POP_JUMP_FORWARD_IF_FALSE     2 (to 44)
+                            40 LOAD_FAST                3 (b)
+                            42 JUMP_FORWARD             1 (to 46)
+                       >>   44 LOAD_FAST                2 (a)
+                       >>   46 RETURN_VALUE
                consts
-                  "\n        Calculate the score for a piece and it's attached pieces\n        "
-                  0
-                  'Recursion too deep, some pieces linked in a loop?'
                   None
+               names      ('sides',)
+               varnames   ('self', 'other', 'a', 'b')
+               freevars   ()
+               cellvars   ()
+               filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
+               name       'unlinked_side'
+               firstlineno 50
+               lnotab 0x02011401
+            code
+               argcount  : 1
+               nlocals   : 3
+               stacksize : 6
+               flags     : 3
+               code
+                  0x97007c006a000000000000000000720b64017d0164027c019b0064037c
+                  019b0064049d05530067006405a2017d0264027c027c006a010000000000
+                  000000640619000000000000000000190000000000000000009b0064037c
+                  027c006a0100000000000000006407190000000000000000001900000000
+                  00000000009b0064049d055300
+                54           0 RESUME                   0
+               
+                56           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (closed)
+                            14 POP_JUMP_FORWARD_IF_FALSE    11 (to 38)
+               
+                57          16 LOAD_CONST               1 ('▩')
+                            18 STORE_FAST               1 (closed)
+               
+                58          20 LOAD_CONST               2 ('[')
+                            22 LOAD_FAST                1 (closed)
+                            24 FORMAT_VALUE             0
+                            26 LOAD_CONST               3 ('|')
+                            28 LOAD_FAST                1 (closed)
+                            30 FORMAT_VALUE             0
+                            32 LOAD_CONST               4 (']')
+                            34 BUILD_STRING             5
+                            36 RETURN_VALUE
+               
+                60     >>   38 BUILD_LIST               0
+                            40 LOAD_CONST               5 (('□', '⚀', '⚁', '⚂', '⚃', '⚄', '⚅'))
+                            42 LIST_EXTEND              1
+                            44 STORE_FAST               2 (sides)
+               
+                70          46 LOAD_CONST               2 ('[')
+                            48 LOAD_FAST                2 (sides)
+                            50 LOAD_FAST                0 (self)
+                            52 LOAD_ATTR                1 (sides)
+                            62 LOAD_CONST               6 (0)
+                            64 BINARY_SUBSCR
+                            74 BINARY_SUBSCR
+                            84 FORMAT_VALUE             0
+                            86 LOAD_CONST               3 ('|')
+                            88 LOAD_FAST                2 (sides)
+                            90 LOAD_FAST                0 (self)
+                            92 LOAD_ATTR                1 (sides)
+                           102 LOAD_CONST               7 (1)
+                           104 BINARY_SUBSCR
+                           114 BINARY_SUBSCR
+                           124 FORMAT_VALUE             0
+                           126 LOAD_CONST               4 (']')
+                           128 BUILD_STRING             5
+                           130 RETURN_VALUE
+               consts
+                  'Simple visual representation using die face Unicode symbols'
+                  '▩'
+                  '['
+                  '|'
+                  ']'
+                  ('□', '⚀', '⚁', '⚂', '⚃', '⚄', '⚅')
+                  0
                   1
-                  3
-               names      ('Exception', 'linked_to', 'linked', 'points', 'len', 'is_double', 'unlinked_side', 'is_crossing', 'sides', 'Piece', 'score_piece')
-               varnames   ('piece', 'depth', 'score', 'linked_piece')
+               names      ('closed', 'sides')
+               varnames   ('self', 'closed', 'sides')
                freevars   ()
                cellvars   ()
-               filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py'
-               name       'score_piece'
-               firstlineno 44
-               lnotab 0x02060c011e0204031c0114035a010e0116023a033e01200312013802
+               filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
+               name       '__str__'
+               firstlineno 54
+               lnotab 0x02020e0104011202080a
             code
                argcount  : 1
-               nlocals   : 2
+               nlocals   : 1
+               stacksize : 3
+               flags     : 3
+               code
+                  0x97007401000000000000000000007c00a6010000ab0100000000000000
+                  005300
+                72           0 RESUME                   0
+               
+                74           2 LOAD_GLOBAL              1 (NULL + str)
+                            14 LOAD_FAST                0 (self)
+                            16 PRECALL                  1
+                            20 CALL                     1
+                            30 RETURN_VALUE
+               consts
+                  'Use string representation'
+               names      ('str',)
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
+               name       '__repr__'
+               firstlineno 72
+               lnotab 0x0202
+            code
+               argcount  : 1
+               nlocals   : 1
                stacksize : 3
                flags     : 3
                code
-                  0x97007c00a00000000000000000000000000000000000000000007c006a
-                  010000000000000000a6010000ab0100000000000000007d017c006a0200
-                  0000000000000078016a0300000000000000007c017a0d000063025f0300
-                  0000000000000064005300
+                  0x97007c006a00000000000000000064011900000000000000000064027a
+                  0500007c006a0000000000000000006403190000000000000000007a0000
+                  005300
                 76           0 RESUME                   0
                
-                77           2 LOAD_FAST                0 (self)
-                             4 LOAD_METHOD              0 (score_piece)
-                            26 LOAD_FAST                0 (self)
-                            28 LOAD_ATTR                1 (origin)
-                            38 PRECALL                  1
-                            42 CALL                     1
-                            52 STORE_FAST               1 (score)
-               
-                78          54 LOAD_FAST                0 (self)
-                            56 LOAD_ATTR                2 (current_player)
-                            66 COPY                     1
-                            68 LOAD_ATTR                3 (score)
-                            78 LOAD_FAST                1 (score)
-                            80 BINARY_OP               13 (+=)
-                            84 SWAP                     2
-                            86 STORE_ATTR               3 (score)
-                            96 LOAD_CONST               0 (None)
-                            98 RETURN_VALUE
+                78           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (sides)
+                            14 LOAD_CONST               1 (0)
+                            16 BINARY_SUBSCR
+                            26 LOAD_CONST               2 (10)
+                            28 BINARY_OP                5 (*)
+                            32 LOAD_FAST                0 (self)
+                            34 LOAD_ATTR                0 (sides)
+                            44 LOAD_CONST               3 (1)
+                            46 BINARY_SUBSCR
+                            56 BINARY_OP                0 (+)
+                            60 RETURN_VALUE
                consts
-                  None
-               names      ('score_piece', 'origin', 'current_player', 'score')
-               varnames   ('self', 'score')
+                  'Integer representation, e.g. 46 for a [4|6] piece'
+                  0
+                  10
+                  1
+               names      ('sides',)
+               varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py'
-               name       'score'
+               filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
+               name       '__hash__'
                firstlineno 76
-               lnotab 0x02013401
-            False
-            'player'
-            'origin'
-            None
+               lnotab 0x0202
             code
-               argcount  : 5
-               nlocals   : 5
-               stacksize : 6
+               argcount  : 2
+               nlocals   : 2
+               stacksize : 4
                flags     : 3
                code
-                  0x97007c027c016a00000000000000000076017213740300000000000000
-                  00000064017c029b0064029d03a6010000ab01000000000000000082017c
-                  026a02000000000000000072107c006a03000000000000000072097c0472
-                  0764037c025f0400000000000000007c016a000000000000000000a00500
-                  000000000000000000000000000000000000007c02a6010000ab01000000
-                  000000000001007c0380297c006a060000000000000000811a7403000000
-                  0000000000000064017c029b0064047c006a0600000000000000009b009d
-                  04a6010000ab01000000000000000082017c027c005f0600000000000000
-                  006e157c03a00700000000000000000000000000000000000000007c02a6
-                  010000ab01000000000000000001007c00a0080000000000000000000000
-                  000000000000000000a6000000ab00000000000000000001007c006a0900
-                  000000000000007c006a0a00000000000000006b0200000000720e7c006a
-                  0b00000000000000007c005f090000000000000000640053007c006a0a00
-                  000000000000007c005f09000000000000000064005300
+                  0x97007401000000000000000000007c00a6010000ab0100000000000000
+                  007401000000000000000000007c01a6010000ab0100000000000000006b
+                  02000000005300
                 80           0 RESUME                   0
                
-                81           2 LOAD_FAST                2 (piece)
-                             4 LOAD_FAST                1 (player)
-                             6 LOAD_ATTR                0 (hand)
-                            16 CONTAINS_OP              1
-                            18 POP_JUMP_FORWARD_IF_FALSE    19 (to 58)
-               
-                82          20 LOAD_GLOBAL              3 (NULL + Exception)
-                            32 LOAD_CONST               1 ('Player attempted to play ')
-                            34 LOAD_FAST                2 (piece)
-                            36 FORMAT_VALUE             0
-                            38 LOAD_CONST               2 (", but it's not in their hand")
-                            40 BUILD_STRING             3
-                            42 PRECALL                  1
-                            46 CALL                     1
-                            56 RAISE_VARARGS            1
-               
-                84     >>   58 LOAD_FAST                2 (piece)
-                            60 LOAD_ATTR                2 (is_double)
-                            70 POP_JUMP_FORWARD_IF_FALSE    16 (to 104)
-                            72 LOAD_FAST                0 (self)
-                            74 LOAD_ATTR                3 (has_crossing)
-                            84 POP_JUMP_FORWARD_IF_FALSE     9 (to 104)
-                            86 LOAD_FAST                4 (close)
-                            88 POP_JUMP_FORWARD_IF_FALSE     7 (to 104)
-               
-                85          90 LOAD_CONST               3 (True)
-                            92 LOAD_FAST                2 (piece)
-                            94 STORE_ATTR               4 (closed)
-               
-                87     >>  104 LOAD_FAST                1 (player)
-                           106 LOAD_ATTR                0 (hand)
-                           116 LOAD_METHOD              5 (pop)
-                           138 LOAD_FAST                2 (piece)
-                           140 PRECALL                  1
-                           144 CALL                     1
-                           154 POP_TOP
-               
-                89         156 LOAD_FAST                3 (origin)
-                           158 POP_JUMP_FORWARD_IF_NOT_NONE    41 (to 242)
-               
-                90         160 LOAD_FAST                0 (self)
-                           162 LOAD_ATTR                6 (origin)
-                           172 POP_JUMP_FORWARD_IF_NONE    26 (to 226)
-               
-                91         174 LOAD_GLOBAL              3 (NULL + Exception)
-                           186 LOAD_CONST               1 ('Player attempted to play ')
-                           188 LOAD_FAST                2 (piece)
-                           190 FORMAT_VALUE             0
-                           192 LOAD_CONST               4 (' as origin, but there is already origin piece ')
-               
-                92         194 LOAD_FAST                0 (self)
-                           196 LOAD_ATTR                6 (origin)
-               
-                91         206 FORMAT_VALUE             0
-                           208 BUILD_STRING             4
-                           210 PRECALL                  1
-                           214 CALL                     1
-                           224 RAISE_VARARGS            1
-               
-                93     >>  226 LOAD_FAST                2 (piece)
-                           228 LOAD_FAST                0 (self)
-                           230 STORE_ATTR               6 (origin)
-                           240 JUMP_FORWARD            21 (to 284)
-               
-                95     >>  242 LOAD_FAST                3 (origin)
-                           244 LOAD_METHOD              7 (append)
-                           266 LOAD_FAST                2 (piece)
-                           268 PRECALL                  1
-                           272 CALL                     1
-                           282 POP_TOP
-               
-                96     >>  284 LOAD_FAST                0 (self)
-                           286 LOAD_METHOD              8 (score)
-                           308 PRECALL                  0
-                           312 CALL                     0
-                           322 POP_TOP
-               
-                98         324 LOAD_FAST                0 (self)
-                           326 LOAD_ATTR                9 (current_player)
-                           336 LOAD_FAST                0 (self)
-                           338 LOAD_ATTR               10 (player1)
-                           348 COMPARE_OP               2 (==)
-                           354 POP_JUMP_FORWARD_IF_FALSE    14 (to 384)
-               
-                99         356 LOAD_FAST                0 (self)
-                           358 LOAD_ATTR               11 (player2)
-                           368 LOAD_FAST                0 (self)
-                           370 STORE_ATTR               9 (current_player)
-                           380 LOAD_CONST               0 (None)
-                           382 RETURN_VALUE
-               
-               101     >>  384 LOAD_FAST                0 (self)
-                           386 LOAD_ATTR               10 (player1)
-                           396 LOAD_FAST                0 (self)
-                           398 STORE_ATTR               9 (current_player)
-                           408 LOAD_CONST               0 (None)
-                           410 RETURN_VALUE
+                82           2 LOAD_GLOBAL              1 (NULL + hash)
+                            14 LOAD_FAST                0 (self)
+                            16 PRECALL                  1
+                            20 CALL                     1
+                            30 LOAD_GLOBAL              1 (NULL + hash)
+                            42 LOAD_FAST                1 (other)
+                            44 PRECALL                  1
+                            48 CALL                     1
+                            58 COMPARE_OP               2 (==)
+                            64 RETURN_VALUE
                consts
-                  None
-                  'Player attempted to play '
-                  ", but it's not in their hand"
-                  True
-                  ' as origin, but there is already origin piece '
-               names      ('hand', 'Exception', 'is_double', 'has_crossing', 'closed', 'pop', 'origin', 'append', 'score', 'current_player', 'player1', 'player2')
-               varnames   ('self', 'player', 'piece', 'origin', 'close')
+                  'Returns whether the pieces are equal based on their hash'
+               names      ('hash',)
+               varnames   ('self', 'other')
                freevars   ()
                cellvars   ()
-               filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py'
-               name       'play'
+               filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
+               name       '__eq__'
                firstlineno 80
-               lnotab
-                  0x02011201260220010e02340204010e0114010cff140210022a01280220
-                  011c02
+               lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 2
-               stacksize : 1
+               stacksize : 2
                flags     : 3
-               code 0x970067005300
-               103           0 RESUME                   0
-               
-               104           2 BUILD_LIST               0
-                             4 RETURN_VALUE
+               code
+                  0x97007c006a0000000000000000007c016a0000000000000000006b0000
+                  0000005300
+                84           0 RESUME                   0
+               
+                86           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (points)
+                            14 LOAD_FAST                1 (other)
+                            16 LOAD_ATTR                0 (points)
+                            26 COMPARE_OP               0 (<)
+                            32 RETURN_VALUE
                consts
-                  None
-               names      ()
-               varnames   ('self', 'hand')
+                  'Returns whether a piece is bigger based on point value'
+               names      ('points',)
+               varnames   ('self', 'other')
                freevars   ()
                cellvars   ()
-               filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py'
-               name       'valid_options'
-               firstlineno 103
-               lnotab 0x0201
+               filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
+               name       '__lt__'
+               firstlineno 84
+               lnotab 0x0202
             code
-               argcount  : 1
+               argcount  : 2
                nlocals   : 2
-               stacksize : 5
+               stacksize : 2
                flags     : 3
                code
-                  0x97007c00a0000000000000000000000000000000000000000000a60000
-                  00ab0000000000000000007d017c01811c7c00a001000000000000000000
-                  00000000000000000000007c006a0200000000000000007c016400a60300
-                  00ab0300000000000000000100090009008c02
-               106           0 RESUME                   0
-               
-               107           2 LOAD_FAST                0 (self)
-                             4 LOAD_METHOD              0 (get_required_starting_piece)
-                            26 PRECALL                  0
-                            30 CALL                     0
-                            40 STORE_FAST               1 (starting_piece)
-               
-               108          42 LOAD_FAST                1 (starting_piece)
-                            44 POP_JUMP_FORWARD_IF_NONE    28 (to 102)
-               
-               109          46 LOAD_FAST                0 (self)
-                            48 LOAD_METHOD              1 (play)
-                            70 LOAD_FAST                0 (self)
-                            72 LOAD_ATTR                2 (current_player)
-                            82 LOAD_FAST                1 (starting_piece)
-                            84 LOAD_CONST               0 (None)
-                            86 PRECALL                  3
-                            90 CALL                     3
-                           100 POP_TOP
-               
-               111     >>  102 NOP
-               
-               112     >>  104 NOP
-               
-               111         106 JUMP_BACKWARD            2 (to 104)
+                  0x97007c006a0000000000000000007c016a0000000000000000006b0400
+                  0000005300
+                88           0 RESUME                   0
+               
+                90           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (points)
+                            14 LOAD_FAST                1 (other)
+                            16 LOAD_ATTR                0 (points)
+                            26 COMPARE_OP               4 (>)
+                            32 RETURN_VALUE
                consts
-                  None
-               names      ('get_required_starting_piece', 'play', 'current_player')
-               varnames   ('self', 'starting_piece')
+                  'Returns whether a piece is smaller based on point value'
+               names      ('points',)
+               varnames   ('self', 'other')
                freevars   ()
                cellvars   ()
-               filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py'
-               name       'run'
-               firstlineno 106
-               lnotab 0x0201280104013802020102ff
-            (28,)
-            (False,)
-         names      ('__name__', '__module__', '__qualname__', 'Union', '__init__', 'deal_hand', 'get_required_starting_piece', 'staticmethod', 'Piece', 'int', 'score_piece', 'score', 'Player', 'play', 'valid_options', 'run')
+               filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
+               name       '__gt__'
+               firstlineno 88
+               lnotab 0x0202
+            None
+            ('piece', 'Piece')
+         names      ('__name__', '__module__', '__qualname__', 'int', '__init__', 'append', 'property', 'total_sides', 'closed_sides', 'open_sides', 'unlinked_side', '__str__', '__repr__', '__hash__', '__eq__', '__lt__', '__gt__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py'
-         name       'DominoRound'
-         firstlineno 7
-         lnotab 0x0a01200806060616020110ff0e01021f060426170603
-      'DominoRound'
+         filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
+         name       'Piece'
+         firstlineno 4
+         lnotab
+            0x0a0110180806020104ff0e010203020104ff0e010206020104ff0e0102
+            03100406120604060406040604
+      'Piece'
+      code
+         argcount  : 0
+         nlocals   : 3
+         stacksize : 8
+         flags     : 3
+         code
+            0x9700740100000000000000000000a6000000ab0000000000000000007d
+            007403000000000000000000006401a6010000ab01000000000000000044
+            005d3d7d017403000000000000000000006401a6010000ab010000000000
+            00000044005d2b7d027c017c026b010000000072237c00a0020000000000
+            0000000000000000000000000000007407000000000000000000007c017c
+            02a6020000ab020000000000000000a6010000ab01000000000000000001
+            008c2c8c3e7409000000000000000000007c00a6010000ab010000000000
+            0000005300
+          93           0 RESUME                   0
+         
+          94           2 LOAD_GLOBAL              1 (NULL + set)
+                      14 PRECALL                  0
+                      18 CALL                     0
+                      28 STORE_FAST               0 (pieces)
+         
+          95          30 LOAD_GLOBAL              3 (NULL + range)
+                      42 LOAD_CONST               1 (7)
+                      44 PRECALL                  1
+                      48 CALL                     1
+                      58 GET_ITER
+                 >>   60 FOR_ITER                61 (to 184)
+                      62 STORE_FAST               1 (i)
+         
+          96          64 LOAD_GLOBAL              3 (NULL + range)
+                      76 LOAD_CONST               1 (7)
+                      78 PRECALL                  1
+                      82 CALL                     1
+                      92 GET_ITER
+                 >>   94 FOR_ITER                43 (to 182)
+                      96 STORE_FAST               2 (j)
+         
+          97          98 LOAD_FAST                1 (i)
+                     100 LOAD_FAST                2 (j)
+                     102 COMPARE_OP               1 (<=)
+                     108 POP_JUMP_FORWARD_IF_FALSE    35 (to 180)
+         
+          98         110 LOAD_FAST                0 (pieces)
+                     112 LOAD_METHOD              2 (add)
+                     134 LOAD_GLOBAL              7 (NULL + Piece)
+                     146 LOAD_FAST                1 (i)
+                     148 LOAD_FAST                2 (j)
+                     150 PRECALL                  2
+                     154 CALL                     2
+                     164 PRECALL                  1
+                     168 CALL                     1
+                     178 POP_TOP
+                 >>  180 JUMP_BACKWARD           44 (to 94)
+         
+          96     >>  182 JUMP_BACKWARD           62 (to 60)
+         
+         100     >>  184 LOAD_GLOBAL              9 (NULL + sorted)
+                     196 LOAD_FAST                0 (pieces)
+                     198 PRECALL                  1
+                     202 CALL                     1
+                     212 RETURN_VALUE
+         consts
+            None
+            7
+         names      ('set', 'range', 'add', 'Piece', 'sorted')
+         varnames   ('pieces', 'i', 'j')
+         freevars   ()
+         cellvars   ()
+         filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
+         name       'domino_set'
+         firstlineno 93
+         lnotab 0x02011c01220122010c0148fe0204
       None
-   names      ('typing', 'Union', 'List', 'Tuple', 'src.main.game.Piece', 'domino_set', 'Piece', 'src.main.player.Player', 'Player', 'DominoRound')
+   names      ('typing', 'List', 'Union', 'Piece', 'domino_set')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py'
+   filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/Piece.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff0201140210010c03
+   lnotab 0x00ff020110031a59
```

### Comparing `all-fives-domino-1.0.8/src/main/player/Hand.py` & `all-fives-domino-1.0.9/src/main/player/Hand.py`

 * *Files identical despite different names*

### Comparing `all-fives-domino-1.0.8/src/main/player/__pycache__/Hand.cpython-311.pyc` & `all-fives-domino-1.0.9/src/main/player/__pycache__/Hand.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `all-fives-domino-1.0.8/src/main/player/__pycache__/Player.cpython-311.pyc` & `all-fives-domino-1.0.9/src/main/player/__pycache__/Player.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `all-fives-domino-1.0.8/src/test/game/__pycache__/test_pieces.cpython-311-pytest-7.3.1.pyc` & `all-fives-domino-1.0.9/src/test/game/__pycache__/test_pieces.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `all-fives-domino-1.0.8/src/test/game/__pycache__/test_round.cpython-311-pytest-7.3.1.pyc` & `all-fives-domino-1.0.9/src/test/game/__pycache__/test_round.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `all-fives-domino-1.0.8/src/test/game/test_pieces.py` & `all-fives-domino-1.0.9/src/test/game/test_pieces.py`

 * *Files identical despite different names*

### Comparing `all-fives-domino-1.0.8/src/test/player/__pycache__/test_hand.cpython-311-pytest-7.3.1.pyc` & `all-fives-domino-1.0.9/src/test/player/__pycache__/test_hand.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `all-fives-domino-1.0.8/src/test/player/test_hand.py` & `all-fives-domino-1.0.9/src/test/player/test_hand.py`

 * *Files identical despite different names*

