# Comparing `tmp/readlog-1.1.9.tar.gz` & `tmp/readlog-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readlog-1.1.9.tar", last modified: Tue Jun 20 11:46:42 2023, max compression
+gzip compressed data, was "readlog-1.2.0.tar", last modified: Tue Jun 20 14:09:01 2023, max compression
```

## Comparing `readlog-1.1.9.tar` & `readlog-1.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 11:46:42.263453 readlog-1.1.9/
--rw-rw-rw-   0        0        0      128 2023-06-02 08:43:49.000000 readlog-1.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0      921 2023-06-20 11:46:42.262453 readlog-1.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      653 2023-06-20 11:46:06.000000 readlog-1.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 11:46:42.219982 readlog-1.1.9/demo/
--rw-rw-rw-   0        0        0   235181 2023-06-07 06:29:27.000000 readlog-1.1.9/demo/1_hydrate_dissociation_log.lammps
-drwxrwxrwx   0        0        0        0 2023-06-20 11:46:42.221982 readlog-1.1.9/demo/__pycache__/
--rw-rw-rw-   0        0        0     5413 2023-06-07 06:40:50.000000 readlog-1.1.9/demo/__pycache__/readlog.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2023-06-20 11:46:42.233539 readlog-1.1.9/demo/imgs/
--rw-rw-rw-   0        0        0   220194 2023-06-07 06:41:45.000000 readlog-1.1.9/demo/imgs/PotEng.png
--rw-rw-rw-   0        0        0   222242 2023-06-07 06:35:07.000000 readlog-1.1.9/demo/imgs/PotEng_incomplete.png
--rw-rw-rw-   0        0        0    80763 2023-06-20 10:44:42.000000 readlog-1.1.9/demo/log.lammps
--rw-rw-rw-   0        0        0    28861 2023-06-07 06:32:27.000000 readlog-1.1.9/demo/log_incomplete.lammps
--rw-rw-rw-   0        0        0     1272 2023-06-07 06:41:43.000000 readlog-1.1.9/demo/plot_themo.py
--rw-rw-rw-   0        0        0     4265 2023-06-20 11:43:31.000000 readlog-1.1.9/demo/readlog.py
--rw-rw-rw-   0        0        0       27 2023-06-20 07:38:09.000000 readlog-1.1.9/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 11:46:42.263453 readlog-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0      758 2023-06-20 11:44:03.000000 readlog-1.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 11:46:42.250452 readlog-1.1.9/src/
-drwxrwxrwx   0        0        0        0 2023-06-20 11:46:42.260453 readlog-1.1.9/src/readlog.egg-info/
--rw-rw-rw-   0        0        0      921 2023-06-20 11:46:41.000000 readlog-1.1.9/src/readlog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-06-20 11:46:42.000000 readlog-1.1.9/src/readlog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 11:46:41.000000 readlog-1.1.9/src/readlog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-20 11:46:41.000000 readlog-1.1.9/src/readlog.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-20 11:46:41.000000 readlog-1.1.9/src/readlog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4265 2023-06-20 11:43:31.000000 readlog-1.1.9/src/readlog.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:09:00.995926 readlog-1.2.0/
+-rw-rw-rw-   0        0        0      128 2023-06-02 08:43:49.000000 readlog-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      921 2023-06-20 14:09:00.994927 readlog-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      653 2023-06-20 11:46:06.000000 readlog-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 14:09:00.977882 readlog-1.2.0/demo/
+-rw-rw-rw-   0        0        0   235181 2023-06-07 06:29:27.000000 readlog-1.2.0/demo/1_hydrate_dissociation_log.lammps
+drwxrwxrwx   0        0        0        0 2023-06-20 14:09:00.978884 readlog-1.2.0/demo/__pycache__/
+-rw-rw-rw-   0        0        0     5413 2023-06-07 06:40:50.000000 readlog-1.2.0/demo/__pycache__/readlog.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2023-06-20 14:09:00.982882 readlog-1.2.0/demo/imgs/
+-rw-rw-rw-   0        0        0   220194 2023-06-07 06:41:45.000000 readlog-1.2.0/demo/imgs/PotEng.png
+-rw-rw-rw-   0        0        0   222242 2023-06-07 06:35:07.000000 readlog-1.2.0/demo/imgs/PotEng_incomplete.png
+-rw-rw-rw-   0        0        0    80763 2023-06-20 10:44:42.000000 readlog-1.2.0/demo/log.lammps
+-rw-rw-rw-   0        0        0    28861 2023-06-07 06:32:27.000000 readlog-1.2.0/demo/log_incomplete.lammps
+-rw-rw-rw-   0        0        0     1272 2023-06-07 06:41:43.000000 readlog-1.2.0/demo/plot_themo.py
+-rw-rw-rw-   0        0        0     4291 2023-06-20 14:08:39.000000 readlog-1.2.0/demo/readlog.py
+-rw-rw-rw-   0        0        0       27 2023-06-20 07:38:09.000000 readlog-1.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 14:09:00.995926 readlog-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      758 2023-06-20 13:35:22.000000 readlog-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:09:00.984883 readlog-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-20 14:09:00.992926 readlog-1.2.0/src/readlog.egg-info/
+-rw-rw-rw-   0        0        0      921 2023-06-20 14:09:00.000000 readlog-1.2.0/src/readlog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-06-20 14:09:00.000000 readlog-1.2.0/src/readlog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 14:09:00.000000 readlog-1.2.0/src/readlog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-20 14:09:00.000000 readlog-1.2.0/src/readlog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-20 14:09:00.000000 readlog-1.2.0/src/readlog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4291 2023-06-20 14:08:39.000000 readlog-1.2.0/src/readlog.py
```

### Comparing `readlog-1.1.9/PKG-INFO` & `readlog-1.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readlog
-Version: 1.1.9
+Version: 1.2.0
 Summary: Read themo info from lammps output file or log file
 Home-page: https://github.com/eastsheng/readlog
 Author: CHENDONGSHENG
 Author-email: eastsheng@hotmail.com
 Description-Content-Type: text/markdown
 
 ## readlog
```

### Comparing `readlog-1.1.9/README.md` & `readlog-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `readlog-1.1.9/demo/1_hydrate_dissociation_log.lammps` & `readlog-1.2.0/demo/1_hydrate_dissociation_log.lammps`

 * *Files identical despite different names*

### Comparing `readlog-1.1.9/demo/__pycache__/readlog.cpython-311.pyc` & `readlog-1.2.0/demo/__pycache__/readlog.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `readlog-1.1.9/demo/imgs/PotEng.png` & `readlog-1.2.0/demo/imgs/PotEng.png`

 * *Files identical despite different names*

### Comparing `readlog-1.1.9/demo/imgs/PotEng_incomplete.png` & `readlog-1.2.0/demo/imgs/PotEng_incomplete.png`

 * *Files identical despite different names*

### Comparing `readlog-1.1.9/demo/log.lammps` & `readlog-1.2.0/demo/log.lammps`

 * *Files identical despite different names*

### Comparing `readlog-1.1.9/demo/log_incomplete.lammps` & `readlog-1.2.0/demo/log_incomplete.lammps`

 * *Files identical despite different names*

### Comparing `readlog-1.1.9/demo/plot_themo.py` & `readlog-1.2.0/demo/plot_themo.py`

 * *Files identical despite different names*

### Comparing `readlog-1.1.9/demo/readlog.py` & `readlog-1.2.0/demo/readlog.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,32 +2,35 @@
 read lammps log file for some thermo data
 """
 import numpy as np
 import pandas as pd
 # from pathlib import Path
 import matplotlib.pyplot as plt
 
+version = "1.2.0"
+
 def print_readlog():
     cloud = [
-	"	                        _  _          	   	 ",
-	"	 _ __   ___   __ _   __| || |  ___    __ _ 	 ",
-	"	| '__| / _ \ / _` | / _` || | / _ \  / _` |	 ",
-	"	| |   |  __/| (_| || (_| || || (_) || (_| |	 ",
-	"	|_|    \___| \__,_| \__,_||_| \___/  \__, |	 ",
-	"	                                     |___/ 	 ",
-	"	                                     	 	 ", 
+	"                        _  _               ",
+	" _ __   ___   __ _   __| || |  ___    __ _ ",
+	"| '__| / _ \ / _` | / _` || | / _ \  / _` |",
+	"| |   |  __/| (_| || (_| || || (_) || (_| |",
+	"|_|    \___| \__,_| \__,_||_| \___/  \__, |",
+	"                                     |___/ ",
     ]
-
-    print(51*"*")
-    print(51*"*")
+    print("\n")
+    print(22*"- ")
+    print(22*". ")
     for line in cloud:
-        print(2*"*"+line+2*"*")
+        print(line)
+    print('@readlog-'+version,", Good Luck!")
+    print(22*". ")
+    print(22*"- ")
+    return None
 
-    print(51*"*")
-    print(51*"*")
 print_readlog()
 
 
 class ReadLog(object):
 	"""docstring for ClassName"""
 	def __init__(self, logfile):
 		super(ReadLog, self).__init__()
```

### Comparing `readlog-1.1.9/setup.py` & `readlog-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 with open("requirements.txt","r") as f:
     required = f.read().splitlines()
 
 
 setup(
 name         = 'readlog',
-version      = '1.1.9',
+version      = '1.2.0',
 py_modules   = ['readlog'],
 author       = 'CHENDONGSHENG',
 author_email = 'eastsheng@hotmail.com',
 packages=find_packages('src'),
 package_dir={'': 'src'},
 install_requires=required,
 url          = 'https://github.com/eastsheng/readlog',
```

### Comparing `readlog-1.1.9/src/readlog.egg-info/PKG-INFO` & `readlog-1.2.0/src/readlog.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readlog
-Version: 1.1.9
+Version: 1.2.0
 Summary: Read themo info from lammps output file or log file
 Home-page: https://github.com/eastsheng/readlog
 Author: CHENDONGSHENG
 Author-email: eastsheng@hotmail.com
 Description-Content-Type: text/markdown
 
 ## readlog
```

### Comparing `readlog-1.1.9/src/readlog.py` & `readlog-1.2.0/src/readlog.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,32 +2,35 @@
 read lammps log file for some thermo data
 """
 import numpy as np
 import pandas as pd
 # from pathlib import Path
 import matplotlib.pyplot as plt
 
+version = "1.2.0"
+
 def print_readlog():
     cloud = [
-	"	                        _  _          	   	 ",
-	"	 _ __   ___   __ _   __| || |  ___    __ _ 	 ",
-	"	| '__| / _ \ / _` | / _` || | / _ \  / _` |	 ",
-	"	| |   |  __/| (_| || (_| || || (_) || (_| |	 ",
-	"	|_|    \___| \__,_| \__,_||_| \___/  \__, |	 ",
-	"	                                     |___/ 	 ",
-	"	                                     	 	 ", 
+	"                        _  _               ",
+	" _ __   ___   __ _   __| || |  ___    __ _ ",
+	"| '__| / _ \ / _` | / _` || | / _ \  / _` |",
+	"| |   |  __/| (_| || (_| || || (_) || (_| |",
+	"|_|    \___| \__,_| \__,_||_| \___/  \__, |",
+	"                                     |___/ ",
     ]
-
-    print(51*"*")
-    print(51*"*")
+    print("\n")
+    print(22*"- ")
+    print(22*". ")
     for line in cloud:
-        print(2*"*"+line+2*"*")
+        print(line)
+    print('@readlog-'+version,", Good Luck!")
+    print(22*". ")
+    print(22*"- ")
+    return None
 
-    print(51*"*")
-    print(51*"*")
 print_readlog()
 
 
 class ReadLog(object):
 	"""docstring for ClassName"""
 	def __init__(self, logfile):
 		super(ReadLog, self).__init__()
```

