# Comparing `tmp/linki-0.0.6.tar.gz` & `tmp/linki-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linki-0.0.6.tar", last modified: Tue Jun 20 01:33:17 2023, max compression
+gzip compressed data, was "linki-0.0.7.tar", last modified: Tue Jun 20 02:14:16 2023, max compression
```

## Comparing `linki-0.0.6.tar` & `linki-0.0.7.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 01:33:17.497367 linki-0.0.6/
--rw-r--r--   0 zone      (1000) zone      (1001)    34888 2023-06-20 01:08:26.000000 linki-0.0.6/LICENSE
--rw-r--r--   0 zone      (1000) zone      (1001)    10828 2023-06-20 01:33:17.497367 linki-0.0.6/PKG-INFO
--rw-r--r--   0 zone      (1000) zone      (1001)    10288 2023-06-19 07:55:18.000000 linki-0.0.6/README.md
-drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 01:33:17.487367 linki-0.0.6/linki/
--rw-r--r--   0 zone      (1000) zone      (1001)        0 2023-04-16 23:56:36.000000 linki-0.0.6/linki/__init__.py
--rw-r--r--   0 zone      (1000) zone      (1001)     1971 2023-04-24 04:57:19.000000 linki-0.0.6/linki/article.py
--rw-r--r--   0 zone      (1000) zone      (1001)     1773 2023-04-30 19:02:36.000000 linki-0.0.6/linki/change.py
--rw-r--r--   0 zone      (1000) zone      (1001)     2003 2023-04-30 19:07:29.000000 linki-0.0.6/linki/config.py
--rw-r--r--   0 zone      (1000) zone      (1001)     5330 2023-04-29 20:30:45.000000 linki-0.0.6/linki/connection.py
--rw-r--r--   0 zone      (1000) zone      (1001)     1949 2023-04-30 17:33:37.000000 linki-0.0.6/linki/contribution.py
--rw-r--r--   0 zone      (1000) zone      (1001)     1606 2023-04-22 21:37:54.000000 linki-0.0.6/linki/draft.py
--rw-r--r--   0 zone      (1000) zone      (1001)     5425 2023-04-29 20:25:23.000000 linki-0.0.6/linki/editor.py
--rw-r--r--   0 zone      (1000) zone      (1001)     3540 2023-04-24 15:45:14.000000 linki-0.0.6/linki/id.py
--rw-r--r--   0 zone      (1000) zone      (1001)     4136 2023-04-30 19:16:39.000000 linki-0.0.6/linki/inbox.py
--rw-r--r--   0 zone      (1000) zone      (1001)     9925 2023-06-19 06:01:16.000000 linki-0.0.6/linki/main.py
--rw-r--r--   0 zone      (1000) zone      (1001)      473 2023-04-18 07:35:07.000000 linki-0.0.6/linki/outbox.py
--rw-r--r--   0 zone      (1000) zone      (1001)     7170 2023-04-28 23:18:48.000000 linki-0.0.6/linki/repository.py
--rw-r--r--   0 zone      (1000) zone      (1001)      614 2023-04-24 19:48:37.000000 linki-0.0.6/linki/subscription.py
-drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 01:33:17.490700 linki-0.0.6/linki/testing/
--rw-r--r--   0 zone      (1000) zone      (1001)        0 2023-03-27 03:02:27.000000 linki-0.0.6/linki/testing/__init__.py
-drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 01:33:17.490700 linki-0.0.6/linki/testing/connection/
--rw-r--r--   0 zone      (1000) zone      (1001)        0 2023-04-07 20:24:28.000000 linki-0.0.6/linki/testing/connection/__init__.py
--rw-r--r--   0 zone      (1000) zone      (1001)      957 2023-04-18 11:26:31.000000 linki-0.0.6/linki/testing/connection/test_connection.py
-drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 01:33:17.494034 linki-0.0.6/linki/testing/editor/
--rw-r--r--   0 zone      (1000) zone      (1001)        0 2023-04-05 07:06:36.000000 linki-0.0.6/linki/testing/editor/__init__.py
--rw-r--r--   0 zone      (1000) zone      (1001)     4550 2023-04-22 12:59:18.000000 linki-0.0.6/linki/testing/editor/test_editor.py
--rw-r--r--   0 zone      (1000) zone      (1001)     6733 2023-04-24 16:38:27.000000 linki-0.0.6/linki/testing/editor/test_file_editor.py
-drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 01:33:17.494034 linki-0.0.6/linki/testing/main/
--rw-r--r--   0 zone      (1000) zone      (1001)        0 2023-04-17 00:00:13.000000 linki-0.0.6/linki/testing/main/__init__.py
--rw-r--r--   0 zone      (1000) zone      (1001)     4651 2023-06-19 06:57:23.000000 linki-0.0.6/linki/testing/main/test_complex_cases.py
--rw-r--r--   0 zone      (1000) zone      (1001)    10641 2023-06-19 06:36:59.000000 linki-0.0.6/linki/testing/main/test_successful_output.py
-drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 01:33:17.497367 linki-0.0.6/linki/testing/server/
--rw-r--r--   0 zone      (1000) zone      (1001)        0 2023-04-06 23:58:54.000000 linki-0.0.6/linki/testing/server/__init__.py
--rw-r--r--   0 zone      (1000) zone      (1001)     8226 2023-06-19 06:51:10.000000 linki-0.0.6/linki/testing/server/test_happy_path.py
-drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 01:33:17.497367 linki-0.0.6/linki/testing/strategies/
--rw-r--r--   0 zone      (1000) zone      (1001)        0 2023-03-27 04:11:40.000000 linki-0.0.6/linki/testing/strategies/__init__.py
--rw-r--r--   0 zone      (1000) zone      (1001)     1132 2023-04-22 21:34:16.000000 linki-0.0.6/linki/testing/strategies/article.py
--rw-r--r--   0 zone      (1000) zone      (1001)     1399 2023-04-22 21:37:54.000000 linki-0.0.6/linki/testing/strategies/draft.py
--rw-r--r--   0 zone      (1000) zone      (1001)      200 2023-04-15 08:40:19.000000 linki-0.0.6/linki/testing/strategies/type.py
--rw-r--r--   0 zone      (1000) zone      (1001)     1730 2023-04-22 16:55:55.000000 linki-0.0.6/linki/title.py
--rw-r--r--   0 zone      (1000) zone      (1001)     1743 2023-06-19 05:53:22.000000 linki-0.0.6/linki/url.py
--rw-r--r--   0 zone      (1000) zone      (1001)      777 2023-04-30 17:16:59.000000 linki-0.0.6/linki/user.py
--rw-r--r--   0 zone      (1000) zone      (1001)     7797 2023-04-30 17:33:12.000000 linki-0.0.6/linki/viewer.py
-drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 01:33:17.490700 linki-0.0.6/linki.egg-info/
--rw-r--r--   0 zone      (1000) zone      (1001)    10828 2023-06-20 01:33:17.000000 linki-0.0.6/linki.egg-info/PKG-INFO
--rw-r--r--   0 zone      (1000) zone      (1001)     1052 2023-06-20 01:33:17.000000 linki-0.0.6/linki.egg-info/SOURCES.txt
--rw-r--r--   0 zone      (1000) zone      (1001)        1 2023-06-20 01:33:17.000000 linki-0.0.6/linki.egg-info/dependency_links.txt
--rw-r--r--   0 zone      (1000) zone      (1001)       41 2023-06-20 01:33:17.000000 linki-0.0.6/linki.egg-info/entry_points.txt
--rw-r--r--   0 zone      (1000) zone      (1001)      158 2023-06-20 01:33:17.000000 linki-0.0.6/linki.egg-info/requires.txt
--rw-r--r--   0 zone      (1000) zone      (1001)        6 2023-06-20 01:33:17.000000 linki-0.0.6/linki.egg-info/top_level.txt
--rw-r--r--   0 zone      (1000) zone      (1001)      787 2023-06-20 01:30:53.000000 linki-0.0.6/pyproject.toml
--rw-r--r--   0 zone      (1000) zone      (1001)       38 2023-06-20 01:33:17.497367 linki-0.0.6/setup.cfg
+drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 02:14:16.622502 linki-0.0.7/
+-rw-r--r--   0 zone      (1000) zone      (1001)    34888 2023-06-20 01:08:26.000000 linki-0.0.7/LICENSE
+-rw-r--r--   0 zone      (1000) zone      (1001)    10828 2023-06-20 02:14:16.619169 linki-0.0.7/PKG-INFO
+-rw-r--r--   0 zone      (1000) zone      (1001)    10288 2023-06-19 07:55:18.000000 linki-0.0.7/README.md
+drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 02:14:16.615836 linki-0.0.7/linki/
+-rw-r--r--   0 zone      (1000) zone      (1001)        0 2023-04-16 23:56:36.000000 linki-0.0.7/linki/__init__.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     1971 2023-04-24 04:57:19.000000 linki-0.0.7/linki/article.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     1773 2023-04-30 19:02:36.000000 linki-0.0.7/linki/change.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     2003 2023-04-30 19:07:29.000000 linki-0.0.7/linki/config.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     5330 2023-04-29 20:30:45.000000 linki-0.0.7/linki/connection.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     1949 2023-04-30 17:33:37.000000 linki-0.0.7/linki/contribution.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     1606 2023-04-22 21:37:54.000000 linki-0.0.7/linki/draft.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     5425 2023-04-29 20:25:23.000000 linki-0.0.7/linki/editor.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     3540 2023-04-24 15:45:14.000000 linki-0.0.7/linki/id.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     4136 2023-04-30 19:16:39.000000 linki-0.0.7/linki/inbox.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     9925 2023-06-19 06:01:16.000000 linki-0.0.7/linki/main.py
+-rw-r--r--   0 zone      (1000) zone      (1001)      473 2023-04-18 07:35:07.000000 linki-0.0.7/linki/outbox.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     7170 2023-04-28 23:18:48.000000 linki-0.0.7/linki/repository.py
+-rw-r--r--   0 zone      (1000) zone      (1001)      614 2023-04-24 19:48:37.000000 linki-0.0.7/linki/subscription.py
+drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 02:14:16.615836 linki-0.0.7/linki/testing/
+-rw-r--r--   0 zone      (1000) zone      (1001)        0 2023-03-27 03:02:27.000000 linki-0.0.7/linki/testing/__init__.py
+drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 02:14:16.615836 linki-0.0.7/linki/testing/connection/
+-rw-r--r--   0 zone      (1000) zone      (1001)        0 2023-04-07 20:24:28.000000 linki-0.0.7/linki/testing/connection/__init__.py
+-rw-r--r--   0 zone      (1000) zone      (1001)      957 2023-04-18 11:26:31.000000 linki-0.0.7/linki/testing/connection/test_connection.py
+drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 02:14:16.619169 linki-0.0.7/linki/testing/editor/
+-rw-r--r--   0 zone      (1000) zone      (1001)        0 2023-04-05 07:06:36.000000 linki-0.0.7/linki/testing/editor/__init__.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     4550 2023-04-22 12:59:18.000000 linki-0.0.7/linki/testing/editor/test_editor.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     6733 2023-04-24 16:38:27.000000 linki-0.0.7/linki/testing/editor/test_file_editor.py
+drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 02:14:16.619169 linki-0.0.7/linki/testing/main/
+-rw-r--r--   0 zone      (1000) zone      (1001)        0 2023-04-17 00:00:13.000000 linki-0.0.7/linki/testing/main/__init__.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     4651 2023-06-19 06:57:23.000000 linki-0.0.7/linki/testing/main/test_complex_cases.py
+-rw-r--r--   0 zone      (1000) zone      (1001)    10641 2023-06-19 06:36:59.000000 linki-0.0.7/linki/testing/main/test_successful_output.py
+drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 02:14:16.619169 linki-0.0.7/linki/testing/server/
+-rw-r--r--   0 zone      (1000) zone      (1001)        0 2023-04-06 23:58:54.000000 linki-0.0.7/linki/testing/server/__init__.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     8226 2023-06-19 06:51:10.000000 linki-0.0.7/linki/testing/server/test_happy_path.py
+drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 02:14:16.619169 linki-0.0.7/linki/testing/strategies/
+-rw-r--r--   0 zone      (1000) zone      (1001)        0 2023-03-27 04:11:40.000000 linki-0.0.7/linki/testing/strategies/__init__.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     1132 2023-04-22 21:34:16.000000 linki-0.0.7/linki/testing/strategies/article.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     1399 2023-04-22 21:37:54.000000 linki-0.0.7/linki/testing/strategies/draft.py
+-rw-r--r--   0 zone      (1000) zone      (1001)      200 2023-04-15 08:40:19.000000 linki-0.0.7/linki/testing/strategies/type.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     1730 2023-04-22 16:55:55.000000 linki-0.0.7/linki/title.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     1743 2023-06-19 05:53:22.000000 linki-0.0.7/linki/url.py
+-rw-r--r--   0 zone      (1000) zone      (1001)      777 2023-04-30 17:16:59.000000 linki-0.0.7/linki/user.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     7797 2023-04-30 17:33:12.000000 linki-0.0.7/linki/viewer.py
+drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 02:14:16.615836 linki-0.0.7/linki.egg-info/
+-rw-r--r--   0 zone      (1000) zone      (1001)    10828 2023-06-20 02:14:16.000000 linki-0.0.7/linki.egg-info/PKG-INFO
+-rw-r--r--   0 zone      (1000) zone      (1001)     1052 2023-06-20 02:14:16.000000 linki-0.0.7/linki.egg-info/SOURCES.txt
+-rw-r--r--   0 zone      (1000) zone      (1001)        1 2023-06-20 02:14:16.000000 linki-0.0.7/linki.egg-info/dependency_links.txt
+-rw-r--r--   0 zone      (1000) zone      (1001)       41 2023-06-20 02:14:16.000000 linki-0.0.7/linki.egg-info/entry_points.txt
+-rw-r--r--   0 zone      (1000) zone      (1001)      158 2023-06-20 02:14:16.000000 linki-0.0.7/linki.egg-info/requires.txt
+-rw-r--r--   0 zone      (1000) zone      (1001)        6 2023-06-20 02:14:16.000000 linki-0.0.7/linki.egg-info/top_level.txt
+-rw-r--r--   0 zone      (1000) zone      (1001)      787 2023-06-20 02:13:55.000000 linki-0.0.7/pyproject.toml
+-rw-r--r--   0 zone      (1000) zone      (1001)       38 2023-06-20 02:14:16.622502 linki-0.0.7/setup.cfg
```

### Comparing `linki-0.0.6/LICENSE` & `linki-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `linki-0.0.6/PKG-INFO` & `linki-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linki
-Version: 0.0.6
+Version: 0.0.7
 Summary: Distributed wiki tools
 Project-URL: Homepage, https://github.com/roughdrafts-xyz/Linki
 Project-URL: Bug Tracker, https://github.com/roughdrafts-xyz/Linki/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `linki-0.0.6/README.md` & `linki-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `linki-0.0.6/linki/article.py` & `linki-0.0.7/linki/article.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.6/linki/change.py` & `linki-0.0.7/linki/change.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.6/linki/config.py` & `linki-0.0.7/linki/config.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.6/linki/connection.py` & `linki-0.0.7/linki/connection.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.6/linki/contribution.py` & `linki-0.0.7/linki/contribution.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.6/linki/draft.py` & `linki-0.0.7/linki/draft.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.6/linki/editor.py` & `linki-0.0.7/linki/editor.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.6/linki/id.py` & `linki-0.0.7/linki/id.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.6/linki/inbox.py` & `linki-0.0.7/linki/inbox.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.6/linki/main.py` & `linki-0.0.7/linki/main.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.6/linki/repository.py` & `linki-0.0.7/linki/repository.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.6/linki/subscription.py` & `linki-0.0.7/linki/subscription.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.6/linki/testing/connection/test_connection.py` & `linki-0.0.7/linki/testing/connection/test_connection.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.6/linki/testing/editor/test_editor.py` & `linki-0.0.7/linki/testing/editor/test_editor.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.6/linki/testing/editor/test_file_editor.py` & `linki-0.0.7/linki/testing/editor/test_file_editor.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.6/linki/testing/main/test_complex_cases.py` & `linki-0.0.7/linki/testing/main/test_complex_cases.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.6/linki/testing/main/test_successful_output.py` & `linki-0.0.7/linki/testing/main/test_successful_output.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.6/linki/testing/server/test_happy_path.py` & `linki-0.0.7/linki/testing/server/test_happy_path.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.6/linki/testing/strategies/article.py` & `linki-0.0.7/linki/testing/strategies/article.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.6/linki/testing/strategies/draft.py` & `linki-0.0.7/linki/testing/strategies/draft.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.6/linki/title.py` & `linki-0.0.7/linki/title.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.6/linki/url.py` & `linki-0.0.7/linki/url.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.6/linki/user.py` & `linki-0.0.7/linki/user.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.6/linki/viewer.py` & `linki-0.0.7/linki/viewer.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.6/linki.egg-info/PKG-INFO` & `linki-0.0.7/linki.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linki
-Version: 0.0.6
+Version: 0.0.7
 Summary: Distributed wiki tools
 Project-URL: Homepage, https://github.com/roughdrafts-xyz/Linki
 Project-URL: Bug Tracker, https://github.com/roughdrafts-xyz/Linki/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `linki-0.0.6/linki.egg-info/SOURCES.txt` & `linki-0.0.7/linki.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linki-0.0.6/pyproject.toml` & `linki-0.0.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [project]
 name = "linki"
-version = '0.0.6'
+version = '0.0.7'
 description = 'Distributed wiki tools'
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
-    "typer==0.7.0",
-    "typing_extensions==4.5.0",
-    "bottle==0.12.25",
-    "msgspec==0.16.0",
-    "Werkzeug==2.3.6",
-    "pypandoc==1.11",
-    "requests==2.31.0"
+    "typer~=0.7.0",
+    "typing_extensions~=4.5.0",
+    "bottle~=0.12.25",
+    "msgspec~=0.16.0",
+    "Werkzeug~=2.3.6",
+    "pypandoc~=1.11",
+    "requests~=2.31.0"
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent"
 ]
 
 [project.optional-dependencies]
-dev = ["pytest==7.3.2", "hypothesis==6.78.3"]
+dev = ["pytest~=7.3.2", "hypothesis~=6.78.3"]
 
 [project.scripts]
 linki = "linki:main.run"
 
 [project.urls]
 "Homepage" = "https://github.com/roughdrafts-xyz/Linki"
 "Bug Tracker" = "https://github.com/roughdrafts-xyz/Linki/issues"
```

