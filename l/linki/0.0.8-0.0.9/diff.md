# Comparing `tmp/linki-0.0.8.tar.gz` & `tmp/linki-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linki-0.0.8.tar", last modified: Tue Jun 20 04:28:17 2023, max compression
+gzip compressed data, was "linki-0.0.9.tar", last modified: Tue Jun 20 04:40:52 2023, max compression
```

## Comparing `linki-0.0.8.tar` & `linki-0.0.9.tar`

### file list

```diff
@@ -1,53 +1,58 @@
-drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 04:28:17.808173 linki-0.0.8/
--rw-r--r--   0 zone      (1000) zone      (1001)    34888 2023-06-20 01:08:26.000000 linki-0.0.8/LICENSE
--rw-r--r--   0 zone      (1000) zone      (1001)    10828 2023-06-20 04:28:17.808173 linki-0.0.8/PKG-INFO
--rw-r--r--   0 zone      (1000) zone      (1001)    10288 2023-06-19 07:55:18.000000 linki-0.0.8/README.md
-drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 04:28:17.801506 linki-0.0.8/linki/
--rw-r--r--   0 zone      (1000) zone      (1001)        0 2023-04-16 23:56:36.000000 linki-0.0.8/linki/__init__.py
--rw-r--r--   0 zone      (1000) zone      (1001)     1971 2023-04-24 04:57:19.000000 linki-0.0.8/linki/article.py
--rw-r--r--   0 zone      (1000) zone      (1001)     1773 2023-04-30 19:02:36.000000 linki-0.0.8/linki/change.py
--rw-r--r--   0 zone      (1000) zone      (1001)     2003 2023-04-30 19:07:29.000000 linki-0.0.8/linki/config.py
--rw-r--r--   0 zone      (1000) zone      (1001)     5330 2023-04-29 20:30:45.000000 linki-0.0.8/linki/connection.py
--rw-r--r--   0 zone      (1000) zone      (1001)     1949 2023-04-30 17:33:37.000000 linki-0.0.8/linki/contribution.py
--rw-r--r--   0 zone      (1000) zone      (1001)     1606 2023-04-22 21:37:54.000000 linki-0.0.8/linki/draft.py
--rw-r--r--   0 zone      (1000) zone      (1001)     5425 2023-04-29 20:25:23.000000 linki-0.0.8/linki/editor.py
--rw-r--r--   0 zone      (1000) zone      (1001)     3540 2023-04-24 15:45:14.000000 linki-0.0.8/linki/id.py
--rw-r--r--   0 zone      (1000) zone      (1001)     4136 2023-04-30 19:16:39.000000 linki-0.0.8/linki/inbox.py
--rw-r--r--   0 zone      (1000) zone      (1001)     9950 2023-06-20 04:24:04.000000 linki-0.0.8/linki/main.py
--rw-r--r--   0 zone      (1000) zone      (1001)      473 2023-04-18 07:35:07.000000 linki-0.0.8/linki/outbox.py
--rw-r--r--   0 zone      (1000) zone      (1001)     7170 2023-04-28 23:18:48.000000 linki-0.0.8/linki/repository.py
--rw-r--r--   0 zone      (1000) zone      (1001)      614 2023-04-24 19:48:37.000000 linki-0.0.8/linki/subscription.py
-drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 04:28:17.804839 linki-0.0.8/linki/testing/
--rw-r--r--   0 zone      (1000) zone      (1001)        0 2023-03-27 03:02:27.000000 linki-0.0.8/linki/testing/__init__.py
-drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 04:28:17.804839 linki-0.0.8/linki/testing/connection/
--rw-r--r--   0 zone      (1000) zone      (1001)        0 2023-04-07 20:24:28.000000 linki-0.0.8/linki/testing/connection/__init__.py
--rw-r--r--   0 zone      (1000) zone      (1001)      957 2023-04-18 11:26:31.000000 linki-0.0.8/linki/testing/connection/test_connection.py
-drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 04:28:17.804839 linki-0.0.8/linki/testing/editor/
--rw-r--r--   0 zone      (1000) zone      (1001)        0 2023-04-05 07:06:36.000000 linki-0.0.8/linki/testing/editor/__init__.py
--rw-r--r--   0 zone      (1000) zone      (1001)     4550 2023-04-22 12:59:18.000000 linki-0.0.8/linki/testing/editor/test_editor.py
--rw-r--r--   0 zone      (1000) zone      (1001)     6733 2023-04-24 16:38:27.000000 linki-0.0.8/linki/testing/editor/test_file_editor.py
-drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 04:28:17.804839 linki-0.0.8/linki/testing/main/
--rw-r--r--   0 zone      (1000) zone      (1001)        0 2023-04-17 00:00:13.000000 linki-0.0.8/linki/testing/main/__init__.py
--rw-r--r--   0 zone      (1000) zone      (1001)     4651 2023-06-19 06:57:23.000000 linki-0.0.8/linki/testing/main/test_complex_cases.py
--rw-r--r--   0 zone      (1000) zone      (1001)    10641 2023-06-19 06:36:59.000000 linki-0.0.8/linki/testing/main/test_successful_output.py
-drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 04:28:17.808173 linki-0.0.8/linki/testing/server/
--rw-r--r--   0 zone      (1000) zone      (1001)        0 2023-04-06 23:58:54.000000 linki-0.0.8/linki/testing/server/__init__.py
--rw-r--r--   0 zone      (1000) zone      (1001)     8226 2023-06-19 06:51:10.000000 linki-0.0.8/linki/testing/server/test_happy_path.py
-drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 04:28:17.808173 linki-0.0.8/linki/testing/strategies/
--rw-r--r--   0 zone      (1000) zone      (1001)        0 2023-03-27 04:11:40.000000 linki-0.0.8/linki/testing/strategies/__init__.py
--rw-r--r--   0 zone      (1000) zone      (1001)     1132 2023-04-22 21:34:16.000000 linki-0.0.8/linki/testing/strategies/article.py
--rw-r--r--   0 zone      (1000) zone      (1001)     1399 2023-04-22 21:37:54.000000 linki-0.0.8/linki/testing/strategies/draft.py
--rw-r--r--   0 zone      (1000) zone      (1001)      200 2023-04-15 08:40:19.000000 linki-0.0.8/linki/testing/strategies/type.py
--rw-r--r--   0 zone      (1000) zone      (1001)     1730 2023-04-22 16:55:55.000000 linki-0.0.8/linki/title.py
--rw-r--r--   0 zone      (1000) zone      (1001)     1743 2023-06-19 05:53:22.000000 linki-0.0.8/linki/url.py
--rw-r--r--   0 zone      (1000) zone      (1001)      777 2023-04-30 17:16:59.000000 linki-0.0.8/linki/user.py
--rw-r--r--   0 zone      (1000) zone      (1001)     7797 2023-04-30 17:33:12.000000 linki-0.0.8/linki/viewer.py
-drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 04:28:17.804839 linki-0.0.8/linki.egg-info/
--rw-r--r--   0 zone      (1000) zone      (1001)    10828 2023-06-20 04:28:17.000000 linki-0.0.8/linki.egg-info/PKG-INFO
--rw-r--r--   0 zone      (1000) zone      (1001)     1052 2023-06-20 04:28:17.000000 linki-0.0.8/linki.egg-info/SOURCES.txt
--rw-r--r--   0 zone      (1000) zone      (1001)        1 2023-06-20 04:28:17.000000 linki-0.0.8/linki.egg-info/dependency_links.txt
--rw-r--r--   0 zone      (1000) zone      (1001)       41 2023-06-20 04:28:17.000000 linki-0.0.8/linki.egg-info/entry_points.txt
--rw-r--r--   0 zone      (1000) zone      (1001)      158 2023-06-20 04:28:17.000000 linki-0.0.8/linki.egg-info/requires.txt
--rw-r--r--   0 zone      (1000) zone      (1001)        6 2023-06-20 04:28:17.000000 linki-0.0.8/linki.egg-info/top_level.txt
--rw-r--r--   0 zone      (1000) zone      (1001)      787 2023-06-20 04:27:51.000000 linki-0.0.8/pyproject.toml
--rw-r--r--   0 zone      (1000) zone      (1001)       38 2023-06-20 04:28:17.808173 linki-0.0.8/setup.cfg
+drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 04:40:52.609120 linki-0.0.9/
+-rw-r--r--   0 zone      (1000) zone      (1001)    34888 2023-06-20 01:08:26.000000 linki-0.0.9/LICENSE
+-rw-r--r--   0 zone      (1000) zone      (1001)       30 2023-06-20 04:40:33.000000 linki-0.0.9/MANIFEST.in
+-rw-r--r--   0 zone      (1000) zone      (1001)    10828 2023-06-20 04:40:52.609120 linki-0.0.9/PKG-INFO
+-rw-r--r--   0 zone      (1000) zone      (1001)    10288 2023-06-19 07:55:18.000000 linki-0.0.9/README.md
+drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 04:40:52.602453 linki-0.0.9/linki/
+-rw-r--r--   0 zone      (1000) zone      (1001)        0 2023-04-16 23:56:36.000000 linki-0.0.9/linki/__init__.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     1971 2023-04-24 04:57:19.000000 linki-0.0.9/linki/article.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     1773 2023-04-30 19:02:36.000000 linki-0.0.9/linki/change.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     2003 2023-04-30 19:07:29.000000 linki-0.0.9/linki/config.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     5330 2023-04-29 20:30:45.000000 linki-0.0.9/linki/connection.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     1949 2023-04-30 17:33:37.000000 linki-0.0.9/linki/contribution.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     1606 2023-04-22 21:37:54.000000 linki-0.0.9/linki/draft.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     5425 2023-04-29 20:25:23.000000 linki-0.0.9/linki/editor.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     3540 2023-04-24 15:45:14.000000 linki-0.0.9/linki/id.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     4136 2023-04-30 19:16:39.000000 linki-0.0.9/linki/inbox.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     9950 2023-06-20 04:24:04.000000 linki-0.0.9/linki/main.py
+-rw-r--r--   0 zone      (1000) zone      (1001)      473 2023-04-18 07:35:07.000000 linki-0.0.9/linki/outbox.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     7170 2023-04-28 23:18:48.000000 linki-0.0.9/linki/repository.py
+-rw-r--r--   0 zone      (1000) zone      (1001)      614 2023-04-24 19:48:37.000000 linki-0.0.9/linki/subscription.py
+drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 04:40:52.605787 linki-0.0.9/linki/templates/
+-rw-r--r--   0 zone      (1000) zone      (1001)      507 2023-04-24 02:36:10.000000 linki-0.0.9/linki/templates/base.html
+-rw-r--r--   0 zone      (1000) zone      (1001)      300 2023-04-24 02:32:39.000000 linki-0.0.9/linki/templates/many.html
+-rw-r--r--   0 zone      (1000) zone      (1001)      320 2023-04-24 16:26:42.000000 linki-0.0.9/linki/templates/one.html
+drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 04:40:52.605787 linki-0.0.9/linki/testing/
+-rw-r--r--   0 zone      (1000) zone      (1001)        0 2023-03-27 03:02:27.000000 linki-0.0.9/linki/testing/__init__.py
+drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 04:40:52.605787 linki-0.0.9/linki/testing/connection/
+-rw-r--r--   0 zone      (1000) zone      (1001)        0 2023-04-07 20:24:28.000000 linki-0.0.9/linki/testing/connection/__init__.py
+-rw-r--r--   0 zone      (1000) zone      (1001)      957 2023-04-18 11:26:31.000000 linki-0.0.9/linki/testing/connection/test_connection.py
+drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 04:40:52.605787 linki-0.0.9/linki/testing/editor/
+-rw-r--r--   0 zone      (1000) zone      (1001)        0 2023-04-05 07:06:36.000000 linki-0.0.9/linki/testing/editor/__init__.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     4550 2023-04-22 12:59:18.000000 linki-0.0.9/linki/testing/editor/test_editor.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     6733 2023-04-24 16:38:27.000000 linki-0.0.9/linki/testing/editor/test_file_editor.py
+drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 04:40:52.605787 linki-0.0.9/linki/testing/main/
+-rw-r--r--   0 zone      (1000) zone      (1001)        0 2023-04-17 00:00:13.000000 linki-0.0.9/linki/testing/main/__init__.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     4651 2023-06-19 06:57:23.000000 linki-0.0.9/linki/testing/main/test_complex_cases.py
+-rw-r--r--   0 zone      (1000) zone      (1001)    10641 2023-06-19 06:36:59.000000 linki-0.0.9/linki/testing/main/test_successful_output.py
+drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 04:40:52.605787 linki-0.0.9/linki/testing/server/
+-rw-r--r--   0 zone      (1000) zone      (1001)        0 2023-04-06 23:58:54.000000 linki-0.0.9/linki/testing/server/__init__.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     8226 2023-06-19 06:51:10.000000 linki-0.0.9/linki/testing/server/test_happy_path.py
+drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 04:40:52.609120 linki-0.0.9/linki/testing/strategies/
+-rw-r--r--   0 zone      (1000) zone      (1001)        0 2023-03-27 04:11:40.000000 linki-0.0.9/linki/testing/strategies/__init__.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     1132 2023-04-22 21:34:16.000000 linki-0.0.9/linki/testing/strategies/article.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     1399 2023-04-22 21:37:54.000000 linki-0.0.9/linki/testing/strategies/draft.py
+-rw-r--r--   0 zone      (1000) zone      (1001)      200 2023-04-15 08:40:19.000000 linki-0.0.9/linki/testing/strategies/type.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     1730 2023-04-22 16:55:55.000000 linki-0.0.9/linki/title.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     1743 2023-06-19 05:53:22.000000 linki-0.0.9/linki/url.py
+-rw-r--r--   0 zone      (1000) zone      (1001)      777 2023-04-30 17:16:59.000000 linki-0.0.9/linki/user.py
+-rw-r--r--   0 zone      (1000) zone      (1001)     7797 2023-04-30 17:33:12.000000 linki-0.0.9/linki/viewer.py
+drwxr-xr-x   0 zone      (1000) zone      (1001)        0 2023-06-20 04:40:52.602453 linki-0.0.9/linki.egg-info/
+-rw-r--r--   0 zone      (1000) zone      (1001)    10828 2023-06-20 04:40:52.000000 linki-0.0.9/linki.egg-info/PKG-INFO
+-rw-r--r--   0 zone      (1000) zone      (1001)     1141 2023-06-20 04:40:52.000000 linki-0.0.9/linki.egg-info/SOURCES.txt
+-rw-r--r--   0 zone      (1000) zone      (1001)        1 2023-06-20 04:40:52.000000 linki-0.0.9/linki.egg-info/dependency_links.txt
+-rw-r--r--   0 zone      (1000) zone      (1001)       41 2023-06-20 04:40:52.000000 linki-0.0.9/linki.egg-info/entry_points.txt
+-rw-r--r--   0 zone      (1000) zone      (1001)      158 2023-06-20 04:40:52.000000 linki-0.0.9/linki.egg-info/requires.txt
+-rw-r--r--   0 zone      (1000) zone      (1001)        6 2023-06-20 04:40:52.000000 linki-0.0.9/linki.egg-info/top_level.txt
+-rw-r--r--   0 zone      (1000) zone      (1001)      787 2023-06-20 04:40:40.000000 linki-0.0.9/pyproject.toml
+-rw-r--r--   0 zone      (1000) zone      (1001)       38 2023-06-20 04:40:52.609120 linki-0.0.9/setup.cfg
```

### Comparing `linki-0.0.8/LICENSE` & `linki-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `linki-0.0.8/PKG-INFO` & `linki-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linki
-Version: 0.0.8
+Version: 0.0.9
 Summary: Distributed wiki tools
 Project-URL: Homepage, https://github.com/roughdrafts-xyz/Linki
 Project-URL: Bug Tracker, https://github.com/roughdrafts-xyz/Linki/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `linki-0.0.8/README.md` & `linki-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `linki-0.0.8/linki/article.py` & `linki-0.0.9/linki/article.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.8/linki/change.py` & `linki-0.0.9/linki/change.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.8/linki/config.py` & `linki-0.0.9/linki/config.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.8/linki/connection.py` & `linki-0.0.9/linki/connection.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.8/linki/contribution.py` & `linki-0.0.9/linki/contribution.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.8/linki/draft.py` & `linki-0.0.9/linki/draft.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.8/linki/editor.py` & `linki-0.0.9/linki/editor.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.8/linki/id.py` & `linki-0.0.9/linki/id.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.8/linki/inbox.py` & `linki-0.0.9/linki/inbox.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.8/linki/main.py` & `linki-0.0.9/linki/main.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.8/linki/repository.py` & `linki-0.0.9/linki/repository.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.8/linki/subscription.py` & `linki-0.0.9/linki/subscription.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.8/linki/testing/connection/test_connection.py` & `linki-0.0.9/linki/testing/connection/test_connection.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.8/linki/testing/editor/test_editor.py` & `linki-0.0.9/linki/testing/editor/test_editor.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.8/linki/testing/editor/test_file_editor.py` & `linki-0.0.9/linki/testing/editor/test_file_editor.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.8/linki/testing/main/test_complex_cases.py` & `linki-0.0.9/linki/testing/main/test_complex_cases.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.8/linki/testing/main/test_successful_output.py` & `linki-0.0.9/linki/testing/main/test_successful_output.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.8/linki/testing/server/test_happy_path.py` & `linki-0.0.9/linki/testing/server/test_happy_path.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.8/linki/testing/strategies/article.py` & `linki-0.0.9/linki/testing/strategies/article.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.8/linki/testing/strategies/draft.py` & `linki-0.0.9/linki/testing/strategies/draft.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.8/linki/title.py` & `linki-0.0.9/linki/title.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.8/linki/url.py` & `linki-0.0.9/linki/url.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.8/linki/user.py` & `linki-0.0.9/linki/user.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.8/linki/viewer.py` & `linki-0.0.9/linki/viewer.py`

 * *Files identical despite different names*

### Comparing `linki-0.0.8/linki.egg-info/PKG-INFO` & `linki-0.0.9/linki.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linki
-Version: 0.0.8
+Version: 0.0.9
 Summary: Distributed wiki tools
 Project-URL: Homepage, https://github.com/roughdrafts-xyz/Linki
 Project-URL: Bug Tracker, https://github.com/roughdrafts-xyz/Linki/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `linki-0.0.8/linki.egg-info/SOURCES.txt` & `linki-0.0.9/linki.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 linki/__init__.py
 linki/article.py
 linki/change.py
 linki/config.py
 linki/connection.py
@@ -21,14 +22,17 @@
 linki/viewer.py
 linki.egg-info/PKG-INFO
 linki.egg-info/SOURCES.txt
 linki.egg-info/dependency_links.txt
 linki.egg-info/entry_points.txt
 linki.egg-info/requires.txt
 linki.egg-info/top_level.txt
+linki/templates/base.html
+linki/templates/many.html
+linki/templates/one.html
 linki/testing/__init__.py
 linki/testing/connection/__init__.py
 linki/testing/connection/test_connection.py
 linki/testing/editor/__init__.py
 linki/testing/editor/test_editor.py
 linki/testing/editor/test_file_editor.py
 linki/testing/main/__init__.py
```

### Comparing `linki-0.0.8/pyproject.toml` & `linki-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "linki"
-version = '0.0.8'
+version = '0.0.9'
 description = 'Distributed wiki tools'
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
     "typer~=0.9.0",
     "typing_extensions~=4.5.0",
     "bottle~=0.12.25",
```

