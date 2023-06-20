# Comparing `tmp/fedfind-5.1.0.tar.gz` & `tmp/fedfind-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedfind-5.1.0.tar", last modified: Mon Jun 19 16:04:29 2023, max compression
+gzip compressed data, was "fedfind-5.1.1.tar", last modified: Tue Jun 20 05:11:10 2023, max compression
```

## Comparing `fedfind-5.1.0.tar` & `fedfind-5.1.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-19 16:04:29.408843 fedfind-5.1.0/
--rw-rw-r--   0 adamw     (1000) adamw     (1000)       86 2019-06-18 21:22:51.000000 fedfind-5.1.0/.gitignore
--rw-rw-r--   0 adamw     (1000) adamw     (1000)       29 2019-06-18 21:22:51.000000 fedfind-5.1.0/.pylintrc
--rw-rw-r--   0 adamw     (1000) adamw     (1000)      143 2021-12-09 00:14:01.000000 fedfind-5.1.0/.zuul.yaml
--rw-r--r--   0 adamw     (1000) adamw     (1000)    39157 2023-06-19 16:03:27.000000 fedfind-5.1.0/CHANGELOG.md
--rw-rw-r--   0 adamw     (1000) adamw     (1000)    35147 2015-02-09 17:48:14.000000 fedfind-5.1.0/COPYING
--rw-rw-r--   0 adamw     (1000) adamw     (1000)       37 2019-06-18 21:22:51.000000 fedfind-5.1.0/MANIFEST.in
--rw-r--r--   0 adamw     (1000) adamw     (1000)    27694 2023-06-19 16:04:29.408843 fedfind-5.1.0/PKG-INFO
--rw-rw-r--   0 adamw     (1000) adamw     (1000)    27184 2023-06-19 13:00:44.000000 fedfind-5.1.0/README.md
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-19 16:04:29.399843 fedfind-5.1.0/ci/
--rw-rw-r--   0 adamw     (1000) adamw     (1000)      397 2021-12-09 00:14:01.000000 fedfind-5.1.0/ci/tox.yaml
--rwxrwxr-x   0 adamw     (1000) adamw     (1000)      251 2022-12-03 01:39:32.000000 fedfind-5.1.0/fedfindlocal.py
--rwxrwxr-x   0 adamw     (1000) adamw     (1000)     3012 2021-06-01 19:25:03.000000 fedfind-5.1.0/gen-allstable
--rw-rw-r--   0 adamw     (1000) adamw     (1000)       62 2021-12-03 21:56:52.000000 fedfind-5.1.0/install.requires
--rw-rw-r--   0 adamw     (1000) adamw     (1000)      334 2023-05-05 20:37:05.000000 fedfind-5.1.0/pyproject.toml
--rwxrwxr-x   0 adamw     (1000) adamw     (1000)      658 2021-12-09 00:13:31.000000 fedfind-5.1.0/release.sh
--rw-r--r--   0 adamw     (1000) adamw     (1000)       38 2023-06-19 16:04:29.409843 fedfind-5.1.0/setup.cfg
--rw-rw-r--   0 adamw     (1000) adamw     (1000)     1899 2023-06-19 16:04:05.000000 fedfind-5.1.0/setup.py
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-19 16:04:29.397843 fedfind-5.1.0/src/
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-19 16:04:29.400843 fedfind-5.1.0/src/fedfind/
--rw-rw-r--   0 adamw     (1000) adamw     (1000)      934 2023-06-19 16:04:05.000000 fedfind-5.1.0/src/fedfind/__init__.py
--rwxrwxr-x   0 adamw     (1000) adamw     (1000)    10744 2023-06-19 13:04:57.000000 fedfind-5.1.0/src/fedfind/cli.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)     6962 2023-06-19 12:29:38.000000 fedfind-5.1.0/src/fedfind/const.py
--rw-rw-r--   0 adamw     (1000) adamw     (1000)     2502 2021-12-09 00:14:01.000000 fedfind-5.1.0/src/fedfind/exceptions.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)    31808 2023-06-19 12:29:38.000000 fedfind-5.1.0/src/fedfind/helpers.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)    95352 2023-06-19 16:01:09.000000 fedfind-5.1.0/src/fedfind/release.py
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-19 16:04:29.400843 fedfind-5.1.0/src/fedfind.egg-info/
--rw-rw-r--   0 adamw     (1000) adamw     (1000)    27694 2023-06-19 16:04:29.000000 fedfind-5.1.0/src/fedfind.egg-info/PKG-INFO
--rw-rw-r--   0 adamw     (1000) adamw     (1000)     1611 2023-06-19 16:04:29.000000 fedfind-5.1.0/src/fedfind.egg-info/SOURCES.txt
--rw-rw-r--   0 adamw     (1000) adamw     (1000)        1 2023-06-19 16:04:29.000000 fedfind-5.1.0/src/fedfind.egg-info/dependency_links.txt
--rw-rw-r--   0 adamw     (1000) adamw     (1000)       45 2023-06-19 16:04:29.000000 fedfind-5.1.0/src/fedfind.egg-info/entry_points.txt
--rw-rw-r--   0 adamw     (1000) adamw     (1000)       68 2023-06-19 16:04:29.000000 fedfind-5.1.0/src/fedfind.egg-info/requires.txt
--rw-rw-r--   0 adamw     (1000) adamw     (1000)        8 2023-06-19 16:04:29.000000 fedfind-5.1.0/src/fedfind.egg-info/top_level.txt
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-19 16:04:29.400843 fedfind-5.1.0/tests/
--rw-rw-r--   0 adamw     (1000) adamw     (1000)     7365 2023-06-19 12:27:47.000000 fedfind-5.1.0/tests/conftest.py
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-19 16:04:29.407843 fedfind-5.1.0/tests/data/
--rw-rw-r--   0 adamw     (1000) adamw     (1000)   935072 2023-05-08 23:30:10.000000 fedfind-5.1.0/tests/data/allstable.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)   333754 2023-05-08 23:09:59.000000 fedfind-5.1.0/tests/data/compose-urls-20230508.json
--rwxrwxr-x   0 adamw     (1000) adamw     (1000)     1437 2022-08-02 21:15:03.000000 fedfind-5.1.0/tests/data/fedfindloc.py
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-19 16:04:29.397843 fedfind-5.1.0/tests/data/http/
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-19 16:04:29.397843 fedfind-5.1.0/tests/data/http/pub/
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-19 16:04:29.407843 fedfind-5.1.0/tests/data/http/pub/alt/
--rw-r--r--   0 adamw     (1000) adamw     (1000)   134720 2023-06-19 16:01:37.000000 fedfind-5.1.0/tests/data/http/pub/alt/imagelist-alt
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-19 16:04:29.407843 fedfind-5.1.0/tests/data/http/pub/archive/
--rw-r--r--   0 adamw     (1000) adamw     (1000)   143953 2023-06-19 16:01:37.000000 fedfind-5.1.0/tests/data/http/pub/archive/imagelist-archive
-drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-19 16:04:29.408843 fedfind-5.1.0/tests/data/http/pub/fedora/
--rw-r--r--   0 adamw     (1000) adamw     (1000)    24243 2023-06-19 16:01:37.000000 fedfind-5.1.0/tests/data/http/pub/fedora/imagelist-fedora
--rw-rw-r--   0 adamw     (1000) adamw     (1000)    38788 2019-06-18 21:22:51.000000 fedfind-5.1.0/tests/data/pdc-compimages-Fedora-24-20160614.0.json
--rw-rw-r--   0 adamw     (1000) adamw     (1000)    43446 2019-06-18 21:22:51.000000 fedfind-5.1.0/tests/data/pdc-compimages-Fedora-25-20161115.0.json
--rw-rw-r--   0 adamw     (1000) adamw     (1000)    73734 2019-06-18 21:22:51.000000 fedfind-5.1.0/tests/data/pdc-compimages-Fedora-26-20170705.0.json
--rw-rw-r--   0 adamw     (1000) adamw     (1000)    70323 2019-06-18 21:22:51.000000 fedfind-5.1.0/tests/data/pdc-compimages-Fedora-27-20171105.0.json
--rw-rw-r--   0 adamw     (1000) adamw     (1000)    81069 2020-02-22 02:12:59.000000 fedfind-5.1.0/tests/data/pdc-compimages-Fedora-28-20180425.0.json
--rw-rw-r--   0 adamw     (1000) adamw     (1000)    59560 2020-02-22 02:12:59.000000 fedfind-5.1.0/tests/data/pdc-compimages-Fedora-29-20181024.1.json
--rw-rw-r--   0 adamw     (1000) adamw     (1000)    61551 2020-02-22 02:12:59.000000 fedfind-5.1.0/tests/data/pdc-compimages-Fedora-30-20190425.0.json
--rw-rw-r--   0 adamw     (1000) adamw     (1000)    57550 2020-02-22 02:12:59.000000 fedfind-5.1.0/tests/data/pdc-compimages-Fedora-31-20191023.0.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    59948 2020-04-28 22:05:51.000000 fedfind-5.1.0/tests/data/pdc-compimages-Fedora-32-20200422.0.json
--rw-rw-r--   0 adamw     (1000) adamw     (1000)    65722 2020-10-27 19:34:35.000000 fedfind-5.1.0/tests/data/pdc-compimages-Fedora-33-20201019.0.json
--rw-rw-r--   0 adamw     (1000) adamw     (1000)    63265 2021-12-09 00:14:01.000000 fedfind-5.1.0/tests/data/pdc-compimages-Fedora-34-20210423.0.json
--rw-rw-r--   0 adamw     (1000) adamw     (1000)    66775 2021-12-09 00:14:01.000000 fedfind-5.1.0/tests/data/pdc-compimages-Fedora-35-20211026.0.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    65980 2022-08-02 20:39:18.000000 fedfind-5.1.0/tests/data/pdc-compimages-Fedora-36-20220504.1.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    27726 2023-05-08 23:36:30.000000 fedfind-5.1.0/tests/data/pdc-compimages-Fedora-37-20221105.0.json
--rw-r--r--   0 adamw     (1000) adamw     (1000)    29444 2023-05-08 23:37:40.000000 fedfind-5.1.0/tests/data/pdc-compimages-Fedora-38-20230413.1.json
--rw-rw-r--   0 adamw     (1000) adamw     (1000)    29635 2023-06-19 12:34:05.000000 fedfind-5.1.0/tests/test_helpers.py
--rw-r--r--   0 adamw     (1000) adamw     (1000)    50013 2023-06-19 16:01:09.000000 fedfind-5.1.0/tests/test_release.py
--rw-rw-r--   0 adamw     (1000) adamw     (1000)       58 2021-12-09 00:14:01.000000 fedfind-5.1.0/tests.requires
--rw-rw-r--   0 adamw     (1000) adamw     (1000)      528 2021-12-09 02:15:34.000000 fedfind-5.1.0/tox.ini
--rw-r--r--   0 adamw     (1000) adamw     (1000)       39 2023-01-18 23:43:26.000000 fedfind-5.1.0/tox.requires
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-20 05:11:10.243281 fedfind-5.1.1/
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)       86 2019-06-18 21:22:51.000000 fedfind-5.1.1/.gitignore
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)       29 2019-06-18 21:22:51.000000 fedfind-5.1.1/.pylintrc
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)      143 2021-12-09 00:14:01.000000 fedfind-5.1.1/.zuul.yaml
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    39356 2023-06-20 05:10:28.000000 fedfind-5.1.1/CHANGELOG.md
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)    35147 2015-02-09 17:48:14.000000 fedfind-5.1.1/COPYING
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)       37 2019-06-18 21:22:51.000000 fedfind-5.1.1/MANIFEST.in
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    27694 2023-06-20 05:11:10.243281 fedfind-5.1.1/PKG-INFO
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)    27184 2023-06-19 13:00:44.000000 fedfind-5.1.1/README.md
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-20 05:11:10.240280 fedfind-5.1.1/ci/
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)      397 2021-12-09 00:14:01.000000 fedfind-5.1.1/ci/tox.yaml
+-rwxrwxr-x   0 adamw     (1000) adamw     (1000)      251 2022-12-03 01:39:32.000000 fedfind-5.1.1/fedfindlocal.py
+-rwxrwxr-x   0 adamw     (1000) adamw     (1000)     3012 2021-06-01 19:25:03.000000 fedfind-5.1.1/gen-allstable
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)       62 2021-12-03 21:56:52.000000 fedfind-5.1.1/install.requires
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)      334 2023-05-05 20:37:05.000000 fedfind-5.1.1/pyproject.toml
+-rwxrwxr-x   0 adamw     (1000) adamw     (1000)      658 2021-12-09 00:13:31.000000 fedfind-5.1.1/release.sh
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       38 2023-06-20 05:11:10.243281 fedfind-5.1.1/setup.cfg
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)     1899 2023-06-20 05:10:44.000000 fedfind-5.1.1/setup.py
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-20 05:11:10.239281 fedfind-5.1.1/src/
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-20 05:11:10.240280 fedfind-5.1.1/src/fedfind/
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)      934 2023-06-20 05:10:44.000000 fedfind-5.1.1/src/fedfind/__init__.py
+-rwxrwxr-x   0 adamw     (1000) adamw     (1000)    10744 2023-06-19 13:04:57.000000 fedfind-5.1.1/src/fedfind/cli.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)     6962 2023-06-19 12:29:38.000000 fedfind-5.1.1/src/fedfind/const.py
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)     2502 2021-12-09 00:14:01.000000 fedfind-5.1.1/src/fedfind/exceptions.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    31808 2023-06-19 12:29:38.000000 fedfind-5.1.1/src/fedfind/helpers.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    95491 2023-06-20 05:07:25.000000 fedfind-5.1.1/src/fedfind/release.py
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-20 05:11:10.241280 fedfind-5.1.1/src/fedfind.egg-info/
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)    27694 2023-06-20 05:11:10.000000 fedfind-5.1.1/src/fedfind.egg-info/PKG-INFO
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)     1611 2023-06-20 05:11:10.000000 fedfind-5.1.1/src/fedfind.egg-info/SOURCES.txt
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)        1 2023-06-20 05:11:10.000000 fedfind-5.1.1/src/fedfind.egg-info/dependency_links.txt
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)       45 2023-06-20 05:11:10.000000 fedfind-5.1.1/src/fedfind.egg-info/entry_points.txt
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)       68 2023-06-20 05:11:10.000000 fedfind-5.1.1/src/fedfind.egg-info/requires.txt
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)        8 2023-06-20 05:11:10.000000 fedfind-5.1.1/src/fedfind.egg-info/top_level.txt
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-20 05:11:10.241280 fedfind-5.1.1/tests/
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)     7365 2023-06-19 12:27:47.000000 fedfind-5.1.1/tests/conftest.py
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-20 05:11:10.243281 fedfind-5.1.1/tests/data/
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)   935072 2023-05-08 23:30:10.000000 fedfind-5.1.1/tests/data/allstable.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)   333754 2023-05-08 23:09:59.000000 fedfind-5.1.1/tests/data/compose-urls-20230508.json
+-rwxrwxr-x   0 adamw     (1000) adamw     (1000)     1437 2022-08-02 21:15:03.000000 fedfind-5.1.1/tests/data/fedfindloc.py
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-20 05:11:10.239281 fedfind-5.1.1/tests/data/http/
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-20 05:11:10.239281 fedfind-5.1.1/tests/data/http/pub/
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-20 05:11:10.243281 fedfind-5.1.1/tests/data/http/pub/alt/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)   134720 2023-06-20 05:08:39.000000 fedfind-5.1.1/tests/data/http/pub/alt/imagelist-alt
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-20 05:11:10.243281 fedfind-5.1.1/tests/data/http/pub/archive/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)   143953 2023-06-20 05:08:39.000000 fedfind-5.1.1/tests/data/http/pub/archive/imagelist-archive
+drwxr-xr-x   0 adamw     (1000) adamw     (1000)        0 2023-06-20 05:11:10.243281 fedfind-5.1.1/tests/data/http/pub/fedora/
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    24243 2023-06-20 05:08:39.000000 fedfind-5.1.1/tests/data/http/pub/fedora/imagelist-fedora
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)    38788 2019-06-18 21:22:51.000000 fedfind-5.1.1/tests/data/pdc-compimages-Fedora-24-20160614.0.json
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)    43446 2019-06-18 21:22:51.000000 fedfind-5.1.1/tests/data/pdc-compimages-Fedora-25-20161115.0.json
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)    73734 2019-06-18 21:22:51.000000 fedfind-5.1.1/tests/data/pdc-compimages-Fedora-26-20170705.0.json
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)    70323 2019-06-18 21:22:51.000000 fedfind-5.1.1/tests/data/pdc-compimages-Fedora-27-20171105.0.json
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)    81069 2020-02-22 02:12:59.000000 fedfind-5.1.1/tests/data/pdc-compimages-Fedora-28-20180425.0.json
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)    59560 2020-02-22 02:12:59.000000 fedfind-5.1.1/tests/data/pdc-compimages-Fedora-29-20181024.1.json
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)    61551 2020-02-22 02:12:59.000000 fedfind-5.1.1/tests/data/pdc-compimages-Fedora-30-20190425.0.json
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)    57550 2020-02-22 02:12:59.000000 fedfind-5.1.1/tests/data/pdc-compimages-Fedora-31-20191023.0.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    59948 2020-04-28 22:05:51.000000 fedfind-5.1.1/tests/data/pdc-compimages-Fedora-32-20200422.0.json
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)    65722 2020-10-27 19:34:35.000000 fedfind-5.1.1/tests/data/pdc-compimages-Fedora-33-20201019.0.json
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)    63265 2021-12-09 00:14:01.000000 fedfind-5.1.1/tests/data/pdc-compimages-Fedora-34-20210423.0.json
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)    66775 2021-12-09 00:14:01.000000 fedfind-5.1.1/tests/data/pdc-compimages-Fedora-35-20211026.0.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    65980 2022-08-02 20:39:18.000000 fedfind-5.1.1/tests/data/pdc-compimages-Fedora-36-20220504.1.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    27726 2023-05-08 23:36:30.000000 fedfind-5.1.1/tests/data/pdc-compimages-Fedora-37-20221105.0.json
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    29444 2023-05-08 23:37:40.000000 fedfind-5.1.1/tests/data/pdc-compimages-Fedora-38-20230413.1.json
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)    29635 2023-06-19 12:34:05.000000 fedfind-5.1.1/tests/test_helpers.py
+-rw-r--r--   0 adamw     (1000) adamw     (1000)    50122 2023-06-20 05:08:26.000000 fedfind-5.1.1/tests/test_release.py
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)       58 2021-12-09 00:14:01.000000 fedfind-5.1.1/tests.requires
+-rw-rw-r--   0 adamw     (1000) adamw     (1000)      528 2021-12-09 02:15:34.000000 fedfind-5.1.1/tox.ini
+-rw-r--r--   0 adamw     (1000) adamw     (1000)       39 2023-01-18 23:43:26.000000 fedfind-5.1.1/tox.requires
```

### Comparing `fedfind-5.1.0/CHANGELOG.md` & `fedfind-5.1.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 ## Changelog
 
+### 5.1.1 - 2023-06-19
+
+*   [fedfind-5.1.1.tar.gz](https://files.pythonhosted.org/packages/source/f/fedfind/fedfind-5.1.1.tar.gz)
+
+1.  Specifically refuse to try and find ELN composes by compose ID
+
 ### 5.1.0 - 2023-06-19
 
 *   [fedfind-5.1.0.tar.gz](https://files.pythonhosted.org/packages/source/f/fedfind/fedfind-5.1.0.tar.gz)
 
 1.  Handle Fedora ELN composes as new `ElnCompose` class
 2.  Update test data etc. for Fedora 38 release
```

### Comparing `fedfind-5.1.0/COPYING` & `fedfind-5.1.1/COPYING`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/PKG-INFO` & `fedfind-5.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedfind
-Version: 5.1.0
+Version: 5.1.1
 Summary: Fedora Finder finds Fedora - images, more to come?
 Home-page: https://pagure.io/fedora-qa/fedfind
 Author: Adam Williamson
 Author-email: awilliam@redhat.com
 License: GPLv3+
 Keywords: fedora release image media iso
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fedfind-5.1.0/README.md` & `fedfind-5.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/gen-allstable` & `fedfind-5.1.1/gen-allstable`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/release.sh` & `fedfind-5.1.1/release.sh`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/setup.py` & `fedfind-5.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         LONGDESC = f.read()
 except TypeError:
     with open(path.join(HERE, 'README.md')) as f:
         LONGDESC = f.read()
 
 setup(
     name="fedfind",
-    version="5.1.0",
+    version="5.1.1",
     entry_points={'console_scripts': ['fedfind = fedfind.cli:main'],},
     author="Adam Williamson",
     author_email="awilliam@redhat.com",
     description="Fedora Finder finds Fedora - images, more to come?",
     license="GPLv3+",
     keywords="fedora release image media iso",
     url="https://pagure.io/fedora-qa/fedfind",
```

### Comparing `fedfind-5.1.0/src/fedfind/__init__.py` & `fedfind-5.1.1/src/fedfind/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,10 +18,10 @@
 """Library and CLI tool for locating and getting information about
 Fedora composes.
 """
 
 from __future__ import unicode_literals
 from __future__ import print_function
 
-__version__ = "5.1.0"
+__version__ = "5.1.1"
 
 # vim: set textwidth=100 ts=8 et sw=4:
```

### Comparing `fedfind-5.1.0/src/fedfind/cli.py` & `fedfind-5.1.1/src/fedfind/cli.py`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/src/fedfind/const.py` & `fedfind-5.1.1/src/fedfind/const.py`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/src/fedfind/exceptions.py` & `fedfind-5.1.1/src/fedfind/exceptions.py`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/src/fedfind/helpers.py` & `fedfind-5.1.1/src/fedfind/helpers.py`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/src/fedfind/release.py` & `fedfind-5.1.1/src/fedfind/release.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,18 @@
 
     # Reject EPEL composes, we do not handle these
     if "-epel-" in dist.lower():
         raise fedfind.exceptions.UnsupportedComposeError(
             "get_release(): fedfind does not support EPEL composes"
         )
 
+    # Cannot find ELN composes by compose ID
+    if release == "Eln":
+        raise ValueError("Cannot find ELN composes by compose ID!")
+
     # Various stable nightly compose types
     if dist in ("Fedora-Container", "Fedora-Cloud", "Fedora-IoT"):
         return (dist, release, "", date, int(respin))
 
     # Semi-official stable live respin composes
     if dist == "FedoraRespin":
         return (dist, release, "", date, 0)
```

### Comparing `fedfind-5.1.0/src/fedfind.egg-info/PKG-INFO` & `fedfind-5.1.1/src/fedfind.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedfind
-Version: 5.1.0
+Version: 5.1.1
 Summary: Fedora Finder finds Fedora - images, more to come?
 Home-page: https://pagure.io/fedora-qa/fedfind
 Author: Adam Williamson
 Author-email: awilliam@redhat.com
 License: GPLv3+
 Keywords: fedora release image media iso
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fedfind-5.1.0/src/fedfind.egg-info/SOURCES.txt` & `fedfind-5.1.1/src/fedfind.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/tests/conftest.py` & `fedfind-5.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/tests/data/allstable.json` & `fedfind-5.1.1/tests/data/allstable.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/tests/data/compose-urls-20230508.json` & `fedfind-5.1.1/tests/data/compose-urls-20230508.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/tests/data/fedfindloc.py` & `fedfind-5.1.1/tests/data/fedfindloc.py`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/tests/data/http/pub/alt/imagelist-alt` & `fedfind-5.1.1/tests/data/http/pub/alt/imagelist-alt`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/tests/data/http/pub/archive/imagelist-archive` & `fedfind-5.1.1/tests/data/http/pub/archive/imagelist-archive`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/tests/data/http/pub/fedora/imagelist-fedora` & `fedfind-5.1.1/tests/data/http/pub/fedora/imagelist-fedora`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/tests/data/pdc-compimages-Fedora-24-20160614.0.json` & `fedfind-5.1.1/tests/data/pdc-compimages-Fedora-24-20160614.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/tests/data/pdc-compimages-Fedora-25-20161115.0.json` & `fedfind-5.1.1/tests/data/pdc-compimages-Fedora-25-20161115.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/tests/data/pdc-compimages-Fedora-26-20170705.0.json` & `fedfind-5.1.1/tests/data/pdc-compimages-Fedora-26-20170705.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/tests/data/pdc-compimages-Fedora-27-20171105.0.json` & `fedfind-5.1.1/tests/data/pdc-compimages-Fedora-27-20171105.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/tests/data/pdc-compimages-Fedora-28-20180425.0.json` & `fedfind-5.1.1/tests/data/pdc-compimages-Fedora-28-20180425.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/tests/data/pdc-compimages-Fedora-29-20181024.1.json` & `fedfind-5.1.1/tests/data/pdc-compimages-Fedora-29-20181024.1.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/tests/data/pdc-compimages-Fedora-30-20190425.0.json` & `fedfind-5.1.1/tests/data/pdc-compimages-Fedora-30-20190425.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/tests/data/pdc-compimages-Fedora-31-20191023.0.json` & `fedfind-5.1.1/tests/data/pdc-compimages-Fedora-31-20191023.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/tests/data/pdc-compimages-Fedora-32-20200422.0.json` & `fedfind-5.1.1/tests/data/pdc-compimages-Fedora-32-20200422.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/tests/data/pdc-compimages-Fedora-33-20201019.0.json` & `fedfind-5.1.1/tests/data/pdc-compimages-Fedora-33-20201019.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/tests/data/pdc-compimages-Fedora-34-20210423.0.json` & `fedfind-5.1.1/tests/data/pdc-compimages-Fedora-34-20210423.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/tests/data/pdc-compimages-Fedora-35-20211026.0.json` & `fedfind-5.1.1/tests/data/pdc-compimages-Fedora-35-20211026.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/tests/data/pdc-compimages-Fedora-36-20220504.1.json` & `fedfind-5.1.1/tests/data/pdc-compimages-Fedora-36-20220504.1.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/tests/data/pdc-compimages-Fedora-37-20221105.0.json` & `fedfind-5.1.1/tests/data/pdc-compimages-Fedora-37-20221105.0.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/tests/data/pdc-compimages-Fedora-38-20230413.1.json` & `fedfind-5.1.1/tests/data/pdc-compimages-Fedora-38-20230413.1.json`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/tests/test_helpers.py` & `fedfind-5.1.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `fedfind-5.1.0/tests/test_release.py` & `fedfind-5.1.1/tests/test_release.py`

 * *Files 1% similar despite different names*

```diff
@@ -851,14 +851,16 @@
             got.get_package_nevras_pdc(["somepackage"])
         got = fedfind.release.get_release(url="https://odcs.fedoraproject.org/composes/odcs-28282")
         assert isinstance(got, fedfind.release.ElnCompose)
         with pytest.raises(ValueError):
             fedfind.release.get_release("ELN")
         with pytest.raises(ValueError):
             fedfind.release.get_release("ELN", "", "notanum")
+        with pytest.raises(ValueError):
+            fedfind.release.get_release(cid="Fedora-ELN-20230620.0")
 
     @mock.patch("fedfind.helpers.urlopen_retries", urlopen_fake_package)
     def test_get_package_nvras_fc1(self):
         """FC1: no /Everything, no /source, no split-by-initials."""
         rel = fedfind.release.get_release(1)
         pkgs = rel.get_package_nvras(["amanda", "anaconda", "bash", "fakepackage"])
         assert pkgs == {
```

### Comparing `fedfind-5.1.0/tox.ini` & `fedfind-5.1.1/tox.ini`

 * *Files identical despite different names*

