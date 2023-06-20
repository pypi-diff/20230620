# Comparing `tmp/mgtron-2.16.1.tar.gz` & `tmp/mgtron-2.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mgtron-2.16.1.tar", last modified: Tue Jun 20 13:36:02 2023, max compression
+gzip compressed data, was "mgtron-2.17.0.tar", last modified: Tue Jun 20 13:49:54 2023, max compression
```

## Comparing `mgtron-2.16.1.tar` & `mgtron-2.17.0.tar`

### file list

```diff
@@ -1,87 +1,101 @@
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:36:02.165434 mgtron-2.16.1/
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:36:02.155433 mgtron-2.16.1/.github/
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:36:02.155433 mgtron-2.16.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      602 2023-06-09 13:32:26.000000 mgtron-2.16.1/.github/ISSUE_TEMPLATE/mgtron--.md
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1524 2023-06-09 13:32:26.000000 mgtron-2.16.1/.github/ISSUE_TEMPLATE/mgtron_issue.yml
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:36:02.155433 mgtron-2.16.1/.github/workflows/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      457 2023-06-09 13:32:26.000000 mgtron-2.16.1/.github/workflows/black_actions.yml
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      365 2023-06-19 20:47:25.000000 mgtron-2.16.1/.gitignore
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     7692 2023-06-19 20:47:25.000000 mgtron-2.16.1/CHANGELOG.md
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      957 2023-06-19 20:47:25.000000 mgtron-2.16.1/LICENSE.rst
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    11983 2023-06-20 13:36:02.165434 mgtron-2.16.1/PKG-INFO
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3794 2023-06-19 20:47:25.000000 mgtron-2.16.1/README.md
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:36:02.155433 mgtron-2.16.1/docs/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    17614 2023-06-09 13:32:26.000000 mgtron-2.16.1/docs/MGTron Command Description.docx
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    23088 2023-06-09 13:32:26.000000 mgtron-2.16.1/docs/MGTron Function Descriptions.docx
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2788 2023-06-20 13:21:31.000000 mgtron-2.16.1/pyproject.toml
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1553 2023-06-19 20:47:25.000000 mgtron-2.16.1/requirements.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       38 2023-06-20 13:36:02.165434 mgtron-2.16.1/setup.cfg
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:36:02.155433 mgtron-2.16.1/src/
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        1 2023-06-16 17:38:51.000000 mgtron-2.16.1/src/__init__.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:36:02.162100 mgtron-2.16.1/src/assets/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    83964 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/assets/CA logo without subtext.JPG
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    65978 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/assets/CA_subheading.png
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     7692 2023-06-19 20:47:25.000000 mgtron-2.16.1/src/assets/CHANGELOG.cpy
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000) 12822184 2023-06-19 20:53:16.000000 mgtron-2.16.1/src/assets/blueio_rs
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)     1303 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/assets/init_cellantenna.sh
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      291 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/assets/mgtron.desktop
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2655 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/assets/mgtron.svg
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    67646 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/assets/network-wireless.ico
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:36:02.162100 mgtron-2.16.1/src/ble/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-16 17:38:51.000000 mgtron-2.16.1/src/ble/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      832 2023-06-19 20:47:25.000000 mgtron-2.16.1/src/ble/ble.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2728 2023-06-19 20:47:25.000000 mgtron-2.16.1/src/ble/ble_data.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1738 2023-06-19 20:47:25.000000 mgtron-2.16.1/src/ble/helpers.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:36:02.162100 mgtron-2.16.1/src/gui/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       80 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/__init__.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:36:02.162100 mgtron-2.16.1/src/gui/_configs/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/_configs/card_1.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/_configs/card_2.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/_configs/card_3.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/_configs/card_4.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/_configs/card_5.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/_configs/card_6.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      263 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/_configs/card_7.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/_configs/card_8.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      105 2023-06-20 13:34:54.000000 mgtron-2.16.1/src/gui/_configs/card_config.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      317 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/_configs/mission_alpha.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      292 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/_configs/mission_bravo.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      324 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/_configs/mission_charlie.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      312 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/_configs/mission_delta.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      273 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/_configs/mission_echo.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      313 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/_configs/mission_fox.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      279 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/_configs/mission_golf.ini
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:36:02.162100 mgtron-2.16.1/src/gui/db/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/db/channel_1.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/db/channel_2.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/db/channel_3.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/db/channel_4.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/db/channel_5.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/db/channel_6.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/db/channel_7.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/db/channel_8.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2516 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/db/init_db.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10906 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/db/long_save.json
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/db/long_save.json.lock
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    49152 2023-06-14 02:00:32.000000 mgtron-2.16.1/src/gui/db/mgtron_db.db
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     8856 2023-06-16 17:38:51.000000 mgtron-2.16.1/src/gui/db/models.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1170 2023-06-16 17:38:51.000000 mgtron-2.16.1/src/gui/db/quick_save.json
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:36:02.162100 mgtron-2.16.1/src/gui/fonts/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1260156 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/fonts/MesloLGS NF Bold Italic.ttf
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1251424 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/fonts/MesloLGS NF Italic.ttf
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1292408 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/gui/fonts/MesloLGS NF Regular.ttf
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    64899 2023-06-20 13:25:32.000000 mgtron-2.16.1/src/gui/helpers.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10789 2023-06-19 20:47:25.000000 mgtron-2.16.1/src/gui/interface.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    43537 2023-06-20 13:17:12.000000 mgtron-2.16.1/src/main.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:36:02.165434 mgtron-2.16.1/src/mgtron.egg-info/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    11983 2023-06-20 13:36:02.000000 mgtron-2.16.1/src/mgtron.egg-info/PKG-INFO
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1926 2023-06-20 13:36:02.000000 mgtron-2.16.1/src/mgtron.egg-info/SOURCES.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        1 2023-06-20 13:36:02.000000 mgtron-2.16.1/src/mgtron.egg-info/dependency_links.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       37 2023-06-20 13:36:02.000000 mgtron-2.16.1/src/mgtron.egg-info/entry_points.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1531 2023-06-20 13:36:02.000000 mgtron-2.16.1/src/mgtron.egg-info/requires.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       21 2023-06-20 13:36:02.000000 mgtron-2.16.1/src/mgtron.egg-info/top_level.txt
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:36:02.165434 mgtron-2.16.1/src/tests/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       33 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/tests/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       70 2023-06-19 20:47:25.000000 mgtron-2.16.1/src/tests/test_ble.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    63110 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/tests/test_configfiles.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    19813 2023-06-09 13:32:26.000000 mgtron-2.16.1/src/tests/test_helpers.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:49:54.370065 mgtron-2.17.0/
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:49:54.363398 mgtron-2.17.0/.github/
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:49:54.363398 mgtron-2.17.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      602 2023-06-09 13:32:26.000000 mgtron-2.17.0/.github/ISSUE_TEMPLATE/mgtron--.md
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1524 2023-06-09 13:32:26.000000 mgtron-2.17.0/.github/ISSUE_TEMPLATE/mgtron_issue.yml
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:49:54.363398 mgtron-2.17.0/.github/workflows/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      457 2023-06-09 13:32:26.000000 mgtron-2.17.0/.github/workflows/black_actions.yml
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      365 2023-06-19 20:47:25.000000 mgtron-2.17.0/.gitignore
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     7692 2023-06-19 20:47:25.000000 mgtron-2.17.0/CHANGELOG.md
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      957 2023-06-19 20:47:25.000000 mgtron-2.17.0/LICENSE.rst
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    11983 2023-06-20 13:49:54.370065 mgtron-2.17.0/PKG-INFO
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3794 2023-06-19 20:47:25.000000 mgtron-2.17.0/README.md
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:49:54.363398 mgtron-2.17.0/docs/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    17614 2023-06-09 13:32:26.000000 mgtron-2.17.0/docs/MGTron Command Description.docx
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    23088 2023-06-09 13:32:26.000000 mgtron-2.17.0/docs/MGTron Function Descriptions.docx
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:49:54.363398 mgtron-2.17.0/mgtron.egg-info/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    11983 2023-06-20 13:49:52.000000 mgtron-2.17.0/mgtron.egg-info/PKG-INFO
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2171 2023-06-20 13:49:54.000000 mgtron-2.17.0/mgtron.egg-info/SOURCES.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        1 2023-06-20 13:49:52.000000 mgtron-2.17.0/mgtron.egg-info/dependency_links.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       37 2023-06-20 13:49:52.000000 mgtron-2.17.0/mgtron.egg-info/entry_points.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1531 2023-06-20 13:49:52.000000 mgtron-2.17.0/mgtron.egg-info/requires.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       25 2023-06-20 13:49:52.000000 mgtron-2.17.0/mgtron.egg-info/top_level.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2786 2023-06-20 13:49:45.000000 mgtron-2.17.0/pyproject.toml
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1553 2023-06-19 20:47:25.000000 mgtron-2.17.0/requirements.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       38 2023-06-20 13:49:54.370065 mgtron-2.17.0/setup.cfg
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:49:54.363398 mgtron-2.17.0/src/
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        1 2023-06-16 17:38:51.000000 mgtron-2.17.0/src/__init__.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:49:54.366732 mgtron-2.17.0/src/assets/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    83964 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/assets/CA logo without subtext.JPG
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    65978 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/assets/CA_subheading.png
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     7692 2023-06-20 13:48:47.000000 mgtron-2.17.0/src/assets/CHANGELOG.cpy
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000) 12822184 2023-06-19 20:53:16.000000 mgtron-2.17.0/src/assets/blueio_rs
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)     1303 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/assets/init_cellantenna.sh
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      291 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/assets/mgtron.desktop
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2655 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/assets/mgtron.svg
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    67646 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/assets/network-wireless.ico
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:49:54.366732 mgtron-2.17.0/src/ble/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-16 17:38:51.000000 mgtron-2.17.0/src/ble/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      832 2023-06-19 20:47:25.000000 mgtron-2.17.0/src/ble/ble.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2728 2023-06-19 20:47:25.000000 mgtron-2.17.0/src/ble/ble_data.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1738 2023-06-19 20:47:25.000000 mgtron-2.17.0/src/ble/helpers.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:49:54.366732 mgtron-2.17.0/src/gui/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       80 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/__init__.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:49:54.366732 mgtron-2.17.0/src/gui/_configs/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/_configs/card_1.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/_configs/card_2.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/_configs/card_3.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/_configs/card_4.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/_configs/card_5.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/_configs/card_6.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      263 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/_configs/card_7.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/_configs/card_8.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      105 2023-06-20 13:48:53.000000 mgtron-2.17.0/src/gui/_configs/card_config.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      317 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/_configs/mission_alpha.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      292 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/_configs/mission_bravo.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      324 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/_configs/mission_charlie.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      312 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/_configs/mission_delta.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      273 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/_configs/mission_echo.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      313 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/_configs/mission_fox.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      279 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/_configs/mission_golf.ini
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:49:54.370065 mgtron-2.17.0/src/gui/db/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/db/channel_1.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/db/channel_2.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/db/channel_3.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/db/channel_4.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/db/channel_5.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/db/channel_6.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/db/channel_7.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/db/channel_8.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2516 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/db/init_db.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10906 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/db/long_save.json
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/db/long_save.json.lock
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    49152 2023-06-14 02:00:32.000000 mgtron-2.17.0/src/gui/db/mgtron_db.db
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     8856 2023-06-16 17:38:51.000000 mgtron-2.17.0/src/gui/db/models.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1170 2023-06-16 17:38:51.000000 mgtron-2.17.0/src/gui/db/quick_save.json
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:49:54.370065 mgtron-2.17.0/src/gui/fonts/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1260156 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/fonts/MesloLGS NF Bold Italic.ttf
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1251424 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/fonts/MesloLGS NF Italic.ttf
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1292408 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/gui/fonts/MesloLGS NF Regular.ttf
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    64899 2023-06-20 13:25:32.000000 mgtron-2.17.0/src/gui/helpers.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10789 2023-06-19 20:47:25.000000 mgtron-2.17.0/src/gui/interface.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    43537 2023-06-20 13:17:12.000000 mgtron-2.17.0/src/main.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:49:54.370065 mgtron-2.17.0/src/tests/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       33 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/tests/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       70 2023-06-19 20:47:25.000000 mgtron-2.17.0/src/tests/test_ble.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    63110 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/tests/test_configfiles.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    19813 2023-06-09 13:32:26.000000 mgtron-2.17.0/src/tests/test_helpers.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:49:54.363398 mgtron-2.17.0/venv/
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-20 13:49:54.370065 mgtron-2.17.0/venv/bin/
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      666 2023-06-16 19:42:57.000000 mgtron-2.17.0/venv/bin/rst2html.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      788 2023-06-16 19:42:57.000000 mgtron-2.17.0/venv/bin/rst2html4.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)     1123 2023-06-16 19:42:57.000000 mgtron-2.17.0/venv/bin/rst2html5.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      865 2023-06-16 19:42:57.000000 mgtron-2.17.0/venv/bin/rst2latex.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      688 2023-06-16 19:42:57.000000 mgtron-2.17.0/venv/bin/rst2man.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      854 2023-06-16 19:42:57.000000 mgtron-2.17.0/venv/bin/rst2odt.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      660 2023-06-16 19:42:57.000000 mgtron-2.17.0/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      673 2023-06-16 19:42:57.000000 mgtron-2.17.0/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      709 2023-06-16 19:42:57.000000 mgtron-2.17.0/venv/bin/rst2s5.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      945 2023-06-16 19:42:57.000000 mgtron-2.17.0/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      674 2023-06-16 19:42:57.000000 mgtron-2.17.0/venv/bin/rst2xml.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      742 2023-06-16 19:42:57.000000 mgtron-2.17.0/venv/bin/rstpep2html.py
```

### Comparing `mgtron-2.16.1/.github/ISSUE_TEMPLATE/mgtron--.md` & `mgtron-2.17.0/.github/ISSUE_TEMPLATE/mgtron--.md`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/.github/ISSUE_TEMPLATE/mgtron_issue.yml` & `mgtron-2.17.0/.github/ISSUE_TEMPLATE/mgtron_issue.yml`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/CHANGELOG.md` & `mgtron-2.17.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/LICENSE.rst` & `mgtron-2.17.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/PKG-INFO` & `mgtron-2.17.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mgtron
-Version: 2.16.1
+Version: 2.17.0
 Summary: Package for MGTron GUI, a user interface for signal generation
 Author-email: Christerpher Hunter <chunter@cellantenna.com>
 Project-URL: Source, https://github.com/cellantenna/mg_tron
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
```

### Comparing `mgtron-2.16.1/README.md` & `mgtron-2.17.0/README.md`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/docs/MGTron Command Description.docx` & `mgtron-2.17.0/docs/MGTron Command Description.docx`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/docs/MGTron Function Descriptions.docx` & `mgtron-2.17.0/docs/MGTron Function Descriptions.docx`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/pyproject.toml` & `mgtron-2.17.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "mgtron"
 authors = [
   { name="Christerpher Hunter", email="chunter@cellantenna.com" },
 ]
 dynamic = ["readme"]
 description = "Package for MGTron GUI, a user interface for signal generation"
-version = "2.16.1"
+version = "2.17.0"
 requires-python = ">=3.10"
 classifiers = [
 "Programming Language :: Python :: 3",
 "License :: Other/Proprietary License",
 "Operating System :: POSIX :: Linux",
 ]
 
@@ -122,15 +122,15 @@
 mgtron = "src.main:main"
 
 [tools.setuptools]
 include-package-data = "True"
 
 [tool.setuptools.packages.find]
 namespaces = true
-where = ["src"]
+where = ["."]
 
 [tool.setuptools.package-data]
 "*" = [
 "*.ini",
 "*.sql",
 "*.db",
 "*.json",
```

### Comparing `mgtron-2.16.1/requirements.txt` & `mgtron-2.17.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/src/assets/CA logo without subtext.JPG` & `mgtron-2.17.0/src/assets/CA logo without subtext.JPG`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/src/assets/CA_subheading.png` & `mgtron-2.17.0/src/assets/CA_subheading.png`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/src/assets/CHANGELOG.cpy` & `mgtron-2.17.0/src/assets/CHANGELOG.cpy`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/src/assets/blueio_rs` & `mgtron-2.17.0/src/assets/blueio_rs`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/src/assets/init_cellantenna.sh` & `mgtron-2.17.0/src/assets/init_cellantenna.sh`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/src/assets/mgtron.svg` & `mgtron-2.17.0/src/assets/mgtron.svg`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/src/assets/network-wireless.ico` & `mgtron-2.17.0/src/assets/network-wireless.ico`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/src/ble/ble.py` & `mgtron-2.17.0/src/ble/ble.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/src/ble/ble_data.py` & `mgtron-2.17.0/src/ble/ble_data.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/src/ble/helpers.py` & `mgtron-2.17.0/src/ble/helpers.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/src/gui/db/init_db.sql` & `mgtron-2.17.0/src/gui/db/init_db.sql`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/src/gui/db/long_save.json` & `mgtron-2.17.0/src/gui/db/long_save.json`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/src/gui/db/mgtron_db.db` & `mgtron-2.17.0/src/gui/db/mgtron_db.db`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/src/gui/db/models.py` & `mgtron-2.17.0/src/gui/db/models.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/src/gui/db/quick_save.json` & `mgtron-2.17.0/src/gui/db/quick_save.json`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/src/gui/fonts/MesloLGS NF Bold Italic.ttf` & `mgtron-2.17.0/src/gui/fonts/MesloLGS NF Bold Italic.ttf`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/src/gui/fonts/MesloLGS NF Italic.ttf` & `mgtron-2.17.0/src/gui/fonts/MesloLGS NF Italic.ttf`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/src/gui/fonts/MesloLGS NF Regular.ttf` & `mgtron-2.17.0/src/gui/fonts/MesloLGS NF Regular.ttf`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/src/gui/helpers.py` & `mgtron-2.17.0/src/gui/helpers.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/src/gui/interface.py` & `mgtron-2.17.0/src/gui/interface.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/src/main.py` & `mgtron-2.17.0/src/main.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/src/mgtron.egg-info/PKG-INFO` & `mgtron-2.17.0/mgtron.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mgtron
-Version: 2.16.1
+Version: 2.17.0
 Summary: Package for MGTron GUI, a user interface for signal generation
 Author-email: Christerpher Hunter <chunter@cellantenna.com>
 Project-URL: Source, https://github.com/cellantenna/mg_tron
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
```

### Comparing `mgtron-2.16.1/src/mgtron.egg-info/SOURCES.txt` & `mgtron-2.17.0/mgtron.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -5,14 +5,20 @@
 pyproject.toml
 requirements.txt
 .github/ISSUE_TEMPLATE/mgtron--.md
 .github/ISSUE_TEMPLATE/mgtron_issue.yml
 .github/workflows/black_actions.yml
 docs/MGTron Command Description.docx
 docs/MGTron Function Descriptions.docx
+mgtron.egg-info/PKG-INFO
+mgtron.egg-info/SOURCES.txt
+mgtron.egg-info/dependency_links.txt
+mgtron.egg-info/entry_points.txt
+mgtron.egg-info/requires.txt
+mgtron.egg-info/top_level.txt
 src/__init__.py
 src/main.py
 src/assets/CA logo without subtext.JPG
 src/assets/CA_subheading.png
 src/assets/CHANGELOG.cpy
 src/assets/blueio_rs
 src/assets/init_cellantenna.sh
@@ -55,17 +61,23 @@
 src/gui/db/long_save.json.lock
 src/gui/db/mgtron_db.db
 src/gui/db/models.py
 src/gui/db/quick_save.json
 src/gui/fonts/MesloLGS NF Bold Italic.ttf
 src/gui/fonts/MesloLGS NF Italic.ttf
 src/gui/fonts/MesloLGS NF Regular.ttf
-src/mgtron.egg-info/PKG-INFO
-src/mgtron.egg-info/SOURCES.txt
-src/mgtron.egg-info/dependency_links.txt
-src/mgtron.egg-info/entry_points.txt
-src/mgtron.egg-info/requires.txt
-src/mgtron.egg-info/top_level.txt
 src/tests/__init__.py
 src/tests/test_ble.py
 src/tests/test_configfiles.py
-src/tests/test_helpers.py
+src/tests/test_helpers.py
+venv/bin/rst2html.py
+venv/bin/rst2html4.py
+venv/bin/rst2html5.py
+venv/bin/rst2latex.py
+venv/bin/rst2man.py
+venv/bin/rst2odt.py
+venv/bin/rst2odt_prepstyles.py
+venv/bin/rst2pseudoxml.py
+venv/bin/rst2s5.py
+venv/bin/rst2xetex.py
+venv/bin/rst2xml.py
+venv/bin/rstpep2html.py
```

### Comparing `mgtron-2.16.1/src/mgtron.egg-info/requires.txt` & `mgtron-2.17.0/mgtron.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/src/tests/test_configfiles.py` & `mgtron-2.17.0/src/tests/test_configfiles.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.16.1/src/tests/test_helpers.py` & `mgtron-2.17.0/src/tests/test_helpers.py`

 * *Files identical despite different names*

