# Comparing `tmp/fx-bin-0.5.0.tar.gz` & `tmp/fx-bin-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fx-bin-0.5.0.tar", last modified: Sat Feb 19 11:38:02 2022, max compression
+gzip compressed data, was "fx-bin-0.6.0.tar", last modified: Tue Jun 20 15:51:04 2023, max compression
```

## Comparing `fx-bin-0.5.0.tar` & `fx-bin-0.6.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-19 11:38:02.043853 fx-bin-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     3559 2022-02-19 11:37:56.000000 fx-bin-0.5.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-02-19 11:37:56.000000 fx-bin-0.5.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-02-19 11:37:56.000000 fx-bin-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      758 2022-02-19 11:38:02.043853 fx-bin-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-02-19 11:37:56.000000 fx-bin-0.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-19 11:38:02.043853 fx-bin-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-02-19 11:37:56.000000 fx-bin-0.5.0/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (121)     4845 2022-02-19 11:37:56.000000 fx-bin-0.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-02-19 11:37:56.000000 fx-bin-0.5.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-02-19 11:37:56.000000 fx-bin-0.5.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-02-19 11:37:56.000000 fx-bin-0.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1146 2022-02-19 11:37:56.000000 fx-bin-0.5.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      771 2022-02-19 11:37:56.000000 fx-bin-0.5.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-02-19 11:37:56.000000 fx-bin-0.5.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-02-19 11:37:56.000000 fx-bin-0.5.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-19 11:38:02.043853 fx-bin-0.5.0/fx_bin/
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-02-19 11:37:56.000000 fx-bin-0.5.0/fx_bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-02-19 11:37:56.000000 fx-bin-0.5.0/fx_bin/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1870 2022-02-19 11:37:56.000000 fx-bin-0.5.0/fx_bin/files.py
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-02-19 11:37:56.000000 fx-bin-0.5.0/fx_bin/find_files.py
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-02-19 11:37:56.000000 fx-bin-0.5.0/fx_bin/lib.py
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-02-19 11:37:56.000000 fx-bin-0.5.0/fx_bin/pd.py
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-02-19 11:37:56.000000 fx-bin-0.5.0/fx_bin/py_fx_bin.py
--rw-r--r--   0 runner    (1001) docker     (121)      738 2022-02-19 11:37:56.000000 fx-bin-0.5.0/fx_bin/replace.py
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-02-19 11:37:56.000000 fx-bin-0.5.0/fx_bin/run_upgrade_program.py
--rw-r--r--   0 runner    (1001) docker     (121)     2039 2022-02-19 11:37:56.000000 fx-bin-0.5.0/fx_bin/size.py
--rw-r--r--   0 runner    (1001) docker     (121)    11740 2022-02-19 11:37:56.000000 fx-bin-0.5.0/fx_bin/upload_server.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-19 11:38:02.043853 fx-bin-0.5.0/fx_bin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      758 2022-02-19 11:38:01.000000 fx-bin-0.5.0/fx_bin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      675 2022-02-19 11:38:02.000000 fx-bin-0.5.0/fx_bin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-19 11:38:01.000000 fx-bin-0.5.0/fx_bin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-02-19 11:38:01.000000 fx-bin-0.5.0/fx_bin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-19 11:38:01.000000 fx-bin-0.5.0/fx_bin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-02-19 11:38:01.000000 fx-bin-0.5.0/fx_bin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-02-19 11:38:01.000000 fx-bin-0.5.0/fx_bin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-02-19 11:38:02.043853 fx-bin-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1541 2022-02-19 11:37:56.000000 fx-bin-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-19 11:38:02.043853 fx-bin-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-19 11:37:56.000000 fx-bin-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      890 2022-02-19 11:37:56.000000 fx-bin-0.5.0/tests/test_py_fx_bin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:04.164736 fx-bin-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-20 15:50:59.000000 fx-bin-0.6.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 15:50:59.000000 fx-bin-0.6.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-20 15:50:59.000000 fx-bin-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-20 15:51:04.164736 fx-bin-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-20 15:50:59.000000 fx-bin-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:04.160736 fx-bin-0.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-20 15:50:59.000000 fx-bin-0.6.0/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4845 2023-06-20 15:50:59.000000 fx-bin-0.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 15:50:59.000000 fx-bin-0.6.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 15:50:59.000000 fx-bin-0.6.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-20 15:50:59.000000 fx-bin-0.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-20 15:50:59.000000 fx-bin-0.6.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-20 15:50:59.000000 fx-bin-0.6.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-20 15:50:59.000000 fx-bin-0.6.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-20 15:50:59.000000 fx-bin-0.6.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:04.160736 fx-bin-0.6.0/fx_bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-20 15:50:59.000000 fx-bin-0.6.0/fx_bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-20 15:50:59.000000 fx-bin-0.6.0/fx_bin/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-20 15:50:59.000000 fx-bin-0.6.0/fx_bin/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-20 15:50:59.000000 fx-bin-0.6.0/fx_bin/find_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-20 15:50:59.000000 fx-bin-0.6.0/fx_bin/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-20 15:50:59.000000 fx-bin-0.6.0/fx_bin/pd.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-20 15:50:59.000000 fx-bin-0.6.0/fx_bin/py_fx_bin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-20 15:50:59.000000 fx-bin-0.6.0/fx_bin/replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-20 15:50:59.000000 fx-bin-0.6.0/fx_bin/run_upgrade_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-20 15:50:59.000000 fx-bin-0.6.0/fx_bin/size.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12017 2023-06-20 15:50:59.000000 fx-bin-0.6.0/fx_bin/upload_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:04.160736 fx-bin-0.6.0/fx_bin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-20 15:51:04.000000 fx-bin-0.6.0/fx_bin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-20 15:51:04.000000 fx-bin-0.6.0/fx_bin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:51:04.000000 fx-bin-0.6.0/fx_bin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-20 15:51:04.000000 fx-bin-0.6.0/fx_bin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:51:04.000000 fx-bin-0.6.0/fx_bin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 15:51:04.000000 fx-bin-0.6.0/fx_bin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 15:51:04.000000 fx-bin-0.6.0/fx_bin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-20 15:50:59.000000 fx-bin-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-20 15:51:04.164736 fx-bin-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-20 15:50:59.000000 fx-bin-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:51:04.160736 fx-bin-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-20 15:50:59.000000 fx-bin-0.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-20 15:50:59.000000 fx-bin-0.6.0/tests/test_py_fx_bin.py
```

### Comparing `fx-bin-0.5.0/CONTRIBUTING.rst` & `fx-bin-0.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `fx-bin-0.5.0/PKG-INFO` & `fx-bin-0.6.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: fx-bin
-Version: 0.5.0
+Version: 0.6.0
 Summary: A common bin collection for my own usage
 Home-page: https://github.com/frankyxhl/py_fx_bin
 Author: Frank Xu
 Author-email: frank@frankxu.me
-License: UNKNOWN
 Keywords: fx_bin
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 
 =============
 Python FX bin
 =============
 
 
 
@@ -42,9 +42,7 @@
 History
 =======
 
 0.1.0 (2019-07-27)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `fx-bin-0.5.0/docs/Makefile` & `fx-bin-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fx-bin-0.5.0/docs/conf.py` & `fx-bin-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fx-bin-0.5.0/docs/installation.rst` & `fx-bin-0.6.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `fx-bin-0.5.0/docs/make.bat` & `fx-bin-0.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fx-bin-0.5.0/fx_bin/files.py` & `fx-bin-0.6.0/fx_bin/files.py`

 * *Files identical despite different names*

### Comparing `fx-bin-0.5.0/fx_bin/lib.py` & `fx-bin-0.6.0/fx_bin/lib.py`

 * *Files identical despite different names*

### Comparing `fx-bin-0.5.0/fx_bin/pd.py` & `fx-bin-0.6.0/fx_bin/pd.py`

 * *Files identical despite different names*

### Comparing `fx-bin-0.5.0/fx_bin/replace.py` & `fx-bin-0.6.0/fx_bin/replace.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
-import os.path
+# import os.path
 import sys
 import tempfile
 import click
+from loguru import logger as L
 
 
 def work(s, t, f):
     tmp = tempfile.mkstemp()[1]
     with open(f) as fd1, open(tmp, 'w') as fd2:
         for line in fd1:
             line = line.replace(s, t)
@@ -14,19 +15,20 @@
     os.rename(tmp, f)
 
 
 @click.command()
 @click.argument('search_text', nargs=1)
 @click.argument('replace_text', nargs=1)
 @click.argument('filenames', nargs=-1)
-def main(search_text, replace_text, filenames, args=None):
-    for f in filenames:
+def main(search_text: str, replace_text: str, file_names):
+    for f in file_names:
         if not os.path.isfile(f):
-            print(f"This file does not exist: {f}")
+            L.error(f"This file does not exist: {f}")
             return 1
-    for f in filenames:
+    for f in file_names:
+        L.debug(f'Replacing {search_text} with {replace_text} in {f}')
         work(search_text, replace_text, f)
     return 0
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `fx-bin-0.5.0/fx_bin/size.py` & `fx-bin-0.6.0/fx_bin/size.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import math
 from dataclasses import dataclass
 from enum import Enum
 from functools import total_ordering
+from loguru import Logger as L
 
 __all__ = ["list_size"]
 
 
 class EntryType(Enum):
     FILE = 1
     FOLDER = 2
```

### Comparing `fx-bin-0.5.0/fx_bin/upload_server.py` & `fx-bin-0.6.0/fx_bin/upload_server.py`

 * *Files 7% similar despite different names*

```diff
@@ -291,17 +291,26 @@
         })
 
 
 def get_lan_ip():
     """
     https://www.w3resource.com/python-exercises/python-basic-exercise-55.php
     """
-    return [l for l in ([ip for ip in socket.gethostbyname_ex(socket.gethostname())[2]
-                         if not ip.startswith("127.")][:1], [[(s.connect(('8.8.8.8', 53)), s.getsockname()[0], s.close())
-                                                              for s in [socket.socket(socket.AF_INET, socket.SOCK_DGRAM)]][0][1]]) if l][0][0]
+    # Attempt to get IP from host name
+    hostname = socket.gethostname()
+    ips_from_hostname = socket.gethostbyname_ex(hostname)[2]
+    non_local_ips_from_hostname = [ip for ip in ips_from_hostname if not ip.startswith("127.")]
+    # If there are non-local IPs from the hostname, return the first one
+    if non_local_ips_from_hostname:
+        return non_local_ips_from_hostname[0]
+    # If there are no non-local IPs from the hostname, try another method
+    with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as s:
+        s.connect(('8.8.8.8', 53))
+        ip_from_socket = s.getsockname()[0]
+    return ip_from_socket
 
 
 def main():
     ip = get_lan_ip()
     port = 8000
     while port < 8050:
         try:
@@ -319,12 +328,12 @@
                 print(e)
                 break
         except KeyboardInterrupt:
             print('Interrupted By User')
             try:
                 sys.exit(0)
             except SystemExit:
-                os._exit(0)
+                os.exit(0)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `fx-bin-0.5.0/fx_bin.egg-info/PKG-INFO` & `fx-bin-0.6.0/fx_bin.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: fx-bin
-Version: 0.5.0
+Version: 0.6.0
 Summary: A common bin collection for my own usage
 Home-page: https://github.com/frankyxhl/py_fx_bin
 Author: Frank Xu
 Author-email: frank@frankxu.me
-License: UNKNOWN
 Keywords: fx_bin
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 
 =============
 Python FX bin
 =============
 
 
 
@@ -42,9 +42,7 @@
 History
 =======
 
 0.1.0 (2019-07-27)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `fx-bin-0.5.0/fx_bin.egg-info/SOURCES.txt` & `fx-bin-0.6.0/fx_bin.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 CONTRIBUTING.rst
 HISTORY.rst
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 docs/Makefile
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
```

### Comparing `fx-bin-0.5.0/setup.py` & `fx-bin-0.6.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
-requirements = ['Click>=7.0', ]
+requirements = ['Click>=8.1.3', ]
 
 setup_requirements = []
 
 test_requirements = []
 
 setup(
     name='fx-bin',
@@ -23,32 +23,34 @@
     author_email='frank@frankxu.me',
     classifiers=[
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
     description="A common bin collection for my own usage",
     entry_points={
         'console_scripts': [
-            'fx.upgrade=fx_bin.run_upgrade_program:main',
-            'fx.files=fx_bin.files:main',
-            'fx.size=fx_bin.size:main',
-            'fx.ff=fx_bin.find_files:main',
-            'fx.replace=fx_bin.replace:main',
-            'fx.grab_json_api_to_excel=fx_bin.pd:main',
-            'fx.server=fx_bin.upload_server:main',
+            'fx_upgrade=fx_bin.run_upgrade_program:main',
+            'fx_files=fx_bin.files:main',
+            'fx_size=fx_bin.size:main',
+            'fx_ff=fx_bin.find_files:main',
+            'fx_replace=fx_bin.replace:main',
+            'fx_grab_json_api_to_excel=fx_bin.pd:main',
+            'fx_server=fx_bin.upload_server:main',
         ],
     },
     install_requires=requirements,
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='fx_bin',
     packages=find_packages(include=['fx_bin']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/frankyxhl/py_fx_bin',
-    version='0.5.0',
+    version='0.6.0',
     zip_safe=False,
 )
```

### Comparing `fx-bin-0.5.0/tests/test_py_fx_bin.py` & `fx-bin-0.6.0/tests/test_py_fx_bin.py`

 * *Files identical despite different names*

