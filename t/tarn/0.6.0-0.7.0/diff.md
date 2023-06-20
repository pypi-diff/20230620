# Comparing `tmp/tarn-0.6.0.tar.gz` & `tmp/tarn-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarn-0.6.0.tar", last modified: Thu Jun  8 11:40:19 2023, max compression
+gzip compressed data, was "tarn-0.7.0.tar", last modified: Tue Jun 20 16:08:05 2023, max compression
```

## Comparing `tarn-0.6.0.tar` & `tarn-0.7.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:40:19.944898 tarn-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-06-08 11:40:16.000000 tarn-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-08 11:40:16.000000 tarn-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-08 11:40:19.944898 tarn-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-08 11:40:16.000000 tarn-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-08 11:40:16.000000 tarn-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 11:40:16.000000 tarn-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 11:40:19.944898 tarn-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-08 11:40:16.000000 tarn-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:40:19.936898 tarn-0.6.0/tarn/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:40:19.940898 tarn-0.6.0/tarn/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/cache/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/cache/index.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/cache/pickler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/cache/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/cache/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/digest.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:40:19.940898 tarn-0.6.0/tarn/local/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/local/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/local/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:40:19.940898 tarn-0.6.0/tarn/location/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/location/disk_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/location/fanout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/location/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/location/levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/location/nginx.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/location/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:40:19.940898 tarn-0.6.0/tarn/pickler/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/pickler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/pickler/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/pickler/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:40:19.940898 tarn-0.6.0/tarn/pool/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/pool/hash_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/pool/pickle_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:40:19.940898 tarn-0.6.0/tarn/remote/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/remote/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/remote/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:40:19.944898 tarn-0.6.0/tarn/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/tools/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/tools/locker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/tools/size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/tools/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-08 11:40:16.000000 tarn-0.6.0/tarn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:40:19.940898 tarn-0.6.0/tarn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-08 11:40:19.000000 tarn-0.6.0/tarn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-08 11:40:19.000000 tarn-0.6.0/tarn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 11:40:19.000000 tarn-0.6.0/tarn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 11:40:19.000000 tarn-0.6.0/tarn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-08 11:40:19.000000 tarn-0.6.0/tarn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:05.920478 tarn-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-06-20 16:08:03.000000 tarn-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-20 16:08:03.000000 tarn-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-20 16:08:05.920478 tarn-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-20 16:08:03.000000 tarn-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-20 16:08:03.000000 tarn-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-20 16:08:03.000000 tarn-0.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 16:08:05.920478 tarn-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-20 16:08:03.000000 tarn-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:05.916478 tarn-0.7.0/tarn/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:05.916478 tarn-0.7.0/tarn/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/cache/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/cache/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/cache/pickler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/cache/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/cache/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:05.916478 tarn-0.7.0/tarn/local/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/local/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/local/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:05.916478 tarn-0.7.0/tarn/location/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/location/disk_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/location/fanout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/location/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/location/levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/location/nginx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/location/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:05.916478 tarn-0.7.0/tarn/pickler/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/pickler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/pickler/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/pickler/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:05.916478 tarn-0.7.0/tarn/pool/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/pool/hash_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/pool/pickle_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:05.916478 tarn-0.7.0/tarn/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/remote/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/remote/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:05.920478 tarn-0.7.0/tarn/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/tools/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/tools/locker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/tools/size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/tools/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-20 16:08:03.000000 tarn-0.7.0/tarn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:08:05.916478 tarn-0.7.0/tarn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-06-20 16:08:05.000000 tarn-0.7.0/tarn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-20 16:08:05.000000 tarn-0.7.0/tarn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:08:05.000000 tarn-0.7.0/tarn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-20 16:08:05.000000 tarn-0.7.0/tarn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-20 16:08:05.000000 tarn-0.7.0/tarn.egg-info/top_level.txt
```

### Comparing `tarn-0.6.0/LICENSE` & `tarn-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tarn-0.6.0/PKG-INFO` & `tarn-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tarn
-Version: 0.6.0
+Version: 0.7.0
 Summary: A hashmap-based storage on local and remote disks
 Home-page: https://github.com/neuro-ml/tarn
 Author: Max
 Author-email: max@ira-labs.com
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/tarn/archive/v0.6.0.tar.gz
+Download-URL: https://github.com/neuro-ml/tarn/archive/v0.7.0.tar.gz
 Keywords: storage,cache,invalidation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tarn-0.6.0/README.md` & `tarn-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `tarn-0.6.0/pyproject.toml` & `tarn-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tarn-0.6.0/setup.py` & `tarn-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `tarn-0.6.0/tarn/cache/storage.py` & `tarn-0.7.0/tarn/cache/storage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.6.0/tarn/compat.py` & `tarn-0.7.0/tarn/compat.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import errno
 import os
 import platform
 import shutil
 import stat
 from pathlib import Path
 from typing import Union
+from tempfile import SpooledTemporaryFile as _SpooledTemporaryFile
 
 try:
     from typing import Protocol
 except ImportError:
     Protocol = object
 try:
     from gzip import BadGzipFile
@@ -39,14 +40,21 @@
     rmtree = shutil.rmtree
     remove_file = os.remove
 
 
     def get_path_group(path: PathOrStr) -> Union[int, None]:
         return Path(path).stat().st_gid
 
+if hasattr(_SpooledTemporaryFile, 'seekable'):
+    SpooledTemporaryFile = _SpooledTemporaryFile
+else:
+    class SpooledTemporaryFile(_SpooledTemporaryFile):
+        def seekable(self) -> bool:
+            return True
+
 
 def set_path_attrs(path: Path, permissions: Union[int, None] = None, group: Union[str, int, None] = None):
     if permissions is not None:
         path.chmod(permissions)
     if group is not None:
         shutil.chown(path, group=group)
```

### Comparing `tarn-0.6.0/tarn/config.py` & `tarn-0.7.0/tarn/config.py`

 * *Files identical despite different names*

### Comparing `tarn-0.6.0/tarn/digest.py` & `tarn-0.7.0/tarn/digest.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+from io import BytesIO
 import os
 from contextlib import contextmanager
 from pathlib import Path
-from typing import AnyStr, Sequence, Type
+from typing import AnyStr, Sequence, Type, Union
 
 from .compat import HashAlgorithm
 from .interface import Value
 
 
 def digest_file(path, algorithm, block_size=2 ** 20):
     return digest_value(path, algorithm, block_size).hex()
 
 
-def digest_value(value: Value, algorithm: Type[HashAlgorithm], block_size: int = 2 ** 20) -> bytes:
-    with _value_to_buffer(value) as buffer:
+def digest_value(value: Union[Value, bytes], algorithm: Type[HashAlgorithm], block_size: int = 2 ** 20) -> bytes:
+    with value_to_buffer(value) as buffer:
         hasher = algorithm()
         while True:
             chunk = buffer.read(block_size)
             if not chunk:
                 break
             hasher.update(chunk)
 
@@ -44,14 +45,17 @@
     size = sum(levels)
     if string:
         size *= 2
     return size
 
 
 @contextmanager
-def _value_to_buffer(value: Value):
-    if isinstance(value, (str, os.PathLike)):
+def value_to_buffer(value: Union[Value, bytes]):
+    if isinstance(value, bytes):
+        yield BytesIO(value)
+
+    elif isinstance(value, (str, os.PathLike)):
         with open(value, 'rb') as file:
             yield file
 
     else:
         yield value
```

### Comparing `tarn-0.6.0/tarn/interface.py` & `tarn-0.7.0/tarn/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.6.0/tarn/local/storage.py` & `tarn-0.7.0/tarn/local/storage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.6.0/tarn/location/disk_dict.py` & `tarn-0.7.0/tarn/location/disk_dict.py`

 * *Files identical despite different names*

### Comparing `tarn-0.6.0/tarn/location/fanout.py` & `tarn-0.7.0/tarn/location/fanout.py`

 * *Files identical despite different names*

### Comparing `tarn-0.6.0/tarn/location/interface.py` & `tarn-0.7.0/tarn/location/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.6.0/tarn/location/levels.py` & `tarn-0.7.0/tarn/location/levels.py`

 * *Files identical despite different names*

### Comparing `tarn-0.6.0/tarn/location/nginx.py` & `tarn-0.7.0/tarn/location/nginx.py`

 * *Files identical despite different names*

### Comparing `tarn-0.6.0/tarn/location/scp.py` & `tarn-0.7.0/tarn/location/scp.py`

 * *Files identical despite different names*

### Comparing `tarn-0.6.0/tarn/pickler/compat.py` & `tarn-0.7.0/tarn/pickler/compat.py`

 * *Files identical despite different names*

### Comparing `tarn-0.6.0/tarn/pickler/interface.py` & `tarn-0.7.0/tarn/pickler/interface.py`

 * *Files identical despite different names*

### Comparing `tarn-0.6.0/tarn/pool/hash_key.py` & `tarn-0.7.0/tarn/pool/hash_key.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from io import BytesIO
 import os
 from contextlib import contextmanager
+from pathlib import Path
 from typing import Any, Callable, ContextManager, Iterable, Optional, Sequence, Tuple, Type, Union, Collection
 
 from ..compat import HashAlgorithm
 from ..digest import digest_value
 from ..exceptions import ReadError, WriteError
-from ..interface import Key, Keys, MaybeValue, PathOrStr, MaybeLabels
+from ..interface import Key, Keys, MaybeValue, PathOrStr, MaybeLabels, Value
 from ..location import DiskDict, Fanout, Levels, Location
 
 LocationLike = Union[Location, PathOrStr]
 LocationsLike = Union[LocationLike, Sequence[LocationLike]]
 
 
 class HashKeyStorage:
@@ -56,20 +58,30 @@
                 raise ReadError(f'The key {key.hex()} is not found')
             yield value
 
     def _read_func(self, func: Callable, key: Key, *args, fetch, error, **kwargs) -> Any:
         with self._read_context(key, fetch, error) as value:
             return func(value, *args, **kwargs)
 
-    # TODO: add support for buffers
-    def write(self, value: PathOrStr, error: Optional[bool] = None, labels: MaybeLabels = None) -> Optional[Key]:
+    def write(self, value: Union[Value, bytes], error: Optional[bool] = None,
+              labels: MaybeLabels = None) -> Optional[Key]:
         error = self._resolve_value(error, self._error, 'error')
         labels = self._resolve_value(labels, self.labels, None)
 
-        digest = digest_value(value, self.algorithm)
+        if isinstance(value, (bytes, Path, str)):
+            digest = digest_value(value, self.algorithm)
+        else:
+            assert value.seekable(), value
+            position = value.tell()
+            digest = digest_value(value, self.algorithm)
+            value.seek(position)
+
+        if isinstance(value, bytes):
+            value = BytesIO(value)
+
         with self._local.write(digest, value, labels) as written:
             # TODO: check digest?
             if written is None:
                 if error:
                     raise WriteError(digest.hex())
                 return None
```

### Comparing `tarn-0.6.0/tarn/pool/pickle_key.py` & `tarn-0.7.0/tarn/pool/pickle_key.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import json
 import logging
-from contextlib import contextmanager
 from io import BytesIO
 from pathlib import Path
-from tempfile import TemporaryDirectory
 from typing import Any, NamedTuple, Optional, Sequence, Type, Union
 
 from ..compat import HashAlgorithm
 from ..exceptions import ReadError, StorageCorruption, WriteError, DeserializationError
 from ..interface import Key, PathOrStr, MaybeLabels
 from ..location import Level, Location
 from ..pickler import PREVIOUS_VERSIONS, dumps
@@ -63,26 +61,15 @@
 
     def write(self, key: ProxyKey, value: Any, *, error: bool = True, labels: MaybeLabels = None) -> Optional[Key]:
         if not isinstance(key, _PreparedKey):
             key = self.prepare(key)
 
         digest = key.digest
         logger.info('Serializing %s', digest)
-        mapping = {}
-        with TemporaryDirectory() as temp_folder:
-            temp_folder = Path(temp_folder)
-            self.serializer.save(value, temp_folder)
-
-            for file in temp_folder.glob('**/*'):
-                if file.is_dir():
-                    continue
-
-                relative = str(file.relative_to(temp_folder))
-                assert relative not in mapping
-                mapping[relative] = self.storage.write(file, labels=labels).hex()
+        mapping = dict(self.serializer.save(value, lambda v: self.storage.write(v, labels=labels).hex()))
 
         # we want a reproducible mapping each time
         logger.info('Saving to index %s', digest)
         with self.index.write(digest, BytesIO(json.dumps(mapping, sort_keys=True).encode()), labels=None) as written:
             if written is None:
                 if error:
                     raise WriteError('The index could not be written to any storage')
@@ -91,38 +78,38 @@
         return digest
 
     def _read_for_digest(self, digest):
         with self.index.read(digest) as index:
             if index is None:
                 return None, False
 
-            with _unpack_mapping(index) as folder:
-                try:
-                    return self.serializer.load(folder, self.storage), True
-                # either the data is corrupted or missing
-                except (DeserializationError, ReadError) as e:
-                    raise StorageCorruption from e
-                except SerializerError as e:
-                    raise SerializerError(f'Could not deserialize the data from key {digest.hex()}') from e
-                except Exception as e:
-                    raise RuntimeError(f'An error occurred while loading the cache for "{digest.hex()}"') from e
+            contents = list(_unpack_mapping(index))
+            try:
+                return self.serializer.load(contents, self.storage.read), True
+            # either the data is corrupted or missing
+            except (DeserializationError, ReadError) as e:
+                raise StorageCorruption from e
+            except SerializerError as e:
+                raise SerializerError(f'Could not deserialize the data from key {digest.hex()}') from e
+            except Exception as e:
+                raise RuntimeError(f'An error occurred while loading the cache for "{digest.hex()}"') from e
 
         return None, False
 
     def _read(self, key: _PreparedKey):
         digest = key.digest
         value, exists = self._read_for_digest(digest)
         if exists:
             logger.info('Key %s found', digest)
             return value, True
 
         # the cache is empty, but we can try and restore it from an older version
         for version in reversed(PREVIOUS_VERSIONS):
             _, local_digest = _key_to_digest(self.algorithm, key.raw, version)
-            value, exists = self._read_for_digest(digest)
+            value, exists = self._read_for_digest(local_digest)
             if exists:
                 logger.info('Key %s found in previous version (%d). Updating', digest, version)
                 # and store it for faster access next time
                 self.write(key, value, error=False)
                 return value, True
 
         logger.info('Key %s not found', digest)
@@ -131,27 +118,26 @@
 
 def _key_to_digest(algorithm, key, version=None):
     pickled = dumps(key, version=version)
     digest = algorithm(pickled).digest()
     return pickled, digest
 
 
-@contextmanager
 def _unpack_mapping(path: Path):
     if path.is_file():
         with open(path, 'r') as file:
             try:
                 mapping = json.load(file)
             except json.JSONDecodeError as e:
                 raise StorageCorruption from e
 
-        with TemporaryDirectory() as temp:
-            temp = Path(temp)
-            for relative, content in mapping.items():
-                (temp / relative).parent.mkdir(parents=True, exist_ok=True)
-                (temp / relative).write_text(content)
-
-            yield temp
+            for k, v in mapping.items():
+                yield k, bytes.fromhex(v)
 
     else:
         # TODO: warn
-        yield path
+        for file in path.glob('**/*'):
+            if file.is_dir():
+                continue
+
+            relative = str(file.relative_to(path))
+            yield relative, bytes.fromhex(file.read_text())
```

### Comparing `tarn-0.6.0/tarn/tools/labels.py` & `tarn-0.7.0/tarn/tools/labels.py`

 * *Files identical despite different names*

### Comparing `tarn-0.6.0/tarn/tools/locker.py` & `tarn-0.7.0/tarn/tools/locker.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,28 +74,28 @@
 
     @classmethod
     def from_url(cls, url: str, prefix: AnyStr, expire: int):
         return cls(Redis.from_url(url), prefix=prefix, expire=expire)
 
     @contextmanager
     def read(self, key: Key) -> ContextManager[None]:
-        sleep_time = 0.1
+        sleep_time = 0.01
         sleep_iters = int(self._expire / sleep_time) or 1
         wait_for_true(self._start_reading, key, sleep_time, sleep_iters)
 
         try:
             yield
         finally:
             lock = self._safe_eval(self._stop_reading_script, 1, self._prefix + key)
         if lock != b'1':
             raise RuntimeError(f'The locker is in a wrong state ({lock}). Did it expire?')
 
     @contextmanager
     def write(self, key: Key) -> ContextManager[None]:
-        sleep_time = 0.1
+        sleep_time = 0.01
         sleep_iters = int(self._expire / sleep_time) or 1
         wait_for_true(self._start_writing, key, sleep_time, sleep_iters)
 
         try:
             yield
         finally:
             lock = self._safe_eval(self._stop_writing_script, 1, self._prefix + key)
```

### Comparing `tarn-0.6.0/tarn/tools/size.py` & `tarn-0.7.0/tarn/tools/size.py`

 * *Files identical despite different names*

### Comparing `tarn-0.6.0/tarn/tools/usage.py` & `tarn-0.7.0/tarn/tools/usage.py`

 * *Files identical despite different names*

### Comparing `tarn-0.6.0/tarn/utils.py` & `tarn-0.7.0/tarn/utils.py`

 * *Files identical despite different names*

### Comparing `tarn-0.6.0/tarn.egg-info/PKG-INFO` & `tarn-0.7.0/tarn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tarn
-Version: 0.6.0
+Version: 0.7.0
 Summary: A hashmap-based storage on local and remote disks
 Home-page: https://github.com/neuro-ml/tarn
 Author: Max
 Author-email: max@ira-labs.com
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/tarn/archive/v0.6.0.tar.gz
+Download-URL: https://github.com/neuro-ml/tarn/archive/v0.7.0.tar.gz
 Keywords: storage,cache,invalidation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tarn-0.6.0/tarn.egg-info/SOURCES.txt` & `tarn-0.7.0/tarn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

