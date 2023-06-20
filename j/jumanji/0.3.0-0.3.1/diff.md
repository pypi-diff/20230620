# Comparing `tmp/jumanji-0.3.0.tar.gz` & `tmp/jumanji-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jumanji-0.3.0.tar", last modified: Fri Jun  9 16:54:07 2023, max compression
+gzip compressed data, was "jumanji-0.3.1.tar", last modified: Tue Jun 20 15:44:49 2023, max compression
```

## Comparing `jumanji-0.3.0.tar` & `jumanji-0.3.1.tar`

### file list

```diff
@@ -1,295 +1,295 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.481079 jumanji-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-09 16:53:56.000000 jumanji-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-09 16:53:56.000000 jumanji-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18237 2023-06-09 16:54:07.481079 jumanji-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17282 2023-06-09 16:53:56.000000 jumanji-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.433078 jumanji-0.3.0/jumanji/
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.437078 jumanji-0.3.0/jumanji/environments/
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.437078 jumanji-0.3.0/jumanji/environments/commons/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/commons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.437078 jumanji-0.3.0/jumanji/environments/commons/maze_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/commons/maze_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/commons/maze_utils/maze_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/commons/maze_utils/maze_rendering.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/commons/maze_utils/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.437078 jumanji-0.3.0/jumanji/environments/logic/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.437078 jumanji-0.3.0/jumanji/environments/logic/game_2048/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/game_2048/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12404 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/game_2048/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/game_2048/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/game_2048/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/game_2048/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.441078 jumanji-0.3.0/jumanji/environments/logic/graph_coloring/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/graph_coloring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/graph_coloring/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/graph_coloring/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/graph_coloring/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/graph_coloring/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.441078 jumanji-0.3.0/jumanji/environments/logic/minesweeper/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/minesweeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/minesweeper/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/minesweeper/done.py
--rw-r--r--   0 runner    (1001) docker     (123)    11768 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/minesweeper/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/minesweeper/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/minesweeper/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/minesweeper/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/minesweeper/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/minesweeper/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.441078 jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9746 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.445078 jumanji-0.3.0/jumanji/environments/logic/sudoku/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/sudoku/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/sudoku/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.445078 jumanji-0.3.0/jumanji/environments/logic/sudoku/data/
--rw-r--r--   0 runner    (1001) docker     (123)   810128 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/sudoku/data/10000_mixed_puzzles.npy
--rw-r--r--   0 runner    (1001) docker     (123)    81128 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/sudoku/data/1000_very_easy_puzzles.npy
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/sudoku/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/sudoku/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/sudoku/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/sudoku/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/sudoku/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/sudoku/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/sudoku/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.445078 jumanji-0.3.0/jumanji/environments/packing/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.445078 jumanji-0.3.0/jumanji/environments/packing/bin_pack/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/bin_pack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30996 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/bin_pack/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    31516 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/bin_pack/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/bin_pack/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/bin_pack/space.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/bin_pack/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/bin_pack/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.449079 jumanji-0.3.0/jumanji/environments/packing/job_shop/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/job_shop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24068 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/job_shop/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/job_shop/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/job_shop/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/job_shop/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.449079 jumanji-0.3.0/jumanji/environments/packing/knapsack/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/knapsack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/knapsack/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/knapsack/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/knapsack/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/knapsack/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/knapsack/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.453079 jumanji-0.3.0/jumanji/environments/packing/tetris/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/tetris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/tetris/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    14175 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/tetris/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/tetris/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/tetris/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/tetris/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.453079 jumanji-0.3.0/jumanji/environments/routing/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.453079 jumanji-0.3.0/jumanji/environments/routing/cleaner/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/cleaner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/cleaner/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    15120 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/cleaner/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/cleaner/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/cleaner/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/cleaner/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.453079 jumanji-0.3.0/jumanji/environments/routing/connector/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/connector/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    14491 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/connector/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    22636 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/connector/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/connector/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/connector/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/connector/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/connector/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.453079 jumanji-0.3.0/jumanji/environments/routing/cvrp/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/cvrp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/cvrp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    14532 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/cvrp/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/cvrp/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/cvrp/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/cvrp/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/cvrp/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.457079 jumanji-0.3.0/jumanji/environments/routing/maze/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/maze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/maze/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12892 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/maze/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/maze/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/maze/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/maze/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.457079 jumanji-0.3.0/jumanji/environments/routing/mmst/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/mmst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/mmst/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    24530 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/mmst/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/mmst/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/mmst/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/mmst/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    20495 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/mmst/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11708 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/mmst/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.457079 jumanji-0.3.0/jumanji/environments/routing/multi_cvrp/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/multi_cvrp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/multi_cvrp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    17123 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/multi_cvrp/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/multi_cvrp/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/multi_cvrp/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/multi_cvrp/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/multi_cvrp/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/multi_cvrp/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9209 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/multi_cvrp/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.461079 jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    19997 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/utils_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/utils_shelf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/utils_spawn.py
--rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.461079 jumanji-0.3.0/jumanji/environments/routing/snake/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/snake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/snake/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/snake/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/snake/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.461079 jumanji-0.3.0/jumanji/environments/routing/tsp/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/tsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/tsp/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/tsp/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/tsp/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/tsp/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/tsp/viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)    21752 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.465079 jumanji-0.3.0/jumanji/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/testing/env_not_smoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     9142 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/testing/fakes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/testing/pytrees.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.465079 jumanji-0.3.0/jumanji/training/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.465079 jumanji-0.3.0/jumanji/training/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.465079 jumanji-0.3.0/jumanji/training/agents/a2c/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/agents/a2c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9577 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/agents/a2c/a2c_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/agents/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.465079 jumanji-0.3.0/jumanji/training/agents/random/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/agents/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/agents/random/random_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.469079 jumanji-0.3.0/jumanji/training/networks/
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.469079 jumanji-0.3.0/jumanji/training/networks/bin_pack/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/bin_pack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/bin_pack/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/bin_pack/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.469079 jumanji-0.3.0/jumanji/training/networks/cleaner/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/cleaner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/cleaner/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/cleaner/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.469079 jumanji-0.3.0/jumanji/training/networks/connector/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/connector/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/connector/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.469079 jumanji-0.3.0/jumanji/training/networks/cvrp/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/cvrp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/cvrp/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/cvrp/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/distribution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.473079 jumanji-0.3.0/jumanji/training/networks/game_2048/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/game_2048/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/game_2048/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/game_2048/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.473079 jumanji-0.3.0/jumanji/training/networks/graph_coloring/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/graph_coloring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/graph_coloring/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/graph_coloring/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.473079 jumanji-0.3.0/jumanji/training/networks/job_shop/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/job_shop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13904 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/job_shop/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/job_shop/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.473079 jumanji-0.3.0/jumanji/training/networks/knapsack/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/knapsack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/knapsack/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/knapsack/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/masked_categorical_random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.473079 jumanji-0.3.0/jumanji/training/networks/maze/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/maze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/maze/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/maze/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.473079 jumanji-0.3.0/jumanji/training/networks/minesweeper/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/minesweeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/minesweeper/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/minesweeper/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.473079 jumanji-0.3.0/jumanji/training/networks/mmst/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/mmst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/mmst/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/mmst/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.477079 jumanji-0.3.0/jumanji/training/networks/multi_cvrp/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/multi_cvrp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/multi_cvrp/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/multi_cvrp/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/parametric_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.477079 jumanji-0.3.0/jumanji/training/networks/robot_warehouse/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/robot_warehouse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/robot_warehouse/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/robot_warehouse/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.477079 jumanji-0.3.0/jumanji/training/networks/rubiks_cube/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/rubiks_cube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/rubiks_cube/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/rubiks_cube/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.477079 jumanji-0.3.0/jumanji/training/networks/snake/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/snake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/snake/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/snake/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.477079 jumanji-0.3.0/jumanji/training/networks/sudoku/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/sudoku/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/sudoku/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/sudoku/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.477079 jumanji-0.3.0/jumanji/training/networks/tetris/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/tetris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/tetris/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/tetris/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/transformer_block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.481079 jumanji-0.3.0/jumanji/training/networks/tsp/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/tsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9602 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/tsp/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/tsp/random.py
--rw-r--r--   0 runner    (1001) docker     (123)    18340 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/setup_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/tree_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    25577 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.437078 jumanji-0.3.0/jumanji.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18237 2023-06-09 16:54:07.000000 jumanji-0.3.0/jumanji.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10569 2023-06-09 16:54:07.000000 jumanji-0.3.0/jumanji.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 16:54:07.000000 jumanji-0.3.0/jumanji.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 16:54:07.000000 jumanji-0.3.0/jumanji.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-09 16:54:07.000000 jumanji-0.3.0/jumanji.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 16:54:07.000000 jumanji-0.3.0/jumanji.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-09 16:53:56.000000 jumanji-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.481079 jumanji-0.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-09 16:53:56.000000 jumanji-0.3.0/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-09 16:53:56.000000 jumanji-0.3.0/requirements/requirements-train.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 16:53:56.000000 jumanji-0.3.0/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-09 16:54:07.481079 jumanji-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-09 16:53:56.000000 jumanji-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.413550 jumanji-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-20 15:44:36.000000 jumanji-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-20 15:44:36.000000 jumanji-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18452 2023-06-20 15:44:49.413550 jumanji-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17497 2023-06-20 15:44:36.000000 jumanji-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.365549 jumanji-0.3.1/jumanji/
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.369549 jumanji-0.3.1/jumanji/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.369549 jumanji-0.3.1/jumanji/environments/commons/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/commons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.369549 jumanji-0.3.1/jumanji/environments/commons/maze_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/commons/maze_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/commons/maze_utils/maze_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/commons/maze_utils/maze_rendering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/commons/maze_utils/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.369549 jumanji-0.3.1/jumanji/environments/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.369549 jumanji-0.3.1/jumanji/environments/logic/game_2048/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/game_2048/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11869 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/game_2048/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/game_2048/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/game_2048/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/game_2048/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.369549 jumanji-0.3.1/jumanji/environments/logic/graph_coloring/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/graph_coloring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/graph_coloring/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/graph_coloring/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/graph_coloring/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/graph_coloring/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.373549 jumanji-0.3.1/jumanji/environments/logic/minesweeper/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/minesweeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/minesweeper/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/minesweeper/done.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11768 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/minesweeper/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/minesweeper/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/minesweeper/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/minesweeper/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/minesweeper/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/minesweeper/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.373549 jumanji-0.3.1/jumanji/environments/logic/rubiks_cube/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/rubiks_cube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/rubiks_cube/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9746 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/rubiks_cube/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/rubiks_cube/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/rubiks_cube/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/rubiks_cube/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/rubiks_cube/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/rubiks_cube/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.377550 jumanji-0.3.1/jumanji/environments/logic/sudoku/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/sudoku/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/sudoku/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.377550 jumanji-0.3.1/jumanji/environments/logic/sudoku/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   810128 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/sudoku/data/10000_mixed_puzzles.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    81128 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/sudoku/data/1000_very_easy_puzzles.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/sudoku/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/sudoku/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/sudoku/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/sudoku/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/sudoku/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/sudoku/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/logic/sudoku/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.377550 jumanji-0.3.1/jumanji/environments/packing/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/packing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.377550 jumanji-0.3.1/jumanji/environments/packing/bin_pack/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/packing/bin_pack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30996 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/packing/bin_pack/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31516 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/packing/bin_pack/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/packing/bin_pack/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/packing/bin_pack/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/packing/bin_pack/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/packing/bin_pack/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.381549 jumanji-0.3.1/jumanji/environments/packing/job_shop/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/packing/job_shop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24068 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/packing/job_shop/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/packing/job_shop/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/packing/job_shop/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/packing/job_shop/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.381549 jumanji-0.3.1/jumanji/environments/packing/knapsack/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/packing/knapsack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/packing/knapsack/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/packing/knapsack/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/packing/knapsack/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/packing/knapsack/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/packing/knapsack/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.381549 jumanji-0.3.1/jumanji/environments/packing/tetris/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/packing/tetris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/packing/tetris/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14175 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/packing/tetris/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/packing/tetris/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/packing/tetris/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/packing/tetris/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.381549 jumanji-0.3.1/jumanji/environments/routing/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.385549 jumanji-0.3.1/jumanji/environments/routing/cleaner/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/cleaner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/cleaner/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15120 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/cleaner/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/cleaner/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/cleaner/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/cleaner/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.385549 jumanji-0.3.1/jumanji/environments/routing/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/connector/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14491 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/connector/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22636 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/connector/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/connector/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/connector/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/connector/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/connector/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.385549 jumanji-0.3.1/jumanji/environments/routing/cvrp/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/cvrp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/cvrp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14532 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/cvrp/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/cvrp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/cvrp/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/cvrp/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/cvrp/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.389550 jumanji-0.3.1/jumanji/environments/routing/maze/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/maze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/maze/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12892 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/maze/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/maze/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/maze/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/maze/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.389550 jumanji-0.3.1/jumanji/environments/routing/mmst/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/mmst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/mmst/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24530 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/mmst/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/mmst/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/mmst/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/mmst/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20495 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/mmst/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11708 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/mmst/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.393550 jumanji-0.3.1/jumanji/environments/routing/multi_cvrp/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/multi_cvrp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/multi_cvrp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17123 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/multi_cvrp/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/multi_cvrp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/multi_cvrp/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/multi_cvrp/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/multi_cvrp/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/multi_cvrp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9209 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/multi_cvrp/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.393550 jumanji-0.3.1/jumanji/environments/routing/robot_warehouse/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/robot_warehouse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/robot_warehouse/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19997 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/robot_warehouse/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/robot_warehouse/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/robot_warehouse/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/robot_warehouse/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/robot_warehouse/utils_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/robot_warehouse/utils_shelf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/robot_warehouse/utils_spawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/robot_warehouse/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.393550 jumanji-0.3.1/jumanji/environments/routing/snake/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/snake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/snake/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/snake/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/snake/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.397550 jumanji-0.3.1/jumanji/environments/routing/tsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/tsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/tsp/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/tsp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/tsp/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/tsp/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/environments/routing/tsp/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21752 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.397550 jumanji-0.3.1/jumanji/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/testing/env_not_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9142 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/testing/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/testing/pytrees.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.397550 jumanji-0.3.1/jumanji/training/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.397550 jumanji-0.3.1/jumanji/training/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.397550 jumanji-0.3.1/jumanji/training/agents/a2c/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/agents/a2c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9577 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/agents/a2c/a2c_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/agents/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.401550 jumanji-0.3.1/jumanji/training/agents/random/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/agents/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/agents/random/random_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.401550 jumanji-0.3.1/jumanji/training/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.401550 jumanji-0.3.1/jumanji/training/networks/bin_pack/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/bin_pack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/bin_pack/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/bin_pack/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.401550 jumanji-0.3.1/jumanji/training/networks/cleaner/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/cleaner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/cleaner/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/cleaner/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.401550 jumanji-0.3.1/jumanji/training/networks/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/connector/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/connector/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.405550 jumanji-0.3.1/jumanji/training/networks/cvrp/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/cvrp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/cvrp/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/cvrp/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/distribution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.405550 jumanji-0.3.1/jumanji/training/networks/game_2048/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/game_2048/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/game_2048/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/game_2048/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.405550 jumanji-0.3.1/jumanji/training/networks/graph_coloring/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/graph_coloring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/graph_coloring/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/graph_coloring/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.405550 jumanji-0.3.1/jumanji/training/networks/job_shop/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/job_shop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13904 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/job_shop/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/job_shop/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.405550 jumanji-0.3.1/jumanji/training/networks/knapsack/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/knapsack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/knapsack/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/knapsack/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/masked_categorical_random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.405550 jumanji-0.3.1/jumanji/training/networks/maze/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/maze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/maze/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/maze/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.405550 jumanji-0.3.1/jumanji/training/networks/minesweeper/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/minesweeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/minesweeper/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/minesweeper/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.409550 jumanji-0.3.1/jumanji/training/networks/mmst/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/mmst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/mmst/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/mmst/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.409550 jumanji-0.3.1/jumanji/training/networks/multi_cvrp/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/multi_cvrp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/multi_cvrp/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/multi_cvrp/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/parametric_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.409550 jumanji-0.3.1/jumanji/training/networks/robot_warehouse/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/robot_warehouse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/robot_warehouse/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/robot_warehouse/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.409550 jumanji-0.3.1/jumanji/training/networks/rubiks_cube/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/rubiks_cube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/rubiks_cube/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/rubiks_cube/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.409550 jumanji-0.3.1/jumanji/training/networks/snake/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/snake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/snake/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/snake/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.409550 jumanji-0.3.1/jumanji/training/networks/sudoku/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/sudoku/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/sudoku/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/sudoku/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.413550 jumanji-0.3.1/jumanji/training/networks/tetris/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/tetris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/tetris/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/tetris/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/transformer_block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.413550 jumanji-0.3.1/jumanji/training/networks/tsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/tsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9602 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/tsp/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/networks/tsp/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18340 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/setup_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/training/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/tree_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25578 2023-06-20 15:44:36.000000 jumanji-0.3.1/jumanji/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.369549 jumanji-0.3.1/jumanji.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18452 2023-06-20 15:44:49.000000 jumanji-0.3.1/jumanji.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10569 2023-06-20 15:44:49.000000 jumanji-0.3.1/jumanji.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:44:49.000000 jumanji-0.3.1/jumanji.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:44:49.000000 jumanji-0.3.1/jumanji.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-20 15:44:49.000000 jumanji-0.3.1/jumanji.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 15:44:49.000000 jumanji-0.3.1/jumanji.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-20 15:44:36.000000 jumanji-0.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:44:49.413550 jumanji-0.3.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-20 15:44:36.000000 jumanji-0.3.1/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-20 15:44:36.000000 jumanji-0.3.1/requirements/requirements-train.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-20 15:44:36.000000 jumanji-0.3.1/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-20 15:44:49.413550 jumanji-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-20 15:44:36.000000 jumanji-0.3.1/setup.py
```

### Comparing `jumanji-0.3.0/LICENSE` & `jumanji-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/PKG-INFO` & `jumanji-0.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: jumanji
-Version: 0.3.0
-Summary: A diverse suite of scalable reinforcement learning environments in JAX
-Home-page: https://github.com/instadeepai/jumanji/
-Author: InstaDeep
-Author-email: c.bonnet@instadeep.com
-License: Apache 2.0
-Keywords: reinforcement-learning python jax
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: train
-License-File: LICENSE
-
 <p align="center">
     <a href="docs/img/jumanji_logo.png">
         <img src="docs/img/jumanji_logo.png" alt="Jumanji logo" width="50%"/>
     </a>
 </p>
 
 [![Python Versions](https://img.shields.io/pypi/pyversions/jumanji.svg?style=flat-square)](https://www.python.org/doc/versions/)
@@ -243,23 +218,29 @@
 details on how to submit pull requests, our Contributor License Agreement, and community guidelines.
 
 ## Citing Jumanji ✏️
 
 If you use Jumanji in your work, please cite the library using:
 
 ```
-@software{jumanji2023github,
-  author = {Clément Bonnet and Daniel Luo and Donal Byrne and Sasha Abramowitz
-        and Vincent Coyette and Paul Duckworth and Daniel Furelos-Blanco and
-        Nathan Grinsztajn and Tristan Kalloniatis and Victor Le and Omayma Mahjoub
-        and Laurence Midgley and Shikha Surana and Cemlyn Waters and Alexandre Laterre},
-  title = {Jumanji: a Suite of Diverse and Challenging Reinforcement Learning Environments in JAX},
-  url = {https://github.com/instadeepai/jumanji},
-  version = {0.2.2},
-  year = {2023},
+@misc{bonnet2023jumanji,
+    title={Jumanji: a Diverse Suite of Scalable Reinforcement Learning Environments in JAX},
+    author={
+        Clément Bonnet and Daniel Luo and Donal Byrne and Shikha Surana and Vincent Coyette and
+        Paul Duckworth and Laurence I. Midgley and Tristan Kalloniatis and Sasha Abramowitz and
+        Cemlyn N. Waters and Andries P. Smit and Nathan Grinsztajn and Ulrich A. Mbou Sob and
+        Omayma Mahjoub and Elshadai Tegegn and Mohamed A. Mimouni and Raphael Boige and
+        Ruan de Kock and Daniel Furelos-Blanco and Victor Le and Arnu Pretorius and
+        Alexandre Laterre
+    },
+    year={2023},
+    eprint={2306.09884},
+    url={https://arxiv.org/abs/2306.09884},
+    archivePrefix={arXiv},
+    primaryClass={cs.LG}
 }
 ```
 
 ## See Also 🔎
 
 Other works have embraced the approach of writing RL environments in JAX.
 In particular, we suggest users check out the following sister repositories:
```

#### html2text {}

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1 Name: jumanji Version: 0.3.0 Summary: A diverse suite of
-scalable reinforcement learning environments in JAX Home-page: https://
-github.com/instadeepai/jumanji/ Author: InstaDeep Author-email:
-c.bonnet@instadeep.com License: Apache 2.0 Keywords: reinforcement-learning
-python jax Classifier: Development Status :: 4 - Beta Classifier: Environment
-:: Console Classifier: Intended Audience :: Science/Research Classifier:
-Intended Audience :: Developers Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Topic :: Scientific/Engineering ::
-Artificial Intelligence Classifier: Topic :: Software Development :: Libraries
-:: Python Modules Classifier: License :: OSI Approved :: Apache Software
-License Requires-Python: >=3.8 Description-Content-Type: text/markdown
-Provides-Extra: dev Provides-Extra: train License-File: LICENSE
                                 [Jumanji_logo]
 [![Python Versions](https://img.shields.io/pypi/pyversions/
 jumanji.svg?style=flat-square)](https://www.python.org/doc/versions/) [![PyPI
 Version](https://badge.fury.io/py/jumanji.svg)](https://badge.fury.io/py/
 jumanji) [![Tests](https://github.com/instadeepai/jumanji/actions/workflows/
 tests_linters.yml/badge.svg)](https://github.com/instadeepai/jumanji/actions/
 workflows/tests_linters.yml) [![Code Style](https://img.shields.io/badge/
@@ -180,30 +167,32 @@
 [training guide](https://instadeepai.github.io/jumanji/guides/training/). ##
 Contributing ð¤ Contributions are welcome! See our issue tracker for [good
 first issues](https://github.com/instadeepai/jumanji/labels/
 good%20first%20issue). Please read our [contributing guidelines](https://
 github.com/instadeepai/jumanji/blob/main/CONTRIBUTING.md) for details on how to
 submit pull requests, our Contributor License Agreement, and community
 guidelines. ## Citing Jumanji âï¸ If you use Jumanji in your work, please
-cite the library using: ``` @software{jumanji2023github, author = {ClÃ©ment
-Bonnet and Daniel Luo and Donal Byrne and Sasha Abramowitz and Vincent Coyette
-and Paul Duckworth and Daniel Furelos-Blanco and Nathan Grinsztajn and Tristan
-Kalloniatis and Victor Le and Omayma Mahjoub and Laurence Midgley and Shikha
-Surana and Cemlyn Waters and Alexandre Laterre}, title = {Jumanji: a Suite of
-Diverse and Challenging Reinforcement Learning Environments in JAX}, url =
-{https://github.com/instadeepai/jumanji}, version = {0.2.2}, year = {2023}, }
-``` ## See Also ð Other works have embraced the approach of writing RL
-environments in JAX. In particular, we suggest users check out the following
-sister repositories: - ð¤ [Qdax](https://github.com/adaptive-intelligent-
-robotics/QDax) is a library to accelerate Quality-Diversity and neuro-evolution
-algorithms through hardware accelerators and parallelization. - ð³ [Evojax]
-(https://github.com/google/evojax) provides tools to enable neuroevolution
-algorithms to work with neural networks running across multiple TPU/GPUs. -
-ð¦¾ [Brax](https://github.com/google/brax) is a differentiable physics engine
-that simulates environments made up of rigid bodies, joints, and actuators. -
-ðï¸â [Gymnax](https://github.com/RobertTLange/gymnax) implements classic
-environments including classic control, bsuite, MinAtar and a collection of
-meta RL tasks. - ð² [Pgx](https://github.com/sotetsuk/pgx) provides classic
-board game environments like Backgammon, Shogi, and Go. ## Acknowledgements
-ð The development of this library was supported with Cloud TPUs from
-Google's [TPU Research Cloud](https://sites.research.google/trc/about/) (TRC)
-ð¤.
+cite the library using: ``` @misc{bonnet2023jumanji, title={Jumanji: a Diverse
+Suite of Scalable Reinforcement Learning Environments in JAX}, author=
+{ ClÃ©ment Bonnet and Daniel Luo and Donal Byrne and Shikha Surana and Vincent
+Coyette and Paul Duckworth and Laurence I. Midgley and Tristan Kalloniatis and
+Sasha Abramowitz and Cemlyn N. Waters and Andries P. Smit and Nathan Grinsztajn
+and Ulrich A. Mbou Sob and Omayma Mahjoub and Elshadai Tegegn and Mohamed A.
+Mimouni and Raphael Boige and Ruan de Kock and Daniel Furelos-Blanco and Victor
+Le and Arnu Pretorius and Alexandre Laterre }, year={2023}, eprint=
+{2306.09884}, url={https://arxiv.org/abs/2306.09884}, archivePrefix={arXiv},
+primaryClass={cs.LG} } ``` ## See Also ð Other works have embraced the
+approach of writing RL environments in JAX. In particular, we suggest users
+check out the following sister repositories: - ð¤ [Qdax](https://github.com/
+adaptive-intelligent-robotics/QDax) is a library to accelerate Quality-
+Diversity and neuro-evolution algorithms through hardware accelerators and
+parallelization. - ð³ [Evojax](https://github.com/google/evojax) provides
+tools to enable neuroevolution algorithms to work with neural networks running
+across multiple TPU/GPUs. - ð¦¾ [Brax](https://github.com/google/brax) is a
+differentiable physics engine that simulates environments made up of rigid
+bodies, joints, and actuators. - ðï¸â [Gymnax](https://github.com/
+RobertTLange/gymnax) implements classic environments including classic control,
+bsuite, MinAtar and a collection of meta RL tasks. - ð² [Pgx](https://
+github.com/sotetsuk/pgx) provides classic board game environments like
+Backgammon, Shogi, and Go. ## Acknowledgements ð The development of this
+library was supported with Cloud TPUs from Google's [TPU Research Cloud](https:
+//sites.research.google/trc/about/) (TRC) ð¤.
```

### Comparing `jumanji-0.3.0/README.md` & `jumanji-0.3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: jumanji
+Version: 0.3.1
+Summary: A diverse suite of scalable reinforcement learning environments in JAX
+Home-page: https://github.com/instadeepai/jumanji/
+Author: InstaDeep
+Author-email: c.bonnet@instadeep.com
+License: Apache 2.0
+Keywords: reinforcement-learning python jax
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: train
+License-File: LICENSE
+
 <p align="center">
     <a href="docs/img/jumanji_logo.png">
         <img src="docs/img/jumanji_logo.png" alt="Jumanji logo" width="50%"/>
     </a>
 </p>
 
 [![Python Versions](https://img.shields.io/pypi/pyversions/jumanji.svg?style=flat-square)](https://www.python.org/doc/versions/)
@@ -218,23 +243,29 @@
 details on how to submit pull requests, our Contributor License Agreement, and community guidelines.
 
 ## Citing Jumanji ✏️
 
 If you use Jumanji in your work, please cite the library using:
 
 ```
-@software{jumanji2023github,
-  author = {Clément Bonnet and Daniel Luo and Donal Byrne and Sasha Abramowitz
-        and Vincent Coyette and Paul Duckworth and Daniel Furelos-Blanco and
-        Nathan Grinsztajn and Tristan Kalloniatis and Victor Le and Omayma Mahjoub
-        and Laurence Midgley and Shikha Surana and Cemlyn Waters and Alexandre Laterre},
-  title = {Jumanji: a Suite of Diverse and Challenging Reinforcement Learning Environments in JAX},
-  url = {https://github.com/instadeepai/jumanji},
-  version = {0.2.2},
-  year = {2023},
+@misc{bonnet2023jumanji,
+    title={Jumanji: a Diverse Suite of Scalable Reinforcement Learning Environments in JAX},
+    author={
+        Clément Bonnet and Daniel Luo and Donal Byrne and Shikha Surana and Vincent Coyette and
+        Paul Duckworth and Laurence I. Midgley and Tristan Kalloniatis and Sasha Abramowitz and
+        Cemlyn N. Waters and Andries P. Smit and Nathan Grinsztajn and Ulrich A. Mbou Sob and
+        Omayma Mahjoub and Elshadai Tegegn and Mohamed A. Mimouni and Raphael Boige and
+        Ruan de Kock and Daniel Furelos-Blanco and Victor Le and Arnu Pretorius and
+        Alexandre Laterre
+    },
+    year={2023},
+    eprint={2306.09884},
+    url={https://arxiv.org/abs/2306.09884},
+    archivePrefix={arXiv},
+    primaryClass={cs.LG}
 }
 ```
 
 ## See Also 🔎
 
 Other works have embraced the approach of writing RL environments in JAX.
 In particular, we suggest users check out the following sister repositories:
```

#### html2text {}

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1 Name: jumanji Version: 0.3.1 Summary: A diverse suite of
+scalable reinforcement learning environments in JAX Home-page: https://
+github.com/instadeepai/jumanji/ Author: InstaDeep Author-email:
+c.bonnet@instadeep.com License: Apache 2.0 Keywords: reinforcement-learning
+python jax Classifier: Development Status :: 4 - Beta Classifier: Environment
+:: Console Classifier: Intended Audience :: Science/Research Classifier:
+Intended Audience :: Developers Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Classifier: Topic :: Software Development :: Libraries
+:: Python Modules Classifier: License :: OSI Approved :: Apache Software
+License Requires-Python: >=3.8 Description-Content-Type: text/markdown
+Provides-Extra: dev Provides-Extra: train License-File: LICENSE
                                 [Jumanji_logo]
 [![Python Versions](https://img.shields.io/pypi/pyversions/
 jumanji.svg?style=flat-square)](https://www.python.org/doc/versions/) [![PyPI
 Version](https://badge.fury.io/py/jumanji.svg)](https://badge.fury.io/py/
 jumanji) [![Tests](https://github.com/instadeepai/jumanji/actions/workflows/
 tests_linters.yml/badge.svg)](https://github.com/instadeepai/jumanji/actions/
 workflows/tests_linters.yml) [![Code Style](https://img.shields.io/badge/
@@ -167,30 +180,32 @@
 [training guide](https://instadeepai.github.io/jumanji/guides/training/). ##
 Contributing ð¤ Contributions are welcome! See our issue tracker for [good
 first issues](https://github.com/instadeepai/jumanji/labels/
 good%20first%20issue). Please read our [contributing guidelines](https://
 github.com/instadeepai/jumanji/blob/main/CONTRIBUTING.md) for details on how to
 submit pull requests, our Contributor License Agreement, and community
 guidelines. ## Citing Jumanji âï¸ If you use Jumanji in your work, please
-cite the library using: ``` @software{jumanji2023github, author = {ClÃ©ment
-Bonnet and Daniel Luo and Donal Byrne and Sasha Abramowitz and Vincent Coyette
-and Paul Duckworth and Daniel Furelos-Blanco and Nathan Grinsztajn and Tristan
-Kalloniatis and Victor Le and Omayma Mahjoub and Laurence Midgley and Shikha
-Surana and Cemlyn Waters and Alexandre Laterre}, title = {Jumanji: a Suite of
-Diverse and Challenging Reinforcement Learning Environments in JAX}, url =
-{https://github.com/instadeepai/jumanji}, version = {0.2.2}, year = {2023}, }
-``` ## See Also ð Other works have embraced the approach of writing RL
-environments in JAX. In particular, we suggest users check out the following
-sister repositories: - ð¤ [Qdax](https://github.com/adaptive-intelligent-
-robotics/QDax) is a library to accelerate Quality-Diversity and neuro-evolution
-algorithms through hardware accelerators and parallelization. - ð³ [Evojax]
-(https://github.com/google/evojax) provides tools to enable neuroevolution
-algorithms to work with neural networks running across multiple TPU/GPUs. -
-ð¦¾ [Brax](https://github.com/google/brax) is a differentiable physics engine
-that simulates environments made up of rigid bodies, joints, and actuators. -
-ðï¸â [Gymnax](https://github.com/RobertTLange/gymnax) implements classic
-environments including classic control, bsuite, MinAtar and a collection of
-meta RL tasks. - ð² [Pgx](https://github.com/sotetsuk/pgx) provides classic
-board game environments like Backgammon, Shogi, and Go. ## Acknowledgements
-ð The development of this library was supported with Cloud TPUs from
-Google's [TPU Research Cloud](https://sites.research.google/trc/about/) (TRC)
-ð¤.
+cite the library using: ``` @misc{bonnet2023jumanji, title={Jumanji: a Diverse
+Suite of Scalable Reinforcement Learning Environments in JAX}, author=
+{ ClÃ©ment Bonnet and Daniel Luo and Donal Byrne and Shikha Surana and Vincent
+Coyette and Paul Duckworth and Laurence I. Midgley and Tristan Kalloniatis and
+Sasha Abramowitz and Cemlyn N. Waters and Andries P. Smit and Nathan Grinsztajn
+and Ulrich A. Mbou Sob and Omayma Mahjoub and Elshadai Tegegn and Mohamed A.
+Mimouni and Raphael Boige and Ruan de Kock and Daniel Furelos-Blanco and Victor
+Le and Arnu Pretorius and Alexandre Laterre }, year={2023}, eprint=
+{2306.09884}, url={https://arxiv.org/abs/2306.09884}, archivePrefix={arXiv},
+primaryClass={cs.LG} } ``` ## See Also ð Other works have embraced the
+approach of writing RL environments in JAX. In particular, we suggest users
+check out the following sister repositories: - ð¤ [Qdax](https://github.com/
+adaptive-intelligent-robotics/QDax) is a library to accelerate Quality-
+Diversity and neuro-evolution algorithms through hardware accelerators and
+parallelization. - ð³ [Evojax](https://github.com/google/evojax) provides
+tools to enable neuroevolution algorithms to work with neural networks running
+across multiple TPU/GPUs. - ð¦¾ [Brax](https://github.com/google/brax) is a
+differentiable physics engine that simulates environments made up of rigid
+bodies, joints, and actuators. - ðï¸â [Gymnax](https://github.com/
+RobertTLange/gymnax) implements classic environments including classic control,
+bsuite, MinAtar and a collection of meta RL tasks. - ð² [Pgx](https://
+github.com/sotetsuk/pgx) provides classic board game environments like
+Backgammon, Shogi, and Go. ## Acknowledgements ð The development of this
+library was supported with Cloud TPUs from Google's [TPU Research Cloud](https:
+//sites.research.google/trc/about/) (TRC) ð¤.
```

### Comparing `jumanji-0.3.0/jumanji/__init__.py` & `jumanji-0.3.1/jumanji/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/env.py` & `jumanji-0.3.1/jumanji/env.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/__init__.py` & `jumanji-0.3.1/jumanji/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/commons/__init__.py` & `jumanji-0.3.1/jumanji/environments/commons/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/commons/maze_utils/__init__.py` & `jumanji-0.3.1/jumanji/environments/commons/maze_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/commons/maze_utils/maze_generation.py` & `jumanji-0.3.1/jumanji/environments/commons/maze_utils/maze_generation.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/commons/maze_utils/maze_rendering.py` & `jumanji-0.3.1/jumanji/environments/commons/maze_utils/maze_rendering.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/commons/maze_utils/stack.py` & `jumanji-0.3.1/jumanji/environments/commons/maze_utils/stack.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/__init__.py` & `jumanji-0.3.1/jumanji/environments/logic/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/game_2048/__init__.py` & `jumanji-0.3.1/jumanji/environments/logic/game_2048/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/game_2048/env.py` & `jumanji-0.3.1/jumanji/environments/logic/game_2048/env.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,20 +19,15 @@
 import jax.numpy as jnp
 import matplotlib.animation as animation
 from numpy.typing import NDArray
 
 from jumanji import specs
 from jumanji.env import Environment
 from jumanji.environments.logic.game_2048.types import Board, Observation, State
-from jumanji.environments.logic.game_2048.utils import (
-    move_down,
-    move_left,
-    move_right,
-    move_up,
-)
+from jumanji.environments.logic.game_2048.utils import can_move, move
 from jumanji.environments.logic.game_2048.viewer import Game2048Viewer
 from jumanji.types import TimeStep, restart, termination, transition
 from jumanji.viewer import Viewer
 
 
 class Game2048(Environment[State]):
     """Environment for the game 2048. The game consists of a board of size board_size x board_size
@@ -177,19 +172,15 @@
             action: the action taken by the agent.
 
         Returns:
             state: the new state of the environment.
             timestep: the next timestep.
         """
         # Take the action in the environment: Up, Right, Down, Left.
-        updated_board, additional_reward = jax.lax.switch(
-            action,
-            [move_up, move_right, move_down, move_left],
-            state.board,
-        )
+        updated_board, reward = move(state.board, action)
 
         # Generate new key.
         random_cell_key, new_state_key = jax.random.split(state.key)
 
         # Update the state of the board by adding a new random cell.
         updated_board = jax.lax.cond(
             state.action_mask[action],
@@ -205,15 +196,15 @@
 
         # Build the state.
         state = State(
             board=updated_board,
             action_mask=action_mask,
             step_count=state.step_count + 1,
             key=new_state_key,
-            score=state.score + additional_reward.astype(float),
+            score=state.score + reward,
         )
 
         # Generate the observation from the environment state.
         observation = Observation(
             board=updated_board,
             action_mask=action_mask,
         )
@@ -223,20 +214,20 @@
 
         # Return either a MID or a LAST timestep depending on done.
         highest_tile = 2 ** jnp.max(updated_board)
         extras = {"highest_tile": highest_tile}
         timestep = jax.lax.cond(
             done,
             lambda: termination(
-                reward=additional_reward,
+                reward=reward,
                 observation=observation,
                 extras=extras,
             ),
             lambda: transition(
-                reward=additional_reward,
+                reward=reward,
                 observation=observation,
                 extras=extras,
             ),
         )
 
         return state, timestep
 
@@ -299,23 +290,15 @@
 
         Args:
             board: current board of the environment.
 
         Returns:
             action_mask: action mask for the current state of the environment.
         """
-        action_mask = jnp.array(
-            [
-                jnp.any(move_up(board, final_shift=False)[0] != board),
-                jnp.any(move_right(board, final_shift=False)[0] != board),
-                jnp.any(move_down(board, final_shift=False)[0] != board),
-                jnp.any(move_left(board, final_shift=False)[0] != board),
-            ],
-        )
-        return action_mask
+        return jax.vmap(can_move, (None, 0))(board, jnp.arange(4))
 
     def render(self, state: State) -> Optional[NDArray]:
         """Renders the current state of the game board.
 
         Args:
             state: is the current game state to be rendered.
         """
```

### Comparing `jumanji-0.3.0/jumanji/environments/logic/game_2048/types.py` & `jumanji-0.3.1/jumanji/environments/logic/game_2048/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/game_2048/viewer.py` & `jumanji-0.3.1/jumanji/environments/logic/game_2048/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/graph_coloring/__init__.py` & `jumanji-0.3.1/jumanji/environments/logic/graph_coloring/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/graph_coloring/env.py` & `jumanji-0.3.1/jumanji/environments/logic/graph_coloring/env.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/graph_coloring/generator.py` & `jumanji-0.3.1/jumanji/environments/logic/graph_coloring/generator.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/graph_coloring/types.py` & `jumanji-0.3.1/jumanji/environments/logic/graph_coloring/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/graph_coloring/viewer.py` & `jumanji-0.3.1/jumanji/environments/logic/graph_coloring/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/minesweeper/__init__.py` & `jumanji-0.3.1/jumanji/environments/logic/minesweeper/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/minesweeper/constants.py` & `jumanji-0.3.1/jumanji/environments/logic/minesweeper/constants.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/minesweeper/done.py` & `jumanji-0.3.1/jumanji/environments/logic/minesweeper/done.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/minesweeper/env.py` & `jumanji-0.3.1/jumanji/environments/logic/minesweeper/env.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/minesweeper/generator.py` & `jumanji-0.3.1/jumanji/environments/logic/minesweeper/generator.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/minesweeper/reward.py` & `jumanji-0.3.1/jumanji/environments/logic/minesweeper/reward.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/minesweeper/types.py` & `jumanji-0.3.1/jumanji/environments/logic/minesweeper/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/minesweeper/utils.py` & `jumanji-0.3.1/jumanji/environments/logic/minesweeper/utils.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/minesweeper/viewer.py` & `jumanji-0.3.1/jumanji/environments/logic/minesweeper/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/__init__.py` & `jumanji-0.3.1/jumanji/environments/logic/rubiks_cube/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/constants.py` & `jumanji-0.3.1/jumanji/environments/logic/rubiks_cube/constants.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/env.py` & `jumanji-0.3.1/jumanji/environments/logic/rubiks_cube/env.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/generator.py` & `jumanji-0.3.1/jumanji/environments/logic/rubiks_cube/generator.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/reward.py` & `jumanji-0.3.1/jumanji/environments/logic/rubiks_cube/reward.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/types.py` & `jumanji-0.3.1/jumanji/environments/logic/rubiks_cube/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/utils.py` & `jumanji-0.3.1/jumanji/environments/logic/rubiks_cube/utils.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/viewer.py` & `jumanji-0.3.1/jumanji/environments/logic/rubiks_cube/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/sudoku/__init__.py` & `jumanji-0.3.1/jumanji/environments/logic/sudoku/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/sudoku/constants.py` & `jumanji-0.3.1/jumanji/environments/logic/sudoku/constants.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/sudoku/data/10000_mixed_puzzles.npy` & `jumanji-0.3.1/jumanji/environments/logic/sudoku/data/10000_mixed_puzzles.npy`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/sudoku/data/1000_very_easy_puzzles.npy` & `jumanji-0.3.1/jumanji/environments/logic/sudoku/data/1000_very_easy_puzzles.npy`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/sudoku/data/__init__.py` & `jumanji-0.3.1/jumanji/environments/logic/sudoku/data/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/sudoku/env.py` & `jumanji-0.3.1/jumanji/environments/logic/sudoku/env.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/sudoku/generator.py` & `jumanji-0.3.1/jumanji/environments/logic/sudoku/generator.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/sudoku/reward.py` & `jumanji-0.3.1/jumanji/environments/logic/sudoku/reward.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/sudoku/types.py` & `jumanji-0.3.1/jumanji/environments/logic/sudoku/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/sudoku/utils.py` & `jumanji-0.3.1/jumanji/environments/logic/sudoku/utils.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/logic/sudoku/viewer.py` & `jumanji-0.3.1/jumanji/environments/logic/sudoku/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/packing/__init__.py` & `jumanji-0.3.1/jumanji/environments/packing/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/packing/bin_pack/__init__.py` & `jumanji-0.3.1/jumanji/environments/packing/bin_pack/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/packing/bin_pack/env.py` & `jumanji-0.3.1/jumanji/environments/packing/bin_pack/env.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/packing/bin_pack/generator.py` & `jumanji-0.3.1/jumanji/environments/packing/bin_pack/generator.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/packing/bin_pack/reward.py` & `jumanji-0.3.1/jumanji/environments/packing/bin_pack/reward.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/packing/bin_pack/space.py` & `jumanji-0.3.1/jumanji/environments/packing/bin_pack/space.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/packing/bin_pack/types.py` & `jumanji-0.3.1/jumanji/environments/packing/bin_pack/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/packing/bin_pack/viewer.py` & `jumanji-0.3.1/jumanji/environments/packing/bin_pack/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/packing/job_shop/__init__.py` & `jumanji-0.3.1/jumanji/environments/packing/job_shop/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/packing/job_shop/env.py` & `jumanji-0.3.1/jumanji/environments/packing/job_shop/env.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/packing/job_shop/generator.py` & `jumanji-0.3.1/jumanji/environments/packing/job_shop/generator.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/packing/job_shop/types.py` & `jumanji-0.3.1/jumanji/environments/packing/job_shop/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/packing/job_shop/viewer.py` & `jumanji-0.3.1/jumanji/environments/packing/job_shop/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/packing/knapsack/__init__.py` & `jumanji-0.3.1/jumanji/environments/packing/knapsack/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/packing/knapsack/env.py` & `jumanji-0.3.1/jumanji/environments/packing/knapsack/env.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/packing/knapsack/generator.py` & `jumanji-0.3.1/jumanji/environments/packing/knapsack/generator.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/packing/knapsack/reward.py` & `jumanji-0.3.1/jumanji/environments/packing/knapsack/reward.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/packing/knapsack/types.py` & `jumanji-0.3.1/jumanji/environments/packing/knapsack/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/packing/knapsack/viewer.py` & `jumanji-0.3.1/jumanji/environments/packing/knapsack/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/packing/tetris/__init__.py` & `jumanji-0.3.1/jumanji/environments/packing/tetris/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/packing/tetris/constants.py` & `jumanji-0.3.1/jumanji/environments/packing/tetris/constants.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/packing/tetris/env.py` & `jumanji-0.3.1/jumanji/environments/packing/tetris/env.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/packing/tetris/types.py` & `jumanji-0.3.1/jumanji/environments/packing/tetris/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/packing/tetris/utils.py` & `jumanji-0.3.1/jumanji/environments/packing/tetris/utils.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/packing/tetris/viewer.py` & `jumanji-0.3.1/jumanji/environments/packing/tetris/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/__init__.py` & `jumanji-0.3.1/jumanji/environments/routing/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/cleaner/__init__.py` & `jumanji-0.3.1/jumanji/environments/routing/cleaner/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/cleaner/constants.py` & `jumanji-0.3.1/jumanji/environments/routing/cleaner/constants.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/cleaner/env.py` & `jumanji-0.3.1/jumanji/environments/routing/cleaner/env.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/cleaner/generator.py` & `jumanji-0.3.1/jumanji/environments/routing/cleaner/generator.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/cleaner/types.py` & `jumanji-0.3.1/jumanji/environments/routing/cleaner/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/cleaner/viewer.py` & `jumanji-0.3.1/jumanji/environments/routing/cleaner/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/connector/__init__.py` & `jumanji-0.3.1/jumanji/environments/routing/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/connector/constants.py` & `jumanji-0.3.1/jumanji/environments/routing/connector/constants.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/connector/env.py` & `jumanji-0.3.1/jumanji/environments/routing/connector/env.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/connector/generator.py` & `jumanji-0.3.1/jumanji/environments/routing/connector/generator.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/connector/reward.py` & `jumanji-0.3.1/jumanji/environments/routing/connector/reward.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/connector/types.py` & `jumanji-0.3.1/jumanji/environments/routing/connector/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/connector/utils.py` & `jumanji-0.3.1/jumanji/environments/routing/connector/utils.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/connector/viewer.py` & `jumanji-0.3.1/jumanji/environments/routing/connector/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/cvrp/__init__.py` & `jumanji-0.3.1/jumanji/environments/routing/cvrp/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/cvrp/constants.py` & `jumanji-0.3.1/jumanji/environments/routing/cvrp/constants.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/cvrp/env.py` & `jumanji-0.3.1/jumanji/environments/routing/cvrp/env.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/cvrp/generator.py` & `jumanji-0.3.1/jumanji/environments/routing/cvrp/generator.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/cvrp/reward.py` & `jumanji-0.3.1/jumanji/environments/routing/cvrp/reward.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/cvrp/types.py` & `jumanji-0.3.1/jumanji/environments/routing/cvrp/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/cvrp/viewer.py` & `jumanji-0.3.1/jumanji/environments/routing/cvrp/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/maze/__init__.py` & `jumanji-0.3.1/jumanji/environments/routing/maze/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/maze/constants.py` & `jumanji-0.3.1/jumanji/environments/routing/maze/constants.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/maze/env.py` & `jumanji-0.3.1/jumanji/environments/routing/maze/env.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/maze/generator.py` & `jumanji-0.3.1/jumanji/environments/routing/maze/generator.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/maze/types.py` & `jumanji-0.3.1/jumanji/environments/routing/maze/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/maze/viewer.py` & `jumanji-0.3.1/jumanji/environments/routing/maze/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/mmst/__init__.py` & `jumanji-0.3.1/jumanji/environments/routing/mmst/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/mmst/constants.py` & `jumanji-0.3.1/jumanji/environments/routing/mmst/constants.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/mmst/env.py` & `jumanji-0.3.1/jumanji/environments/routing/mmst/env.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/mmst/generator.py` & `jumanji-0.3.1/jumanji/environments/routing/mmst/generator.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/mmst/reward.py` & `jumanji-0.3.1/jumanji/environments/routing/mmst/reward.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/mmst/types.py` & `jumanji-0.3.1/jumanji/environments/routing/mmst/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/mmst/utils.py` & `jumanji-0.3.1/jumanji/environments/routing/mmst/utils.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/mmst/viewer.py` & `jumanji-0.3.1/jumanji/environments/routing/mmst/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/multi_cvrp/__init__.py` & `jumanji-0.3.1/jumanji/environments/routing/multi_cvrp/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/multi_cvrp/constants.py` & `jumanji-0.3.1/jumanji/environments/routing/multi_cvrp/constants.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/multi_cvrp/env.py` & `jumanji-0.3.1/jumanji/environments/routing/multi_cvrp/env.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/multi_cvrp/generator.py` & `jumanji-0.3.1/jumanji/environments/routing/multi_cvrp/generator.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/multi_cvrp/reward.py` & `jumanji-0.3.1/jumanji/environments/routing/multi_cvrp/reward.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/multi_cvrp/test_data.py` & `jumanji-0.3.1/jumanji/environments/routing/multi_cvrp/test_data.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/multi_cvrp/types.py` & `jumanji-0.3.1/jumanji/environments/routing/multi_cvrp/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/multi_cvrp/utils.py` & `jumanji-0.3.1/jumanji/environments/routing/multi_cvrp/utils.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/multi_cvrp/viewer.py` & `jumanji-0.3.1/jumanji/environments/routing/multi_cvrp/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/__init__.py` & `jumanji-0.3.1/jumanji/environments/routing/robot_warehouse/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/constants.py` & `jumanji-0.3.1/jumanji/environments/routing/robot_warehouse/constants.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/env.py` & `jumanji-0.3.1/jumanji/environments/routing/robot_warehouse/env.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/generator.py` & `jumanji-0.3.1/jumanji/environments/routing/robot_warehouse/generator.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/types.py` & `jumanji-0.3.1/jumanji/environments/routing/robot_warehouse/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/utils.py` & `jumanji-0.3.1/jumanji/environments/routing/robot_warehouse/utils.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/utils_agent.py` & `jumanji-0.3.1/jumanji/environments/routing/robot_warehouse/utils_agent.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/utils_shelf.py` & `jumanji-0.3.1/jumanji/environments/routing/robot_warehouse/utils_shelf.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/utils_spawn.py` & `jumanji-0.3.1/jumanji/environments/routing/robot_warehouse/utils_spawn.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/viewer.py` & `jumanji-0.3.1/jumanji/environments/routing/robot_warehouse/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/snake/__init__.py` & `jumanji-0.3.1/jumanji/environments/routing/snake/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/snake/env.py` & `jumanji-0.3.1/jumanji/environments/routing/snake/env.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/snake/types.py` & `jumanji-0.3.1/jumanji/environments/routing/snake/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/snake/viewer.py` & `jumanji-0.3.1/jumanji/environments/routing/snake/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/tsp/__init__.py` & `jumanji-0.3.1/jumanji/environments/routing/tsp/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/tsp/env.py` & `jumanji-0.3.1/jumanji/environments/routing/tsp/env.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/tsp/generator.py` & `jumanji-0.3.1/jumanji/environments/routing/tsp/generator.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/tsp/reward.py` & `jumanji-0.3.1/jumanji/environments/routing/tsp/reward.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/tsp/types.py` & `jumanji-0.3.1/jumanji/environments/routing/tsp/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/environments/routing/tsp/viewer.py` & `jumanji-0.3.1/jumanji/environments/routing/tsp/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/registration.py` & `jumanji-0.3.1/jumanji/registration.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/specs.py` & `jumanji-0.3.1/jumanji/specs.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/testing/__init__.py` & `jumanji-0.3.1/jumanji/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/testing/env_not_smoke.py` & `jumanji-0.3.1/jumanji/testing/env_not_smoke.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/testing/fakes.py` & `jumanji-0.3.1/jumanji/testing/fakes.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/testing/pytrees.py` & `jumanji-0.3.1/jumanji/testing/pytrees.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Any, Type, TypeVar
 
 import chex
 import jax
+import jax.numpy as jnp
 import jax.tree_util
 import numpy as np
 import tree as tree_lib
 
 # In these testing utils we often operate on trees composed of leaves that we can call
 # `np.asarray(leaf)` on. This allows for backend agnostic functionality (e.g. will work for tf
 # tensors or jax arrays, as well as floats, strings, None etc). We define the below type to
@@ -85,16 +86,16 @@
         input_tree, *leaf_type
     ), "The tree has at least one leaf that is not of type {}.".format(
         " or ".join([str(type_) for type_ in leaf_type])
     )
 
 
 def assert_is_jax_array_tree(input_tree: chex.ArrayTree) -> None:
-    """Asserts that the `input_tree` has leaves that are exclusively of type `chex.Array`."""
-    assert_tree_with_leaves_of_type(input_tree, chex.Array, type(None))
+    """Asserts that the `input_tree` has leaves that are exclusively of type `jnp.ndarray`."""
+    assert_tree_with_leaves_of_type(input_tree, jnp.ndarray, type(None))
 
 
 def has_at_least_rank(input_tree: chex.ArrayTree, rank: int) -> bool:
     """Indicate if all leaves have a rank greater or equal to `rank`."""
     has_rank_greater, _ = jax.tree_util.tree_flatten(
         jax.tree_util.tree_map(lambda x: x.ndim >= rank, input_tree)
     )
```

### Comparing `jumanji-0.3.0/jumanji/training/__init__.py` & `jumanji-0.3.1/jumanji/training/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/agents/__init__.py` & `jumanji-0.3.1/jumanji/training/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/agents/a2c/__init__.py` & `jumanji-0.3.1/jumanji/training/agents/a2c/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/agents/a2c/a2c_agent.py` & `jumanji-0.3.1/jumanji/training/agents/a2c/a2c_agent.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/agents/base.py` & `jumanji-0.3.1/jumanji/training/agents/base.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/agents/random/__init__.py` & `jumanji-0.3.1/jumanji/training/agents/random/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/agents/random/random_agent.py` & `jumanji-0.3.1/jumanji/training/agents/random/random_agent.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/evaluator.py` & `jumanji-0.3.1/jumanji/training/evaluator.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/loggers.py` & `jumanji-0.3.1/jumanji/training/loggers.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/__init__.py` & `jumanji-0.3.1/jumanji/training/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/actor_critic.py` & `jumanji-0.3.1/jumanji/training/networks/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/base.py` & `jumanji-0.3.1/jumanji/training/networks/base.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/bin_pack/__init__.py` & `jumanji-0.3.1/jumanji/training/networks/bin_pack/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/bin_pack/actor_critic.py` & `jumanji-0.3.1/jumanji/training/networks/bin_pack/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/bin_pack/random.py` & `jumanji-0.3.1/jumanji/training/networks/bin_pack/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/cleaner/__init__.py` & `jumanji-0.3.1/jumanji/training/networks/cleaner/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/cleaner/actor_critic.py` & `jumanji-0.3.1/jumanji/training/networks/cleaner/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/cleaner/random.py` & `jumanji-0.3.1/jumanji/training/networks/cleaner/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/connector/__init__.py` & `jumanji-0.3.1/jumanji/training/networks/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/connector/actor_critic.py` & `jumanji-0.3.1/jumanji/training/networks/connector/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/connector/random.py` & `jumanji-0.3.1/jumanji/training/networks/connector/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/cvrp/__init__.py` & `jumanji-0.3.1/jumanji/training/networks/cvrp/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/cvrp/actor_critic.py` & `jumanji-0.3.1/jumanji/training/networks/cvrp/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/cvrp/random.py` & `jumanji-0.3.1/jumanji/training/networks/cvrp/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/distribution.py` & `jumanji-0.3.1/jumanji/training/networks/distribution.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/game_2048/__init__.py` & `jumanji-0.3.1/jumanji/training/networks/game_2048/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/game_2048/actor_critic.py` & `jumanji-0.3.1/jumanji/training/networks/game_2048/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/game_2048/random.py` & `jumanji-0.3.1/jumanji/training/networks/game_2048/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/graph_coloring/__init__.py` & `jumanji-0.3.1/jumanji/training/networks/graph_coloring/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/graph_coloring/actor_critic.py` & `jumanji-0.3.1/jumanji/training/networks/graph_coloring/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/graph_coloring/random.py` & `jumanji-0.3.1/jumanji/training/networks/graph_coloring/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/job_shop/__init__.py` & `jumanji-0.3.1/jumanji/training/networks/job_shop/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/job_shop/actor_critic.py` & `jumanji-0.3.1/jumanji/training/networks/job_shop/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/job_shop/random.py` & `jumanji-0.3.1/jumanji/training/networks/job_shop/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/knapsack/__init__.py` & `jumanji-0.3.1/jumanji/training/networks/knapsack/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/knapsack/actor_critic.py` & `jumanji-0.3.1/jumanji/training/networks/knapsack/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/knapsack/random.py` & `jumanji-0.3.1/jumanji/training/networks/knapsack/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/masked_categorical_random.py` & `jumanji-0.3.1/jumanji/training/networks/masked_categorical_random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/maze/__init__.py` & `jumanji-0.3.1/jumanji/training/networks/maze/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/maze/actor_critic.py` & `jumanji-0.3.1/jumanji/training/networks/maze/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/maze/random.py` & `jumanji-0.3.1/jumanji/training/networks/maze/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/minesweeper/__init__.py` & `jumanji-0.3.1/jumanji/training/networks/minesweeper/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/minesweeper/actor_critic.py` & `jumanji-0.3.1/jumanji/training/networks/minesweeper/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/minesweeper/random.py` & `jumanji-0.3.1/jumanji/training/networks/minesweeper/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/mmst/__init__.py` & `jumanji-0.3.1/jumanji/training/networks/mmst/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/mmst/actor_critic.py` & `jumanji-0.3.1/jumanji/training/networks/mmst/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/mmst/random.py` & `jumanji-0.3.1/jumanji/training/networks/mmst/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/multi_cvrp/__init__.py` & `jumanji-0.3.1/jumanji/training/networks/multi_cvrp/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/multi_cvrp/actor_critic.py` & `jumanji-0.3.1/jumanji/training/networks/multi_cvrp/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/multi_cvrp/random.py` & `jumanji-0.3.1/jumanji/training/networks/multi_cvrp/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/parametric_distribution.py` & `jumanji-0.3.1/jumanji/training/networks/parametric_distribution.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/postprocessor.py` & `jumanji-0.3.1/jumanji/training/networks/postprocessor.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/protocols.py` & `jumanji-0.3.1/jumanji/training/networks/protocols.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/robot_warehouse/__init__.py` & `jumanji-0.3.1/jumanji/training/networks/robot_warehouse/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/robot_warehouse/actor_critic.py` & `jumanji-0.3.1/jumanji/training/networks/robot_warehouse/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/robot_warehouse/random.py` & `jumanji-0.3.1/jumanji/training/networks/robot_warehouse/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/rubiks_cube/__init__.py` & `jumanji-0.3.1/jumanji/training/networks/rubiks_cube/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/rubiks_cube/actor_critic.py` & `jumanji-0.3.1/jumanji/training/networks/rubiks_cube/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/rubiks_cube/random.py` & `jumanji-0.3.1/jumanji/training/networks/rubiks_cube/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/snake/__init__.py` & `jumanji-0.3.1/jumanji/training/networks/snake/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/snake/actor_critic.py` & `jumanji-0.3.1/jumanji/training/networks/snake/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/snake/random.py` & `jumanji-0.3.1/jumanji/training/networks/snake/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/sudoku/__init__.py` & `jumanji-0.3.1/jumanji/training/networks/sudoku/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/sudoku/actor_critic.py` & `jumanji-0.3.1/jumanji/training/networks/sudoku/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/sudoku/random.py` & `jumanji-0.3.1/jumanji/training/networks/sudoku/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/tetris/__init__.py` & `jumanji-0.3.1/jumanji/training/networks/tetris/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/tetris/actor_critic.py` & `jumanji-0.3.1/jumanji/training/networks/tetris/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/tetris/random.py` & `jumanji-0.3.1/jumanji/training/networks/tetris/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/transformer_block.py` & `jumanji-0.3.1/jumanji/training/networks/transformer_block.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/tsp/__init__.py` & `jumanji-0.3.1/jumanji/training/networks/tsp/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/tsp/actor_critic.py` & `jumanji-0.3.1/jumanji/training/networks/tsp/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/networks/tsp/random.py` & `jumanji-0.3.1/jumanji/training/networks/tsp/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/setup_train.py` & `jumanji-0.3.1/jumanji/training/setup_train.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/timer.py` & `jumanji-0.3.1/jumanji/training/timer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/train.py` & `jumanji-0.3.1/jumanji/training/train.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/types.py` & `jumanji-0.3.1/jumanji/training/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/training/utils.py` & `jumanji-0.3.1/jumanji/training/utils.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/tree_utils.py` & `jumanji-0.3.1/jumanji/tree_utils.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/types.py` & `jumanji-0.3.1/jumanji/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/version.py` & `jumanji-0.3.1/jumanji/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
```

### Comparing `jumanji-0.3.0/jumanji/viewer.py` & `jumanji-0.3.1/jumanji/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji/wrappers.py` & `jumanji-0.3.1/jumanji/wrappers.py`

 * *Files 0% similar despite different names*

```diff
@@ -638,15 +638,15 @@
     Args:
         observation: JAX pytree with (possibly nested) containers that
             either have the `__dict__` or `_asdict` methods implemented.
 
     Returns:
         Numpy array or nested dictionary of numpy arrays.
     """
-    if isinstance(observation, chex.Array):
+    if isinstance(observation, jnp.ndarray):
         return np.asarray(observation)
     elif hasattr(observation, "__dict__"):
         # Applies to various containers including `chex.dataclass`
         return {
             key: jumanji_to_gym_obs(value) for key, value in vars(observation).items()
         }
     elif hasattr(observation, "_asdict"):
```

### Comparing `jumanji-0.3.0/jumanji.egg-info/PKG-INFO` & `jumanji-0.3.1/jumanji.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jumanji
-Version: 0.3.0
+Version: 0.3.1
 Summary: A diverse suite of scalable reinforcement learning environments in JAX
 Home-page: https://github.com/instadeepai/jumanji/
 Author: InstaDeep
 Author-email: c.bonnet@instadeep.com
 License: Apache 2.0
 Keywords: reinforcement-learning python jax
 Classifier: Development Status :: 4 - Beta
@@ -243,23 +243,29 @@
 details on how to submit pull requests, our Contributor License Agreement, and community guidelines.
 
 ## Citing Jumanji ✏️
 
 If you use Jumanji in your work, please cite the library using:
 
 ```
-@software{jumanji2023github,
-  author = {Clément Bonnet and Daniel Luo and Donal Byrne and Sasha Abramowitz
-        and Vincent Coyette and Paul Duckworth and Daniel Furelos-Blanco and
-        Nathan Grinsztajn and Tristan Kalloniatis and Victor Le and Omayma Mahjoub
-        and Laurence Midgley and Shikha Surana and Cemlyn Waters and Alexandre Laterre},
-  title = {Jumanji: a Suite of Diverse and Challenging Reinforcement Learning Environments in JAX},
-  url = {https://github.com/instadeepai/jumanji},
-  version = {0.2.2},
-  year = {2023},
+@misc{bonnet2023jumanji,
+    title={Jumanji: a Diverse Suite of Scalable Reinforcement Learning Environments in JAX},
+    author={
+        Clément Bonnet and Daniel Luo and Donal Byrne and Shikha Surana and Vincent Coyette and
+        Paul Duckworth and Laurence I. Midgley and Tristan Kalloniatis and Sasha Abramowitz and
+        Cemlyn N. Waters and Andries P. Smit and Nathan Grinsztajn and Ulrich A. Mbou Sob and
+        Omayma Mahjoub and Elshadai Tegegn and Mohamed A. Mimouni and Raphael Boige and
+        Ruan de Kock and Daniel Furelos-Blanco and Victor Le and Arnu Pretorius and
+        Alexandre Laterre
+    },
+    year={2023},
+    eprint={2306.09884},
+    url={https://arxiv.org/abs/2306.09884},
+    archivePrefix={arXiv},
+    primaryClass={cs.LG}
 }
 ```
 
 ## See Also 🔎
 
 Other works have embraced the approach of writing RL environments in JAX.
 In particular, we suggest users check out the following sister repositories:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jumanji Version: 0.3.0 Summary: A diverse suite of
+Metadata-Version: 2.1 Name: jumanji Version: 0.3.1 Summary: A diverse suite of
 scalable reinforcement learning environments in JAX Home-page: https://
 github.com/instadeepai/jumanji/ Author: InstaDeep Author-email:
 c.bonnet@instadeep.com License: Apache 2.0 Keywords: reinforcement-learning
 python jax Classifier: Development Status :: 4 - Beta Classifier: Environment
 :: Console Classifier: Intended Audience :: Science/Research Classifier:
 Intended Audience :: Developers Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
@@ -180,30 +180,32 @@
 [training guide](https://instadeepai.github.io/jumanji/guides/training/). ##
 Contributing ð¤ Contributions are welcome! See our issue tracker for [good
 first issues](https://github.com/instadeepai/jumanji/labels/
 good%20first%20issue). Please read our [contributing guidelines](https://
 github.com/instadeepai/jumanji/blob/main/CONTRIBUTING.md) for details on how to
 submit pull requests, our Contributor License Agreement, and community
 guidelines. ## Citing Jumanji âï¸ If you use Jumanji in your work, please
-cite the library using: ``` @software{jumanji2023github, author = {ClÃ©ment
-Bonnet and Daniel Luo and Donal Byrne and Sasha Abramowitz and Vincent Coyette
-and Paul Duckworth and Daniel Furelos-Blanco and Nathan Grinsztajn and Tristan
-Kalloniatis and Victor Le and Omayma Mahjoub and Laurence Midgley and Shikha
-Surana and Cemlyn Waters and Alexandre Laterre}, title = {Jumanji: a Suite of
-Diverse and Challenging Reinforcement Learning Environments in JAX}, url =
-{https://github.com/instadeepai/jumanji}, version = {0.2.2}, year = {2023}, }
-``` ## See Also ð Other works have embraced the approach of writing RL
-environments in JAX. In particular, we suggest users check out the following
-sister repositories: - ð¤ [Qdax](https://github.com/adaptive-intelligent-
-robotics/QDax) is a library to accelerate Quality-Diversity and neuro-evolution
-algorithms through hardware accelerators and parallelization. - ð³ [Evojax]
-(https://github.com/google/evojax) provides tools to enable neuroevolution
-algorithms to work with neural networks running across multiple TPU/GPUs. -
-ð¦¾ [Brax](https://github.com/google/brax) is a differentiable physics engine
-that simulates environments made up of rigid bodies, joints, and actuators. -
-ðï¸â [Gymnax](https://github.com/RobertTLange/gymnax) implements classic
-environments including classic control, bsuite, MinAtar and a collection of
-meta RL tasks. - ð² [Pgx](https://github.com/sotetsuk/pgx) provides classic
-board game environments like Backgammon, Shogi, and Go. ## Acknowledgements
-ð The development of this library was supported with Cloud TPUs from
-Google's [TPU Research Cloud](https://sites.research.google/trc/about/) (TRC)
-ð¤.
+cite the library using: ``` @misc{bonnet2023jumanji, title={Jumanji: a Diverse
+Suite of Scalable Reinforcement Learning Environments in JAX}, author=
+{ ClÃ©ment Bonnet and Daniel Luo and Donal Byrne and Shikha Surana and Vincent
+Coyette and Paul Duckworth and Laurence I. Midgley and Tristan Kalloniatis and
+Sasha Abramowitz and Cemlyn N. Waters and Andries P. Smit and Nathan Grinsztajn
+and Ulrich A. Mbou Sob and Omayma Mahjoub and Elshadai Tegegn and Mohamed A.
+Mimouni and Raphael Boige and Ruan de Kock and Daniel Furelos-Blanco and Victor
+Le and Arnu Pretorius and Alexandre Laterre }, year={2023}, eprint=
+{2306.09884}, url={https://arxiv.org/abs/2306.09884}, archivePrefix={arXiv},
+primaryClass={cs.LG} } ``` ## See Also ð Other works have embraced the
+approach of writing RL environments in JAX. In particular, we suggest users
+check out the following sister repositories: - ð¤ [Qdax](https://github.com/
+adaptive-intelligent-robotics/QDax) is a library to accelerate Quality-
+Diversity and neuro-evolution algorithms through hardware accelerators and
+parallelization. - ð³ [Evojax](https://github.com/google/evojax) provides
+tools to enable neuroevolution algorithms to work with neural networks running
+across multiple TPU/GPUs. - ð¦¾ [Brax](https://github.com/google/brax) is a
+differentiable physics engine that simulates environments made up of rigid
+bodies, joints, and actuators. - ðï¸â [Gymnax](https://github.com/
+RobertTLange/gymnax) implements classic environments including classic control,
+bsuite, MinAtar and a collection of meta RL tasks. - ð² [Pgx](https://
+github.com/sotetsuk/pgx) provides classic board game environments like
+Backgammon, Shogi, and Go. ## Acknowledgements ð The development of this
+library was supported with Cloud TPUs from Google's [TPU Research Cloud](https:
+//sites.research.google/trc/about/) (TRC) ð¤.
```

### Comparing `jumanji-0.3.0/jumanji.egg-info/SOURCES.txt` & `jumanji-0.3.1/jumanji.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/jumanji.egg-info/requires.txt` & `jumanji-0.3.1/jumanji.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-chex<0.1.6,>=0.1.3
+chex>=0.1.3
 dm-env>=1.5
 gym>=0.22.0
-jax<=0.4.10,>=0.2.26
-jaxlib<=0.4.10,>=0.1.74
+jax>=0.2.26
 matplotlib>=3.3.4
 numpy>=1.19.5
 Pillow>=9.0.0
 typing-extensions>=4.0.0
 
 [dev]
 black==22.3.0
```

### Comparing `jumanji-0.3.0/pyproject.toml` & `jumanji-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/setup.cfg` & `jumanji-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `jumanji-0.3.0/setup.py` & `jumanji-0.3.1/setup.py`

 * *Files identical despite different names*

