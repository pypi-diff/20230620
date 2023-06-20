# Comparing `tmp/pymonetdb-1.6.4.tar.gz` & `tmp/pymonetdb-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonetdb-1.6.4.tar", last modified: Fri Mar  3 10:33:23 2023, max compression
+gzip compressed data, was "pymonetdb-1.7.0.tar", last modified: Tue Jun 20 10:09:25 2023, max compression
```

## Comparing `pymonetdb-1.6.4.tar` & `pymonetdb-1.7.0.tar`

### file list

```diff
@@ -1,59 +1,61 @@
-drwxr-xr-x   0 jvr       (1000) jvr       (1000)        0 2023-03-03 10:33:23.669340 pymonetdb-1.6.4/
--rw-r--r--   0 jvr       (1000) jvr       (1000)     4264 2023-03-03 10:29:09.000000 pymonetdb-1.6.4/CHANGES
--rw-r--r--   0 jvr       (1000) jvr       (1000)    16724 2020-04-17 14:15:11.000000 pymonetdb-1.6.4/LICENSE
--rw-r--r--   0 jvr       (1000) jvr       (1000)       40 2020-04-17 14:15:11.000000 pymonetdb-1.6.4/MANIFEST.in
--rw-r--r--   0 jvr       (1000) jvr       (1000)     2231 2023-03-03 10:33:23.669340 pymonetdb-1.6.4/PKG-INFO
--rw-r--r--   0 jvr       (1000) jvr       (1000)     1354 2022-12-14 11:07:36.000000 pymonetdb-1.6.4/README.rst
--rwxr-xr-x   0 jvr       (1000) jvr       (1000)     1881 2023-02-21 16:38:41.000000 pymonetdb-1.6.4/p.py
-drwxr-xr-x   0 jvr       (1000) jvr       (1000)        0 2023-03-03 10:33:23.665339 pymonetdb-1.6.4/pymonetdb/
--rw-r--r--   0 jvr       (1000) jvr       (1000)     2303 2023-02-15 15:27:22.000000 pymonetdb-1.6.4/pymonetdb/__init__.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)     7777 2022-12-14 11:07:36.000000 pymonetdb-1.6.4/pymonetdb/control.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)     3007 2022-12-14 11:07:36.000000 pymonetdb-1.6.4/pymonetdb/exceptions.py
-drwxr-xr-x   0 jvr       (1000) jvr       (1000)        0 2023-03-03 10:33:23.665339 pymonetdb-1.6.4/pymonetdb/filetransfer/
--rw-r--r--   0 jvr       (1000) jvr       (1000)     3645 2023-02-15 08:53:32.000000 pymonetdb-1.6.4/pymonetdb/filetransfer/__init__.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)     6113 2022-12-14 11:07:36.000000 pymonetdb-1.6.4/pymonetdb/filetransfer/directoryhandler.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)     5079 2022-12-14 11:07:36.000000 pymonetdb-1.6.4/pymonetdb/filetransfer/downloads.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)     9889 2022-12-14 11:07:36.000000 pymonetdb-1.6.4/pymonetdb/filetransfer/uploads.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)    20710 2023-03-03 10:22:31.000000 pymonetdb-1.6.4/pymonetdb/mapi.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)     1515 2022-12-14 11:07:36.000000 pymonetdb-1.6.4/pymonetdb/profiler.py
-drwxr-xr-x   0 jvr       (1000) jvr       (1000)        0 2023-03-03 10:33:23.665339 pymonetdb-1.6.4/pymonetdb/sql/
--rw-r--r--   0 jvr       (1000) jvr       (1000)      268 2020-04-17 14:15:11.000000 pymonetdb-1.6.4/pymonetdb/sql/__init__.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)     8503 2023-03-03 10:22:31.000000 pymonetdb-1.6.4/pymonetdb/sql/connections.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)    18543 2023-03-03 10:22:31.000000 pymonetdb-1.6.4/pymonetdb/sql/cursors.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)     9158 2022-12-14 11:07:36.000000 pymonetdb-1.6.4/pymonetdb/sql/debug.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)     2786 2022-12-14 11:07:36.000000 pymonetdb-1.6.4/pymonetdb/sql/monetize.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)     5933 2023-03-03 10:22:31.000000 pymonetdb-1.6.4/pymonetdb/sql/pythonize.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)     2469 2023-01-09 14:22:39.000000 pymonetdb-1.6.4/pymonetdb/sql/types.py
-drwxr-xr-x   0 jvr       (1000) jvr       (1000)        0 2023-03-03 10:33:23.665339 pymonetdb-1.6.4/pymonetdb.egg-info/
--rw-r--r--   0 jvr       (1000) jvr       (1000)     2231 2023-03-03 10:33:23.000000 pymonetdb-1.6.4/pymonetdb.egg-info/PKG-INFO
--rw-r--r--   0 jvr       (1000) jvr       (1000)     1157 2023-03-03 10:33:23.000000 pymonetdb-1.6.4/pymonetdb.egg-info/SOURCES.txt
--rw-r--r--   0 jvr       (1000) jvr       (1000)        1 2023-03-03 10:33:23.000000 pymonetdb-1.6.4/pymonetdb.egg-info/dependency_links.txt
--rw-r--r--   0 jvr       (1000) jvr       (1000)       80 2023-03-03 10:33:23.000000 pymonetdb-1.6.4/pymonetdb.egg-info/requires.txt
--rw-r--r--   0 jvr       (1000) jvr       (1000)       16 2023-03-03 10:33:23.000000 pymonetdb-1.6.4/pymonetdb.egg-info/top_level.txt
--rw-r--r--   0 jvr       (1000) jvr       (1000)      116 2023-03-03 10:33:23.669340 pymonetdb-1.6.4/setup.cfg
--rwxr-xr-x   0 jvr       (1000) jvr       (1000)     1646 2023-03-03 10:22:48.000000 pymonetdb-1.6.4/setup.py
--rwxr-xr-x   0 jvr       (1000) jvr       (1000)      538 2023-02-28 11:38:38.000000 pymonetdb-1.6.4/t.py
-drwxr-xr-x   0 jvr       (1000) jvr       (1000)        0 2023-03-03 10:33:23.669340 pymonetdb-1.6.4/tests/
--rw-r--r--   0 jvr       (1000) jvr       (1000)        0 2022-12-14 11:07:36.000000 pymonetdb-1.6.4/tests/__init__.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)     4559 2022-12-14 11:07:36.000000 pymonetdb-1.6.4/tests/install_monetdb_from_msi_dir.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)    13727 2022-12-14 11:07:36.000000 pymonetdb-1.6.4/tests/test_capabilities.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)     5810 2023-02-15 08:53:32.000000 pymonetdb-1.6.4/tests/test_control.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)    27404 2022-12-14 11:07:36.000000 pymonetdb-1.6.4/tests/test_dbapi2.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)     1329 2022-12-14 11:07:36.000000 pymonetdb-1.6.4/tests/test_exceptions.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)    31037 2023-03-03 10:22:31.000000 pymonetdb-1.6.4/tests/test_filetransfer.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)      581 2023-03-03 10:22:31.000000 pymonetdb-1.6.4/tests/test_mapi.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)     3283 2023-02-15 08:53:32.000000 pymonetdb-1.6.4/tests/test_mapi_uri.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)     1938 2022-12-14 11:07:36.000000 pymonetdb-1.6.4/tests/test_monetize.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)     2321 2022-12-14 11:07:36.000000 pymonetdb-1.6.4/tests/test_multiline.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)     1148 2022-12-14 11:07:36.000000 pymonetdb-1.6.4/tests/test_namedtuple.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)      382 2023-02-24 08:37:34.000000 pymonetdb-1.6.4/tests/test_oid.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)      962 2023-03-01 09:18:47.000000 pymonetdb-1.6.4/tests/test_prepare.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)     1055 2023-03-03 10:22:31.000000 pymonetdb-1.6.4/tests/test_profiler.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)     2703 2022-12-14 11:07:36.000000 pymonetdb-1.6.4/tests/test_pythonize.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)     2169 2022-12-14 11:07:36.000000 pymonetdb-1.6.4/tests/test_temporal.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)     1740 2022-12-14 11:07:36.000000 pymonetdb-1.6.4/tests/test_udf.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)     5969 2022-12-14 11:07:36.000000 pymonetdb-1.6.4/tests/test_unicode.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)     1103 2023-03-03 10:22:31.000000 pymonetdb-1.6.4/tests/util.py
--rw-r--r--   0 jvr       (1000) jvr       (1000)     2646 2022-12-14 11:07:36.000000 pymonetdb-1.6.4/tests/windows_tests.py
--rwxr-xr-x   0 jvr       (1000) jvr       (1000)      663 2023-02-23 09:10:00.000000 pymonetdb-1.6.4/tt.py
--rwxr-xr-x   0 jvr       (1000) jvr       (1000)      548 2023-02-13 12:25:12.000000 pymonetdb-1.6.4/ttt.py
+drwxr-xr-x   0 jvr       (1000) jvr       (1000)        0 2023-06-20 10:09:25.202924 pymonetdb-1.7.0/
+-rw-r--r--   0 jvr       (1000) jvr       (1000)    16724 2020-04-17 14:15:11.000000 pymonetdb-1.7.0/LICENSE
+-rw-r--r--   0 jvr       (1000) jvr       (1000)       40 2020-04-17 14:15:11.000000 pymonetdb-1.7.0/MANIFEST.in
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     2282 2023-06-20 10:09:25.202924 pymonetdb-1.7.0/PKG-INFO
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     1354 2023-06-16 14:17:29.000000 pymonetdb-1.7.0/README.rst
+drwxr-xr-x   0 jvr       (1000) jvr       (1000)        0 2023-06-20 10:09:25.198924 pymonetdb-1.7.0/pymonetdb/
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     2303 2023-05-12 14:19:33.000000 pymonetdb-1.7.0/pymonetdb/__init__.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     7776 2023-06-20 07:12:44.000000 pymonetdb-1.7.0/pymonetdb/control.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     3007 2023-05-12 14:19:33.000000 pymonetdb-1.7.0/pymonetdb/exceptions.py
+drwxr-xr-x   0 jvr       (1000) jvr       (1000)        0 2023-06-20 10:09:25.198924 pymonetdb-1.7.0/pymonetdb/filetransfer/
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     3645 2023-05-12 14:19:33.000000 pymonetdb-1.7.0/pymonetdb/filetransfer/__init__.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     6113 2023-05-12 14:19:33.000000 pymonetdb-1.7.0/pymonetdb/filetransfer/directoryhandler.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     5079 2023-05-12 14:19:33.000000 pymonetdb-1.7.0/pymonetdb/filetransfer/downloads.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     9889 2023-05-25 10:35:44.000000 pymonetdb-1.7.0/pymonetdb/filetransfer/uploads.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)    23044 2023-06-20 07:12:44.000000 pymonetdb-1.7.0/pymonetdb/mapi.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     3733 2023-06-16 15:01:58.000000 pymonetdb-1.7.0/pymonetdb/policy.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     1515 2023-06-20 07:12:44.000000 pymonetdb-1.7.0/pymonetdb/profiler.py
+drwxr-xr-x   0 jvr       (1000) jvr       (1000)        0 2023-06-20 10:09:25.198924 pymonetdb-1.7.0/pymonetdb/sql/
+-rw-r--r--   0 jvr       (1000) jvr       (1000)      268 2023-05-12 14:19:33.000000 pymonetdb-1.7.0/pymonetdb/sql/__init__.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)    11301 2023-06-20 07:12:44.000000 pymonetdb-1.7.0/pymonetdb/sql/connections.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)    23282 2023-06-20 07:42:00.000000 pymonetdb-1.7.0/pymonetdb/sql/cursors.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     9158 2023-05-12 14:19:33.000000 pymonetdb-1.7.0/pymonetdb/sql/debug.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     2786 2023-05-12 14:19:33.000000 pymonetdb-1.7.0/pymonetdb/sql/monetize.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     6720 2023-06-16 15:01:58.000000 pymonetdb-1.7.0/pymonetdb/sql/pythonize.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)    12731 2023-06-16 15:01:58.000000 pymonetdb-1.7.0/pymonetdb/sql/pythonizebin.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     2469 2023-05-12 14:19:33.000000 pymonetdb-1.7.0/pymonetdb/sql/types.py
+drwxr-xr-x   0 jvr       (1000) jvr       (1000)        0 2023-06-20 10:09:25.198924 pymonetdb-1.7.0/pymonetdb.egg-info/
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     2282 2023-06-20 10:09:25.000000 pymonetdb-1.7.0/pymonetdb.egg-info/PKG-INFO
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     1277 2023-06-20 10:09:25.000000 pymonetdb-1.7.0/pymonetdb.egg-info/SOURCES.txt
+-rw-r--r--   0 jvr       (1000) jvr       (1000)        1 2023-06-20 10:09:25.000000 pymonetdb-1.7.0/pymonetdb.egg-info/dependency_links.txt
+-rw-r--r--   0 jvr       (1000) jvr       (1000)       80 2023-06-20 10:09:25.000000 pymonetdb-1.7.0/pymonetdb.egg-info/requires.txt
+-rw-r--r--   0 jvr       (1000) jvr       (1000)       16 2023-06-20 10:09:25.000000 pymonetdb-1.7.0/pymonetdb.egg-info/top_level.txt
+-rw-r--r--   0 jvr       (1000) jvr       (1000)      116 2023-06-20 10:09:25.202924 pymonetdb-1.7.0/setup.cfg
+-rwxr-xr-x   0 jvr       (1000) jvr       (1000)     1696 2023-06-20 10:04:33.000000 pymonetdb-1.7.0/setup.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)      470 2023-06-20 07:20:53.000000 pymonetdb-1.7.0/t.py
+drwxr-xr-x   0 jvr       (1000) jvr       (1000)        0 2023-06-20 10:09:25.202924 pymonetdb-1.7.0/tests/
+-rw-r--r--   0 jvr       (1000) jvr       (1000)        0 2023-05-12 14:19:33.000000 pymonetdb-1.7.0/tests/__init__.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     4559 2023-05-12 14:19:33.000000 pymonetdb-1.7.0/tests/install_monetdb_from_msi_dir.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)    13727 2023-06-16 13:36:57.000000 pymonetdb-1.7.0/tests/test_capabilities.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     3247 2023-06-16 13:36:57.000000 pymonetdb-1.7.0/tests/test_contextmanager.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     6147 2023-06-20 07:12:44.000000 pymonetdb-1.7.0/tests/test_control.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)    27404 2023-06-16 13:36:57.000000 pymonetdb-1.7.0/tests/test_dbapi2.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     1329 2023-06-16 13:36:57.000000 pymonetdb-1.7.0/tests/test_exceptions.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     1199 2023-06-20 09:53:39.000000 pymonetdb-1.7.0/tests/test_execute.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)    31047 2023-06-16 15:01:58.000000 pymonetdb-1.7.0/tests/test_filetransfer.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)      591 2023-06-16 15:01:58.000000 pymonetdb-1.7.0/tests/test_mapi.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     3283 2023-06-20 07:12:44.000000 pymonetdb-1.7.0/tests/test_mapi_uri.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     1938 2023-05-12 14:19:33.000000 pymonetdb-1.7.0/tests/test_monetize.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     2321 2023-05-12 14:19:33.000000 pymonetdb-1.7.0/tests/test_multiline.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     1148 2023-06-16 13:36:57.000000 pymonetdb-1.7.0/tests/test_namedtuple.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)      382 2023-06-16 13:36:57.000000 pymonetdb-1.7.0/tests/test_oid.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)    16927 2023-06-20 07:12:44.000000 pymonetdb-1.7.0/tests/test_policy.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)      962 2023-06-16 13:36:57.000000 pymonetdb-1.7.0/tests/test_prepare.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     1060 2023-06-16 15:01:58.000000 pymonetdb-1.7.0/tests/test_profiler.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     3367 2023-06-16 14:30:59.000000 pymonetdb-1.7.0/tests/test_pythonize.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)    19558 2023-06-16 15:01:58.000000 pymonetdb-1.7.0/tests/test_resultset.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     2169 2023-05-12 14:19:33.000000 pymonetdb-1.7.0/tests/test_temporal.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     1733 2023-06-16 15:01:58.000000 pymonetdb-1.7.0/tests/test_udf.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     5969 2023-06-16 13:36:57.000000 pymonetdb-1.7.0/tests/test_unicode.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     2325 2023-06-20 07:12:44.000000 pymonetdb-1.7.0/tests/util.py
+-rw-r--r--   0 jvr       (1000) jvr       (1000)     2646 2023-05-12 14:19:33.000000 pymonetdb-1.7.0/tests/windows_tests.py
```

### Comparing `pymonetdb-1.6.4/LICENSE` & `pymonetdb-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymonetdb-1.6.4/PKG-INFO` & `pymonetdb-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonetdb
-Version: 1.6.4
+Version: 1.7.0
 Summary: Native MonetDB client Python API
 Home-page: http://www.monetdb.org/
 Download-URL: https://github.com/MonetDB/pymonetdb
 Author: MonetDB BV
 Author-email: info@monetdb.org
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Database Engines/Servers
@@ -12,14 +12,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Provides-Extra: test
 Provides-Extra: doc
 License-File: LICENSE
 
 .. This Source Code Form is subject to the terms of the Mozilla Public
 .. License, v. 2.0.  If a copy of the MPL was not distributed with this
```

### Comparing `pymonetdb-1.6.4/README.rst` & `pymonetdb-1.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `pymonetdb-1.6.4/pymonetdb/__init__.py` & `pymonetdb-1.7.0/pymonetdb/__init__.py`

 * *Files identical despite different names*

### Comparing `pymonetdb-1.6.4/pymonetdb/control.py` & `pymonetdb-1.7.0/pymonetdb/control.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         result = self.server.cmd("%s %s\n" % (database_name, command))
         self.server.disconnect()
         return result
 
     def create(self, database_name):
         """
         Initialises a new database or multiplexfunnel in the MonetDB Server.
-        A database created with this command makes it available  for use,
+        A database created with this command makes it available for use,
         however in maintenance mode (see pymonetdb lock).
         """
         return isempty(self._send_command(database_name, "create"))
 
     def destroy(self, database_name):
         """
         Removes the given database, including all its data and
```

### Comparing `pymonetdb-1.6.4/pymonetdb/exceptions.py` & `pymonetdb-1.7.0/pymonetdb/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymonetdb-1.6.4/pymonetdb/filetransfer/__init__.py` & `pymonetdb-1.7.0/pymonetdb/filetransfer/__init__.py`

 * *Files identical despite different names*

### Comparing `pymonetdb-1.6.4/pymonetdb/filetransfer/directoryhandler.py` & `pymonetdb-1.7.0/pymonetdb/filetransfer/directoryhandler.py`

 * *Files identical despite different names*

### Comparing `pymonetdb-1.6.4/pymonetdb/filetransfer/downloads.py` & `pymonetdb-1.7.0/pymonetdb/filetransfer/downloads.py`

 * *Files identical despite different names*

### Comparing `pymonetdb-1.6.4/pymonetdb/filetransfer/uploads.py` & `pymonetdb-1.7.0/pymonetdb/filetransfer/uploads.py`

 * *Files identical despite different names*

### Comparing `pymonetdb-1.6.4/pymonetdb/mapi.py` & `pymonetdb-1.7.0/pymonetdb/mapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 import socket
 import logging
 import struct
 import hashlib
 import os
 import typing
-from typing import Optional, Tuple
-from urllib.parse import urlparse, parse_qs
+from typing import Callable, Dict, List, Optional, Tuple
+from urllib.parse import parse_qsl, urlparse
 
 from pymonetdb.exceptions import OperationalError, DatabaseError, \
     ProgrammingError, NotSupportedError, IntegrityError
 
 if typing.TYPE_CHECKING:
     from pymonetdb.filetransfer.downloads import Downloader
     from pymonetdb.filetransfer.uploads import Uploader
@@ -42,15 +42,16 @@
 MSG_QBLOCK = "&6"
 MSG_HEADER = "%"
 MSG_TUPLE = "["
 MSG_TUPLE_NOSLICE = "="
 MSG_REDIRECT = "^"
 MSG_OK = "=OK"
 
-MSG_FILETRANS_B = bytes(MSG_FILETRANS, 'utf-8')
+MSG_ERROR_B = bytes(MSG_ERROR, 'ascii')
+MSG_FILETRANS_B = bytes(MSG_FILETRANS, 'ascii')
 
 STATE_INIT = 0
 STATE_READY = 1
 
 # MonetDB error codes
 errors = {
     '42S02': OperationalError,  # no such table
@@ -96,33 +97,36 @@
         self.socket = None
         self.unix_socket = None
         self.hostname = ""
         self.port = 0
         self.username = ""
         self.database = ""
         self.language = ""
-        self.handshake_options = None
+        self.handshake_options_callback = None
+        self.remaining_handshake_options = []
         self.connect_timeout = socket.getdefaulttimeout()
         self.uploader = None
         self.downloader = None
         self.stashed_buffer = None
 
     def connect(self, database: str, username: str, password: str, language: str,  # noqa: C901
                 hostname: Optional[str] = None, port: Optional[int] = None, unix_socket=None, connect_timeout=-1,
-                handshake_options=None):
+                handshake_options_callback: Callable[[bool], List['HandshakeOption']] = lambda x: []):
         """ setup connection to MAPI server
 
         unix_socket is used if hostname is not defined.
         """
 
+        url_options = {}
         if ':' in database:
             if not database.startswith('mapi:monetdb:'):
                 raise DatabaseError("colon not allowed in database name, except as part of "
                                     "mapi:monetdb://<hostname>[:<port>]/<database> URI")
             parsed = urlparse(database[5:])
+            url_options = dict(parse_qsl(parsed.query))
             # parse basic settings
             if parsed.hostname or parsed.port:
                 # connect over tcp
                 if not parsed.path.startswith('/'):
                     raise DatabaseError('invalid mapi url')
                 database = parsed.path[1:]
                 if '/' in database:
@@ -133,23 +137,19 @@
                 port = parsed.port or port
             else:
                 # connect over unix domain socket
                 unix_socket = parsed.path or unix_socket
                 username = parsed.username or username
                 password = parsed.password or password
                 database = ''  # must be set in uri parameter
-            # parse uri parameters
-            if parsed.query:
-                parms = parse_qs(parsed.query)
-                if 'database' in parms:
-                    if database == '':
-                        database = parms['database'][-1]
-                    else:
-                        raise DatabaseError('database= query parameter is only allowed with unix domain sockets')
-                # Future work: parse other parameters such as reply_size.
+            if 'database' in url_options:
+                if database == '':
+                    database = url_options['database']
+                else:
+                    raise DatabaseError('database= query parameter is only allowed with unix domain sockets')
 
         if hostname and hostname[:1] == '/' and not unix_socket:
             unix_socket = f'{hostname}/.s.monetdb.{port}'
             hostname = None
         if not unix_socket and os.path.exists(f"/tmp/.s.monetdb.{port}"):
             unix_socket = f"/tmp/.s.monetdb.{port}"
         elif not unix_socket and not hostname:
@@ -162,15 +162,15 @@
 
         self.hostname = hostname
         self.port = port
         self.username = username
         self.database = database
         self.language = language
         self.unix_socket = unix_socket
-        self.handshake_options = handshake_options or []
+        self.handshake_options_callback = handshake_options_callback
         if hostname:
             if self.socket:
                 self.socket.close()
                 self.socket = None
             for af, socktype, proto, canonname, sa in socket.getaddrinfo(hostname, port,
                                                                          socket.AF_UNSPEC, socket.SOCK_STREAM):
                 try:
@@ -199,25 +199,31 @@
             self.socket.connect(unix_socket)
             if self.language != 'control':
                 # don't know why, but we need to do this
                 self.socket.send('0'.encode())
 
         if not (self.language == 'control' and not self.hostname):
             # control doesn't require authentication over socket
-            self._login(password=password)
+            self._login(password=password, url_options=url_options)
 
         self.socket.settimeout(socket.getdefaulttimeout())
         self.state = STATE_READY
 
-    def _login(self, password: str, iteration=0):
+        for opt in self.remaining_handshake_options:
+            opt.fallback(opt.value)
+
+    def _login(self, password: str, url_options: Dict[str, str], iteration=0):
         """ Reads challenge from line, generate response and check if
         everything is okay """
 
+        assert self.socket
+        self.socket.sendall(b'\x00\x00\x00\x00\x00\x00\x00\x00')
+
         challenge = self._getblock()
-        response = self._challenge_response(challenge, password)
+        response = self._challenge_response(challenge, password, url_options)
         self._putblock(response)
         prompt = self._getblock().strip()
 
         if len(prompt) == 0:
             # Empty response, server is happy
             pass
         elif prompt == MSG_OK:
@@ -232,15 +238,15 @@
         elif prompt.startswith(MSG_REDIRECT):
             # a redirect can contain multiple redirects, for now we only use
             # the first
             redirect = prompt.split()[0][1:].split(':')
             if redirect[1] == "merovingian":
                 logger.debug("restarting authentication")
                 if iteration <= 10:
-                    self._login(iteration=iteration + 1, password=password)
+                    self._login(iteration=iteration + 1, password=password, url_options={})
                 else:
                     raise OperationalError("maximal number of redirects "
                                            "reached (10)")
 
             elif redirect[1] == "monetdb":
                 self.hostname = redirect[2][2:]
                 self.port, self.database = redirect[3].split('/')
@@ -278,15 +284,15 @@
             sock.send(bad_header + bad_body)
             # and then we hang up
             sock.close()
         except Exception:
             # don't care
             pass
 
-    def cmd(self, operation):  # noqa: C901
+    def cmd(self, operation: str):  # noqa: C901
         """ put a mapi command on the line"""
         logger.debug("executing command %s" % operation)
 
         if self.state != STATE_READY:
             raise ProgrammingError("Not connected")
 
         self._putblock(operation)
@@ -323,24 +329,59 @@
             if response.startswith("OK"):
                 return response[2:].strip() or ""
             else:
                 return response
         else:
             raise ProgrammingError("unknown state: %s" % response)
 
-    def _challenge_response(self, challenge: str, password: str):  # noqa: C901
+    def binary_cmd(self, operation: str) -> memoryview:
+        """ put a mapi command on the line, with a binary response.
+
+        returns a memoryview that can only be used until the next
+        operation on this Connection object.
+        """
+        logger.debug("executing binary command %s" % operation)
+
+        if self.state != STATE_READY:
+            raise ProgrammingError("Not connected")
+
+        self._putblock(operation)
+        buffer = self._get_buffer()
+        n = self._getblock_raw(buffer, 0)
+        view = memoryview(buffer)[:n]
+        self._stash_buffer(buffer)
+
+        # Handle !Error message
+        if view[0:len(MSG_ERROR_B)] == MSG_ERROR_B:
+            msg_bytes = bytes(view)
+            idx = msg_bytes.find(b'\n')
+            if idx > 0:
+                msg_bytes = msg_bytes[1:idx + 1]
+            exception, msg = handle_error(str(msg_bytes, 'utf-8'))
+            raise exception(msg)
+
+        return view
+
+    def _challenge_response(self, challenge: str, password: str, url_options: Dict[str, str]):  # noqa: C901
         """ generate a response to a mapi login challenge """
 
         challenges = challenge.split(':')
         if challenges[-1] != '' or len(challenges) < 7:
             raise OperationalError("Server sent invalid challenge")
         challenges.pop()
 
         salt, identity, protocol, hashes, endian = challenges[:5]
 
+        if endian == 'LIT':
+            self.server_endian = 'little'
+        elif endian == 'BIG':
+            self.server_endian = 'big'
+        else:
+            raise NotSupportedError('Unknown byte order: ' + endian)
+
         if protocol == '9':
             algo = challenges[5]
             try:
                 h = hashlib.new(algo)
                 h.update(password.encode())
                 password = h.hexdigest()
             except ValueError as e:
@@ -360,33 +401,43 @@
                 break
         else:
             raise NotSupportedError("Unsupported hash algorithms required"
                                     " for login: %s" % hashes)
 
         response = ":".join(["BIG", self.username, pwhash, self.language, self.database]) + ":"
 
+        self.binexport_level = 0
+        if len(challenges) >= 8:
+            part = challenges[7]
+            assert part.startswith('BINARY=')
+            self.binexport_level = int(part[7:])
+
+        handshake_options = self.handshake_options_callback(self.binexport_level)
+
         if len(challenges) >= 7:
             response += "FILETRANS:"
             options_level = 0
             for part in challenges[6].split(","):
                 if part.startswith("sql="):
                     try:
                         options_level = int(part[4:])
                     except ValueError:
                         raise OperationalError("invalid sql options level in server challenge: " + part)
             options = []
-            for opt in self.handshake_options:
+            for opt in handshake_options:
                 if opt.level < options_level:
                     options.append(opt.name + "=" + str(int(opt.value)))
                     opt.sent = True
             response += ",".join(options) + ":"
 
+        self.remaining_handshake_options = [opt for opt in handshake_options if not opt.sent]
+
         return response
 
-    def _getblock_and_transfer_files(self):
+    def _getblock_and_transfer_files(self) -> str:
         """ read one mapi encoded block and take care of any file transfers the server requests"""
         if self.language == 'control' and not self.hostname:
             # control connections do not use the blocking protocol and do not transfer files
             return self._recv_to_end()
 
         buffer = self._get_buffer()
         offset = 0
@@ -514,15 +565,18 @@
         pos = 0
         end = len(block)
         block = memoryview(block)
         while pos < end:
             data = block[pos:pos + 8192]
             nsent = self.socket.send(data)
             pos += nsent
-        self.socket.shutdown(socket.SHUT_WR)
+        try:
+            self.socket.shutdown(socket.SHUT_WR)
+        except OSError:
+            pass
 
     def __del__(self):
         if self.socket:
             self.socket.close()
 
     def set_reply_size(self, size):
         # type: (int) -> None
@@ -557,7 +611,18 @@
     """
     def __init__(self, level, name, fallback, value):
         self.level = level
         self.name = name
         self.value = value
         self.fallback = fallback
         self.sent = False
+
+
+def mapi_url_options(possible_mapi_url: str) -> Dict[str, str]:
+    """Try to parse the argument as a MAPI URL and return a Dict of url options
+
+    Return empty dict if it's not a MAPI URL.
+    """
+    if not possible_mapi_url.startswith('mapi:monetdb:'):
+        return {}
+    url = possible_mapi_url[5:]
+    return dict(parse_qsl(urlparse(url).query))
```

### Comparing `pymonetdb-1.6.4/pymonetdb/profiler.py` & `pymonetdb-1.7.0/pymonetdb/profiler.py`

 * *Files identical despite different names*

### Comparing `pymonetdb-1.6.4/pymonetdb/sql/cursors.py` & `pymonetdb-1.7.0/pymonetdb/sql/cursors.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 # License, v. 2.0.  If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 #
 # Copyright 1997 - July 2008 CWI, August 2008 - 2016 MonetDB B.V.
 
 import logging
 from collections import namedtuple
-from typing import Optional, Dict
+import struct
+from typing import List, Optional, Dict, Tuple
+from pymonetdb.policy import BatchPolicy
+import pymonetdb.sql.connections
 from pymonetdb.sql.debug import debug, export
-from pymonetdb.sql import monetize, pythonize
+from pymonetdb.sql import monetize, pythonize, pythonizebin
 from pymonetdb.exceptions import Error, ProgrammingError, InterfaceError
 from pymonetdb import mapi
 
 logger = logging.getLogger("pymonetdb")
 
 Description = namedtuple('Description', ('name', 'type_code', 'display_size', 'internal_size', 'precision', 'scale',
                                          'null_ok'))
@@ -21,25 +24,46 @@
 class Cursor(object):
     """This object represents a database cursor, which is used to manage
     the context of a fetch operation. Cursors created from the same
     connection are not isolated, i.e., any changes done to the
     database by a cursor are immediately visible by the other
     cursors"""
 
-    def __init__(self, connection):
+    connection: 'pymonetdb.sql.connections.Connection'
+    _policy: BatchPolicy
+    operation: str
+
+    arraysize: int
+    """Default value for the size parameter of :func:`~pymonetdb.sql.cursors.Cursor.fetchmany`. """
+
+    rowcount: int
+    description: Optional[Description]
+    _can_bindecode: Optional[bool]
+    _bindecoders: Optional[List['pythonizebin.BinaryDecoder']]
+    rownumber: int
+    _executed: Optional[str]
+    _offset: int
+    _rows: List[Tuple]
+    _resultsets_to_close: List[str]
+    _query_id: int
+    messages: List[str]
+    lastrowid: Optional[int]
+
+    def __init__(self, connection: 'pymonetdb.sql.connections.Connection'):
         """This read-only attribute return a reference to the Connection
         object on which the cursor was created."""
         self.connection = connection
+        self._policy = connection._policy.clone()
 
         # last executed operation (query)
         self.operation = ""
 
         # This read/write attribute specifies the number of rows to
         # fetch at a time with .fetchmany()
-        self.arraysize = connection.replysize
+        self.arraysize = self._policy.decide_arraysize()
 
         # This read-only attribute specifies the number of rows that
         # the last .execute*() produced (for DQL statements like
         # 'select') or affected (for DML statements like 'update' or
         # 'insert').
         #
         # The attribute is -1 in case no .execute*() has been
@@ -62,14 +86,21 @@
         #    null_ok)
         #
         # This attribute will be None for operations that
         # do not return rows or if the cursor has not had an
         # operation invoked via the .execute*() method yet.
         self.description = None
 
+        # When the opportunity presents itself to fetch a result set in binary
+        # we need to know if we can handle the result and if so, how.
+        #
+        # These attributes are cleared by execute() and set by _nextchunk()
+        self._can_bindecode = None
+        self._bindecoders = None
+
         # This read-only attribute indicates at which row
         # we currently are
         self.rownumber = -1
 
         self._executed = None
 
         # the offset of the current resultset in the total resultset
@@ -107,14 +138,22 @@
         # attribute should be set to None.
         #
         # The semantics of .lastrowid are undefined in case the last
         # executed statement modified more than one row, e.g. when
         # using INSERT with .executemany().
         self.lastrowid = None
 
+        # This is used to unpack binary result sets
+        server_endian = self.connection.mapi.server_endian
+        if server_endian == 'little':
+            unpacker = '<q'
+        elif server_endian == 'big':
+            unpacker = '>q'
+        self._unpack_int64 = unpacker
+
     def _check_executed(self):
         if not self._executed:
             self._exception_handler(ProgrammingError, "do a execute() first")
 
     def _close_earlier_resultsets(self):
         for rs in self._resultsets_to_close:
             command = 'Xclose %s' % rs
@@ -129,31 +168,49 @@
 
         try:
             self._close_earlier_resultsets()
         except Error:
             pass
         self.connection = None
 
+    def __enter__(self):
+        """This method is invoked when this Cursor is used in a with-statement.
+        """
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        """This method is invoked when this Cursor is used in a with-statement.
+        """
+        try:
+            self.close()
+        except Error:
+            pass
+        # Propagate any errors
+        return False
+
     def execute(self, operation: str, parameters: Optional[Dict] = None):
         """Prepare and execute a database operation (query or
         command).  Parameters may be provided as mapping and
         will be bound to variables in the operation.
         """
 
         if not self.connection:
             self._exception_handler(ProgrammingError, "cursor is closed")
 
         # clear message history
         self.messages = []
 
         self._close_earlier_resultsets()
+        self._can_bindecode = None
+        self._bindecoders = None
 
         # set the number of rows to fetch
-        if self.arraysize != self.connection.replysize:
-            self.connection.set_replysize(self.arraysize)
+        desired_replysize = self._policy.new_query()
+        if self.connection._current_replysize != desired_replysize:
+            self.connection._change_replysize(desired_replysize)
 
         if operation == self.operation:
             # same operation, DBAPI mentioned something about reuse
             # but monetdb doesn't support this
             pass
         else:
             self.operation = operation
@@ -173,15 +230,15 @@
         else:
             query = operation
 
         block = self.connection.execute(query)
         self._store_result(block)
         self.rownumber = 0
         self._executed = operation
-        return self.rowcount
+        return self.rowcount if self.rowcount >= 0 else None
 
     def executemany(self, operation, seq_of_parameters):
         """Prepare a database operation (query or command) and then
         execute it against all parameter sequences or mappings
         found in the sequence seq_of_parameters.
 
         It will return the number or rows affected
@@ -204,107 +261,107 @@
         return export(self, query, fname, sample, filespath)
 
     def fetchone(self):
         """Fetch the next row of a query result set, returning a
         single sequence, or None when no more data is available."""
 
         self._check_executed()
-
         if self._query_id == -1:
             msg = "query didn't result in a resultset"
             self._exception_handler(ProgrammingError, msg)
 
-        if self.rownumber >= self.rowcount:
-            return None
-
-        if self.rownumber >= (self._offset + len(self._rows)):
-            self._nextchunk()
+        cache_end = self._offset + len(self._rows)
+        if self.rownumber >= cache_end:
+            if self.rownumber >= self.rowcount:
+                return None
+            self._populate_cache(0, self.rownumber + 1)
 
         result = self._rows[self.rownumber - self._offset]
         self.rownumber += 1
         return result
 
     def fetchmany(self, size=None):
         """Fetch the next set of rows of a query result, returning a
         sequence of sequences (e.g. a list of tuples). An empty
         sequence is returned when no more rows are available.
 
         The number of rows to fetch per call is specified by the
         parameter.  If it is not given, the cursor's arraysize
-        determines the number of rows to be fetched. The method
-        should try to fetch as many rows as indicated by the size
-        parameter. If this is not possible due to the specified
-        number of rows not being available, fewer rows may be
-        returned.
+        determines the number of rows to be fetched.
 
-        An Error (or subclass) exception is raised if the previous
-        call to .execute*() did not produce any result set or no
-        call was issued yet.
-
-        Note there are performance considerations involved with
-        the size parameter.  For optimal performance, it is
-        usually best to use the arraysize attribute.  If the size
-        parameter is used, then it is best for it to retain the
-        same value from one .fetchmany() call to the next."""
-
-        self._check_executed()
-
-        if self.rownumber >= self.rowcount:
-            return []
-
-        end = min(self.rownumber + (size or self.arraysize), self.rowcount)
-        result = self._rows[self.rownumber - self._offset:end - self._offset]
-        self.rownumber = min(end, len(self._rows) + self._offset)
-
-        while (end > self.rownumber) and self._nextchunk():
-            result += self._rows[self.rownumber - self._offset:end - self._offset]
-            self.rownumber = min(end, len(self._rows) + self._offset)
-        return result
-
-    def fetchall(self):
-        """Fetch all (remaining) rows of a query result, returning
-        them as a sequence of sequences (e.g. a list of tuples).
-        Note that the cursor's arraysize attribute can affect the
-        performance of this operation.
-
-        An Error (or subclass) exception is raised if the previous
+        A :class:`~pymonetdb.ProgrammingError` is raised if the previous
         call to .execute*() did not produce any result set or no
         call was issued yet."""
 
         self._check_executed()
-
         if self._query_id == -1:
             msg = "query didn't result in a resultset"
             self._exception_handler(ProgrammingError, msg)
 
-        result = self._rows[self.rownumber - self._offset:]
-        self.rownumber = len(self._rows) + self._offset
+        if size is None:
+            size = self.arraysize
 
-        # slide the window over the resultset
-        while self._nextchunk():
-            result += self._rows
-            self.rownumber = len(self._rows) + self._offset
+        cache_end = self._offset + len(self._rows)
+        requested_end = min(self.rownumber + size, self.rowcount)
 
-        return result
+        if requested_end <= cache_end:
+            result = self._rows[self.rownumber - self._offset:requested_end - self._offset]
+            self.rownumber = requested_end
+        else:
+            result = self._rows[self.rownumber - self._offset:cache_end - self._offset]
+            self.rownumber = cache_end
+            self._populate_cache(len(result), requested_end)
+            result += self._rows[self.rownumber - self._offset:requested_end - self._offset]
+            self.rownumber = requested_end
 
-    def _nextchunk(self):
-        self._check_executed()
+        return result
 
-        if self.rownumber >= self.rowcount:
-            return False
+    def fetchall(self):
+        """Fetch all remaining rows of a query result, returning
+        them as a sequence of sequences (e.g. a list of tuples).
 
-        self._offset += len(self._rows)
+        A :class:`~pymonetdb.ProgrammingError` is raised if the previous
+        call to .execute*() did not produce any result set or no
+        call was issued yet."""
 
-        end = min(self.rowcount, self.rownumber + self.arraysize)
-        amount = end - self._offset
+        return self.fetchmany(self.rowcount)
 
-        command = 'Xexport %s %s %s' % (self._query_id, self._offset, amount)
-        block = self.connection.command(command)
-        self._store_result(block)
-        return True
+    def _populate_cache(self, already_used, requested_end):
+        del self._rows[:]
+        self._offset = self.rownumber
+
+        rows_to_fetch = self._policy.batch_size(
+            already_used,
+            self.rownumber, requested_end,
+            self.rowcount)
+
+        if self._can_bindecode is None:
+            self._check_bindecode_possible()
+        if self._can_bindecode:
+            command = 'Xexportbin %s %s %s' % (self._query_id, self.rownumber, rows_to_fetch)
+            binary_block = self.connection.binary_command(command)
+            self._store_binary_result(binary_block)
+        else:
+            command = 'Xexport %s %s %s' % (self._query_id, self.rownumber, rows_to_fetch)
+            block = self.connection.command(command)
+            self._store_result(block)
+
+    def _check_bindecode_possible(self):
+        self._can_bindecode = False
+        decoders = []
+        if not self.connection._policy.use_binary():
+            return
+        for i in range(len(self.description)):
+            dec = pythonizebin.get_decoder(self, i)
+            if not dec:
+                return
+            decoders.append(dec)
+        # if we get here, all columns have a decoder
+        self._can_bindecode = True
+        self._bindecoders = decoders
 
     def setinputsizes(self, sizes):
         """
         This method would be used before the .execute*() method
         is invoked to reserve memory. This implementation doesn't
         use this.
         """
@@ -337,47 +394,26 @@
 
         columns = 0
         column_name = ""
         scale = display_size = internal_size = precision = 0
         null_ok = False
         type_ = []
 
-        for line in block.split("\n"):
-            if line.startswith(mapi.MSG_INFO):
-                logger.info(line[1:])
-                self.messages.append((Warning, line[1:]))
-
-            elif line.startswith(mapi.MSG_QTABLE) or line.startswith(mapi.MSG_QPREPARE):
-                self._query_id, rowcount, columns, tuples = line[2:].split()[:4]
-
-                columns = int(columns)  # number of columns in result
-                self.rowcount = int(rowcount)  # total number of rows
-                tuples = int(tuples)     # number of rows in this set
-                if tuples < self.rowcount:
-                    self._resultsets_to_close.append(self._query_id)
-                self._rows = []
+        msg_tuple = mapi.MSG_TUPLE
+        assert len(msg_tuple) == 1
+        msg_header = mapi.MSG_HEADER
+        assert len(msg_header) == 1
 
-                # set up fields for description
-                # table_name = [None] * columns
-                column_name = [None] * columns
-                type_ = [None] * columns
-                display_size = [None] * columns
-                internal_size = [None] * columns
-                precision = [None] * columns
-                scale = [None] * columns
-                null_ok = [None] * columns
-                # typesizes = [(0, 0)] * columns
+        for line in block.split("\n"):
+            first = line[:1]
 
-                self._offset = 0
-                if line.startswith(mapi.MSG_QPREPARE):
-                    self.lastrowid = int(self._query_id)
-                else:
-                    self.lastrowid = None
+            if first == msg_tuple:
+                self._rows.append(self._parse_tuple(line))
 
-            elif line.startswith(mapi.MSG_HEADER):
+            elif first == msg_header:
                 (data, identity) = line[1:].split("#")
                 values = [x.strip() for x in data.split(",")]
                 identity = identity.strip()
 
                 if identity == "name":
                     column_name = values
                 elif identity == "table_name":
@@ -401,17 +437,44 @@
                 description = []
                 for i in range(columns):
                     description.append(Description(column_name[i], type_[i], display_size[i], internal_size[i],
                                                    precision[i], scale[i], null_ok[i]))
                 self.description = description
                 self._offset = 0
 
-            elif line.startswith(mapi.MSG_TUPLE):
-                values = self._parse_tuple(line)
-                self._rows.append(values)
+            elif line.startswith(mapi.MSG_INFO):
+                logger.info(line[1:])
+                self.messages.append((Warning, line[1:]))
+
+            elif line.startswith(mapi.MSG_QTABLE) or line.startswith(mapi.MSG_QPREPARE):
+                self._query_id, rowcount, columns, tuples = line[2:].split()[:4]
+
+                columns = int(columns)  # number of columns in result
+                self.rowcount = int(rowcount)  # total number of rows
+                tuples = int(tuples)     # number of rows in this set
+                if tuples < self.rowcount:
+                    self._resultsets_to_close.append(self._query_id)
+                self._rows = []
+
+                # set up fields for description
+                # table_name = [None] * columns
+                column_name = [None] * columns
+                type_ = [None] * columns
+                display_size = [None] * columns
+                internal_size = [None] * columns
+                precision = [None] * columns
+                scale = [None] * columns
+                null_ok = [None] * columns
+                # typesizes = [(0, 0)] * columns
+
+                self._offset = 0
+                if line.startswith(mapi.MSG_QPREPARE):
+                    self.lastrowid = int(self._query_id)
+                else:
+                    self.lastrowid = None
 
             elif line.startswith(mapi.MSG_TUPLE_NOSLICE):
                 self._rows.append((line[1:],))
 
             elif line.startswith(mapi.MSG_QBLOCK):
                 self._rows = []
 
@@ -442,14 +505,47 @@
                 return
 
             elif line.startswith(mapi.MSG_ERROR):
                 self._exception_handler(ProgrammingError, line[1:])
 
         self._exception_handler(InterfaceError, "Unknown state, %s" % block)
 
+    def _store_binary_result(self, block: memoryview):
+        assert self._bindecoders is not None
+        if len(block) < 8:
+            self._exception_handler(InterfaceError, "binary response too short")
+
+        toc_pos = struct.unpack_from(self._unpack_int64, block, len(block) - 8)[0]
+        if toc_pos < 0:
+            # It actually points to the error message.
+            # The message ends at the first \x00.
+            bmsg = bytes(block[toc_pos:-8])
+            bmsg = bmsg.split(b'\x00', 1)[0]
+            try:
+                msg = str(bmsg, 'utf-8')
+            except UnicodeDecodeError:
+                self._exception_handler(InterfaceError, "invalid utf-8 in error message")
+            self._exception_handler(ProgrammingError, msg)
+
+        # if we get here toc_pos actually points to the toc.
+        ncols = len(self._bindecoders)
+        cols = []
+        for i in range(ncols):
+            # TODO fix endianness
+            start_pos = toc_pos + 16 * i
+            length_pos = start_pos + 8
+            start = struct.unpack_from(self._unpack_int64, block, start_pos)[0]
+            length = struct.unpack_from(self._unpack_int64, block, length_pos)[0]
+            slice = block[start:start + length]
+            decoder = self._bindecoders[i]
+            col = decoder.decode(self.connection.mapi.server_endian, slice)
+            cols.append(col)
+        rows = list(zip(*cols))
+        self._rows = rows
+
     def _parse_tuple(self, line):
         """
         parses a mapi data tuple, and returns a list of python types
         """
         elements = line[1:-1].split(',\t')
         if len(elements) == len(self.description):
             return tuple([pythonize.convert(element.strip(), description[1])
@@ -475,24 +571,62 @@
         if mode not in ['relative', 'absolute']:
             msg = "unknown mode '%s'" % mode
             self._exception_handler(ProgrammingError, msg)
 
         if mode == 'relative':
             value += self.rownumber
 
+        if self._offset <= value < self._offset + len(self._rows):
+            self.rownumber = value
+            return
+
         if value > self.rowcount:
             self._exception_handler(IndexError, "value beyond length of resultset")
 
+        self.rownumber = value
         self._offset = value
-        end = min(self.rowcount, self.rownumber + self.arraysize)
-        amount = end - self._offset
-        command = 'Xexport %s %s %s' % (self._query_id, self._offset, amount)
-        block = self.connection.command(command)
-        self._store_result(block)
+        self._rows = []
+        self._policy.scroll()
 
     def _exception_handler(self, exception_class, message):
         """
         raises the exception specified by exception, and add the error
         to the message list
         """
         self.messages.append((exception_class, message))
         raise exception_class(message)
+
+    def get_replysize(self) -> int:
+        return self._policy.replysize
+
+    def set_replysize(self, replysize: int):
+        self._policy.replysize = replysize
+
+    replysize = property(get_replysize, set_replysize)
+
+    def get_maxprefetch(self) -> int:
+        return self._policy.maxprefetch
+
+    def set_maxprefetch(self, maxprefetch: int):
+        self._policy.maxprefetch = maxprefetch
+
+    maxprefetch = property(get_maxprefetch, set_maxprefetch)
+
+    def get_binary(self) -> int:
+        return self._policy.binary_level
+
+    def set_binary(self, level: int):
+        self._policy.binary_level = level
+
+    binary = property(get_binary, set_binary)
+
+    def used_binary_protocol(self) -> bool:
+        """Pymonetdb-specific. Return True if the last fetch{one,many,all}
+        for the current statement made use of the binary protocol.
+
+        Primarily used for testing.
+
+        Note that the binary protocol is never used for the first few rows
+        of a result set. Exactly when it kicks in depends on the
+        `replysize` setting.
+        """
+        return self._can_bindecode is True  # True as opposed to False or None
```

### Comparing `pymonetdb-1.6.4/pymonetdb/sql/debug.py` & `pymonetdb-1.7.0/pymonetdb/sql/debug.py`

 * *Files identical despite different names*

### Comparing `pymonetdb-1.6.4/pymonetdb/sql/monetize.py` & `pymonetdb-1.7.0/pymonetdb/sql/monetize.py`

 * *Files identical despite different names*

### Comparing `pymonetdb-1.6.4/pymonetdb/sql/pythonize.py` & `pymonetdb-1.7.0/pymonetdb/sql/pythonize.py`

 * *Files 22% similar despite different names*

```diff
@@ -70,23 +70,35 @@
     t, timezone_delta = _extract_timezone(data)
     return py_time(t).replace(tzinfo=timezone_delta)
 
 
 def py_date(data):
     """ Returns a python Date
     """
-    year, month, day = data.split('-', 3)
+    try:
+        year, month, day = data.split('-', 3)
+    except ValueError:
+        if data.startswith('-'):
+            raise ValueError("year out of range, must be positive")
+        else:
+            raise
     return datetime.date(int(year), int(month), int(day))
 
 
 def py_timestamp(data):
     """ Returns a python Timestamp
     """
     date_part, time_part = data.split(' ', 2)
-    year, month, day = date_part.split('-', 3)
+    try:
+        year, month, day = date_part.split('-', 3)
+    except ValueError:
+        if date_part.startswith('-'):
+            raise ValueError("year out of range, must be positive")
+        else:
+            raise
     hour, min, sec_usec = time_part.split(':', 3)
     sec_parts = sec_usec.split('.', 2)
     sec = sec_parts[0]
     if len(sec_parts) == 2:
         usec = int((sec_parts[1] + '000000')[:6])
     else:
         usec = 0
@@ -100,22 +112,28 @@
     return py_timestamp(dt).replace(tzinfo=timezone_delta)
 
 
 def py_sec_interval(data: str) -> timedelta:
     """ Returns a python TimeDelta where data represents a value of MonetDB's INTERVAL SECOND type
     which resembles a stringified decimal.
     """
-    return timedelta(seconds=int(Decimal(data)))
+    # It comes in as a decimal but we use Pythons float parser to parse it.
+    # That's ok because the precision of the decimal is only three decimal digits
+    # so far coarser than the rounding errors introduced by the float.
+    return timedelta(seconds=float(data))
 
 
 def py_day_interval(data: str) -> int:
     """ Returns a python number of days where data represents a value of MonetDB's INTERVAL DAY type
     which resembles a stringified decimal.
     """
-    return timedelta(seconds=int(Decimal(data))).days
+    # It comes in as a decimal but we use Pythons float parser to parse it.
+    # That's ok because the precision of the decimal is only three decimal digits
+    # so far coarser than the rounding errors introduced by the float.
+    return timedelta(seconds=float(data)).days
 
 
 def py_bytes(data: str):
     """Returns a bytes (py3) or string (py2) object representing the input blob."""
     return bytes.fromhex(data)
```

### Comparing `pymonetdb-1.6.4/pymonetdb/sql/types.py` & `pymonetdb-1.7.0/pymonetdb/sql/types.py`

 * *Files identical despite different names*

### Comparing `pymonetdb-1.6.4/pymonetdb.egg-info/PKG-INFO` & `pymonetdb-1.7.0/pymonetdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonetdb
-Version: 1.6.4
+Version: 1.7.0
 Summary: Native MonetDB client Python API
 Home-page: http://www.monetdb.org/
 Download-URL: https://github.com/MonetDB/pymonetdb
 Author: MonetDB BV
 Author-email: info@monetdb.org
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Database Engines/Servers
@@ -12,14 +12,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Provides-Extra: test
 Provides-Extra: doc
 License-File: LICENSE
 
 .. This Source Code Form is subject to the terms of the Mozilla Public
 .. License, v. 2.0.  If a copy of the MPL was not distributed with this
```

### Comparing `pymonetdb-1.6.4/pymonetdb.egg-info/SOURCES.txt` & `pymonetdb-1.7.0/pymonetdb.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-CHANGES
 LICENSE
 MANIFEST.in
 README.rst
-p.py
 setup.cfg
 setup.py
 t.py
-tt.py
-ttt.py
 pymonetdb/__init__.py
 pymonetdb/control.py
 pymonetdb/exceptions.py
 pymonetdb/mapi.py
+pymonetdb/policy.py
 pymonetdb/profiler.py
 pymonetdb.egg-info/PKG-INFO
 pymonetdb.egg-info/SOURCES.txt
 pymonetdb.egg-info/dependency_links.txt
 pymonetdb.egg-info/requires.txt
 pymonetdb.egg-info/top_level.txt
 pymonetdb/filetransfer/__init__.py
@@ -24,29 +21,34 @@
 pymonetdb/filetransfer/uploads.py
 pymonetdb/sql/__init__.py
 pymonetdb/sql/connections.py
 pymonetdb/sql/cursors.py
 pymonetdb/sql/debug.py
 pymonetdb/sql/monetize.py
 pymonetdb/sql/pythonize.py
+pymonetdb/sql/pythonizebin.py
 pymonetdb/sql/types.py
 tests/__init__.py
 tests/install_monetdb_from_msi_dir.py
 tests/test_capabilities.py
+tests/test_contextmanager.py
 tests/test_control.py
 tests/test_dbapi2.py
 tests/test_exceptions.py
+tests/test_execute.py
 tests/test_filetransfer.py
 tests/test_mapi.py
 tests/test_mapi_uri.py
 tests/test_monetize.py
 tests/test_multiline.py
 tests/test_namedtuple.py
 tests/test_oid.py
+tests/test_policy.py
 tests/test_prepare.py
 tests/test_profiler.py
 tests/test_pythonize.py
+tests/test_resultset.py
 tests/test_temporal.py
 tests/test_udf.py
 tests/test_unicode.py
 tests/util.py
 tests/windows_tests.py
```

### Comparing `pymonetdb-1.6.4/setup.py` & `pymonetdb-1.7.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 }
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
-__version__ = '1.6.4'
+__version__ = '1.7.0'
 
 setup(
     name='pymonetdb',
     version=__version__,
     description='Native MonetDB client Python API',
     long_description=read('README.rst'),
     author='MonetDB BV',
@@ -41,13 +41,14 @@
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
     tests_require=tests_require,
     test_suite="tests",
     extras_require=extras_require,
 )
```

### Comparing `pymonetdb-1.6.4/tests/install_monetdb_from_msi_dir.py` & `pymonetdb-1.7.0/tests/install_monetdb_from_msi_dir.py`

 * *Files identical despite different names*

### Comparing `pymonetdb-1.6.4/tests/test_capabilities.py` & `pymonetdb-1.7.0/tests/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `pymonetdb-1.6.4/tests/test_control.py` & `pymonetdb-1.7.0/tests/test_control.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,19 +3,22 @@
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 #
 # Copyright 1997 - July 2008 CWI, August 2008 - 2016 MonetDB B.V.
 
 import unittest
 from pymonetdb.control import Control
 from pymonetdb.exceptions import OperationalError
-from tests.util import test_hostname, test_port, test_passphrase, test_full, test_control
+from tests.util import test_hostname, test_port, test_passphrase, test_control
 
 database_prefix = 'controltest_'
 database_name = database_prefix + 'other'
 
+test_control_tcp = 'tcp' in test_control.split(',')
+test_control_local = 'local' in test_control.split(',')
+
 
 def do_without_fail(function):
     try:
         function()
     except OperationalError:
         pass
 
@@ -28,89 +31,88 @@
     $ monetdbd set passphrase=testdb /var/lib/monetdb
 
     Where /var/lib/monetdb is the path to your dbfarm. Don't forget to restart the db after setting the credentials.
     """
 
     def setUpControl(self):
         # use tcp
-        if 'tcp' not in (test_control or '').split(','):
+        if not test_control_tcp:
             raise unittest.SkipTest("Skipping 'tcp' Control test")
         return Control(hostname=test_hostname, port=test_port, passphrase=test_passphrase)
 
     def setUp(self):
         self.control = self.setUpControl()
-
-        do_without_fail(lambda: self.control.stop(database_name))
-        do_without_fail(lambda: self.control.destroy(database_name))
+        self.ensure_destroyed(database_name)
         self.control.create(database_name)
 
-    def _cleanup(self, old, new):
-        do_without_fail(lambda: self.control.destroy(old))
-        do_without_fail(lambda: self.control.destroy(new))
-        self.control.create(old)
-        self.control.rename(old, new)
-        statuses = self.control.status()
-        self.assertTrue(new in [status["name"] for status in statuses])
-        do_without_fail(lambda: self.control.destroy(new))
-        return statuses
+    def tearDown(self):
+        self.ensure_destroyed(database_name)
 
-    def tear_down(self):
+    def ensure_destroyed(self, database_name):
         do_without_fail(lambda: self.control.stop(database_name))
         do_without_fail(lambda: self.control.destroy(database_name))
 
     def test_create(self):
         create_name = database_prefix + "create"
-        do_without_fail(lambda: self.control.destroy(create_name))
+        self.ensure_destroyed(create_name)
         self.control.create(create_name)
         self.assertRaises(OperationalError, self.control.create, create_name)
-        do_without_fail(lambda: self.control.destroy(create_name))
+        self.ensure_destroyed(create_name)
 
     def test_destroy(self):
         destroy_name = database_prefix + "destroy"
+        self.ensure_destroyed(destroy_name)
         self.control.create(destroy_name)
         self.control.destroy(destroy_name)
         self.assertRaises(OperationalError, self.control.destroy, destroy_name)
 
     def test_lock(self):
         do_without_fail(lambda: self.control.release(database_name))
+        self.assertEqual(self.control.status(database_name)['locked'], False)
         self.control.lock(database_name)
+        self.assertEqual(self.control.status(database_name)['locked'], True)
         with self.assertRaises(OperationalError):
             self.control.lock(database_name)
         self.control.release(database_name)
+        self.assertEqual(self.control.status(database_name)['locked'], False)
 
     def test_release(self):
         do_without_fail(lambda: self.control.release(database_name))
+        self.assertEqual(self.control.status(database_name)['locked'], False)
         do_without_fail(lambda: self.control.lock(database_name))
+        self.assertEqual(self.control.status(database_name)['locked'], True)
         self.assertTrue(self.control.release(database_name))
+        self.assertEqual(self.control.status(database_name)['locked'], False)
         self.assertRaises(OperationalError, self.control.release, database_name)
 
-    @unittest.skipUnless(test_full, "full test disabled")
     def test_status(self):
         status = self.control.status(database_name)
         self.assertEqual(status["name"], database_name)
 
-    @unittest.skipUnless(test_full, "full test disabled")
     def test_statuses(self):
         status1 = database_prefix + "status1"
         status2 = database_prefix + "status2"
-        statuses = self._cleanup(status1, status2)
+        self.ensure_destroyed(status1)
+        self.ensure_destroyed(status2)
+        self.control.create(status1)
+        self.control.rename(status1, status2)
+        statuses = self.control.status()
+        self.assertFalse(status1 in [status["name"] for status in statuses])
         self.assertTrue(status2 in [status["name"] for status in statuses])
-        do_without_fail(lambda: self.control.destroy(status1))
+        self.assertRaises(OperationalError, self.control.destroy, status1)
         do_without_fail(lambda: self.control.destroy(status2))
 
     def test_start(self):
         do_without_fail(lambda: self.control.stop(database_name))
         self.assertTrue(self.control.start(database_name))
 
-    @unittest.skipUnless(test_full, "full test disabled")
     def test_stop(self):
-        do_without_fail(lambda: self.control.start(database_name))
-        self.assertTrue(self.control.stop(database_name))
+        self.ensure_destroyed(database_name)
+        self.assertNotIn(database_name, [st['name'] for st in self.control.status()])
 
-    @unittest.skipUnless(test_full, "full test disabled")
     def test_kill(self):
         do_without_fail(lambda: self.control.start(database_name))
         self.assertTrue(self.control.kill(database_name))
 
     def test_set(self):
         property_ = "readonly"
         value = "yes"
@@ -127,25 +129,31 @@
         self.control.inherit(database_name, "readonly")
         # TODO: False on OSX, True on travis?
         # self.assertTrue("readonly" in self.control.get(database_name))
 
     def test_rename(self):
         old = database_prefix + "old"
         new = database_prefix + "new"
-        self._cleanup(old, new)
-        do_without_fail(lambda: self.control.destroy(new))
+        self.ensure_destroyed(old)
+        self.ensure_destroyed(new)
+        self.control.create(old)
+        self.control.rename(old, new)
+        names = [st['name'] for st in self.control.status()]
+        self.assertIn(new, names)
+        self.assertNotIn(old, names)
+        self.ensure_destroyed(new)
+        self.assertRaises(OperationalError, self.control.destroy, old)
 
     def test_defaults(self):
         defaults = self.control.defaults()
         self.assertTrue("readonly" in defaults)
 
-    @unittest.skipUnless(test_full, "full test disabled")
     def test_neighbours(self):
         self.control.neighbours()
 
 
 class TestLocalControl(TestControl):
     def setUpControl(self):
         # use unix domain socket
-        if 'local' not in (test_control or '').split(','):
+        if not test_control_local:
             raise unittest.SkipTest("Skipping 'local' Control test")
         return Control(port=test_port, passphrase=test_passphrase)
```

### Comparing `pymonetdb-1.6.4/tests/test_dbapi2.py` & `pymonetdb-1.7.0/tests/test_dbapi2.py`

 * *Files identical despite different names*

### Comparing `pymonetdb-1.6.4/tests/test_exceptions.py` & `pymonetdb-1.7.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pymonetdb-1.6.4/tests/test_filetransfer.py` & `pymonetdb-1.7.0/tests/test_filetransfer.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 from pymonetdb import connect, Error as MonetError
 from pymonetdb.exceptions import OperationalError, ProgrammingError
 from pymonetdb import Download, Downloader, Upload, Uploader
 from pymonetdb.filetransfer.directoryhandler import SafeDirectoryHandler, lookup_compression_algorithm
 from pymonetdb.filetransfer.uploads import NormalizeCrLf
-from tests.util import have_lz4, test_args, test_full
+from tests.util import test_have_lz4, test_args, test_full
 
 
 class MyException(Exception):
     pass
 
 
 class MyUploader(Uploader):
@@ -674,15 +674,15 @@
     def test_download_encodings_and_line_endings(self):
         compressions = [
             None,
             'gz',
             'bz2',
             'xz',
         ]
-        if have_lz4:
+        if test_have_lz4:
             compressions.append('lz4')
         encodings = [
             'utf-8',
             'latin1',
             'shift-jis',
             None  # means native
         ]
```

### Comparing `pymonetdb-1.6.4/tests/test_mapi.py` & `pymonetdb-1.7.0/tests/test_mapi.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from unittest import TestCase
-from tests.util import test_args
+from tests.util import test_mapi_args
 from pymonetdb.mapi import Connection
 
 
 class TestMapi(TestCase):
     @classmethod
     def setUpClass(cls):
         cls.conn = Connection()
-        cls.conn.connect(language='sql', **test_args)
+        cls.conn.connect(language='sql', **test_mapi_args)
 
     def test_set_size(self):
         query = 'sselect * from tables t1, tables t2;'
         for size in (2, 10):
             self.conn.set_reply_size(size)
             data = self.conn.cmd(query)
             cleaned = [i for i in data.split('\n') if i and not i[0] in '%&']
```

### Comparing `pymonetdb-1.6.4/tests/test_mapi_uri.py` & `pymonetdb-1.7.0/tests/test_mapi_uri.py`

 * *Files identical despite different names*

### Comparing `pymonetdb-1.6.4/tests/test_monetize.py` & `pymonetdb-1.7.0/tests/test_monetize.py`

 * *Files identical despite different names*

### Comparing `pymonetdb-1.6.4/tests/test_multiline.py` & `pymonetdb-1.7.0/tests/test_multiline.py`

 * *Files identical despite different names*

### Comparing `pymonetdb-1.6.4/tests/test_namedtuple.py` & `pymonetdb-1.7.0/tests/test_namedtuple.py`

 * *Files identical despite different names*

### Comparing `pymonetdb-1.6.4/tests/test_prepare.py` & `pymonetdb-1.7.0/tests/test_prepare.py`

 * *Files identical despite different names*

### Comparing `pymonetdb-1.6.4/tests/test_profiler.py` & `pymonetdb-1.7.0/tests/test_profiler.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     """Test the profiler connection."""
 
     conn: Optional[ProfilerConnection] = None
 
     @classmethod
     def setUpClass(cls):
         cls.conn = ProfilerConnection()
-        cls.conn.connect(**util.test_args)
+        cls.conn.connect(**util.test_mapi_args)
 
     @classmethod
     def tearDownClass(cls) -> None:
         if cls.conn:
             cls.conn.close()
 
     @patch('pymonetdb.mapi.Connection._getblock')
```

### Comparing `pymonetdb-1.6.4/tests/test_pythonize.py` & `pymonetdb-1.7.0/tests/test_pythonize.py`

 * *Files 15% similar despite different names*

```diff
@@ -63,14 +63,30 @@
 
         self.cursor.execute('SELECT %s, %s', [dt, dtz])
         row = self.cursor.fetchone()
 
         self.assertEqual(row[0].isoformat(), dt.isoformat())
         self.assertEqual(row[1].isoformat(), dtz.isoformat())
 
+    def test_date_year0(self):
+        with self.assertRaisesRegex(ValueError, "out of range"):
+            self.cursor.execute("SELECT DATE '0-1-1'")
+
+    def test_date_negative_year(self):
+        with self.assertRaisesRegex(ValueError, "out of range"):
+            self.cursor.execute("SELECT DATE '-1-1-1'")
+
+    def test_timestamp_year0(self):
+        with self.assertRaisesRegex(ValueError, "out of range"):
+            self.cursor.execute("SELECT TIMESTAMP '0-1-1 11:12:13'")
+
+    def test_timestamp_negative_year(self):
+        with self.assertRaisesRegex(ValueError, "out of range"):
+            self.cursor.execute("SELECT TIMESTAMP '-1-1-1 11:12:13'")
+
     def test_roundtrip_binary(self):
         raw = b'BLUB\x00BLOB'
         wrapped = pymonetdb.Binary(raw)
         self.cursor.execute('SELECT %s, %s', [raw, wrapped])
         row = self.cursor.fetchone()
 
         self.assertEqual(row[0], raw)
```

### Comparing `pymonetdb-1.6.4/tests/test_temporal.py` & `pymonetdb-1.7.0/tests/test_temporal.py`

 * *Files identical despite different names*

### Comparing `pymonetdb-1.6.4/tests/test_udf.py` & `pymonetdb-1.7.0/tests/test_udf.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                 return i * 2;
             };
             """)
         # test if Python UDFs are enabled on the server
         try:
             self.cursor.execute('SELECT test_python_udf(1);')
         except pymonetdb.exceptions.OperationalError:
-            raise SkipTest("We cant assume MonetDB is compiled with embbed python support enabled")
+            raise SkipTest("Don't know if MonetDB has with embedded Python support enabled")
 
         else:
             result = self.cursor.fetchall()
             self.assertEqual(result, [(2,)])
             # test python debugging capabilities
             with tempfile.NamedTemporaryFile(delete=False) as f:
                 fname = f.name
```

### Comparing `pymonetdb-1.6.4/tests/test_unicode.py` & `pymonetdb-1.7.0/tests/test_unicode.py`

 * *Files identical despite different names*

### Comparing `pymonetdb-1.6.4/tests/windows_tests.py` & `pymonetdb-1.7.0/tests/windows_tests.py`

 * *Files identical despite different names*

