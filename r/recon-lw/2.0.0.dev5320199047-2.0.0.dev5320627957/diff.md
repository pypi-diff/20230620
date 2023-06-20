# Comparing `tmp/recon_lw-2.0.0.dev5320199047.tar.gz` & `tmp/recon_lw-2.0.0.dev5320627957.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5320199047.tar", last modified: Tue Jun 20 08:20:34 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5320627957.tar", last modified: Tue Jun 20 09:05:13 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5320199047.tar` & `recon_lw-2.0.0.dev5320627957.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:20:34.000000 recon_lw-2.0.0.dev5320199047/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-20 08:19:43.000000 recon_lw-2.0.0.dev5320199047/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-20 08:20:34.000000 recon_lw-2.0.0.dev5320199047/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-20 08:19:43.000000 recon_lw-2.0.0.dev5320199047/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-20 08:20:10.000000 recon_lw-2.0.0.dev5320199047/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:20:34.000000 recon_lw-2.0.0.dev5320199047/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-20 08:19:43.000000 recon_lw-2.0.0.dev5320199047/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-06-20 08:19:43.000000 recon_lw-2.0.0.dev5320199047/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-20 08:19:43.000000 recon_lw-2.0.0.dev5320199047/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-06-20 08:19:43.000000 recon_lw-2.0.0.dev5320199047/recon_lw/SequenceCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-06-20 08:19:43.000000 recon_lw-2.0.0.dev5320199047/recon_lw/StateSequenceGenerator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-20 08:19:43.000000 recon_lw-2.0.0.dev5320199047/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-20 08:19:43.000000 recon_lw-2.0.0.dev5320199047/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13503 2023-06-20 08:19:43.000000 recon_lw-2.0.0.dev5320199047/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    32984 2023-06-20 08:19:43.000000 recon_lw-2.0.0.dev5320199047/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-06-20 08:19:43.000000 recon_lw-2.0.0.dev5320199047/recon_lw/recon_ob_cross_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     6018 2023-06-20 08:19:43.000000 recon_lw-2.0.0.dev5320199047/recon_lw/recon_ob_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:20:34.000000 recon_lw-2.0.0.dev5320199047/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-20 08:20:34.000000 recon_lw-2.0.0.dev5320199047/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-20 08:20:34.000000 recon_lw-2.0.0.dev5320199047/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-20 08:20:34.000000 recon_lw-2.0.0.dev5320199047/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-20 08:20:34.000000 recon_lw-2.0.0.dev5320199047/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-20 08:20:34.000000 recon_lw-2.0.0.dev5320199047/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-20 08:19:43.000000 recon_lw-2.0.0.dev5320199047/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-20 08:20:34.000000 recon_lw-2.0.0.dev5320199047/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-20 08:19:43.000000 recon_lw-2.0.0.dev5320199047/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 08:20:34.000000 recon_lw-2.0.0.dev5320199047/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-20 08:19:43.000000 recon_lw-2.0.0.dev5320199047/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 09:05:13.000000 recon_lw-2.0.0.dev5320627957/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-20 09:05:13.000000 recon_lw-2.0.0.dev5320627957/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-20 09:04:51.000000 recon_lw-2.0.0.dev5320627957/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 09:05:13.000000 recon_lw-2.0.0.dev5320627957/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4937 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/recon_lw/SequenceCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/recon_lw/StateSequenceGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13503 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32984 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/recon_lw/recon_ob_cross_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6018 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/recon_lw/recon_ob_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 09:05:13.000000 recon_lw-2.0.0.dev5320627957/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-20 09:05:13.000000 recon_lw-2.0.0.dev5320627957/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-20 09:05:13.000000 recon_lw-2.0.0.dev5320627957/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-20 09:05:13.000000 recon_lw-2.0.0.dev5320627957/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-20 09:05:13.000000 recon_lw-2.0.0.dev5320627957/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-20 09:05:13.000000 recon_lw-2.0.0.dev5320627957/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-20 09:05:13.000000 recon_lw-2.0.0.dev5320627957/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 09:05:13.000000 recon_lw-2.0.0.dev5320627957/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5320199047/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5320627957/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5320199047/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5320627957/recon_lw/LastStateMatcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                 o2 = None
             else:
                 records_times = self._state_cache[key1]["records_times"]
                 i = records_times.bisect_key_right(recon_lw.time_stamp_key(ts1))
                 if i == 0:
                     o2 = self._state_cache[key1]["prior_o"]
                 else:
-                    ts2 = records_times[i]
+                    ts2 = records_times[i-1]
                     sti = self._state_time_index.bisect_key_left(recon_lw.time_stamp_key(ts2) + "_" + key1)
                     o2 = self._state_time_index[sti][3]
             self._interpret_func([o1,o2], self._custom_settings, self._create_event, self._send_events)
 
         if horizon_time is not None:
             edge_timestamp = {"epochSecond": horizon_time["epochSecond"] - self._horizon_delay_seconds,
                               "nano": 0}
```

### Comparing `recon_lw-2.0.0.dev5320199047/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5320627957/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5320199047/recon_lw/SequenceCache.py` & `recon_lw-2.0.0.dev5320627957/recon_lw/SequenceCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5320199047/recon_lw/StateSequenceGenerator.py` & `recon_lw-2.0.0.dev5320627957/recon_lw/StateSequenceGenerator.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5320199047/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5320627957/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5320199047/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5320627957/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5320199047/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5320627957/recon_lw/recon_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5320199047/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5320627957/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5320199047/recon_lw/recon_ob_stats.py` & `recon_lw-2.0.0.dev5320627957/recon_lw/recon_ob_stats.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5320199047/recon_lw.egg-info/SOURCES.txt` & `recon_lw-2.0.0.dev5320627957/recon_lw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5320199047/setup.py` & `recon_lw-2.0.0.dev5320627957/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5320199047/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5320627957/test/test_recon_ob.py`

 * *Files identical despite different names*

