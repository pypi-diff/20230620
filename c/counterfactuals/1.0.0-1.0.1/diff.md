# Comparing `tmp/counterfactuals-1.0.0.tar.gz` & `tmp/counterfactuals-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "counterfactuals-1.0.0.tar", last modified: Mon Mar 27 10:02:44 2023, max compression
+gzip compressed data, was "counterfactuals-1.0.1.tar", last modified: Tue Jun 20 18:21:55 2023, max compression
```

## Comparing `counterfactuals-1.0.0.tar` & `counterfactuals-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 rkiesel   (1718) groot     (1000)        0 2023-03-27 10:02:44.227755 counterfactuals-1.0.0/
--rw-r--r--   0 rkiesel   (1718) groot     (1000)     1064 2023-03-27 09:36:49.000000 counterfactuals-1.0.0/LICENCE
--rw-r--r--   0 rkiesel   (1718) groot     (1000)     6039 2023-03-27 10:02:44.225458 counterfactuals-1.0.0/PKG-INFO
--rw-r--r--   0 rkiesel   (1718) groot     (1000)     5139 2023-03-27 09:56:04.000000 counterfactuals-1.0.0/README.md
-drwxr-xr-x   0 rkiesel   (1718) groot     (1000)        0 2023-03-27 10:02:44.197558 counterfactuals-1.0.0/counterfactuals/
--rw-r--r--   0 rkiesel   (1718) groot     (1000)       16 2022-12-06 18:59:35.000000 counterfactuals-1.0.0/counterfactuals/__init__.py
--rw-r--r--   0 rkiesel   (1718) groot     (1000)    32513 2023-03-27 09:07:43.000000 counterfactuals-1.0.0/counterfactuals/counterfactualprogram.py
--rw-r--r--   0 rkiesel   (1718) groot     (1000)     7644 2023-03-27 09:59:57.000000 counterfactuals-1.0.0/counterfactuals/main.py
-drwxr-xr-x   0 rkiesel   (1718) groot     (1000)        0 2023-03-27 10:02:44.221490 counterfactuals-1.0.0/counterfactuals.egg-info/
--rw-r--r--   0 rkiesel   (1718) groot     (1000)     6039 2023-03-27 10:02:44.000000 counterfactuals-1.0.0/counterfactuals.egg-info/PKG-INFO
--rw-r--r--   0 rkiesel   (1718) groot     (1000)      355 2023-03-27 10:02:44.000000 counterfactuals-1.0.0/counterfactuals.egg-info/SOURCES.txt
--rw-r--r--   0 rkiesel   (1718) groot     (1000)        1 2023-03-27 10:02:44.000000 counterfactuals-1.0.0/counterfactuals.egg-info/dependency_links.txt
--rw-r--r--   0 rkiesel   (1718) groot     (1000)       53 2023-03-27 10:02:44.000000 counterfactuals-1.0.0/counterfactuals.egg-info/entry_points.txt
--rw-r--r--   0 rkiesel   (1718) groot     (1000)       12 2023-03-27 10:02:44.000000 counterfactuals-1.0.0/counterfactuals.egg-info/requires.txt
--rw-r--r--   0 rkiesel   (1718) groot     (1000)       16 2023-03-27 10:02:44.000000 counterfactuals-1.0.0/counterfactuals.egg-info/top_level.txt
--rw-r--r--   0 rkiesel   (1718) groot     (1000)       38 2023-03-27 10:02:44.228353 counterfactuals-1.0.0/setup.cfg
--rw-r--r--   0 rkiesel   (1718) groot     (1000)     8531 2023-03-27 10:01:52.000000 counterfactuals-1.0.0/setup.py
+drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2023-06-20 18:21:55.392525 counterfactuals-1.0.1/
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     1064 2023-06-20 17:55:10.000000 counterfactuals-1.0.1/LICENCE
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     6039 2023-06-20 18:21:55.388525 counterfactuals-1.0.1/PKG-INFO
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     5139 2023-06-20 17:55:10.000000 counterfactuals-1.0.1/README.md
+drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2023-06-20 18:21:55.388525 counterfactuals-1.0.1/counterfactuals/
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)       16 2023-06-20 17:55:10.000000 counterfactuals-1.0.1/counterfactuals/__init__.py
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)    32513 2023-06-20 17:55:10.000000 counterfactuals-1.0.1/counterfactuals/counterfactualprogram.py
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     7642 2023-06-20 18:18:24.000000 counterfactuals-1.0.1/counterfactuals/main.py
+drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2023-06-20 18:21:55.388525 counterfactuals-1.0.1/counterfactuals.egg-info/
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     6039 2023-06-20 18:21:55.000000 counterfactuals-1.0.1/counterfactuals.egg-info/PKG-INFO
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)      355 2023-06-20 18:21:55.000000 counterfactuals-1.0.1/counterfactuals.egg-info/SOURCES.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)        1 2023-06-20 18:21:55.000000 counterfactuals-1.0.1/counterfactuals.egg-info/dependency_links.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)       53 2023-06-20 18:21:55.000000 counterfactuals-1.0.1/counterfactuals.egg-info/entry_points.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)       12 2023-06-20 18:21:55.000000 counterfactuals-1.0.1/counterfactuals.egg-info/requires.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)       16 2023-06-20 18:21:55.000000 counterfactuals-1.0.1/counterfactuals.egg-info/top_level.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)       38 2023-06-20 18:21:55.392525 counterfactuals-1.0.1/setup.cfg
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     8531 2023-06-20 18:20:17.000000 counterfactuals-1.0.1/setup.py
```

### Comparing `counterfactuals-1.0.0/LICENCE` & `counterfactuals-1.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `counterfactuals-1.0.0/PKG-INFO` & `counterfactuals-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: counterfactuals
-Version: 1.0.0
+Version: 1.0.1
 Summary: A solver for Counterfactual Inference.
 Author: R. Kiesel
 Author-email: rafael.kiesel@tuwien.ac.at
 License: MIT
 Keywords: probabilistic,logic programming,counterfactual reasoning
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `counterfactuals-1.0.0/README.md` & `counterfactuals-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `counterfactuals-1.0.0/counterfactuals/counterfactualprogram.py` & `counterfactuals-1.0.1/counterfactuals/counterfactualprogram.py`

 * *Files identical despite different names*

### Comparing `counterfactuals-1.0.0/counterfactuals/main.py` & `counterfactuals-1.0.1/counterfactuals/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,20 +26,20 @@
 WhatIf [-e .] [-ds .] [-dt .] [-k .] [-v .] [-h] [<INPUT-FILES>]
     --knowlege          -k  COMPILER    set the knowledge compiler to COMPILER:
                                         * sharpsat-td       : uses a compilation version of sharpsat-td (default)
                                         * d4                : uses the (slightly modified) d4 compiler. 
                                         * c2d               : uses the c2d compiler. 
                                         * miniC2D           : uses the miniC2D compiler. 
                                         * pysdd             : uses the PySDD compiler. 
-    --evidence          -e  NAME,PHASE  add evidence NAME:
-                                        * the evidence is negated if PHASE is `True`.
-                                        * the evidence is not negated if PHASE is `False`.
-    --intervene         -i  NAME,PHASE  intervene on NAME:
-                                        * the intervention is negative if PHASE is `True`.
-                                        * the intervention is not negative if PHASE is `False`.
+    --evidence          -e  NAME,VALUE  add evidence NAME:
+                                        * the evidence is not negated if VALUE is `True`.
+                                        * the evidence is negated if VALUE is `False`.
+    --intervene         -i  NAME,VALUE  intervene on NAME:
+                                        * the intervention is not negated if VALUE is `True`.
+                                        * the intervention is negated if VALUE is `False`.
     --query             -q  NAME        query for the probability of NAME.
     --decos             -ds SOLVER      set the solver that computes tree decompositions to SOLVER:
                                         * flow-cutter       : uses flow_cutter_pace17 (default)
     --decot             -dt SECONDS     set the timeout for computing tree decompositions to SECONDS (default: 1)
     --verbosity         -v  VERBOSITY   set the logging level to VERBOSITY:
                                         * debug             : print everything
                                         * info              : print as usual
@@ -85,39 +85,39 @@
                 if sys.argv[2] != "c2d" and sys.argv[2] != "miniC2D" and sys.argv[2] != "sharpsat-td" and sys.argv[2] != "d4" and sys.argv[2] != "pysdd":
                     logger.error("  Unknown knowledge compiler: " + sys.argv[2])
                     exit(-1)
                 del sys.argv[1:3]
             elif sys.argv[1] == "-e" or sys.argv[1] == "--evidence":
                 last_comma = sys.argv[2].rfind(",")
                 if last_comma == -1:
-                    logger.error(f" Invalid evidence string {sys.argv[2]}.\nExpected a string of the form `name,phase`, \
-                        where name is the name of an atom and phase is either `True` or `False`")
+                    logger.error(f" Invalid evidence string {sys.argv[2]}.\nExpected a string of the form `name,value`, \
+                        where name is the name of an atom and value is either `True` or `False`")
                 name = sys.argv[2][:last_comma]
-                phase = sys.argv[2][last_comma + 1:]
-                if phase != "True" and phase != "False":
-                    logger.error(f" Invalid evidence string {sys.argv[2]}.\nExpected a string of the form `name,phase`, \
-                        where name is the name of an atom and phase is either `True` or `False`")
-                phase = True if phase == "True" else False
+                value = sys.argv[2][last_comma + 1:]
+                if value != "True" and value != "False":
+                    logger.error(f" Invalid evidence string {sys.argv[2]}.\nExpected a string of the form `name,value`, \
+                        where name is the name of an atom and value is either `True` or `False`")
+                phase = False if value == "True" else True
                 if name in evidence:
-                    logger.warning(f"   Double specification of evidence for atom {name}. Using the last specified phase {phase}.")
+                    logger.warning(f"   Double specification of evidence for atom {name}. Using the last specified value {value}.")
                 evidence[name] = phase
                 del sys.argv[1:3]
             elif sys.argv[1] == "-i" or sys.argv[1] == "--intervene":
                 last_comma = sys.argv[2].rfind(",")
                 if last_comma == -1:
-                    logger.error(f" Invalid intervention string {sys.argv[2]}.\nExpected a string of the form `name,phase`, \
-                        where name is the name of an atom and phase is either `True` or `False`")
+                    logger.error(f" Invalid intervention string {sys.argv[2]}.\nExpected a string of the form `name,value`, \
+                        where name is the name of an atom and value is either `True` or `False`")
                 name = sys.argv[2][:last_comma]
-                phase = sys.argv[2][last_comma + 1:]
-                if phase != "True" and phase != "False":
-                    logger.error(f" Invalid intervention string {sys.argv[2]}.\nExpected a string of the form `name,phase`, \
-                        where name is the name of an atom and phase is either `True` or `False`")
-                phase = True if phase == "True" else False
+                value = sys.argv[2][last_comma + 1:]
+                if value != "True" and value != "False":
+                    logger.error(f" Invalid intervention string {sys.argv[2]}.\nExpected a string of the form `name,value`, \
+                        where name is the name of an atom and value is either `True` or `False`")
+                phase = False if value == "True" else True
                 if name in interventions:
-                    logger.warning(f"   Double specification of intervention for atom {name}. Using the last specified phase {phase}.")
+                    logger.warning(f"   Double specification of intervention for atom {name}. Using the last specified value {value}.")
                 interventions[name] = phase
                 del sys.argv[1:3]
             elif sys.argv[1] == "-q" or sys.argv[1] == "--query":
                 query = sys.argv[2]
                 queries.append(query)
                 del sys.argv[1:3]
             elif sys.argv[1] == "-h" or sys.argv[1] == "--help":
```

### Comparing `counterfactuals-1.0.0/counterfactuals.egg-info/PKG-INFO` & `counterfactuals-1.0.1/counterfactuals.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: counterfactuals
-Version: 1.0.0
+Version: 1.0.1
 Summary: A solver for Counterfactual Inference.
 Author: R. Kiesel
 Author-email: rafael.kiesel@tuwien.ac.at
 License: MIT
 Keywords: probabilistic,logic programming,counterfactual reasoning
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `counterfactuals-1.0.0/setup.py` & `counterfactuals-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version='1.0.0',  # Required
+    version='1.0.1',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='A solver for Counterfactual Inference.',  # Optional
 
     # This is an optional longer description of your project that represents
```

