# Comparing `tmp/xklb-2.1.4.tar.gz` & `tmp/xklb-2.1.5.tar.gz`

## Comparing `xklb-2.1.4.tar` & `xklb-2.1.5.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-2.1.4/.gitattributes
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 xklb-2.1.4/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-2.1.4/Windows.md
--rw-r--r--   0        0        0   490396 2020-02-02 00:00:00.000000 xklb-2.1.4/pdm.lock
--rw-r--r--   0        0        0    13086 2020-02-02 00:00:00.000000 xklb-2.1.4/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.1.4/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-2.1.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-2.1.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.1.4/.github/workflows/green.yaml
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 xklb-2.1.4/.github/workflows/push.yaml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/__init__.py
--rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/av.py
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/books.py
--rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/consts.py
--rw-r--r--   0        0        0     8337 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/db.py
--rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/dl_config.py
--rw-r--r--   0        0        0    11943 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/dl_extract.py
--rw-r--r--   0        0        0    13784 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/fs_extract.py
--rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/gdl_backend.py
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/gdl_extract.py
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/gui.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/history.py
--rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/hn_extract.py
--rw-r--r--   0        0        0    12072 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/lb.py
--rw-r--r--   0        0        0     7483 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/media.py
--rw-r--r--   0        0        0    25300 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/play_actions.py
--rw-r--r--   0        0        0    34425 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/player.py
--rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/playlists.py
--rw-r--r--   0        0        0    13549 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/praw_extract.py
--rw-r--r--   0        0        0     7979 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/search.py
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/subtitle.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/tabs_actions.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/tabs_extract.py
--rw-r--r--   0        0        0    15676 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/tube_backend.py
--rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/tube_extract.py
--rw-r--r--   0        0        0    83310 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/usage.py
--rw-r--r--   0        0        0    40986 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/scripts/block.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/scripts/christen.py
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/scripts/dedupe_db.py
--rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/scripts/download_status.py
--rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/scripts/history.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/scripts/playback_control.py
--rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/scripts/playlists.py
--rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/scripts/mining/mpv_watchlater.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.1.4/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 xklb-2.1.4/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.1.4/LICENSE
--rw-r--r--   0        0        0    84858 2020-02-02 00:00:00.000000 xklb-2.1.4/README.md
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 xklb-2.1.4/pyproject.toml
--rw-r--r--   0        0        0    88484 2020-02-02 00:00:00.000000 xklb-2.1.4/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-2.1.5/.gitattributes
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 xklb-2.1.5/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-2.1.5/Windows.md
+-rw-r--r--   0        0        0   490396 2020-02-02 00:00:00.000000 xklb-2.1.5/pdm.lock
+-rw-r--r--   0        0        0    13120 2020-02-02 00:00:00.000000 xklb-2.1.5/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.1.5/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-2.1.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-2.1.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.1.5/.github/workflows/green.yaml
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 xklb-2.1.5/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/__init__.py
+-rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/av.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/books.py
+-rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/consts.py
+-rw-r--r--   0        0        0     8335 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/db.py
+-rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/dl_config.py
+-rw-r--r--   0        0        0    11943 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/dl_extract.py
+-rw-r--r--   0        0        0    13784 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/fs_extract.py
+-rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/gdl_backend.py
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/gdl_extract.py
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/gui.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/history.py
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/hn_extract.py
+-rw-r--r--   0        0        0    12072 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/lb.py
+-rw-r--r--   0        0        0     7483 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/media.py
+-rw-r--r--   0        0        0    25300 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/play_actions.py
+-rw-r--r--   0        0        0    34425 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/player.py
+-rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/playlists.py
+-rw-r--r--   0        0        0    13549 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/praw_extract.py
+-rw-r--r--   0        0        0     7979 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/search.py
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/subtitle.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    15676 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/tube_backend.py
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/tube_extract.py
+-rw-r--r--   0        0        0    83240 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/usage.py
+-rw-r--r--   0        0        0    40973 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/block.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/dedupe_db.py
+-rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/download_status.py
+-rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/history.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/playback_control.py
+-rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/playlists.py
+-rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/mining/mpv_watchlater.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-2.1.5/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.1.5/LICENSE
+-rw-r--r--   0        0        0    94004 2020-02-02 00:00:00.000000 xklb-2.1.5/README.md
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 xklb-2.1.5/pyproject.toml
+-rw-r--r--   0        0        0    97630 2020-02-02 00:00:00.000000 xklb-2.1.5/PKG-INFO
```

### Comparing `xklb-2.1.4/TODO` & `xklb-2.1.5/TODO`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/Windows.md` & `xklb-2.1.5/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/pdm.lock` & `xklb-2.1.5/pdm.lock`

 * *Files 0% similar despite different names*

```diff
@@ -595,15 +595,15 @@
 name = "pathspec"
 version = "0.11.1"
 requires_python = ">=3.7"
 summary = "Utility library for gitignore style pattern matching of file paths."
 
 [[package]]
 name = "pathy"
-version = "0.10.1"
+version = "0.10.2"
 requires_python = ">= 3.6"
 summary = "pathlib.Path subclasses for local and cloud bucket storage"
 dependencies = [
     "smart-open<7.0.0,>=5.2.1",
     "typer<1.0.0,>=0.3.0",
 ]
 
@@ -910,15 +910,15 @@
 dependencies = [
     "Cython; sys_platform == \"darwin\"",
     "pyobjc-framework-Cocoa; sys_platform == \"darwin\"",
 ]
 
 [[package]]
 name = "setuptools"
-version = "67.8.0"
+version = "68.0.0"
 requires_python = ">=3.7"
 summary = "Easily download, build, install, upgrade, and uninstall Python packages"
 
 [[package]]
 name = "six"
 version = "1.12.0"
 requires_python = ">=2.6, !=3.0.*, !=3.1.*"
@@ -2431,17 +2431,17 @@
     {url = "https://files.pythonhosted.org/packages/05/63/8011bd08a4111858f79d2b09aad86638490d62fbf881c44e434a6dfca87b/parso-0.8.3-py2.py3-none-any.whl", hash = "sha256:c001d4636cd3aecdaf33cbb40aebb59b094be2a74c556778ef5576c175e19e75"},
     {url = "https://files.pythonhosted.org/packages/a2/0e/41f0cca4b85a6ea74d66d2226a7cda8e41206a624f5b330b958ef48e2e52/parso-0.8.3.tar.gz", hash = "sha256:8c07be290bb59f03588915921e29e8a50002acaf2cdc5fa0e0114f91709fafa0"},
 ]
 "pathspec 0.11.1" = [
     {url = "https://files.pythonhosted.org/packages/95/60/d93628975242cc515ab2b8f5b2fc831d8be2eff32f5a1be4776d49305d13/pathspec-0.11.1.tar.gz", hash = "sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687"},
     {url = "https://files.pythonhosted.org/packages/be/c8/551a803a6ebb174ec1c124e68b449b98a0961f0b737def601e3c1fbb4cfd/pathspec-0.11.1-py3-none-any.whl", hash = "sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293"},
 ]
-"pathy 0.10.1" = [
-    {url = "https://files.pythonhosted.org/packages/82/c6/683e3955de9a13b14dfa3ea358cd58f3914057e8064a2dcbfd450958e72e/pathy-0.10.1-py3-none-any.whl", hash = "sha256:a7613ee2d99a0a3300e1d836322e2d947c85449fde59f52906f995dbff67dad4"},
-    {url = "https://files.pythonhosted.org/packages/e9/fe/9fdf2ced8f3a4c25f3aac5141aad474b7701d288651472c9154a50b5a571/pathy-0.10.1.tar.gz", hash = "sha256:4cd6e71b4cd5ff875cfbb949ad9fa5519d8d1dbe69d5fc1d1b23aa3cb049618b"},
+"pathy 0.10.2" = [
+    {url = "https://files.pythonhosted.org/packages/b5/c3/04a002ace658133f5ac48d30258ed9ceab720595dc1ac36df02fe52018af/pathy-0.10.2-py3-none-any.whl", hash = "sha256:681bc98dbff28e7de3e50efa8246910f727e8ac254c4318c47ce341f7c1ce21d"},
+    {url = "https://files.pythonhosted.org/packages/be/c2/3c0b7d320c53d3ff213fe8e6cca5cf43da011be1b8c1bc9e8aba97d72161/pathy-0.10.2.tar.gz", hash = "sha256:79c572ab7fed84dc46837346edae58565992d0477a789cd4691a41d8eab9917d"},
 ]
 "pbr 5.11.1" = [
     {url = "https://files.pythonhosted.org/packages/01/06/4ab11bf70db5a60689fc521b636849c8593eb67a2c6bdf73a16c72d16a12/pbr-5.11.1-py2.py3-none-any.whl", hash = "sha256:567f09558bae2b3ab53cb3c1e2e33e726ff3338e7bae3db5dc954b3a44eef12b"},
     {url = "https://files.pythonhosted.org/packages/02/d8/acee75603f31e27c51134a858e0dea28d321770c5eedb9d1d673eb7d3817/pbr-5.11.1.tar.gz", hash = "sha256:aefc51675b0b533d56bb5fd1c8c6c0522fe31896679882e1c4c63d5e4a0fccb3"},
 ]
 "pdfminer-six 20191110" = [
     {url = "https://files.pythonhosted.org/packages/cb/83/200b2723bcbf1d1248a8a7d16e6dd6cb970b5331397b11948428d7ebcf37/pdfminer.six-20191110-py2.py3-none-any.whl", hash = "sha256:ca2ca58f3ac66a486bce53a6ddba95dc2b27781612915fa41c444790ba9cd2a8"},
@@ -2940,17 +2940,17 @@
     {url = "https://files.pythonhosted.org/packages/f1/95/dae88019fcff89cc1cc3b6fc85b9fc3a25a264b21b67000a665dd3ae372a/scalene-1.5.19-cp310-cp310-win_amd64.whl", hash = "sha256:cdb9be734cfb6b42eef1105fee1876a5c465eb72e109c0d0ceea6e6bdbce21c6"},
     {url = "https://files.pythonhosted.org/packages/fb/08/ed0d55f81bc2bc261c922a2d4171360b1a3a5d6a4e57ccc640fb09a02706/scalene-1.5.19-cp39-cp39-manylinux_2_24_x86_64.whl", hash = "sha256:d8bc53334b13e486ed6ba03fe4b7595ad4038d05537793eed9999952ba1b34c6"},
 ]
 "screeninfo 0.8.1" = [
     {url = "https://files.pythonhosted.org/packages/6e/bf/c5205d480307bef660e56544b9e3d7ff687da776abb30c9cb3f330887570/screeninfo-0.8.1-py3-none-any.whl", hash = "sha256:e97d6b173856edcfa3bd282f81deb528188aff14b11ec3e195584e7641be733c"},
     {url = "https://files.pythonhosted.org/packages/ec/bb/e69e5e628d43f118e0af4fc063c20058faa8635c95a1296764acc8167e27/screeninfo-0.8.1.tar.gz", hash = "sha256:9983076bcc7e34402a1a9e4d7dabf3729411fd2abb3f3b4be7eba73519cd2ed1"},
 ]
-"setuptools 67.8.0" = [
-    {url = "https://files.pythonhosted.org/packages/03/20/630783571e76e5fa5f3e9f29398ca3ace377207b8196b54e0ffdf09f12c1/setuptools-67.8.0.tar.gz", hash = "sha256:62642358adc77ffa87233bc4d2354c4b2682d214048f500964dbe760ccedf102"},
-    {url = "https://files.pythonhosted.org/packages/f5/2c/074ab1c5be9c7d523d8d6d69d1f46f450fe7f11713147dc9e779aa4ca4ea/setuptools-67.8.0-py3-none-any.whl", hash = "sha256:5df61bf30bb10c6f756eb19e7c9f3b473051f48db77fddbe06ff2ca307df9a6f"},
+"setuptools 68.0.0" = [
+    {url = "https://files.pythonhosted.org/packages/c7/42/be1c7bbdd83e1bfb160c94b9cafd8e25efc7400346cf7ccdbdb452c467fa/setuptools-68.0.0-py3-none-any.whl", hash = "sha256:11e52c67415a381d10d6b462ced9cfb97066179f0e871399e006c4ab101fc85f"},
+    {url = "https://files.pythonhosted.org/packages/dc/98/5f896af066c128669229ff1aa81553ac14cfb3e5e74b6b44594132b8540e/setuptools-68.0.0.tar.gz", hash = "sha256:baf1fdb41c6da4cd2eae722e135500da913332ab3f2f5c7d33af9b492acb5235"},
 ]
 "six 1.12.0" = [
     {url = "https://files.pythonhosted.org/packages/73/fb/00a976f728d0d1fecfe898238ce23f502a721c0ac0ecfedb80e0d88c64e9/six-1.12.0-py2.py3-none-any.whl", hash = "sha256:3350809f0555b11f552448330d0b52d5f24c91a322ea4a15ef22629740f3761c"},
     {url = "https://files.pythonhosted.org/packages/dd/bf/4138e7bfb757de47d1f4b6994648ec67a51efe58fa907c1e11e350cddfca/six-1.12.0.tar.gz", hash = "sha256:d16a0141ec1a18405cd4ce8b4613101da75da0e9a7aec5bdd4fa804d0e0eba73"},
 ]
 "sklearn 0.0.post5" = [
     {url = "https://files.pythonhosted.org/packages/7a/93/e0e1b1e98f39dfca7ec9795cb46f6e09e88a2fd5d4a28e4b3d1f618a2aec/sklearn-0.0.post5.tar.gz", hash = "sha256:7377c714a03a79bbe9196f435db931fd2a6fa8c68514da7ed3a251fd08c52e2c"},
```

### Comparing `xklb-2.1.4/readme.py` & `xklb-2.1.5/readme.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,29 @@
     ("Download Status", "download-status"),
     ("Update local media", "fsupdate"),
     ("Update online media", "tubeupdate"),
     ("Update reddit media", "redditupdate"),
     ("Convert pushshift data to reddit.db format", "pushshift"),
     ("List playlists", "playlists"),
     ("Blocklist a channel", "block"),
-    ("Show large folders", "bigdirs"),
-    ("Copy play history", "copy-play-counts"),
-    ("Dedupe music", "dedupe"),
     ("Re-optimize database", "optimize"),
     ("Re-download media", "redownload"),
     ("Merge online and local data", "merge-online-local"),
     ("Convert selftext links to media table", "reddit-selftext"),
     ("Merge SQLITE databases", "merge-dbs"),
     ("Dedupe SQLITE tables", "dedupe-db"),
-    ("Sort lines of text by similarity", "cluster-sort"),
+    ("Show large folders", "bigdirs"),
+    ("Copy play history", "copy-play-counts"),
+    ("Import mpv watchlater files", "mpv-watchlater"),
+    ("Sort data by similarity", "cluster-sort"),
+    ("Scatter files between folders or disks", "scatter"),
     ("Move files preserving parent folder hierarchy", "relmv"),
-    ("Automatic tab loader", "surf"),
     ("Clean filenames", "christen"),
-    # scatter usage is already in readme so intentionally skipped here
+    ("Dedupe music", "dedupe"),
+    ("Automatic tab loader", "surf"),
 ]:
     if subcommand not in title.lower():
         title += f" ({subcommand})"
     usage_details.append(
         f"""
 <details><summary>{title}</summary>
```

### Comparing `xklb-2.1.4/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-2.1.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-2.1.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/.github/workflows/push.yaml` & `xklb-2.1.5/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/av.py` & `xklb-2.1.5/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/books.py` & `xklb-2.1.5/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/consts.py` & `xklb-2.1.5/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/db.py` & `xklb-2.1.5/xklb/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,23 +73,23 @@
         return args.db[table_name].columns_dict
     except Exception:
         return {}
 
 
 config = {
     "playlists": {
-        "column_order": ["path", "extractor_key"],
-        "ignore_columns": ["id", "extractor_playlist_id"],
+        "column_order": ["id", "path", "extractor_key"],
+        "ignore_columns": ["extractor_playlist_id"],
     },
     "media": {
         "search_columns": ["path", "title", "mood", "genre", "description", "artist", "album"],
-        "column_order": ["path", "webpath", "extractor_id"],
-        "ignore_columns": ["id", "extractor_id"],
+        "column_order": ["id", "path", "webpath", "extractor_id"],
+        "ignore_columns": ["extractor_id"],
     },
-    "history": {"ignore_columns": ["id"]},
+    "history": {"column_order": ["id"]},
     "captions": {"search_columns": ["text"]},
     "reddit_posts": {
         "search_columns": ["title", "selftext"],
         "column_order": ["path"],
     },
     "reddit_comments": {
         "search_columns": ["body"],
```

### Comparing `xklb-2.1.4/xklb/dl_config.py` & `xklb-2.1.5/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/dl_extract.py` & `xklb-2.1.5/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/fs_extract.py` & `xklb-2.1.5/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/gdl_backend.py` & `xklb-2.1.5/xklb/gdl_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/gdl_extract.py` & `xklb-2.1.5/xklb/gdl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/gui.py` & `xklb-2.1.5/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/history.py` & `xklb-2.1.5/xklb/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/hn_extract.py` & `xklb-2.1.5/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/lb.py` & `xklb-2.1.5/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/media.py` & `xklb-2.1.5/xklb/media.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/play_actions.py` & `xklb-2.1.5/xklb/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/player.py` & `xklb-2.1.5/xklb/player.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/playlists.py` & `xklb-2.1.5/xklb/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/praw_extract.py` & `xklb-2.1.5/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/search.py` & `xklb-2.1.5/xklb/search.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/subtitle.py` & `xklb-2.1.5/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/tabs_actions.py` & `xklb-2.1.5/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/tabs_extract.py` & `xklb-2.1.5/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/tube_backend.py` & `xklb-2.1.5/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/tube_extract.py` & `xklb-2.1.5/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/usage.py` & `xklb-2.1.5/xklb/usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -810,18 +810,16 @@
     broccoli
     yellow
     green
     orange apple
     red apple' | library cluster-sort --print-groups
 
     [
-        {'common_prefix': '',
-        'grouped_paths': ['orange apple\n', 'red apple\n', 'red apple\n']},
-        {'common_prefix': '',
-        'grouped_paths': ['broccoli\n', 'green\n', 'yellow\n']}
+        {'grouped_paths': ['orange apple', 'red apple', 'red apple']},
+        {'grouped_paths': ['broccoli', 'green', 'yellow']}
     ]
 
     Auto-sort images into directories
 
     $ echo 'image1.jpg
     image2.jpg
     image3.jpg' | library cluster-sort --image --move-groups
```

### Comparing `xklb-2.1.4/xklb/utils.py` & `xklb-2.1.5/xklb/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from ast import literal_eval
 from collections import Counter
 from collections.abc import Iterable
 from copy import deepcopy
 from datetime import datetime, timedelta, timezone
 from functools import wraps
 from pathlib import Path
-from random import shuffle
 from shutil import which
 from timeit import default_timer
 from typing import Any, Dict, Generator, List, NoReturn, Optional, Union
 
 import humanize
 from IPython.core import ultratb
 from IPython.terminal.debugger import TerminalPdb
@@ -809,21 +808,21 @@
     def create_completer(list_):
         def list_completer(_text, state):
             line = readline.get_line_buffer()
 
             if not line:
                 min_depth = min([s.count(os.sep) for s in list_]) + 1
                 result_list = [c + " " for c in list_ if c.count(os.sep) <= min_depth]
-                shuffle(result_list)
+                random.shuffle(result_list)
                 return result_list[:25][state]
             else:
                 match_list = [s for s in list_ if s.startswith(line)]
                 min_depth = min([s.count(os.sep) for s in match_list]) + 1
                 result_list = [c + " " for c in match_list if c.count(os.sep) <= min_depth]
-                shuffle(result_list)
+                random.shuffle(result_list)
                 return result_list[:15][state]
 
         return list_completer
 
     readline.set_completer(create_completer(list_))
     readline.set_completer_delims("\t")
     readline.parse_and_bind("tab: complete")
```

### Comparing `xklb-2.1.4/xklb/scripts/bigdirs.py` & `xklb-2.1.5/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/scripts/block.py` & `xklb-2.1.5/xklb/scripts/block.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/scripts/christen.py` & `xklb-2.1.5/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/scripts/cluster_sort.py` & `xklb-2.1.5/xklb/scripts/cluster_sort.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse, sys
 from pathlib import Path
 from pprint import pprint
 
-from xklb import usage, utils
+from xklb import consts, usage, utils
 from xklb.consts import DBType
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library cluster-sort", usage=usage.cluster_sort)
 
@@ -76,20 +76,41 @@
     elif args.profile == "image":
         groups = utils.cluster_images(lines, args.clusters)
     else:
         raise NotImplementedError
     groups = sorted(groups, key=lambda d: (len(d["grouped_paths"]), -len(d["common_prefix"])))
 
     if args.print_groups:
+        for group in groups:
+            group["grouped_paths"] = [s.rstrip("\n") for s in group["grouped_paths"]]
+
         pprint(groups)
     elif args.move_groups:
         min_len = len(str(len(groups) + 1))
-        for i, group in enumerate(groups, start=1):
-            paths = [s.rstrip("\n") for s in group["grouped_paths"]]
-            utils.move_files([(p, str(Path(p).parent / str(i).zfill(min_len) / Path(p).name)) for p in paths])
+
+        if args.profile == "lines":
+            if args.output_path:
+                output_parent = Path(args.output_path).parent
+                output_name = Path(args.output_path).name
+            elif args.input_path.name == "<stdin>" or Path(args.input_path.name).parent == consts.TEMP_DIR:
+                output_parent = Path.cwd()
+                output_name = "stdin"
+            else:
+                output_parent = Path(args.input_path.name).parent
+                output_name = Path(args.input_path.name).name
+
+            for i, group in enumerate(groups, start=1):
+                output_path = output_parent / (output_name + "_" + str(i).zfill(min_len))
+                with open(output_path, "w") as output_fd:
+                    output_fd.writelines(group["grouped_paths"])
+
+        elif args.profile in ("image",):
+            for i, group in enumerate(groups, start=1):
+                paths = [s.rstrip("\n") for s in group["grouped_paths"]]
+                utils.move_files([(p, str(Path(p).parent / str(i).zfill(min_len) / Path(p).name)) for p in paths])
     else:
         lines = utils.flatten(d["grouped_paths"] for d in groups)
         if args.output_path:
             with open(args.output_path, "w") as output_fd:
                 output_fd.writelines(lines)
         else:
             utils.pipe_lines(lines)
```

### Comparing `xklb-2.1.4/xklb/scripts/copy_play_counts.py` & `xklb-2.1.5/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/scripts/dedupe.py` & `xklb-2.1.5/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/scripts/dedupe_db.py` & `xklb-2.1.5/xklb/scripts/dedupe_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/scripts/download_status.py` & `xklb-2.1.5/xklb/scripts/download_status.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/scripts/history.py` & `xklb-2.1.5/xklb/scripts/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/scripts/merge_dbs.py` & `xklb-2.1.5/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/scripts/merge_online_local.py` & `xklb-2.1.5/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/scripts/move_list.py` & `xklb-2.1.5/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/scripts/optimize_db.py` & `xklb-2.1.5/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/scripts/playback_control.py` & `xklb-2.1.5/xklb/scripts/playback_control.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/scripts/playlists.py` & `xklb-2.1.5/xklb/scripts/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/scripts/redownload.py` & `xklb-2.1.5/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/scripts/relmv.py` & `xklb-2.1.5/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/scripts/scatter.py` & `xklb-2.1.5/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/scripts/streaming_tab_loader.py` & `xklb-2.1.5/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/scripts/mining/data.py` & `xklb-2.1.5/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/scripts/mining/extract_links.py` & `xklb-2.1.5/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/scripts/mining/mpv_watchlater.py` & `xklb-2.1.5/xklb/scripts/mining/mpv_watchlater.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/scripts/mining/nouns.py` & `xklb-2.1.5/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/scripts/mining/pushshift.py` & `xklb-2.1.5/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/scripts/mining/reddit_selftext.py` & `xklb-2.1.5/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/xklb/assets/kotobago.png` & `xklb-2.1.5/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/.gitignore` & `xklb-2.1.5/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-/image_cluster_indexes/
 /.ruff_cache/
 /__pypackages__/
 /.pdm-python
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
```

### Comparing `xklb-2.1.4/LICENSE` & `xklb-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/README.md` & `xklb-2.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.1.004)
+    xk media library subcommands (v2.1.005)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
@@ -1228,50 +1228,14 @@
         library block dl.db "%fastcompany.com%"
         library block dl.db --match-column title "% bitcoin%"
         library block dl.db --force --match-column uploader Zeducation
 
 
 </details>
 
-<details><summary>Show large folders (bigdirs)</summary>
-
-    $ library bigdirs -h
-    usage: library bigdirs DATABASE [--limit (4000)] [--depth (0)] [--sort-by deleted | played] [--size=+5MB]
-
-    See what folders take up space
-
-        library bigdirs video.db
-        library bigdirs audio.db
-        library bigdirs fs.db
-
-
-</details>
-
-<details><summary>Copy play history (copy-play-counts)</summary>
-
-    $ library copy-play-counts -h
-    usage: library copy-play-counts DEST_DB SOURCE_DB ... [--source-prefix x] [--target-prefix y]
-
-    Copy play count information between databases
-
-        library copy-play-counts audio.db phone.db --source-prefix /storage/6E7B-7DCE/d --target-prefix /mnt/d
-
-
-</details>
-
-<details><summary>Dedupe music</summary>
-
-    $ library dedupe -h
-    usage: library [--audio | --id | --title | --filesystem] [--only-soft-delete] [--limit LIMIT] DATABASE
-
-    Dedupe your files
-
-
-</details>
-
 <details><summary>Re-optimize database</summary>
 
     $ library optimize -h
     usage: library optimize DATABASE [--force]
 
     Optimize library databases
 
@@ -1390,15 +1354,51 @@
     If --primary-keys is not provided table metadata primary keys will be used
     If --only-columns is not provided all non-primary and non-business key columns will be upserted
     If your duplicate rows contain exactly the same data in all the columns you can run with --skip-upsert to save a lot of time
 
 
 </details>
 
-<details><summary>Sort lines of text by similarity (cluster-sort)</summary>
+<details><summary>Show large folders (bigdirs)</summary>
+
+    $ library bigdirs -h
+    usage: library bigdirs DATABASE [--limit (4000)] [--depth (0)] [--sort-by deleted | played] [--size=+5MB]
+
+    See what folders take up space
+
+        library bigdirs video.db
+        library bigdirs audio.db
+        library bigdirs fs.db
+
+
+</details>
+
+<details><summary>Copy play history (copy-play-counts)</summary>
+
+    $ library copy-play-counts -h
+    usage: library copy-play-counts DEST_DB SOURCE_DB ... [--source-prefix x] [--target-prefix y]
+
+    Copy play count information between databases
+
+        library copy-play-counts audio.db phone.db --source-prefix /storage/6E7B-7DCE/d --target-prefix /mnt/d
+
+
+</details>
+
+<details><summary>Import mpv watchlater files (mpv-watchlater)</summary>
+
+    $ library mpv-watchlater -h
+    usage: library mpv-watchlater DATABASE [--watch-later-directory ~/.config/mpv/watch_later/]
+
+    Extract timestamps from MPV to the history table
+
+
+</details>
+
+<details><summary>Sort data by similarity (cluster-sort)</summary>
 
     $ library cluster-sort -h
     usage: library cluster-sort [input_path | stdin] [output_path | stdout]
 
     Group lines of text into sorted output
 
     $ echo 'red apple
@@ -1421,35 +1421,100 @@
     broccoli
     yellow
     green
     orange apple
     red apple' | library cluster-sort --print-groups
 
     [
-        {'common_prefix': '',
-        'grouped_paths': ['orange apple
-', 'red apple
-', 'red apple
-']},
-        {'common_prefix': '',
-        'grouped_paths': ['broccoli
-', 'green
-', 'yellow
-']}
+        {'grouped_paths': ['orange apple', 'red apple', 'red apple']},
+        {'grouped_paths': ['broccoli', 'green', 'yellow']}
     ]
 
     Auto-sort images into directories
 
     $ echo 'image1.jpg
     image2.jpg
     image3.jpg' | library cluster-sort --image --move-groups
 
 
 </details>
 
+<details><summary>Scatter files between folders or disks</summary>
+
+    $ library scatter -h
+    usage: library scatter [--limit LIMIT] [--policy POLICY] [--sort SORT] --srcmounts SRCMOUNTS DATABASE RELATIVE_PATHS ...
+
+Balance files across filesystem folder trees or multiple devices (mostly useful for mergerfs)
+
+    Scatter filesystem folder trees (without mountpoints; limited functionality; good for balancing fs inodes)
+
+        $ library scatter scatter.db /test/{0,1,2,3,4,5,6,7,8,9}
+
+    Reduce number of files per folder (creates more folders)
+
+        $ library scatter scatter.db --max-files-per-folder 16000 /test/{0,1,2,3,4,5,6,7,8,9}
+
+    Multi-device re-bin: balance by size
+
+        $ library scatter -m /mnt/d1:/mnt/d2:/mnt/d3:/mnt/d4/:/mnt/d5:/mnt/d6:/mnt/d7 ~/lb/fs/scatter.db subfolder/of/mergerfs/mnt
+        Current path distribution:
+        ╒═════════╤══════════════╤══════════════╤═══════════════╤════════════════╤═════════════════╤════════════════╕
+        │ mount   │   file_count │ total_size   │ median_size   │ time_created   │ time_modified   │ time_scanned   │
+        ╞═════════╪══════════════╪══════════════╪═══════════════╪════════════════╪═════════════════╪════════════════╡
+        │ /mnt/d1 │        12793 │ 169.5 GB     │ 4.5 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d2 │        13226 │ 177.9 GB     │ 4.7 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d3 │            1 │ 717.6 kB     │ 717.6 kB      │ Jan 31         │ Jul 18 2022     │ yesterday      │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d4 │           82 │ 1.5 GB       │ 12.5 MB       │ Jan 31         │ Apr 22 2022     │ yesterday      │
+        ╘═════════╧══════════════╧══════════════╧═══════════════╧════════════════╧═════════════════╧════════════════╛
+
+        Simulated path distribution:
+        5845 files should be moved
+        20257 files should not be moved
+        ╒═════════╤══════════════╤══════════════╤═══════════════╤════════════════╤═════════════════╤════════════════╕
+        │ mount   │   file_count │ total_size   │ median_size   │ time_created   │ time_modified   │ time_scanned   │
+        ╞═════════╪══════════════╪══════════════╪═══════════════╪════════════════╪═════════════════╪════════════════╡
+        │ /mnt/d1 │         9989 │ 46.0 GB      │ 2.4 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d2 │        10185 │ 46.0 GB      │ 2.4 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d3 │         1186 │ 53.6 GB      │ 30.8 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d4 │         1216 │ 49.5 GB      │ 29.5 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d5 │         1146 │ 53.0 GB      │ 30.9 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d6 │         1198 │ 48.8 GB      │ 30.6 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d7 │         1182 │ 52.0 GB      │ 30.9 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
+        ╘═════════╧══════════════╧══════════════╧═══════════════╧════════════════╧═════════════════╧════════════════╛
+        ### Move 1182 files to /mnt/d7 with this command: ###
+        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpmr1628ij / /mnt/d7
+        ### Move 1198 files to /mnt/d6 with this command: ###
+        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmp9yd75f6j / /mnt/d6
+        ### Move 1146 files to /mnt/d5 with this command: ###
+        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpfrj141jj / /mnt/d5
+        ### Move 1185 files to /mnt/d3 with this command: ###
+        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpqh2euc8n / /mnt/d3
+        ### Move 1134 files to /mnt/d4 with this command: ###
+        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmphzb0gj92 / /mnt/d4
+
+    Multi-device re-bin: balance device inodes for specific subfolder
+
+        $ library scatter -m /mnt/d1:/mnt/d2 ~/lb/fs/scatter.db subfolder --group count --sort 'size desc'
+
+    Multi-device re-bin: only consider the most recent 100 files
+
+        $ library scatter -m /mnt/d1:/mnt/d2 -l 100 -s 'time_modified desc' ~/lb/fs/scatter.db /
+
+
+</details>
+
 <details><summary>Move files preserving parent folder hierarchy (relmv)</summary>
 
     $ library relmv -h
     usage: library relmv [--dry-run] SOURCE ... DEST
 
     Move files/folders without losing hierarchy metadata
 
@@ -1462,52 +1527,62 @@
         library relmv (
             library listen ~/lb/audio.db --local-media-only --where 'play_count=0' --random -L 600 -p f
         ) /mnt/d/80_Now_Listening/
 
 
 </details>
 
-<details><summary>Automatic tab loader (surf)</summary>
+<details><summary>Clean filenames (christen)</summary>
 
-    $ library surf -h
-    usage: library surf [--count COUNT] [--target-hosts TARGET_HOSTS] < stdin
+    $ library christen -h
+    usage: library christen DATABASE [--run]
 
-    Streaming tab loader: press ctrl+c to stop.
+    Rename files to be somewhat normalized
 
-    Open tabs from a line-delimited file:
+    Default mode is dry-run
 
-        cat tabs.txt | library surf -n 5
+        library christen fs.db
 
-    You will likely want to use this setting in `about:config`
+    To actually do stuff use the run flag
 
-        browser.tabs.loadDivertedInBackground = True
+        library christen audio.db --run
 
-    If you prefer GUI, check out https://unli.xyz/tabsender/
+    You can optionally replace all the spaces in your filenames with dots
+
+        library christen --dot-space video.db
 
 
 </details>
 
-<details><summary>Clean filenames (christen)</summary>
+<details><summary>Dedupe music</summary>
 
-    $ library christen -h
-    usage: library christen DATABASE [--run]
+    $ library dedupe -h
+    usage: library [--audio | --id | --title | --filesystem] [--only-soft-delete] [--limit LIMIT] DATABASE
 
-    Rename files to be somewhat normalized
+    Dedupe your files
 
-    Default mode is dry-run
 
-        library christen fs.db
+</details>
 
-    To actually do stuff use the run flag
+<details><summary>Automatic tab loader (surf)</summary>
 
-        library christen audio.db --run
+    $ library surf -h
+    usage: library surf [--count COUNT] [--target-hosts TARGET_HOSTS] < stdin
 
-    You can optionally replace all the spaces in your filenames with dots
+    Streaming tab loader: press ctrl+c to stop.
 
-        library christen --dot-space video.db
+    Open tabs from a line-delimited file:
+
+        cat tabs.txt | library surf -n 5
+
+    You will likely want to use this setting in `about:config`
+
+        browser.tabs.loadDivertedInBackground = True
+
+    If you prefer GUI, check out https://unli.xyz/tabsender/
 
 
 </details>
 
 
 You can expand all by running this in your browser console:
```

### Comparing `xklb-2.1.4/pyproject.toml` & `xklb-2.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-2.1.4/PKG-INFO` & `xklb-2.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 2.1.4
+Version: 2.1.5
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -224,15 +224,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.1.004)
+    xk media library subcommands (v2.1.005)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
@@ -1313,50 +1313,14 @@
         library block dl.db "%fastcompany.com%"
         library block dl.db --match-column title "% bitcoin%"
         library block dl.db --force --match-column uploader Zeducation
 
 
 </details>
 
-<details><summary>Show large folders (bigdirs)</summary>
-
-    $ library bigdirs -h
-    usage: library bigdirs DATABASE [--limit (4000)] [--depth (0)] [--sort-by deleted | played] [--size=+5MB]
-
-    See what folders take up space
-
-        library bigdirs video.db
-        library bigdirs audio.db
-        library bigdirs fs.db
-
-
-</details>
-
-<details><summary>Copy play history (copy-play-counts)</summary>
-
-    $ library copy-play-counts -h
-    usage: library copy-play-counts DEST_DB SOURCE_DB ... [--source-prefix x] [--target-prefix y]
-
-    Copy play count information between databases
-
-        library copy-play-counts audio.db phone.db --source-prefix /storage/6E7B-7DCE/d --target-prefix /mnt/d
-
-
-</details>
-
-<details><summary>Dedupe music</summary>
-
-    $ library dedupe -h
-    usage: library [--audio | --id | --title | --filesystem] [--only-soft-delete] [--limit LIMIT] DATABASE
-
-    Dedupe your files
-
-
-</details>
-
 <details><summary>Re-optimize database</summary>
 
     $ library optimize -h
     usage: library optimize DATABASE [--force]
 
     Optimize library databases
 
@@ -1475,15 +1439,51 @@
     If --primary-keys is not provided table metadata primary keys will be used
     If --only-columns is not provided all non-primary and non-business key columns will be upserted
     If your duplicate rows contain exactly the same data in all the columns you can run with --skip-upsert to save a lot of time
 
 
 </details>
 
-<details><summary>Sort lines of text by similarity (cluster-sort)</summary>
+<details><summary>Show large folders (bigdirs)</summary>
+
+    $ library bigdirs -h
+    usage: library bigdirs DATABASE [--limit (4000)] [--depth (0)] [--sort-by deleted | played] [--size=+5MB]
+
+    See what folders take up space
+
+        library bigdirs video.db
+        library bigdirs audio.db
+        library bigdirs fs.db
+
+
+</details>
+
+<details><summary>Copy play history (copy-play-counts)</summary>
+
+    $ library copy-play-counts -h
+    usage: library copy-play-counts DEST_DB SOURCE_DB ... [--source-prefix x] [--target-prefix y]
+
+    Copy play count information between databases
+
+        library copy-play-counts audio.db phone.db --source-prefix /storage/6E7B-7DCE/d --target-prefix /mnt/d
+
+
+</details>
+
+<details><summary>Import mpv watchlater files (mpv-watchlater)</summary>
+
+    $ library mpv-watchlater -h
+    usage: library mpv-watchlater DATABASE [--watch-later-directory ~/.config/mpv/watch_later/]
+
+    Extract timestamps from MPV to the history table
+
+
+</details>
+
+<details><summary>Sort data by similarity (cluster-sort)</summary>
 
     $ library cluster-sort -h
     usage: library cluster-sort [input_path | stdin] [output_path | stdout]
 
     Group lines of text into sorted output
 
     $ echo 'red apple
@@ -1506,35 +1506,100 @@
     broccoli
     yellow
     green
     orange apple
     red apple' | library cluster-sort --print-groups
 
     [
-        {'common_prefix': '',
-        'grouped_paths': ['orange apple
-', 'red apple
-', 'red apple
-']},
-        {'common_prefix': '',
-        'grouped_paths': ['broccoli
-', 'green
-', 'yellow
-']}
+        {'grouped_paths': ['orange apple', 'red apple', 'red apple']},
+        {'grouped_paths': ['broccoli', 'green', 'yellow']}
     ]
 
     Auto-sort images into directories
 
     $ echo 'image1.jpg
     image2.jpg
     image3.jpg' | library cluster-sort --image --move-groups
 
 
 </details>
 
+<details><summary>Scatter files between folders or disks</summary>
+
+    $ library scatter -h
+    usage: library scatter [--limit LIMIT] [--policy POLICY] [--sort SORT] --srcmounts SRCMOUNTS DATABASE RELATIVE_PATHS ...
+
+Balance files across filesystem folder trees or multiple devices (mostly useful for mergerfs)
+
+    Scatter filesystem folder trees (without mountpoints; limited functionality; good for balancing fs inodes)
+
+        $ library scatter scatter.db /test/{0,1,2,3,4,5,6,7,8,9}
+
+    Reduce number of files per folder (creates more folders)
+
+        $ library scatter scatter.db --max-files-per-folder 16000 /test/{0,1,2,3,4,5,6,7,8,9}
+
+    Multi-device re-bin: balance by size
+
+        $ library scatter -m /mnt/d1:/mnt/d2:/mnt/d3:/mnt/d4/:/mnt/d5:/mnt/d6:/mnt/d7 ~/lb/fs/scatter.db subfolder/of/mergerfs/mnt
+        Current path distribution:
+        ╒═════════╤══════════════╤══════════════╤═══════════════╤════════════════╤═════════════════╤════════════════╕
+        │ mount   │   file_count │ total_size   │ median_size   │ time_created   │ time_modified   │ time_scanned   │
+        ╞═════════╪══════════════╪══════════════╪═══════════════╪════════════════╪═════════════════╪════════════════╡
+        │ /mnt/d1 │        12793 │ 169.5 GB     │ 4.5 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d2 │        13226 │ 177.9 GB     │ 4.7 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d3 │            1 │ 717.6 kB     │ 717.6 kB      │ Jan 31         │ Jul 18 2022     │ yesterday      │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d4 │           82 │ 1.5 GB       │ 12.5 MB       │ Jan 31         │ Apr 22 2022     │ yesterday      │
+        ╘═════════╧══════════════╧══════════════╧═══════════════╧════════════════╧═════════════════╧════════════════╛
+
+        Simulated path distribution:
+        5845 files should be moved
+        20257 files should not be moved
+        ╒═════════╤══════════════╤══════════════╤═══════════════╤════════════════╤═════════════════╤════════════════╕
+        │ mount   │   file_count │ total_size   │ median_size   │ time_created   │ time_modified   │ time_scanned   │
+        ╞═════════╪══════════════╪══════════════╪═══════════════╪════════════════╪═════════════════╪════════════════╡
+        │ /mnt/d1 │         9989 │ 46.0 GB      │ 2.4 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d2 │        10185 │ 46.0 GB      │ 2.4 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d3 │         1186 │ 53.6 GB      │ 30.8 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d4 │         1216 │ 49.5 GB      │ 29.5 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d5 │         1146 │ 53.0 GB      │ 30.9 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d6 │         1198 │ 48.8 GB      │ 30.6 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
+        ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
+        │ /mnt/d7 │         1182 │ 52.0 GB      │ 30.9 MB       │ Jan 27         │ Apr 07 2022     │ Jan 31         │
+        ╘═════════╧══════════════╧══════════════╧═══════════════╧════════════════╧═════════════════╧════════════════╛
+        ### Move 1182 files to /mnt/d7 with this command: ###
+        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpmr1628ij / /mnt/d7
+        ### Move 1198 files to /mnt/d6 with this command: ###
+        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmp9yd75f6j / /mnt/d6
+        ### Move 1146 files to /mnt/d5 with this command: ###
+        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpfrj141jj / /mnt/d5
+        ### Move 1185 files to /mnt/d3 with this command: ###
+        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpqh2euc8n / /mnt/d3
+        ### Move 1134 files to /mnt/d4 with this command: ###
+        rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmphzb0gj92 / /mnt/d4
+
+    Multi-device re-bin: balance device inodes for specific subfolder
+
+        $ library scatter -m /mnt/d1:/mnt/d2 ~/lb/fs/scatter.db subfolder --group count --sort 'size desc'
+
+    Multi-device re-bin: only consider the most recent 100 files
+
+        $ library scatter -m /mnt/d1:/mnt/d2 -l 100 -s 'time_modified desc' ~/lb/fs/scatter.db /
+
+
+</details>
+
 <details><summary>Move files preserving parent folder hierarchy (relmv)</summary>
 
     $ library relmv -h
     usage: library relmv [--dry-run] SOURCE ... DEST
 
     Move files/folders without losing hierarchy metadata
 
@@ -1547,52 +1612,62 @@
         library relmv (
             library listen ~/lb/audio.db --local-media-only --where 'play_count=0' --random -L 600 -p f
         ) /mnt/d/80_Now_Listening/
 
 
 </details>
 
-<details><summary>Automatic tab loader (surf)</summary>
+<details><summary>Clean filenames (christen)</summary>
 
-    $ library surf -h
-    usage: library surf [--count COUNT] [--target-hosts TARGET_HOSTS] < stdin
+    $ library christen -h
+    usage: library christen DATABASE [--run]
 
-    Streaming tab loader: press ctrl+c to stop.
+    Rename files to be somewhat normalized
 
-    Open tabs from a line-delimited file:
+    Default mode is dry-run
 
-        cat tabs.txt | library surf -n 5
+        library christen fs.db
 
-    You will likely want to use this setting in `about:config`
+    To actually do stuff use the run flag
 
-        browser.tabs.loadDivertedInBackground = True
+        library christen audio.db --run
 
-    If you prefer GUI, check out https://unli.xyz/tabsender/
+    You can optionally replace all the spaces in your filenames with dots
+
+        library christen --dot-space video.db
 
 
 </details>
 
-<details><summary>Clean filenames (christen)</summary>
+<details><summary>Dedupe music</summary>
 
-    $ library christen -h
-    usage: library christen DATABASE [--run]
+    $ library dedupe -h
+    usage: library [--audio | --id | --title | --filesystem] [--only-soft-delete] [--limit LIMIT] DATABASE
 
-    Rename files to be somewhat normalized
+    Dedupe your files
 
-    Default mode is dry-run
 
-        library christen fs.db
+</details>
 
-    To actually do stuff use the run flag
+<details><summary>Automatic tab loader (surf)</summary>
 
-        library christen audio.db --run
+    $ library surf -h
+    usage: library surf [--count COUNT] [--target-hosts TARGET_HOSTS] < stdin
 
-    You can optionally replace all the spaces in your filenames with dots
+    Streaming tab loader: press ctrl+c to stop.
 
-        library christen --dot-space video.db
+    Open tabs from a line-delimited file:
+
+        cat tabs.txt | library surf -n 5
+
+    You will likely want to use this setting in `about:config`
+
+        browser.tabs.loadDivertedInBackground = True
+
+    If you prefer GUI, check out https://unli.xyz/tabsender/
 
 
 </details>
 
 
 You can expand all by running this in your browser console:
```

