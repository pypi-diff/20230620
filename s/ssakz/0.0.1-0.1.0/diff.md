# Comparing `tmp/ssakz-0.0.1.tar.gz` & `tmp/ssakz-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssakz-0.0.1.tar", last modified: Sun Jun 18 14:45:01 2023, max compression
+gzip compressed data, was "ssakz-0.1.0.tar", last modified: Tue Jun 20 06:27:03 2023, max compression
```

## Comparing `ssakz-0.0.1.tar` & `ssakz-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-18 14:45:01.976278 ssakz-0.0.1/
--rw-r--r--   0 max       (1000) max       (1000)     1078 2023-06-18 14:38:59.000000 ssakz-0.0.1/LICENSE
--rw-r--r--   0 max       (1000) max       (1000)       34 2023-06-18 14:39:16.000000 ssakz-0.0.1/MANIFEST.in
--rw-r--r--   0 max       (1000) max       (1000)      201 2023-06-18 14:45:01.976278 ssakz-0.0.1/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)      408 2023-06-18 14:36:27.000000 ssakz-0.0.1/README.md
--rw-r--r--   0 max       (1000) max       (1000)       38 2023-06-18 14:45:01.976278 ssakz-0.0.1/setup.cfg
--rw-r--r--   0 max       (1000) max       (1000)      328 2023-06-18 14:44:47.000000 ssakz-0.0.1/setup.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-06-18 14:45:01.976278 ssakz-0.0.1/ssakz.egg-info/
--rw-r--r--   0 max       (1000) max       (1000)      201 2023-06-18 14:45:01.000000 ssakz-0.0.1/ssakz.egg-info/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)      219 2023-06-18 14:45:01.000000 ssakz-0.0.1/ssakz.egg-info/SOURCES.txt
--rw-r--r--   0 max       (1000) max       (1000)        1 2023-06-18 14:45:01.000000 ssakz-0.0.1/ssakz.egg-info/dependency_links.txt
--rw-r--r--   0 max       (1000) max       (1000)        1 2023-06-18 14:45:01.000000 ssakz-0.0.1/ssakz.egg-info/not-zip-safe
--rw-r--r--   0 max       (1000) max       (1000)        6 2023-06-18 14:45:01.000000 ssakz-0.0.1/ssakz.egg-info/requires.txt
--rw-r--r--   0 max       (1000) max       (1000)        6 2023-06-18 14:45:01.000000 ssakz-0.0.1/ssakz.egg-info/top_level.txt
--rw-r-xr-x   0 max       (1000) max       (1000)     2366 2023-06-18 14:24:34.000000 ssakz-0.0.1/ssakz.py
+drwxr-xr-x   0 max      (1000003) max       (1000)        0 2023-06-20 06:27:03.718271 ssakz-0.1.0/
+-rw-r--r--   0 max      (1000003) max       (1000)     1078 2023-06-18 15:39:54.000000 ssakz-0.1.0/LICENSE
+-rw-r--r--   0 max      (1000003) max       (1000)       35 2023-06-20 06:24:11.000000 ssakz-0.1.0/MANIFEST.in
+-rw-r--r--   0 max      (1000003) max       (1000)     1341 2023-06-20 06:27:03.718271 ssakz-0.1.0/PKG-INFO
+-rw-r--r--   0 max      (1000003) max       (1000)     1102 2023-06-20 06:23:44.000000 ssakz-0.1.0/README.rst
+-rw-r--r--   0 max      (1000003) max       (1000)       38 2023-06-20 06:27:03.718271 ssakz-0.1.0/setup.cfg
+-rw-r--r--   0 max      (1000003) max       (1000)      501 2023-06-20 06:26:56.000000 ssakz-0.1.0/setup.py
+drwxr-xr-x   0 max      (1000003) max       (1000)        0 2023-06-20 06:27:03.718271 ssakz-0.1.0/ssakz.egg-info/
+-rw-r--r--   0 max      (1000003) max       (1000)     1341 2023-06-20 06:27:03.000000 ssakz-0.1.0/ssakz.egg-info/PKG-INFO
+-rw-r--r--   0 max      (1000003) max       (1000)      220 2023-06-20 06:27:03.000000 ssakz-0.1.0/ssakz.egg-info/SOURCES.txt
+-rw-r--r--   0 max      (1000003) max       (1000)        1 2023-06-20 06:27:03.000000 ssakz-0.1.0/ssakz.egg-info/dependency_links.txt
+-rw-r--r--   0 max      (1000003) max       (1000)        1 2023-06-20 06:24:43.000000 ssakz-0.1.0/ssakz.egg-info/not-zip-safe
+-rw-r--r--   0 max      (1000003) max       (1000)        6 2023-06-20 06:27:03.000000 ssakz-0.1.0/ssakz.egg-info/requires.txt
+-rw-r--r--   0 max      (1000003) max       (1000)        6 2023-06-20 06:27:03.000000 ssakz-0.1.0/ssakz.egg-info/top_level.txt
+-rw-r--r--   0 max      (1000003) max       (1000)     3819 2023-06-20 06:07:30.000000 ssakz-0.1.0/ssakz.py
```

### Comparing `ssakz-0.0.1/LICENSE` & `ssakz-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ssakz-0.0.1/ssakz.py` & `ssakz-0.1.0/ssakz.py`

 * *Files 13% similar despite different names*

```diff
@@ -68,8 +68,55 @@
                 "until": until,
                 "rate": rate
             }
         }
         self.socket.send_string(json.dumps(request))
         return json.loads(self.socket.recv_string())
 
+    def get_sw_geomag_x(self, since, until=None, rate=None):
+        request = {
+            "type": "sw_geomag_x",
+            "filter": {
+                "since": since,
+                "until": until,
+                "rate": rate
+            }
+        }
+        self.socket.send_string(json.dumps(request))
+        return json.loads(self.socket.recv_string())
+
+    def get_sw_geomag_y(self, since, until=None, rate=None):
+        request = {
+            "type": "sw_geomag_y",
+            "filter": {
+                "since": since,
+                "until": until,
+                "rate": rate
+            }
+        }
+        self.socket.send_string(json.dumps(request))
+        return json.loads(self.socket.recv_string())
+
+    def get_sw_geomag_z(self, since, until=None, rate=None):
+        request = {
+            "type": "sw_geomag_z",
+            "filter": {
+                "since": since,
+                "until": until,
+                "rate": rate
+            }
+        }
+        self.socket.send_string(json.dumps(request))
+        return json.loads(self.socket.recv_string())
+
+    def get_sw_k_index(self, since, until=None, rate=None):
+        request = {
+            "type": "sw_k_index",
+            "filter": {
+                "since": since,
+                "until": until,
+                "rate": rate
+            }
+        }
+        self.socket.send_string(json.dumps(request))
+        return json.loads(self.socket.recv_string())
```

