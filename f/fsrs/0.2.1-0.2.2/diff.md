# Comparing `tmp/fsrs-0.2.1.tar.gz` & `tmp/fsrs-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs-0.2.1.tar", last modified: Mon Jun 12 06:06:41 2023, max compression
+gzip compressed data, was "fsrs-0.2.2.tar", last modified: Tue Jun 20 08:33:55 2023, max compression
```

## Comparing `fsrs-0.2.1.tar` & `fsrs-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:06:41.140491 fsrs-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-12 06:06:19.000000 fsrs-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-12 06:06:41.140491 fsrs-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-12 06:06:19.000000 fsrs-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-12 06:06:19.000000 fsrs-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 06:06:41.140491 fsrs-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-12 06:06:19.000000 fsrs-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:06:41.140491 fsrs-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:06:41.140491 fsrs-0.2.1/src/fsrs/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-12 06:06:19.000000 fsrs-0.2.1/src/fsrs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-06-12 06:06:19.000000 fsrs-0.2.1/src/fsrs/fsrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-06-12 06:06:19.000000 fsrs-0.2.1/src/fsrs/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:06:41.140491 fsrs-0.2.1/src/fsrs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-12 06:06:41.000000 fsrs-0.2.1/src/fsrs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-12 06:06:41.000000 fsrs-0.2.1/src/fsrs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 06:06:41.000000 fsrs-0.2.1/src/fsrs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-12 06:06:41.000000 fsrs-0.2.1/src/fsrs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 06:06:41.140491 fsrs-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-12 06:06:19.000000 fsrs-0.2.1/tests/test_fsrs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:33:55.552683 fsrs-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-20 08:33:38.000000 fsrs-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-20 08:33:55.552683 fsrs-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-20 08:33:38.000000 fsrs-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-20 08:33:38.000000 fsrs-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 08:33:55.552683 fsrs-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 08:33:38.000000 fsrs-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:33:55.548683 fsrs-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:33:55.552683 fsrs-0.2.2/src/fsrs/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-20 08:33:38.000000 fsrs-0.2.2/src/fsrs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-06-20 08:33:38.000000 fsrs-0.2.2/src/fsrs/fsrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-06-20 08:33:38.000000 fsrs-0.2.2/src/fsrs/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:33:55.552683 fsrs-0.2.2/src/fsrs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-20 08:33:55.000000 fsrs-0.2.2/src/fsrs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-20 08:33:55.000000 fsrs-0.2.2/src/fsrs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 08:33:55.000000 fsrs-0.2.2/src/fsrs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-20 08:33:55.000000 fsrs-0.2.2/src/fsrs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:33:55.552683 fsrs-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-20 08:33:38.000000 fsrs-0.2.2/tests/test_fsrs.py
```

### Comparing `fsrs-0.2.1/LICENSE` & `fsrs-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fsrs-0.2.1/PKG-INFO` & `fsrs-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsrs
-Version: 0.2.1
+Version: 0.2.2
 Summary: Free Spaced Repetition Scheduler
 Author-email: Jarrett Ye <jarrett.ye@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Open Spaced Repetition
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fsrs-0.2.1/README.md` & `fsrs-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `fsrs-0.2.1/pyproject.toml` & `fsrs-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fsrs"
-version = "0.2.1"
+version = "0.2.2"
 description = "Free Spaced Repetition Scheduler"
 readme = "README.md"
 authors = [{ name = "Jarrett Ye", email = "jarrett.ye@outlook.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

### Comparing `fsrs-0.2.1/src/fsrs/fsrs.py` & `fsrs-0.2.2/src/fsrs/fsrs.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,16 +72,16 @@
     def init_stability(self, r: int) -> float:
         return max(self.p.w[0] + self.p.w[1] * r, 0.1)
 
     def init_difficulty(self, r: int) -> float:
         return min(max(self.p.w[2] + self.p.w[3] * (r - 2), 1), 10)
 
     def next_interval(self, s: float) -> int:
-        State.New_interval = s * math.log(self.p.request_retention) / math.log(0.9)
-        return min(max(round(State.New_interval), 1), self.p.maximum_interval)
+        new_interval = s * math.log(self.p.request_retention) / math.log(0.9)
+        return min(max(round(new_interval), 1), self.p.maximum_interval)
 
     def next_difficulty(self, d: float, r: int) -> float:
         next_d = d + self.p.w[4] * (r - 2)
         return min(max(self.mean_reversion(self.p.w[2], next_d), 1), 10)
 
     def mean_reversion(self, init: float, current: float) -> float:
         return self.p.w[5] * init + (1 - self.p.w[5]) * current
```

### Comparing `fsrs-0.2.1/src/fsrs/models.py` & `fsrs-0.2.2/src/fsrs/models.py`

 * *Files identical despite different names*

### Comparing `fsrs-0.2.1/src/fsrs.egg-info/PKG-INFO` & `fsrs-0.2.2/src/fsrs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsrs
-Version: 0.2.1
+Version: 0.2.2
 Summary: Free Spaced Repetition Scheduler
 Author-email: Jarrett Ye <jarrett.ye@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Open Spaced Repetition
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `fsrs-0.2.1/tests/test_fsrs.py` & `fsrs-0.2.2/tests/test_fsrs.py`

 * *Files identical despite different names*

