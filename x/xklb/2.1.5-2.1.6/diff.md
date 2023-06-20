# Comparing `tmp/xklb-2.1.5.tar.gz` & `tmp/xklb-2.1.6.tar.gz`

## Comparing `xklb-2.1.5.tar` & `xklb-2.1.6.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-2.1.5/.gitattributes
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 xklb-2.1.5/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-2.1.5/Windows.md
--rw-r--r--   0        0        0   490396 2020-02-02 00:00:00.000000 xklb-2.1.5/pdm.lock
--rw-r--r--   0        0        0    13120 2020-02-02 00:00:00.000000 xklb-2.1.5/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.1.5/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-2.1.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-2.1.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.1.5/.github/workflows/green.yaml
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 xklb-2.1.5/.github/workflows/push.yaml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/__init__.py
--rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/av.py
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/books.py
--rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/consts.py
--rw-r--r--   0        0        0     8335 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/db.py
--rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/dl_config.py
--rw-r--r--   0        0        0    11943 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/dl_extract.py
--rw-r--r--   0        0        0    13784 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/fs_extract.py
--rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/gdl_backend.py
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/gdl_extract.py
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/gui.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/history.py
--rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/hn_extract.py
--rw-r--r--   0        0        0    12072 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/lb.py
--rw-r--r--   0        0        0     7483 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/media.py
--rw-r--r--   0        0        0    25300 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/play_actions.py
--rw-r--r--   0        0        0    34425 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/player.py
--rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/playlists.py
--rw-r--r--   0        0        0    13549 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/praw_extract.py
--rw-r--r--   0        0        0     7979 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/search.py
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/subtitle.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/tabs_actions.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/tabs_extract.py
--rw-r--r--   0        0        0    15676 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/tube_backend.py
--rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/tube_extract.py
--rw-r--r--   0        0        0    83240 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/usage.py
--rw-r--r--   0        0        0    40973 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/block.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/christen.py
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/dedupe_db.py
--rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/download_status.py
--rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/history.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/playback_control.py
--rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/playlists.py
--rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/mining/mpv_watchlater.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.1.5/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-2.1.5/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.1.5/LICENSE
--rw-r--r--   0        0        0    94004 2020-02-02 00:00:00.000000 xklb-2.1.5/README.md
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 xklb-2.1.5/pyproject.toml
--rw-r--r--   0        0        0    97630 2020-02-02 00:00:00.000000 xklb-2.1.5/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-2.1.6/.gitattributes
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 xklb-2.1.6/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-2.1.6/Windows.md
+-rw-r--r--   0        0        0   490396 2020-02-02 00:00:00.000000 xklb-2.1.6/pdm.lock
+-rw-r--r--   0        0        0    13120 2020-02-02 00:00:00.000000 xklb-2.1.6/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.1.6/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-2.1.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-2.1.6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.1.6/.github/workflows/green.yaml
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 xklb-2.1.6/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/__init__.py
+-rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/av.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/books.py
+-rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/consts.py
+-rw-r--r--   0        0        0     8335 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/db.py
+-rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/dl_config.py
+-rw-r--r--   0        0        0    11943 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/dl_extract.py
+-rw-r--r--   0        0        0    13784 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/fs_extract.py
+-rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/gdl_backend.py
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/gdl_extract.py
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/gui.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/history.py
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/hn_extract.py
+-rw-r--r--   0        0        0    12072 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/lb.py
+-rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/media.py
+-rw-r--r--   0        0        0    25386 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/play_actions.py
+-rw-r--r--   0        0        0    34451 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/player.py
+-rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/playlists.py
+-rw-r--r--   0        0        0    13549 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/praw_extract.py
+-rw-r--r--   0        0        0     7979 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/search.py
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/subtitle.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    15676 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/tube_backend.py
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/tube_extract.py
+-rw-r--r--   0        0        0    83349 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/usage.py
+-rw-r--r--   0        0        0    41240 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     7248 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/block.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/dedupe_db.py
+-rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/download_status.py
+-rw-r--r--   0        0        0     5849 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/history.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/playback_control.py
+-rw-r--r--   0        0        0     5659 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/playlists.py
+-rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/mining/mpv_watchlater.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.1.6/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-2.1.6/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.1.6/LICENSE
+-rw-r--r--   0        0        0    94113 2020-02-02 00:00:00.000000 xklb-2.1.6/README.md
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 xklb-2.1.6/pyproject.toml
+-rw-r--r--   0        0        0    97739 2020-02-02 00:00:00.000000 xklb-2.1.6/PKG-INFO
```

### Comparing `xklb-2.1.5/TODO` & `xklb-2.1.6/TODO`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/Windows.md` & `xklb-2.1.6/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/pdm.lock` & `xklb-2.1.6/pdm.lock`

 * *Files 0% similar despite different names*

```diff
@@ -539,15 +539,15 @@
 name = "mypy-extensions"
 version = "1.0.0"
 requires_python = ">=3.5"
 summary = "Type system extensions for programs checked with the mypy type checker."
 
 [[package]]
 name = "natsort"
-version = "8.3.1"
+version = "8.4.0"
 requires_python = ">=3.7"
 summary = "Simple yet flexible natural sorting in Python."
 
 [[package]]
 name = "numpy"
 version = "1.24.3"
 requires_python = ">=3.8"
@@ -2307,17 +2307,17 @@
     {url = "https://files.pythonhosted.org/packages/03/ee/114d7016d2e34f341e212fefb5e7bd87785077ebcfff0ad23a497c70eea1/mutagen-1.46.0-py3-none-any.whl", hash = "sha256:8af0728aa2d5c3ee5a727e28d0627966641fddfe804c23eabb5926a4d770aed5"},
     {url = "https://files.pythonhosted.org/packages/b1/54/d1760a363d0fe345528e37782f6c18123b0e99e8ea755022fd51f1ecd0f9/mutagen-1.46.0.tar.gz", hash = "sha256:6e5f8ba84836b99fe60be5fb27f84be4ad919bbb6b49caa6ae81e70584b55e58"},
 ]
 "mypy-extensions 1.0.0" = [
     {url = "https://files.pythonhosted.org/packages/2a/e2/5d3f6ada4297caebe1a2add3b126fe800c96f56dbe5d1988a2cbe0b267aa/mypy_extensions-1.0.0-py3-none-any.whl", hash = "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d"},
     {url = "https://files.pythonhosted.org/packages/98/a4/1ab47638b92648243faf97a5aeb6ea83059cc3624972ab6b8d2316078d3f/mypy_extensions-1.0.0.tar.gz", hash = "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"},
 ]
-"natsort 8.3.1" = [
-    {url = "https://files.pythonhosted.org/packages/47/2a/bf13bfc1a51b6df2f823909c6d4f674a256e3f29401825e1d56ca2a95dc9/natsort-8.3.1.tar.gz", hash = "sha256:517595492dde570a4fd6b6a76f644440c1ba51e2338c8a671d7f0475fda8f9fd"},
-    {url = "https://files.pythonhosted.org/packages/5f/e1/70d203ba3ae5476f25fb8a2015d6a7ff156a4ce4795e36955c144ea5a826/natsort-8.3.1-py3-none-any.whl", hash = "sha256:d583bc9050dd10538de36297c960b93f873f0cd01671a3c50df5bd86dd391dcb"},
+"natsort 8.4.0" = [
+    {url = "https://files.pythonhosted.org/packages/e2/a9/a0c57aee75f77794adaf35322f8b6404cbd0f89ad45c87197a937764b7d0/natsort-8.4.0.tar.gz", hash = "sha256:45312c4a0e5507593da193dedd04abb1469253b601ecaf63445ad80f0a1ea581"},
+    {url = "https://files.pythonhosted.org/packages/ef/82/7a9d0550484a62c6da82858ee9419f3dd1ccc9aa1c26a1e43da3ecd20b0d/natsort-8.4.0-py3-none-any.whl", hash = "sha256:4732914fb471f56b5cce04d7bae6f164a592c7712e1c85f9ef585e197299521c"},
 ]
 "numpy 1.24.3" = [
     {url = "https://files.pythonhosted.org/packages/0d/43/643629a4a278b4815541c7d69856c07ddb0e99bdc62b43538d3751eae2d8/numpy-1.24.3-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:4719d5aefb5189f50887773699eaf94e7d1e02bf36c1a9d353d9f46703758ca4"},
     {url = "https://files.pythonhosted.org/packages/15/b8/cbe1750b9ec78062e5a00ef39ff8bdf189ce753b411b6b35931ababaee47/numpy-1.24.3-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:35400e6a8d102fd07c71ed7dcadd9eb62ee9a6e84ec159bd48c28235bbb0f8e4"},
     {url = "https://files.pythonhosted.org/packages/1a/62/af7e78a12207608b23e3b2e248fc823fbef75f17d5defc8a127c5661daca/numpy-1.24.3-cp38-cp38-win_amd64.whl", hash = "sha256:56e48aec79ae238f6e4395886b5eaed058abb7231fb3361ddd7bfdf4eed54289"},
     {url = "https://files.pythonhosted.org/packages/2c/d4/590ae7df5044465cc9fa2db152ae12468694d62d952b1528ecff328ef7fc/numpy-1.24.3.tar.gz", hash = "sha256:ab344f1bf21f140adab8e47fdbc7c35a477dc01408791f8ba00d018dd0bc5155"},
     {url = "https://files.pythonhosted.org/packages/53/f7/bf6e2b973c6d6a4c60f722dd95322d4997b4999347d67c5c74a4042a07b7/numpy-1.24.3-cp38-cp38-win32.whl", hash = "sha256:d933fabd8f6a319e8530d0de4fcc2e6a61917e0b0c271fded460032db42a0fe4"},
```

### Comparing `xklb-2.1.5/readme.py` & `xklb-2.1.6/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-2.1.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-2.1.6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/.github/workflows/push.yaml` & `xklb-2.1.6/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/av.py` & `xklb-2.1.6/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/books.py` & `xklb-2.1.6/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/consts.py` & `xklb-2.1.6/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/db.py` & `xklb-2.1.6/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/dl_config.py` & `xklb-2.1.6/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/dl_extract.py` & `xklb-2.1.6/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/fs_extract.py` & `xklb-2.1.6/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/gdl_backend.py` & `xklb-2.1.6/xklb/gdl_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/gdl_extract.py` & `xklb-2.1.6/xklb/gdl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/gui.py` & `xklb-2.1.6/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/history.py` & `xklb-2.1.6/xklb/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/hn_extract.py` & `xklb-2.1.6/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/lb.py` & `xklb-2.1.6/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/media.py` & `xklb-2.1.6/xklb/media.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,20 @@
         log.info("Extra media data %s", v)
         # breakpoint()
 
     return utils.dict_filter_bool(cv)
 
 
 def _add(args, entry):
+    if "path" not in entry:
+        log.warning('Skipping insert: no "path" in entry %s', entry)
+        return
+
     tags = entry.pop("tags", None) or ""
+
     media_id = args.db.pop("select id from media where path = ?", [entry["path"]])
     if media_id:
         entry["id"] = media_id
 
         args.db["media"].upsert(utils.dict_filter_bool(entry), pk="id", alter=True)
     else:
         args.db["media"].insert(utils.dict_filter_bool(entry), pk="id", alter=True)
```

### Comparing `xklb-2.1.5/xklb/play_actions.py` & `xklb-2.1.6/xklb/play_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -503,15 +503,15 @@
             existing_playhead=m.get("playhead"),
             media_duration=m.get("duration"),
         )
         if playhead:
             history.add(args, [m["original_path"]], playhead=playhead)
 
 
-def play(args, m) -> None:
+def play(args, m, media_len) -> None:
     t = utils.Timer()
     print(m["now_playing"])
     log.debug("now_playing: %s", t.elapsed())
 
     args.player = player.parse(args, m)
     log.debug("player.parse: %s", t.elapsed())
 
@@ -521,26 +521,26 @@
 
     start_time = time.time()
     try:
         if args.chromecast:
             try:
                 chromecast_play(args, m)
                 t.reset()
-                player.post_act(args, m["original_path"])
+                player.post_act(args, m["original_path"], media_len=media_len)
                 log.debug("player.post_act: %s", t.elapsed())
             except Exception:
                 if args.ignore_errors:
                     return
                 else:
                     raise
         else:
             r = player.local_player(args, m)
             if r.returncode == 0:
                 t.reset()
-                player.post_act(args, m["original_path"])
+                player.post_act(args, m["original_path"], media_len=media_len)
                 log.debug("player.post_act: %s", t.elapsed())
             else:
                 log.warning("Player exited with code %s", r.returncode)
                 if args.ignore_errors:
                     return
                 else:
                     raise SystemExit(r.returncode)
@@ -606,15 +606,15 @@
         log.debug("big_dirs: %s", t.elapsed())
 
     if args.related >= consts.RELATED:
         media = player.get_related_media(args, media[0])
         log.debug("player.get_related_media: %s", t.elapsed())
 
     if args.cluster:
-        media = utils.cluster_dicts(media)
+        media = utils.cluster_dicts(args, media)
         log.debug("cluster: %s", t.elapsed())
 
     if args.print:
         if args.play_in_order >= consts.SIMILAR:
             media = [player.get_ordinal_media(args, d) for d in media]
         player.media_printer(args, media)
     elif args.multiple_playback:
@@ -636,15 +636,15 @@
                         ignore_paths.append(m["path"])
                         futures.append(future)
 
                     if futures:
                         future = futures.popleft()
                         m = future.result()
                         if m is not None and (m["path"].startswith("http") or Path(m["path"]).exists()):
-                            play(args, m)
+                            play(args, m, len(media) + len(futures))
         finally:
             if args.interdimensional_cable:
                 args.sock.send(b"raw quit \n")
             Path(args.mpv_socket).unlink(missing_ok=True)
             if args.chromecast:
                 Path(consts.CAST_NOW_PLAYING).unlink(missing_ok=True)
```

### Comparing `xklb-2.1.5/xklb/player.py` & `xklb-2.1.6/xklb/player.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,15 +275,15 @@
     ASK_KEEP = (Action.KEEP, Action.DELETE)
     ASK_MOVE = (Action.MOVE, Action.KEEP)
     ASK_DELETE = (Action.DELETE, Action.KEEP)
     ASK_SOFTDELETE = (Action.SOFTDELETE, Action.KEEP)
     ASK_MOVE_OR_DELETE = (Action.MOVE, Action.DELETE)
 
 
-def post_act(args, media_file: str, action: Optional[str] = None, geom_data=None, media=None) -> None:
+def post_act(args, media_file: str, action: Optional[str] = None, geom_data=None, media_len=0) -> None:
     history.add(args, [media_file], mark_done=True)
 
     def handle_delete_action():
         if media_file.startswith("http"):
             mark_media_deleted(args, media_file)
         else:
             delete_media(args, media_file)
@@ -296,22 +296,22 @@
             mv_to_keep_folder(args, media_file)
 
     def handle_ask_action(ask_action: str):
         true_action, false_action = getattr(AskAction, ask_action)
         if gui and args.gui:
             response = gui.askkeep(
                 media_file,
-                len(media or []),
+                media_len,
                 geom_data,
                 true_action=true_action,
                 false_action=false_action,
             )
         else:
             response = utils.confirm(true_action.title() + "?")
-        post_act(args, media_file, action=true_action if response else false_action)
+        post_act(args, media_file, action=true_action if response else false_action)  # answer the question
 
     action = action or args.post_action
     action = action.upper()
 
     if action == Action.KEEP:
         pass
     elif action == Action.DELETE:
@@ -787,15 +787,15 @@
                         r = utils.Pclose(m["process"])
                         if r.returncode != 0:
                             log.warning("Player exited with code %s", r.returncode)
                             log.debug(join(r.args))
                             if not args.ignore_errors:
                                 raise SystemExit(r.returncode)
 
-                        post_act(args, m["path"], geom_data=geom_data, media=media)
+                        post_act(args, m["path"], geom_data=geom_data, media_len=len(media))
 
                         if media:
                             players[t_idx] = _create_player(args, player_hole, media)
                         else:
                             del players[t_idx]
 
             log.debug("%s media", len(media))
```

### Comparing `xklb-2.1.5/xklb/playlists.py` & `xklb-2.1.6/xklb/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/praw_extract.py` & `xklb-2.1.6/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/search.py` & `xklb-2.1.6/xklb/search.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/subtitle.py` & `xklb-2.1.6/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/tabs_actions.py` & `xklb-2.1.6/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/tabs_extract.py` & `xklb-2.1.6/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/tube_backend.py` & `xklb-2.1.6/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/tube_extract.py` & `xklb-2.1.6/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/usage.py` & `xklb-2.1.6/xklb/usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -678,27 +678,27 @@
         ╘═══════════════════════════════════════╧═════════════╧══════════════╛
 """
 
 tabsadd = r"""library tabsadd [--frequency daily weekly (monthly) quarterly yearly] [--no-sanitize] DATABASE URLS ...
 
     Adding one URL:
 
-        library tabsadd -f monthly -c travel ~/lb/tabs.db https://old.reddit.com/r/Colombia/top/?sort=top&t=month
+        library tabsadd -f monthly -c travel tabs.db https://old.reddit.com/r/Colombia/top/?sort=top&t=month
 
         Depending on your shell you may need to escape the URL (add quotes)
 
         If you use Fish shell know that you can enable features to make pasting easier:
             set -U fish_features stderr-nocaret qmark-noglob regex-easyesc ampersand-nobg-in-token
 
         Also I recommend turning Ctrl+Backspace into a super-backspace for repeating similar commands with long args:
             echo 'bind \b backward-kill-bigword' >> ~/.config/fish/config.fish
 
     Importing from a line-delimitated file:
 
-        library tabsadd -f yearly -c reddit ~/lb/tabs.db (cat ~/mc/yearly-subreddit.cron)
+        library tabsadd -f yearly -c reddit tabs.db (cat ~/mc/yearly-subreddit.cron)
 
 """
 
 tubeadd = r"""library tubeadd [--safe] [--extra] [--subs] [--auto-subs] DATABASE URLS ...
 
     Create a dl database / add links to an existing database
 
@@ -763,14 +763,19 @@
 bigdirs = """library bigdirs DATABASE [--limit (4000)] [--depth (0)] [--sort-by deleted | played] [--size=+5MB]
 
     See what folders take up space
 
         library bigdirs video.db
         library bigdirs audio.db
         library bigdirs fs.db
+
+    lb bigdirs video.db --folder-size=+10G --lower 400 --upper 14000
+
+    lb bigdirs video.db --depth 5
+    lb bigdirs video.db --depth 7
 """
 
 christen = """library christen DATABASE [--run]
 
     Rename files to be somewhat normalized
 
     Default mode is dry-run
@@ -934,15 +939,15 @@
     Move fresh music to your phone every Sunday:
 
         # move last weeks' music back to their source folders
         library relmv /mnt/d/80_Now_Listening/ /mnt/d/
 
         # move new music for this week
         library relmv (
-            library listen ~/lb/audio.db --local-media-only --where 'play_count=0' --random -L 600 -p f
+            library listen audio.db --local-media-only --where 'play_count=0' --random -L 600 -p f
         ) /mnt/d/80_Now_Listening/
 """
 
 mv_list = """library mv-list [--limit LIMIT] [--lower LOWER] [--upper UPPER] MOUNT_POINT DATABASE
 
 Free up space on a specific disk. Find candidates for moving data to a different mount point
 
@@ -1014,15 +1019,15 @@
 
     Reduce number of files per folder (creates more folders)
 
         $ library scatter scatter.db --max-files-per-folder 16000 /test/{0,1,2,3,4,5,6,7,8,9}
 
     Multi-device re-bin: balance by size
 
-        $ library scatter -m /mnt/d1:/mnt/d2:/mnt/d3:/mnt/d4/:/mnt/d5:/mnt/d6:/mnt/d7 ~/lb/fs/scatter.db subfolder/of/mergerfs/mnt
+        $ library scatter -m /mnt/d1:/mnt/d2:/mnt/d3:/mnt/d4/:/mnt/d5:/mnt/d6:/mnt/d7 fs/scatter.db subfolder/of/mergerfs/mnt
         Current path distribution:
         ╒═════════╤══════════════╤══════════════╤═══════════════╤════════════════╤═════════════════╤════════════════╕
         │ mount   │   file_count │ total_size   │ median_size   │ time_created   │ time_modified   │ time_scanned   │
         ╞═════════╪══════════════╪══════════════╪═══════════════╪════════════════╪═════════════════╪════════════════╡
         │ /mnt/d1 │        12793 │ 169.5 GB     │ 4.5 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
         ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
         │ /mnt/d2 │        13226 │ 177.9 GB     │ 4.7 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
@@ -1061,19 +1066,19 @@
         ### Move 1185 files to /mnt/d3 with this command: ###
         rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpqh2euc8n / /mnt/d3
         ### Move 1134 files to /mnt/d4 with this command: ###
         rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmphzb0gj92 / /mnt/d4
 
     Multi-device re-bin: balance device inodes for specific subfolder
 
-        $ library scatter -m /mnt/d1:/mnt/d2 ~/lb/fs/scatter.db subfolder --group count --sort 'size desc'
+        $ library scatter -m /mnt/d1:/mnt/d2 fs/scatter.db subfolder --group count --sort 'size desc'
 
     Multi-device re-bin: only consider the most recent 100 files
 
-        $ library scatter -m /mnt/d1:/mnt/d2 -l 100 -s 'time_modified desc' ~/lb/fs/scatter.db /
+        $ library scatter -m /mnt/d1:/mnt/d2 -l 100 -s 'time_modified desc' fs/scatter.db /
 """
 surf = """library surf [--count COUNT] [--target-hosts TARGET_HOSTS] < stdin
 
     Streaming tab loader: press ctrl+c to stop.
 
     Open tabs from a line-delimited file:
```

### Comparing `xklb-2.1.5/xklb/utils.py` & `xklb-2.1.6/xklb/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1196,19 +1196,25 @@
         }
         result.append(metadata)
     log.info("common_prefix %s", t.elapsed())
 
     return result
 
 
-def cluster_dicts(media):
+def cluster_dicts(args, media):
     media_keyed = {d["path"]: d for d in media}
     groups = cluster_paths([d["path"] for d in media])
     groups = sorted(groups, key=lambda d: (-len(d["grouped_paths"]), -len(d["common_prefix"])))
-    sorted_paths = flatten(d["grouped_paths"] for d in groups)
+    if hasattr(args, "sort") and "duration" in args.sort:
+        sorted_paths = flatten(
+            sorted(d["grouped_paths"], key=lambda p: media_keyed[p]["duration"], reverse="duration desc" in args.sort)
+            for d in groups
+        )
+    else:
+        sorted_paths = flatten(d["grouped_paths"] for d in groups)
     media = [media_keyed[p] for p in sorted_paths]
     return media
 
 
 def is_timecode_like(text):
     for char in text:
         if not (char in ":,_-;. " or char.isdigit()):
```

### Comparing `xklb-2.1.5/xklb/scripts/bigdirs.py` & `xklb-2.1.6/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/scripts/block.py` & `xklb-2.1.6/xklb/scripts/block.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
                         )
 
         if not matching_media:
             unmatched_playlists.append(p)
             continue
 
         try:
-            matching_media = list(reversed(utils.cluster_dicts(matching_media)))
+            matching_media = list(reversed(utils.cluster_dicts(args, matching_media)))
         except ModuleNotFoundError:
             pass
 
         tbl = utils.list_dict_filter_bool(matching_media)
         tbl = [
             {
                 "title_path": "\n".join(utils.concat(d.get("title"), d.get("webpath"), d["path"])),
```

### Comparing `xklb-2.1.5/xklb/scripts/christen.py` & `xklb-2.1.6/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/scripts/cluster_sort.py` & `xklb-2.1.6/xklb/scripts/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/scripts/copy_play_counts.py` & `xklb-2.1.6/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/scripts/dedupe.py` & `xklb-2.1.6/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/scripts/dedupe_db.py` & `xklb-2.1.6/xklb/scripts/dedupe_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/scripts/download_status.py` & `xklb-2.1.6/xklb/scripts/download_status.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/scripts/history.py` & `xklb-2.1.6/xklb/scripts/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/scripts/merge_dbs.py` & `xklb-2.1.6/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/scripts/merge_online_local.py` & `xklb-2.1.6/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/scripts/move_list.py` & `xklb-2.1.6/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/scripts/optimize_db.py` & `xklb-2.1.6/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/scripts/playback_control.py` & `xklb-2.1.6/xklb/scripts/playback_control.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/scripts/playlists.py` & `xklb-2.1.6/xklb/scripts/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/scripts/redownload.py` & `xklb-2.1.6/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/scripts/relmv.py` & `xklb-2.1.6/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/scripts/scatter.py` & `xklb-2.1.6/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/scripts/streaming_tab_loader.py` & `xklb-2.1.6/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/scripts/mining/data.py` & `xklb-2.1.6/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/scripts/mining/extract_links.py` & `xklb-2.1.6/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/scripts/mining/mpv_watchlater.py` & `xklb-2.1.6/xklb/scripts/mining/mpv_watchlater.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/scripts/mining/nouns.py` & `xklb-2.1.6/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/scripts/mining/pushshift.py` & `xklb-2.1.6/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/scripts/mining/reddit_selftext.py` & `xklb-2.1.6/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/xklb/assets/kotobago.png` & `xklb-2.1.6/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/.gitignore` & `xklb-2.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/LICENSE` & `xklb-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/README.md` & `xklb-2.1.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.1.005)
+    xk media library subcommands (v2.1.006)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
@@ -523,27 +523,27 @@
 <details><summary>Add tabs (tabsadd)</summary>
 
     $ library tabsadd -h
     usage: library tabsadd [--frequency daily weekly (monthly) quarterly yearly] [--no-sanitize] DATABASE URLS ...
 
     Adding one URL:
 
-        library tabsadd -f monthly -c travel ~/lb/tabs.db https://old.reddit.com/r/Colombia/top/?sort=top&t=month
+        library tabsadd -f monthly -c travel tabs.db https://old.reddit.com/r/Colombia/top/?sort=top&t=month
 
         Depending on your shell you may need to escape the URL (add quotes)
 
         If you use Fish shell know that you can enable features to make pasting easier:
             set -U fish_features stderr-nocaret qmark-noglob regex-easyesc ampersand-nobg-in-token
 
         Also I recommend turning Ctrl+Backspace into a super-backspace for repeating similar commands with long args:
             echo 'bind \b backward-kill-bigword' >> ~/.config/fish/config.fish
 
     Importing from a line-delimitated file:
 
-        library tabsadd -f yearly -c reddit ~/lb/tabs.db (cat ~/mc/yearly-subreddit.cron)
+        library tabsadd -f yearly -c reddit tabs.db (cat ~/mc/yearly-subreddit.cron)
 
 
 
 </details>
 
 <details><summary>Watch / Listen</summary>
 
@@ -1365,14 +1365,19 @@
 
     See what folders take up space
 
         library bigdirs video.db
         library bigdirs audio.db
         library bigdirs fs.db
 
+    lb bigdirs video.db --folder-size=+10G --lower 400 --upper 14000
+
+    lb bigdirs video.db --depth 5
+    lb bigdirs video.db --depth 7
+
 
 </details>
 
 <details><summary>Copy play history (copy-play-counts)</summary>
 
     $ library copy-play-counts -h
     usage: library copy-play-counts DEST_DB SOURCE_DB ... [--source-prefix x] [--target-prefix y]
@@ -1451,15 +1456,15 @@
 
     Reduce number of files per folder (creates more folders)
 
         $ library scatter scatter.db --max-files-per-folder 16000 /test/{0,1,2,3,4,5,6,7,8,9}
 
     Multi-device re-bin: balance by size
 
-        $ library scatter -m /mnt/d1:/mnt/d2:/mnt/d3:/mnt/d4/:/mnt/d5:/mnt/d6:/mnt/d7 ~/lb/fs/scatter.db subfolder/of/mergerfs/mnt
+        $ library scatter -m /mnt/d1:/mnt/d2:/mnt/d3:/mnt/d4/:/mnt/d5:/mnt/d6:/mnt/d7 fs/scatter.db subfolder/of/mergerfs/mnt
         Current path distribution:
         ╒═════════╤══════════════╤══════════════╤═══════════════╤════════════════╤═════════════════╤════════════════╕
         │ mount   │   file_count │ total_size   │ median_size   │ time_created   │ time_modified   │ time_scanned   │
         ╞═════════╪══════════════╪══════════════╪═══════════════╪════════════════╪═════════════════╪════════════════╡
         │ /mnt/d1 │        12793 │ 169.5 GB     │ 4.5 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
         ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
         │ /mnt/d2 │        13226 │ 177.9 GB     │ 4.7 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
@@ -1498,19 +1503,19 @@
         ### Move 1185 files to /mnt/d3 with this command: ###
         rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpqh2euc8n / /mnt/d3
         ### Move 1134 files to /mnt/d4 with this command: ###
         rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmphzb0gj92 / /mnt/d4
 
     Multi-device re-bin: balance device inodes for specific subfolder
 
-        $ library scatter -m /mnt/d1:/mnt/d2 ~/lb/fs/scatter.db subfolder --group count --sort 'size desc'
+        $ library scatter -m /mnt/d1:/mnt/d2 fs/scatter.db subfolder --group count --sort 'size desc'
 
     Multi-device re-bin: only consider the most recent 100 files
 
-        $ library scatter -m /mnt/d1:/mnt/d2 -l 100 -s 'time_modified desc' ~/lb/fs/scatter.db /
+        $ library scatter -m /mnt/d1:/mnt/d2 -l 100 -s 'time_modified desc' fs/scatter.db /
 
 
 </details>
 
 <details><summary>Move files preserving parent folder hierarchy (relmv)</summary>
 
     $ library relmv -h
@@ -1521,15 +1526,15 @@
     Move fresh music to your phone every Sunday:
 
         # move last weeks' music back to their source folders
         library relmv /mnt/d/80_Now_Listening/ /mnt/d/
 
         # move new music for this week
         library relmv (
-            library listen ~/lb/audio.db --local-media-only --where 'play_count=0' --random -L 600 -p f
+            library listen audio.db --local-media-only --where 'play_count=0' --random -L 600 -p f
         ) /mnt/d/80_Now_Listening/
 
 
 </details>
 
 <details><summary>Clean filenames (christen)</summary>
```

### Comparing `xklb-2.1.5/pyproject.toml` & `xklb-2.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-2.1.5/PKG-INFO` & `xklb-2.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 2.1.5
+Version: 2.1.6
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
-    xk media library subcommands (v2.1.005)
+    xk media library subcommands (v2.1.006)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
@@ -608,27 +608,27 @@
 <details><summary>Add tabs (tabsadd)</summary>
 
     $ library tabsadd -h
     usage: library tabsadd [--frequency daily weekly (monthly) quarterly yearly] [--no-sanitize] DATABASE URLS ...
 
     Adding one URL:
 
-        library tabsadd -f monthly -c travel ~/lb/tabs.db https://old.reddit.com/r/Colombia/top/?sort=top&t=month
+        library tabsadd -f monthly -c travel tabs.db https://old.reddit.com/r/Colombia/top/?sort=top&t=month
 
         Depending on your shell you may need to escape the URL (add quotes)
 
         If you use Fish shell know that you can enable features to make pasting easier:
             set -U fish_features stderr-nocaret qmark-noglob regex-easyesc ampersand-nobg-in-token
 
         Also I recommend turning Ctrl+Backspace into a super-backspace for repeating similar commands with long args:
             echo 'bind \b backward-kill-bigword' >> ~/.config/fish/config.fish
 
     Importing from a line-delimitated file:
 
-        library tabsadd -f yearly -c reddit ~/lb/tabs.db (cat ~/mc/yearly-subreddit.cron)
+        library tabsadd -f yearly -c reddit tabs.db (cat ~/mc/yearly-subreddit.cron)
 
 
 
 </details>
 
 <details><summary>Watch / Listen</summary>
 
@@ -1450,14 +1450,19 @@
 
     See what folders take up space
 
         library bigdirs video.db
         library bigdirs audio.db
         library bigdirs fs.db
 
+    lb bigdirs video.db --folder-size=+10G --lower 400 --upper 14000
+
+    lb bigdirs video.db --depth 5
+    lb bigdirs video.db --depth 7
+
 
 </details>
 
 <details><summary>Copy play history (copy-play-counts)</summary>
 
     $ library copy-play-counts -h
     usage: library copy-play-counts DEST_DB SOURCE_DB ... [--source-prefix x] [--target-prefix y]
@@ -1536,15 +1541,15 @@
 
     Reduce number of files per folder (creates more folders)
 
         $ library scatter scatter.db --max-files-per-folder 16000 /test/{0,1,2,3,4,5,6,7,8,9}
 
     Multi-device re-bin: balance by size
 
-        $ library scatter -m /mnt/d1:/mnt/d2:/mnt/d3:/mnt/d4/:/mnt/d5:/mnt/d6:/mnt/d7 ~/lb/fs/scatter.db subfolder/of/mergerfs/mnt
+        $ library scatter -m /mnt/d1:/mnt/d2:/mnt/d3:/mnt/d4/:/mnt/d5:/mnt/d6:/mnt/d7 fs/scatter.db subfolder/of/mergerfs/mnt
         Current path distribution:
         ╒═════════╤══════════════╤══════════════╤═══════════════╤════════════════╤═════════════════╤════════════════╕
         │ mount   │   file_count │ total_size   │ median_size   │ time_created   │ time_modified   │ time_scanned   │
         ╞═════════╪══════════════╪══════════════╪═══════════════╪════════════════╪═════════════════╪════════════════╡
         │ /mnt/d1 │        12793 │ 169.5 GB     │ 4.5 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
         ├─────────┼──────────────┼──────────────┼───────────────┼────────────────┼─────────────────┼────────────────┤
         │ /mnt/d2 │        13226 │ 177.9 GB     │ 4.7 MB        │ Jan 27         │ Jul 19 2022     │ Jan 31         │
@@ -1583,19 +1588,19 @@
         ### Move 1185 files to /mnt/d3 with this command: ###
         rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmpqh2euc8n / /mnt/d3
         ### Move 1134 files to /mnt/d4 with this command: ###
         rsync -aE --xattrs --info=progress2 --remove-source-files --files-from=/tmp/tmphzb0gj92 / /mnt/d4
 
     Multi-device re-bin: balance device inodes for specific subfolder
 
-        $ library scatter -m /mnt/d1:/mnt/d2 ~/lb/fs/scatter.db subfolder --group count --sort 'size desc'
+        $ library scatter -m /mnt/d1:/mnt/d2 fs/scatter.db subfolder --group count --sort 'size desc'
 
     Multi-device re-bin: only consider the most recent 100 files
 
-        $ library scatter -m /mnt/d1:/mnt/d2 -l 100 -s 'time_modified desc' ~/lb/fs/scatter.db /
+        $ library scatter -m /mnt/d1:/mnt/d2 -l 100 -s 'time_modified desc' fs/scatter.db /
 
 
 </details>
 
 <details><summary>Move files preserving parent folder hierarchy (relmv)</summary>
 
     $ library relmv -h
@@ -1606,15 +1611,15 @@
     Move fresh music to your phone every Sunday:
 
         # move last weeks' music back to their source folders
         library relmv /mnt/d/80_Now_Listening/ /mnt/d/
 
         # move new music for this week
         library relmv (
-            library listen ~/lb/audio.db --local-media-only --where 'play_count=0' --random -L 600 -p f
+            library listen audio.db --local-media-only --where 'play_count=0' --random -L 600 -p f
         ) /mnt/d/80_Now_Listening/
 
 
 </details>
 
 <details><summary>Clean filenames (christen)</summary>
```

