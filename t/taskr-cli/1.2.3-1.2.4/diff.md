# Comparing `tmp/taskr_cli-1.2.3-py3-none-any.whl.zip` & `tmp/taskr_cli-1.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 14699 bytes, number of entries: 13
+Zip file size: 14838 bytes, number of entries: 13
 -rw-r--r--  2.0 unx       61 b- defN 23-Jan-18 04:37 taskr/__init__.py
 -rw-r--r--  2.0 unx       78 b- defN 23-Jan-18 04:37 taskr/__version__.py
 -rw-r--r--  2.0 unx     1995 b- defN 23-Mar-05 18:49 taskr/cli.py
 -rw-r--r--  2.0 unx     2709 b- defN 23-Jan-18 04:37 taskr/runners.py
 -rw-r--r--  2.0 unx     8853 b- defN 23-Mar-05 18:49 taskr/taskr.py
 -rw-r--r--  2.0 unx     1950 b- defN 23-Jan-18 04:37 taskr/template.py
--rw-r--r--  2.0 unx     5462 b- defN 23-Jun-19 19:39 taskr/utils.py
--rw-r--r--  2.0 unx     1069 b- defN 23-Jun-19 19:40 taskr_cli-1.2.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     8860 b- defN 23-Jun-19 19:40 taskr_cli-1.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-19 19:40 taskr_cli-1.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       41 b- defN 23-Jun-19 19:40 taskr_cli-1.2.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-19 19:40 taskr_cli-1.2.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      997 b- defN 23-Jun-19 19:40 taskr_cli-1.2.3.dist-info/RECORD
-13 files, 32173 bytes uncompressed, 13047 bytes compressed:  59.4%
+-rw-r--r--  2.0 unx     5454 b- defN 23-Jun-20 04:11 taskr/utils.py
+-rw-r--r--  2.0 unx     1069 b- defN 23-Jun-20 04:12 taskr_cli-1.2.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9159 b- defN 23-Jun-20 04:12 taskr_cli-1.2.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 04:12 taskr_cli-1.2.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       41 b- defN 23-Jun-20 04:12 taskr_cli-1.2.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-20 04:12 taskr_cli-1.2.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      997 b- defN 23-Jun-20 04:12 taskr_cli-1.2.4.dist-info/RECORD
+13 files, 32464 bytes uncompressed, 13186 bytes compressed:  59.4%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: taskr/template.py
 Comment: 
 
 Filename: taskr/utils.py
 Comment: 
 
-Filename: taskr_cli-1.2.3.dist-info/LICENSE
+Filename: taskr_cli-1.2.4.dist-info/LICENSE
 Comment: 
 
-Filename: taskr_cli-1.2.3.dist-info/METADATA
+Filename: taskr_cli-1.2.4.dist-info/METADATA
 Comment: 
 
-Filename: taskr_cli-1.2.3.dist-info/WHEEL
+Filename: taskr_cli-1.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: taskr_cli-1.2.3.dist-info/entry_points.txt
+Filename: taskr_cli-1.2.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: taskr_cli-1.2.3.dist-info/top_level.txt
+Filename: taskr_cli-1.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: taskr_cli-1.2.3.dist-info/RECORD
+Filename: taskr_cli-1.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## taskr/utils.py

```diff
@@ -33,14 +33,16 @@
         return False
 
 
 def cleanCompiles() -> bool:
     """
     Finds compiled (.pyc) files and removes them recursively from the base
     of the project, where 'tasks.py' is
+
+    TODO: Build list first, then delete them for better debugging
     """
     try:
         for root, dirs, files in os.walk(".", topdown=False):
             if "__pycache__" in dirs:
                 _removeFolder("__pycache__", root)
             for name in files:
                 if ".pyc" in name:
@@ -80,49 +82,46 @@
 
     return ret
 
 
 def _bump(version: str) -> str:
     """
     Internal function for easier testing
-    TODO - use regex maybe - seems overkill
+    TODO - Maybe use regex?
     """
     cleaned = version.replace("'", "").replace(",", "").replace('"', "")  # "1.2.3"
     verSplit = cleaned.split(".")  # ["1", "2", "3"]
     oldMinor = verSplit[2].strip()  # "3"
     newMinor = str(int(oldMinor) + 1)  # "4"
     newVersion = f"{verSplit[0]}.{verSplit[1]}.{newMinor}"  # "1.2.4
     return newVersion
 
 
 def bumpVersion(
     version: Optional[str] = None,
-    filename: Optional[str] = None,
-    variable: Optional[str] = None,
+    filename: str = "setup.py",
+    variable: str = "version",
 ) -> bool:
     """
-    Bumps the minor version in setup.py by 1, or the given argument
-    May support other files in the future
+    Bumps the minor version in setup.py by 1
 
+    If a version is give, overwrites the version instead
     If a path is provided, looks for 'version' in the file
     If a variable is also provided, it' replaces that variable name
     """
-    if not filename:
-        filename = "setup.py"
-    if not variable:
-        variable = "version"
+
     addComma = False
 
     if not os.path.exists(filename):
         raise FileExistsError(f"Can't find {filename}")
 
+    # Modify the copy first, and replace if nothing breaks
     with open(filename, "r") as fd:
         temp = fd.read()
 
-
     try:
         out = []
         for line in temp.split("\n"):
             var = line.split("=")[0].strip()
             if var == variable:
                 toReplace = line.split("=")[1].lstrip()
                 if "," in toReplace:
```

## Comparing `taskr_cli-1.2.3.dist-info/LICENSE` & `taskr_cli-1.2.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `taskr_cli-1.2.3.dist-info/METADATA` & `taskr_cli-1.2.4.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskr-cli
-Version: 1.2.3
+Version: 1.2.4
 Summary: A language agnostic make-like tool meant for python projects
 Author-email: Kyle Peasley <Kyle.Peasley@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Kyle Peasley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,23 +38,23 @@
 # Taskr
 [![PyPI version](https://badge.fury.io/py/taskr-cli.svg)](https://badge.fury.io/py/taskr-cli)
 
 A magical, zero dependency, easy to use task runner with an original name. Inspired by [Mage](https://github.com/magefile/mage), a make-like tool for go. Made for python projects, but usable for any.
 
 All that's needed is a tasks.py file.
 
-A few highlights
+A few highlights:
 
 - Basically make(1) without a build system
 - Zero dependencies
 - Auto load environment variable files
-- Easily pass arguments
-- Auto generated cli docs
+- Easily pass arguments to tasks from the command line
+- Auto generated cli documentation
 - Usable in any subdirectory of your project
-- Built functions to easily run system commands inside venvs
+- Built in functions to easily run system commands inside virtual environments
 - Built in helper functions for python development
 
 ## Installing
 
 ```shell
 pip install taskr-cli
 ```
@@ -134,15 +134,15 @@
 ```python
 from taskr import runners
 
 DEFAULT = "test"
 VENV_REQUIRED = True
 ENVS = "dev.env"
 
-# Run tests, and passed dev.env vars when running
+# Run tests, and passed dev.env vars when running 'taskr' in the cli
 def test
   runners.run("python -m pytest tests/")
 ```
 
 ## Helpful functions for running tasks
 
 A few task running methods are provided for system running tasks. Taskr expects task functions to return either  ```True``` (The task was successful) for ```False```it failed. To determine if a subprocess/system call was successful or not, taskr looks at the return code of the called program. 0 is success, anything else fails.
@@ -255,36 +255,37 @@
 
 ```shell
 taskr start timeout=60
 ```
 
 ## Utilities
 
-There are a few utility functions included, mostly for python package development. 
+There are a few utility functions included, mostly for python package development. These are not the main focus of the package and more will probably not be added, rather spun out into a different package
 
 ```python
 from taskr import utils
 
 # Removes dist/build folders
 utils.cleanBuilds()
 
-# Remove compiled files and folders
+# Remove compiled files and folders (.pyc, __pycache__)
 utils.cleanCompiles()
 
 # In a venv or not
 utils.inVenv()
 
 # Transforms an ENV file into a dict
-utils.readEnvFile(filename)
+utils.readEnvFile(filename = None)
 
 # Bumps setup.py's version number by 0.0.1, or replaces it with argument
-utils.bumpVersion(version=None):
+utils.bumpVersion(version = None, variable = "version", filename = "setup.py"):
 
 # Adds `export TASKR_DIR=CWD' to your VENV activation, so
 # you can use taskr from any location in the VENV (e.g. sub directories)
+# Probably don't use this
 utils.addTaskrToEnv()
 ```
 
 ## Developing
 
 This project uses pipenv. Make sure it's installed. Then call
 ```shell
```

## Comparing `taskr_cli-1.2.3.dist-info/RECORD` & `taskr_cli-1.2.4.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 taskr/__init__.py,sha256=HYyXgZ4SQ_RWUTv3TM7IBKVz0_daPGS1MdmjNkBVHRs,61
 taskr/__version__.py,sha256=UpLk4osKJTqB53nr1gFoPa9lNzecaM2WpL_-opMzswY,78
 taskr/cli.py,sha256=OXD0e-vNJ_5HGyN8blfP5iKLY6dc8kxmgrKr-G57JwM,1995
 taskr/runners.py,sha256=dQxljblRsvDWtE7s_9nzeNAMTj_xNEk3cR7pP9SVCMI,2709
 taskr/taskr.py,sha256=Y1uUr6JN-auSfB6X2l8m2sRnn17mgmF5mKinYVr95VU,8853
 taskr/template.py,sha256=uzT2HlbPJcL-OlYaxrpm5mmIbS2RnaypxV55_p3u3io,1950
-taskr/utils.py,sha256=CDDQ8DRZOA0aHn0fR7r9cOuJDGqhA7rVpGvDECe6j9A,5462
-taskr_cli-1.2.3.dist-info/LICENSE,sha256=r-dZ3nX2dvIGBQgIGllf9ITlGguIqi8OqBm-x6oWS7U,1069
-taskr_cli-1.2.3.dist-info/METADATA,sha256=FXswInDtUZwU8AktgOaZHGsG-MV6EiXFINAVMsFx2qY,8860
-taskr_cli-1.2.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-taskr_cli-1.2.3.dist-info/entry_points.txt,sha256=Mc2MUGWo4v25gpWXBZVzox8NklMvXZQt352WLhs9oiA,41
-taskr_cli-1.2.3.dist-info/top_level.txt,sha256=nUs61tNfbfharkZ-iKd9ugpnblA61ctB_cj3yljwmPs,6
-taskr_cli-1.2.3.dist-info/RECORD,,
+taskr/utils.py,sha256=RQOP159B14eL0wCWNrzVpA0MvXUtwro7Ccox-dtbC2Q,5454
+taskr_cli-1.2.4.dist-info/LICENSE,sha256=r-dZ3nX2dvIGBQgIGllf9ITlGguIqi8OqBm-x6oWS7U,1069
+taskr_cli-1.2.4.dist-info/METADATA,sha256=SzwZNbmUU4YcMB8ypdUNP0YsGDCKPNeU9gqwSXpR2zA,9159
+taskr_cli-1.2.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+taskr_cli-1.2.4.dist-info/entry_points.txt,sha256=Mc2MUGWo4v25gpWXBZVzox8NklMvXZQt352WLhs9oiA,41
+taskr_cli-1.2.4.dist-info/top_level.txt,sha256=nUs61tNfbfharkZ-iKd9ugpnblA61ctB_cj3yljwmPs,6
+taskr_cli-1.2.4.dist-info/RECORD,,
```

