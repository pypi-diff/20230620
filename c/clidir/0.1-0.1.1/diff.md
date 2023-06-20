# Comparing `tmp/clidir-0.1.tar.gz` & `tmp/clidir-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clidir-0.1.tar", last modified: Tue Jun 20 14:01:23 2023, max compression
+gzip compressed data, was "clidir-0.1.1.tar", last modified: Tue Jun 20 14:25:36 2023, max compression
```

## Comparing `clidir-0.1.tar` & `clidir-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 isaacb     (502) staff       (20)        0 2023-06-20 14:01:23.020844 clidir-0.1/
--rw-r--r--   0 isaacb     (502) staff       (20)     1079 2023-06-20 13:58:56.000000 clidir-0.1/LICENSE
--rw-r--r--   0 isaacb     (502) staff       (20)     3031 2023-06-20 14:01:23.020715 clidir-0.1/PKG-INFO
--rw-r--r--   0 isaacb     (502) staff       (20)     2588 2023-06-20 13:58:56.000000 clidir-0.1/README.md
--rw-r--r--   0 isaacb     (502) staff       (20)      521 2023-06-20 13:58:56.000000 clidir-0.1/pyproject.toml
--rw-r--r--   0 isaacb     (502) staff       (20)       38 2023-06-20 14:01:23.020891 clidir-0.1/setup.cfg
-drwxr-xr-x   0 isaacb     (502) staff       (20)        0 2023-06-20 14:01:23.019890 clidir-0.1/src/
--rw-r--r--   0 isaacb     (502) staff       (20)        0 2023-06-20 13:58:56.000000 clidir-0.1/src/__init__.py
--rw-r--r--   0 isaacb     (502) staff       (20)      603 2023-06-20 13:58:56.000000 clidir-0.1/src/arg_parser.py
-drwxr-xr-x   0 isaacb     (502) staff       (20)        0 2023-06-20 14:01:23.020533 clidir-0.1/src/clidir.egg-info/
--rw-r--r--   0 isaacb     (502) staff       (20)     3031 2023-06-20 14:01:23.000000 clidir-0.1/src/clidir.egg-info/PKG-INFO
--rw-r--r--   0 isaacb     (502) staff       (20)      250 2023-06-20 14:01:23.000000 clidir-0.1/src/clidir.egg-info/SOURCES.txt
--rw-r--r--   0 isaacb     (502) staff       (20)        1 2023-06-20 14:01:23.000000 clidir-0.1/src/clidir.egg-info/dependency_links.txt
--rw-r--r--   0 isaacb     (502) staff       (20)       47 2023-06-20 14:01:23.000000 clidir-0.1/src/clidir.egg-info/top_level.txt
--rw-r--r--   0 isaacb     (502) staff       (20)      830 2023-06-20 13:58:56.000000 clidir-0.1/src/clidir.py
--rw-r--r--   0 isaacb     (502) staff       (20)      511 2023-06-20 13:58:56.000000 clidir-0.1/src/command_loader.py
--rw-r--r--   0 isaacb     (502) staff       (20)     1024 2023-06-20 13:58:56.000000 clidir-0.1/src/help.py
+drwxr-xr-x   0 isaacb     (502) staff       (20)        0 2023-06-20 14:25:36.538418 clidir-0.1.1/
+-rw-r--r--   0 isaacb     (502) staff       (20)     1079 2023-06-20 13:58:56.000000 clidir-0.1.1/LICENSE
+-rw-r--r--   0 isaacb     (502) staff       (20)     2464 2023-06-20 14:25:36.538287 clidir-0.1.1/PKG-INFO
+-rw-r--r--   0 isaacb     (502) staff       (20)     2019 2023-06-20 14:19:57.000000 clidir-0.1.1/README.md
+-rw-r--r--   0 isaacb     (502) staff       (20)      523 2023-06-20 14:24:36.000000 clidir-0.1.1/pyproject.toml
+-rw-r--r--   0 isaacb     (502) staff       (20)       38 2023-06-20 14:25:36.538463 clidir-0.1.1/setup.cfg
+drwxr-xr-x   0 isaacb     (502) staff       (20)        0 2023-06-20 14:25:36.537458 clidir-0.1.1/src/
+-rw-r--r--   0 isaacb     (502) staff       (20)        0 2023-06-20 13:58:56.000000 clidir-0.1.1/src/__init__.py
+-rw-r--r--   0 isaacb     (502) staff       (20)      603 2023-06-20 13:58:56.000000 clidir-0.1.1/src/arg_parser.py
+drwxr-xr-x   0 isaacb     (502) staff       (20)        0 2023-06-20 14:25:36.538071 clidir-0.1.1/src/clidir.egg-info/
+-rw-r--r--   0 isaacb     (502) staff       (20)     2464 2023-06-20 14:25:36.000000 clidir-0.1.1/src/clidir.egg-info/PKG-INFO
+-rw-r--r--   0 isaacb     (502) staff       (20)      250 2023-06-20 14:25:36.000000 clidir-0.1.1/src/clidir.egg-info/SOURCES.txt
+-rw-r--r--   0 isaacb     (502) staff       (20)        1 2023-06-20 14:25:36.000000 clidir-0.1.1/src/clidir.egg-info/dependency_links.txt
+-rw-r--r--   0 isaacb     (502) staff       (20)       47 2023-06-20 14:25:36.000000 clidir-0.1.1/src/clidir.egg-info/top_level.txt
+-rw-r--r--   0 isaacb     (502) staff       (20)      830 2023-06-20 13:58:56.000000 clidir-0.1.1/src/clidir.py
+-rw-r--r--   0 isaacb     (502) staff       (20)      511 2023-06-20 13:58:56.000000 clidir-0.1.1/src/command_loader.py
+-rw-r--r--   0 isaacb     (502) staff       (20)     1024 2023-06-20 13:58:56.000000 clidir-0.1.1/src/help.py
```

### Comparing `clidir-0.1/LICENSE` & `clidir-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clidir-0.1/PKG-INFO` & `clidir-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clidir
-Version: 0.1
+Version: 0.1.1
 Summary: A tiny Python library to easily create CLI applications with sub commands
 Author: Isaac Benitez
 Project-URL: Homepage, https://github.com/isacben/clidir
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -43,15 +43,19 @@
     parser.add_argument("url")
     
     # the rest of the implementation
 ```
 
 ## Installation
 
-TODO
+Install this tool using `pip`:
+
+```
+pip install clidir
+```
 
 ## Usage
 
 1. Create a `main.py` file with the following code:
 
 ```python
 import sys
@@ -91,34 +95,7 @@
 
 5. Test the execution of the command:
 
 ```shell
 % python3 main.py remote add      
 running the add command...
 ```
-
-## Command Execution Flow
-
-Below is a diagram that outlines at a high level the process that occurs every time a user executes a command through clidir.
-
-```mermaid
-flowchart TD
-    subgraph "CLI app"
-        a1[Get arguments]-->a2[Call clidir]
-    end
-
-    a2-->A
-
-    subgraph "clidir"
-        A[Parse arguments]-->B[Look for commands in the filesystem]
-        B-->C[Import the command files as modules]
-        C-->D{First argument}
-        D-->|Command| H[Run command]
-        D-->|Topic or empty| I[Display topic help]
-    end
-    
-    H-->J
-
-    subgraph Command Module
-        J["Execute the command"]
-    end
-```
```

### Comparing `clidir-0.1/README.md` & `clidir-0.1.1/src/clidir.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: clidir
+Version: 0.1.1
+Summary: A tiny Python library to easily create CLI applications with sub commands
+Author: Isaac Benitez
+Project-URL: Homepage, https://github.com/isacben/clidir
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # clidir
 
 Create CLI applications with sub commands easily.
 
 ## Description
 
 Even simple CLI applications usually require sub commands. For example, `git` has `git remote add`, where *remote* and *add* are sub commands. Doing this with `argparse` or even with more developer friendly libraries can be challenging.
@@ -30,15 +43,19 @@
     parser.add_argument("url")
     
     # the rest of the implementation
 ```
 
 ## Installation
 
-TODO
+Install this tool using `pip`:
+
+```
+pip install clidir
+```
 
 ## Usage
 
 1. Create a `main.py` file with the following code:
 
 ```python
 import sys
@@ -78,34 +95,7 @@
 
 5. Test the execution of the command:
 
 ```shell
 % python3 main.py remote add      
 running the add command...
 ```
-
-## Command Execution Flow
-
-Below is a diagram that outlines at a high level the process that occurs every time a user executes a command through clidir.
-
-```mermaid
-flowchart TD
-    subgraph "CLI app"
-        a1[Get arguments]-->a2[Call clidir]
-    end
-
-    a2-->A
-
-    subgraph "clidir"
-        A[Parse arguments]-->B[Look for commands in the filesystem]
-        B-->C[Import the command files as modules]
-        C-->D{First argument}
-        D-->|Command| H[Run command]
-        D-->|Topic or empty| I[Display topic help]
-    end
-    
-    H-->J
-
-    subgraph Command Module
-        J["Execute the command"]
-    end
-```
```

### Comparing `clidir-0.1/pyproject.toml` & `clidir-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clidir"
-version = "0.1"
+version = "0.1.1"
 authors = [
   { name="Isaac Benitez"},
 ]
 description = "A tiny Python library to easily create CLI applications with sub commands"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `clidir-0.1/src/arg_parser.py` & `clidir-0.1.1/src/arg_parser.py`

 * *Files identical despite different names*

### Comparing `clidir-0.1/src/clidir.py` & `clidir-0.1.1/src/clidir.py`

 * *Files identical despite different names*

### Comparing `clidir-0.1/src/help.py` & `clidir-0.1.1/src/help.py`

 * *Files identical despite different names*

