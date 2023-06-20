# Comparing `tmp/recon_lw-2.0.0.dev5320627957.tar.gz` & `tmp/recon_lw-2.0.0.dev5321044174.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5320627957.tar", last modified: Tue Jun 20 09:05:13 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5321044174.tar", last modified: Tue Jun 20 09:47:17 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5320627957.tar` & `recon_lw-2.0.0.dev5321044174.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 09:05:13.000000 recon_lw-2.0.0.dev5320627957/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-20 09:05:13.000000 recon_lw-2.0.0.dev5320627957/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-20 09:04:51.000000 recon_lw-2.0.0.dev5320627957/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 09:05:13.000000 recon_lw-2.0.0.dev5320627957/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     4937 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/recon_lw/SequenceCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/recon_lw/StateSequenceGenerator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13503 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    32984 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/recon_lw/recon_ob_cross_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     6018 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/recon_lw/recon_ob_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 09:05:13.000000 recon_lw-2.0.0.dev5320627957/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-20 09:05:13.000000 recon_lw-2.0.0.dev5320627957/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-20 09:05:13.000000 recon_lw-2.0.0.dev5320627957/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-20 09:05:13.000000 recon_lw-2.0.0.dev5320627957/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-20 09:05:13.000000 recon_lw-2.0.0.dev5320627957/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-20 09:05:13.000000 recon_lw-2.0.0.dev5320627957/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-20 09:05:13.000000 recon_lw-2.0.0.dev5320627957/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 09:05:13.000000 recon_lw-2.0.0.dev5320627957/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-20 09:04:29.000000 recon_lw-2.0.0.dev5320627957/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 09:47:17.000000 recon_lw-2.0.0.dev5321044174/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-20 09:47:17.000000 recon_lw-2.0.0.dev5321044174/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-20 09:46:55.000000 recon_lw-2.0.0.dev5321044174/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 09:47:17.000000 recon_lw-2.0.0.dev5321044174/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4937 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/recon_lw/SequenceCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/recon_lw/StateSequenceGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13503 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32984 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/recon_lw/recon_ob_cross_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6293 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/recon_lw/recon_ob_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 09:47:17.000000 recon_lw-2.0.0.dev5321044174/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-20 09:47:17.000000 recon_lw-2.0.0.dev5321044174/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-20 09:47:17.000000 recon_lw-2.0.0.dev5321044174/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-20 09:47:17.000000 recon_lw-2.0.0.dev5321044174/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-20 09:47:17.000000 recon_lw-2.0.0.dev5321044174/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-20 09:47:17.000000 recon_lw-2.0.0.dev5321044174/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-20 09:47:17.000000 recon_lw-2.0.0.dev5321044174/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 09:47:17.000000 recon_lw-2.0.0.dev5321044174/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5320627957/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5321044174/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5320627957/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5321044174/recon_lw/LastStateMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5320627957/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5321044174/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5320627957/recon_lw/SequenceCache.py` & `recon_lw-2.0.0.dev5321044174/recon_lw/SequenceCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5320627957/recon_lw/StateSequenceGenerator.py` & `recon_lw-2.0.0.dev5321044174/recon_lw/StateSequenceGenerator.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5320627957/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5321044174/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5320627957/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5321044174/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5320627957/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5321044174/recon_lw/recon_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5320627957/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5321044174/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5320627957/recon_lw/recon_ob_stats.py` & `recon_lw-2.0.0.dev5321044174/recon_lw/recon_ob_stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,22 @@
         error_event["attachedMessageIds"] = [match[0]["messageId"]]
         save_events([error_event])
         return
 
     stats = custom_settings["get_expected_stats_func"](match[0])
     fails = {}
     for k, v in stats.items():
+        if v is None:
+            if k in match[1]["body"] and match[1]["body"][k] is not None:
+                fails[k] = [v, match[1]["body"][k]]
+            continue
+        if k not in match[1]["body"]:
+            fails[k] = [v, "not initialized"]
+            continue
+
         if str(v) != str(match[1]["body"][k]):
             fails[k] = [v, str(match[1]["body"][k])]
 
     result_event = create_event("StatsCheck" + match[0]["messageType"],
                                 "StatsCheck",
                                 len(fails) == 0,
                                 {"stats_message": match[0],
```

### Comparing `recon_lw-2.0.0.dev5320627957/recon_lw.egg-info/SOURCES.txt` & `recon_lw-2.0.0.dev5321044174/recon_lw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5320627957/setup.py` & `recon_lw-2.0.0.dev5321044174/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5320627957/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5321044174/test/test_recon_ob.py`

 * *Files identical despite different names*

