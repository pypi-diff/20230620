# Comparing `tmp/gxabm-2.7.0.tar.gz` & `tmp/gxabm-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gxabm-2.7.0.tar", last modified: Tue Jun 13 14:44:32 2023, max compression
+gzip compressed data, was "gxabm-2.7.1.tar", last modified: Tue Jun 20 16:58:13 2023, max compression
```

## Comparing `gxabm-2.7.0.tar` & `gxabm-2.7.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-13 14:44:32.728587 gxabm-2.7.0/
--rw-r--r--   0 suderman   (502) staff       (20)       42 2022-03-07 12:56:12.000000 gxabm-2.7.0/MANIFEST.in
--rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-06-13 14:44:32.728415 gxabm-2.7.0/PKG-INFO
--rw-r--r--   0 suderman   (502) staff       (20)    16395 2022-03-22 19:06:33.000000 gxabm-2.7.0/README.md
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-13 14:44:32.720556 gxabm-2.7.0/abm/
--rw-r--r--   0 suderman   (502) staff       (20)        6 2023-06-13 14:43:37.000000 gxabm-2.7.0/abm/VERSION
--rw-r--r--   0 suderman   (502) staff       (20)      290 2022-03-07 12:56:12.000000 gxabm-2.7.0/abm/__init__.py
--rw-r--r--   0 suderman   (502) staff       (20)     8374 2023-05-01 01:43:54.000000 gxabm-2.7.0/abm/__main__.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-13 14:44:32.725123 gxabm-2.7.0/abm/lib/
--rw-r--r--   0 suderman   (502) staff       (20)      447 2022-03-07 12:56:12.000000 gxabm-2.7.0/abm/lib/__init__.py
--rw-r--r--   0 suderman   (502) staff       (20)    19882 2023-06-13 14:43:19.000000 gxabm-2.7.0/abm/lib/benchmark.py
--rw-r--r--   0 suderman   (502) staff       (20)     7812 2022-10-19 17:36:24.000000 gxabm-2.7.0/abm/lib/cloudlaunch.py
--rw-r--r--   0 suderman   (502) staff       (20)     9068 2023-06-13 14:43:19.000000 gxabm-2.7.0/abm/lib/common.py
--rw-r--r--   0 suderman   (502) staff       (20)     5433 2022-10-19 17:36:24.000000 gxabm-2.7.0/abm/lib/config.py
--rw-r--r--   0 suderman   (502) staff       (20)     7902 2023-06-13 14:43:19.000000 gxabm-2.7.0/abm/lib/dataset.py
--rw-r--r--   0 suderman   (502) staff       (20)     7661 2023-04-29 03:35:40.000000 gxabm-2.7.0/abm/lib/experiment.py
--rw-r--r--   0 suderman   (502) staff       (20)      883 2022-03-07 12:56:12.000000 gxabm-2.7.0/abm/lib/folder.py
--rw-r--r--   0 suderman   (502) staff       (20)     4185 2022-10-27 02:48:01.000000 gxabm-2.7.0/abm/lib/helm.py
--rw-r--r--   0 suderman   (502) staff       (20)      282 2022-03-07 12:56:12.000000 gxabm-2.7.0/abm/lib/histories.yml
--rw-r--r--   0 suderman   (502) staff       (20)    11467 2023-06-13 14:43:19.000000 gxabm-2.7.0/abm/lib/history.py
--rw-r--r--   0 suderman   (502) staff       (20)     1217 2023-05-01 01:43:54.000000 gxabm-2.7.0/abm/lib/invocation.py
--rw-r--r--   0 suderman   (502) staff       (20)     5037 2023-06-13 14:43:19.000000 gxabm-2.7.0/abm/lib/job.py
--rw-r--r--   0 suderman   (502) staff       (20)     1264 2022-03-07 12:56:12.000000 gxabm-2.7.0/abm/lib/kubectl.py
--rw-r--r--   0 suderman   (502) staff       (20)     2518 2023-04-24 20:08:21.000000 gxabm-2.7.0/abm/lib/library.py
--rw-r--r--   0 suderman   (502) staff       (20)    12347 2023-06-13 14:43:19.000000 gxabm-2.7.0/abm/lib/menu.yml
--rw-r--r--   0 suderman   (502) staff       (20)     3480 2022-10-19 17:36:24.000000 gxabm-2.7.0/abm/lib/users.py
--rw-r--r--   0 suderman   (502) staff       (20)     7817 2023-05-01 01:43:54.000000 gxabm-2.7.0/abm/lib/workflow.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-13 14:44:32.726089 gxabm-2.7.0/gxabm.egg-info/
--rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-06-13 14:44:32.000000 gxabm-2.7.0/gxabm.egg-info/PKG-INFO
--rw-r--r--   0 suderman   (502) staff       (20)      691 2023-06-13 14:44:32.000000 gxabm-2.7.0/gxabm.egg-info/SOURCES.txt
--rw-r--r--   0 suderman   (502) staff       (20)        1 2023-06-13 14:44:32.000000 gxabm-2.7.0/gxabm.egg-info/dependency_links.txt
--rw-r--r--   0 suderman   (502) staff       (20)       49 2023-06-13 14:44:32.000000 gxabm-2.7.0/gxabm.egg-info/entry_points.txt
--rw-r--r--   0 suderman   (502) staff       (20)       48 2023-06-13 14:44:32.000000 gxabm-2.7.0/gxabm.egg-info/requires.txt
--rw-r--r--   0 suderman   (502) staff       (20)        9 2023-06-13 14:44:32.000000 gxabm-2.7.0/gxabm.egg-info/top_level.txt
--rw-r--r--   0 suderman   (502) staff       (20)       38 2023-06-13 14:44:32.728637 gxabm-2.7.0/setup.cfg
--rw-r--r--   0 suderman   (502) staff       (20)     1036 2022-10-19 17:36:24.000000 gxabm-2.7.0/setup.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-13 14:44:32.727845 gxabm-2.7.0/test/
--rw-r--r--   0 suderman   (502) staff       (20)      147 2022-03-07 12:56:12.000000 gxabm-2.7.0/test/__init__.py
--rwxr-xr-x   0 suderman   (502) staff       (20)     8684 2022-12-23 17:29:52.000000 gxabm-2.7.0/test/check_tools.py
--rw-r--r--   0 suderman   (502) staff       (20)     2160 2022-10-27 04:03:53.000000 gxabm-2.7.0/test/metrics.py
--rw-r--r--   0 suderman   (502) staff       (20)      298 2022-03-07 12:56:12.000000 gxabm-2.7.0/test/test_environments.py
--rw-r--r--   0 suderman   (502) staff       (20)      718 2023-06-04 14:10:38.000000 gxabm-2.7.0/test/workflow.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-20 16:58:13.709203 gxabm-2.7.1/
+-rw-r--r--   0 suderman   (502) staff       (20)       42 2022-03-07 12:56:12.000000 gxabm-2.7.1/MANIFEST.in
+-rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-06-20 16:58:13.708827 gxabm-2.7.1/PKG-INFO
+-rw-r--r--   0 suderman   (502) staff       (20)    16395 2022-03-22 19:06:33.000000 gxabm-2.7.1/README.md
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-20 16:58:13.699522 gxabm-2.7.1/abm/
+-rw-r--r--   0 suderman   (502) staff       (20)        6 2023-06-20 16:57:31.000000 gxabm-2.7.1/abm/VERSION
+-rw-r--r--   0 suderman   (502) staff       (20)      290 2022-03-07 12:56:12.000000 gxabm-2.7.1/abm/__init__.py
+-rw-r--r--   0 suderman   (502) staff       (20)     8374 2023-05-01 01:43:54.000000 gxabm-2.7.1/abm/__main__.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-20 16:58:13.705106 gxabm-2.7.1/abm/lib/
+-rw-r--r--   0 suderman   (502) staff       (20)      447 2022-03-07 12:56:12.000000 gxabm-2.7.1/abm/lib/__init__.py
+-rw-r--r--   0 suderman   (502) staff       (20)    19882 2023-06-13 14:43:19.000000 gxabm-2.7.1/abm/lib/benchmark.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7812 2022-10-19 17:36:24.000000 gxabm-2.7.1/abm/lib/cloudlaunch.py
+-rw-r--r--   0 suderman   (502) staff       (20)     9068 2023-06-13 14:43:19.000000 gxabm-2.7.1/abm/lib/common.py
+-rw-r--r--   0 suderman   (502) staff       (20)     5433 2022-10-19 17:36:24.000000 gxabm-2.7.1/abm/lib/config.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7902 2023-06-13 14:43:19.000000 gxabm-2.7.1/abm/lib/dataset.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7661 2023-04-29 03:35:40.000000 gxabm-2.7.1/abm/lib/experiment.py
+-rw-r--r--   0 suderman   (502) staff       (20)      883 2022-03-07 12:56:12.000000 gxabm-2.7.1/abm/lib/folder.py
+-rw-r--r--   0 suderman   (502) staff       (20)     4185 2022-10-27 02:48:01.000000 gxabm-2.7.1/abm/lib/helm.py
+-rw-r--r--   0 suderman   (502) staff       (20)      282 2022-03-07 12:56:12.000000 gxabm-2.7.1/abm/lib/histories.yml
+-rw-r--r--   0 suderman   (502) staff       (20)    11467 2023-06-13 14:43:19.000000 gxabm-2.7.1/abm/lib/history.py
+-rw-r--r--   0 suderman   (502) staff       (20)     1217 2023-05-01 01:43:54.000000 gxabm-2.7.1/abm/lib/invocation.py
+-rw-r--r--   0 suderman   (502) staff       (20)     5049 2023-06-20 16:56:58.000000 gxabm-2.7.1/abm/lib/job.py
+-rw-r--r--   0 suderman   (502) staff       (20)     1264 2022-03-07 12:56:12.000000 gxabm-2.7.1/abm/lib/kubectl.py
+-rw-r--r--   0 suderman   (502) staff       (20)     2518 2023-04-24 20:08:21.000000 gxabm-2.7.1/abm/lib/library.py
+-rw-r--r--   0 suderman   (502) staff       (20)    12347 2023-06-13 14:43:19.000000 gxabm-2.7.1/abm/lib/menu.yml
+-rw-r--r--   0 suderman   (502) staff       (20)     3480 2022-10-19 17:36:24.000000 gxabm-2.7.1/abm/lib/users.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7817 2023-05-01 01:43:54.000000 gxabm-2.7.1/abm/lib/workflow.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-20 16:58:13.706230 gxabm-2.7.1/gxabm.egg-info/
+-rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-06-20 16:58:13.000000 gxabm-2.7.1/gxabm.egg-info/PKG-INFO
+-rw-r--r--   0 suderman   (502) staff       (20)      691 2023-06-20 16:58:13.000000 gxabm-2.7.1/gxabm.egg-info/SOURCES.txt
+-rw-r--r--   0 suderman   (502) staff       (20)        1 2023-06-20 16:58:13.000000 gxabm-2.7.1/gxabm.egg-info/dependency_links.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       49 2023-06-20 16:58:13.000000 gxabm-2.7.1/gxabm.egg-info/entry_points.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       48 2023-06-20 16:58:13.000000 gxabm-2.7.1/gxabm.egg-info/requires.txt
+-rw-r--r--   0 suderman   (502) staff       (20)        9 2023-06-20 16:58:13.000000 gxabm-2.7.1/gxabm.egg-info/top_level.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       38 2023-06-20 16:58:13.709335 gxabm-2.7.1/setup.cfg
+-rw-r--r--   0 suderman   (502) staff       (20)     1036 2022-10-19 17:36:24.000000 gxabm-2.7.1/setup.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-06-20 16:58:13.707894 gxabm-2.7.1/test/
+-rw-r--r--   0 suderman   (502) staff       (20)      147 2022-03-07 12:56:12.000000 gxabm-2.7.1/test/__init__.py
+-rwxr-xr-x   0 suderman   (502) staff       (20)     8684 2022-12-23 17:29:52.000000 gxabm-2.7.1/test/check_tools.py
+-rw-r--r--   0 suderman   (502) staff       (20)     2160 2022-10-27 04:03:53.000000 gxabm-2.7.1/test/metrics.py
+-rw-r--r--   0 suderman   (502) staff       (20)      298 2022-03-07 12:56:12.000000 gxabm-2.7.1/test/test_environments.py
+-rw-r--r--   0 suderman   (502) staff       (20)      718 2023-06-04 14:10:38.000000 gxabm-2.7.1/test/workflow.py
```

### Comparing `gxabm-2.7.0/PKG-INFO` & `gxabm-2.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gxabm
-Version: 2.7.0
+Version: 2.7.1
 Summary: Opinionated Benchmarking Automatation in Galaxy
 Home-page: https://github.com/galaxyproject/gxabm
 Author: Keith Suderman
 Author-email: suderman@jhu.edu
 License: MIT
 Description: # Automated Benchmarking in Galaxy
         An opinionated Python Bioblend script for automating benchmarking tasks in Galaxy.
```

### Comparing `gxabm-2.7.0/README.md` & `gxabm-2.7.1/README.md`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.0/abm/__main__.py` & `gxabm-2.7.1/abm/__main__.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.0/abm/lib/benchmark.py` & `gxabm-2.7.1/abm/lib/benchmark.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.0/abm/lib/cloudlaunch.py` & `gxabm-2.7.1/abm/lib/cloudlaunch.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.0/abm/lib/common.py` & `gxabm-2.7.1/abm/lib/common.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.0/abm/lib/config.py` & `gxabm-2.7.1/abm/lib/config.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.0/abm/lib/dataset.py` & `gxabm-2.7.1/abm/lib/dataset.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.0/abm/lib/experiment.py` & `gxabm-2.7.1/abm/lib/experiment.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.0/abm/lib/folder.py` & `gxabm-2.7.1/abm/lib/folder.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.0/abm/lib/helm.py` & `gxabm-2.7.1/abm/lib/helm.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.0/abm/lib/history.py` & `gxabm-2.7.1/abm/lib/history.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.0/abm/lib/invocation.py` & `gxabm-2.7.1/abm/lib/invocation.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.0/abm/lib/job.py` & `gxabm-2.7.1/abm/lib/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,17 +31,17 @@
     gi = connect(context)
     if log_state:
         log.debug(f"Getting jobs with state {state}")
     else:
         log.debug("Getting job list")
     if history_id:
         history_id = find_history(gi, history_id)
-    if history_id is None:
-        print("ERROR: No such history")
-        return
+        if history_id is None:
+            print("ERROR: No such history")
+            return
     job_list = gi.jobs.get_jobs(state=state, history_id=history_id)
     log.debug(f"Iterating over job list with {len(job_list)} items")
     for job in job_list:
         print(f"{job['id']}\t{job['state']}\t{job['update_time']}\t{job['tool_id']}")
 
 
 def show(context: Context, args: list):
```

### Comparing `gxabm-2.7.0/abm/lib/kubectl.py` & `gxabm-2.7.1/abm/lib/kubectl.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.0/abm/lib/library.py` & `gxabm-2.7.1/abm/lib/library.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.0/abm/lib/menu.yml` & `gxabm-2.7.1/abm/lib/menu.yml`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.0/abm/lib/users.py` & `gxabm-2.7.1/abm/lib/users.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.0/abm/lib/workflow.py` & `gxabm-2.7.1/abm/lib/workflow.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.0/gxabm.egg-info/PKG-INFO` & `gxabm-2.7.1/gxabm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gxabm
-Version: 2.7.0
+Version: 2.7.1
 Summary: Opinionated Benchmarking Automatation in Galaxy
 Home-page: https://github.com/galaxyproject/gxabm
 Author: Keith Suderman
 Author-email: suderman@jhu.edu
 License: MIT
 Description: # Automated Benchmarking in Galaxy
         An opinionated Python Bioblend script for automating benchmarking tasks in Galaxy.
```

### Comparing `gxabm-2.7.0/gxabm.egg-info/SOURCES.txt` & `gxabm-2.7.1/gxabm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.0/setup.py` & `gxabm-2.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.0/test/check_tools.py` & `gxabm-2.7.1/test/check_tools.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.0/test/metrics.py` & `gxabm-2.7.1/test/metrics.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.7.0/test/workflow.py` & `gxabm-2.7.1/test/workflow.py`

 * *Files identical despite different names*

