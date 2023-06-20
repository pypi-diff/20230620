# Comparing `tmp/dassana-0.8.6.tar.gz` & `tmp/dassana-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dassana-0.8.6.tar", last modified: Wed Jun 14 08:35:47 2023, max compression
+gzip compressed data, was "dassana-0.8.7.tar", last modified: Tue Jun 20 06:20:02 2023, max compression
```

## Comparing `dassana-0.8.6.tar` & `dassana-0.8.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:35:47.756596 dassana-0.8.6/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-14 08:35:47.756596 dassana-0.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-14 08:35:39.000000 dassana-0.8.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:35:47.756596 dassana-0.8.6/dassana/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-14 08:35:39.000000 dassana-0.8.6/dassana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-06-14 08:35:39.000000 dassana-0.8.6/dassana/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-14 08:35:39.000000 dassana-0.8.6/dassana/dassana_env.py
--rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-06-14 08:35:39.000000 dassana-0.8.6/dassana/data_pipes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-06-14 08:35:39.000000 dassana-0.8.6/dassana/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:35:47.756596 dassana-0.8.6/dassana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-14 08:35:47.000000 dassana-0.8.6/dassana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-14 08:35:47.000000 dassana-0.8.6/dassana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:35:47.000000 dassana-0.8.6/dassana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:35:47.000000 dassana-0.8.6/dassana.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-14 08:35:47.000000 dassana-0.8.6/dassana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 08:35:47.000000 dassana-0.8.6/dassana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 08:35:47.756596 dassana-0.8.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-14 08:35:39.000000 dassana-0.8.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:20:02.314661 dassana-0.8.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-20 06:20:02.314661 dassana-0.8.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-20 06:19:53.000000 dassana-0.8.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:20:02.314661 dassana-0.8.7/dassana/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-20 06:19:53.000000 dassana-0.8.7/dassana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-06-20 06:19:53.000000 dassana-0.8.7/dassana/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-20 06:19:53.000000 dassana-0.8.7/dassana/dassana_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-06-20 06:19:53.000000 dassana-0.8.7/dassana/data_pipes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-06-20 06:19:53.000000 dassana-0.8.7/dassana/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:20:02.314661 dassana-0.8.7/dassana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-20 06:20:02.000000 dassana-0.8.7/dassana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-20 06:20:02.000000 dassana-0.8.7/dassana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 06:20:02.000000 dassana-0.8.7/dassana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 06:20:02.000000 dassana-0.8.7/dassana.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-20 06:20:02.000000 dassana-0.8.7/dassana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 06:20:02.000000 dassana-0.8.7/dassana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 06:20:02.314661 dassana-0.8.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-20 06:19:53.000000 dassana-0.8.7/setup.py
```

### Comparing `dassana-0.8.6/dassana/common.py` & `dassana-0.8.7/dassana/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
 
     def write_json(self, json_object):
         self.file.flush()
         json.dump(json_object, self.file)
         self.file.write('\n')
         self.bytes_written = self.file.tell()
         if self.bytes_written >= 99 * 1000 * 1000:
-            self.close()
+            self.file.close()
             self.compress_file()
             self.upload_to_cloud()
             self.file_path = self.get_file_path()
             self.file = open(self.file_path, 'a')
             print("Ingested data: " + self.bytes_written)
             self.bytes_written = 0
```

### Comparing `dassana-0.8.6/dassana/dassana_env.py` & `dassana-0.8.7/dassana/dassana_env.py`

 * *Files identical despite different names*

### Comparing `dassana-0.8.6/dassana/data_pipes.py` & `dassana-0.8.7/dassana/data_pipes.py`

 * *Files identical despite different names*

### Comparing `dassana-0.8.6/dassana/rest.py` & `dassana-0.8.7/dassana/rest.py`

 * *Files identical despite different names*

