# Comparing `tmp/open-prime-rando-0.4.2.tar.gz` & `tmp/open-prime-rando-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-prime-rando-0.4.2.tar", last modified: Wed Mar  1 20:30:41 2023, max compression
+gzip compressed data, was "open-prime-rando-0.5.0.tar", last modified: Mon Jun 19 22:52:45 2023, max compression
```

## Comparing `open-prime-rando-0.4.2.tar` & `open-prime-rando-0.5.0.tar`

### file list

```diff
@@ -1,76 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:30:41.123208 open-prime-rando-0.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:30:41.115207 open-prime-rando-0.4.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:30:41.115207 open-prime-rando-0.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/.github/workflows/python.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-01 20:30:41.123208 open-prime-rando-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:30:41.115207 open-prime-rando-0.4.2/open_prime_rando/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:30:41.119207 open-prime-rando-0.4.2/open_prime_rando/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/__pyinstaller/hook-open_prime_rando.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/dynamic_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:30:41.119207 open-prime-rando-0.4.2/open_prime_rando/echoes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:30:41.119207 open-prime-rando-0.4.2/open_prime_rando/echoes/asset_ids/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes/asset_ids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes/asset_ids/agon_wastes.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes/asset_ids/frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes/asset_ids/great_temple.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes/asset_ids/m01_sidehopperstation.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes/asset_ids/m02_spires.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes/asset_ids/m03_crossfirechaos.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes/asset_ids/m04_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes/asset_ids/m05_spidercomplex.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes/asset_ids/m06_shootinggallery.py
--rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes/asset_ids/sanctuary_fortress.py
--rw-r--r--   0 runner    (1001) docker     (123)    10303 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes/asset_ids/temple_grounds.py
--rw-r--r--   0 runner    (1001) docker     (123)    11831 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes/asset_ids/torvus_bog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes/asset_ids/world.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:30:41.111207 open-prime-rando-0.4.2/open_prime_rando/echoes/custom_assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:30:41.119207 open-prime-rando-0.4.2/open_prime_rando/echoes/custom_assets/rubiks/
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes/custom_assets/rubiks/rubiks_blue.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes/custom_assets/rubiks/rubiks_green.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes/custom_assets/rubiks/rubiks_red.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes/custom_assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:30:41.119207 open-prime-rando-0.4.2/open_prime_rando/echoes/dock_lock_rando/
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes/dock_lock_rando/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes/dock_lock_rando/dock_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes/dock_lock_rando/dock_type_database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:30:41.123208 open-prime-rando-0.4.2/open_prime_rando/echoes/inverted/
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes/inverted/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes/inverted/area_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:30:41.123208 open-prime-rando-0.4.2/open_prime_rando/echoes/small_randomizations/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes/small_randomizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes/small_randomizations/echo_locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes/small_randomizations/minigyro_chamber.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes/small_randomizations/rubiks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes/specific_area_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/echoes_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/p1r_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/patcher_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:30:41.123208 open-prime-rando-0.4.2/open_prime_rando/prime_remastered/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/prime_remastered/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/unique_area_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/open_prime_rando/validator_with_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-01 20:30:41.000000 open-prime-rando-0.4.2/open_prime_rando/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:30:41.115207 open-prime-rando-0.4.2/open_prime_rando.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-01 20:30:41.000000 open-prime-rando-0.4.2/open_prime_rando.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-03-01 20:30:41.000000 open-prime-rando-0.4.2/open_prime_rando.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 20:30:41.000000 open-prime-rando-0.4.2/open_prime_rando.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-01 20:30:41.000000 open-prime-rando-0.4.2/open_prime_rando.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 20:30:40.000000 open-prime-rando-0.4.2/open_prime_rando.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-01 20:30:41.000000 open-prime-rando-0.4.2/open_prime_rando.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-01 20:30:41.000000 open-prime-rando-0.4.2/open_prime_rando.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-01 20:30:41.123208 open-prime-rando-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:30:41.123208 open-prime-rando-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/tests/test_echoes_custom_Assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 20:30:41.123208 open-prime-rando-0.4.2/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-03-01 20:30:29.000000 open-prime-rando-0.4.2/tools/asset_id_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.291379 open-prime-rando-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.283379 open-prime-rando-0.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.283379 open-prime-rando-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/.github/workflows/python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-19 22:52:45.291379 open-prime-rando-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.283379 open-prime-rando-0.5.0/open_prime_rando/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.283379 open-prime-rando-0.5.0/open_prime_rando/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/__pyinstaller/hook-open_prime_rando.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/dynamic_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.283379 open-prime-rando-0.5.0/open_prime_rando/echoes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.287379 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/agon_wastes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/great_temple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/m01_sidehopperstation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/m02_spires.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/m03_crossfirechaos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/m04_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/m05_spidercomplex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/m06_shootinggallery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/sanctuary_fortress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14819 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/temple_grounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16919 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/torvus_bog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/world.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/auto_enabled_elevator_patches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.279379 open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.287379 open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/doors/
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_greyscale_emissive.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sonicboom.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sunburst.TXTR
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.287379 open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/rubiks/
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/rubiks/rubiks_blue.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/rubiks/rubiks_green.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/rubiks/rubiks_red.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.287379 open-prime-rando-0.5.0/open_prime_rando/echoes/dock_lock_rando/
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/dock_lock_rando/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14939 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/dock_lock_rando/dock_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/dock_lock_rando/dock_type_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/dock_lock_rando/map_icons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.287379 open-prime-rando-0.5.0/open_prime_rando/echoes/inverted/
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/inverted/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/inverted/area_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.291379 open-prime-rando-0.5.0/open_prime_rando/echoes/small_randomizations/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/small_randomizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/small_randomizations/echo_locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/small_randomizations/minigyro_chamber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/small_randomizations/rubiks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes/specific_area_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/echoes_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/p1r_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/patcher_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.291379 open-prime-rando-0.5.0/open_prime_rando/prime_remastered/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/prime_remastered/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/unique_area_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/open_prime_rando/validator_with_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 22:52:45.000000 open-prime-rando-0.5.0/open_prime_rando/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.283379 open-prime-rando-0.5.0/open_prime_rando.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-19 22:52:45.000000 open-prime-rando-0.5.0/open_prime_rando.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-06-19 22:52:45.000000 open-prime-rando-0.5.0/open_prime_rando.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 22:52:45.000000 open-prime-rando-0.5.0/open_prime_rando.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-19 22:52:45.000000 open-prime-rando-0.5.0/open_prime_rando.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 22:52:45.000000 open-prime-rando-0.5.0/open_prime_rando.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-19 22:52:45.000000 open-prime-rando-0.5.0/open_prime_rando.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-19 22:52:45.000000 open-prime-rando-0.5.0/open_prime_rando.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-19 22:52:45.291379 open-prime-rando-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.291379 open-prime-rando-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/tests/test_echoes_custom_Assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:52:45.291379 open-prime-rando-0.5.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-06-19 22:52:33.000000 open-prime-rando-0.5.0/tools/asset_id_files.py
```

### Comparing `open-prime-rando-0.4.2/.github/dependabot.yml` & `open-prime-rando-0.5.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.4.2/.github/workflows/python.yml` & `open-prime-rando-0.5.0/.github/workflows/python.yml`

 * *Files 6% similar despite different names*

```diff
@@ -19,40 +19,40 @@
         with:
           fetch-depth: 0
           submodules: 'recursive'
 
       - name: Set up Python
         uses: actions/setup-python@v2
         with:
-          python-version: "3.9"
-     
+          python-version: "3.10"
+
       - name: Install Python packages
         run: python -m pip install --upgrade pip setuptools build
 
       - name: build
         run: python -m build
-      
+
       - name: Store the packages
         uses: actions/upload-artifact@v2
         with:
           name: python-package-distributions
           path: dist
 
   test:
     needs:
       - build
-      
+
     runs-on: ubuntu-latest
     name: Test Python ${{ matrix.python.version }}
     strategy:
       fail-fast: false
       matrix:
         python:
-          - {version: '3.9', wheel: 'cp39-cp39'}
           - {version: '3.10', wheel: 'cp310-cp310'}
+          - {version: '3.11', wheel: 'cp311-cp311'}
 
     steps:
       - name: Checkout
         uses: actions/checkout@v2
 
       - name: Set up Python
         uses: actions/setup-python@v2
@@ -60,15 +60,15 @@
           python-version: ${{ matrix.python.version }}
 
       - name: Download all the dists
         uses: actions/download-artifact@v2
         with:
           name: python-package-distributions
           path: dist/
-            
+
       - name: Install Python packages
         run: python -m pip install --upgrade pip pytest
 
       - name: install built wheel
         run: python -m pip install dist/*.whl
         shell: bash
 
@@ -89,13 +89,13 @@
 
       - name: Publish 📦 to TestPyPI
         if: ${{ github.ref == 'refs/heads/main' }}
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.testpypi_password }}
           repository_url: https://test.pypi.org/legacy/
-      
+
       - name: Publish 📦 to PyPI
         if: ${{ startsWith(github.ref, 'refs/tags/') }}
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.pypi_password }}
```

### Comparing `open-prime-rando-0.4.2/.gitignore` & `open-prime-rando-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.4.2/LICENSE` & `open-prime-rando-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.4.2/PKG-INFO` & `open-prime-rando-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: open-prime-rando
-Version: 0.4.2
+Version: 0.5.0
 Summary: An open source randomizer patcher for Metroid Prime 2 and 3.
 Home-page: https://github.com/randovania/open-prime-rando
 Author: Henrique Gemignani
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Open Prime Rando
 Open Source randomizer patcher for Prime 2 and eventually 3.
```

### Comparing `open-prime-rando-0.4.2/open_prime_rando/cli.py` & `open-prime-rando-0.5.0/open_prime_rando/cli.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.4.2/open_prime_rando/dynamic_schema.py` & `open-prime-rando-0.5.0/open_prime_rando/dynamic_schema.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 from open_prime_rando.unique_area_name import get_name_for_area
 
 
 def expand_schema(base_schema: dict, editor: PatcherEditor) -> dict:
     schema = copy.deepcopy(base_schema)
 
     world_props = schema["properties"]["worlds"]["properties"] = {}
-    for world, mlvl_id in open_prime_rando.echoes.asset_ids.world.NAME_TO_ID.items():
+    for world, mlvl_id in open_prime_rando.echoes.asset_ids.world.NAME_TO_ID_MLVL.items():
         world_def = copy.deepcopy(schema["$defs"]["world"])
         world_props[world] = world_def
 
         mlvl = editor.get_mlvl(mlvl_id)
         area_props = {}
-        world_def["properties"]["areas"] = {"type": "object", "additionalProperties": False, "properties": area_props}
+        # FIXME: setting it to True for now to fix elevator rooms breaking when renamed
+        world_def["properties"]["areas"] = {"type": "object", "additionalProperties": True, "properties": area_props}
 
         world_details = open_prime_rando.echoes.asset_ids.world.load_dedicated_file(world)
 
         for area in mlvl.areas:
             area_name = get_name_for_area(area)
             area_def = copy.deepcopy(schema["$defs"]["area"])
             area_props[area_name] = area_def
```

### Comparing `open-prime-rando-0.4.2/open_prime_rando/echoes/asset_ids/world.py` & `open-prime-rando-0.5.0/open_prime_rando/echoes/asset_ids/world.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,28 +9,57 @@
 M04_PIPELINE_MLVL = 0x233E42BE
 M05_SPIDERCOMPLEX_MLVL = 0x406ADD7F
 M06_SHOOTINGGALLERY_MLVL = 0x7E19ED26
 SANCTUARY_FORTRESS_MLVL = 0x1BAA96C2
 TEMPLE_GROUNDS_MLVL = 0x3BFA3EFF
 TORVUS_BOG_MLVL = 0x3DFD2249
 
-NAME_TO_ID = {
+NAME_TO_ID_MLVL = {
     "Agon Wastes": 0x42B935E4,
     "FrontEnd": 0x69802220,
     "Great Temple": 0x863FCD72,
     "M01_SidehopperStation": 0xA50A80CC,
     "M02_Spires": 0xAE171602,
     "M03_CrossfireChaos": 0xE3B0C703,
     "M04_Pipeline": 0x233E42BE,
     "M05_SpiderComplex": 0x406ADD7F,
     "M06_ShootingGallery": 0x7E19ED26,
     "Sanctuary Fortress": 0x1BAA96C2,
     "Temple Grounds": 0x3BFA3EFF,
     "Torvus Bog": 0x3DFD2249,
 }
+# Generated by asset_id_files.py
+
+AGON_WASTES_MAPW = 0x38DBF6A5
+FRONTEND_MAPW = 0x13E2E161
+GREAT_TEMPLE_MAPW = 0xFC5D0E33
+M01_SIDEHOPPERSTATION_MAPW = 0xDF68438D
+M02_SPIRES_MAPW = 0xD475D543
+M03_CROSSFIRECHAOS_MAPW = 0x99D20442
+M04_PIPELINE_MAPW = 0x595C81FF
+M05_SPIDERCOMPLEX_MAPW = 0x3A081E3E
+M06_SHOOTINGGALLERY_MAPW = 0x047B2E67
+SANCTUARY_FORTRESS_MAPW = 0x61C85583
+TEMPLE_GROUNDS_MAPW = 0x4198FDBE
+TORVUS_BOG_MAPW = 0x479FE108
+
+NAME_TO_ID_MAPW = {
+    "Agon Wastes": 0x38DBF6A5,
+    "FrontEnd": 0x13E2E161,
+    "Great Temple": 0xFC5D0E33,
+    "M01_SidehopperStation": 0xDF68438D,
+    "M02_Spires": 0xD475D543,
+    "M03_CrossfireChaos": 0x99D20442,
+    "M04_Pipeline": 0x595C81FF,
+    "M05_SpiderComplex": 0x3A081E3E,
+    "M06_ShootingGallery": 0x047B2E67,
+    "Sanctuary Fortress": 0x61C85583,
+    "Temple Grounds": 0x4198FDBE,
+    "Torvus Bog": 0x479FE108,
+}
 
 _DEDICATED_FILES = {
     "Agon Wastes": ".agon_wastes",
     "FrontEnd": ".frontend",
     "Great Temple": ".great_temple",
     "M01_SidehopperStation": ".m01_sidehopperstation",
     "M02_Spires": ".m02_spires",
```

### Comparing `open-prime-rando-0.4.2/open_prime_rando/echoes/custom_assets/rubiks/rubiks_blue.TXTR` & `open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/rubiks/rubiks_blue.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.4.2/open_prime_rando/echoes/custom_assets/rubiks/rubiks_green.TXTR` & `open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/rubiks/rubiks_green.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.4.2/open_prime_rando/echoes/custom_assets/rubiks/rubiks_red.TXTR` & `open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets/rubiks/rubiks_red.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.4.2/open_prime_rando/echoes/custom_assets.py` & `open-prime-rando-0.5.0/open_prime_rando/echoes/custom_assets.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.4.2/open_prime_rando/echoes/inverted/__init__.py` & `open-prime-rando-0.5.0/open_prime_rando/echoes/inverted/__init__.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.4.2/open_prime_rando/echoes/inverted/area_pairs.py` & `open-prime-rando-0.5.0/open_prime_rando/echoes/inverted/area_pairs.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.4.2/open_prime_rando/echoes/schema.json` & `open-prime-rando-0.5.0/open_prime_rando/echoes/schema.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9638310185185186%*

 * *Differences: {"'$defs'": "{'area': {'properties': {'low_memory_mode': OrderedDict([('type', 'boolean'), "*

 * *            "('default', False)])}}, 'dock': {'properties': {'old_door_type': "*

 * *            "OrderedDict([('$ref', '#/$defs/dock_type')]), 'new_door_type': OrderedDict([('$ref', "*

 * *            "'#/$defs/dock_type')])}}, 'dock_type': OrderedDict([('type', 'string'), ('enum', "*

 * *            "['Normal', 'Dark', 'Light', 'Annihilator', 'Disabled', 'Missile', 'SuperMissile', "*

 * *            "'PowerBomb', 'SeekerMissile', 'Sc […]*

```diff
@@ -18,14 +18,18 @@
                     "default": {},
                     "patternProperties": {
                         ".*": {
                             "type": "boolean"
                         }
                     },
                     "type": "object"
+                },
+                "low_memory_mode": {
+                    "default": false,
+                    "type": "boolean"
                 }
             },
             "type": "object"
         },
         "dock": {
             "additionalProperties": false,
             "default": {},
@@ -41,18 +45,48 @@
                         }
                     },
                     "required": [
                         "area",
                         "dock"
                     ],
                     "type": "object"
+                },
+                "new_door_type": {
+                    "$ref": "#/$defs/dock_type"
+                },
+                "old_door_type": {
+                    "$ref": "#/$defs/dock_type"
                 }
             },
             "type": "object"
         },
+        "dock_type": {
+            "enum": [
+                "Normal",
+                "Dark",
+                "Light",
+                "Annihilator",
+                "Disabled",
+                "Missile",
+                "SuperMissile",
+                "PowerBomb",
+                "SeekerMissile",
+                "ScrewAttack",
+                "Bomb",
+                "Boost",
+                "Grapple",
+                "Darkburst",
+                "Sunburst",
+                "SonicBoom",
+                "AgonEnergy",
+                "TorvusEnergy",
+                "SanctuaryEnergy"
+            ],
+            "type": "string"
+        },
         "world": {
             "$comment": "The list of areas is replaced in runtime with the existing areas of each specific world.",
             "additionalProperties": false,
             "properties": {
                 "areas": {
                     "patternProperties": {
                         ".*": {
@@ -83,14 +117,19 @@
                     "default": false,
                     "description": "Remove objects to minimize the chance of alloc failure",
                     "type": "boolean"
                 }
             },
             "type": "object"
         },
+        "auto_enabled_elevators": {
+            "default": false,
+            "description": "Set elevators to be activated on room load",
+            "type": "boolean"
+        },
         "inverted": {
             "default": false,
             "description": "Inverts Light and Dark Aether",
             "type": "boolean"
         },
         "small_randomizations": {
             "additionalProperties": false,
```

### Comparing `open-prime-rando-0.4.2/open_prime_rando/echoes/small_randomizations/__init__.py` & `open-prime-rando-0.5.0/open_prime_rando/echoes/small_randomizations/__init__.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.4.2/open_prime_rando/echoes/small_randomizations/echo_locks.py` & `open-prime-rando-0.5.0/open_prime_rando/echoes/small_randomizations/echo_locks.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.4.2/open_prime_rando/echoes/small_randomizations/minigyro_chamber.py` & `open-prime-rando-0.5.0/open_prime_rando/echoes/small_randomizations/minigyro_chamber.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.4.2/open_prime_rando/echoes/small_randomizations/rubiks.py` & `open-prime-rando-0.5.0/open_prime_rando/echoes/small_randomizations/rubiks.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.4.2/open_prime_rando/echoes/specific_area_patches.py` & `open-prime-rando-0.5.0/open_prime_rando/echoes/specific_area_patches.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import logging
 
 from construct import Container
 
-from open_prime_rando.echoes.asset_ids.agon_wastes import MINING_STATION_B_MREA
+from open_prime_rando.echoes.asset_ids.agon_wastes import MINING_STATION_B_MREA, PORTAL_TERMINAL_MREA
 from open_prime_rando.echoes.asset_ids.torvus_bog import TORVUS_ENERGY_CONTROLLER_MREA, TORVUS_TEMPLE_MREA
 from open_prime_rando.echoes.asset_ids.world import TORVUS_BOG_MLVL
 from open_prime_rando.patcher_editor import PatcherEditor
 from retro_data_structures.formats.script_object import ScriptInstanceHelper
 from retro_data_structures.game_check import Game
+from retro_data_structures.properties.echoes.objects.Counter import Counter
 from retro_data_structures.properties.echoes.objects.Relay import Relay
 from retro_data_structures.properties.echoes.objects.ScriptLayerController import ScriptLayerController
 
 LOG = logging.getLogger("echoes_patcher")
 
 
 def specific_patches(editor: PatcherEditor, area_patches: dict):
@@ -91,7 +92,36 @@
 
     # These are generated objects, so to remove these we need to change the generated objects layer
     # Since that isn't properly exposed by RDS, let's skip for now
     # debris = ["SwampCrateDebris"] * 7
     # for obj in ["GibFlash", "Sound - Swamp Crate Gib"] + debris:
     #     default.remove_instance(obj)
 
+
+def agon_wastes_portal_terminal_puzzle_patch(editor: PatcherEditor):
+    """
+    Patches Agon Wastes - Portal Terminal to behave like in GC NTSC-U/PAL
+    In GC NTSC-J version a counter was added to check for each cork to be broken
+    """
+    area = editor.get_mrea(PORTAL_TERMINAL_MREA)
+
+    """
+    Remove counter increment on the 2 first corks to destroy
+    """
+    relay_ids = [0x12033A, 0x120343]  # 0x120307 is the last cork to destroy
+    for relay_id in relay_ids:
+        relay = area.get_instance(relay_id)
+
+        properties = relay.get_properties()
+        assert isinstance(properties, Relay)
+        relay.remove_connections([0x12044E])
+        relay.set_properties(properties)
+
+    """
+    Set the destroyed cork counter to expect only one cork to be destroyed
+    """
+    counter = area.get_instance(0x12044E)
+
+    properties = counter.get_properties_as(Counter)
+    properties.editor_properties.unknown = 1
+    properties.max_count = 1
+    counter.set_properties(properties)
```

### Comparing `open-prime-rando-0.4.2/open_prime_rando/echoes_patcher.py` & `open-prime-rando-0.5.0/open_prime_rando/echoes_patcher.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import logging
 from pathlib import Path
 
 from open_prime_rando import dynamic_schema
-from open_prime_rando.echoes import specific_area_patches, asset_ids
+from open_prime_rando.echoes import auto_enabled_elevator_patches, specific_area_patches, asset_ids, dock_lock_rando
 from open_prime_rando.echoes.inverted import apply_inverted
 from open_prime_rando.echoes.small_randomizations import apply_small_randomizations
 from open_prime_rando.patcher_editor import PatcherEditor
 from open_prime_rando.unique_area_name import get_name_for_area
 from open_prime_rando.validator_with_default import DefaultValidatingDraft7Validator
 from retro_data_structures.asset_manager import FileProvider
 from retro_data_structures.formats.mlvl import AreaWrapper
@@ -20,57 +20,76 @@
     with Path(__file__).parent.joinpath("echoes", "schema.json").open() as f:
         return json.load(f)
 
 
 def apply_area_modifications(editor: PatcherEditor, configuration: dict[str, dict]):
     for world_name, world_config in configuration.items():
         world_meta = asset_ids.world.load_dedicated_file(world_name)
-        mlvl = editor.get_mlvl(asset_ids.world.NAME_TO_ID[world_name])
+        mlvl = editor.get_mlvl(asset_ids.world.NAME_TO_ID_MLVL[world_name])
 
         areas_by_name: dict[str, AreaWrapper] = {
             get_name_for_area(area): area
             for area in mlvl.areas
         }
 
-        for area_name, area in areas_by_name.items():
+        for i, (area_name, area) in enumerate(areas_by_name.items()):
             if area_name not in world_config["areas"]:
                 continue
+            
+            LOG.info(f"[{100*i/len(areas_by_name)}%] Processing {area_name}...")
 
             area_config = world_config["areas"][area_name]
+            low_memory = area_config["low_memory_mode"]
 
             for dock_name, dock_config in area_config["docks"].items():
                 dock_number = world_meta.DOCK_NAMES[area_name][dock_name]
+
+                if "new_door_type" in dock_config:
+                    dock_lock_rando.apply_door_rando(
+                        editor,
+                        world_name,
+                        area_name,
+                        dock_name,
+                        dock_config["new_door_type"],
+                        dock_config.get("old_door_type"),
+                        low_memory
+                    )
+                
                 if "connect_to" in dock_config:
                     dock_target = dock_config["connect_to"]
                     LOG.debug("Connecting dock %s of %s - %s to %s - %s",
                               dock_name, world_name, area_name, dock_target["area"], dock_target["dock"])
                     area.connect_dock_to(dock_number, areas_by_name[dock_target["area"]],
                                          world_meta.DOCK_NAMES[dock_target["area"]][dock_target["dock"]])
 
             for layer_name, layer_state in area_config["layers"].items():
                 LOG.debug("Setting layer %s of %s - %s to %s", layer_name, world_name, area_name, str(layer_state))
                 area.get_layer(layer_name).active = layer_state
+        
+            area.build_mlvl_dependencies(only_modified=True)
 
 
 def patch_paks(file_provider: FileProvider, output_path: Path, configuration: dict):
     LOG.info("Will patch files at %s", file_provider)
 
     editor = PatcherEditor(file_provider, Game.ECHOES)
 
     LOG.info("Preparing schema")
     schema = dynamic_schema.expand_schema(_read_schema(), editor)
 
     LOG.info("Validating schema")
     DefaultValidatingDraft7Validator(schema).validate(configuration)
 
     # custom_assets.create_custom_assets(editor)
+    dock_lock_rando.add_custom_models(editor)
+    if configuration["auto_enabled_elevators"]:
+        auto_enabled_elevator_patches.apply_auto_enabled_elevators_patch(editor)
     specific_area_patches.specific_patches(editor, configuration["area_patches"])
     apply_area_modifications(editor, configuration["worlds"])
     apply_small_randomizations(editor, configuration["small_randomizations"])
-    # apply_door_rando(editor, [])
 
     if configuration["inverted"]:
         apply_inverted(editor)
 
     # Save our changes
     editor.flush_modified_assets()
```

### Comparing `open-prime-rando-0.4.2/open_prime_rando/p1r_patcher.py` & `open-prime-rando-0.5.0/open_prime_rando/p1r_patcher.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.4.2/open_prime_rando/patcher_editor.py` & `open-prime-rando-0.5.0/open_prime_rando/patcher_editor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import io
 import typing
 from concurrent.futures import ThreadPoolExecutor
 from pathlib import Path
 
 from ppc_asm.dol_file import DolEditor, DolHeader
 from retro_data_structures.asset_manager import AssetManager, FileProvider
-from retro_data_structures.base_resource import BaseResource, NameOrAssetId, RawResource, AssetId
+from retro_data_structures.base_resource import Resource, BaseResource, NameOrAssetId, RawResource, AssetId
 from retro_data_structures.crc import crc32
 from retro_data_structures.formats.mlvl import Mlvl, AreaWrapper
 from retro_data_structures.formats.mrea import Mrea
 from retro_data_structures.game_check import Game
 
 T = typing.TypeVar("T")
 
@@ -73,7 +73,16 @@
     def save_modifications(self, output_path: Path):
         super().save_modifications(output_path)
 
         if self.dol is not None:
             target_dol = output_path.joinpath("sys/main.dol")
             target_dol.parent.mkdir(exist_ok=True, parents=True)
             target_dol.write_bytes(self.dol.dol_file.getvalue())
+
+    def add_or_replace_custom_asset(self, name: str, new_data: Resource, in_paks: typing.Iterable[str] = ()) -> AssetId:
+        if self.does_asset_exists(name):
+            asset_id = self.replace_asset(name, new_data)
+            for pak in in_paks:
+                self.ensure_present(pak, asset_id)
+        else:
+            asset_id = self.add_file(name, new_data, in_paks)
+        return asset_id
```

### Comparing `open-prime-rando-0.4.2/open_prime_rando/validator_with_default.py` & `open-prime-rando-0.5.0/open_prime_rando/validator_with_default.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.4.2/open_prime_rando.egg-info/PKG-INFO` & `open-prime-rando-0.5.0/open_prime_rando.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: open-prime-rando
-Version: 0.4.2
+Version: 0.5.0
 Summary: An open source randomizer patcher for Metroid Prime 2 and 3.
 Home-page: https://github.com/randovania/open-prime-rando
 Author: Henrique Gemignani
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Open Prime Rando
 Open Source randomizer patcher for Prime 2 and eventually 3.
```

### Comparing `open-prime-rando-0.4.2/open_prime_rando.egg-info/SOURCES.txt` & `open-prime-rando-0.5.0/open_prime_rando.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .gitignore
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 .github/dependabot.yml
 .github/workflows/python.yml
 open_prime_rando/__init__.py
@@ -21,14 +22,15 @@
 open_prime_rando.egg-info/dependency_links.txt
 open_prime_rando.egg-info/entry_points.txt
 open_prime_rando.egg-info/not-zip-safe
 open_prime_rando.egg-info/requires.txt
 open_prime_rando.egg-info/top_level.txt
 open_prime_rando/__pyinstaller/__init__.py
 open_prime_rando/__pyinstaller/hook-open_prime_rando.py
+open_prime_rando/echoes/auto_enabled_elevator_patches.py
 open_prime_rando/echoes/custom_assets.py
 open_prime_rando/echoes/schema.json
 open_prime_rando/echoes/specific_area_patches.py
 open_prime_rando/echoes/asset_ids/__init__.py
 open_prime_rando/echoes/asset_ids/agon_wastes.py
 open_prime_rando/echoes/asset_ids/frontend.py
 open_prime_rando/echoes/asset_ids/great_temple.py
@@ -38,20 +40,25 @@
 open_prime_rando/echoes/asset_ids/m04_pipeline.py
 open_prime_rando/echoes/asset_ids/m05_spidercomplex.py
 open_prime_rando/echoes/asset_ids/m06_shootinggallery.py
 open_prime_rando/echoes/asset_ids/sanctuary_fortress.py
 open_prime_rando/echoes/asset_ids/temple_grounds.py
 open_prime_rando/echoes/asset_ids/torvus_bog.py
 open_prime_rando/echoes/asset_ids/world.py
+open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst.TXTR
+open_prime_rando/echoes/custom_assets/doors/custom_door_lock_greyscale_emissive.TXTR
+open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sonicboom.TXTR
+open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sunburst.TXTR
 open_prime_rando/echoes/custom_assets/rubiks/rubiks_blue.TXTR
 open_prime_rando/echoes/custom_assets/rubiks/rubiks_green.TXTR
 open_prime_rando/echoes/custom_assets/rubiks/rubiks_red.TXTR
 open_prime_rando/echoes/dock_lock_rando/__init__.py
 open_prime_rando/echoes/dock_lock_rando/dock_type.py
 open_prime_rando/echoes/dock_lock_rando/dock_type_database.py
+open_prime_rando/echoes/dock_lock_rando/map_icons.py
 open_prime_rando/echoes/inverted/__init__.py
 open_prime_rando/echoes/inverted/area_pairs.py
 open_prime_rando/echoes/small_randomizations/__init__.py
 open_prime_rando/echoes/small_randomizations/echo_locks.py
 open_prime_rando/echoes/small_randomizations/minigyro_chamber.py
 open_prime_rando/echoes/small_randomizations/rubiks.py
 open_prime_rando/prime_remastered/schema.json
```

### Comparing `open-prime-rando-0.4.2/setup.cfg` & `open-prime-rando-0.5.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 long_description_content_type = text/markdown
 url = https://github.com/randovania/open-prime-rando
 author = Henrique Gemignani
 classifiers = 
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Development Status :: 3 - Alpha
 	Intended Audience :: Developers
-	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 
 [options]
 packages = find:
 install_requires = 
-	retro-data-structures>=0.18.0
+	retro-data-structures>=0.19.1
 	jsonschema>=4.0.0
 	ppc-asm
 include_package_data = True
 zip_safe = False
-python_requires = >=3.9
+python_requires = >=3.10
 
 [options.packages.find]
 exclude = 
 	test
 
 [options.package_data]
 open_prime_rando.echoes =
```

### Comparing `open-prime-rando-0.4.2/tests/test_echoes_custom_Assets.py` & `open-prime-rando-0.5.0/tests/test_echoes_custom_Assets.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.4.2/tools/asset_id_files.py` & `open-prime-rando-0.5.0/tools/asset_id_files.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,27 +51,28 @@
     template = f"# Generated by {os.path.basename(__file__)}\n\n"
     template += "\n".join(
         f"{filter_name(key)}{suffix} = 0x{items[key]:08X}"
         for key in sorted(items)
     )
     template += "\n"
 
-    template += "\nNAME_TO_ID = {\n"
+    template += f"\nNAME_TO_ID{suffix}" + " = {\n"
     for name in sorted(items):
         template += f"    \"{name}\": 0x{items[name]:08X},\n"
     template += "}\n"
 
     return template
 
 
 def create_asset_id_files(editor: PatcherEditor, output_path: Path):
     output_path.mkdir(parents=True, exist_ok=True)
 
     custom_world_names = _CUSTOM_WORLD_NAMES.get(editor.target_game, {})
     world_names = {}
+    mapw_names = {}
 
     for value in editor.all_asset_ids():
         if editor.get_asset_type(value).lower() != "mlvl":
             continue
 
         mlvl = editor.get_mlvl(value)
 
@@ -81,28 +82,31 @@
         except retro_data_structures.exceptions.UnknownAssetId:
             if value not in custom_world_names:
                 print(f"Skipping MLVL {value}: no name found")
                 continue
             world_name = custom_world_names[value]
 
         world_names[world_name] = value
+        mapw_names[world_name] = mlvl.raw.world_map_id
 
         area_names = {}
+        mapa_names = {}
         dock_names = {}
 
-        for area in mlvl.raw.areas:
+        for area, mapa in zip(mlvl.raw.areas, mlvl.mapw.mapa_ids):
             try:
                 strg = editor.get_parsed_asset(area.area_name_id, type_hint=Strg)
                 area_name = strg.raw.string_tables[0].strings[0].string
             except retro_data_structures.exceptions.UnknownAssetId:
                 area_name = area.internal_area_name
             area_name = _CUSTOM_AREA_NAMES[editor.target_game].get(area.area_mrea_id, area_name)
 
             assert area_name not in area_names, area_name
             area_names[area_name] = area.area_mrea_id
+            mapa_names[area_name] = mapa
             mrea = editor.get_parsed_asset(area_names[area_name], type_hint=Mrea)
 
             docks = {}
             for layer in mrea.script_layers:
                 for obj in layer.instances:
                     if obj.type_name == "DOCK":
                         dock: Dock = obj.get_properties_as(Dock)
@@ -112,18 +116,20 @@
                 # Docks are in the default layer, ignore the rest
                 break
 
             assert max(docks.values(), default=-1) == len(docks) - 1
             dock_names[area_name] = docks
 
         world_file_body = generate_template(area_names, "_MREA")
+        world_file_body += generate_template(mapa_names, "_MAPA")
         world_file_body += dock_name_templates(dock_names)
         output_path.joinpath(f"{filter_name(world_name).lower()}.py").write_text(world_file_body)
 
     global_file_body = generate_template(world_names, "_MLVL")
+    global_file_body += generate_template(mapw_names, "_MAPW")
 
     global_file_body += "\n_DEDICATED_FILES = {\n"
     for name in sorted(world_names.keys()):
         global_file_body += f"    \"{name}\": \".{filter_name(name).lower()}\",\n"
     global_file_body += """}
```

