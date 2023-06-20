# Comparing `tmp/tomato-cooker-0.2.0.tar.gz` & `tmp/tomato-cooker-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomato-cooker-0.2.0.tar", last modified: Tue Jun 20 09:56:32 2023, max compression
+gzip compressed data, was "tomato-cooker-0.2.1.tar", last modified: Tue Jun 20 10:36:44 2023, max compression
```

## Comparing `tomato-cooker-0.2.0.tar` & `tomato-cooker-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:56:32.978687 tomato-cooker-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-20 09:56:19.000000 tomato-cooker-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-20 09:56:32.974687 tomato-cooker-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-20 09:56:19.000000 tomato-cooker-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 09:56:32.978687 tomato-cooker-0.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1557 2023-06-20 09:56:19.000000 tomato-cooker-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:56:32.974687 tomato-cooker-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-06-20 09:56:19.000000 tomato-cooker-0.2.0/tests/test_grill.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:56:32.974687 tomato-cooker-0.2.0/tomato_cooker/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-20 09:56:19.000000 tomato-cooker-0.2.0/tomato_cooker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:56:32.974687 tomato-cooker-0.2.0/tomato_cooker/grill/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 09:56:19.000000 tomato-cooker-0.2.0/tomato_cooker/grill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-20 09:56:19.000000 tomato-cooker-0.2.0/tomato_cooker/grill/grill.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:56:32.974687 tomato-cooker-0.2.0/tomato_cooker/models/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-20 09:56:19.000000 tomato-cooker-0.2.0/tomato_cooker/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-20 09:56:19.000000 tomato-cooker-0.2.0/tomato_cooker/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:56:32.974687 tomato-cooker-0.2.0/tomato_cooker/models/tomatic/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 09:56:19.000000 tomato-cooker-0.2.0/tomato_cooker/models/tomatic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-06-20 09:56:19.000000 tomato-cooker-0.2.0/tomato_cooker/models/tomatic/phone_grill.mzn
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-20 09:56:19.000000 tomato-cooker-0.2.0/tomato_cooker/models/tomatic/tomatic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:56:32.974687 tomato-cooker-0.2.0/tomato_cooker/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-20 09:56:19.000000 tomato-cooker-0.2.0/tomato_cooker/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:56:32.974687 tomato-cooker-0.2.0/tomato_cooker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-20 09:56:32.000000 tomato-cooker-0.2.0/tomato_cooker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-20 09:56:32.000000 tomato-cooker-0.2.0/tomato_cooker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:56:32.000000 tomato-cooker-0.2.0/tomato_cooker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-20 09:56:32.000000 tomato-cooker-0.2.0/tomato_cooker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 09:56:32.000000 tomato-cooker-0.2.0/tomato_cooker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:56:32.000000 tomato-cooker-0.2.0/tomato_cooker.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:36:44.421661 tomato-cooker-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-20 10:36:34.000000 tomato-cooker-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-20 10:36:44.421661 tomato-cooker-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-20 10:36:34.000000 tomato-cooker-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 10:36:44.421661 tomato-cooker-0.2.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1557 2023-06-20 10:36:34.000000 tomato-cooker-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:36:44.417661 tomato-cooker-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-06-20 10:36:34.000000 tomato-cooker-0.2.1/tests/test_grill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:36:44.417661 tomato-cooker-0.2.1/tomato_cooker/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-20 10:36:34.000000 tomato-cooker-0.2.1/tomato_cooker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:36:44.417661 tomato-cooker-0.2.1/tomato_cooker/grill/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 10:36:34.000000 tomato-cooker-0.2.1/tomato_cooker/grill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-20 10:36:34.000000 tomato-cooker-0.2.1/tomato_cooker/grill/grill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:36:44.417661 tomato-cooker-0.2.1/tomato_cooker/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-20 10:36:34.000000 tomato-cooker-0.2.1/tomato_cooker/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-20 10:36:34.000000 tomato-cooker-0.2.1/tomato_cooker/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:36:44.421661 tomato-cooker-0.2.1/tomato_cooker/models/tomatic/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 10:36:34.000000 tomato-cooker-0.2.1/tomato_cooker/models/tomatic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-06-20 10:36:34.000000 tomato-cooker-0.2.1/tomato_cooker/models/tomatic/phone_grill.mzn
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-20 10:36:34.000000 tomato-cooker-0.2.1/tomato_cooker/models/tomatic/tomatic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:36:44.421661 tomato-cooker-0.2.1/tomato_cooker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-20 10:36:34.000000 tomato-cooker-0.2.1/tomato_cooker/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:36:44.417661 tomato-cooker-0.2.1/tomato_cooker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-20 10:36:44.000000 tomato-cooker-0.2.1/tomato_cooker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-20 10:36:44.000000 tomato-cooker-0.2.1/tomato_cooker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 10:36:44.000000 tomato-cooker-0.2.1/tomato_cooker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-20 10:36:44.000000 tomato-cooker-0.2.1/tomato_cooker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 10:36:44.000000 tomato-cooker-0.2.1/tomato_cooker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 10:36:44.000000 tomato-cooker-0.2.1/tomato_cooker.egg-info/zip-safe
```

### Comparing `tomato-cooker-0.2.0/LICENSE` & `tomato-cooker-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tomato-cooker-0.2.0/PKG-INFO` & `tomato-cooker-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomato-cooker
-Version: 0.2.0
+Version: 0.2.1
 Summary: Minizinc problem solver
 Home-page: https://github.com/Som-Energia/Som-Minizinc
 Author: Som Energia SCCL
 Author-email: info@somenergia.coop
 License: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tomato-cooker-0.2.0/README.md` & `tomato-cooker-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tomato-cooker-0.2.0/setup.py` & `tomato-cooker-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `tomato-cooker-0.2.0/tests/test_grill.py` & `tomato-cooker-0.2.1/tests/test_grill.py`

 * *Files identical despite different names*

### Comparing `tomato-cooker-0.2.0/tomato_cooker/grill/grill.py` & `tomato-cooker-0.2.1/tomato_cooker/grill/grill.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,26 +7,27 @@
 
 
 class GrillTomatoCooker:
     def __init__(self, model_path: str, solvers: list) -> None:
         self.model = minizinc.Model(model_path)
         self.solvers = solvers
 
-    async def cook(self, problem_instance: TomaticProblem) -> Any:
+    async def cook(self, problem_instance: TomaticProblem, deterministic=False) -> Any:
         result = []
         for attr, value in problem_instance._asdict().items():
             self.model[attr] = value
 
         tasks = set()
         for solver_name in self.solvers:
             # Create an instance of the model for every solver
             solver = minizinc.Solver.lookup(solver_name)
             inst = minizinc.Instance(solver, self.model)
 
-            task = asyncio.create_task(inst.solve_async())
+            seed = 0 if deterministic else None
+            task = asyncio.create_task(inst.solve_async(random_seed = seed))
             task.solver = solver.name
             tasks.add(task)
 
         # Wait on the first task to finish and cancel the other tasks
         done, pending = await asyncio.wait(tasks, return_when=asyncio.FIRST_COMPLETED)
         if done:
             result = done.pop().result()
```

### Comparing `tomato-cooker-0.2.0/tomato_cooker/models/tomatic/phone_grill.mzn` & `tomato-cooker-0.2.1/tomato_cooker/models/tomatic/phone_grill.mzn`

 * *Files identical despite different names*

### Comparing `tomato-cooker-0.2.0/tomato_cooker/utils/__init__.py` & `tomato-cooker-0.2.1/tomato_cooker/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tomato-cooker-0.2.0/tomato_cooker.egg-info/PKG-INFO` & `tomato-cooker-0.2.1/tomato_cooker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomato-cooker
-Version: 0.2.0
+Version: 0.2.1
 Summary: Minizinc problem solver
 Home-page: https://github.com/Som-Energia/Som-Minizinc
 Author: Som Energia SCCL
 Author-email: info@somenergia.coop
 License: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tomato-cooker-0.2.0/tomato_cooker.egg-info/SOURCES.txt` & `tomato-cooker-0.2.1/tomato_cooker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

