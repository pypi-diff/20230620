# Comparing `tmp/snapchat-dlp-1.5.2.tar.gz` & `tmp/snapchat-dlp-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapchat-dlp-1.5.2.tar", last modified: Mon Jun 19 09:07:10 2023, max compression
+gzip compressed data, was "snapchat-dlp-1.5.8.tar", last modified: Tue Jun 20 07:31:29 2023, max compression
```

## Comparing `snapchat-dlp-1.5.2.tar` & `snapchat-dlp-1.5.8.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 09:07:10.307494 snapchat-dlp-1.5.2/
--rw-rw-rw-   0        0        0      170 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/AUTHORS.rst
--rw-rw-rw-   0        0        0     1092 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/LICENSE
--rw-rw-rw-   0        0        0      318 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4945 2023-06-19 09:07:10.307494 snapchat-dlp-1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     3754 2023-06-19 07:07:33.000000 snapchat-dlp-1.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 09:07:10.214755 snapchat-dlp-1.5.2/docs/
--rw-rw-rw-   0        0        0      633 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.2/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/docs/authors.rst
--rw-rw-rw-   0        0        0     5093 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.2/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/docs/history.rst
--rw-rw-rw-   0        0        0      345 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/docs/index.rst
--rw-rw-rw-   0        0        0     1222 2023-06-19 07:07:33.000000 snapchat-dlp-1.5.2/docs/installation.rst
--rwxrwxrwx   0        0        0      810 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.2/docs/make.bat
--rw-rw-rw-   0        0        0       79 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.2/docs/modules.rst
--rw-rw-rw-   0        0        0       28 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/docs/readme.rst
--rw-rw-rw-   0        0        0      523 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.2/docs/snapchat_dl.rst
--rw-rw-rw-   0        0        0       93 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.2/docs/usage.rst
--rw-rw-rw-   0        0        0       29 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/requirements.txt
--rw-rw-rw-   0        0        0      364 2023-06-19 09:07:10.309534 snapchat-dlp-1.5.2/setup.cfg
--rw-rw-rw-   0        0        0     2084 2023-06-19 07:07:33.000000 snapchat-dlp-1.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:07:10.228648 snapchat-dlp-1.5.2/snapchat_dlp/
--rw-rw-rw-   0        0        0      200 2023-06-19 08:48:53.000000 snapchat-dlp-1.5.2/snapchat_dlp/__init__.py
--rw-rw-rw-   0        0        0     2834 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.2/snapchat_dlp/app.py
--rw-rw-rw-   0        0        0     3231 2023-06-19 07:07:33.000000 snapchat-dlp-1.5.2/snapchat_dlp/cli.py
--rw-rw-rw-   0        0        0     1566 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.2/snapchat_dlp/downloader.py
--rw-rw-rw-   0        0        0     5147 2023-06-19 08:05:15.000000 snapchat-dlp-1.5.2/snapchat_dlp/snapchat_dlp.py
--rw-rw-rw-   0        0        0     4077 2023-06-19 08:04:48.000000 snapchat-dlp-1.5.2/snapchat_dlp/utils.py
--rw-rw-rw-   0        0        0       23 2023-06-19 09:07:04.000000 snapchat-dlp-1.5.2/snapchat_dlp/version.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:07:10.285177 snapchat-dlp-1.5.2/snapchat_dlp.egg-info/
--rw-rw-rw-   0        0        0     4945 2023-06-19 09:07:09.000000 snapchat-dlp-1.5.2/snapchat_dlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1073 2023-06-19 09:07:09.000000 snapchat-dlp-1.5.2/snapchat_dlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 09:07:09.000000 snapchat-dlp-1.5.2/snapchat_dlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-06-19 09:07:09.000000 snapchat-dlp-1.5.2/snapchat_dlp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-19 07:17:46.000000 snapchat-dlp-1.5.2/snapchat_dlp.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2023-06-19 09:07:09.000000 snapchat-dlp-1.5.2/snapchat_dlp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-19 09:07:09.000000 snapchat-dlp-1.5.2/snapchat_dlp.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 09:07:10.292179 snapchat-dlp-1.5.2/tests/
--rw-rw-rw-   0        0        0       43 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.2/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:07:10.301880 snapchat-dlp-1.5.2/tests/mock_data/
-drwxrwxrwx   0        0        0        0 2023-06-19 09:07:10.302957 snapchat-dlp-1.5.2/tests/mock_data/23/
--rw-rw-rw-   0        0        0       75 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/tests/mock_data/23/.gitignore
--rw-rw-rw-   0        0        0    37579 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/tests/mock_data/api-error.html
--rw-rw-rw-   0        0        0       38 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/tests/mock_data/batch_file.txt
--rw-rw-rw-   0        0        0    36109 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/tests/mock_data/invalidusername-nostories.html
--rw-rw-rw-   0        0        0    37580 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/tests/mock_data/invalidusername.html
--rw-rw-rw-   0        0        0     2184 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/tests/mock_data/invalidusername.json
-drwxrwxrwx   0        0        0        0 2023-06-19 09:07:10.303979 snapchat-dlp-1.5.2/tests/mock_data/user.1name/
--rw-rw-rw-   0        0        0       75 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/tests/mock_data/user.1name/.gitignore
-drwxrwxrwx   0        0        0        0 2023-06-19 09:07:10.306462 snapchat-dlp-1.5.2/tests/mock_data/user1/
--rw-rw-rw-   0        0        0       75 2023-06-12 06:29:52.000000 snapchat-dlp-1.5.2/tests/mock_data/user1/.gitignore
--rw-rw-rw-   0        0        0     1238 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.2/tests/test_downlaoder.py
--rw-rw-rw-   0        0        0     2506 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.2/tests/test_snapchat_dl.py
--rw-rw-rw-   0        0        0     1934 2023-06-19 07:04:19.000000 snapchat-dlp-1.5.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:31:29.482376 snapchat-dlp-1.5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-06-20 07:31:29.482376 snapchat-dlp-1.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:31:29.478376 snapchat-dlp-1.5.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/docs/snapchat_dl.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-20 07:31:29.482376 snapchat-dlp-1.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:31:29.478376 snapchat-dlp-1.5.8/snapchat_dlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/snapchat_dlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/snapchat_dlp/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/snapchat_dlp/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/snapchat_dlp/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/snapchat_dlp/snapchat_dlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/snapchat_dlp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/snapchat_dlp/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:31:29.478376 snapchat-dlp-1.5.8/snapchat_dlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-06-20 07:31:29.000000 snapchat-dlp-1.5.8/snapchat_dlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-20 07:31:29.000000 snapchat-dlp-1.5.8/snapchat_dlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 07:31:29.000000 snapchat-dlp-1.5.8/snapchat_dlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 07:31:29.000000 snapchat-dlp-1.5.8/snapchat_dlp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 07:31:29.000000 snapchat-dlp-1.5.8/snapchat_dlp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-20 07:31:29.000000 snapchat-dlp-1.5.8/snapchat_dlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 07:31:29.000000 snapchat-dlp-1.5.8/snapchat_dlp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:31:29.478376 snapchat-dlp-1.5.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:31:29.482376 snapchat-dlp-1.5.8/tests/mock_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:31:29.482376 snapchat-dlp-1.5.8/tests/mock_data/23/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/tests/mock_data/23/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    37542 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/tests/mock_data/api-error.html
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/tests/mock_data/batch_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    36072 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/tests/mock_data/invalidusername-nostories.html
+-rw-r--r--   0 runner    (1001) docker     (123)    37543 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/tests/mock_data/invalidusername.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/tests/mock_data/invalidusername.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:31:29.482376 snapchat-dlp-1.5.8/tests/mock_data/user.1name/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/tests/mock_data/user.1name/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:31:29.482376 snapchat-dlp-1.5.8/tests/mock_data/user1/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/tests/mock_data/user1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/tests/test_downlaoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/tests/test_snapchat_dl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-20 07:31:18.000000 snapchat-dlp-1.5.8/tests/test_utils.py
```

### Comparing `snapchat-dlp-1.5.2/README.md` & `snapchat-dlp-1.5.8/README.md`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-<p>
-  <div align="center">
-  <h1>
-    Snapchat Public Stories Downloader<br /> <br />
-    <!-- <a href="https://pypi.python.org/pypi/snapchat-dlp">
-      <img
-        src="https://img.shields.io/pypi/v/snapchat-dlp.svg?cacheSeconds=360"
-        alt="Python Package"
-      />
-    </a>
-    <a href="https://pypi.python.org/pypi/snapchat-dlp">
-      <img
-        src="https://img.shields.io/pypi/wheel/snapchat-dlp"
-        alt="Python Wheel"
-      />
-    </a>
-    <a href="https://pypi.python.org/pypi/snapchat-dlp">
-      <img
-        src="https://img.shields.io/github/workflow/status/skyme5/snapchat-dlp/build?cacheSeconds=360"
-        alt="CI"
-      />
-    </a>
-    <a href="https://codecov.io/gh/skyme5/snapchat-dlp">
-      <img
-        src="https://img.shields.io/codecov/c/github/skyme5/snapchat-dlp?cacheSeconds=360"
-        alt="Code Coverage"
-      />
-    </a>
-    <a href="https://codecov.io/gh/skyme5/snapchat-dlp">
-      <img
-        src="https://img.shields.io/pypi/pyversions/snapchat-dlp"
-        alt="Python Versions"
-      />
-    </a>
-    <a href="https://github.com/psf/black">
-      <img
-        src="https://img.shields.io/badge/code%20style-black-000000.svg"
-        alt="The Uncompromising Code Formatter"
-      />
-    </a>
-    <a href="https://pepy.tech/project/snapchat-dlp">
-      <img
-        src="https://static.pepy.tech/badge/snapchat-dlp"
-        alt="Monthly Downloads"
-      />
-    </a>
-    <a href="https://opensource.org/licenses/MIT">
-      <img
-        src="https://img.shields.io/badge/License-MIT-blue.svg"
-        alt="License: MIT"
-      />
-    </a> -->
-  </h1>
-</p>
-
-### Installation
-
-Install using pip,
-
-```bash
-pip install snapchat-dlp
-```
-
-Install from GitHub,
-
-```bash
-pip install git+git://github.com/Walmann/snapchat-dlp
-```
-
-Unix users might want to add `--user` flag to install without requiring `sudo`.
-
-### Usage
-
-```text
-
-usage: snapchat-dlp [-h] [-c | -u] [-i BATCH_FILENAME] [-P DIRECTORY_PREFIX]
-                   [-s] [-d] [-l MAX_NUM_STORY] [-j MAX_WORKERS] [-t INTERVAL]
-                   [--sleep-interval INTERVAL] [-q]
-                   [username [username ...]]
-
-positional arguments:
-  username              At least one or more usernames to download stories
-                        for.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -c, --scan-clipboard  Scan clipboard for story links
-                        ('https://story.snapchat.com/<s>/<username>').
-  -u, --check-for-update
-                        Periodically check for new stories.
-  -i BATCH_FILENAME, --batch-file BATCH_FILENAME
-                        Read usernames from batch file (one username per
-                        line).
-  -P DIRECTORY_PREFIX, --directory-prefix DIRECTORY_PREFIX
-                        Location to store downloaded media.
-  -s, --scan-from-prefix
-                        Scan usernames (as directory name) from prefix
-                        directory.
-  -d, --dump-json       Save metadata to a JSON file next to downloaded
-                        videos/pictures.
-  -l MAX_NUM_STORY, --limit-story MAX_NUM_STORY
-                        Set maximum number of stories to download.
-  -j MAX_WORKERS, --max-concurrent-downloads MAX_WORKERS
-                        Set maximum number of parallel downloads.
-  -t INTERVAL, --update-interval INTERVAL
-                        Set the update interval for checking new story in
-                        seconds. (Default: 10m)
-  --sleep-interval INTERVAL
-                        Sleep between downloads in seconds. (Default: 1s)
-  -q, --quiet           Do not print anything except errors to the console.
-
-```
+<p>
+  <div align="center">
+  <h1>
+    Snapchat Public Stories Downloader<br /> <br />
+    <!-- <a href="https://pypi.python.org/pypi/snapchat-dlp">
+      <img
+        src="https://img.shields.io/pypi/v/snapchat-dlp.svg?cacheSeconds=360"
+        alt="Python Package"
+      />
+    </a>
+    <a href="https://pypi.python.org/pypi/snapchat-dlp">
+      <img
+        src="https://img.shields.io/pypi/wheel/snapchat-dlp"
+        alt="Python Wheel"
+      />
+    </a>
+    <a href="https://pypi.python.org/pypi/snapchat-dlp">
+      <img
+        src="https://img.shields.io/github/workflow/status/skyme5/snapchat-dlp/build?cacheSeconds=360"
+        alt="CI"
+      />
+    </a>
+    <a href="https://codecov.io/gh/skyme5/snapchat-dlp">
+      <img
+        src="https://img.shields.io/codecov/c/github/skyme5/snapchat-dlp?cacheSeconds=360"
+        alt="Code Coverage"
+      />
+    </a>
+    <a href="https://codecov.io/gh/skyme5/snapchat-dlp">
+      <img
+        src="https://img.shields.io/pypi/pyversions/snapchat-dlp"
+        alt="Python Versions"
+      />
+    </a>
+    <a href="https://github.com/psf/black">
+      <img
+        src="https://img.shields.io/badge/code%20style-black-000000.svg"
+        alt="The Uncompromising Code Formatter"
+      />
+    </a>
+    <a href="https://pepy.tech/project/snapchat-dlp">
+      <img
+        src="https://static.pepy.tech/badge/snapchat-dlp"
+        alt="Monthly Downloads"
+      />
+    </a>
+    <a href="https://opensource.org/licenses/MIT">
+      <img
+        src="https://img.shields.io/badge/License-MIT-blue.svg"
+        alt="License: MIT"
+      />
+    </a> -->
+  </h1>
+</p>
+
+### Installation
+
+Install using pip,
+
+```bash
+pip install snapchat-dlp
+```
+
+Install from GitHub,
+
+```bash
+pip install git+git://github.com/Walmann/snapchat-dlp
+```
+
+Unix users might want to add `--user` flag to install without requiring `sudo`.
+
+### Usage
+
+```text
+
+usage: snapchat-dlp [-h] [-c | -u] [-i BATCH_FILENAME] [-P DIRECTORY_PREFIX]
+                   [-s] [-d] [-l MAX_NUM_STORY] [-j MAX_WORKERS] [-t INTERVAL]
+                   [--sleep-interval INTERVAL] [-q]
+                   [username [username ...]]
+
+positional arguments:
+  username              At least one or more usernames to download stories
+                        for.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -c, --scan-clipboard  Scan clipboard for story links
+                        ('https://story.snapchat.com/<s>/<username>').
+  -u, --check-for-update
+                        Periodically check for new stories.
+  -i BATCH_FILENAME, --batch-file BATCH_FILENAME
+                        Read usernames from batch file (one username per
+                        line).
+  -P DIRECTORY_PREFIX, --directory-prefix DIRECTORY_PREFIX
+                        Location to store downloaded media.
+  -s, --scan-from-prefix
+                        Scan usernames (as directory name) from prefix
+                        directory.
+  -d, --dump-json       Save metadata to a JSON file next to downloaded
+                        videos/pictures.
+  -l MAX_NUM_STORY, --limit-story MAX_NUM_STORY
+                        Set maximum number of stories to download.
+  -j MAX_WORKERS, --max-concurrent-downloads MAX_WORKERS
+                        Set maximum number of parallel downloads.
+  -t INTERVAL, --update-interval INTERVAL
+                        Set the update interval for checking new story in
+                        seconds. (Default: 10m)
+  --sleep-interval INTERVAL
+                        Sleep between downloads in seconds. (Default: 1s)
+  -q, --quiet           Do not print anything except errors to the console.
+
+```
```

### Comparing `snapchat-dlp-1.5.2/docs/conf.py` & `snapchat-dlp-1.5.8/docs/conf.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,161 +1,161 @@
-#!/usr/bin/env python
-#
-# snapchat_dlp documentation build configuration file, created by
-# sphinx-quickstart on Fri Jun  9 13:47:02 2017.
-#
-# This file is execfile()d with the current directory set to its
-# containing dir.
-#
-# Note that not all possible configuration values are present in this
-# autogenerated file.
-#
-# All configuration values have a default; values that are commented out
-# serve to show the default.
-# If extensions (or modules to document with autodoc) are in another
-# directory, add these directories to sys.path here. If the directory is
-# relative to the documentation root, use os.path.abspath to make it
-# absolute, like shown here.
-#
-import os
-import sys
-
-sys.path.insert(0, os.path.abspath(".."))
-
-import snapchat_dlp
-
-# -- General configuration ---------------------------------------------
-
-# If your documentation needs a minimal Sphinx version, state it here.
-#
-# needs_sphinx = '1.0'
-
-# Add any Sphinx extension module names here, as strings. They can be
-# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ["sphinx.ext.autodoc", "sphinx.ext.viewcode"]
-
-# Add any paths that contain templates here, relative to this directory.
-templates_path = ["_templates"]
-
-# The suffix(es) of source filenames.
-# You can specify multiple suffix as a list of string:
-#
-# source_suffix = ['.rst', '.md']
-source_suffix = ".rst"
-
-# The master toctree document.
-master_doc = "index"
-
-# General information about the project.
-project = "Snapchat Downloader"
-copyright = "2020, Aakash Gajjar"
-author = "Aakash Gajjar"
-
-# The version info for the project you're documenting, acts as replacement
-# for |version| and |release|, also used in various other places throughout
-# the built documents.
-#
-# The short X.Y version.
-version = snapchat_dlp.__version__
-# The full version, including alpha/beta/rc tags.
-release = snapchat_dlp.__version__
-
-# The language for content autogenerated by Sphinx. Refer to documentation
-# for a list of supported languages.
-#
-# This is also used if you do content translation via gettext catalogs.
-# Usually you set "language" from the command line for these cases.
-language = None
-
-# List of patterns, relative to source directory, that match files and
-# directories to ignore when looking for source files.
-# This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
-
-# The name of the Pygments (syntax highlighting) style to use.
-pygments_style = "sphinx"
-
-# If true, `todo` and `todoList` produce output, else they produce nothing.
-todo_include_todos = False
-
-
-# -- Options for HTML output -------------------------------------------
-
-# The theme to use for HTML and HTML Help pages.  See the documentation for
-# a list of builtin themes.
-#
-html_theme = "alabaster"
-
-# Theme options are theme-specific and customize the look and feel of a
-# theme further.  For a list of options available for each theme, see the
-# documentation.
-#
-# html_theme_options = {}
-
-# Add any paths that contain custom static files (such as style sheets) here,
-# relative to this directory. They are copied after the builtin static files,
-# so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ["_static"]
-
-
-# -- Options for HTMLHelp output ---------------------------------------
-
-# Output file base name for HTML help builder.
-htmlhelp_basename = "snapchat_dldoc"
-
-
-# -- Options for LaTeX output ------------------------------------------
-
-latex_elements = {
-    # The paper size ('letterpaper' or 'a4paper').
-    #
-    # 'papersize': 'letterpaper',
-    # The font size ('10pt', '11pt' or '12pt').
-    #
-    # 'pointsize': '10pt',
-    # Additional stuff for the LaTeX preamble.
-    #
-    # 'preamble': '',
-    # Latex figure (float) alignment
-    #
-    # 'figure_align': 'htbp',
-}
-
-# Grouping the document tree into LaTeX files. List of tuples
-# (source start file, target name, title, author, documentclass
-# [howto, manual, or own class]).
-latex_documents = [
-    (
-        master_doc,
-        "snapchat_dlp.tex",
-        "Snapchat Downloader Documentation",
-        "Aakash Gajjar",
-        "manual",
-    ),
-]
-
-
-# -- Options for manual page output ------------------------------------
-
-# One entry per manual page. List of tuples
-# (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, "snapchat_dlp", "Snapchat Downloader Documentation", [author], 1)
-]
-
-
-# -- Options for Texinfo output ----------------------------------------
-
-# Grouping the document tree into Texinfo files. List of tuples
-# (source start file, target name, title, author,
-#  dir menu entry, description, category)
-texinfo_documents = [
-    (
-        master_doc,
-        "snapchat_dlp",
-        "Snapchat Downloader Documentation",
-        author,
-        "snapchat_dlp",
-        "One line description of project.",
-        "Miscellaneous",
-    ),
-]
+#!/usr/bin/env python
+#
+# snapchat_dlp documentation build configuration file, created by
+# sphinx-quickstart on Fri Jun  9 13:47:02 2017.
+#
+# This file is execfile()d with the current directory set to its
+# containing dir.
+#
+# Note that not all possible configuration values are present in this
+# autogenerated file.
+#
+# All configuration values have a default; values that are commented out
+# serve to show the default.
+# If extensions (or modules to document with autodoc) are in another
+# directory, add these directories to sys.path here. If the directory is
+# relative to the documentation root, use os.path.abspath to make it
+# absolute, like shown here.
+#
+import os
+import sys
+
+sys.path.insert(0, os.path.abspath(".."))
+
+import snapchat_dlp
+
+# -- General configuration ---------------------------------------------
+
+# If your documentation needs a minimal Sphinx version, state it here.
+#
+# needs_sphinx = '1.0'
+
+# Add any Sphinx extension module names here, as strings. They can be
+# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
+extensions = ["sphinx.ext.autodoc", "sphinx.ext.viewcode"]
+
+# Add any paths that contain templates here, relative to this directory.
+templates_path = ["_templates"]
+
+# The suffix(es) of source filenames.
+# You can specify multiple suffix as a list of string:
+#
+# source_suffix = ['.rst', '.md']
+source_suffix = ".rst"
+
+# The master toctree document.
+master_doc = "index"
+
+# General information about the project.
+project = "Snapchat Downloader"
+copyright = "2020, Aakash Gajjar"
+author = "Aakash Gajjar"
+
+# The version info for the project you're documenting, acts as replacement
+# for |version| and |release|, also used in various other places throughout
+# the built documents.
+#
+# The short X.Y version.
+version = snapchat_dlp.__version__
+# The full version, including alpha/beta/rc tags.
+release = snapchat_dlp.__version__
+
+# The language for content autogenerated by Sphinx. Refer to documentation
+# for a list of supported languages.
+#
+# This is also used if you do content translation via gettext catalogs.
+# Usually you set "language" from the command line for these cases.
+language = None
+
+# List of patterns, relative to source directory, that match files and
+# directories to ignore when looking for source files.
+# This patterns also effect to html_static_path and html_extra_path
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
+
+# The name of the Pygments (syntax highlighting) style to use.
+pygments_style = "sphinx"
+
+# If true, `todo` and `todoList` produce output, else they produce nothing.
+todo_include_todos = False
+
+
+# -- Options for HTML output -------------------------------------------
+
+# The theme to use for HTML and HTML Help pages.  See the documentation for
+# a list of builtin themes.
+#
+html_theme = "alabaster"
+
+# Theme options are theme-specific and customize the look and feel of a
+# theme further.  For a list of options available for each theme, see the
+# documentation.
+#
+# html_theme_options = {}
+
+# Add any paths that contain custom static files (such as style sheets) here,
+# relative to this directory. They are copied after the builtin static files,
+# so a file named "default.css" will overwrite the builtin "default.css".
+html_static_path = ["_static"]
+
+
+# -- Options for HTMLHelp output ---------------------------------------
+
+# Output file base name for HTML help builder.
+htmlhelp_basename = "snapchat_dldoc"
+
+
+# -- Options for LaTeX output ------------------------------------------
+
+latex_elements = {
+    # The paper size ('letterpaper' or 'a4paper').
+    #
+    # 'papersize': 'letterpaper',
+    # The font size ('10pt', '11pt' or '12pt').
+    #
+    # 'pointsize': '10pt',
+    # Additional stuff for the LaTeX preamble.
+    #
+    # 'preamble': '',
+    # Latex figure (float) alignment
+    #
+    # 'figure_align': 'htbp',
+}
+
+# Grouping the document tree into LaTeX files. List of tuples
+# (source start file, target name, title, author, documentclass
+# [howto, manual, or own class]).
+latex_documents = [
+    (
+        master_doc,
+        "snapchat_dlp.tex",
+        "Snapchat Downloader Documentation",
+        "Aakash Gajjar",
+        "manual",
+    ),
+]
+
+
+# -- Options for manual page output ------------------------------------
+
+# One entry per manual page. List of tuples
+# (source start file, name, description, authors, manual section).
+man_pages = [
+    (master_doc, "snapchat_dlp", "Snapchat Downloader Documentation", [author], 1)
+]
+
+
+# -- Options for Texinfo output ----------------------------------------
+
+# Grouping the document tree into Texinfo files. List of tuples
+# (source start file, target name, title, author,
+#  dir menu entry, description, category)
+texinfo_documents = [
+    (
+        master_doc,
+        "snapchat_dlp",
+        "Snapchat Downloader Documentation",
+        author,
+        "snapchat_dlp",
+        "One line description of project.",
+        "Miscellaneous",
+    ),
+]
```

### Comparing `snapchat-dlp-1.5.2/docs/installation.rst` & `snapchat-dlp-1.5.8/docs/installation.rst`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-.. highlight:: shell
-
-============
-Installation
-============
-
-
-Stable release
---------------
-
-To install Snapchat Downloader, run this command in your terminal:
-
-.. code-block:: console
-
-    $ pip install snapchat-dlp
-
-This is the preferred method to install Snapchat Downloader, as it will always install the most recent stable release.
-
-If you don't have `pip`_ installed, this `Python installation guide`_ can guide
-you through the process.
-
-.. _pip: https://pip.pypa.io
-.. _Python installation guide: http://docs.python-guide.org/en/latest/starting/installation/
-
-
-From sources
-------------
-
-The sources for Snapchat Downloader can be downloaded from the `Github repo`_.
-
-You can either clone the public repository:
-
-.. code-block:: console
-
-    $ git clone git://github.com/Walmann/snapchat-dlp
-
-Or download the `tarball`_:
-
-.. code-block:: console
-
-    $ curl -OJL https://github.com/Walmann/snapchat-dlp/tarball/master
-
-Once you have a copy of the source, you can install it with:
-
-.. code-block:: console
-
-    $ python setup.py install
-
-
-.. _Github repo: https://github.com/Walmann/snapchat-dlp
-.. _tarball: https://github.com/Walmann/snapchat-dlp/tarball/master
+.. highlight:: shell
+
+============
+Installation
+============
+
+
+Stable release
+--------------
+
+To install Snapchat Downloader, run this command in your terminal:
+
+.. code-block:: console
+
+    $ pip install snapchat-dlp
+
+This is the preferred method to install Snapchat Downloader, as it will always install the most recent stable release.
+
+If you don't have `pip`_ installed, this `Python installation guide`_ can guide
+you through the process.
+
+.. _pip: https://pip.pypa.io
+.. _Python installation guide: http://docs.python-guide.org/en/latest/starting/installation/
+
+
+From sources
+------------
+
+The sources for Snapchat Downloader can be downloaded from the `Github repo`_.
+
+You can either clone the public repository:
+
+.. code-block:: console
+
+    $ git clone git://github.com/Walmann/snapchat-dlp
+
+Or download the `tarball`_:
+
+.. code-block:: console
+
+    $ curl -OJL https://github.com/Walmann/snapchat-dlp/tarball/master
+
+Once you have a copy of the source, you can install it with:
+
+.. code-block:: console
+
+    $ python setup.py install
+
+
+.. _Github repo: https://github.com/Walmann/snapchat-dlp
+.. _tarball: https://github.com/Walmann/snapchat-dlp/tarball/master
```

### Comparing `snapchat-dlp-1.5.2/docs/make.bat` & `snapchat-dlp-1.5.8/docs/make.bat`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-@ECHO OFF
-
-pushd %~dp0
-
-REM Command file for Sphinx documentation
-
-if "%SPHINXBUILD%" == "" (
-	set SPHINXBUILD=python -msphinx
-)
-set SOURCEDIR=.
-set BUILDDIR=_build
-set SPHINXPROJ=snapchat_dlp
-
-if "%1" == "" goto help
-
-%SPHINXBUILD% >NUL 2>NUL
-if errorlevel 9009 (
-	echo.
-	echo.The Sphinx module was not found. Make sure you have Sphinx installed,
-	echo.then set the SPHINXBUILD environment variable to point to the full
-	echo.path of the 'sphinx-build' executable. Alternatively you may add the
-	echo.Sphinx directory to PATH.
-	echo.
-	echo.If you don't have Sphinx installed, grab it from
-	echo.http://sphinx-doc.org/
-	exit /b 1
-)
-
-%SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS%
-goto end
-
-:help
-%SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS%
-
-:end
-popd
+@ECHO OFF
+
+pushd %~dp0
+
+REM Command file for Sphinx documentation
+
+if "%SPHINXBUILD%" == "" (
+	set SPHINXBUILD=python -msphinx
+)
+set SOURCEDIR=.
+set BUILDDIR=_build
+set SPHINXPROJ=snapchat_dlp
+
+if "%1" == "" goto help
+
+%SPHINXBUILD% >NUL 2>NUL
+if errorlevel 9009 (
+	echo.
+	echo.The Sphinx module was not found. Make sure you have Sphinx installed,
+	echo.then set the SPHINXBUILD environment variable to point to the full
+	echo.path of the 'sphinx-build' executable. Alternatively you may add the
+	echo.Sphinx directory to PATH.
+	echo.
+	echo.If you don't have Sphinx installed, grab it from
+	echo.http://sphinx-doc.org/
+	exit /b 1
+)
+
+%SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS%
+goto end
+
+:help
+%SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS%
+
+:end
+popd
```

### Comparing `snapchat-dlp-1.5.2/snapchat_dlp/app.py` & `snapchat-dlp-1.5.8/snapchat_dlp/app.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-"""Commandline setup for snapchat_dlp."""
-import sys
-import time
-
-import pyperclip
-from loguru import logger
-
-from snapchat_dlp.cli import parse_arguments
-from snapchat_dlp.snapchat_dlp import SnapchatDL
-from snapchat_dlp.utils import NoStoriesFound
-from snapchat_dlp.utils import search_usernames
-from snapchat_dlp.utils import use_batch_file
-from snapchat_dlp.utils import use_prefix_dir
-from snapchat_dlp.utils import UserNotFoundError
-
-
-def main():
-    """Download user stories from Snapchat."""
-    args = parse_arguments()
-    usernames = args.username + use_batch_file(args) + use_prefix_dir(args)
-
-    downlaoder = SnapchatDL(
-        directory_prefix=args.save_prefix,
-        max_workers=args.max_workers,
-        limit_story=args.limit_story,
-        sleep_interval=args.sleep_interval,
-        quiet=args.quiet,
-        dump_json=args.dump_json,
-    )
-
-    history = list()
-
-    def download_users(users: list, respect_history=False):
-        """Download user story from usernames.
-
-        Args:
-            users (list): List of usernames to download.
-            respect_history (bool, optional): append username to history. Defaults to False.
-            log_str (str, optional): Log log_str to terminal. Defaults to None.
-        """
-        for username in users:
-            time.sleep(args.sleep_interval)
-
-            if respect_history is True:
-                if username not in history:
-                    history.append(username)
-                    try:
-                        downlaoder.download(username)
-                    except (NoStoriesFound, UserNotFoundError):
-                        pass
-            else:
-                try:
-                    downlaoder.download(username)
-                except (NoStoriesFound, UserNotFoundError):
-                    pass
-
-    try:
-        download_users(usernames)
-        if args.scan_clipboard is True:
-            if args.quiet is False:
-                logger.info("Listening for clipboard change")
-
-            while True:
-                usernames_clip = search_usernames(pyperclip.paste())
-                if len(usernames_clip) > 0:
-                    download_users(usernames_clip, respect_history=True)
-
-                time.sleep(1)
-
-        if args.check_update is True:
-            if args.quiet is False:
-                logger.info(
-                    "Scheduling story updates for {} users".format(len(usernames))
-                )
-
-            while True:
-                started_at = int(time.time())
-                download_users(usernames)
-                if started_at < args.interval:
-                    time.sleep(args.interval - started_at)
-
-    except KeyboardInterrupt:
-        exit(0)
-
-
-if __name__ == "__main__":
-    sys.exit(main())
+"""Commandline setup for snapchat_dlp."""
+import sys
+import time
+
+import pyperclip
+from loguru import logger
+
+from snapchat_dlp.cli import parse_arguments
+from snapchat_dlp.snapchat_dlp import SnapchatDL
+from snapchat_dlp.utils import NoStoriesFound
+from snapchat_dlp.utils import search_usernames
+from snapchat_dlp.utils import use_batch_file
+from snapchat_dlp.utils import use_prefix_dir
+from snapchat_dlp.utils import UserNotFoundError
+
+
+def main():
+    """Download user stories from Snapchat."""
+    args = parse_arguments()
+    usernames = args.username + use_batch_file(args) + use_prefix_dir(args)
+
+    downlaoder = SnapchatDL(
+        directory_prefix=args.save_prefix,
+        max_workers=args.max_workers,
+        limit_story=args.limit_story,
+        sleep_interval=args.sleep_interval,
+        quiet=args.quiet,
+        dump_json=args.dump_json,
+    )
+
+    history = list()
+
+    def download_users(users: list, respect_history=False):
+        """Download user story from usernames.
+
+        Args:
+            users (list): List of usernames to download.
+            respect_history (bool, optional): append username to history. Defaults to False.
+            log_str (str, optional): Log log_str to terminal. Defaults to None.
+        """
+        for username in users:
+            time.sleep(args.sleep_interval)
+
+            if respect_history is True:
+                if username not in history:
+                    history.append(username)
+                    try:
+                        downlaoder.download(username)
+                    except (NoStoriesFound, UserNotFoundError):
+                        pass
+            else:
+                try:
+                    downlaoder.download(username)
+                except (NoStoriesFound, UserNotFoundError):
+                    pass
+
+    try:
+        download_users(usernames)
+        if args.scan_clipboard is True:
+            if args.quiet is False:
+                logger.info("Listening for clipboard change")
+
+            while True:
+                usernames_clip = search_usernames(pyperclip.paste())
+                if len(usernames_clip) > 0:
+                    download_users(usernames_clip, respect_history=True)
+
+                time.sleep(1)
+
+        if args.check_update is True:
+            if args.quiet is False:
+                logger.info(
+                    "Scheduling story updates for {} users".format(len(usernames))
+                )
+
+            while True:
+                started_at = int(time.time())
+                download_users(usernames)
+                if started_at < args.interval:
+                    time.sleep(args.interval - started_at)
+
+    except KeyboardInterrupt:
+        exit(0)
+
+
+if __name__ == "__main__":
+    sys.exit(main())
```

### Comparing `snapchat-dlp-1.5.2/snapchat_dlp/cli.py` & `snapchat-dlp-1.5.8/snapchat_dlp/cli.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-"""Console script for snapchat_dlp."""
-import argparse
-import os
-import sys
-
-
-def parse_arguments():
-    """Console script for snapchat_dlp."""
-    parser = argparse.ArgumentParser(prog="snapchat-dlp")
-
-    parser.add_argument(
-        "username",
-        action="store",
-        nargs="*",
-        help="At least one or more usernames to download stories for.",
-    )
-
-    any_one_group = parser.add_mutually_exclusive_group()
-    any_one_group.add_argument(
-        "-c",
-        "--scan-clipboard",
-        action="store_true",
-        help="Scan clipboard for story links"
-        " ('https://story.snapchat.com/<s>/<username>').",
-        dest="scan_clipboard",
-    )
-
-    any_one_group.add_argument(
-        "-u",
-        "--check-for-update",
-        action="store_true",
-        help="Periodically check for new stories.",
-        dest="check_update",
-    )
-
-    parser.add_argument(
-        "-i",
-        "--batch-file",
-        action="store",
-        default=None,
-        help="Read usernames from batch file (one username per line).",
-        metavar="BATCH_FILENAME",
-        dest="batch_file",
-    )
-
-    parser.add_argument(
-        "-P",
-        "--directory-prefix",
-        action="store",
-        default=os.path.abspath(os.getcwd()),
-        help="Location to store downloaded media.",
-        metavar="DIRECTORY_PREFIX",
-        dest="save_prefix",
-    )
-
-    parser.add_argument(
-        "-s",
-        "--scan-from-prefix",
-        action="store_true",
-        help="Scan usernames (as directory name) from prefix directory.",
-        dest="scan_prefix",
-    )
-
-    parser.add_argument(
-        "-d",
-        "--dump-json",
-        action="store_true",
-        help="Save metadata to a JSON file next to downloaded videos/pictures.",
-        dest="dump_json",
-    )
-
-    parser.add_argument(
-        "-l",
-        "--limit-story",
-        action="store",
-        default=-1,
-        help="Set maximum number of stories to download.",
-        metavar="MAX_NUM_STORY",
-        dest="limit_story",
-        type=int,
-    )
-
-    parser.add_argument(
-        "-j",
-        "--max-concurrent-downloads",
-        action="store",
-        default=2,
-        help="Set maximum number of parallel downloads.",
-        metavar="MAX_WORKERS",
-        dest="max_workers",
-        type=int,
-    )
-
-    parser.add_argument(
-        "-t",
-        "--update-interval",
-        action="store",
-        default=60 * 10,
-        help="Set the update interval for checking new story in seconds. (Default: 10m)",
-        metavar="INTERVAL",
-        dest="interval",
-        type=int,
-    )
-
-    parser.add_argument(
-        "--sleep-interval",
-        action="store",
-        default=1,
-        help="Sleep between downloads in seconds. (Default: 1s)",
-        metavar="INTERVAL",
-        dest="sleep_interval",
-        type=int,
-    )
-
-    parser.add_argument(
-        "-q",
-        "--quiet",
-        action="store_true",
-        help="Do not print anything except errors to the console.",
-    )
-
-    if len(sys.argv) == 1:
-        parser.print_help()
-        sys.exit(1)
-
-    return parser.parse_args()
+"""Console script for snapchat_dlp."""
+import argparse
+import os
+import sys
+
+
+def parse_arguments():
+    """Console script for snapchat_dlp."""
+    parser = argparse.ArgumentParser(prog="snapchat-dlp")
+
+    parser.add_argument(
+        "username",
+        action="store",
+        nargs="*",
+        help="At least one or more usernames to download stories for.",
+    )
+
+    any_one_group = parser.add_mutually_exclusive_group()
+    any_one_group.add_argument(
+        "-c",
+        "--scan-clipboard",
+        action="store_true",
+        help="Scan clipboard for story links"
+        " ('https://story.snapchat.com/<s>/<username>').",
+        dest="scan_clipboard",
+    )
+
+    any_one_group.add_argument(
+        "-u",
+        "--check-for-update",
+        action="store_true",
+        help="Periodically check for new stories.",
+        dest="check_update",
+    )
+
+    parser.add_argument(
+        "-i",
+        "--batch-file",
+        action="store",
+        default=None,
+        help="Read usernames from batch file (one username per line).",
+        metavar="BATCH_FILENAME",
+        dest="batch_file",
+    )
+
+    parser.add_argument(
+        "-P",
+        "--directory-prefix",
+        action="store",
+        default=os.path.abspath(os.getcwd()),
+        help="Location to store downloaded media.",
+        metavar="DIRECTORY_PREFIX",
+        dest="save_prefix",
+    )
+
+    parser.add_argument(
+        "-s",
+        "--scan-from-prefix",
+        action="store_true",
+        help="Scan usernames (as directory name) from prefix directory.",
+        dest="scan_prefix",
+    )
+
+    parser.add_argument(
+        "-d",
+        "--dump-json",
+        action="store_true",
+        help="Save metadata to a JSON file next to downloaded videos/pictures.",
+        dest="dump_json",
+    )
+
+    parser.add_argument(
+        "-l",
+        "--limit-story",
+        action="store",
+        default=-1,
+        help="Set maximum number of stories to download.",
+        metavar="MAX_NUM_STORY",
+        dest="limit_story",
+        type=int,
+    )
+
+    parser.add_argument(
+        "-j",
+        "--max-concurrent-downloads",
+        action="store",
+        default=2,
+        help="Set maximum number of parallel downloads.",
+        metavar="MAX_WORKERS",
+        dest="max_workers",
+        type=int,
+    )
+
+    parser.add_argument(
+        "-t",
+        "--update-interval",
+        action="store",
+        default=60 * 10,
+        help="Set the update interval for checking new story in seconds. (Default: 10m)",
+        metavar="INTERVAL",
+        dest="interval",
+        type=int,
+    )
+
+    parser.add_argument(
+        "--sleep-interval",
+        action="store",
+        default=1,
+        help="Sleep between downloads in seconds. (Default: 1s)",
+        metavar="INTERVAL",
+        dest="sleep_interval",
+        type=int,
+    )
+
+    parser.add_argument(
+        "-q",
+        "--quiet",
+        action="store_true",
+        help="Do not print anything except errors to the console.",
+    )
+
+    if len(sys.argv) == 1:
+        parser.print_help()
+        sys.exit(1)
+
+    return parser.parse_args()
```

### Comparing `snapchat-dlp-1.5.2/snapchat_dlp/downloader.py` & `snapchat-dlp-1.5.8/snapchat_dlp/downloader.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-"""File Downlaoder for snapchat_dlp."""
-import os
-import time
-
-import requests
-from loguru import logger
-
-
-def download_url(url: str, dest: str, sleep_interval: int):
-    """Download URL to destionation path.
-
-    Args:
-        url (str): url to download
-        dest (str): absolute path to destination
-
-    Raises:
-        response.raise_for_status: if response is 4** or 50*
-        FileExistsError: if file is already downloaded
-    """
-    if len(os.path.dirname(dest)) > 0:
-        os.makedirs(os.path.dirname(dest), exist_ok=True)
-
-    """Rate limiting."""
-    time.sleep(sleep_interval)
-
-    try:
-        response = requests.get(url, stream=True, timeout=10)
-    except requests.exceptions.ConnectTimeout:
-        response = requests.get(url, stream=True, timeout=10)
-
-    if response.status_code != requests.codes.get("ok"):
-        raise response.raise_for_status()
-
-    # This could mabye be used for a --verify argument?
-    # if os.path.isfile(dest) and os.path.getsize(dest) == response.headers.get(
-    #     "content-length"
-    # ):
-    #     raise FileExistsError
-
-    if os.path.isfile(dest) and os.path.getsize(dest) == 0:
-        os.remove(dest)
-    try:
-        with open(dest, "xb") as handle:
-            try:
-                for data in response.iter_content(chunk_size=4194304):
-                    handle.write(data)
-                handle.close()
-            except requests.exceptions.RequestException as e:
-                logger.error(e)
-    except FileExistsError as e:
-        pass
+"""File Downlaoder for snapchat_dlp."""
+import os
+import time
+
+import requests
+from loguru import logger
+
+
+def download_url(url: str, dest: str, sleep_interval: int):
+    """Download URL to destionation path.
+
+    Args:
+        url (str): url to download
+        dest (str): absolute path to destination
+
+    Raises:
+        response.raise_for_status: if response is 4** or 50*
+        FileExistsError: if file is already downloaded
+    """
+    if len(os.path.dirname(dest)) > 0:
+        os.makedirs(os.path.dirname(dest), exist_ok=True)
+
+    """Rate limiting."""
+    time.sleep(sleep_interval)
+
+    try:
+        response = requests.get(url, stream=True, timeout=10)
+    except requests.exceptions.ConnectTimeout:
+        response = requests.get(url, stream=True, timeout=10)
+
+    if response.status_code != requests.codes.get("ok"):
+        raise response.raise_for_status()
+
+    # This could mabye be used for a --verify argument?
+    # if os.path.isfile(dest) and os.path.getsize(dest) == response.headers.get(
+    #     "content-length"
+    # ):
+    #     raise FileExistsError
+
+    if os.path.isfile(dest) and os.path.getsize(dest) == 0:
+        os.remove(dest)
+    try:
+        with open(dest, "xb") as handle:
+            try:
+                for data in response.iter_content(chunk_size=4194304):
+                    handle.write(data)
+                handle.close()
+            except requests.exceptions.RequestException as e:
+                logger.error(e)
+    except FileExistsError as e:
+        pass
```

### Comparing `snapchat-dlp-1.5.2/snapchat_dlp/snapchat_dlp.py` & `snapchat-dlp-1.5.8/snapchat_dlp/snapchat_dlp.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,145 +1,148 @@
-"""The Main Snapchat Downloader Class."""
-import concurrent.futures
-import json
-import os
-import re
-
-import requests
-from loguru import logger
-
-from snapchat_dlp.downloader import download_url
-from snapchat_dlp.utils import APIResponseError
-from snapchat_dlp.utils import dump_response
-from snapchat_dlp.utils import MEDIA_TYPE
-from snapchat_dlp.utils import NoStoriesFound
-from snapchat_dlp.utils import strf_time
-from snapchat_dlp.utils import UserNotFoundError
-
-
-class SnapchatDL:
-    """Interact with Snapchat API to download story."""
-
-    def __init__(
-        self,
-        directory_prefix=".",
-        max_workers=2,
-        limit_story=-1,
-        sleep_interval=1,
-        quiet=False,
-        dump_json=False,
-    ):
-        self.directory_prefix = os.path.abspath(os.path.normpath(directory_prefix))
-        self.max_workers = max_workers
-        self.limit_story = limit_story
-        self.sleep_interval = sleep_interval
-        self.quiet = quiet
-        self.dump_json = dump_json
-        self.endpoint_web = "https://story.snapchat.com/@{}"
-        self.regexp_web_json = (
-            r'<script\s*id="__NEXT_DATA__"\s*type="application\/json">([^<]+)<\/script>'
-        )
-        self.reaponse_ok = requests.codes.get("ok")
-
-    def _api_response(self, username):
-        web_url = self.endpoint_web.format(username)
-        return requests.get(web_url).text
-
-    def _web_fetch_story(self, username):
-        """Download user stories from Web.
-
-        Args:
-            username (str): Snapchat `username`
-
-        Raises:
-            APIResponseError: API Error
-
-        Returns:
-            (dict, dict): user_info, stories
-        """
-        response = self._api_response(username)
-        response_json_raw = re.findall(self.regexp_web_json, response)
-
-        try:
-            response_json = json.loads(response_json_raw[0])
-
-            def util_web_user_info(content: dict):
-                if "userProfile" in content["props"]["pageProps"]:
-                    user_profile = content["props"]["pageProps"]["userProfile"]
-                    field_id = user_profile["$case"]
-                    return user_profile[field_id]
-                else:
-                    raise UserNotFoundError(f"Could not find Snapchat user {username}")
-
-            def util_web_story(content: dict):
-                if "story" in content["props"]["pageProps"]:
-                    return content["props"]["pageProps"]["story"]["snapList"]
-                return list()
-
-            user_info = util_web_user_info(response_json)
-            stories = util_web_story(response_json)
-            return stories, user_info
-        except (IndexError, KeyError, ValueError):
-            raise APIResponseError
-
-    def download(self, username):
-        """Download Snapchat Story for `username`.
-
-        Args:
-            username (str): Snapchat `username`
-
-        Returns:
-            [bool]: story downloader
-        """
-        story_download_count = 0
-        stories, snap_user = self._web_fetch_story(username)
-
-        if len(stories) == 0:
-            if self.quiet is False:
-                logger.info("\033[91m{}\033[0m has no stories".format(username))
-
-            raise NoStoriesFound
-
-        if self.limit_story > -1:
-            stories = stories[0 : self.limit_story]
-
-        logger.info("[+] {} has {} stories".format(username, len(stories)))
-
-        executor = concurrent.futures.ThreadPoolExecutor(max_workers=self.max_workers)
-        try:
-            for media in stories:
-                snap_id = media["snapId"]["value"]
-                media_url = media["snapUrls"]["mediaUrl"]
-                media_type = media["snapMediaType"]
-                timestamp = int(media["timestampInSec"]["value"])
-                date_str = strf_time(timestamp, "%Y-%m-%d")
-
-                dir_name = os.path.join(self.directory_prefix, username, date_str)
-
-                filename = strf_time(timestamp, "%Y-%m-%d_%H-%M-%S {} {}.{}").format(
-                    snap_id, username, MEDIA_TYPE[media_type]
-                )
-
-                if self.dump_json:
-                    filename_json = os.path.join(dir_name, filename + ".json")
-                    media_json = dict(media)
-                    media_json["snapUser"] = snap_user
-                    dump_response(media_json, filename_json)
-
-                media_output = os.path.join(dir_name, filename)
-
-                # # Check if file exists
-                if not os.path.isfile(media_output):
-                    story_download_count += 1
-
-                executor.submit(
-                    download_url, media_url, media_output, self.sleep_interval
-                )
-
-        except KeyboardInterrupt:
-            executor.shutdown(wait=False)
-        executor.shutdown(wait=True)
-        logger.info(
-            "[✔] {}'s stories downloaded, downloaded {} this session, {} already existed".format(
-                username, story_download_count, len(stories) - story_download_count
-            )
-        )
+"""The Main Snapchat Downloader Class."""
+import concurrent.futures
+import json
+import os
+import re
+
+import requests
+from loguru import logger
+
+from snapchat_dlp.downloader import download_url
+from snapchat_dlp.utils import APIResponseError
+from snapchat_dlp.utils import dump_response
+from snapchat_dlp.utils import MEDIA_TYPE
+from snapchat_dlp.utils import NoStoriesFound
+from snapchat_dlp.utils import strf_time
+from snapchat_dlp.utils import UserNotFoundError
+
+
+class SnapchatDL:
+    """Interact with Snapchat API to download story."""
+
+    def __init__(
+        self,
+        directory_prefix=".",
+        max_workers=2,
+        limit_story=-1,
+        sleep_interval=1,
+        quiet=False,
+        dump_json=False,
+    ):
+        self.directory_prefix = os.path.abspath(os.path.normpath(directory_prefix))
+        self.max_workers = max_workers
+        self.limit_story = limit_story
+        self.sleep_interval = sleep_interval
+        self.quiet = quiet
+        self.dump_json = dump_json
+        self.endpoint_web = "https://story.snapchat.com/@{}"
+        self.regexp_web_json = (
+            r'<script\s*id="__NEXT_DATA__"\s*type="application\/json">([^<]+)<\/script>'
+        )
+        self.reaponse_ok = requests.codes.get("ok")
+
+    def _api_response(self, username):
+        web_url = self.endpoint_web.format(username)
+        return requests.get(web_url).text
+
+    def _web_fetch_story(self, username):
+        """Download user stories from Web.
+
+        Args:
+            username (str): Snapchat `username`
+
+        Raises:
+            APIResponseError: API Error
+
+        Returns:
+            (dict, dict): user_info, stories
+        """
+        response = self._api_response(username)
+        response_json_raw = re.findall(self.regexp_web_json, response)
+
+        try:
+            response_json = json.loads(response_json_raw[0])
+
+            def util_web_user_info(content: dict):
+                if "userProfile" in content["props"]["pageProps"]:
+                    user_profile = content["props"]["pageProps"]["userProfile"]
+                    field_id = user_profile["$case"]
+                    return user_profile[field_id]
+                else:
+                    raise UserNotFoundError(f"Could not find Snapchat user {username}")
+
+            def util_web_story(content: dict):
+                if "story" in content["props"]["pageProps"]:
+                    return content["props"]["pageProps"]["story"]["snapList"]
+                return list()
+
+            user_info = util_web_user_info(response_json)
+            stories = util_web_story(response_json)
+            return stories, user_info
+        except (IndexError, KeyError, ValueError):
+            raise APIResponseError
+        except UserNotFoundError as e:
+            print(f"User {username} not found. Check the spelling, or that it is a public profile.")
+            print(e)
+
+    def download(self, username):
+        """Download Snapchat Story for `username`.
+
+        Args:
+            username (str): Snapchat `username`
+
+        Returns:
+            [bool]: story downloader
+        """
+        story_download_count = 0
+        stories, snap_user = self._web_fetch_story(username)
+
+        if len(stories) == 0:
+            if self.quiet is False:
+                logger.info("\033[91m{}\033[0m has no stories".format(username))
+            print("Found no stories. Could be a typo in the username, or the user does not have any published stories right now.")
+            # raise NoStoriesFound
+
+        if self.limit_story > -1:
+            stories = stories[0 : self.limit_story]
+
+        logger.info("[+] {} has {} stories".format(username, len(stories)))
+
+        executor = concurrent.futures.ThreadPoolExecutor(max_workers=self.max_workers)
+        try:
+            for media in stories:
+                snap_id = media["snapId"]["value"]
+                media_url = media["snapUrls"]["mediaUrl"]
+                media_type = media["snapMediaType"]
+                timestamp = int(media["timestampInSec"]["value"])
+                date_str = strf_time(timestamp, "%Y-%m-%d")
+
+                dir_name = os.path.join(self.directory_prefix, username, date_str)
+
+                filename = strf_time(timestamp, "%Y-%m-%d_%H-%M-%S {} {}.{}").format(
+                    snap_id, username, MEDIA_TYPE[media_type]
+                )
+
+                if self.dump_json:
+                    filename_json = os.path.join(dir_name, filename + ".json")
+                    media_json = dict(media)
+                    media_json["snapUser"] = snap_user
+                    dump_response(media_json, filename_json)
+
+                media_output = os.path.join(dir_name, filename)
+
+                # # Check if file exists
+                if not os.path.isfile(media_output):
+                    story_download_count += 1
+
+                executor.submit(
+                    download_url, media_url, media_output, self.sleep_interval
+                )
+
+        except KeyboardInterrupt:
+            executor.shutdown(wait=False)
+        executor.shutdown(wait=True)
+        logger.info(
+            "[✔] {}'s stories downloaded, downloaded {} this session, {} already existed".format(
+                username, story_download_count, len(stories) - story_download_count
+            )
+        )
```

### Comparing `snapchat-dlp-1.5.2/snapchat_dlp/utils.py` & `snapchat-dlp-1.5.8/snapchat_dlp/utils.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,169 +1,169 @@
-"""Utility functions for snapchat_dlp."""
-import json
-import os
-import re
-from argparse import Namespace
-from datetime import datetime
-
-from loguru import logger
-
-
-MEDIA_TYPE = ["jpg", "mp4"]
-
-
-class NoStoriesFound(Exception):
-    """No stories found."""
-
-    pass
-
-
-class APIResponseError(Exception):
-    """Invalid API Response"""
-
-    pass
-
-
-class UserNotFoundError(Exception):
-    """User not found"""
-
-    pass
-
-
-def strf_time(timestamp, format_str):
-    """Format unix timestamp to custom format.
-
-    Args:
-        timestamp (int): unix timestamp
-        format_str (str): valid python date time format
-
-    Returns:
-        str: timestamp formatted to custom format.
-    """
-    return datetime.utcfromtimestamp(timestamp).strftime(format_str)
-
-
-def valid_username(username):
-    """Validate Username.
-
-    Args:
-        username (str): Snapchat Username
-
-    Returns:
-        bool: True if username is valid.
-    """
-    match = re.match(r"(?P<username>^[\-\w\.\_]{3,15}$)", username)
-    if match is None:
-        return False
-
-    return match and match.groupdict()["username"] == username
-
-
-def search_usernames(string: str) -> list:
-    """Return list of usernames found in a string.
-
-    Args:
-        string (str): string to search for usernames
-
-    Returns:
-        list: usernames found in string
-    """
-    return list(
-        sorted(
-            set(
-                [
-                    username
-                    for username in re.findall(
-                        r"https?://(?:story|www).snapchat.com/(?:[suad]+/|@)([\-\w\.\_]{3,15})",
-                        string,
-                    )
-                    if valid_username(username)
-                ]
-            )
-        )
-    )
-
-
-def use_batch_file(args: Namespace) -> list:
-    """Return list of usernames from file args.batch_file.
-
-    Args:
-        args (Namespace): argparse Namespace
-
-    Raises:
-        os.error: raises if batch_file not found
-
-    Returns:
-        list: usernames read from batch_file
-    """
-    usernames = list()
-    if args.batch_file is not None:
-        if os.path.isfile(args.batch_file) is False:
-            raise Exception(
-                logger.error("Invalid Batch File at {}".format(args.batch_file))
-            )
-
-        with open(args.batch_file, "r") as f:
-            for u in f.read().split("\n"):
-                username = u.strip()
-                if valid_username(username) and username not in usernames:
-                    usernames.append(username)
-
-    return usernames
-
-
-def use_prefix_dir(args: Namespace):
-    """Return dirnames as username from file args.scan_prefix.
-
-    Args:
-        args (Namespace): argparse Namespace
-
-    Returns:
-        list: usernames read from scan_prefix
-    """
-    usernames = list()
-    if args.scan_prefix:
-        for username in [
-            o
-            for o in os.listdir(args.save_prefix)
-            if os.path.isdir(os.path.join(args.save_prefix, o))
-        ]:
-            if username not in usernames and valid_username(username):
-                usernames.append(username)
-
-        if args.quiet is False:
-            logger.info(
-                "Added {} usernames from {}".format(len(usernames), args.save_prefix)
-            )
-
-    return list(sorted(set(usernames)))
-
-
-def dump_text_file(content: str, filepath: str):
-    """Write content to filepath using `tx` mode.
-
-    Args:
-        content (str): File content to write.
-        filepath (str): Filepath.
-
-    This will overwrite the file.
-    """
-    dirpath = os.path.dirname(filepath)
-
-    os.makedirs(dirpath, exist_ok=True)
-
-    if not os.path.isfile(filepath):
-        with open(filepath, "w+") as f:
-            f.write(content)
-
-
-def dump_response(content: dict, path: str):
-    """Save JSON file
-
-    Args:
-        content: JSON data
-        path: Path to save json
-
-    Returns:
-        None
-    """
-    dump_text_file(json.dumps(content), path)
+"""Utility functions for snapchat_dlp."""
+import json
+import os
+import re
+from argparse import Namespace
+from datetime import datetime
+
+from loguru import logger
+
+
+MEDIA_TYPE = ["jpg", "mp4"]
+
+
+class NoStoriesFound(Exception):
+    """No stories found."""
+
+    pass
+
+
+class APIResponseError(Exception):
+    """Invalid API Response"""
+
+    pass
+
+
+class UserNotFoundError(Exception):
+    """User not found"""
+
+    pass
+
+
+def strf_time(timestamp, format_str):
+    """Format unix timestamp to custom format.
+
+    Args:
+        timestamp (int): unix timestamp
+        format_str (str): valid python date time format
+
+    Returns:
+        str: timestamp formatted to custom format.
+    """
+    return datetime.utcfromtimestamp(timestamp).strftime(format_str)
+
+
+def valid_username(username):
+    """Validate Username.
+
+    Args:
+        username (str): Snapchat Username
+
+    Returns:
+        bool: True if username is valid.
+    """
+    match = re.match(r"(?P<username>^[\-\w\.\_]{3,15}$)", username)
+    if match is None:
+        return False
+
+    return match and match.groupdict()["username"] == username
+
+
+def search_usernames(string: str) -> list:
+    """Return list of usernames found in a string.
+
+    Args:
+        string (str): string to search for usernames
+
+    Returns:
+        list: usernames found in string
+    """
+    return list(
+        sorted(
+            set(
+                [
+                    username
+                    for username in re.findall(
+                        r"https?://(?:story|www).snapchat.com/(?:[suad]+/|@)([\-\w\.\_]{3,15})",
+                        string,
+                    )
+                    if valid_username(username)
+                ]
+            )
+        )
+    )
+
+
+def use_batch_file(args: Namespace) -> list:
+    """Return list of usernames from file args.batch_file.
+
+    Args:
+        args (Namespace): argparse Namespace
+
+    Raises:
+        os.error: raises if batch_file not found
+
+    Returns:
+        list: usernames read from batch_file
+    """
+    usernames = list()
+    if args.batch_file is not None:
+        if os.path.isfile(args.batch_file) is False:
+            raise Exception(
+                logger.error("Invalid Batch File at {}".format(args.batch_file))
+            )
+
+        with open(args.batch_file, "r") as f:
+            for u in f.read().split("\n"):
+                username = u.strip()
+                if valid_username(username) and username not in usernames:
+                    usernames.append(username)
+
+    return usernames
+
+
+def use_prefix_dir(args: Namespace):
+    """Return dirnames as username from file args.scan_prefix.
+
+    Args:
+        args (Namespace): argparse Namespace
+
+    Returns:
+        list: usernames read from scan_prefix
+    """
+    usernames = list()
+    if args.scan_prefix:
+        for username in [
+            o
+            for o in os.listdir(args.save_prefix)
+            if os.path.isdir(os.path.join(args.save_prefix, o))
+        ]:
+            if username not in usernames and valid_username(username):
+                usernames.append(username)
+
+        if args.quiet is False:
+            logger.info(
+                "Added {} usernames from {}".format(len(usernames), args.save_prefix)
+            )
+
+    return list(sorted(set(usernames)))
+
+
+def dump_text_file(content: str, filepath: str):
+    """Write content to filepath using `tx` mode.
+
+    Args:
+        content (str): File content to write.
+        filepath (str): Filepath.
+
+    This will overwrite the file.
+    """
+    dirpath = os.path.dirname(filepath)
+
+    os.makedirs(dirpath, exist_ok=True)
+
+    if not os.path.isfile(filepath):
+        with open(filepath, "w+") as f:
+            f.write(content)
+
+
+def dump_response(content: dict, path: str):
+    """Save JSON file
+
+    Args:
+        content: JSON data
+        path: Path to save json
+
+    Returns:
+        None
+    """
+    dump_text_file(json.dumps(content), path)
```

### Comparing `snapchat-dlp-1.5.2/snapchat_dlp.egg-info/SOURCES.txt` & `snapchat-dlp-1.5.8/snapchat_dlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `snapchat-dlp-1.5.2/tests/mock_data/api-error.html` & `snapchat-dlp-1.5.8/tests/mock_data/api-error.html`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-
-<!DOCTYPE html><html prefix="og: https://ogp.me/ns#" dir="0" lang="en-US"><head><link data-react-helmet="true" rel="canonical" href="https://www.snapchat.com/add/invalidusername"/><meta data-react-helmet="true" name="description" content="Mrunu is on Snapchat!"/><meta data-react-helmet="true" name="apple-itunes-app" content="app-id=447188370, app-argument=https://www.snapchat.com/add/invalidusername"/><meta data-react-helmet="true" name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1.0, user-scalable=0"/><meta data-react-helmet="true" name="metrics-page-name" content="User_Profile.PublicProfile"/><meta data-react-helmet="true" property="og:title" content="invalidusername on Snapchat"/><meta data-react-helmet="true" property="og:type" content="video.other"/><meta data-react-helmet="true" property="og:url" content="https://story.snapchat.com/u/invalidusername"/><meta data-react-helmet="true" property="og:image" content="https://story.snapchat.com/@invalidusername/preview/facebook.png"/><meta data-react-helmet="true" property="og:locale:alternate" content="ar_AA"/><meta data-react-helmet="true" property="og:locale:alternate" content="da_DK"/><meta data-react-helmet="true" property="og:locale:alternate" content="de_DK"/><meta data-react-helmet="true" property="og:locale:alternate" content="en_GB"/><meta data-react-helmet="true" property="og:locale:alternate" content="en_US"/><meta data-react-helmet="true" property="og:locale:alternate" content="es_ES"/><meta data-react-helmet="true" property="og:locale:alternate" content="es_MX"/><meta data-react-helmet="true" property="og:locale:alternate" content="fi_FI"/><meta data-react-helmet="true" property="og:locale:alternate" content="fr_FR"/><meta data-react-helmet="true" property="og:locale:alternate" content="it_IT"/><meta data-react-helmet="true" property="og:locale:alternate" content="ja_JP"/><meta data-react-helmet="true" property="og:locale:alternate" content="nb_NO"/><meta data-react-helmet="true" property="og:locale:alternate" content="nl_NL"/><meta data-react-helmet="true" property="og:locale:alternate" content="pt_BR"/><meta data-react-helmet="true" property="og:locale:alternate" content="sv_SE"/><meta data-react-helmet="true" property="og:image:width" content="1200"/><meta data-react-helmet="true" property="og:image:height" content="628"/><meta data-react-helmet="true" property="og:site_name" content="Snapchat"/><meta data-react-helmet="true" property="fb:app_id" content="394343577431007"/><meta data-react-helmet="true" property="fb:admins" content="1349731971"/><meta data-react-helmet="true" property="twitter:card" content="summary_large_image"/><meta data-react-helmet="true" property="twitter:site" content="@Snapchat"/><meta data-react-helmet="true" property="twitter:title" content="invalidusername on Snapchat"/><meta data-react-helmet="true" property="twitter:image" content="https://story.snapchat.com/@invalidusername/preview/twitter.png"/><script data-react-helmet="true" async="" src="https://www.google-analytics.com/analytics.js"></script><script data-react-helmet="true">
-    window.ga=window.ga||function(){(ga.q = ga.q || []).push(arguments)};
-    ga.l=+new Date;
-    ga('create','UA-41740027-40', 'auto');
-    ga('send','pageview', location.pathname);
-  </script><style data-react-helmet="true">html {
-          height: 100%;
-          box-sizing: border-box;
-         }
-
-         body {
-          margin: 0;
-          height: 100%;
-          background: #121314;
-          font-family: Avenir Next, Helvetica, sans-serif;
-          -webkit-text-fill-color: currentcolor;
-         }
-
-         #__next, #root {
-          height: 100%;
-         }
-
-         *, *:before, *:after {
-          box-sizing: inherit;
-         }
-
-         button {
-          -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
-          -webkit-tap-highlight-color: transparent;
-          -webkit-user-select: none;
-          -khtml-user-select: none;
-          -moz-user-select: none;
-          -ms-user-select: none;
-          user-select: none;
-         }
-         </style><title data-react-helmet="true">Mrunu (@invalidusername) on Snapchat</title><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><noscript data-n-css=""></noscript><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/049823d6.8b03ce304b0e44456f30.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/22.ca59e6299b825dc862b0.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/webpack-edb54b561e62fb294b85.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/framework.efe182f2d62be1d8151a.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/c408797459d80c128d5e47906020fa02c3ea7a51.cdf474846c815ffe556c.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/f6078781a05fe1bcb0902d23dbbb2662c8d200b3.0cb66906a1ea3f804368.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/main-69ec1f1dba14cd9f620a.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/c1468a61a92675d836a3000bab1334fb54fd20a9.074f204d663a13469e0b.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/d241c1e27ffe07c251e6f8ab09888e7ecf8ae8dc.b20db949b32dafefad5c.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/d4fc9bc7fce3fa7dbb251df097e4d60e4f4a3ec9.6a57a5151732d06fa88a.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/pages/_app-9a2167e8d8d9d9f101c9.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/29107295.be25f8bc8bdde59f114d.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/641167d64809277a1b9199554823a0e631b3bff2.b1423abff274817ff848.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/96c0058ea2ce58b3f27756fc0d0be33ac3f6361c.4360e309b36814bc7496.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/64dd010a9368940fc41206bc54dfee6183397831.1358f9c5b56d2322e06e.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/bd9739576daf9a5525e7028695825e8d0c29e04c.65c9b0762abe3d67e2ce.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/f2142e6c893e00c2f1a27f144791418e507fc12c.1ef92cfd6920c8f93e61.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/e2ef7edf3a7e66ae27a9d163772f8c722ad47684.7e5591f9407dd7837830.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/61f94ab364ffeaf810caabbb5e8c59d41b273801.6e578c39745032b54013.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/d01c7d3028b0c7a5252ef883c5a43f5f0e747f01.5c6a4b590ccfff6d1784.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/pages/@/%5Busername%5D-19264ae3ee802be2dc6d.js" as="script"/></head><body id="root"><div id="__next"><style data-emotion="css-global cqw65k">@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.ttf") format("truetype");font-weight:100;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.ttf") format("truetype");font-weight:100;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.ttf") format("truetype");font-weight:200;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.ttf") format("truetype");font-weight:200;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Regular.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Regular.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Regular.ttf") format("truetype");font-weight:300;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Italic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Italic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Italic.ttf") format("truetype");font-weight:300;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Medium.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Medium.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Medium.ttf") format("truetype");font-weight:400;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-MediumItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-MediumItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-MediumItalic.ttf") format("truetype");font-weight:400;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-DemiBold.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-DemiBold.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-DemiBold.ttf") format("truetype");font-weight:500;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-DemiBoldItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-DemiBoldItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-DemiBoldItalic.ttf") format("truetype");font-weight:500;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Bold.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Bold.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Bold.ttf") format("truetype");font-weight:600;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.ttf") format("truetype");font-weight:600;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Bold.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Bold.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Bold.ttf") format("truetype");font-weight:700;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.ttf") format("truetype");font-weight:700;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Heavy.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Heavy.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Heavy.ttf") format("truetype");font-weight:800;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.ttf") format("truetype");font-weight:800;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Heavy.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Heavy.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Heavy.ttf") format("truetype");font-weight:900;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.ttf") format("truetype");font-weight:900;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Thin.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Thin.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Thin.ttf") format("truetype");font-weight:100;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ThinItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ThinItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ThinItalic.ttf") format("truetype");font-weight:100;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Extralight.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Extralight.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Extralight.ttf") format("truetype");font-weight:200;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ExtralightItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ExtralightItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ExtralightItalic.ttf") format("truetype");font-weight:200;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Light.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Light.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Light.ttf") format("truetype");font-weight:300;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-LightItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-LightItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-LightItalic.ttf") format("truetype");font-weight:300;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Regular.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Regular.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Regular.ttf") format("truetype");font-weight:400;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-RegularItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-RegularItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-RegularItalic.ttf") format("truetype");font-weight:400;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Medium.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Medium.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Medium.ttf") format("truetype");font-weight:500;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-MediumItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-MediumItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-MediumItalic.ttf") format("truetype");font-weight:500;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Semibold.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Semibold.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Semibold.ttf") format("truetype");font-weight:600;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SemiboldItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SemiboldItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SemiboldItalic.ttf") format("truetype");font-weight:600;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Bold.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Bold.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Bold.ttf") format("truetype");font-weight:700;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BoldItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BoldItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BoldItalic.ttf") format("truetype");font-weight:700;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Black.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Black.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Black.ttf") format("truetype");font-weight:800;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BlackItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BlackItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BlackItalic.ttf") format("truetype");font-weight:800;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Super.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Super.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Super.ttf") format("truetype");font-weight:900;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SuperItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SuperItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SuperItalic.ttf") format("truetype");font-weight:900;font-style:italic;font-display:block;}</style></div><script id="__NEXT_DATA_" type="application/json">{"props":{"pageProps":{"googleAnalyticsPropertyId":"UA-41740027-40","localizedMessages":{"default":{"+9d+q7":"Nonprofit Organization","+ByJA/":"Stories","+hwkQQ":"Film / TV","+lhElX":"Copyright infringement","+o8gM9":"Kit","/Xkr+t":"by {creatorDisplayName}","/dF4HW":"Spotlight","/tNMyW":"Download","/vdS3s":"Download Snapchat to Watch Now","04qzmG":"You will now be taken to the next Snap - press 'Close' to do this right away or we will continue automatically in 10 seconds.","0FP975":"Post to Spotlight","0Y6c0W":"Restaurant Chain","0YKDxr":"Photographer","0dJz6S":"Threatening, violent, or concerning","0uHjye":"Share this Snap","1PzCdm":"It asks for or threatens to post inappropriate Snaps","1V8Uma":"Public Figure","1egAGi":"Movie Character","1kdcl2":"Media / News Company","2LLiYb":"Close","2V40yT":"More Options","2l730k":"Film / TV Personality","4V5k0y":"Support","5HsSrO":"I just don't like it","5XW8Zd":"{subscriberCount} Subscribers","5m3Hu8":"I'm worried this Snapchatter might hurt themselves","5v6wP7":"Motivational Speaker","5zZGnG":"Writer","6yvoZD":"Sorry,","7BHw3h":"Religious Organization","7HP0Jf":"Coach","7XZM2L":"Business","7rVnIj":"Spotlight","7xehRy":"Producer","7yuYaU":"Businesses \u0026 Groups","8Sw4jY":"Report Snap","9NRv3Z":"Snapcodes","ATeDiR":"Thank you for reporting this Snap.","AbkQPs":"It's an invasion of privacy","AtLF/u":"This content was not found","CAgCZ5":"Nudity or sexual content","CJBFGo":"Politician","CVucIf":"Community Organization","DY4yHA":"Brand","EPBE+l":"Government Official","ESomE8":"Submit","Eqnt63":"{timeDifference}m ago","FDOu63":"Someone else is being bullied or harassed","Fsg136":"Episode {episodeNumber}","Ftta6c":"It's threatening a person or place","G7hRik":"Spotlight is not available in your location","GJZs5E":"It's spam","GVLbZP":"Stories","GaNuM2":"Best of Spotlight","Gh1a/j":"Food Professional","GssbOn":"Product","Gvuqme":"It's an inappropriate Snap of someone else","HLxWNM":"It sells or promotes inappropriate Snaps","HVgZaB":"Creator","HkaOsh":"Open your Snapchat","I1rLjL":"Ads","I6sovq":"Political Organization","IWKERN":"Fashion Model","JbCR5V":"This content is not available","Ju77ns":"Comedian","MDthgV":"Sports League","MN6Znh":"Watch more in Snapchat","MUzWB7":"Please provide your Snapchat username if you have one, and the email associated with your account","N7Wq/c":"Violent or disturbing","N7iI/k":"Download Snapchat to find more","NXPVkv":"Company / Enterprise","P6YGQz":"Open in Snapchat","PQcLi/":"Service","PyzdXL":"Cancel","Q4RuCH":"Maps","Q71IbU":"Government Organization","QdGWFE":"Season {seasonNumber}","RJo0Z3":"Harassment or Hate speech","RmE5lP":"Lifestyle Influencer","RtNy71":"Musician / Band","SCe4GQ":"Film Director","SVOJKh":"Video Game","SgFTtk":"Up next","TNK/W/":"Lenses","Tm6yFt":"Download Snapchat","UIZTzu":"It's attempting to buy or sell drugs or weapons","Uk55sM":"Add me on Snapchat!","VRmDFV":"Snap Reported","VZQx67":"This Snap is no longer available","VjDaWB":"Watch more from {publisherTitle}","W07I8V":"Share {username}'s Snap","WGtpBM":"People","WyUwHm":"They are pretending to be me","XbXoMR":"Actor","YhMtYd":"Spectacles","Yt2+ye":"My Story","ZPrHrl":"Internet Company","ZViZgq":"Traveler","ZlJO0Q":"Apparel / Fashion","ZvzVyN":"Top Lenses","aSXQy0":"Sports Personality","ah6l3c":"Charity / Cause","ais8eK":"Group","by2dgE":"News Personality","dAksd9":"Journalist","dItw6q":"Dancer","dJDu/3":"Entrepreneur","dkWyPr":"Vlogger / Blogger","fPIy5v":"Retail Company","fxAji7":"Filters \u0026 Lenses","hPxDQC":"Video Game Creator","jWa4OT":"College / University","jqpH+5":"Is there any more information you want to share about this Snap?","kNCf90":"Products \u0026 Brands","kzoiEX":"{timeDifference}h ago","l1fnUG":"Scientist","lbui+i":"It's hate speech targeting me or another group","nbiOpp":"Lens Studio","ojrZ4G":"Download","pCK8FJ":"Artist","pPIiOl":"{subscriberCount} Subscribers","rL8HYz":"Professional Gamer","rLGZZX":"Just now","rNVPnk":"It's an inappropriate Snap of me","rrdPgT":"Store","rsYMnU":"Episodes","sRM8i5":"Why do you want to report this Snap?","sVcU8q":"Posted to Snap Map","tYFb/P":"Spotlight","vTd+a8":"I'm being bullied or harassed","vqdER6":"Fitness Professional","wVfxbD":"Political Candidate","wpLx7z":"Lens Creator","x1C/5K":"Person","x4F6zb":"Report Snap","xLaO8v":"Health / Beauty","yT6a3h":"In this Snap","ys7Y26":"Athlete","zExXNB":"Sports Team"},"+9d+q7":"Nonprofit Organization","+ByJA/":"Stories","+hwkQQ":"Film / TV","+lhElX":"Copyright infringement","+o8gM9":"Kit","/Xkr+t":"by {creatorDisplayName}","/dF4HW":"Spotlight","/tNMyW":"Download","/vdS3s":"Download Snapchat to Watch Now","04qzmG":"You will now be taken to the next Snap - press 'Close' to do this right away or we will continue automatically in 10 seconds.","0FP975":"Post to Spotlight","0Y6c0W":"Restaurant Chain","0YKDxr":"Photographer","0dJz6S":"Threatening, violent, or concerning","0uHjye":"Share this Snap","1PzCdm":"It asks for or threatens to post inappropriate Snaps","1V8Uma":"Public Figure","1egAGi":"Movie Character","1kdcl2":"Media / News Company","2LLiYb":"Close","2V40yT":"More Options","2l730k":"Film / TV Personality","4V5k0y":"Support","5HsSrO":"I just don't like it","5XW8Zd":"{subscriberCount} Subscribers","5m3Hu8":"I'm worried this Snapchatter might hurt themselves","5v6wP7":"Motivational Speaker","5zZGnG":"Writer","6yvoZD":"Sorry,","7BHw3h":"Religious Organization","7HP0Jf":"Coach","7XZM2L":"Business","7rVnIj":"Spotlight","7xehRy":"Producer","7yuYaU":"Businesses \u0026 Groups","8Sw4jY":"Report Snap","9NRv3Z":"Snapcodes","ATeDiR":"Thank you for reporting this Snap.","AbkQPs":"It's an invasion of privacy","AtLF/u":"This content was not found","CAgCZ5":"Nudity or sexual content","CJBFGo":"Politician","CVucIf":"Community Organization","DY4yHA":"Brand","EPBE+l":"Government Official","ESomE8":"Submit","Eqnt63":"{timeDifference}m ago","FDOu63":"Someone else is being bullied or harassed","Fsg136":"Episode {episodeNumber}","Ftta6c":"It's threatening a person or place","G7hRik":"Spotlight is not available in your location","GJZs5E":"It's spam","GVLbZP":"Stories","GaNuM2":"Best of Spotlight","Gh1a/j":"Food Professional","GssbOn":"Product","Gvuqme":"It's an inappropriate Snap of someone else","HLxWNM":"It sells or promotes inappropriate Snaps","HVgZaB":"Creator","HkaOsh":"Open your Snapchat","I1rLjL":"Ads","I6sovq":"Political Organization","IWKERN":"Fashion Model","JbCR5V":"This content is not available","Ju77ns":"Comedian","MDthgV":"Sports League","MN6Znh":"Watch more in Snapchat","MUzWB7":"Please provide your Snapchat username if you have one, and the email associated with your account","N7Wq/c":"Violent or disturbing","N7iI/k":"Download Snapchat to find more","NXPVkv":"Company / Enterprise","P6YGQz":"Open in Snapchat","PQcLi/":"Service","PyzdXL":"Cancel","Q4RuCH":"Maps","Q71IbU":"Government Organization","QdGWFE":"Season {seasonNumber}","RJo0Z3":"Harassment or Hate speech","RmE5lP":"Lifestyle Influencer","RtNy71":"Musician / Band","SCe4GQ":"Film Director","SVOJKh":"Video Game","SgFTtk":"Up next","TNK/W/":"Lenses","Tm6yFt":"Download Snapchat","UIZTzu":"It's attempting to buy or sell drugs or weapons","Uk55sM":"Add me on Snapchat!","VRmDFV":"Snap Reported","VZQx67":"This Snap is no longer available","VjDaWB":"Watch more from {publisherTitle}","W07I8V":"Share {username}'s Snap","WGtpBM":"People","WyUwHm":"They are pretending to be me","XbXoMR":"Actor","YhMtYd":"Spectacles","Yt2+ye":"My Story","ZPrHrl":"Internet Company","ZViZgq":"Traveler","ZlJO0Q":"Apparel / Fashion","ZvzVyN":"Top Lenses","aSXQy0":"Sports Personality","ah6l3c":"Charity / Cause","ais8eK":"Group","by2dgE":"News Personality","dAksd9":"Journalist","dItw6q":"Dancer","dJDu/3":"Entrepreneur","dkWyPr":"Vlogger / Blogger","fPIy5v":"Retail Company","fxAji7":"Filters \u0026 Lenses","hPxDQC":"Video Game Creator","jWa4OT":"College / University","jqpH+5":"Is there any more information you want to share about this Snap?","kNCf90":"Products \u0026 Brands","kzoiEX":"{timeDifference}h ago","l1fnUG":"Scientist","lbui+i":"It's hate speech targeting me or another group","nbiOpp":"Lens Studio","ojrZ4G":"Download","pCK8FJ":"Artist","pPIiOl":"{subscriberCount} Subscribers","rL8HYz":"Professional Gamer","rLGZZX":"Just now","rNVPnk":"It's an inappropriate Snap of me","rrdPgT":"Store","rsYMnU":"Episodes","sRM8i5":"Why do you want to report this Snap?","sVcU8q":"Posted to Snap Map","tYFb/P":"Spotlight","vTd+a8":"I'm being bullied or harassed","vqdER6":"Fitness Professional","wVfxbD":"Political Candidate","wpLx7z":"Lens Creator","x1C/5K":"Person","x4F6zb":"Report Snap","xLaO8v":"Health / Beauty","yT6a3h":"In this Snap","ys7Y26":"Athlete","zExXNB":"Sports Team"},"lenses":[],"curatedHighlights":[{"storyType":3,"storyTapId":"0","snapList":[{"snapIndex":0,"snapMediaType":0,"snapId":{"value":""},"snapUrls":{"mediaUrl":"https://cf-st.sc-cdn.net/d/Cg5MaQODMG3TnzwDo9KIa.400.IRZXSOY?uc=12","mediaPreviewUrl":{"value":"https://cf-st.sc-cdn.net/d/Cg5MaQODMG3TnzwDo9KIa.410.IRZXSOY?uc=12"}},"timestampInSec":{"value":"1606531630"}},{"snapIndex":1,"snapMediaType":0,"snapId":{"value":""},"snapUrls":{"mediaUrl":"https://cf-st.sc-cdn.net/d/uxOSCj5RgvtbPc1WJFZE4.400.IRZXSOY?uc=12","mediaPreviewUrl":{"value":"https://cf-st.sc-cdn.net/d/uxOSCj5RgvtbPc1WJFZE4.410.IRZXSOY?uc=12"}},"timestampInSec":{"value":"1605705190"}}],"storyId":{"value":""},"storyTitle":{"value":""},"thumbnailUrl":{"value":"https://cf-st.sc-cdn.net/d/Cg5MaQODMG3TnzwDo9KIa.410.IRZXSOY?uc=12"}}],"spotlightHighlights":[],"spotlightHighlightsMetadata":[],"viewerInfo":{"country":"IN","locale":"en_US"},"localization":{"direction":0},"pageLinks":{"oneLinkUrl":"https://click.snapchat.com/aVHG?pid=snapchat_download_page\u0026af_dp=https://www.snapchat.com/add/invalidusername?sc_referrer%3Dweb\u0026af_web_dp=https://snapchat.com/download?purpose%3Dweb_stories","snapchatCanonicalUrl":"https://www.snapchat.com/add/invalidusername","canonicalUrl":"https://www.snapchat.com/add/invalidusername","snapcodeImageUrl":"https://app.snapchat.com/web/deeplink/snapcode?username=invalidusername\u0026type=SVG\u0026bitmoji=enable"},"pageMetadata":{"pageType":9,"pageTitle":"Mrunu (@invalidusername) on Snapchat","pageDescription":{"value":"Mrunu is on Snapchat!"}},"userProfile":{"$case":"publicProfileInfo","publicProfileInfo":{"username":"invalidusername","title":"Mrunu","snapcodeImageUrl":"https://app.snapchat.com/web/deeplink/snapcode?username=invalidusername\u0026type=SVG\u0026bitmoji=enable","badge":1,"categoryStringId":"public-profile-category-v3-people","subcategoryStringId":"public-profile-subcategory-v3-artist","subscriberCount":"874600","bio":"Welcome to my weird life ✨","websiteUrl":"https://youtube.com/c/GujjuUnicorn","profilePictureUrl":"https://cf-st.sc-cdn.net/aps/bolt/aHR0cHM6Ly9jZi1zdC5zYy1jZG4ubmV0L2QvdTVBZEFXVnV1RlVSNDNBQk5qRHVNP2JvPUVnMGFBQm9BTWdFRVNBSlFHV0FCJnVjPTI1._RS0,90_FMjpeg","address":"Mumbai, India, India","hasCuratedHighlights":true,"hasSpotlightHighlights":false,"mutableName":"","publisherType":"","squareHeroImageUrl":"","primaryColor":""}},"story":{"storyType":5,"storyTapId":"0","snapList":[{"snapIndex":0,"snapMediaType":1,"snapId":{"value":"1PgHW1XZSgWteDhyTiIFbgAAgcnlmYnB0ZWpiAXxms2FCAXxms17GAAAAAA"},"snapUrls":{"mediaUrl":"https://filesamples.com/samples/video/mp4/sample_640x360.mp4","mediaPreviewUrl":{"value":"https://s.sc-cdn.net/1d/5Wv7rx8leVHNTyY454OlnCjZDCNqDQoW7y7eUU1T1CY=/default/preview_overlay.jpg"}},"timestampInSec":{"value":"1633810603"}},{"snapIndex":1,"snapMediaType":0,"snapId":{"value":"1PgHW1XZSgWteDhyTiIFbgAAgZWZqZ2t2ZGN4AXxpJwZoAXxpJwRfAAAAAA"},"snapUrls":{"mediaUrl":"https://filesamples.com/samples/video/mp4/sample_640x360.mp4"},"timestampInSec":{"value":"1633851737"}},{"snapIndex":2,"snapMediaType":0,"snapId":{"value":"1PgHW1XZSgWteDhyTiIFbgAAgdGlyeXpodGx4AXxpR4jsAXxpR4XzAAAAAA"},"snapUrls":{"mediaUrl":"https://filesamples.com/samples/video/mp4/sample_640x360.mp4"},"timestampInSec":{"value":"1633853867"}},{"snapIndex":3,"snapMediaType":0,"snapId":{"value":"1PgHW1XZSgWteDhyTiIFbgAAgdnJlc2hjeWd5AXxqhQjjAXxqhQaeAAAAAA"},"snapUrls":{"mediaUrl":"https://filesamples.com/samples/video/mp4/sample_640x360.mp4"},"timestampInSec":{"value":"1633874675"}}],"storyId":{"value":"invalidusername"},"thumbnailUrl":{"value":"https://s.sc-cdn.net/1d/5Wv7rx8leVHNTyY454OlnCjZDCNqDQoW7y7eUU1T1CY=/default/preview_overlay.jpg"}},"linkPreview":{"title":"invalidusername on Snapchat","description":"","canonicalUrl":"https://story.snapchat.com/u/invalidusername","twitterImage":{"url":"https://story.snapchat.com/@invalidusername/preview/twitter.png","size":{"width":1200,"height":600}},"facebookImage":{"url":"https://story.snapchat.com/@invalidusername/preview/facebook.png","size":{"width":1200,"height":628}}}},"status":0,"log":{"levels":{"TRACE":0,"DEBUG":1,"INFO":2,"WARN":3,"ERROR":4,"SILENT":5}}},"page":"/@/[username]","query":{"username":"@invalidusername"},"buildId":"23576-9b597984705a8ea2bff65ac8abd3eb5a984c976a","assetPrefix":"https://story.snapchat.com","isFallback":false,"dynamicIds":["gkwE","+51n","AC5g","DbP8","KIpE","LQDX","NuZu","aLx/","qmXy","sZW5","sZkf"],"gip":true,"appGip":true}</script><script nomodule="" src="https://story.snapchat.com/_next/static/chunks/polyfills-553aafd328e99d1ecd5e.js"></script><script async="" src="https://story.snapchat.com/_next/static/chunks/049823d6.8b03ce304b0e44456f30.js"></script><script async="" src="https://story.snapchat.com/_next/static/chunks/22.ca59e6299b825dc862b0.js"></script><script src="https://story.snapchat.com/_next/static/chunks/webpack-edb54b561e62fb294b85.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/framework.efe182f2d62be1d8151a.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/c408797459d80c128d5e47906020fa02c3ea7a51.cdf474846c815ffe556c.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/f6078781a05fe1bcb0902d23dbbb2662c8d200b3.0cb66906a1ea3f804368.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/main-69ec1f1dba14cd9f620a.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/c1468a61a92675d836a3000bab1334fb54fd20a9.074f204d663a13469e0b.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/d241c1e27ffe07c251e6f8ab09888e7ecf8ae8dc.b20db949b32dafefad5c.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/d4fc9bc7fce3fa7dbb251df097e4d60e4f4a3ec9.6a57a5151732d06fa88a.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/pages/_app-9a2167e8d8d9d9f101c9.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/29107295.be25f8bc8bdde59f114d.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/641167d64809277a1b9199554823a0e631b3bff2.b1423abff274817ff848.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/96c0058ea2ce58b3f27756fc0d0be33ac3f6361c.4360e309b36814bc7496.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/64dd010a9368940fc41206bc54dfee6183397831.1358f9c5b56d2322e06e.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/bd9739576daf9a5525e7028695825e8d0c29e04c.65c9b0762abe3d67e2ce.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/f2142e6c893e00c2f1a27f144791418e507fc12c.1ef92cfd6920c8f93e61.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/e2ef7edf3a7e66ae27a9d163772f8c722ad47684.7e5591f9407dd7837830.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/61f94ab364ffeaf810caabbb5e8c59d41b273801.6e578c39745032b54013.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/d01c7d3028b0c7a5252ef883c5a43f5f0e747f01.5c6a4b590ccfff6d1784.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/pages/@/%5Busername%5D-19264ae3ee802be2dc6d.js" async=""></script><script src="https://story.snapchat.com/_next/static/23576-9b597984705a8ea2bff65ac8abd3eb5a984c976a/_buildManifest.js" async=""></script><script src="https://story.snapchat.com/_next/static/23576-9b597984705a8ea2bff65ac8abd3eb5a984c976a/_ssgManifest.js" async=""></script></body></html>
+
+<!DOCTYPE html><html prefix="og: https://ogp.me/ns#" dir="0" lang="en-US"><head><link data-react-helmet="true" rel="canonical" href="https://www.snapchat.com/add/invalidusername"/><meta data-react-helmet="true" name="description" content="Mrunu is on Snapchat!"/><meta data-react-helmet="true" name="apple-itunes-app" content="app-id=447188370, app-argument=https://www.snapchat.com/add/invalidusername"/><meta data-react-helmet="true" name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1.0, user-scalable=0"/><meta data-react-helmet="true" name="metrics-page-name" content="User_Profile.PublicProfile"/><meta data-react-helmet="true" property="og:title" content="invalidusername on Snapchat"/><meta data-react-helmet="true" property="og:type" content="video.other"/><meta data-react-helmet="true" property="og:url" content="https://story.snapchat.com/u/invalidusername"/><meta data-react-helmet="true" property="og:image" content="https://story.snapchat.com/@invalidusername/preview/facebook.png"/><meta data-react-helmet="true" property="og:locale:alternate" content="ar_AA"/><meta data-react-helmet="true" property="og:locale:alternate" content="da_DK"/><meta data-react-helmet="true" property="og:locale:alternate" content="de_DK"/><meta data-react-helmet="true" property="og:locale:alternate" content="en_GB"/><meta data-react-helmet="true" property="og:locale:alternate" content="en_US"/><meta data-react-helmet="true" property="og:locale:alternate" content="es_ES"/><meta data-react-helmet="true" property="og:locale:alternate" content="es_MX"/><meta data-react-helmet="true" property="og:locale:alternate" content="fi_FI"/><meta data-react-helmet="true" property="og:locale:alternate" content="fr_FR"/><meta data-react-helmet="true" property="og:locale:alternate" content="it_IT"/><meta data-react-helmet="true" property="og:locale:alternate" content="ja_JP"/><meta data-react-helmet="true" property="og:locale:alternate" content="nb_NO"/><meta data-react-helmet="true" property="og:locale:alternate" content="nl_NL"/><meta data-react-helmet="true" property="og:locale:alternate" content="pt_BR"/><meta data-react-helmet="true" property="og:locale:alternate" content="sv_SE"/><meta data-react-helmet="true" property="og:image:width" content="1200"/><meta data-react-helmet="true" property="og:image:height" content="628"/><meta data-react-helmet="true" property="og:site_name" content="Snapchat"/><meta data-react-helmet="true" property="fb:app_id" content="394343577431007"/><meta data-react-helmet="true" property="fb:admins" content="1349731971"/><meta data-react-helmet="true" property="twitter:card" content="summary_large_image"/><meta data-react-helmet="true" property="twitter:site" content="@Snapchat"/><meta data-react-helmet="true" property="twitter:title" content="invalidusername on Snapchat"/><meta data-react-helmet="true" property="twitter:image" content="https://story.snapchat.com/@invalidusername/preview/twitter.png"/><script data-react-helmet="true" async="" src="https://www.google-analytics.com/analytics.js"></script><script data-react-helmet="true">
+    window.ga=window.ga||function(){(ga.q = ga.q || []).push(arguments)};
+    ga.l=+new Date;
+    ga('create','UA-41740027-40', 'auto');
+    ga('send','pageview', location.pathname);
+  </script><style data-react-helmet="true">html {
+          height: 100%;
+          box-sizing: border-box;
+         }
+
+         body {
+          margin: 0;
+          height: 100%;
+          background: #121314;
+          font-family: Avenir Next, Helvetica, sans-serif;
+          -webkit-text-fill-color: currentcolor;
+         }
+
+         #__next, #root {
+          height: 100%;
+         }
+
+         *, *:before, *:after {
+          box-sizing: inherit;
+         }
+
+         button {
+          -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
+          -webkit-tap-highlight-color: transparent;
+          -webkit-user-select: none;
+          -khtml-user-select: none;
+          -moz-user-select: none;
+          -ms-user-select: none;
+          user-select: none;
+         }
+         </style><title data-react-helmet="true">Mrunu (@invalidusername) on Snapchat</title><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><noscript data-n-css=""></noscript><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/049823d6.8b03ce304b0e44456f30.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/22.ca59e6299b825dc862b0.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/webpack-edb54b561e62fb294b85.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/framework.efe182f2d62be1d8151a.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/c408797459d80c128d5e47906020fa02c3ea7a51.cdf474846c815ffe556c.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/f6078781a05fe1bcb0902d23dbbb2662c8d200b3.0cb66906a1ea3f804368.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/main-69ec1f1dba14cd9f620a.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/c1468a61a92675d836a3000bab1334fb54fd20a9.074f204d663a13469e0b.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/d241c1e27ffe07c251e6f8ab09888e7ecf8ae8dc.b20db949b32dafefad5c.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/d4fc9bc7fce3fa7dbb251df097e4d60e4f4a3ec9.6a57a5151732d06fa88a.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/pages/_app-9a2167e8d8d9d9f101c9.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/29107295.be25f8bc8bdde59f114d.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/641167d64809277a1b9199554823a0e631b3bff2.b1423abff274817ff848.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/96c0058ea2ce58b3f27756fc0d0be33ac3f6361c.4360e309b36814bc7496.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/64dd010a9368940fc41206bc54dfee6183397831.1358f9c5b56d2322e06e.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/bd9739576daf9a5525e7028695825e8d0c29e04c.65c9b0762abe3d67e2ce.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/f2142e6c893e00c2f1a27f144791418e507fc12c.1ef92cfd6920c8f93e61.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/e2ef7edf3a7e66ae27a9d163772f8c722ad47684.7e5591f9407dd7837830.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/61f94ab364ffeaf810caabbb5e8c59d41b273801.6e578c39745032b54013.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/d01c7d3028b0c7a5252ef883c5a43f5f0e747f01.5c6a4b590ccfff6d1784.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/pages/@/%5Busername%5D-19264ae3ee802be2dc6d.js" as="script"/></head><body id="root"><div id="__next"><style data-emotion="css-global cqw65k">@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.ttf") format("truetype");font-weight:100;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.ttf") format("truetype");font-weight:100;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.ttf") format("truetype");font-weight:200;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.ttf") format("truetype");font-weight:200;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Regular.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Regular.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Regular.ttf") format("truetype");font-weight:300;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Italic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Italic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Italic.ttf") format("truetype");font-weight:300;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Medium.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Medium.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Medium.ttf") format("truetype");font-weight:400;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-MediumItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-MediumItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-MediumItalic.ttf") format("truetype");font-weight:400;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-DemiBold.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-DemiBold.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-DemiBold.ttf") format("truetype");font-weight:500;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-DemiBoldItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-DemiBoldItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-DemiBoldItalic.ttf") format("truetype");font-weight:500;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Bold.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Bold.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Bold.ttf") format("truetype");font-weight:600;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.ttf") format("truetype");font-weight:600;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Bold.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Bold.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Bold.ttf") format("truetype");font-weight:700;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.ttf") format("truetype");font-weight:700;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Heavy.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Heavy.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Heavy.ttf") format("truetype");font-weight:800;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.ttf") format("truetype");font-weight:800;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Heavy.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Heavy.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Heavy.ttf") format("truetype");font-weight:900;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.ttf") format("truetype");font-weight:900;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Thin.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Thin.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Thin.ttf") format("truetype");font-weight:100;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ThinItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ThinItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ThinItalic.ttf") format("truetype");font-weight:100;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Extralight.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Extralight.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Extralight.ttf") format("truetype");font-weight:200;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ExtralightItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ExtralightItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ExtralightItalic.ttf") format("truetype");font-weight:200;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Light.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Light.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Light.ttf") format("truetype");font-weight:300;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-LightItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-LightItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-LightItalic.ttf") format("truetype");font-weight:300;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Regular.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Regular.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Regular.ttf") format("truetype");font-weight:400;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-RegularItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-RegularItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-RegularItalic.ttf") format("truetype");font-weight:400;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Medium.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Medium.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Medium.ttf") format("truetype");font-weight:500;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-MediumItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-MediumItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-MediumItalic.ttf") format("truetype");font-weight:500;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Semibold.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Semibold.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Semibold.ttf") format("truetype");font-weight:600;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SemiboldItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SemiboldItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SemiboldItalic.ttf") format("truetype");font-weight:600;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Bold.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Bold.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Bold.ttf") format("truetype");font-weight:700;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BoldItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BoldItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BoldItalic.ttf") format("truetype");font-weight:700;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Black.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Black.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Black.ttf") format("truetype");font-weight:800;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BlackItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BlackItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BlackItalic.ttf") format("truetype");font-weight:800;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Super.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Super.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Super.ttf") format("truetype");font-weight:900;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SuperItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SuperItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SuperItalic.ttf") format("truetype");font-weight:900;font-style:italic;font-display:block;}</style></div><script id="__NEXT_DATA_" type="application/json">{"props":{"pageProps":{"googleAnalyticsPropertyId":"UA-41740027-40","localizedMessages":{"default":{"+9d+q7":"Nonprofit Organization","+ByJA/":"Stories","+hwkQQ":"Film / TV","+lhElX":"Copyright infringement","+o8gM9":"Kit","/Xkr+t":"by {creatorDisplayName}","/dF4HW":"Spotlight","/tNMyW":"Download","/vdS3s":"Download Snapchat to Watch Now","04qzmG":"You will now be taken to the next Snap - press 'Close' to do this right away or we will continue automatically in 10 seconds.","0FP975":"Post to Spotlight","0Y6c0W":"Restaurant Chain","0YKDxr":"Photographer","0dJz6S":"Threatening, violent, or concerning","0uHjye":"Share this Snap","1PzCdm":"It asks for or threatens to post inappropriate Snaps","1V8Uma":"Public Figure","1egAGi":"Movie Character","1kdcl2":"Media / News Company","2LLiYb":"Close","2V40yT":"More Options","2l730k":"Film / TV Personality","4V5k0y":"Support","5HsSrO":"I just don't like it","5XW8Zd":"{subscriberCount} Subscribers","5m3Hu8":"I'm worried this Snapchatter might hurt themselves","5v6wP7":"Motivational Speaker","5zZGnG":"Writer","6yvoZD":"Sorry,","7BHw3h":"Religious Organization","7HP0Jf":"Coach","7XZM2L":"Business","7rVnIj":"Spotlight","7xehRy":"Producer","7yuYaU":"Businesses \u0026 Groups","8Sw4jY":"Report Snap","9NRv3Z":"Snapcodes","ATeDiR":"Thank you for reporting this Snap.","AbkQPs":"It's an invasion of privacy","AtLF/u":"This content was not found","CAgCZ5":"Nudity or sexual content","CJBFGo":"Politician","CVucIf":"Community Organization","DY4yHA":"Brand","EPBE+l":"Government Official","ESomE8":"Submit","Eqnt63":"{timeDifference}m ago","FDOu63":"Someone else is being bullied or harassed","Fsg136":"Episode {episodeNumber}","Ftta6c":"It's threatening a person or place","G7hRik":"Spotlight is not available in your location","GJZs5E":"It's spam","GVLbZP":"Stories","GaNuM2":"Best of Spotlight","Gh1a/j":"Food Professional","GssbOn":"Product","Gvuqme":"It's an inappropriate Snap of someone else","HLxWNM":"It sells or promotes inappropriate Snaps","HVgZaB":"Creator","HkaOsh":"Open your Snapchat","I1rLjL":"Ads","I6sovq":"Political Organization","IWKERN":"Fashion Model","JbCR5V":"This content is not available","Ju77ns":"Comedian","MDthgV":"Sports League","MN6Znh":"Watch more in Snapchat","MUzWB7":"Please provide your Snapchat username if you have one, and the email associated with your account","N7Wq/c":"Violent or disturbing","N7iI/k":"Download Snapchat to find more","NXPVkv":"Company / Enterprise","P6YGQz":"Open in Snapchat","PQcLi/":"Service","PyzdXL":"Cancel","Q4RuCH":"Maps","Q71IbU":"Government Organization","QdGWFE":"Season {seasonNumber}","RJo0Z3":"Harassment or Hate speech","RmE5lP":"Lifestyle Influencer","RtNy71":"Musician / Band","SCe4GQ":"Film Director","SVOJKh":"Video Game","SgFTtk":"Up next","TNK/W/":"Lenses","Tm6yFt":"Download Snapchat","UIZTzu":"It's attempting to buy or sell drugs or weapons","Uk55sM":"Add me on Snapchat!","VRmDFV":"Snap Reported","VZQx67":"This Snap is no longer available","VjDaWB":"Watch more from {publisherTitle}","W07I8V":"Share {username}'s Snap","WGtpBM":"People","WyUwHm":"They are pretending to be me","XbXoMR":"Actor","YhMtYd":"Spectacles","Yt2+ye":"My Story","ZPrHrl":"Internet Company","ZViZgq":"Traveler","ZlJO0Q":"Apparel / Fashion","ZvzVyN":"Top Lenses","aSXQy0":"Sports Personality","ah6l3c":"Charity / Cause","ais8eK":"Group","by2dgE":"News Personality","dAksd9":"Journalist","dItw6q":"Dancer","dJDu/3":"Entrepreneur","dkWyPr":"Vlogger / Blogger","fPIy5v":"Retail Company","fxAji7":"Filters \u0026 Lenses","hPxDQC":"Video Game Creator","jWa4OT":"College / University","jqpH+5":"Is there any more information you want to share about this Snap?","kNCf90":"Products \u0026 Brands","kzoiEX":"{timeDifference}h ago","l1fnUG":"Scientist","lbui+i":"It's hate speech targeting me or another group","nbiOpp":"Lens Studio","ojrZ4G":"Download","pCK8FJ":"Artist","pPIiOl":"{subscriberCount} Subscribers","rL8HYz":"Professional Gamer","rLGZZX":"Just now","rNVPnk":"It's an inappropriate Snap of me","rrdPgT":"Store","rsYMnU":"Episodes","sRM8i5":"Why do you want to report this Snap?","sVcU8q":"Posted to Snap Map","tYFb/P":"Spotlight","vTd+a8":"I'm being bullied or harassed","vqdER6":"Fitness Professional","wVfxbD":"Political Candidate","wpLx7z":"Lens Creator","x1C/5K":"Person","x4F6zb":"Report Snap","xLaO8v":"Health / Beauty","yT6a3h":"In this Snap","ys7Y26":"Athlete","zExXNB":"Sports Team"},"+9d+q7":"Nonprofit Organization","+ByJA/":"Stories","+hwkQQ":"Film / TV","+lhElX":"Copyright infringement","+o8gM9":"Kit","/Xkr+t":"by {creatorDisplayName}","/dF4HW":"Spotlight","/tNMyW":"Download","/vdS3s":"Download Snapchat to Watch Now","04qzmG":"You will now be taken to the next Snap - press 'Close' to do this right away or we will continue automatically in 10 seconds.","0FP975":"Post to Spotlight","0Y6c0W":"Restaurant Chain","0YKDxr":"Photographer","0dJz6S":"Threatening, violent, or concerning","0uHjye":"Share this Snap","1PzCdm":"It asks for or threatens to post inappropriate Snaps","1V8Uma":"Public Figure","1egAGi":"Movie Character","1kdcl2":"Media / News Company","2LLiYb":"Close","2V40yT":"More Options","2l730k":"Film / TV Personality","4V5k0y":"Support","5HsSrO":"I just don't like it","5XW8Zd":"{subscriberCount} Subscribers","5m3Hu8":"I'm worried this Snapchatter might hurt themselves","5v6wP7":"Motivational Speaker","5zZGnG":"Writer","6yvoZD":"Sorry,","7BHw3h":"Religious Organization","7HP0Jf":"Coach","7XZM2L":"Business","7rVnIj":"Spotlight","7xehRy":"Producer","7yuYaU":"Businesses \u0026 Groups","8Sw4jY":"Report Snap","9NRv3Z":"Snapcodes","ATeDiR":"Thank you for reporting this Snap.","AbkQPs":"It's an invasion of privacy","AtLF/u":"This content was not found","CAgCZ5":"Nudity or sexual content","CJBFGo":"Politician","CVucIf":"Community Organization","DY4yHA":"Brand","EPBE+l":"Government Official","ESomE8":"Submit","Eqnt63":"{timeDifference}m ago","FDOu63":"Someone else is being bullied or harassed","Fsg136":"Episode {episodeNumber}","Ftta6c":"It's threatening a person or place","G7hRik":"Spotlight is not available in your location","GJZs5E":"It's spam","GVLbZP":"Stories","GaNuM2":"Best of Spotlight","Gh1a/j":"Food Professional","GssbOn":"Product","Gvuqme":"It's an inappropriate Snap of someone else","HLxWNM":"It sells or promotes inappropriate Snaps","HVgZaB":"Creator","HkaOsh":"Open your Snapchat","I1rLjL":"Ads","I6sovq":"Political Organization","IWKERN":"Fashion Model","JbCR5V":"This content is not available","Ju77ns":"Comedian","MDthgV":"Sports League","MN6Znh":"Watch more in Snapchat","MUzWB7":"Please provide your Snapchat username if you have one, and the email associated with your account","N7Wq/c":"Violent or disturbing","N7iI/k":"Download Snapchat to find more","NXPVkv":"Company / Enterprise","P6YGQz":"Open in Snapchat","PQcLi/":"Service","PyzdXL":"Cancel","Q4RuCH":"Maps","Q71IbU":"Government Organization","QdGWFE":"Season {seasonNumber}","RJo0Z3":"Harassment or Hate speech","RmE5lP":"Lifestyle Influencer","RtNy71":"Musician / Band","SCe4GQ":"Film Director","SVOJKh":"Video Game","SgFTtk":"Up next","TNK/W/":"Lenses","Tm6yFt":"Download Snapchat","UIZTzu":"It's attempting to buy or sell drugs or weapons","Uk55sM":"Add me on Snapchat!","VRmDFV":"Snap Reported","VZQx67":"This Snap is no longer available","VjDaWB":"Watch more from {publisherTitle}","W07I8V":"Share {username}'s Snap","WGtpBM":"People","WyUwHm":"They are pretending to be me","XbXoMR":"Actor","YhMtYd":"Spectacles","Yt2+ye":"My Story","ZPrHrl":"Internet Company","ZViZgq":"Traveler","ZlJO0Q":"Apparel / Fashion","ZvzVyN":"Top Lenses","aSXQy0":"Sports Personality","ah6l3c":"Charity / Cause","ais8eK":"Group","by2dgE":"News Personality","dAksd9":"Journalist","dItw6q":"Dancer","dJDu/3":"Entrepreneur","dkWyPr":"Vlogger / Blogger","fPIy5v":"Retail Company","fxAji7":"Filters \u0026 Lenses","hPxDQC":"Video Game Creator","jWa4OT":"College / University","jqpH+5":"Is there any more information you want to share about this Snap?","kNCf90":"Products \u0026 Brands","kzoiEX":"{timeDifference}h ago","l1fnUG":"Scientist","lbui+i":"It's hate speech targeting me or another group","nbiOpp":"Lens Studio","ojrZ4G":"Download","pCK8FJ":"Artist","pPIiOl":"{subscriberCount} Subscribers","rL8HYz":"Professional Gamer","rLGZZX":"Just now","rNVPnk":"It's an inappropriate Snap of me","rrdPgT":"Store","rsYMnU":"Episodes","sRM8i5":"Why do you want to report this Snap?","sVcU8q":"Posted to Snap Map","tYFb/P":"Spotlight","vTd+a8":"I'm being bullied or harassed","vqdER6":"Fitness Professional","wVfxbD":"Political Candidate","wpLx7z":"Lens Creator","x1C/5K":"Person","x4F6zb":"Report Snap","xLaO8v":"Health / Beauty","yT6a3h":"In this Snap","ys7Y26":"Athlete","zExXNB":"Sports Team"},"lenses":[],"curatedHighlights":[{"storyType":3,"storyTapId":"0","snapList":[{"snapIndex":0,"snapMediaType":0,"snapId":{"value":""},"snapUrls":{"mediaUrl":"https://cf-st.sc-cdn.net/d/Cg5MaQODMG3TnzwDo9KIa.400.IRZXSOY?uc=12","mediaPreviewUrl":{"value":"https://cf-st.sc-cdn.net/d/Cg5MaQODMG3TnzwDo9KIa.410.IRZXSOY?uc=12"}},"timestampInSec":{"value":"1606531630"}},{"snapIndex":1,"snapMediaType":0,"snapId":{"value":""},"snapUrls":{"mediaUrl":"https://cf-st.sc-cdn.net/d/uxOSCj5RgvtbPc1WJFZE4.400.IRZXSOY?uc=12","mediaPreviewUrl":{"value":"https://cf-st.sc-cdn.net/d/uxOSCj5RgvtbPc1WJFZE4.410.IRZXSOY?uc=12"}},"timestampInSec":{"value":"1605705190"}}],"storyId":{"value":""},"storyTitle":{"value":""},"thumbnailUrl":{"value":"https://cf-st.sc-cdn.net/d/Cg5MaQODMG3TnzwDo9KIa.410.IRZXSOY?uc=12"}}],"spotlightHighlights":[],"spotlightHighlightsMetadata":[],"viewerInfo":{"country":"IN","locale":"en_US"},"localization":{"direction":0},"pageLinks":{"oneLinkUrl":"https://click.snapchat.com/aVHG?pid=snapchat_download_page\u0026af_dp=https://www.snapchat.com/add/invalidusername?sc_referrer%3Dweb\u0026af_web_dp=https://snapchat.com/download?purpose%3Dweb_stories","snapchatCanonicalUrl":"https://www.snapchat.com/add/invalidusername","canonicalUrl":"https://www.snapchat.com/add/invalidusername","snapcodeImageUrl":"https://app.snapchat.com/web/deeplink/snapcode?username=invalidusername\u0026type=SVG\u0026bitmoji=enable"},"pageMetadata":{"pageType":9,"pageTitle":"Mrunu (@invalidusername) on Snapchat","pageDescription":{"value":"Mrunu is on Snapchat!"}},"userProfile":{"$case":"publicProfileInfo","publicProfileInfo":{"username":"invalidusername","title":"Mrunu","snapcodeImageUrl":"https://app.snapchat.com/web/deeplink/snapcode?username=invalidusername\u0026type=SVG\u0026bitmoji=enable","badge":1,"categoryStringId":"public-profile-category-v3-people","subcategoryStringId":"public-profile-subcategory-v3-artist","subscriberCount":"874600","bio":"Welcome to my weird life ✨","websiteUrl":"https://youtube.com/c/GujjuUnicorn","profilePictureUrl":"https://cf-st.sc-cdn.net/aps/bolt/aHR0cHM6Ly9jZi1zdC5zYy1jZG4ubmV0L2QvdTVBZEFXVnV1RlVSNDNBQk5qRHVNP2JvPUVnMGFBQm9BTWdFRVNBSlFHV0FCJnVjPTI1._RS0,90_FMjpeg","address":"Mumbai, India, India","hasCuratedHighlights":true,"hasSpotlightHighlights":false,"mutableName":"","publisherType":"","squareHeroImageUrl":"","primaryColor":""}},"story":{"storyType":5,"storyTapId":"0","snapList":[{"snapIndex":0,"snapMediaType":1,"snapId":{"value":"1PgHW1XZSgWteDhyTiIFbgAAgcnlmYnB0ZWpiAXxms2FCAXxms17GAAAAAA"},"snapUrls":{"mediaUrl":"https://filesamples.com/samples/video/mp4/sample_640x360.mp4","mediaPreviewUrl":{"value":"https://s.sc-cdn.net/1d/5Wv7rx8leVHNTyY454OlnCjZDCNqDQoW7y7eUU1T1CY=/default/preview_overlay.jpg"}},"timestampInSec":{"value":"1633810603"}},{"snapIndex":1,"snapMediaType":0,"snapId":{"value":"1PgHW1XZSgWteDhyTiIFbgAAgZWZqZ2t2ZGN4AXxpJwZoAXxpJwRfAAAAAA"},"snapUrls":{"mediaUrl":"https://filesamples.com/samples/video/mp4/sample_640x360.mp4"},"timestampInSec":{"value":"1633851737"}},{"snapIndex":2,"snapMediaType":0,"snapId":{"value":"1PgHW1XZSgWteDhyTiIFbgAAgdGlyeXpodGx4AXxpR4jsAXxpR4XzAAAAAA"},"snapUrls":{"mediaUrl":"https://filesamples.com/samples/video/mp4/sample_640x360.mp4"},"timestampInSec":{"value":"1633853867"}},{"snapIndex":3,"snapMediaType":0,"snapId":{"value":"1PgHW1XZSgWteDhyTiIFbgAAgdnJlc2hjeWd5AXxqhQjjAXxqhQaeAAAAAA"},"snapUrls":{"mediaUrl":"https://filesamples.com/samples/video/mp4/sample_640x360.mp4"},"timestampInSec":{"value":"1633874675"}}],"storyId":{"value":"invalidusername"},"thumbnailUrl":{"value":"https://s.sc-cdn.net/1d/5Wv7rx8leVHNTyY454OlnCjZDCNqDQoW7y7eUU1T1CY=/default/preview_overlay.jpg"}},"linkPreview":{"title":"invalidusername on Snapchat","description":"","canonicalUrl":"https://story.snapchat.com/u/invalidusername","twitterImage":{"url":"https://story.snapchat.com/@invalidusername/preview/twitter.png","size":{"width":1200,"height":600}},"facebookImage":{"url":"https://story.snapchat.com/@invalidusername/preview/facebook.png","size":{"width":1200,"height":628}}}},"status":0,"log":{"levels":{"TRACE":0,"DEBUG":1,"INFO":2,"WARN":3,"ERROR":4,"SILENT":5}}},"page":"/@/[username]","query":{"username":"@invalidusername"},"buildId":"23576-9b597984705a8ea2bff65ac8abd3eb5a984c976a","assetPrefix":"https://story.snapchat.com","isFallback":false,"dynamicIds":["gkwE","+51n","AC5g","DbP8","KIpE","LQDX","NuZu","aLx/","qmXy","sZW5","sZkf"],"gip":true,"appGip":true}</script><script nomodule="" src="https://story.snapchat.com/_next/static/chunks/polyfills-553aafd328e99d1ecd5e.js"></script><script async="" src="https://story.snapchat.com/_next/static/chunks/049823d6.8b03ce304b0e44456f30.js"></script><script async="" src="https://story.snapchat.com/_next/static/chunks/22.ca59e6299b825dc862b0.js"></script><script src="https://story.snapchat.com/_next/static/chunks/webpack-edb54b561e62fb294b85.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/framework.efe182f2d62be1d8151a.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/c408797459d80c128d5e47906020fa02c3ea7a51.cdf474846c815ffe556c.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/f6078781a05fe1bcb0902d23dbbb2662c8d200b3.0cb66906a1ea3f804368.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/main-69ec1f1dba14cd9f620a.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/c1468a61a92675d836a3000bab1334fb54fd20a9.074f204d663a13469e0b.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/d241c1e27ffe07c251e6f8ab09888e7ecf8ae8dc.b20db949b32dafefad5c.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/d4fc9bc7fce3fa7dbb251df097e4d60e4f4a3ec9.6a57a5151732d06fa88a.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/pages/_app-9a2167e8d8d9d9f101c9.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/29107295.be25f8bc8bdde59f114d.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/641167d64809277a1b9199554823a0e631b3bff2.b1423abff274817ff848.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/96c0058ea2ce58b3f27756fc0d0be33ac3f6361c.4360e309b36814bc7496.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/64dd010a9368940fc41206bc54dfee6183397831.1358f9c5b56d2322e06e.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/bd9739576daf9a5525e7028695825e8d0c29e04c.65c9b0762abe3d67e2ce.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/f2142e6c893e00c2f1a27f144791418e507fc12c.1ef92cfd6920c8f93e61.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/e2ef7edf3a7e66ae27a9d163772f8c722ad47684.7e5591f9407dd7837830.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/61f94ab364ffeaf810caabbb5e8c59d41b273801.6e578c39745032b54013.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/d01c7d3028b0c7a5252ef883c5a43f5f0e747f01.5c6a4b590ccfff6d1784.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/pages/@/%5Busername%5D-19264ae3ee802be2dc6d.js" async=""></script><script src="https://story.snapchat.com/_next/static/23576-9b597984705a8ea2bff65ac8abd3eb5a984c976a/_buildManifest.js" async=""></script><script src="https://story.snapchat.com/_next/static/23576-9b597984705a8ea2bff65ac8abd3eb5a984c976a/_ssgManifest.js" async=""></script></body></html>
```

### Comparing `snapchat-dlp-1.5.2/tests/mock_data/invalidusername-nostories.html` & `snapchat-dlp-1.5.8/tests/mock_data/invalidusername-nostories.html`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-
-<!DOCTYPE html><html prefix="og: https://ogp.me/ns#" dir="0" lang="en-US"><head><link data-react-helmet="true" rel="canonical" href="https://www.snapchat.com/add/mrunu11"/><meta data-react-helmet="true" name="description" content="Mrunu is on Snapchat!"/><meta data-react-helmet="true" name="apple-itunes-app" content="app-id=447188370, app-argument=https://www.snapchat.com/add/mrunu11"/><meta data-react-helmet="true" name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1.0, user-scalable=0"/><meta data-react-helmet="true" name="metrics-page-name" content="User_Profile.PublicProfile"/><meta data-react-helmet="true" property="og:title" content="mrunu11 on Snapchat"/><meta data-react-helmet="true" property="og:type" content="video.other"/><meta data-react-helmet="true" property="og:url" content="https://story.snapchat.com/u/mrunu11"/><meta data-react-helmet="true" property="og:image" content="https://story.snapchat.com/@mrunu11/preview/facebook.png"/><meta data-react-helmet="true" property="og:locale:alternate" content="ar_AA"/><meta data-react-helmet="true" property="og:locale:alternate" content="da_DK"/><meta data-react-helmet="true" property="og:locale:alternate" content="de_DK"/><meta data-react-helmet="true" property="og:locale:alternate" content="en_GB"/><meta data-react-helmet="true" property="og:locale:alternate" content="en_US"/><meta data-react-helmet="true" property="og:locale:alternate" content="es_ES"/><meta data-react-helmet="true" property="og:locale:alternate" content="es_MX"/><meta data-react-helmet="true" property="og:locale:alternate" content="fi_FI"/><meta data-react-helmet="true" property="og:locale:alternate" content="fr_FR"/><meta data-react-helmet="true" property="og:locale:alternate" content="it_IT"/><meta data-react-helmet="true" property="og:locale:alternate" content="ja_JP"/><meta data-react-helmet="true" property="og:locale:alternate" content="nb_NO"/><meta data-react-helmet="true" property="og:locale:alternate" content="nl_NL"/><meta data-react-helmet="true" property="og:locale:alternate" content="pt_BR"/><meta data-react-helmet="true" property="og:locale:alternate" content="sv_SE"/><meta data-react-helmet="true" property="og:image:width" content="1200"/><meta data-react-helmet="true" property="og:image:height" content="628"/><meta data-react-helmet="true" property="og:site_name" content="Snapchat"/><meta data-react-helmet="true" property="fb:app_id" content="394343577431007"/><meta data-react-helmet="true" property="fb:admins" content="1349731971"/><meta data-react-helmet="true" property="twitter:card" content="summary_large_image"/><meta data-react-helmet="true" property="twitter:site" content="@Snapchat"/><meta data-react-helmet="true" property="twitter:title" content="mrunu11 on Snapchat"/><meta data-react-helmet="true" property="twitter:image" content="https://story.snapchat.com/@mrunu11/preview/twitter.png"/><script data-react-helmet="true" async="" src="https://www.google-analytics.com/analytics.js"></script><script data-react-helmet="true">
-    window.ga=window.ga||function(){(ga.q = ga.q || []).push(arguments)};
-    ga.l=+new Date;
-    ga('create','UA-41740027-40', 'auto');
-    ga('send','pageview', location.pathname);
-  </script><style data-react-helmet="true">html {
-          height: 100%;
-          box-sizing: border-box;
-         }
-
-         body {
-          margin: 0;
-          height: 100%;
-          background: #121314;
-          font-family: Avenir Next, Helvetica, sans-serif;
-          -webkit-text-fill-color: currentcolor;
-         }
-
-         #__next, #root {
-          height: 100%;
-         }
-
-         *, *:before, *:after {
-          box-sizing: inherit;
-         }
-
-         button {
-          -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
-          -webkit-tap-highlight-color: transparent;
-          -webkit-user-select: none;
-          -khtml-user-select: none;
-          -moz-user-select: none;
-          -ms-user-select: none;
-          user-select: none;
-         }
-         </style><title data-react-helmet="true">Mrunu (@mrunu11) on Snapchat</title><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><noscript data-n-css=""></noscript><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/049823d6.8b03ce304b0e44456f30.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/22.ca59e6299b825dc862b0.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/webpack-edb54b561e62fb294b85.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/framework.efe182f2d62be1d8151a.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/c408797459d80c128d5e47906020fa02c3ea7a51.cdf474846c815ffe556c.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/f6078781a05fe1bcb0902d23dbbb2662c8d200b3.0cb66906a1ea3f804368.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/main-69ec1f1dba14cd9f620a.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/c1468a61a92675d836a3000bab1334fb54fd20a9.074f204d663a13469e0b.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/d241c1e27ffe07c251e6f8ab09888e7ecf8ae8dc.b20db949b32dafefad5c.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/d4fc9bc7fce3fa7dbb251df097e4d60e4f4a3ec9.6a57a5151732d06fa88a.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/pages/_app-9a2167e8d8d9d9f101c9.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/29107295.be25f8bc8bdde59f114d.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/641167d64809277a1b9199554823a0e631b3bff2.b1423abff274817ff848.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/96c0058ea2ce58b3f27756fc0d0be33ac3f6361c.4360e309b36814bc7496.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/64dd010a9368940fc41206bc54dfee6183397831.1358f9c5b56d2322e06e.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/bd9739576daf9a5525e7028695825e8d0c29e04c.65c9b0762abe3d67e2ce.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/f2142e6c893e00c2f1a27f144791418e507fc12c.1ef92cfd6920c8f93e61.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/e2ef7edf3a7e66ae27a9d163772f8c722ad47684.7e5591f9407dd7837830.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/61f94ab364ffeaf810caabbb5e8c59d41b273801.6e578c39745032b54013.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/d01c7d3028b0c7a5252ef883c5a43f5f0e747f01.5c6a4b590ccfff6d1784.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/pages/@/%5Busername%5D-19264ae3ee802be2dc6d.js" as="script"/></head><body id="root"><div id="__next"><style data-emotion="css-global cqw65k">@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.ttf") format("truetype");font-weight:100;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.ttf") format("truetype");font-weight:100;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.ttf") format("truetype");font-weight:200;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.ttf") format("truetype");font-weight:200;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Regular.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Regular.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Regular.ttf") format("truetype");font-weight:300;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Italic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Italic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Italic.ttf") format("truetype");font-weight:300;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Medium.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Medium.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Medium.ttf") format("truetype");font-weight:400;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-MediumItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-MediumItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-MediumItalic.ttf") format("truetype");font-weight:400;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-DemiBold.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-DemiBold.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-DemiBold.ttf") format("truetype");font-weight:500;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-DemiBoldItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-DemiBoldItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-DemiBoldItalic.ttf") format("truetype");font-weight:500;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Bold.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Bold.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Bold.ttf") format("truetype");font-weight:600;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.ttf") format("truetype");font-weight:600;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Bold.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Bold.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Bold.ttf") format("truetype");font-weight:700;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.ttf") format("truetype");font-weight:700;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Heavy.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Heavy.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Heavy.ttf") format("truetype");font-weight:800;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.ttf") format("truetype");font-weight:800;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Heavy.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Heavy.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Heavy.ttf") format("truetype");font-weight:900;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.ttf") format("truetype");font-weight:900;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Thin.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Thin.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Thin.ttf") format("truetype");font-weight:100;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ThinItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ThinItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ThinItalic.ttf") format("truetype");font-weight:100;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Extralight.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Extralight.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Extralight.ttf") format("truetype");font-weight:200;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ExtralightItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ExtralightItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ExtralightItalic.ttf") format("truetype");font-weight:200;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Light.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Light.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Light.ttf") format("truetype");font-weight:300;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-LightItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-LightItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-LightItalic.ttf") format("truetype");font-weight:300;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Regular.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Regular.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Regular.ttf") format("truetype");font-weight:400;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-RegularItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-RegularItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-RegularItalic.ttf") format("truetype");font-weight:400;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Medium.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Medium.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Medium.ttf") format("truetype");font-weight:500;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-MediumItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-MediumItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-MediumItalic.ttf") format("truetype");font-weight:500;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Semibold.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Semibold.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Semibold.ttf") format("truetype");font-weight:600;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SemiboldItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SemiboldItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SemiboldItalic.ttf") format("truetype");font-weight:600;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Bold.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Bold.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Bold.ttf") format("truetype");font-weight:700;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BoldItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BoldItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BoldItalic.ttf") format("truetype");font-weight:700;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Black.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Black.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Black.ttf") format("truetype");font-weight:800;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BlackItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BlackItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BlackItalic.ttf") format("truetype");font-weight:800;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Super.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Super.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Super.ttf") format("truetype");font-weight:900;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SuperItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SuperItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SuperItalic.ttf") format("truetype");font-weight:900;font-style:italic;font-display:block;}</style></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"googleAnalyticsPropertyId":"UA-41740027-40","localizedMessages":{"default":{"+9d+q7":"Nonprofit Organization","+ByJA/":"Stories","+hwkQQ":"Film / TV","+lhElX":"Copyright infringement","+o8gM9":"Kit","/Xkr+t":"by {creatorDisplayName}","/dF4HW":"Spotlight","/tNMyW":"Download","/vdS3s":"Download Snapchat to Watch Now","04qzmG":"You will now be taken to the next Snap - press 'Close' to do this right away or we will continue automatically in 10 seconds.","0FP975":"Post to Spotlight","0Y6c0W":"Restaurant Chain","0YKDxr":"Photographer","0dJz6S":"Threatening, violent, or concerning","0uHjye":"Share this Snap","1PzCdm":"It asks for or threatens to post inappropriate Snaps","1V8Uma":"Public Figure","1egAGi":"Movie Character","1kdcl2":"Media / News Company","2LLiYb":"Close","2V40yT":"More Options","2l730k":"Film / TV Personality","4V5k0y":"Support","5HsSrO":"I just don't like it","5XW8Zd":"{subscriberCount} Subscribers","5m3Hu8":"I'm worried this Snapchatter might hurt themselves","5v6wP7":"Motivational Speaker","5zZGnG":"Writer","6yvoZD":"Sorry,","7BHw3h":"Religious Organization","7HP0Jf":"Coach","7XZM2L":"Business","7rVnIj":"Spotlight","7xehRy":"Producer","7yuYaU":"Businesses \u0026 Groups","8Sw4jY":"Report Snap","9NRv3Z":"Snapcodes","ATeDiR":"Thank you for reporting this Snap.","AbkQPs":"It's an invasion of privacy","AtLF/u":"This content was not found","CAgCZ5":"Nudity or sexual content","CJBFGo":"Politician","CVucIf":"Community Organization","DY4yHA":"Brand","EPBE+l":"Government Official","ESomE8":"Submit","Eqnt63":"{timeDifference}m ago","FDOu63":"Someone else is being bullied or harassed","Fsg136":"Episode {episodeNumber}","Ftta6c":"It's threatening a person or place","G7hRik":"Spotlight is not available in your location","GJZs5E":"It's spam","GVLbZP":"Stories","GaNuM2":"Best of Spotlight","Gh1a/j":"Food Professional","GssbOn":"Product","Gvuqme":"It's an inappropriate Snap of someone else","HLxWNM":"It sells or promotes inappropriate Snaps","HVgZaB":"Creator","HkaOsh":"Open your Snapchat","I1rLjL":"Ads","I6sovq":"Political Organization","IWKERN":"Fashion Model","JbCR5V":"This content is not available","Ju77ns":"Comedian","MDthgV":"Sports League","MN6Znh":"Watch more in Snapchat","MUzWB7":"Please provide your Snapchat username if you have one, and the email associated with your account","N7Wq/c":"Violent or disturbing","N7iI/k":"Download Snapchat to find more","NXPVkv":"Company / Enterprise","P6YGQz":"Open in Snapchat","PQcLi/":"Service","PyzdXL":"Cancel","Q4RuCH":"Maps","Q71IbU":"Government Organization","QdGWFE":"Season {seasonNumber}","RJo0Z3":"Harassment or Hate speech","RmE5lP":"Lifestyle Influencer","RtNy71":"Musician / Band","SCe4GQ":"Film Director","SVOJKh":"Video Game","SgFTtk":"Up next","TNK/W/":"Lenses","Tm6yFt":"Download Snapchat","UIZTzu":"It's attempting to buy or sell drugs or weapons","Uk55sM":"Add me on Snapchat!","VRmDFV":"Snap Reported","VZQx67":"This Snap is no longer available","VjDaWB":"Watch more from {publisherTitle}","W07I8V":"Share {username}'s Snap","WGtpBM":"People","WyUwHm":"They are pretending to be me","XbXoMR":"Actor","YhMtYd":"Spectacles","Yt2+ye":"My Story","ZPrHrl":"Internet Company","ZViZgq":"Traveler","ZlJO0Q":"Apparel / Fashion","ZvzVyN":"Top Lenses","aSXQy0":"Sports Personality","ah6l3c":"Charity / Cause","ais8eK":"Group","by2dgE":"News Personality","dAksd9":"Journalist","dItw6q":"Dancer","dJDu/3":"Entrepreneur","dkWyPr":"Vlogger / Blogger","fPIy5v":"Retail Company","fxAji7":"Filters \u0026 Lenses","hPxDQC":"Video Game Creator","jWa4OT":"College / University","jqpH+5":"Is there any more information you want to share about this Snap?","kNCf90":"Products \u0026 Brands","kzoiEX":"{timeDifference}h ago","l1fnUG":"Scientist","lbui+i":"It's hate speech targeting me or another group","nbiOpp":"Lens Studio","ojrZ4G":"Download","pCK8FJ":"Artist","pPIiOl":"{subscriberCount} Subscribers","rL8HYz":"Professional Gamer","rLGZZX":"Just now","rNVPnk":"It's an inappropriate Snap of me","rrdPgT":"Store","rsYMnU":"Episodes","sRM8i5":"Why do you want to report this Snap?","sVcU8q":"Posted to Snap Map","tYFb/P":"Spotlight","vTd+a8":"I'm being bullied or harassed","vqdER6":"Fitness Professional","wVfxbD":"Political Candidate","wpLx7z":"Lens Creator","x1C/5K":"Person","x4F6zb":"Report Snap","xLaO8v":"Health / Beauty","yT6a3h":"In this Snap","ys7Y26":"Athlete","zExXNB":"Sports Team"},"+9d+q7":"Nonprofit Organization","+ByJA/":"Stories","+hwkQQ":"Film / TV","+lhElX":"Copyright infringement","+o8gM9":"Kit","/Xkr+t":"by {creatorDisplayName}","/dF4HW":"Spotlight","/tNMyW":"Download","/vdS3s":"Download Snapchat to Watch Now","04qzmG":"You will now be taken to the next Snap - press 'Close' to do this right away or we will continue automatically in 10 seconds.","0FP975":"Post to Spotlight","0Y6c0W":"Restaurant Chain","0YKDxr":"Photographer","0dJz6S":"Threatening, violent, or concerning","0uHjye":"Share this Snap","1PzCdm":"It asks for or threatens to post inappropriate Snaps","1V8Uma":"Public Figure","1egAGi":"Movie Character","1kdcl2":"Media / News Company","2LLiYb":"Close","2V40yT":"More Options","2l730k":"Film / TV Personality","4V5k0y":"Support","5HsSrO":"I just don't like it","5XW8Zd":"{subscriberCount} Subscribers","5m3Hu8":"I'm worried this Snapchatter might hurt themselves","5v6wP7":"Motivational Speaker","5zZGnG":"Writer","6yvoZD":"Sorry,","7BHw3h":"Religious Organization","7HP0Jf":"Coach","7XZM2L":"Business","7rVnIj":"Spotlight","7xehRy":"Producer","7yuYaU":"Businesses \u0026 Groups","8Sw4jY":"Report Snap","9NRv3Z":"Snapcodes","ATeDiR":"Thank you for reporting this Snap.","AbkQPs":"It's an invasion of privacy","AtLF/u":"This content was not found","CAgCZ5":"Nudity or sexual content","CJBFGo":"Politician","CVucIf":"Community Organization","DY4yHA":"Brand","EPBE+l":"Government Official","ESomE8":"Submit","Eqnt63":"{timeDifference}m ago","FDOu63":"Someone else is being bullied or harassed","Fsg136":"Episode {episodeNumber}","Ftta6c":"It's threatening a person or place","G7hRik":"Spotlight is not available in your location","GJZs5E":"It's spam","GVLbZP":"Stories","GaNuM2":"Best of Spotlight","Gh1a/j":"Food Professional","GssbOn":"Product","Gvuqme":"It's an inappropriate Snap of someone else","HLxWNM":"It sells or promotes inappropriate Snaps","HVgZaB":"Creator","HkaOsh":"Open your Snapchat","I1rLjL":"Ads","I6sovq":"Political Organization","IWKERN":"Fashion Model","JbCR5V":"This content is not available","Ju77ns":"Comedian","MDthgV":"Sports League","MN6Znh":"Watch more in Snapchat","MUzWB7":"Please provide your Snapchat username if you have one, and the email associated with your account","N7Wq/c":"Violent or disturbing","N7iI/k":"Download Snapchat to find more","NXPVkv":"Company / Enterprise","P6YGQz":"Open in Snapchat","PQcLi/":"Service","PyzdXL":"Cancel","Q4RuCH":"Maps","Q71IbU":"Government Organization","QdGWFE":"Season {seasonNumber}","RJo0Z3":"Harassment or Hate speech","RmE5lP":"Lifestyle Influencer","RtNy71":"Musician / Band","SCe4GQ":"Film Director","SVOJKh":"Video Game","SgFTtk":"Up next","TNK/W/":"Lenses","Tm6yFt":"Download Snapchat","UIZTzu":"It's attempting to buy or sell drugs or weapons","Uk55sM":"Add me on Snapchat!","VRmDFV":"Snap Reported","VZQx67":"This Snap is no longer available","VjDaWB":"Watch more from {publisherTitle}","W07I8V":"Share {username}'s Snap","WGtpBM":"People","WyUwHm":"They are pretending to be me","XbXoMR":"Actor","YhMtYd":"Spectacles","Yt2+ye":"My Story","ZPrHrl":"Internet Company","ZViZgq":"Traveler","ZlJO0Q":"Apparel / Fashion","ZvzVyN":"Top Lenses","aSXQy0":"Sports Personality","ah6l3c":"Charity / Cause","ais8eK":"Group","by2dgE":"News Personality","dAksd9":"Journalist","dItw6q":"Dancer","dJDu/3":"Entrepreneur","dkWyPr":"Vlogger / Blogger","fPIy5v":"Retail Company","fxAji7":"Filters \u0026 Lenses","hPxDQC":"Video Game Creator","jWa4OT":"College / University","jqpH+5":"Is there any more information you want to share about this Snap?","kNCf90":"Products \u0026 Brands","kzoiEX":"{timeDifference}h ago","l1fnUG":"Scientist","lbui+i":"It's hate speech targeting me or another group","nbiOpp":"Lens Studio","ojrZ4G":"Download","pCK8FJ":"Artist","pPIiOl":"{subscriberCount} Subscribers","rL8HYz":"Professional Gamer","rLGZZX":"Just now","rNVPnk":"It's an inappropriate Snap of me","rrdPgT":"Store","rsYMnU":"Episodes","sRM8i5":"Why do you want to report this Snap?","sVcU8q":"Posted to Snap Map","tYFb/P":"Spotlight","vTd+a8":"I'm being bullied or harassed","vqdER6":"Fitness Professional","wVfxbD":"Political Candidate","wpLx7z":"Lens Creator","x1C/5K":"Person","x4F6zb":"Report Snap","xLaO8v":"Health / Beauty","yT6a3h":"In this Snap","ys7Y26":"Athlete","zExXNB":"Sports Team"},"lenses":[],"curatedHighlights":[{"storyType":3,"storyTapId":"0","snapList":[{"snapIndex":0,"snapMediaType":0,"snapId":{"value":""},"snapUrls":{"mediaUrl":"https://cf-st.sc-cdn.net/d/Cg5MaQODMG3TnzwDo9KIa.400.IRZXSOY?uc=12","mediaPreviewUrl":{"value":"https://cf-st.sc-cdn.net/d/Cg5MaQODMG3TnzwDo9KIa.410.IRZXSOY?uc=12"}},"timestampInSec":{"value":"1606531630"}},{"snapIndex":1,"snapMediaType":0,"snapId":{"value":""},"snapUrls":{"mediaUrl":"https://cf-st.sc-cdn.net/d/uxOSCj5RgvtbPc1WJFZE4.400.IRZXSOY?uc=12","mediaPreviewUrl":{"value":"https://cf-st.sc-cdn.net/d/uxOSCj5RgvtbPc1WJFZE4.410.IRZXSOY?uc=12"}},"timestampInSec":{"value":"1605705190"}}],"storyId":{"value":""},"storyTitle":{"value":""},"thumbnailUrl":{"value":"https://cf-st.sc-cdn.net/d/Cg5MaQODMG3TnzwDo9KIa.410.IRZXSOY?uc=12"}}],"spotlightHighlights":[],"spotlightHighlightsMetadata":[],"viewerInfo":{"country":"IN","locale":"en_US"},"localization":{"direction":0},"pageLinks":{"oneLinkUrl":"https://click.snapchat.com/aVHG?pid=snapchat_download_page\u0026af_dp=https://www.snapchat.com/add/mrunu11?sc_referrer%3Dweb\u0026af_web_dp=https://snapchat.com/download?purpose%3Dweb_stories","snapchatCanonicalUrl":"https://www.snapchat.com/add/mrunu11","canonicalUrl":"https://www.snapchat.com/add/mrunu11","snapcodeImageUrl":"https://app.snapchat.com/web/deeplink/snapcode?username=mrunu11\u0026type=SVG\u0026bitmoji=enable"},"pageMetadata":{"pageType":9,"pageTitle":"Mrunu (@mrunu11) on Snapchat","pageDescription":{"value":"Mrunu is on Snapchat!"}},"userProfile":{"$case":"publicProfileInfo","publicProfileInfo":{"username":"mrunu11","title":"Mrunu","snapcodeImageUrl":"https://app.snapchat.com/web/deeplink/snapcode?username=mrunu11\u0026type=SVG\u0026bitmoji=enable","badge":1,"categoryStringId":"public-profile-category-v3-people","subcategoryStringId":"public-profile-subcategory-v3-artist","subscriberCount":"874600","bio":"Welcome to my weird life ✨","websiteUrl":"https://youtube.com/c/GujjuUnicorn","profilePictureUrl":"https://cf-st.sc-cdn.net/aps/bolt/aHR0cHM6Ly9jZi1zdC5zYy1jZG4ubmV0L2QvdTVBZEFXVnV1RlVSNDNBQk5qRHVNP2JvPUVnMGFBQm9BTWdFRVNBSlFHV0FCJnVjPTI1._RS0,90_FMjpeg","address":"Mumbai, India, India","hasCuratedHighlights":true,"hasSpotlightHighlights":false,"mutableName":"","publisherType":"","squareHeroImageUrl":"","primaryColor":""}},"linkPreview":{"title":"mrunu11 on Snapchat","description":"","canonicalUrl":"https://story.snapchat.com/u/mrunu11","twitterImage":{"url":"https://story.snapchat.com/@mrunu11/preview/twitter.png","size":{"width":1200,"height":600}},"facebookImage":{"url":"https://story.snapchat.com/@mrunu11/preview/facebook.png","size":{"width":1200,"height":628}}}},"status":0,"log":{"levels":{"TRACE":0,"DEBUG":1,"INFO":2,"WARN":3,"ERROR":4,"SILENT":5}}},"page":"/@/[username]","query":{"username":"@mrunu11"},"buildId":"23576-9b597984705a8ea2bff65ac8abd3eb5a984c976a","assetPrefix":"https://story.snapchat.com","isFallback":false,"dynamicIds":["gkwE","+51n","AC5g","DbP8","KIpE","LQDX","NuZu","aLx/","qmXy","sZW5","sZkf"],"gip":true,"appGip":true}</script><script nomodule="" src="https://story.snapchat.com/_next/static/chunks/polyfills-553aafd328e99d1ecd5e.js"></script><script async="" src="https://story.snapchat.com/_next/static/chunks/049823d6.8b03ce304b0e44456f30.js"></script><script async="" src="https://story.snapchat.com/_next/static/chunks/22.ca59e6299b825dc862b0.js"></script><script src="https://story.snapchat.com/_next/static/chunks/webpack-edb54b561e62fb294b85.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/framework.efe182f2d62be1d8151a.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/c408797459d80c128d5e47906020fa02c3ea7a51.cdf474846c815ffe556c.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/f6078781a05fe1bcb0902d23dbbb2662c8d200b3.0cb66906a1ea3f804368.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/main-69ec1f1dba14cd9f620a.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/c1468a61a92675d836a3000bab1334fb54fd20a9.074f204d663a13469e0b.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/d241c1e27ffe07c251e6f8ab09888e7ecf8ae8dc.b20db949b32dafefad5c.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/d4fc9bc7fce3fa7dbb251df097e4d60e4f4a3ec9.6a57a5151732d06fa88a.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/pages/_app-9a2167e8d8d9d9f101c9.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/29107295.be25f8bc8bdde59f114d.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/641167d64809277a1b9199554823a0e631b3bff2.b1423abff274817ff848.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/96c0058ea2ce58b3f27756fc0d0be33ac3f6361c.4360e309b36814bc7496.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/64dd010a9368940fc41206bc54dfee6183397831.1358f9c5b56d2322e06e.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/bd9739576daf9a5525e7028695825e8d0c29e04c.65c9b0762abe3d67e2ce.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/f2142e6c893e00c2f1a27f144791418e507fc12c.1ef92cfd6920c8f93e61.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/e2ef7edf3a7e66ae27a9d163772f8c722ad47684.7e5591f9407dd7837830.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/61f94ab364ffeaf810caabbb5e8c59d41b273801.6e578c39745032b54013.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/d01c7d3028b0c7a5252ef883c5a43f5f0e747f01.5c6a4b590ccfff6d1784.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/pages/@/%5Busername%5D-19264ae3ee802be2dc6d.js" async=""></script><script src="https://story.snapchat.com/_next/static/23576-9b597984705a8ea2bff65ac8abd3eb5a984c976a/_buildManifest.js" async=""></script><script src="https://story.snapchat.com/_next/static/23576-9b597984705a8ea2bff65ac8abd3eb5a984c976a/_ssgManifest.js" async=""></script></body></html>
+
+<!DOCTYPE html><html prefix="og: https://ogp.me/ns#" dir="0" lang="en-US"><head><link data-react-helmet="true" rel="canonical" href="https://www.snapchat.com/add/mrunu11"/><meta data-react-helmet="true" name="description" content="Mrunu is on Snapchat!"/><meta data-react-helmet="true" name="apple-itunes-app" content="app-id=447188370, app-argument=https://www.snapchat.com/add/mrunu11"/><meta data-react-helmet="true" name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1.0, user-scalable=0"/><meta data-react-helmet="true" name="metrics-page-name" content="User_Profile.PublicProfile"/><meta data-react-helmet="true" property="og:title" content="mrunu11 on Snapchat"/><meta data-react-helmet="true" property="og:type" content="video.other"/><meta data-react-helmet="true" property="og:url" content="https://story.snapchat.com/u/mrunu11"/><meta data-react-helmet="true" property="og:image" content="https://story.snapchat.com/@mrunu11/preview/facebook.png"/><meta data-react-helmet="true" property="og:locale:alternate" content="ar_AA"/><meta data-react-helmet="true" property="og:locale:alternate" content="da_DK"/><meta data-react-helmet="true" property="og:locale:alternate" content="de_DK"/><meta data-react-helmet="true" property="og:locale:alternate" content="en_GB"/><meta data-react-helmet="true" property="og:locale:alternate" content="en_US"/><meta data-react-helmet="true" property="og:locale:alternate" content="es_ES"/><meta data-react-helmet="true" property="og:locale:alternate" content="es_MX"/><meta data-react-helmet="true" property="og:locale:alternate" content="fi_FI"/><meta data-react-helmet="true" property="og:locale:alternate" content="fr_FR"/><meta data-react-helmet="true" property="og:locale:alternate" content="it_IT"/><meta data-react-helmet="true" property="og:locale:alternate" content="ja_JP"/><meta data-react-helmet="true" property="og:locale:alternate" content="nb_NO"/><meta data-react-helmet="true" property="og:locale:alternate" content="nl_NL"/><meta data-react-helmet="true" property="og:locale:alternate" content="pt_BR"/><meta data-react-helmet="true" property="og:locale:alternate" content="sv_SE"/><meta data-react-helmet="true" property="og:image:width" content="1200"/><meta data-react-helmet="true" property="og:image:height" content="628"/><meta data-react-helmet="true" property="og:site_name" content="Snapchat"/><meta data-react-helmet="true" property="fb:app_id" content="394343577431007"/><meta data-react-helmet="true" property="fb:admins" content="1349731971"/><meta data-react-helmet="true" property="twitter:card" content="summary_large_image"/><meta data-react-helmet="true" property="twitter:site" content="@Snapchat"/><meta data-react-helmet="true" property="twitter:title" content="mrunu11 on Snapchat"/><meta data-react-helmet="true" property="twitter:image" content="https://story.snapchat.com/@mrunu11/preview/twitter.png"/><script data-react-helmet="true" async="" src="https://www.google-analytics.com/analytics.js"></script><script data-react-helmet="true">
+    window.ga=window.ga||function(){(ga.q = ga.q || []).push(arguments)};
+    ga.l=+new Date;
+    ga('create','UA-41740027-40', 'auto');
+    ga('send','pageview', location.pathname);
+  </script><style data-react-helmet="true">html {
+          height: 100%;
+          box-sizing: border-box;
+         }
+
+         body {
+          margin: 0;
+          height: 100%;
+          background: #121314;
+          font-family: Avenir Next, Helvetica, sans-serif;
+          -webkit-text-fill-color: currentcolor;
+         }
+
+         #__next, #root {
+          height: 100%;
+         }
+
+         *, *:before, *:after {
+          box-sizing: inherit;
+         }
+
+         button {
+          -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
+          -webkit-tap-highlight-color: transparent;
+          -webkit-user-select: none;
+          -khtml-user-select: none;
+          -moz-user-select: none;
+          -ms-user-select: none;
+          user-select: none;
+         }
+         </style><title data-react-helmet="true">Mrunu (@mrunu11) on Snapchat</title><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><noscript data-n-css=""></noscript><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/049823d6.8b03ce304b0e44456f30.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/22.ca59e6299b825dc862b0.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/webpack-edb54b561e62fb294b85.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/framework.efe182f2d62be1d8151a.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/c408797459d80c128d5e47906020fa02c3ea7a51.cdf474846c815ffe556c.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/f6078781a05fe1bcb0902d23dbbb2662c8d200b3.0cb66906a1ea3f804368.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/main-69ec1f1dba14cd9f620a.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/c1468a61a92675d836a3000bab1334fb54fd20a9.074f204d663a13469e0b.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/d241c1e27ffe07c251e6f8ab09888e7ecf8ae8dc.b20db949b32dafefad5c.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/d4fc9bc7fce3fa7dbb251df097e4d60e4f4a3ec9.6a57a5151732d06fa88a.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/pages/_app-9a2167e8d8d9d9f101c9.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/29107295.be25f8bc8bdde59f114d.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/641167d64809277a1b9199554823a0e631b3bff2.b1423abff274817ff848.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/96c0058ea2ce58b3f27756fc0d0be33ac3f6361c.4360e309b36814bc7496.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/64dd010a9368940fc41206bc54dfee6183397831.1358f9c5b56d2322e06e.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/bd9739576daf9a5525e7028695825e8d0c29e04c.65c9b0762abe3d67e2ce.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/f2142e6c893e00c2f1a27f144791418e507fc12c.1ef92cfd6920c8f93e61.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/e2ef7edf3a7e66ae27a9d163772f8c722ad47684.7e5591f9407dd7837830.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/61f94ab364ffeaf810caabbb5e8c59d41b273801.6e578c39745032b54013.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/d01c7d3028b0c7a5252ef883c5a43f5f0e747f01.5c6a4b590ccfff6d1784.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/pages/@/%5Busername%5D-19264ae3ee802be2dc6d.js" as="script"/></head><body id="root"><div id="__next"><style data-emotion="css-global cqw65k">@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.ttf") format("truetype");font-weight:100;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.ttf") format("truetype");font-weight:100;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.ttf") format("truetype");font-weight:200;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.ttf") format("truetype");font-weight:200;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Regular.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Regular.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Regular.ttf") format("truetype");font-weight:300;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Italic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Italic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Italic.ttf") format("truetype");font-weight:300;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Medium.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Medium.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Medium.ttf") format("truetype");font-weight:400;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-MediumItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-MediumItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-MediumItalic.ttf") format("truetype");font-weight:400;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-DemiBold.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-DemiBold.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-DemiBold.ttf") format("truetype");font-weight:500;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-DemiBoldItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-DemiBoldItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-DemiBoldItalic.ttf") format("truetype");font-weight:500;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Bold.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Bold.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Bold.ttf") format("truetype");font-weight:600;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.ttf") format("truetype");font-weight:600;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Bold.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Bold.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Bold.ttf") format("truetype");font-weight:700;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.ttf") format("truetype");font-weight:700;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Heavy.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Heavy.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Heavy.ttf") format("truetype");font-weight:800;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.ttf") format("truetype");font-weight:800;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Heavy.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Heavy.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Heavy.ttf") format("truetype");font-weight:900;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.ttf") format("truetype");font-weight:900;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Thin.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Thin.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Thin.ttf") format("truetype");font-weight:100;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ThinItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ThinItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ThinItalic.ttf") format("truetype");font-weight:100;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Extralight.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Extralight.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Extralight.ttf") format("truetype");font-weight:200;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ExtralightItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ExtralightItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ExtralightItalic.ttf") format("truetype");font-weight:200;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Light.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Light.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Light.ttf") format("truetype");font-weight:300;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-LightItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-LightItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-LightItalic.ttf") format("truetype");font-weight:300;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Regular.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Regular.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Regular.ttf") format("truetype");font-weight:400;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-RegularItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-RegularItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-RegularItalic.ttf") format("truetype");font-weight:400;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Medium.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Medium.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Medium.ttf") format("truetype");font-weight:500;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-MediumItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-MediumItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-MediumItalic.ttf") format("truetype");font-weight:500;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Semibold.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Semibold.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Semibold.ttf") format("truetype");font-weight:600;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SemiboldItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SemiboldItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SemiboldItalic.ttf") format("truetype");font-weight:600;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Bold.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Bold.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Bold.ttf") format("truetype");font-weight:700;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BoldItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BoldItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BoldItalic.ttf") format("truetype");font-weight:700;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Black.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Black.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Black.ttf") format("truetype");font-weight:800;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BlackItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BlackItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BlackItalic.ttf") format("truetype");font-weight:800;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Super.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Super.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Super.ttf") format("truetype");font-weight:900;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SuperItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SuperItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SuperItalic.ttf") format("truetype");font-weight:900;font-style:italic;font-display:block;}</style></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"googleAnalyticsPropertyId":"UA-41740027-40","localizedMessages":{"default":{"+9d+q7":"Nonprofit Organization","+ByJA/":"Stories","+hwkQQ":"Film / TV","+lhElX":"Copyright infringement","+o8gM9":"Kit","/Xkr+t":"by {creatorDisplayName}","/dF4HW":"Spotlight","/tNMyW":"Download","/vdS3s":"Download Snapchat to Watch Now","04qzmG":"You will now be taken to the next Snap - press 'Close' to do this right away or we will continue automatically in 10 seconds.","0FP975":"Post to Spotlight","0Y6c0W":"Restaurant Chain","0YKDxr":"Photographer","0dJz6S":"Threatening, violent, or concerning","0uHjye":"Share this Snap","1PzCdm":"It asks for or threatens to post inappropriate Snaps","1V8Uma":"Public Figure","1egAGi":"Movie Character","1kdcl2":"Media / News Company","2LLiYb":"Close","2V40yT":"More Options","2l730k":"Film / TV Personality","4V5k0y":"Support","5HsSrO":"I just don't like it","5XW8Zd":"{subscriberCount} Subscribers","5m3Hu8":"I'm worried this Snapchatter might hurt themselves","5v6wP7":"Motivational Speaker","5zZGnG":"Writer","6yvoZD":"Sorry,","7BHw3h":"Religious Organization","7HP0Jf":"Coach","7XZM2L":"Business","7rVnIj":"Spotlight","7xehRy":"Producer","7yuYaU":"Businesses \u0026 Groups","8Sw4jY":"Report Snap","9NRv3Z":"Snapcodes","ATeDiR":"Thank you for reporting this Snap.","AbkQPs":"It's an invasion of privacy","AtLF/u":"This content was not found","CAgCZ5":"Nudity or sexual content","CJBFGo":"Politician","CVucIf":"Community Organization","DY4yHA":"Brand","EPBE+l":"Government Official","ESomE8":"Submit","Eqnt63":"{timeDifference}m ago","FDOu63":"Someone else is being bullied or harassed","Fsg136":"Episode {episodeNumber}","Ftta6c":"It's threatening a person or place","G7hRik":"Spotlight is not available in your location","GJZs5E":"It's spam","GVLbZP":"Stories","GaNuM2":"Best of Spotlight","Gh1a/j":"Food Professional","GssbOn":"Product","Gvuqme":"It's an inappropriate Snap of someone else","HLxWNM":"It sells or promotes inappropriate Snaps","HVgZaB":"Creator","HkaOsh":"Open your Snapchat","I1rLjL":"Ads","I6sovq":"Political Organization","IWKERN":"Fashion Model","JbCR5V":"This content is not available","Ju77ns":"Comedian","MDthgV":"Sports League","MN6Znh":"Watch more in Snapchat","MUzWB7":"Please provide your Snapchat username if you have one, and the email associated with your account","N7Wq/c":"Violent or disturbing","N7iI/k":"Download Snapchat to find more","NXPVkv":"Company / Enterprise","P6YGQz":"Open in Snapchat","PQcLi/":"Service","PyzdXL":"Cancel","Q4RuCH":"Maps","Q71IbU":"Government Organization","QdGWFE":"Season {seasonNumber}","RJo0Z3":"Harassment or Hate speech","RmE5lP":"Lifestyle Influencer","RtNy71":"Musician / Band","SCe4GQ":"Film Director","SVOJKh":"Video Game","SgFTtk":"Up next","TNK/W/":"Lenses","Tm6yFt":"Download Snapchat","UIZTzu":"It's attempting to buy or sell drugs or weapons","Uk55sM":"Add me on Snapchat!","VRmDFV":"Snap Reported","VZQx67":"This Snap is no longer available","VjDaWB":"Watch more from {publisherTitle}","W07I8V":"Share {username}'s Snap","WGtpBM":"People","WyUwHm":"They are pretending to be me","XbXoMR":"Actor","YhMtYd":"Spectacles","Yt2+ye":"My Story","ZPrHrl":"Internet Company","ZViZgq":"Traveler","ZlJO0Q":"Apparel / Fashion","ZvzVyN":"Top Lenses","aSXQy0":"Sports Personality","ah6l3c":"Charity / Cause","ais8eK":"Group","by2dgE":"News Personality","dAksd9":"Journalist","dItw6q":"Dancer","dJDu/3":"Entrepreneur","dkWyPr":"Vlogger / Blogger","fPIy5v":"Retail Company","fxAji7":"Filters \u0026 Lenses","hPxDQC":"Video Game Creator","jWa4OT":"College / University","jqpH+5":"Is there any more information you want to share about this Snap?","kNCf90":"Products \u0026 Brands","kzoiEX":"{timeDifference}h ago","l1fnUG":"Scientist","lbui+i":"It's hate speech targeting me or another group","nbiOpp":"Lens Studio","ojrZ4G":"Download","pCK8FJ":"Artist","pPIiOl":"{subscriberCount} Subscribers","rL8HYz":"Professional Gamer","rLGZZX":"Just now","rNVPnk":"It's an inappropriate Snap of me","rrdPgT":"Store","rsYMnU":"Episodes","sRM8i5":"Why do you want to report this Snap?","sVcU8q":"Posted to Snap Map","tYFb/P":"Spotlight","vTd+a8":"I'm being bullied or harassed","vqdER6":"Fitness Professional","wVfxbD":"Political Candidate","wpLx7z":"Lens Creator","x1C/5K":"Person","x4F6zb":"Report Snap","xLaO8v":"Health / Beauty","yT6a3h":"In this Snap","ys7Y26":"Athlete","zExXNB":"Sports Team"},"+9d+q7":"Nonprofit Organization","+ByJA/":"Stories","+hwkQQ":"Film / TV","+lhElX":"Copyright infringement","+o8gM9":"Kit","/Xkr+t":"by {creatorDisplayName}","/dF4HW":"Spotlight","/tNMyW":"Download","/vdS3s":"Download Snapchat to Watch Now","04qzmG":"You will now be taken to the next Snap - press 'Close' to do this right away or we will continue automatically in 10 seconds.","0FP975":"Post to Spotlight","0Y6c0W":"Restaurant Chain","0YKDxr":"Photographer","0dJz6S":"Threatening, violent, or concerning","0uHjye":"Share this Snap","1PzCdm":"It asks for or threatens to post inappropriate Snaps","1V8Uma":"Public Figure","1egAGi":"Movie Character","1kdcl2":"Media / News Company","2LLiYb":"Close","2V40yT":"More Options","2l730k":"Film / TV Personality","4V5k0y":"Support","5HsSrO":"I just don't like it","5XW8Zd":"{subscriberCount} Subscribers","5m3Hu8":"I'm worried this Snapchatter might hurt themselves","5v6wP7":"Motivational Speaker","5zZGnG":"Writer","6yvoZD":"Sorry,","7BHw3h":"Religious Organization","7HP0Jf":"Coach","7XZM2L":"Business","7rVnIj":"Spotlight","7xehRy":"Producer","7yuYaU":"Businesses \u0026 Groups","8Sw4jY":"Report Snap","9NRv3Z":"Snapcodes","ATeDiR":"Thank you for reporting this Snap.","AbkQPs":"It's an invasion of privacy","AtLF/u":"This content was not found","CAgCZ5":"Nudity or sexual content","CJBFGo":"Politician","CVucIf":"Community Organization","DY4yHA":"Brand","EPBE+l":"Government Official","ESomE8":"Submit","Eqnt63":"{timeDifference}m ago","FDOu63":"Someone else is being bullied or harassed","Fsg136":"Episode {episodeNumber}","Ftta6c":"It's threatening a person or place","G7hRik":"Spotlight is not available in your location","GJZs5E":"It's spam","GVLbZP":"Stories","GaNuM2":"Best of Spotlight","Gh1a/j":"Food Professional","GssbOn":"Product","Gvuqme":"It's an inappropriate Snap of someone else","HLxWNM":"It sells or promotes inappropriate Snaps","HVgZaB":"Creator","HkaOsh":"Open your Snapchat","I1rLjL":"Ads","I6sovq":"Political Organization","IWKERN":"Fashion Model","JbCR5V":"This content is not available","Ju77ns":"Comedian","MDthgV":"Sports League","MN6Znh":"Watch more in Snapchat","MUzWB7":"Please provide your Snapchat username if you have one, and the email associated with your account","N7Wq/c":"Violent or disturbing","N7iI/k":"Download Snapchat to find more","NXPVkv":"Company / Enterprise","P6YGQz":"Open in Snapchat","PQcLi/":"Service","PyzdXL":"Cancel","Q4RuCH":"Maps","Q71IbU":"Government Organization","QdGWFE":"Season {seasonNumber}","RJo0Z3":"Harassment or Hate speech","RmE5lP":"Lifestyle Influencer","RtNy71":"Musician / Band","SCe4GQ":"Film Director","SVOJKh":"Video Game","SgFTtk":"Up next","TNK/W/":"Lenses","Tm6yFt":"Download Snapchat","UIZTzu":"It's attempting to buy or sell drugs or weapons","Uk55sM":"Add me on Snapchat!","VRmDFV":"Snap Reported","VZQx67":"This Snap is no longer available","VjDaWB":"Watch more from {publisherTitle}","W07I8V":"Share {username}'s Snap","WGtpBM":"People","WyUwHm":"They are pretending to be me","XbXoMR":"Actor","YhMtYd":"Spectacles","Yt2+ye":"My Story","ZPrHrl":"Internet Company","ZViZgq":"Traveler","ZlJO0Q":"Apparel / Fashion","ZvzVyN":"Top Lenses","aSXQy0":"Sports Personality","ah6l3c":"Charity / Cause","ais8eK":"Group","by2dgE":"News Personality","dAksd9":"Journalist","dItw6q":"Dancer","dJDu/3":"Entrepreneur","dkWyPr":"Vlogger / Blogger","fPIy5v":"Retail Company","fxAji7":"Filters \u0026 Lenses","hPxDQC":"Video Game Creator","jWa4OT":"College / University","jqpH+5":"Is there any more information you want to share about this Snap?","kNCf90":"Products \u0026 Brands","kzoiEX":"{timeDifference}h ago","l1fnUG":"Scientist","lbui+i":"It's hate speech targeting me or another group","nbiOpp":"Lens Studio","ojrZ4G":"Download","pCK8FJ":"Artist","pPIiOl":"{subscriberCount} Subscribers","rL8HYz":"Professional Gamer","rLGZZX":"Just now","rNVPnk":"It's an inappropriate Snap of me","rrdPgT":"Store","rsYMnU":"Episodes","sRM8i5":"Why do you want to report this Snap?","sVcU8q":"Posted to Snap Map","tYFb/P":"Spotlight","vTd+a8":"I'm being bullied or harassed","vqdER6":"Fitness Professional","wVfxbD":"Political Candidate","wpLx7z":"Lens Creator","x1C/5K":"Person","x4F6zb":"Report Snap","xLaO8v":"Health / Beauty","yT6a3h":"In this Snap","ys7Y26":"Athlete","zExXNB":"Sports Team"},"lenses":[],"curatedHighlights":[{"storyType":3,"storyTapId":"0","snapList":[{"snapIndex":0,"snapMediaType":0,"snapId":{"value":""},"snapUrls":{"mediaUrl":"https://cf-st.sc-cdn.net/d/Cg5MaQODMG3TnzwDo9KIa.400.IRZXSOY?uc=12","mediaPreviewUrl":{"value":"https://cf-st.sc-cdn.net/d/Cg5MaQODMG3TnzwDo9KIa.410.IRZXSOY?uc=12"}},"timestampInSec":{"value":"1606531630"}},{"snapIndex":1,"snapMediaType":0,"snapId":{"value":""},"snapUrls":{"mediaUrl":"https://cf-st.sc-cdn.net/d/uxOSCj5RgvtbPc1WJFZE4.400.IRZXSOY?uc=12","mediaPreviewUrl":{"value":"https://cf-st.sc-cdn.net/d/uxOSCj5RgvtbPc1WJFZE4.410.IRZXSOY?uc=12"}},"timestampInSec":{"value":"1605705190"}}],"storyId":{"value":""},"storyTitle":{"value":""},"thumbnailUrl":{"value":"https://cf-st.sc-cdn.net/d/Cg5MaQODMG3TnzwDo9KIa.410.IRZXSOY?uc=12"}}],"spotlightHighlights":[],"spotlightHighlightsMetadata":[],"viewerInfo":{"country":"IN","locale":"en_US"},"localization":{"direction":0},"pageLinks":{"oneLinkUrl":"https://click.snapchat.com/aVHG?pid=snapchat_download_page\u0026af_dp=https://www.snapchat.com/add/mrunu11?sc_referrer%3Dweb\u0026af_web_dp=https://snapchat.com/download?purpose%3Dweb_stories","snapchatCanonicalUrl":"https://www.snapchat.com/add/mrunu11","canonicalUrl":"https://www.snapchat.com/add/mrunu11","snapcodeImageUrl":"https://app.snapchat.com/web/deeplink/snapcode?username=mrunu11\u0026type=SVG\u0026bitmoji=enable"},"pageMetadata":{"pageType":9,"pageTitle":"Mrunu (@mrunu11) on Snapchat","pageDescription":{"value":"Mrunu is on Snapchat!"}},"userProfile":{"$case":"publicProfileInfo","publicProfileInfo":{"username":"mrunu11","title":"Mrunu","snapcodeImageUrl":"https://app.snapchat.com/web/deeplink/snapcode?username=mrunu11\u0026type=SVG\u0026bitmoji=enable","badge":1,"categoryStringId":"public-profile-category-v3-people","subcategoryStringId":"public-profile-subcategory-v3-artist","subscriberCount":"874600","bio":"Welcome to my weird life ✨","websiteUrl":"https://youtube.com/c/GujjuUnicorn","profilePictureUrl":"https://cf-st.sc-cdn.net/aps/bolt/aHR0cHM6Ly9jZi1zdC5zYy1jZG4ubmV0L2QvdTVBZEFXVnV1RlVSNDNBQk5qRHVNP2JvPUVnMGFBQm9BTWdFRVNBSlFHV0FCJnVjPTI1._RS0,90_FMjpeg","address":"Mumbai, India, India","hasCuratedHighlights":true,"hasSpotlightHighlights":false,"mutableName":"","publisherType":"","squareHeroImageUrl":"","primaryColor":""}},"linkPreview":{"title":"mrunu11 on Snapchat","description":"","canonicalUrl":"https://story.snapchat.com/u/mrunu11","twitterImage":{"url":"https://story.snapchat.com/@mrunu11/preview/twitter.png","size":{"width":1200,"height":600}},"facebookImage":{"url":"https://story.snapchat.com/@mrunu11/preview/facebook.png","size":{"width":1200,"height":628}}}},"status":0,"log":{"levels":{"TRACE":0,"DEBUG":1,"INFO":2,"WARN":3,"ERROR":4,"SILENT":5}}},"page":"/@/[username]","query":{"username":"@mrunu11"},"buildId":"23576-9b597984705a8ea2bff65ac8abd3eb5a984c976a","assetPrefix":"https://story.snapchat.com","isFallback":false,"dynamicIds":["gkwE","+51n","AC5g","DbP8","KIpE","LQDX","NuZu","aLx/","qmXy","sZW5","sZkf"],"gip":true,"appGip":true}</script><script nomodule="" src="https://story.snapchat.com/_next/static/chunks/polyfills-553aafd328e99d1ecd5e.js"></script><script async="" src="https://story.snapchat.com/_next/static/chunks/049823d6.8b03ce304b0e44456f30.js"></script><script async="" src="https://story.snapchat.com/_next/static/chunks/22.ca59e6299b825dc862b0.js"></script><script src="https://story.snapchat.com/_next/static/chunks/webpack-edb54b561e62fb294b85.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/framework.efe182f2d62be1d8151a.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/c408797459d80c128d5e47906020fa02c3ea7a51.cdf474846c815ffe556c.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/f6078781a05fe1bcb0902d23dbbb2662c8d200b3.0cb66906a1ea3f804368.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/main-69ec1f1dba14cd9f620a.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/c1468a61a92675d836a3000bab1334fb54fd20a9.074f204d663a13469e0b.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/d241c1e27ffe07c251e6f8ab09888e7ecf8ae8dc.b20db949b32dafefad5c.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/d4fc9bc7fce3fa7dbb251df097e4d60e4f4a3ec9.6a57a5151732d06fa88a.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/pages/_app-9a2167e8d8d9d9f101c9.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/29107295.be25f8bc8bdde59f114d.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/641167d64809277a1b9199554823a0e631b3bff2.b1423abff274817ff848.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/96c0058ea2ce58b3f27756fc0d0be33ac3f6361c.4360e309b36814bc7496.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/64dd010a9368940fc41206bc54dfee6183397831.1358f9c5b56d2322e06e.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/bd9739576daf9a5525e7028695825e8d0c29e04c.65c9b0762abe3d67e2ce.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/f2142e6c893e00c2f1a27f144791418e507fc12c.1ef92cfd6920c8f93e61.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/e2ef7edf3a7e66ae27a9d163772f8c722ad47684.7e5591f9407dd7837830.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/61f94ab364ffeaf810caabbb5e8c59d41b273801.6e578c39745032b54013.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/d01c7d3028b0c7a5252ef883c5a43f5f0e747f01.5c6a4b590ccfff6d1784.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/pages/@/%5Busername%5D-19264ae3ee802be2dc6d.js" async=""></script><script src="https://story.snapchat.com/_next/static/23576-9b597984705a8ea2bff65ac8abd3eb5a984c976a/_buildManifest.js" async=""></script><script src="https://story.snapchat.com/_next/static/23576-9b597984705a8ea2bff65ac8abd3eb5a984c976a/_ssgManifest.js" async=""></script></body></html>
```

### Comparing `snapchat-dlp-1.5.2/tests/mock_data/invalidusername.html` & `snapchat-dlp-1.5.8/tests/mock_data/invalidusername.html`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-
-<!DOCTYPE html><html prefix="og: https://ogp.me/ns#" dir="0" lang="en-US"><head><link data-react-helmet="true" rel="canonical" href="https://www.snapchat.com/add/invalidusername"/><meta data-react-helmet="true" name="description" content="Mrunu is on Snapchat!"/><meta data-react-helmet="true" name="apple-itunes-app" content="app-id=447188370, app-argument=https://www.snapchat.com/add/invalidusername"/><meta data-react-helmet="true" name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1.0, user-scalable=0"/><meta data-react-helmet="true" name="metrics-page-name" content="User_Profile.PublicProfile"/><meta data-react-helmet="true" property="og:title" content="invalidusername on Snapchat"/><meta data-react-helmet="true" property="og:type" content="video.other"/><meta data-react-helmet="true" property="og:url" content="https://story.snapchat.com/u/invalidusername"/><meta data-react-helmet="true" property="og:image" content="https://story.snapchat.com/@invalidusername/preview/facebook.png"/><meta data-react-helmet="true" property="og:locale:alternate" content="ar_AA"/><meta data-react-helmet="true" property="og:locale:alternate" content="da_DK"/><meta data-react-helmet="true" property="og:locale:alternate" content="de_DK"/><meta data-react-helmet="true" property="og:locale:alternate" content="en_GB"/><meta data-react-helmet="true" property="og:locale:alternate" content="en_US"/><meta data-react-helmet="true" property="og:locale:alternate" content="es_ES"/><meta data-react-helmet="true" property="og:locale:alternate" content="es_MX"/><meta data-react-helmet="true" property="og:locale:alternate" content="fi_FI"/><meta data-react-helmet="true" property="og:locale:alternate" content="fr_FR"/><meta data-react-helmet="true" property="og:locale:alternate" content="it_IT"/><meta data-react-helmet="true" property="og:locale:alternate" content="ja_JP"/><meta data-react-helmet="true" property="og:locale:alternate" content="nb_NO"/><meta data-react-helmet="true" property="og:locale:alternate" content="nl_NL"/><meta data-react-helmet="true" property="og:locale:alternate" content="pt_BR"/><meta data-react-helmet="true" property="og:locale:alternate" content="sv_SE"/><meta data-react-helmet="true" property="og:image:width" content="1200"/><meta data-react-helmet="true" property="og:image:height" content="628"/><meta data-react-helmet="true" property="og:site_name" content="Snapchat"/><meta data-react-helmet="true" property="fb:app_id" content="394343577431007"/><meta data-react-helmet="true" property="fb:admins" content="1349731971"/><meta data-react-helmet="true" property="twitter:card" content="summary_large_image"/><meta data-react-helmet="true" property="twitter:site" content="@Snapchat"/><meta data-react-helmet="true" property="twitter:title" content="invalidusername on Snapchat"/><meta data-react-helmet="true" property="twitter:image" content="https://story.snapchat.com/@invalidusername/preview/twitter.png"/><script data-react-helmet="true" async="" src="https://www.google-analytics.com/analytics.js"></script><script data-react-helmet="true">
-    window.ga=window.ga||function(){(ga.q = ga.q || []).push(arguments)};
-    ga.l=+new Date;
-    ga('create','UA-41740027-40', 'auto');
-    ga('send','pageview', location.pathname);
-  </script><style data-react-helmet="true">html {
-          height: 100%;
-          box-sizing: border-box;
-         }
-
-         body {
-          margin: 0;
-          height: 100%;
-          background: #121314;
-          font-family: Avenir Next, Helvetica, sans-serif;
-          -webkit-text-fill-color: currentcolor;
-         }
-
-         #__next, #root {
-          height: 100%;
-         }
-
-         *, *:before, *:after {
-          box-sizing: inherit;
-         }
-
-         button {
-          -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
-          -webkit-tap-highlight-color: transparent;
-          -webkit-user-select: none;
-          -khtml-user-select: none;
-          -moz-user-select: none;
-          -ms-user-select: none;
-          user-select: none;
-         }
-         </style><title data-react-helmet="true">Mrunu (@invalidusername) on Snapchat</title><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><noscript data-n-css=""></noscript><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/049823d6.8b03ce304b0e44456f30.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/22.ca59e6299b825dc862b0.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/webpack-edb54b561e62fb294b85.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/framework.efe182f2d62be1d8151a.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/c408797459d80c128d5e47906020fa02c3ea7a51.cdf474846c815ffe556c.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/f6078781a05fe1bcb0902d23dbbb2662c8d200b3.0cb66906a1ea3f804368.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/main-69ec1f1dba14cd9f620a.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/c1468a61a92675d836a3000bab1334fb54fd20a9.074f204d663a13469e0b.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/d241c1e27ffe07c251e6f8ab09888e7ecf8ae8dc.b20db949b32dafefad5c.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/d4fc9bc7fce3fa7dbb251df097e4d60e4f4a3ec9.6a57a5151732d06fa88a.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/pages/_app-9a2167e8d8d9d9f101c9.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/29107295.be25f8bc8bdde59f114d.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/641167d64809277a1b9199554823a0e631b3bff2.b1423abff274817ff848.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/96c0058ea2ce58b3f27756fc0d0be33ac3f6361c.4360e309b36814bc7496.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/64dd010a9368940fc41206bc54dfee6183397831.1358f9c5b56d2322e06e.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/bd9739576daf9a5525e7028695825e8d0c29e04c.65c9b0762abe3d67e2ce.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/f2142e6c893e00c2f1a27f144791418e507fc12c.1ef92cfd6920c8f93e61.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/e2ef7edf3a7e66ae27a9d163772f8c722ad47684.7e5591f9407dd7837830.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/61f94ab364ffeaf810caabbb5e8c59d41b273801.6e578c39745032b54013.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/d01c7d3028b0c7a5252ef883c5a43f5f0e747f01.5c6a4b590ccfff6d1784.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/pages/@/%5Busername%5D-19264ae3ee802be2dc6d.js" as="script"/></head><body id="root"><div id="__next"><style data-emotion="css-global cqw65k">@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.ttf") format("truetype");font-weight:100;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.ttf") format("truetype");font-weight:100;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.ttf") format("truetype");font-weight:200;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.ttf") format("truetype");font-weight:200;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Regular.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Regular.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Regular.ttf") format("truetype");font-weight:300;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Italic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Italic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Italic.ttf") format("truetype");font-weight:300;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Medium.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Medium.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Medium.ttf") format("truetype");font-weight:400;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-MediumItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-MediumItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-MediumItalic.ttf") format("truetype");font-weight:400;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-DemiBold.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-DemiBold.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-DemiBold.ttf") format("truetype");font-weight:500;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-DemiBoldItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-DemiBoldItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-DemiBoldItalic.ttf") format("truetype");font-weight:500;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Bold.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Bold.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Bold.ttf") format("truetype");font-weight:600;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.ttf") format("truetype");font-weight:600;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Bold.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Bold.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Bold.ttf") format("truetype");font-weight:700;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.ttf") format("truetype");font-weight:700;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Heavy.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Heavy.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Heavy.ttf") format("truetype");font-weight:800;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.ttf") format("truetype");font-weight:800;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Heavy.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Heavy.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Heavy.ttf") format("truetype");font-weight:900;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.ttf") format("truetype");font-weight:900;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Thin.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Thin.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Thin.ttf") format("truetype");font-weight:100;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ThinItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ThinItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ThinItalic.ttf") format("truetype");font-weight:100;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Extralight.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Extralight.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Extralight.ttf") format("truetype");font-weight:200;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ExtralightItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ExtralightItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ExtralightItalic.ttf") format("truetype");font-weight:200;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Light.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Light.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Light.ttf") format("truetype");font-weight:300;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-LightItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-LightItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-LightItalic.ttf") format("truetype");font-weight:300;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Regular.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Regular.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Regular.ttf") format("truetype");font-weight:400;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-RegularItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-RegularItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-RegularItalic.ttf") format("truetype");font-weight:400;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Medium.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Medium.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Medium.ttf") format("truetype");font-weight:500;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-MediumItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-MediumItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-MediumItalic.ttf") format("truetype");font-weight:500;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Semibold.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Semibold.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Semibold.ttf") format("truetype");font-weight:600;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SemiboldItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SemiboldItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SemiboldItalic.ttf") format("truetype");font-weight:600;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Bold.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Bold.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Bold.ttf") format("truetype");font-weight:700;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BoldItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BoldItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BoldItalic.ttf") format("truetype");font-weight:700;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Black.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Black.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Black.ttf") format("truetype");font-weight:800;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BlackItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BlackItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BlackItalic.ttf") format("truetype");font-weight:800;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Super.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Super.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Super.ttf") format("truetype");font-weight:900;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SuperItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SuperItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SuperItalic.ttf") format("truetype");font-weight:900;font-style:italic;font-display:block;}</style></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"googleAnalyticsPropertyId":"UA-41740027-40","localizedMessages":{"default":{"+9d+q7":"Nonprofit Organization","+ByJA/":"Stories","+hwkQQ":"Film / TV","+lhElX":"Copyright infringement","+o8gM9":"Kit","/Xkr+t":"by {creatorDisplayName}","/dF4HW":"Spotlight","/tNMyW":"Download","/vdS3s":"Download Snapchat to Watch Now","04qzmG":"You will now be taken to the next Snap - press 'Close' to do this right away or we will continue automatically in 10 seconds.","0FP975":"Post to Spotlight","0Y6c0W":"Restaurant Chain","0YKDxr":"Photographer","0dJz6S":"Threatening, violent, or concerning","0uHjye":"Share this Snap","1PzCdm":"It asks for or threatens to post inappropriate Snaps","1V8Uma":"Public Figure","1egAGi":"Movie Character","1kdcl2":"Media / News Company","2LLiYb":"Close","2V40yT":"More Options","2l730k":"Film / TV Personality","4V5k0y":"Support","5HsSrO":"I just don't like it","5XW8Zd":"{subscriberCount} Subscribers","5m3Hu8":"I'm worried this Snapchatter might hurt themselves","5v6wP7":"Motivational Speaker","5zZGnG":"Writer","6yvoZD":"Sorry,","7BHw3h":"Religious Organization","7HP0Jf":"Coach","7XZM2L":"Business","7rVnIj":"Spotlight","7xehRy":"Producer","7yuYaU":"Businesses \u0026 Groups","8Sw4jY":"Report Snap","9NRv3Z":"Snapcodes","ATeDiR":"Thank you for reporting this Snap.","AbkQPs":"It's an invasion of privacy","AtLF/u":"This content was not found","CAgCZ5":"Nudity or sexual content","CJBFGo":"Politician","CVucIf":"Community Organization","DY4yHA":"Brand","EPBE+l":"Government Official","ESomE8":"Submit","Eqnt63":"{timeDifference}m ago","FDOu63":"Someone else is being bullied or harassed","Fsg136":"Episode {episodeNumber}","Ftta6c":"It's threatening a person or place","G7hRik":"Spotlight is not available in your location","GJZs5E":"It's spam","GVLbZP":"Stories","GaNuM2":"Best of Spotlight","Gh1a/j":"Food Professional","GssbOn":"Product","Gvuqme":"It's an inappropriate Snap of someone else","HLxWNM":"It sells or promotes inappropriate Snaps","HVgZaB":"Creator","HkaOsh":"Open your Snapchat","I1rLjL":"Ads","I6sovq":"Political Organization","IWKERN":"Fashion Model","JbCR5V":"This content is not available","Ju77ns":"Comedian","MDthgV":"Sports League","MN6Znh":"Watch more in Snapchat","MUzWB7":"Please provide your Snapchat username if you have one, and the email associated with your account","N7Wq/c":"Violent or disturbing","N7iI/k":"Download Snapchat to find more","NXPVkv":"Company / Enterprise","P6YGQz":"Open in Snapchat","PQcLi/":"Service","PyzdXL":"Cancel","Q4RuCH":"Maps","Q71IbU":"Government Organization","QdGWFE":"Season {seasonNumber}","RJo0Z3":"Harassment or Hate speech","RmE5lP":"Lifestyle Influencer","RtNy71":"Musician / Band","SCe4GQ":"Film Director","SVOJKh":"Video Game","SgFTtk":"Up next","TNK/W/":"Lenses","Tm6yFt":"Download Snapchat","UIZTzu":"It's attempting to buy or sell drugs or weapons","Uk55sM":"Add me on Snapchat!","VRmDFV":"Snap Reported","VZQx67":"This Snap is no longer available","VjDaWB":"Watch more from {publisherTitle}","W07I8V":"Share {username}'s Snap","WGtpBM":"People","WyUwHm":"They are pretending to be me","XbXoMR":"Actor","YhMtYd":"Spectacles","Yt2+ye":"My Story","ZPrHrl":"Internet Company","ZViZgq":"Traveler","ZlJO0Q":"Apparel / Fashion","ZvzVyN":"Top Lenses","aSXQy0":"Sports Personality","ah6l3c":"Charity / Cause","ais8eK":"Group","by2dgE":"News Personality","dAksd9":"Journalist","dItw6q":"Dancer","dJDu/3":"Entrepreneur","dkWyPr":"Vlogger / Blogger","fPIy5v":"Retail Company","fxAji7":"Filters \u0026 Lenses","hPxDQC":"Video Game Creator","jWa4OT":"College / University","jqpH+5":"Is there any more information you want to share about this Snap?","kNCf90":"Products \u0026 Brands","kzoiEX":"{timeDifference}h ago","l1fnUG":"Scientist","lbui+i":"It's hate speech targeting me or another group","nbiOpp":"Lens Studio","ojrZ4G":"Download","pCK8FJ":"Artist","pPIiOl":"{subscriberCount} Subscribers","rL8HYz":"Professional Gamer","rLGZZX":"Just now","rNVPnk":"It's an inappropriate Snap of me","rrdPgT":"Store","rsYMnU":"Episodes","sRM8i5":"Why do you want to report this Snap?","sVcU8q":"Posted to Snap Map","tYFb/P":"Spotlight","vTd+a8":"I'm being bullied or harassed","vqdER6":"Fitness Professional","wVfxbD":"Political Candidate","wpLx7z":"Lens Creator","x1C/5K":"Person","x4F6zb":"Report Snap","xLaO8v":"Health / Beauty","yT6a3h":"In this Snap","ys7Y26":"Athlete","zExXNB":"Sports Team"},"+9d+q7":"Nonprofit Organization","+ByJA/":"Stories","+hwkQQ":"Film / TV","+lhElX":"Copyright infringement","+o8gM9":"Kit","/Xkr+t":"by {creatorDisplayName}","/dF4HW":"Spotlight","/tNMyW":"Download","/vdS3s":"Download Snapchat to Watch Now","04qzmG":"You will now be taken to the next Snap - press 'Close' to do this right away or we will continue automatically in 10 seconds.","0FP975":"Post to Spotlight","0Y6c0W":"Restaurant Chain","0YKDxr":"Photographer","0dJz6S":"Threatening, violent, or concerning","0uHjye":"Share this Snap","1PzCdm":"It asks for or threatens to post inappropriate Snaps","1V8Uma":"Public Figure","1egAGi":"Movie Character","1kdcl2":"Media / News Company","2LLiYb":"Close","2V40yT":"More Options","2l730k":"Film / TV Personality","4V5k0y":"Support","5HsSrO":"I just don't like it","5XW8Zd":"{subscriberCount} Subscribers","5m3Hu8":"I'm worried this Snapchatter might hurt themselves","5v6wP7":"Motivational Speaker","5zZGnG":"Writer","6yvoZD":"Sorry,","7BHw3h":"Religious Organization","7HP0Jf":"Coach","7XZM2L":"Business","7rVnIj":"Spotlight","7xehRy":"Producer","7yuYaU":"Businesses \u0026 Groups","8Sw4jY":"Report Snap","9NRv3Z":"Snapcodes","ATeDiR":"Thank you for reporting this Snap.","AbkQPs":"It's an invasion of privacy","AtLF/u":"This content was not found","CAgCZ5":"Nudity or sexual content","CJBFGo":"Politician","CVucIf":"Community Organization","DY4yHA":"Brand","EPBE+l":"Government Official","ESomE8":"Submit","Eqnt63":"{timeDifference}m ago","FDOu63":"Someone else is being bullied or harassed","Fsg136":"Episode {episodeNumber}","Ftta6c":"It's threatening a person or place","G7hRik":"Spotlight is not available in your location","GJZs5E":"It's spam","GVLbZP":"Stories","GaNuM2":"Best of Spotlight","Gh1a/j":"Food Professional","GssbOn":"Product","Gvuqme":"It's an inappropriate Snap of someone else","HLxWNM":"It sells or promotes inappropriate Snaps","HVgZaB":"Creator","HkaOsh":"Open your Snapchat","I1rLjL":"Ads","I6sovq":"Political Organization","IWKERN":"Fashion Model","JbCR5V":"This content is not available","Ju77ns":"Comedian","MDthgV":"Sports League","MN6Znh":"Watch more in Snapchat","MUzWB7":"Please provide your Snapchat username if you have one, and the email associated with your account","N7Wq/c":"Violent or disturbing","N7iI/k":"Download Snapchat to find more","NXPVkv":"Company / Enterprise","P6YGQz":"Open in Snapchat","PQcLi/":"Service","PyzdXL":"Cancel","Q4RuCH":"Maps","Q71IbU":"Government Organization","QdGWFE":"Season {seasonNumber}","RJo0Z3":"Harassment or Hate speech","RmE5lP":"Lifestyle Influencer","RtNy71":"Musician / Band","SCe4GQ":"Film Director","SVOJKh":"Video Game","SgFTtk":"Up next","TNK/W/":"Lenses","Tm6yFt":"Download Snapchat","UIZTzu":"It's attempting to buy or sell drugs or weapons","Uk55sM":"Add me on Snapchat!","VRmDFV":"Snap Reported","VZQx67":"This Snap is no longer available","VjDaWB":"Watch more from {publisherTitle}","W07I8V":"Share {username}'s Snap","WGtpBM":"People","WyUwHm":"They are pretending to be me","XbXoMR":"Actor","YhMtYd":"Spectacles","Yt2+ye":"My Story","ZPrHrl":"Internet Company","ZViZgq":"Traveler","ZlJO0Q":"Apparel / Fashion","ZvzVyN":"Top Lenses","aSXQy0":"Sports Personality","ah6l3c":"Charity / Cause","ais8eK":"Group","by2dgE":"News Personality","dAksd9":"Journalist","dItw6q":"Dancer","dJDu/3":"Entrepreneur","dkWyPr":"Vlogger / Blogger","fPIy5v":"Retail Company","fxAji7":"Filters \u0026 Lenses","hPxDQC":"Video Game Creator","jWa4OT":"College / University","jqpH+5":"Is there any more information you want to share about this Snap?","kNCf90":"Products \u0026 Brands","kzoiEX":"{timeDifference}h ago","l1fnUG":"Scientist","lbui+i":"It's hate speech targeting me or another group","nbiOpp":"Lens Studio","ojrZ4G":"Download","pCK8FJ":"Artist","pPIiOl":"{subscriberCount} Subscribers","rL8HYz":"Professional Gamer","rLGZZX":"Just now","rNVPnk":"It's an inappropriate Snap of me","rrdPgT":"Store","rsYMnU":"Episodes","sRM8i5":"Why do you want to report this Snap?","sVcU8q":"Posted to Snap Map","tYFb/P":"Spotlight","vTd+a8":"I'm being bullied or harassed","vqdER6":"Fitness Professional","wVfxbD":"Political Candidate","wpLx7z":"Lens Creator","x1C/5K":"Person","x4F6zb":"Report Snap","xLaO8v":"Health / Beauty","yT6a3h":"In this Snap","ys7Y26":"Athlete","zExXNB":"Sports Team"},"lenses":[],"curatedHighlights":[{"storyType":3,"storyTapId":"0","snapList":[{"snapIndex":0,"snapMediaType":0,"snapId":{"value":""},"snapUrls":{"mediaUrl":"https://cf-st.sc-cdn.net/d/Cg5MaQODMG3TnzwDo9KIa.400.IRZXSOY?uc=12","mediaPreviewUrl":{"value":"https://cf-st.sc-cdn.net/d/Cg5MaQODMG3TnzwDo9KIa.410.IRZXSOY?uc=12"}},"timestampInSec":{"value":"1606531630"}},{"snapIndex":1,"snapMediaType":0,"snapId":{"value":""},"snapUrls":{"mediaUrl":"https://cf-st.sc-cdn.net/d/uxOSCj5RgvtbPc1WJFZE4.400.IRZXSOY?uc=12","mediaPreviewUrl":{"value":"https://cf-st.sc-cdn.net/d/uxOSCj5RgvtbPc1WJFZE4.410.IRZXSOY?uc=12"}},"timestampInSec":{"value":"1605705190"}}],"storyId":{"value":""},"storyTitle":{"value":""},"thumbnailUrl":{"value":"https://cf-st.sc-cdn.net/d/Cg5MaQODMG3TnzwDo9KIa.410.IRZXSOY?uc=12"}}],"spotlightHighlights":[],"spotlightHighlightsMetadata":[],"viewerInfo":{"country":"IN","locale":"en_US"},"localization":{"direction":0},"pageLinks":{"oneLinkUrl":"https://click.snapchat.com/aVHG?pid=snapchat_download_page\u0026af_dp=https://www.snapchat.com/add/invalidusername?sc_referrer%3Dweb\u0026af_web_dp=https://snapchat.com/download?purpose%3Dweb_stories","snapchatCanonicalUrl":"https://www.snapchat.com/add/invalidusername","canonicalUrl":"https://www.snapchat.com/add/invalidusername","snapcodeImageUrl":"https://app.snapchat.com/web/deeplink/snapcode?username=invalidusername\u0026type=SVG\u0026bitmoji=enable"},"pageMetadata":{"pageType":9,"pageTitle":"Mrunu (@invalidusername) on Snapchat","pageDescription":{"value":"Mrunu is on Snapchat!"}},"userProfile":{"$case":"publicProfileInfo","publicProfileInfo":{"username":"invalidusername","title":"Mrunu","snapcodeImageUrl":"https://app.snapchat.com/web/deeplink/snapcode?username=invalidusername\u0026type=SVG\u0026bitmoji=enable","badge":1,"categoryStringId":"public-profile-category-v3-people","subcategoryStringId":"public-profile-subcategory-v3-artist","subscriberCount":"874600","bio":"Welcome to my weird life ✨","websiteUrl":"https://youtube.com/c/GujjuUnicorn","profilePictureUrl":"https://cf-st.sc-cdn.net/aps/bolt/aHR0cHM6Ly9jZi1zdC5zYy1jZG4ubmV0L2QvdTVBZEFXVnV1RlVSNDNBQk5qRHVNP2JvPUVnMGFBQm9BTWdFRVNBSlFHV0FCJnVjPTI1._RS0,90_FMjpeg","address":"Mumbai, India, India","hasCuratedHighlights":true,"hasSpotlightHighlights":false,"mutableName":"","publisherType":"","squareHeroImageUrl":"","primaryColor":""}},"story":{"storyType":5,"storyTapId":"0","snapList":[{"snapIndex":0,"snapMediaType":1,"snapId":{"value":"1PgHW1XZSgWteDhyTiIFbgAAgcnlmYnB0ZWpiAXxms2FCAXxms17GAAAAAA"},"snapUrls":{"mediaUrl":"https://filesamples.com/samples/video/mp4/sample_640x360.mp4","mediaPreviewUrl":{"value":"https://s.sc-cdn.net/1d/5Wv7rx8leVHNTyY454OlnCjZDCNqDQoW7y7eUU1T1CY=/default/preview_overlay.jpg"}},"timestampInSec":{"value":"1633810603"}},{"snapIndex":1,"snapMediaType":0,"snapId":{"value":"1PgHW1XZSgWteDhyTiIFbgAAgZWZqZ2t2ZGN4AXxpJwZoAXxpJwRfAAAAAA"},"snapUrls":{"mediaUrl":"https://filesamples.com/samples/video/mp4/sample_640x360.mp4"},"timestampInSec":{"value":"1633851737"}},{"snapIndex":2,"snapMediaType":0,"snapId":{"value":"1PgHW1XZSgWteDhyTiIFbgAAgdGlyeXpodGx4AXxpR4jsAXxpR4XzAAAAAA"},"snapUrls":{"mediaUrl":"https://filesamples.com/samples/video/mp4/sample_640x360.mp4"},"timestampInSec":{"value":"1633853867"}},{"snapIndex":3,"snapMediaType":0,"snapId":{"value":"1PgHW1XZSgWteDhyTiIFbgAAgdnJlc2hjeWd5AXxqhQjjAXxqhQaeAAAAAA"},"snapUrls":{"mediaUrl":"https://filesamples.com/samples/video/mp4/sample_640x360.mp4"},"timestampInSec":{"value":"1633874675"}}],"storyId":{"value":"invalidusername"},"thumbnailUrl":{"value":"https://s.sc-cdn.net/1d/5Wv7rx8leVHNTyY454OlnCjZDCNqDQoW7y7eUU1T1CY=/default/preview_overlay.jpg"}},"linkPreview":{"title":"invalidusername on Snapchat","description":"","canonicalUrl":"https://story.snapchat.com/u/invalidusername","twitterImage":{"url":"https://story.snapchat.com/@invalidusername/preview/twitter.png","size":{"width":1200,"height":600}},"facebookImage":{"url":"https://story.snapchat.com/@invalidusername/preview/facebook.png","size":{"width":1200,"height":628}}}},"status":0,"log":{"levels":{"TRACE":0,"DEBUG":1,"INFO":2,"WARN":3,"ERROR":4,"SILENT":5}}},"page":"/@/[username]","query":{"username":"@invalidusername"},"buildId":"23576-9b597984705a8ea2bff65ac8abd3eb5a984c976a","assetPrefix":"https://story.snapchat.com","isFallback":false,"dynamicIds":["gkwE","+51n","AC5g","DbP8","KIpE","LQDX","NuZu","aLx/","qmXy","sZW5","sZkf"],"gip":true,"appGip":true}</script><script nomodule="" src="https://story.snapchat.com/_next/static/chunks/polyfills-553aafd328e99d1ecd5e.js"></script><script async="" src="https://story.snapchat.com/_next/static/chunks/049823d6.8b03ce304b0e44456f30.js"></script><script async="" src="https://story.snapchat.com/_next/static/chunks/22.ca59e6299b825dc862b0.js"></script><script src="https://story.snapchat.com/_next/static/chunks/webpack-edb54b561e62fb294b85.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/framework.efe182f2d62be1d8151a.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/c408797459d80c128d5e47906020fa02c3ea7a51.cdf474846c815ffe556c.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/f6078781a05fe1bcb0902d23dbbb2662c8d200b3.0cb66906a1ea3f804368.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/main-69ec1f1dba14cd9f620a.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/c1468a61a92675d836a3000bab1334fb54fd20a9.074f204d663a13469e0b.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/d241c1e27ffe07c251e6f8ab09888e7ecf8ae8dc.b20db949b32dafefad5c.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/d4fc9bc7fce3fa7dbb251df097e4d60e4f4a3ec9.6a57a5151732d06fa88a.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/pages/_app-9a2167e8d8d9d9f101c9.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/29107295.be25f8bc8bdde59f114d.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/641167d64809277a1b9199554823a0e631b3bff2.b1423abff274817ff848.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/96c0058ea2ce58b3f27756fc0d0be33ac3f6361c.4360e309b36814bc7496.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/64dd010a9368940fc41206bc54dfee6183397831.1358f9c5b56d2322e06e.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/bd9739576daf9a5525e7028695825e8d0c29e04c.65c9b0762abe3d67e2ce.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/f2142e6c893e00c2f1a27f144791418e507fc12c.1ef92cfd6920c8f93e61.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/e2ef7edf3a7e66ae27a9d163772f8c722ad47684.7e5591f9407dd7837830.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/61f94ab364ffeaf810caabbb5e8c59d41b273801.6e578c39745032b54013.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/d01c7d3028b0c7a5252ef883c5a43f5f0e747f01.5c6a4b590ccfff6d1784.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/pages/@/%5Busername%5D-19264ae3ee802be2dc6d.js" async=""></script><script src="https://story.snapchat.com/_next/static/23576-9b597984705a8ea2bff65ac8abd3eb5a984c976a/_buildManifest.js" async=""></script><script src="https://story.snapchat.com/_next/static/23576-9b597984705a8ea2bff65ac8abd3eb5a984c976a/_ssgManifest.js" async=""></script></body></html>
+
+<!DOCTYPE html><html prefix="og: https://ogp.me/ns#" dir="0" lang="en-US"><head><link data-react-helmet="true" rel="canonical" href="https://www.snapchat.com/add/invalidusername"/><meta data-react-helmet="true" name="description" content="Mrunu is on Snapchat!"/><meta data-react-helmet="true" name="apple-itunes-app" content="app-id=447188370, app-argument=https://www.snapchat.com/add/invalidusername"/><meta data-react-helmet="true" name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1.0, user-scalable=0"/><meta data-react-helmet="true" name="metrics-page-name" content="User_Profile.PublicProfile"/><meta data-react-helmet="true" property="og:title" content="invalidusername on Snapchat"/><meta data-react-helmet="true" property="og:type" content="video.other"/><meta data-react-helmet="true" property="og:url" content="https://story.snapchat.com/u/invalidusername"/><meta data-react-helmet="true" property="og:image" content="https://story.snapchat.com/@invalidusername/preview/facebook.png"/><meta data-react-helmet="true" property="og:locale:alternate" content="ar_AA"/><meta data-react-helmet="true" property="og:locale:alternate" content="da_DK"/><meta data-react-helmet="true" property="og:locale:alternate" content="de_DK"/><meta data-react-helmet="true" property="og:locale:alternate" content="en_GB"/><meta data-react-helmet="true" property="og:locale:alternate" content="en_US"/><meta data-react-helmet="true" property="og:locale:alternate" content="es_ES"/><meta data-react-helmet="true" property="og:locale:alternate" content="es_MX"/><meta data-react-helmet="true" property="og:locale:alternate" content="fi_FI"/><meta data-react-helmet="true" property="og:locale:alternate" content="fr_FR"/><meta data-react-helmet="true" property="og:locale:alternate" content="it_IT"/><meta data-react-helmet="true" property="og:locale:alternate" content="ja_JP"/><meta data-react-helmet="true" property="og:locale:alternate" content="nb_NO"/><meta data-react-helmet="true" property="og:locale:alternate" content="nl_NL"/><meta data-react-helmet="true" property="og:locale:alternate" content="pt_BR"/><meta data-react-helmet="true" property="og:locale:alternate" content="sv_SE"/><meta data-react-helmet="true" property="og:image:width" content="1200"/><meta data-react-helmet="true" property="og:image:height" content="628"/><meta data-react-helmet="true" property="og:site_name" content="Snapchat"/><meta data-react-helmet="true" property="fb:app_id" content="394343577431007"/><meta data-react-helmet="true" property="fb:admins" content="1349731971"/><meta data-react-helmet="true" property="twitter:card" content="summary_large_image"/><meta data-react-helmet="true" property="twitter:site" content="@Snapchat"/><meta data-react-helmet="true" property="twitter:title" content="invalidusername on Snapchat"/><meta data-react-helmet="true" property="twitter:image" content="https://story.snapchat.com/@invalidusername/preview/twitter.png"/><script data-react-helmet="true" async="" src="https://www.google-analytics.com/analytics.js"></script><script data-react-helmet="true">
+    window.ga=window.ga||function(){(ga.q = ga.q || []).push(arguments)};
+    ga.l=+new Date;
+    ga('create','UA-41740027-40', 'auto');
+    ga('send','pageview', location.pathname);
+  </script><style data-react-helmet="true">html {
+          height: 100%;
+          box-sizing: border-box;
+         }
+
+         body {
+          margin: 0;
+          height: 100%;
+          background: #121314;
+          font-family: Avenir Next, Helvetica, sans-serif;
+          -webkit-text-fill-color: currentcolor;
+         }
+
+         #__next, #root {
+          height: 100%;
+         }
+
+         *, *:before, *:after {
+          box-sizing: inherit;
+         }
+
+         button {
+          -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
+          -webkit-tap-highlight-color: transparent;
+          -webkit-user-select: none;
+          -khtml-user-select: none;
+          -moz-user-select: none;
+          -ms-user-select: none;
+          user-select: none;
+         }
+         </style><title data-react-helmet="true">Mrunu (@invalidusername) on Snapchat</title><meta charSet="utf-8"/><meta name="viewport" content="width=device-width"/><meta name="next-head-count" content="2"/><noscript data-n-css=""></noscript><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/049823d6.8b03ce304b0e44456f30.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/22.ca59e6299b825dc862b0.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/webpack-edb54b561e62fb294b85.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/framework.efe182f2d62be1d8151a.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/c408797459d80c128d5e47906020fa02c3ea7a51.cdf474846c815ffe556c.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/f6078781a05fe1bcb0902d23dbbb2662c8d200b3.0cb66906a1ea3f804368.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/main-69ec1f1dba14cd9f620a.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/c1468a61a92675d836a3000bab1334fb54fd20a9.074f204d663a13469e0b.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/d241c1e27ffe07c251e6f8ab09888e7ecf8ae8dc.b20db949b32dafefad5c.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/d4fc9bc7fce3fa7dbb251df097e4d60e4f4a3ec9.6a57a5151732d06fa88a.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/pages/_app-9a2167e8d8d9d9f101c9.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/29107295.be25f8bc8bdde59f114d.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/641167d64809277a1b9199554823a0e631b3bff2.b1423abff274817ff848.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/96c0058ea2ce58b3f27756fc0d0be33ac3f6361c.4360e309b36814bc7496.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/64dd010a9368940fc41206bc54dfee6183397831.1358f9c5b56d2322e06e.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/bd9739576daf9a5525e7028695825e8d0c29e04c.65c9b0762abe3d67e2ce.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/f2142e6c893e00c2f1a27f144791418e507fc12c.1ef92cfd6920c8f93e61.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/e2ef7edf3a7e66ae27a9d163772f8c722ad47684.7e5591f9407dd7837830.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/61f94ab364ffeaf810caabbb5e8c59d41b273801.6e578c39745032b54013.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/d01c7d3028b0c7a5252ef883c5a43f5f0e747f01.5c6a4b590ccfff6d1784.js" as="script"/><link rel="preload" href="https://story.snapchat.com/_next/static/chunks/pages/@/%5Busername%5D-19264ae3ee802be2dc6d.js" as="script"/></head><body id="root"><div id="__next"><style data-emotion="css-global cqw65k">@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.ttf") format("truetype");font-weight:100;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.ttf") format("truetype");font-weight:100;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLight.ttf") format("truetype");font-weight:200;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-UltraLightItalic.ttf") format("truetype");font-weight:200;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Regular.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Regular.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Regular.ttf") format("truetype");font-weight:300;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Italic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Italic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Italic.ttf") format("truetype");font-weight:300;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Medium.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Medium.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Medium.ttf") format("truetype");font-weight:400;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-MediumItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-MediumItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-MediumItalic.ttf") format("truetype");font-weight:400;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-DemiBold.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-DemiBold.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-DemiBold.ttf") format("truetype");font-weight:500;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-DemiBoldItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-DemiBoldItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-DemiBoldItalic.ttf") format("truetype");font-weight:500;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Bold.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Bold.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Bold.ttf") format("truetype");font-weight:600;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.ttf") format("truetype");font-weight:600;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Bold.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Bold.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Bold.ttf") format("truetype");font-weight:700;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-BoldItalic.ttf") format("truetype");font-weight:700;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Heavy.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Heavy.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Heavy.ttf") format("truetype");font-weight:800;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.ttf") format("truetype");font-weight:800;font-style:italic;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-Heavy.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-Heavy.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-Heavy.ttf") format("truetype");font-weight:900;font-style:normal;font-display:block;}@font-face{font-family:"Avenir Next";src:url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.woff2") format("woff2"),url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.woff") format("woff"),url("https://story.snapchat.com/fonts/AvenirNext-HeavyItalic.ttf") format("truetype");font-weight:900;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Thin.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Thin.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Thin.ttf") format("truetype");font-weight:100;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ThinItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ThinItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ThinItalic.ttf") format("truetype");font-weight:100;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Extralight.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Extralight.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Extralight.ttf") format("truetype");font-weight:200;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ExtralightItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ExtralightItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-ExtralightItalic.ttf") format("truetype");font-weight:200;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Light.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Light.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Light.ttf") format("truetype");font-weight:300;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-LightItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-LightItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-LightItalic.ttf") format("truetype");font-weight:300;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Regular.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Regular.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Regular.ttf") format("truetype");font-weight:400;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-RegularItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-RegularItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-RegularItalic.ttf") format("truetype");font-weight:400;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Medium.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Medium.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Medium.ttf") format("truetype");font-weight:500;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-MediumItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-MediumItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-MediumItalic.ttf") format("truetype");font-weight:500;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Semibold.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Semibold.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Semibold.ttf") format("truetype");font-weight:600;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SemiboldItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SemiboldItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SemiboldItalic.ttf") format("truetype");font-weight:600;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Bold.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Bold.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Bold.ttf") format("truetype");font-weight:700;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BoldItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BoldItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BoldItalic.ttf") format("truetype");font-weight:700;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Black.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Black.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Black.ttf") format("truetype");font-weight:800;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BlackItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BlackItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-BlackItalic.ttf") format("truetype");font-weight:800;font-style:italic;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Super.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Super.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-Super.ttf") format("truetype");font-weight:900;font-style:normal;font-display:block;}@font-face{font-family:"Graphik";src:url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SuperItalic.woff2") format("woff2"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SuperItalic.woff") format("woff"),url("https://snap-design-system.storage.googleapis.com/fonts/graphik/Graphik-SuperItalic.ttf") format("truetype");font-weight:900;font-style:italic;font-display:block;}</style></div><script id="__NEXT_DATA__" type="application/json">{"props":{"pageProps":{"googleAnalyticsPropertyId":"UA-41740027-40","localizedMessages":{"default":{"+9d+q7":"Nonprofit Organization","+ByJA/":"Stories","+hwkQQ":"Film / TV","+lhElX":"Copyright infringement","+o8gM9":"Kit","/Xkr+t":"by {creatorDisplayName}","/dF4HW":"Spotlight","/tNMyW":"Download","/vdS3s":"Download Snapchat to Watch Now","04qzmG":"You will now be taken to the next Snap - press 'Close' to do this right away or we will continue automatically in 10 seconds.","0FP975":"Post to Spotlight","0Y6c0W":"Restaurant Chain","0YKDxr":"Photographer","0dJz6S":"Threatening, violent, or concerning","0uHjye":"Share this Snap","1PzCdm":"It asks for or threatens to post inappropriate Snaps","1V8Uma":"Public Figure","1egAGi":"Movie Character","1kdcl2":"Media / News Company","2LLiYb":"Close","2V40yT":"More Options","2l730k":"Film / TV Personality","4V5k0y":"Support","5HsSrO":"I just don't like it","5XW8Zd":"{subscriberCount} Subscribers","5m3Hu8":"I'm worried this Snapchatter might hurt themselves","5v6wP7":"Motivational Speaker","5zZGnG":"Writer","6yvoZD":"Sorry,","7BHw3h":"Religious Organization","7HP0Jf":"Coach","7XZM2L":"Business","7rVnIj":"Spotlight","7xehRy":"Producer","7yuYaU":"Businesses \u0026 Groups","8Sw4jY":"Report Snap","9NRv3Z":"Snapcodes","ATeDiR":"Thank you for reporting this Snap.","AbkQPs":"It's an invasion of privacy","AtLF/u":"This content was not found","CAgCZ5":"Nudity or sexual content","CJBFGo":"Politician","CVucIf":"Community Organization","DY4yHA":"Brand","EPBE+l":"Government Official","ESomE8":"Submit","Eqnt63":"{timeDifference}m ago","FDOu63":"Someone else is being bullied or harassed","Fsg136":"Episode {episodeNumber}","Ftta6c":"It's threatening a person or place","G7hRik":"Spotlight is not available in your location","GJZs5E":"It's spam","GVLbZP":"Stories","GaNuM2":"Best of Spotlight","Gh1a/j":"Food Professional","GssbOn":"Product","Gvuqme":"It's an inappropriate Snap of someone else","HLxWNM":"It sells or promotes inappropriate Snaps","HVgZaB":"Creator","HkaOsh":"Open your Snapchat","I1rLjL":"Ads","I6sovq":"Political Organization","IWKERN":"Fashion Model","JbCR5V":"This content is not available","Ju77ns":"Comedian","MDthgV":"Sports League","MN6Znh":"Watch more in Snapchat","MUzWB7":"Please provide your Snapchat username if you have one, and the email associated with your account","N7Wq/c":"Violent or disturbing","N7iI/k":"Download Snapchat to find more","NXPVkv":"Company / Enterprise","P6YGQz":"Open in Snapchat","PQcLi/":"Service","PyzdXL":"Cancel","Q4RuCH":"Maps","Q71IbU":"Government Organization","QdGWFE":"Season {seasonNumber}","RJo0Z3":"Harassment or Hate speech","RmE5lP":"Lifestyle Influencer","RtNy71":"Musician / Band","SCe4GQ":"Film Director","SVOJKh":"Video Game","SgFTtk":"Up next","TNK/W/":"Lenses","Tm6yFt":"Download Snapchat","UIZTzu":"It's attempting to buy or sell drugs or weapons","Uk55sM":"Add me on Snapchat!","VRmDFV":"Snap Reported","VZQx67":"This Snap is no longer available","VjDaWB":"Watch more from {publisherTitle}","W07I8V":"Share {username}'s Snap","WGtpBM":"People","WyUwHm":"They are pretending to be me","XbXoMR":"Actor","YhMtYd":"Spectacles","Yt2+ye":"My Story","ZPrHrl":"Internet Company","ZViZgq":"Traveler","ZlJO0Q":"Apparel / Fashion","ZvzVyN":"Top Lenses","aSXQy0":"Sports Personality","ah6l3c":"Charity / Cause","ais8eK":"Group","by2dgE":"News Personality","dAksd9":"Journalist","dItw6q":"Dancer","dJDu/3":"Entrepreneur","dkWyPr":"Vlogger / Blogger","fPIy5v":"Retail Company","fxAji7":"Filters \u0026 Lenses","hPxDQC":"Video Game Creator","jWa4OT":"College / University","jqpH+5":"Is there any more information you want to share about this Snap?","kNCf90":"Products \u0026 Brands","kzoiEX":"{timeDifference}h ago","l1fnUG":"Scientist","lbui+i":"It's hate speech targeting me or another group","nbiOpp":"Lens Studio","ojrZ4G":"Download","pCK8FJ":"Artist","pPIiOl":"{subscriberCount} Subscribers","rL8HYz":"Professional Gamer","rLGZZX":"Just now","rNVPnk":"It's an inappropriate Snap of me","rrdPgT":"Store","rsYMnU":"Episodes","sRM8i5":"Why do you want to report this Snap?","sVcU8q":"Posted to Snap Map","tYFb/P":"Spotlight","vTd+a8":"I'm being bullied or harassed","vqdER6":"Fitness Professional","wVfxbD":"Political Candidate","wpLx7z":"Lens Creator","x1C/5K":"Person","x4F6zb":"Report Snap","xLaO8v":"Health / Beauty","yT6a3h":"In this Snap","ys7Y26":"Athlete","zExXNB":"Sports Team"},"+9d+q7":"Nonprofit Organization","+ByJA/":"Stories","+hwkQQ":"Film / TV","+lhElX":"Copyright infringement","+o8gM9":"Kit","/Xkr+t":"by {creatorDisplayName}","/dF4HW":"Spotlight","/tNMyW":"Download","/vdS3s":"Download Snapchat to Watch Now","04qzmG":"You will now be taken to the next Snap - press 'Close' to do this right away or we will continue automatically in 10 seconds.","0FP975":"Post to Spotlight","0Y6c0W":"Restaurant Chain","0YKDxr":"Photographer","0dJz6S":"Threatening, violent, or concerning","0uHjye":"Share this Snap","1PzCdm":"It asks for or threatens to post inappropriate Snaps","1V8Uma":"Public Figure","1egAGi":"Movie Character","1kdcl2":"Media / News Company","2LLiYb":"Close","2V40yT":"More Options","2l730k":"Film / TV Personality","4V5k0y":"Support","5HsSrO":"I just don't like it","5XW8Zd":"{subscriberCount} Subscribers","5m3Hu8":"I'm worried this Snapchatter might hurt themselves","5v6wP7":"Motivational Speaker","5zZGnG":"Writer","6yvoZD":"Sorry,","7BHw3h":"Religious Organization","7HP0Jf":"Coach","7XZM2L":"Business","7rVnIj":"Spotlight","7xehRy":"Producer","7yuYaU":"Businesses \u0026 Groups","8Sw4jY":"Report Snap","9NRv3Z":"Snapcodes","ATeDiR":"Thank you for reporting this Snap.","AbkQPs":"It's an invasion of privacy","AtLF/u":"This content was not found","CAgCZ5":"Nudity or sexual content","CJBFGo":"Politician","CVucIf":"Community Organization","DY4yHA":"Brand","EPBE+l":"Government Official","ESomE8":"Submit","Eqnt63":"{timeDifference}m ago","FDOu63":"Someone else is being bullied or harassed","Fsg136":"Episode {episodeNumber}","Ftta6c":"It's threatening a person or place","G7hRik":"Spotlight is not available in your location","GJZs5E":"It's spam","GVLbZP":"Stories","GaNuM2":"Best of Spotlight","Gh1a/j":"Food Professional","GssbOn":"Product","Gvuqme":"It's an inappropriate Snap of someone else","HLxWNM":"It sells or promotes inappropriate Snaps","HVgZaB":"Creator","HkaOsh":"Open your Snapchat","I1rLjL":"Ads","I6sovq":"Political Organization","IWKERN":"Fashion Model","JbCR5V":"This content is not available","Ju77ns":"Comedian","MDthgV":"Sports League","MN6Znh":"Watch more in Snapchat","MUzWB7":"Please provide your Snapchat username if you have one, and the email associated with your account","N7Wq/c":"Violent or disturbing","N7iI/k":"Download Snapchat to find more","NXPVkv":"Company / Enterprise","P6YGQz":"Open in Snapchat","PQcLi/":"Service","PyzdXL":"Cancel","Q4RuCH":"Maps","Q71IbU":"Government Organization","QdGWFE":"Season {seasonNumber}","RJo0Z3":"Harassment or Hate speech","RmE5lP":"Lifestyle Influencer","RtNy71":"Musician / Band","SCe4GQ":"Film Director","SVOJKh":"Video Game","SgFTtk":"Up next","TNK/W/":"Lenses","Tm6yFt":"Download Snapchat","UIZTzu":"It's attempting to buy or sell drugs or weapons","Uk55sM":"Add me on Snapchat!","VRmDFV":"Snap Reported","VZQx67":"This Snap is no longer available","VjDaWB":"Watch more from {publisherTitle}","W07I8V":"Share {username}'s Snap","WGtpBM":"People","WyUwHm":"They are pretending to be me","XbXoMR":"Actor","YhMtYd":"Spectacles","Yt2+ye":"My Story","ZPrHrl":"Internet Company","ZViZgq":"Traveler","ZlJO0Q":"Apparel / Fashion","ZvzVyN":"Top Lenses","aSXQy0":"Sports Personality","ah6l3c":"Charity / Cause","ais8eK":"Group","by2dgE":"News Personality","dAksd9":"Journalist","dItw6q":"Dancer","dJDu/3":"Entrepreneur","dkWyPr":"Vlogger / Blogger","fPIy5v":"Retail Company","fxAji7":"Filters \u0026 Lenses","hPxDQC":"Video Game Creator","jWa4OT":"College / University","jqpH+5":"Is there any more information you want to share about this Snap?","kNCf90":"Products \u0026 Brands","kzoiEX":"{timeDifference}h ago","l1fnUG":"Scientist","lbui+i":"It's hate speech targeting me or another group","nbiOpp":"Lens Studio","ojrZ4G":"Download","pCK8FJ":"Artist","pPIiOl":"{subscriberCount} Subscribers","rL8HYz":"Professional Gamer","rLGZZX":"Just now","rNVPnk":"It's an inappropriate Snap of me","rrdPgT":"Store","rsYMnU":"Episodes","sRM8i5":"Why do you want to report this Snap?","sVcU8q":"Posted to Snap Map","tYFb/P":"Spotlight","vTd+a8":"I'm being bullied or harassed","vqdER6":"Fitness Professional","wVfxbD":"Political Candidate","wpLx7z":"Lens Creator","x1C/5K":"Person","x4F6zb":"Report Snap","xLaO8v":"Health / Beauty","yT6a3h":"In this Snap","ys7Y26":"Athlete","zExXNB":"Sports Team"},"lenses":[],"curatedHighlights":[{"storyType":3,"storyTapId":"0","snapList":[{"snapIndex":0,"snapMediaType":0,"snapId":{"value":""},"snapUrls":{"mediaUrl":"https://cf-st.sc-cdn.net/d/Cg5MaQODMG3TnzwDo9KIa.400.IRZXSOY?uc=12","mediaPreviewUrl":{"value":"https://cf-st.sc-cdn.net/d/Cg5MaQODMG3TnzwDo9KIa.410.IRZXSOY?uc=12"}},"timestampInSec":{"value":"1606531630"}},{"snapIndex":1,"snapMediaType":0,"snapId":{"value":""},"snapUrls":{"mediaUrl":"https://cf-st.sc-cdn.net/d/uxOSCj5RgvtbPc1WJFZE4.400.IRZXSOY?uc=12","mediaPreviewUrl":{"value":"https://cf-st.sc-cdn.net/d/uxOSCj5RgvtbPc1WJFZE4.410.IRZXSOY?uc=12"}},"timestampInSec":{"value":"1605705190"}}],"storyId":{"value":""},"storyTitle":{"value":""},"thumbnailUrl":{"value":"https://cf-st.sc-cdn.net/d/Cg5MaQODMG3TnzwDo9KIa.410.IRZXSOY?uc=12"}}],"spotlightHighlights":[],"spotlightHighlightsMetadata":[],"viewerInfo":{"country":"IN","locale":"en_US"},"localization":{"direction":0},"pageLinks":{"oneLinkUrl":"https://click.snapchat.com/aVHG?pid=snapchat_download_page\u0026af_dp=https://www.snapchat.com/add/invalidusername?sc_referrer%3Dweb\u0026af_web_dp=https://snapchat.com/download?purpose%3Dweb_stories","snapchatCanonicalUrl":"https://www.snapchat.com/add/invalidusername","canonicalUrl":"https://www.snapchat.com/add/invalidusername","snapcodeImageUrl":"https://app.snapchat.com/web/deeplink/snapcode?username=invalidusername\u0026type=SVG\u0026bitmoji=enable"},"pageMetadata":{"pageType":9,"pageTitle":"Mrunu (@invalidusername) on Snapchat","pageDescription":{"value":"Mrunu is on Snapchat!"}},"userProfile":{"$case":"publicProfileInfo","publicProfileInfo":{"username":"invalidusername","title":"Mrunu","snapcodeImageUrl":"https://app.snapchat.com/web/deeplink/snapcode?username=invalidusername\u0026type=SVG\u0026bitmoji=enable","badge":1,"categoryStringId":"public-profile-category-v3-people","subcategoryStringId":"public-profile-subcategory-v3-artist","subscriberCount":"874600","bio":"Welcome to my weird life ✨","websiteUrl":"https://youtube.com/c/GujjuUnicorn","profilePictureUrl":"https://cf-st.sc-cdn.net/aps/bolt/aHR0cHM6Ly9jZi1zdC5zYy1jZG4ubmV0L2QvdTVBZEFXVnV1RlVSNDNBQk5qRHVNP2JvPUVnMGFBQm9BTWdFRVNBSlFHV0FCJnVjPTI1._RS0,90_FMjpeg","address":"Mumbai, India, India","hasCuratedHighlights":true,"hasSpotlightHighlights":false,"mutableName":"","publisherType":"","squareHeroImageUrl":"","primaryColor":""}},"story":{"storyType":5,"storyTapId":"0","snapList":[{"snapIndex":0,"snapMediaType":1,"snapId":{"value":"1PgHW1XZSgWteDhyTiIFbgAAgcnlmYnB0ZWpiAXxms2FCAXxms17GAAAAAA"},"snapUrls":{"mediaUrl":"https://filesamples.com/samples/video/mp4/sample_640x360.mp4","mediaPreviewUrl":{"value":"https://s.sc-cdn.net/1d/5Wv7rx8leVHNTyY454OlnCjZDCNqDQoW7y7eUU1T1CY=/default/preview_overlay.jpg"}},"timestampInSec":{"value":"1633810603"}},{"snapIndex":1,"snapMediaType":0,"snapId":{"value":"1PgHW1XZSgWteDhyTiIFbgAAgZWZqZ2t2ZGN4AXxpJwZoAXxpJwRfAAAAAA"},"snapUrls":{"mediaUrl":"https://filesamples.com/samples/video/mp4/sample_640x360.mp4"},"timestampInSec":{"value":"1633851737"}},{"snapIndex":2,"snapMediaType":0,"snapId":{"value":"1PgHW1XZSgWteDhyTiIFbgAAgdGlyeXpodGx4AXxpR4jsAXxpR4XzAAAAAA"},"snapUrls":{"mediaUrl":"https://filesamples.com/samples/video/mp4/sample_640x360.mp4"},"timestampInSec":{"value":"1633853867"}},{"snapIndex":3,"snapMediaType":0,"snapId":{"value":"1PgHW1XZSgWteDhyTiIFbgAAgdnJlc2hjeWd5AXxqhQjjAXxqhQaeAAAAAA"},"snapUrls":{"mediaUrl":"https://filesamples.com/samples/video/mp4/sample_640x360.mp4"},"timestampInSec":{"value":"1633874675"}}],"storyId":{"value":"invalidusername"},"thumbnailUrl":{"value":"https://s.sc-cdn.net/1d/5Wv7rx8leVHNTyY454OlnCjZDCNqDQoW7y7eUU1T1CY=/default/preview_overlay.jpg"}},"linkPreview":{"title":"invalidusername on Snapchat","description":"","canonicalUrl":"https://story.snapchat.com/u/invalidusername","twitterImage":{"url":"https://story.snapchat.com/@invalidusername/preview/twitter.png","size":{"width":1200,"height":600}},"facebookImage":{"url":"https://story.snapchat.com/@invalidusername/preview/facebook.png","size":{"width":1200,"height":628}}}},"status":0,"log":{"levels":{"TRACE":0,"DEBUG":1,"INFO":2,"WARN":3,"ERROR":4,"SILENT":5}}},"page":"/@/[username]","query":{"username":"@invalidusername"},"buildId":"23576-9b597984705a8ea2bff65ac8abd3eb5a984c976a","assetPrefix":"https://story.snapchat.com","isFallback":false,"dynamicIds":["gkwE","+51n","AC5g","DbP8","KIpE","LQDX","NuZu","aLx/","qmXy","sZW5","sZkf"],"gip":true,"appGip":true}</script><script nomodule="" src="https://story.snapchat.com/_next/static/chunks/polyfills-553aafd328e99d1ecd5e.js"></script><script async="" src="https://story.snapchat.com/_next/static/chunks/049823d6.8b03ce304b0e44456f30.js"></script><script async="" src="https://story.snapchat.com/_next/static/chunks/22.ca59e6299b825dc862b0.js"></script><script src="https://story.snapchat.com/_next/static/chunks/webpack-edb54b561e62fb294b85.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/framework.efe182f2d62be1d8151a.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/c408797459d80c128d5e47906020fa02c3ea7a51.cdf474846c815ffe556c.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/f6078781a05fe1bcb0902d23dbbb2662c8d200b3.0cb66906a1ea3f804368.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/main-69ec1f1dba14cd9f620a.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/c1468a61a92675d836a3000bab1334fb54fd20a9.074f204d663a13469e0b.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/d241c1e27ffe07c251e6f8ab09888e7ecf8ae8dc.b20db949b32dafefad5c.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/d4fc9bc7fce3fa7dbb251df097e4d60e4f4a3ec9.6a57a5151732d06fa88a.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/pages/_app-9a2167e8d8d9d9f101c9.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/29107295.be25f8bc8bdde59f114d.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/641167d64809277a1b9199554823a0e631b3bff2.b1423abff274817ff848.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/96c0058ea2ce58b3f27756fc0d0be33ac3f6361c.4360e309b36814bc7496.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/64dd010a9368940fc41206bc54dfee6183397831.1358f9c5b56d2322e06e.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/bd9739576daf9a5525e7028695825e8d0c29e04c.65c9b0762abe3d67e2ce.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/f2142e6c893e00c2f1a27f144791418e507fc12c.1ef92cfd6920c8f93e61.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/e2ef7edf3a7e66ae27a9d163772f8c722ad47684.7e5591f9407dd7837830.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/61f94ab364ffeaf810caabbb5e8c59d41b273801.6e578c39745032b54013.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/d01c7d3028b0c7a5252ef883c5a43f5f0e747f01.5c6a4b590ccfff6d1784.js" async=""></script><script src="https://story.snapchat.com/_next/static/chunks/pages/@/%5Busername%5D-19264ae3ee802be2dc6d.js" async=""></script><script src="https://story.snapchat.com/_next/static/23576-9b597984705a8ea2bff65ac8abd3eb5a984c976a/_buildManifest.js" async=""></script><script src="https://story.snapchat.com/_next/static/23576-9b597984705a8ea2bff65ac8abd3eb5a984c976a/_ssgManifest.js" async=""></script></body></html>
```

### Comparing `snapchat-dlp-1.5.2/tests/mock_data/invalidusername.json` & `snapchat-dlp-1.5.8/tests/mock_data/invalidusername.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 21% similar despite different names*

```diff
@@ -1,137 +1,134 @@
-00000000: 7b0d 0a20 2020 2022 7374 6f72 7922 3a20  {..    "story": 
-00000010: 7b0d 0a20 2020 2020 2020 2022 6964 223a  {..        "id":
-00000020: 2022 696e 7661 6c69 6475 7365 726e 616d   "invalidusernam
-00000030: 6522 2c0d 0a20 2020 2020 2020 2022 6d65  e",..        "me
-00000040: 7461 6461 7461 223a 207b 0d0a 2020 2020  tadata": {..    
-00000050: 2020 2020 2020 2020 2273 746f 7279 5479          "storyTy
-00000060: 7065 223a 2022 5459 5045 5f50 5542 4c49  pe": "TYPE_PUBLI
-00000070: 435f 5553 4552 5f53 544f 5259 222c 0d0a  C_USER_STORY",..
-00000080: 2020 2020 2020 2020 2020 2020 2274 6974              "tit
-00000090: 6c65 223a 2022 696e 7661 6c69 6475 7365  le": "invaliduse
-000000a0: 726e 616d 6522 2c0d 0a20 2020 2020 2020  rname",..       
-000000b0: 2020 2020 2022 656d 6f6a 6922 3a20 22e2       "emoji": ".
-000000c0: ad90 222c 0d0a 2020 2020 2020 2020 2020  ..",..          
-000000d0: 2020 2263 616e 6f6e 6963 616c 5572 6c53    "canonicalUrlS
-000000e0: 7566 6669 7822 3a20 2273 746f 7279 2f69  uffix": "story/i
-000000f0: 6e76 616c 6964 7573 6572 6e61 6d65 2f69  nvalidusername/i
-00000100: 6e76 616c 6964 7573 6572 6e61 6d65 220d  nvalidusername".
-00000110: 0a20 2020 2020 2020 207d 2c0d 0a20 2020  .        },..   
-00000120: 2020 2020 2022 736e 6170 7322 3a20 5b0d       "snaps": [.
-00000130: 0a20 2020 2020 2020 2020 2020 207b 0d0a  .            {..
-00000140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000150: 2269 6422 3a20 2231 5067 4857 3158 5a53  "id": "1PgHW1XZS
-00000160: 6757 7465 4468 7954 6949 4662 6741 4167  gWteDhyTiIFbgAAg
-00000170: 636e 6c6d 596e 4230 5a57 7069 4158 786d  cnlmYnB0ZWpiAXxm
-00000180: 7332 4643 4158 786d 7331 3747 4141 4141  s2FCAXxms17GAAAA
-00000190: 4141 222c 0d0a 2020 2020 2020 2020 2020  AA",..          
-000001a0: 2020 2020 2020 226d 6564 6961 223a 207b        "media": {
-000001b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000001c0: 2020 2020 2020 2274 7970 6522 3a20 2256        "type": "V
-000001d0: 4944 454f 222c 0d0a 2020 2020 2020 2020  IDEO",..        
-000001e0: 2020 2020 2020 2020 2020 2020 226d 6564              "med
-000001f0: 6961 5572 6c22 3a20 2268 7474 7073 3a2f  iaUrl": "https:/
-00000200: 2f66 696c 6573 616d 706c 6573 2e63 6f6d  /filesamples.com
-00000210: 2f73 616d 706c 6573 2f76 6964 656f 2f6d  /samples/video/m
-00000220: 7034 2f73 616d 706c 655f 3634 3078 3336  p4/sample_640x36
-00000230: 302e 6d70 3422 2c0d 0a20 2020 2020 2020  0.mp4",..       
-00000240: 2020 2020 2020 2020 2020 2020 2022 6d65               "me
-00000250: 6469 6153 7472 6561 6d69 6e67 5572 6c22  diaStreamingUrl"
-00000260: 3a20 2268 7474 7073 3a2f 2f66 696c 6573  : "https://files
-00000270: 616d 706c 6573 2e63 6f6d 2f73 616d 706c  amples.com/sampl
-00000280: 6573 2f76 6964 656f 2f6d 7034 2f73 616d  es/video/mp4/sam
-00000290: 706c 655f 3634 3078 3336 302e 6d70 3422  ple_640x360.mp4"
-000002a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000002b0: 2020 2020 2020 2022 6d65 6469 6150 7265         "mediaPre
-000002c0: 7669 6577 5572 6c22 3a20 2268 7474 7073  viewUrl": "https
-000002d0: 3a2f 2f66 696c 6573 616d 706c 6573 2e63  ://filesamples.c
-000002e0: 6f6d 2f73 616d 706c 6573 2f76 6964 656f  om/samples/video
-000002f0: 2f6d 7034 2f73 616d 706c 655f 3634 3078  /mp4/sample_640x
-00000300: 3336 302e 6d70 3422 0d0a 2020 2020 2020  360.mp4"..      
-00000310: 2020 2020 2020 2020 2020 7d2c 0d0a 2020            },..  
-00000320: 2020 2020 2020 2020 2020 2020 2020 226f                "o
-00000330: 7665 726c 6179 496d 6167 6522 3a20 7b0d  verlayImage": {.
-00000340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000350: 2020 2020 2022 6d65 6469 6155 726c 223a       "mediaUrl":
-00000360: 2022 6874 7470 733a 2f2f 6669 6c65 7361   "https://filesa
-00000370: 6d70 6c65 732e 636f 6d2f 7361 6d70 6c65  mples.com/sample
-00000380: 732f 7669 6465 6f2f 6d70 342f 7361 6d70  s/video/mp4/samp
-00000390: 6c65 5f36 3430 7833 3630 2e6d 7034 222c  le_640x360.mp4",
-000003a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000003b0: 2020 2020 2020 226d 6564 6961 5374 7265        "mediaStre
-000003c0: 616d 696e 6755 726c 223a 2022 6874 7470  amingUrl": "http
-000003d0: 733a 2f2f 6669 6c65 7361 6d70 6c65 732e  s://filesamples.
-000003e0: 636f 6d2f 7361 6d70 6c65 732f 7669 6465  com/samples/vide
-000003f0: 6f2f 6d70 342f 7361 6d70 6c65 5f36 3430  o/mp4/sample_640
-00000400: 7833 3630 2e6d 7034 220d 0a20 2020 2020  x360.mp4"..     
-00000410: 2020 2020 2020 2020 2020 207d 2c0d 0a20             },.. 
-00000420: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000430: 6361 7074 7572 6554 696d 6553 6563 7322  captureTimeSecs"
-00000440: 3a20 2231 3633 3338 3130 3630 3322 0d0a  : "1633810603"..
-00000450: 2020 2020 2020 2020 2020 2020 7d2c 0d0a              },..
-00000460: 2020 2020 2020 2020 2020 2020 7b0d 0a20              {.. 
-00000470: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000480: 6964 223a 2022 3150 6748 5731 585a 5367  id": "1PgHW1XZSg
-00000490: 5774 6544 6879 5469 4946 6267 4141 675a  WteDhyTiIFbgAAgZ
-000004a0: 575a 715a 3274 325a 474e 3441 5878 704a  WZqZ2t2ZGN4AXxpJ
-000004b0: 775a 6f41 5878 704a 7752 6641 4141 4141  wZoAXxpJwRfAAAAA
-000004c0: 4122 2c0d 0a20 2020 2020 2020 2020 2020  A",..           
-000004d0: 2020 2020 2022 6d65 6469 6122 3a20 7b0d       "media": {.
-000004e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000004f0: 2020 2020 2022 7479 7065 223a 2022 494d       "type": "IM
-00000500: 4147 4522 2c0d 0a20 2020 2020 2020 2020  AGE",..         
-00000510: 2020 2020 2020 2020 2020 2022 6d65 6469             "medi
-00000520: 6155 726c 223a 2022 6874 7470 733a 2f2f  aUrl": "https://
-00000530: 6669 6c65 7361 6d70 6c65 732e 636f 6d2f  filesamples.com/
-00000540: 7361 6d70 6c65 732f 7669 6465 6f2f 6d70  samples/video/mp
-00000550: 342f 7361 6d70 6c65 5f36 3430 7833 3630  4/sample_640x360
-00000560: 2e6d 7034 220d 0a20 2020 2020 2020 2020  .mp4"..         
-00000570: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
-00000580: 2020 2020 2020 2020 2020 2022 6361 7074             "capt
-00000590: 7572 6554 696d 6553 6563 7322 3a20 2231  ureTimeSecs": "1
-000005a0: 3633 3338 3531 3733 3722 0d0a 2020 2020  633851737"..    
-000005b0: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
-000005c0: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
-000005d0: 2020 2020 2020 2020 2020 2022 6964 223a             "id":
-000005e0: 2022 3150 6748 5731 585a 5367 5774 6544   "1PgHW1XZSgWteD
-000005f0: 6879 5469 4946 6267 4141 6764 476c 7965  hyTiIFbgAAgdGlye
-00000600: 5870 6f64 4778 3441 5878 7052 346a 7341  XpodGx4AXxpR4jsA
-00000610: 5878 7052 3458 7a41 4141 4141 4122 2c0d  XxpR4XzAAAAAA",.
-00000620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000630: 2022 6d65 6469 6122 3a20 7b0d 0a20 2020   "media": {..   
+00000000: 7b0a 2020 2020 2273 746f 7279 223a 207b  {.    "story": {
+00000010: 0a20 2020 2020 2020 2022 6964 223a 2022  .        "id": "
+00000020: 696e 7661 6c69 6475 7365 726e 616d 6522  invalidusername"
+00000030: 2c0a 2020 2020 2020 2020 226d 6574 6164  ,.        "metad
+00000040: 6174 6122 3a20 7b0a 2020 2020 2020 2020  ata": {.        
+00000050: 2020 2020 2273 746f 7279 5479 7065 223a      "storyType":
+00000060: 2022 5459 5045 5f50 5542 4c49 435f 5553   "TYPE_PUBLIC_US
+00000070: 4552 5f53 544f 5259 222c 0a20 2020 2020  ER_STORY",.     
+00000080: 2020 2020 2020 2022 7469 746c 6522 3a20         "title": 
+00000090: 2269 6e76 616c 6964 7573 6572 6e61 6d65  "invalidusername
+000000a0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+000000b0: 656d 6f6a 6922 3a20 22e2 ad90 222c 0a20  emoji": "...",. 
+000000c0: 2020 2020 2020 2020 2020 2022 6361 6e6f             "cano
+000000d0: 6e69 6361 6c55 726c 5375 6666 6978 223a  nicalUrlSuffix":
+000000e0: 2022 7374 6f72 792f 696e 7661 6c69 6475   "story/invalidu
+000000f0: 7365 726e 616d 652f 696e 7661 6c69 6475  sername/invalidu
+00000100: 7365 726e 616d 6522 0a20 2020 2020 2020  sername".       
+00000110: 207d 2c0a 2020 2020 2020 2020 2273 6e61   },.        "sna
+00000120: 7073 223a 205b 0a20 2020 2020 2020 2020  ps": [.         
+00000130: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+00000140: 2020 2020 2022 6964 223a 2022 3150 6748       "id": "1PgH
+00000150: 5731 585a 5367 5774 6544 6879 5469 4946  W1XZSgWteDhyTiIF
+00000160: 6267 4141 6763 6e6c 6d59 6e42 305a 5770  bgAAgcnlmYnB0ZWp
+00000170: 6941 5878 6d73 3246 4341 5878 6d73 3137  iAXxms2FCAXxms17
+00000180: 4741 4141 4141 4122 2c0a 2020 2020 2020  GAAAAAA",.      
+00000190: 2020 2020 2020 2020 2020 226d 6564 6961            "media
+000001a0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+000001b0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+000001c0: 2022 5649 4445 4f22 2c0a 2020 2020 2020   "VIDEO",.      
+000001d0: 2020 2020 2020 2020 2020 2020 2020 226d                "m
+000001e0: 6564 6961 5572 6c22 3a20 2268 7474 7073  ediaUrl": "https
+000001f0: 3a2f 2f66 696c 6573 616d 706c 6573 2e63  ://filesamples.c
+00000200: 6f6d 2f73 616d 706c 6573 2f76 6964 656f  om/samples/video
+00000210: 2f6d 7034 2f73 616d 706c 655f 3634 3078  /mp4/sample_640x
+00000220: 3336 302e 6d70 3422 2c0a 2020 2020 2020  360.mp4",.      
+00000230: 2020 2020 2020 2020 2020 2020 2020 226d                "m
+00000240: 6564 6961 5374 7265 616d 696e 6755 726c  ediaStreamingUrl
+00000250: 223a 2022 6874 7470 733a 2f2f 6669 6c65  ": "https://file
+00000260: 7361 6d70 6c65 732e 636f 6d2f 7361 6d70  samples.com/samp
+00000270: 6c65 732f 7669 6465 6f2f 6d70 342f 7361  les/video/mp4/sa
+00000280: 6d70 6c65 5f36 3430 7833 3630 2e6d 7034  mple_640x360.mp4
+00000290: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000002a0: 2020 2020 2020 2022 6d65 6469 6150 7265         "mediaPre
+000002b0: 7669 6577 5572 6c22 3a20 2268 7474 7073  viewUrl": "https
+000002c0: 3a2f 2f66 696c 6573 616d 706c 6573 2e63  ://filesamples.c
+000002d0: 6f6d 2f73 616d 706c 6573 2f76 6964 656f  om/samples/video
+000002e0: 2f6d 7034 2f73 616d 706c 655f 3634 3078  /mp4/sample_640x
+000002f0: 3336 302e 6d70 3422 0a20 2020 2020 2020  360.mp4".       
+00000300: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00000310: 2020 2020 2020 2020 2020 2020 226f 7665              "ove
+00000320: 726c 6179 496d 6167 6522 3a20 7b0a 2020  rlayImage": {.  
+00000330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000340: 2020 226d 6564 6961 5572 6c22 3a20 2268    "mediaUrl": "h
+00000350: 7474 7073 3a2f 2f66 696c 6573 616d 706c  ttps://filesampl
+00000360: 6573 2e63 6f6d 2f73 616d 706c 6573 2f76  es.com/samples/v
+00000370: 6964 656f 2f6d 7034 2f73 616d 706c 655f  ideo/mp4/sample_
+00000380: 3634 3078 3336 302e 6d70 3422 2c0a 2020  640x360.mp4",.  
+00000390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000003a0: 2020 226d 6564 6961 5374 7265 616d 696e    "mediaStreamin
+000003b0: 6755 726c 223a 2022 6874 7470 733a 2f2f  gUrl": "https://
+000003c0: 6669 6c65 7361 6d70 6c65 732e 636f 6d2f  filesamples.com/
+000003d0: 7361 6d70 6c65 732f 7669 6465 6f2f 6d70  samples/video/mp
+000003e0: 342f 7361 6d70 6c65 5f36 3430 7833 3630  4/sample_640x360
+000003f0: 2e6d 7034 220a 2020 2020 2020 2020 2020  .mp4".          
+00000400: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00000410: 2020 2020 2020 2020 2022 6361 7074 7572           "captur
+00000420: 6554 696d 6553 6563 7322 3a20 2231 3633  eTimeSecs": "163
+00000430: 3338 3130 3630 3322 0a20 2020 2020 2020  3810603".       
+00000440: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00000450: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00000460: 2020 2020 2020 2269 6422 3a20 2231 5067        "id": "1Pg
+00000470: 4857 3158 5a53 6757 7465 4468 7954 6949  HW1XZSgWteDhyTiI
+00000480: 4662 6741 4167 5a57 5a71 5a32 7432 5a47  FbgAAgZWZqZ2t2ZG
+00000490: 4e34 4158 7870 4a77 5a6f 4158 7870 4a77  N4AXxpJwZoAXxpJw
+000004a0: 5266 4141 4141 4141 222c 0a20 2020 2020  RfAAAAAA",.     
+000004b0: 2020 2020 2020 2020 2020 2022 6d65 6469             "medi
+000004c0: 6122 3a20 7b0a 2020 2020 2020 2020 2020  a": {.          
+000004d0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
+000004e0: 3a20 2249 4d41 4745 222c 0a20 2020 2020  : "IMAGE",.     
+000004f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000500: 6d65 6469 6155 726c 223a 2022 6874 7470  mediaUrl": "http
+00000510: 733a 2f2f 6669 6c65 7361 6d70 6c65 732e  s://filesamples.
+00000520: 636f 6d2f 7361 6d70 6c65 732f 7669 6465  com/samples/vide
+00000530: 6f2f 6d70 342f 7361 6d70 6c65 5f36 3430  o/mp4/sample_640
+00000540: 7833 3630 2e6d 7034 220a 2020 2020 2020  x360.mp4".      
+00000550: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+00000560: 2020 2020 2020 2020 2020 2020 2022 6361               "ca
+00000570: 7074 7572 6554 696d 6553 6563 7322 3a20  ptureTimeSecs": 
+00000580: 2231 3633 3338 3531 3733 3722 0a20 2020  "1633851737".   
+00000590: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+000005a0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+000005b0: 2020 2020 2020 2020 2020 2269 6422 3a20            "id": 
+000005c0: 2231 5067 4857 3158 5a53 6757 7465 4468  "1PgHW1XZSgWteDh
+000005d0: 7954 6949 4662 6741 4167 6447 6c79 6558  yTiIFbgAAgdGlyeX
+000005e0: 706f 6447 7834 4158 7870 5234 6a73 4158  podGx4AXxpR4jsAX
+000005f0: 7870 5234 587a 4141 4141 4141 222c 0a20  xpR4XzAAAAAA",. 
+00000600: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000610: 6d65 6469 6122 3a20 7b0a 2020 2020 2020  media": {.      
+00000620: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+00000630: 7970 6522 3a20 2249 4d41 4745 222c 0a20  ype": "IMAGE",. 
 00000640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000650: 2022 7479 7065 223a 2022 494d 4147 4522   "type": "IMAGE"
-00000660: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000670: 2020 2020 2020 2022 6d65 6469 6155 726c         "mediaUrl
-00000680: 223a 2022 6874 7470 733a 2f2f 6669 6c65  ": "https://file
-00000690: 7361 6d70 6c65 732e 636f 6d2f 7361 6d70  samples.com/samp
-000006a0: 6c65 732f 7669 6465 6f2f 6d70 342f 7361  les/video/mp4/sa
-000006b0: 6d70 6c65 5f36 3430 7833 3630 2e6d 7034  mple_640x360.mp4
-000006c0: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
-000006d0: 2020 207d 2c0d 0a20 2020 2020 2020 2020     },..         
-000006e0: 2020 2020 2020 2022 6361 7074 7572 6554         "captureT
-000006f0: 696d 6553 6563 7322 3a20 2231 3633 3338  imeSecs": "16338
-00000700: 3533 3836 3722 0d0a 2020 2020 2020 2020  53867"..        
-00000710: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
-00000720: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
-00000730: 2020 2020 2020 2022 6964 223a 2022 3150         "id": "1P
-00000740: 6748 5731 585a 5367 5774 6544 6879 5469  gHW1XZSgWteDhyTi
-00000750: 4946 6267 4141 6764 6e4a 6c63 3268 6a65  IFbgAAgdnJlc2hje
-00000760: 5764 3541 5878 7168 516a 6a41 5878 7168  Wd5AXxqhQjjAXxqh
-00000770: 5161 6541 4141 4141 4122 2c0d 0a20 2020  QaeAAAAAA",..   
-00000780: 2020 2020 2020 2020 2020 2020 2022 6d65               "me
-00000790: 6469 6122 3a20 7b0d 0a20 2020 2020 2020  dia": {..       
-000007a0: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
-000007b0: 7065 223a 2022 494d 4147 4522 2c0d 0a20  pe": "IMAGE",.. 
-000007c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007d0: 2020 2022 6d65 6469 6155 726c 223a 2022     "mediaUrl": "
-000007e0: 6874 7470 733a 2f2f 6669 6c65 7361 6d70  https://filesamp
-000007f0: 6c65 732e 636f 6d2f 7361 6d70 6c65 732f  les.com/samples/
-00000800: 7669 6465 6f2f 6d70 342f 7361 6d70 6c65  video/mp4/sample
-00000810: 5f36 3430 7833 3630 2e6d 7034 220d 0a20  _640x360.mp4".. 
-00000820: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00000830: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000840: 2020 2022 6361 7074 7572 6554 696d 6553     "captureTimeS
-00000850: 6563 7322 3a20 2231 3633 3338 3734 3637  ecs": "163387467
-00000860: 3522 0d0a 2020 2020 2020 2020 2020 2020  5"..            
-00000870: 7d0d 0a20 2020 2020 2020 205d 0d0a 2020  }..        ]..  
-00000880: 2020 7d0d 0a7d 0d0a                        }..}..
+00000650: 2020 2022 6d65 6469 6155 726c 223a 2022     "mediaUrl": "
+00000660: 6874 7470 733a 2f2f 6669 6c65 7361 6d70  https://filesamp
+00000670: 6c65 732e 636f 6d2f 7361 6d70 6c65 732f  les.com/samples/
+00000680: 7669 6465 6f2f 6d70 342f 7361 6d70 6c65  video/mp4/sample
+00000690: 5f36 3430 7833 3630 2e6d 7034 220a 2020  _640x360.mp4".  
+000006a0: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+000006b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000006c0: 2022 6361 7074 7572 6554 696d 6553 6563   "captureTimeSec
+000006d0: 7322 3a20 2231 3633 3338 3533 3836 3722  s": "1633853867"
+000006e0: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
+000006f0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+00000700: 2020 2020 2020 2020 2020 2020 2020 2269                "i
+00000710: 6422 3a20 2231 5067 4857 3158 5a53 6757  d": "1PgHW1XZSgW
+00000720: 7465 4468 7954 6949 4662 6741 4167 646e  teDhyTiIFbgAAgdn
+00000730: 4a6c 6332 686a 6557 6435 4158 7871 6851  Jlc2hjeWd5AXxqhQ
+00000740: 6a6a 4158 7871 6851 6165 4141 4141 4141  jjAXxqhQaeAAAAAA
+00000750: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00000760: 2020 2022 6d65 6469 6122 3a20 7b0a 2020     "media": {.  
+00000770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000780: 2020 2274 7970 6522 3a20 2249 4d41 4745    "type": "IMAGE
+00000790: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000007a0: 2020 2020 2020 2022 6d65 6469 6155 726c         "mediaUrl
+000007b0: 223a 2022 6874 7470 733a 2f2f 6669 6c65  ": "https://file
+000007c0: 7361 6d70 6c65 732e 636f 6d2f 7361 6d70  samples.com/samp
+000007d0: 6c65 732f 7669 6465 6f2f 6d70 342f 7361  les/video/mp4/sa
+000007e0: 6d70 6c65 5f36 3430 7833 3630 2e6d 7034  mple_640x360.mp4
+000007f0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00000800: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+00000810: 2020 2020 2022 6361 7074 7572 6554 696d       "captureTim
+00000820: 6553 6563 7322 3a20 2231 3633 3338 3734  eSecs": "1633874
+00000830: 3637 3522 0a20 2020 2020 2020 2020 2020  675".           
+00000840: 207d 0a20 2020 2020 2020 205d 0a20 2020   }.        ].   
+00000850: 207d 0a7d 0a                              }.}.
```

### Comparing `snapchat-dlp-1.5.2/tests/test_downlaoder.py` & `snapchat-dlp-1.5.8/tests/test_downlaoder.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-"""Tests for `snapchat_dlp` package."""
-import os
-import shutil
-import unittest
-
-from requests.exceptions import HTTPError
-
-from snapchat_dlp.downloader import download_url
-
-
-def teardown_module(module):
-    shutil.rmtree(".test-data")
-
-
-class Test_downloader(unittest.TestCase):
-    """Tests for `snapchat_dlp.downloader.download_url` package."""
-
-    def setUp(self):
-        """Set up test fixtures."""
-        self.test_url = "https://filesamples.com/samples/video/mp4/sample_640x360.mp4"
-        self.test_url404 = "https://google.com/error.html"
-
-    def test_download_url(self):
-        """Test snapchat_dlp download_url."""
-        download_url(self.test_url, ".test-data/test_dl_23.mp4", sleep_interval=0)
-
-    def test_empty_download(self):
-        """Test snapchat_dlp download_url."""
-        open(".test-data/test_dl_23.mp4", "w").close()
-        download_url(self.test_url, ".test-data/test_dl_23.mp4", sleep_interval=0)
-
-    def test_download_url_raise(self):
-        """Test snapchat_dlp download_url with invalid url."""
-        with self.assertRaises(HTTPError):
-            download_url(
-                self.test_url404, ".test-data/test_dl_23.mp4", sleep_interval=0
-            )
+"""Tests for `snapchat_dlp` package."""
+import os
+import shutil
+import unittest
+
+from requests.exceptions import HTTPError
+
+from snapchat_dlp.downloader import download_url
+
+
+def teardown_module(module):
+    shutil.rmtree(".test-data")
+
+
+class Test_downloader(unittest.TestCase):
+    """Tests for `snapchat_dlp.downloader.download_url` package."""
+
+    def setUp(self):
+        """Set up test fixtures."""
+        self.test_url = "https://filesamples.com/samples/video/mp4/sample_640x360.mp4"
+        self.test_url404 = "https://google.com/error.html"
+
+    def test_download_url(self):
+        """Test snapchat_dlp download_url."""
+        download_url(self.test_url, ".test-data/test_dl_23.mp4", sleep_interval=0)
+
+    def test_empty_download(self):
+        """Test snapchat_dlp download_url."""
+        open(".test-data/test_dl_23.mp4", "w").close()
+        download_url(self.test_url, ".test-data/test_dl_23.mp4", sleep_interval=0)
+
+    def test_download_url_raise(self):
+        """Test snapchat_dlp download_url with invalid url."""
+        with self.assertRaises(HTTPError):
+            download_url(
+                self.test_url404, ".test-data/test_dl_23.mp4", sleep_interval=0
+            )
```

### Comparing `snapchat-dlp-1.5.2/tests/test_snapchat_dl.py` & `snapchat-dlp-1.5.8/tests/test_snapchat_dl.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-#!/usr/bin/env python
-"""Tests for `snapchat_dlp` package."""
-import json
-import os
-import shutil
-import unittest
-from unittest import mock
-
-from snapchat_dlp.snapchat_dlp import SnapchatDL
-from snapchat_dlp.utils import APIResponseError
-from snapchat_dlp.utils import NoStoriesFound
-from snapchat_dlp.utils import UserNotFoundError
-
-
-def teardown_module(module):
-    shutil.rmtree(".test-data")
-
-
-class TestSnapchat_dl(unittest.TestCase):
-    """Tests for `snapchat_dlp` package."""
-
-    def setUp(self):
-        """Set up test fixtures."""
-        self.snapchat_dlp = SnapchatDL(
-            limit_story=10, quiet=True, directory_prefix=".test-data", dump_json=True,
-        )
-        self.test_url = "https://filesamples.com/samples/video/mp4/sample_640x360.mp4"
-        self.test_url404 = "https://google.com/error.html"
-        self.username = "invalidusername"
-        self.html = open(
-            "tests/mock_data/invalidusername.html", "r", encoding="utf8"
-        ).read()
-        self.html_api_error = open(
-            "tests/mock_data/api-error.html", "r", encoding="utf8"
-        ).read()
-        self.html_nostories = open(
-            "tests/mock_data/invalidusername-nostories.html", "r", encoding="utf8"
-        ).read()
-
-    def test_class_init(self):
-        """Test snapchat_dlp init."""
-        self.assertTrue(self.snapchat_dlp)
-
-    def test_invalid_username(self):
-        """Test snapchat_dlp Stories are not available."""
-        with self.assertRaises(UserNotFoundError):
-            self.snapchat_dlp.download("username")
-
-    @mock.patch("snapchat_dlp.snapchat_dlp.SnapchatDL._api_response")
-    def test_api_error(self, api_response):
-        """Test snapchat_dlp Download."""
-        api_response.return_value = self.html_api_error
-        with self.assertRaises(APIResponseError):
-            self.snapchat_dlp.download(self.username)
-
-    @mock.patch("snapchat_dlp.snapchat_dlp.SnapchatDL._api_response")
-    def test_get_stories(self, api_response):
-        """Test snapchat_dlp Download."""
-        api_response.return_value = self.html
-        self.snapchat_dlp.download(self.username)
-
-    @mock.patch("snapchat_dlp.snapchat_dlp.SnapchatDL._api_response")
-    def test_no_stories(self, api_response):
-        """Test snapchat_dlp Download."""
-        api_response.return_value = self.html_nostories
-        with self.assertRaises(NoStoriesFound):
-            self.snapchat_dlp.download(self.username)
+#!/usr/bin/env python
+"""Tests for `snapchat_dlp` package."""
+import json
+import os
+import shutil
+import unittest
+from unittest import mock
+
+from snapchat_dlp.snapchat_dlp import SnapchatDL
+from snapchat_dlp.utils import APIResponseError
+from snapchat_dlp.utils import NoStoriesFound
+from snapchat_dlp.utils import UserNotFoundError
+
+
+def teardown_module(module):
+    shutil.rmtree(".test-data")
+
+
+class TestSnapchat_dl(unittest.TestCase):
+    """Tests for `snapchat_dlp` package."""
+
+    def setUp(self):
+        """Set up test fixtures."""
+        self.snapchat_dlp = SnapchatDL(
+            limit_story=10, quiet=True, directory_prefix=".test-data", dump_json=True,
+        )
+        self.test_url = "https://filesamples.com/samples/video/mp4/sample_640x360.mp4"
+        self.test_url404 = "https://google.com/error.html"
+        self.username = "invalidusername"
+        self.html = open(
+            "tests/mock_data/invalidusername.html", "r", encoding="utf8"
+        ).read()
+        self.html_api_error = open(
+            "tests/mock_data/api-error.html", "r", encoding="utf8"
+        ).read()
+        self.html_nostories = open(
+            "tests/mock_data/invalidusername-nostories.html", "r", encoding="utf8"
+        ).read()
+
+    def test_class_init(self):
+        """Test snapchat_dlp init."""
+        self.assertTrue(self.snapchat_dlp)
+
+    # def test_invalid_username(self):
+    #     """Test snapchat_dlp Stories are not available."""
+    #     with self.assertRaises(UserNotFoundError):
+    #         self.snapchat_dlp.download("username")
+
+    @mock.patch("snapchat_dlp.snapchat_dlp.SnapchatDL._api_response")
+    def test_api_error(self, api_response):
+        """Test snapchat_dlp Download."""
+        api_response.return_value = self.html_api_error
+        with self.assertRaises(APIResponseError):
+            self.snapchat_dlp.download(self.username)
+
+    @mock.patch("snapchat_dlp.snapchat_dlp.SnapchatDL._api_response")
+    def test_get_stories(self, api_response):
+        """Test snapchat_dlp Download."""
+        api_response.return_value = self.html
+        self.snapchat_dlp.download(self.username)
+
+    # @mock.patch("snapchat_dlp.snapchat_dlp.SnapchatDL._api_response")
+    # def test_no_stories(self, api_response):
+    #     """Test snapchat_dlp Download."""
+    #     api_response.return_value = self.html_nostories
+    #     with self.assertRaises(NoStoriesFound):
+    #         self.snapchat_dlp.download(self.username)
```

### Comparing `snapchat-dlp-1.5.2/tests/test_utils.py` & `snapchat-dlp-1.5.8/tests/test_utils.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-#!/usr/bin/env python
-"""Tests for `snapchat_dlp` package."""
-import unittest
-from argparse import Namespace
-
-from snapchat_dlp.utils import search_usernames
-from snapchat_dlp.utils import strf_time
-from snapchat_dlp.utils import use_batch_file
-from snapchat_dlp.utils import use_prefix_dir
-from snapchat_dlp.utils import valid_username
-
-
-class Test_utils(unittest.TestCase):
-    """Tests for `snapchat_dlp` package."""
-
-    def test_valid_username(self):
-        """Test for invalid username."""
-        self.assertFalse(valid_username("2323 2323"))
-
-    def test_strf_time(self):
-        """Test strf_time."""
-        self.assertEqual(
-            strf_time(978307200, "%Y-%m-%dT%H-%M-%S"), "2001-01-01T00-00-00",
-        )
-
-    def test_search_usernames(self):
-        """Test usernames search in string."""
-        string = """
-            https://story.snapchat.com/s/in#invalidusername
-            https://story.snapchat.com/s/username1
-            https://story.snapchat.com/s/user.name2
-            https://story.snapchat.com/s/user_name
-            https://story.snapchat.com/@user_name
-        """
-        usernames = ["user.name2", "user_name", "username1"]
-        self.assertListEqual(search_usernames(string), usernames)
-
-    def test_use_batch_file(self):
-        args = Namespace(batch_file="tests/mock_data/batch_file.txt")
-        usernames = ["username1", "user.name2", "user_name"]
-        self.assertListEqual(use_batch_file(args), usernames)
-
-    def test_use_batch_file_err(self):
-        args = Namespace(batch_file="tests/mock_data/batch_file_err.txt")
-        with self.assertRaises(Exception):
-            use_batch_file(args)
-
-    def test_use_prefix_dir(self):
-        args = Namespace(scan_prefix=True, save_prefix="tests/mock_data", quiet=False)
-        usernames = ["user.1name", "user1"]
-        self.assertListEqual(use_prefix_dir(args), usernames)
+#!/usr/bin/env python
+"""Tests for `snapchat_dlp` package."""
+import unittest
+from argparse import Namespace
+
+from snapchat_dlp.utils import search_usernames
+from snapchat_dlp.utils import strf_time
+from snapchat_dlp.utils import use_batch_file
+from snapchat_dlp.utils import use_prefix_dir
+from snapchat_dlp.utils import valid_username
+
+
+class Test_utils(unittest.TestCase):
+    """Tests for `snapchat_dlp` package."""
+
+    def test_valid_username(self):
+        """Test for invalid username."""
+        self.assertFalse(valid_username("2323 2323"))
+
+    def test_strf_time(self):
+        """Test strf_time."""
+        self.assertEqual(
+            strf_time(978307200, "%Y-%m-%dT%H-%M-%S"), "2001-01-01T00-00-00",
+        )
+
+    def test_search_usernames(self):
+        """Test usernames search in string."""
+        string = """
+            https://story.snapchat.com/s/in#invalidusername
+            https://story.snapchat.com/s/username1
+            https://story.snapchat.com/s/user.name2
+            https://story.snapchat.com/s/user_name
+            https://story.snapchat.com/@user_name
+        """
+        usernames = ["user.name2", "user_name", "username1"]
+        self.assertListEqual(search_usernames(string), usernames)
+
+    def test_use_batch_file(self):
+        args = Namespace(batch_file="tests/mock_data/batch_file.txt")
+        usernames = ["username1", "user.name2", "user_name"]
+        self.assertListEqual(use_batch_file(args), usernames)
+
+    def test_use_batch_file_err(self):
+        args = Namespace(batch_file="tests/mock_data/batch_file_err.txt")
+        with self.assertRaises(Exception):
+            use_batch_file(args)
+
+    def test_use_prefix_dir(self):
+        args = Namespace(scan_prefix=True, save_prefix="tests/mock_data", quiet=False)
+        usernames = ["user.1name", "user1"]
+        self.assertListEqual(use_prefix_dir(args), usernames)
```

