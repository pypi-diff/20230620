# Comparing `tmp/rest_uploader-1.5.0.tar.gz` & `tmp/rest_uploader-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rest_uploader-1.5.0.tar", last modified: Wed Feb 19 20:01:31 2020, max compression
+gzip compressed data, was "dist/rest_uploader-1.9.0.tar", last modified: Tue May 12 20:40:09 2020, max compression
```

## Comparing `rest_uploader-1.5.0.tar` & `rest_uploader-1.9.0.tar`

### file list

```diff
@@ -1,45 +1,44 @@
-drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2020-02-19 20:01:31.451115 rest_uploader-1.5.0/
--rwxrwxrwx   0 justin    (1000) justin    (1000)      166 2019-04-15 02:31:41.000000 rest_uploader-1.5.0/AUTHORS.rst
--rwxrwxrwx   0 justin    (1000) justin    (1000)     3608 2019-04-15 02:31:41.000000 rest_uploader-1.5.0/CONTRIBUTING.rst
--rwxrwxrwx   0 justin    (1000) justin    (1000)     1155 2020-02-19 19:58:56.000000 rest_uploader-1.5.0/HISTORY.rst
--rwxrwxrwx   0 justin    (1000) justin    (1000)     1072 2019-04-15 02:31:41.000000 rest_uploader-1.5.0/LICENSE
--rwxrwxrwx   0 justin    (1000) justin    (1000)      262 2019-04-15 02:31:41.000000 rest_uploader-1.5.0/MANIFEST.in
--rw-r--r--   0 justin    (1000) justin    (1000)     3786 2020-02-19 20:01:31.451115 rest_uploader-1.5.0/PKG-INFO
--rwxrwxrwx   0 justin    (1000) justin    (1000)      901 2019-06-26 18:37:09.000000 rest_uploader-1.5.0/README.rst
-drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2020-02-19 20:01:31.447781 rest_uploader-1.5.0/docs/
--rwxrwxrwx   0 justin    (1000) justin    (1000)      614 2019-04-15 02:31:41.000000 rest_uploader-1.5.0/docs/Makefile
-drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2020-02-19 20:01:31.444448 rest_uploader-1.5.0/docs/_build/
-drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2020-02-19 20:01:31.444448 rest_uploader-1.5.0/docs/_build/html/
-drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2020-02-19 20:01:31.447781 rest_uploader-1.5.0/docs/_build/html/_static/
--rwxrwxrwx   0 justin    (1000) justin    (1000)      286 2019-06-26 18:35:58.000000 rest_uploader-1.5.0/docs/_build/html/_static/file.png
--rwxrwxrwx   0 justin    (1000) justin    (1000)       90 2019-06-26 18:35:58.000000 rest_uploader-1.5.0/docs/_build/html/_static/minus.png
--rwxrwxrwx   0 justin    (1000) justin    (1000)       90 2019-06-26 18:35:58.000000 rest_uploader-1.5.0/docs/_build/html/_static/plus.png
--rwxrwxrwx   0 justin    (1000) justin    (1000)       28 2019-04-15 02:31:41.000000 rest_uploader-1.5.0/docs/authors.rst
--rwxrwxrwx   0 justin    (1000) justin    (1000)     4942 2019-06-26 15:30:30.000000 rest_uploader-1.5.0/docs/conf.py
--rwxrwxrwx   0 justin    (1000) justin    (1000)       33 2019-04-15 02:31:41.000000 rest_uploader-1.5.0/docs/contributing.rst
--rwxrwxrwx   0 justin    (1000) justin    (1000)       28 2019-04-15 02:31:41.000000 rest_uploader-1.5.0/docs/history.rst
--rwxrwxrwx   0 justin    (1000) justin    (1000)      310 2019-04-15 02:31:41.000000 rest_uploader-1.5.0/docs/index.rst
--rwxrwxrwx   0 justin    (1000) justin    (1000)     1178 2019-04-15 02:31:41.000000 rest_uploader-1.5.0/docs/installation.rst
--rwxrwxrwx   0 justin    (1000) justin    (1000)      775 2019-04-15 02:31:41.000000 rest_uploader-1.5.0/docs/make.bat
--rwxrwxrwx   0 justin    (1000) justin    (1000)       27 2019-04-15 02:31:41.000000 rest_uploader-1.5.0/docs/readme.rst
--rwxrwxrwx   0 justin    (1000) justin    (1000)       81 2019-04-15 02:31:41.000000 rest_uploader-1.5.0/docs/usage.rst
-drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2020-02-19 20:01:31.447781 rest_uploader-1.5.0/rest_uploader/
--rwxrwxrwx   0 justin    (1000) justin    (1000)      166 2020-02-19 19:59:32.000000 rest_uploader-1.5.0/rest_uploader/__init__.py
--rwxrwxrwx   0 justin    (1000) justin    (1000)      907 2019-06-26 17:53:23.000000 rest_uploader-1.5.0/rest_uploader/api_token.py
--rwxrwxrwx   0 justin    (1000) justin    (1000)     1715 2020-02-19 19:57:44.000000 rest_uploader-1.5.0/rest_uploader/cli.py
--rwxrwxrwx   0 justin    (1000) justin    (1000)     1922 2019-11-14 16:35:03.000000 rest_uploader-1.5.0/rest_uploader/img_process.py
--rwxrwxrwx   0 justin    (1000) justin    (1000)     7674 2020-02-19 15:20:12.000000 rest_uploader-1.5.0/rest_uploader/rest_uploader.py
--rwxrwxrwx   0 justin    (1000) justin    (1000)      154 2019-11-12 20:44:41.000000 rest_uploader-1.5.0/rest_uploader/settings.py
-drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2020-02-19 20:01:31.447781 rest_uploader-1.5.0/rest_uploader.egg-info/
--rwxrwxrwx   0 justin    (1000) justin    (1000)     3786 2020-02-19 20:01:31.000000 rest_uploader-1.5.0/rest_uploader.egg-info/PKG-INFO
--rwxrwxrwx   0 justin    (1000) justin    (1000)      824 2020-02-19 20:01:31.000000 rest_uploader-1.5.0/rest_uploader.egg-info/SOURCES.txt
--rwxrwxrwx   0 justin    (1000) justin    (1000)        1 2020-02-19 20:01:31.000000 rest_uploader-1.5.0/rest_uploader.egg-info/dependency_links.txt
--rwxrwxrwx   0 justin    (1000) justin    (1000)       58 2020-02-19 20:01:31.000000 rest_uploader-1.5.0/rest_uploader.egg-info/entry_points.txt
--rwxrwxrwx   0 justin    (1000) justin    (1000)        1 2019-04-15 19:08:41.000000 rest_uploader-1.5.0/rest_uploader.egg-info/not-zip-safe
--rwxrwxrwx   0 justin    (1000) justin    (1000)       67 2020-02-19 20:01:31.000000 rest_uploader-1.5.0/rest_uploader.egg-info/requires.txt
--rwxrwxrwx   0 justin    (1000) justin    (1000)       14 2020-02-19 20:01:31.000000 rest_uploader-1.5.0/rest_uploader.egg-info/top_level.txt
--rwxrwxrwx   0 justin    (1000) justin    (1000)      396 2020-02-19 20:01:31.451115 rest_uploader-1.5.0/setup.cfg
--rwxrwxrwx   0 justin    (1000) justin    (1000)     1675 2020-02-19 19:59:32.000000 rest_uploader-1.5.0/setup.py
-drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2020-02-19 20:01:31.451115 rest_uploader-1.5.0/tests/
--rwxrwxrwx   0 justin    (1000) justin    (1000)       68 2019-04-15 02:31:41.000000 rest_uploader-1.5.0/tests/__init__.py
--rwxrwxrwx   0 justin    (1000) justin    (1000)      918 2019-06-26 15:30:30.000000 rest_uploader-1.5.0/tests/test_rest_uploader.py
+drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2020-05-12 20:40:09.736682 rest_uploader-1.9.0/
+-rwxrwxrwx   0 justin    (1000) justin    (1000)      166 2019-04-15 02:31:41.000000 rest_uploader-1.9.0/AUTHORS.rst
+-rwxrwxrwx   0 justin    (1000) justin    (1000)     3608 2019-04-15 02:31:41.000000 rest_uploader-1.9.0/CONTRIBUTING.rst
+-rwxrwxrwx   0 justin    (1000) justin    (1000)     1819 2020-05-12 20:37:38.000000 rest_uploader-1.9.0/HISTORY.rst
+-rwxrwxrwx   0 justin    (1000) justin    (1000)     1072 2019-04-15 02:31:41.000000 rest_uploader-1.9.0/LICENSE
+-rwxrwxrwx   0 justin    (1000) justin    (1000)      262 2019-04-15 02:31:41.000000 rest_uploader-1.9.0/MANIFEST.in
+-rw-r--r--   0 justin    (1000) justin    (1000)     4618 2020-05-12 20:40:09.736682 rest_uploader-1.9.0/PKG-INFO
+-rwxrwxrwx   0 justin    (1000) justin    (1000)      901 2019-06-26 18:37:09.000000 rest_uploader-1.9.0/README.rst
+drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2020-05-12 20:40:09.733348 rest_uploader-1.9.0/docs/
+-rwxrwxrwx   0 justin    (1000) justin    (1000)      614 2019-04-15 02:31:41.000000 rest_uploader-1.9.0/docs/Makefile
+drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2020-05-12 20:40:09.726679 rest_uploader-1.9.0/docs/_build/
+drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2020-05-12 20:40:09.726679 rest_uploader-1.9.0/docs/_build/html/
+drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2020-05-12 20:40:09.733348 rest_uploader-1.9.0/docs/_build/html/_static/
+-rwxrwxrwx   0 justin    (1000) justin    (1000)      286 2019-06-26 18:35:58.000000 rest_uploader-1.9.0/docs/_build/html/_static/file.png
+-rwxrwxrwx   0 justin    (1000) justin    (1000)       90 2019-06-26 18:35:58.000000 rest_uploader-1.9.0/docs/_build/html/_static/minus.png
+-rwxrwxrwx   0 justin    (1000) justin    (1000)       90 2019-06-26 18:35:58.000000 rest_uploader-1.9.0/docs/_build/html/_static/plus.png
+-rwxrwxrwx   0 justin    (1000) justin    (1000)       28 2019-04-15 02:31:41.000000 rest_uploader-1.9.0/docs/authors.rst
+-rwxrwxrwx   0 justin    (1000) justin    (1000)     4942 2019-06-26 15:30:30.000000 rest_uploader-1.9.0/docs/conf.py
+-rwxrwxrwx   0 justin    (1000) justin    (1000)       33 2019-04-15 02:31:41.000000 rest_uploader-1.9.0/docs/contributing.rst
+-rwxrwxrwx   0 justin    (1000) justin    (1000)       28 2019-04-15 02:31:41.000000 rest_uploader-1.9.0/docs/history.rst
+-rwxrwxrwx   0 justin    (1000) justin    (1000)      310 2019-04-15 02:31:41.000000 rest_uploader-1.9.0/docs/index.rst
+-rwxrwxrwx   0 justin    (1000) justin    (1000)     1178 2019-04-15 02:31:41.000000 rest_uploader-1.9.0/docs/installation.rst
+-rwxrwxrwx   0 justin    (1000) justin    (1000)      775 2019-04-15 02:31:41.000000 rest_uploader-1.9.0/docs/make.bat
+-rwxrwxrwx   0 justin    (1000) justin    (1000)       27 2019-04-15 02:31:41.000000 rest_uploader-1.9.0/docs/readme.rst
+-rwxrwxrwx   0 justin    (1000) justin    (1000)       81 2019-04-15 02:31:41.000000 rest_uploader-1.9.0/docs/usage.rst
+drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2020-05-12 20:40:09.733348 rest_uploader-1.9.0/rest_uploader/
+-rwxrwxrwx   0 justin    (1000) justin    (1000)      182 2020-05-12 20:38:50.000000 rest_uploader-1.9.0/rest_uploader/__init__.py
+-rwxrwxrwx   0 justin    (1000) justin    (1000)      905 2020-05-11 21:03:27.000000 rest_uploader-1.9.0/rest_uploader/api_token.py
+-rw-r--r--   0 justin    (1000) justin    (1000)     3162 2020-05-12 17:08:51.000000 rest_uploader-1.9.0/rest_uploader/cli.py
+-rw-r--r--   0 justin    (1000) justin    (1000)     2104 2020-05-12 17:10:37.000000 rest_uploader-1.9.0/rest_uploader/img_process.py
+-rw-r--r--   0 justin    (1000) justin    (1000)     8393 2020-05-12 17:08:51.000000 rest_uploader-1.9.0/rest_uploader/rest_uploader.py
+drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2020-05-12 20:40:09.736682 rest_uploader-1.9.0/rest_uploader.egg-info/
+-rw-r--r--   0 justin    (1000) justin    (1000)     4618 2020-05-12 20:40:09.000000 rest_uploader-1.9.0/rest_uploader.egg-info/PKG-INFO
+-rw-r--r--   0 justin    (1000) justin    (1000)      798 2020-05-12 20:40:09.000000 rest_uploader-1.9.0/rest_uploader.egg-info/SOURCES.txt
+-rw-r--r--   0 justin    (1000) justin    (1000)        1 2020-05-12 20:40:09.000000 rest_uploader-1.9.0/rest_uploader.egg-info/dependency_links.txt
+-rw-r--r--   0 justin    (1000) justin    (1000)       58 2020-05-12 20:40:09.000000 rest_uploader-1.9.0/rest_uploader.egg-info/entry_points.txt
+-rw-r--r--   0 justin    (1000) justin    (1000)        1 2020-05-12 20:30:51.000000 rest_uploader-1.9.0/rest_uploader.egg-info/not-zip-safe
+-rw-r--r--   0 justin    (1000) justin    (1000)       67 2020-05-12 20:40:09.000000 rest_uploader-1.9.0/rest_uploader.egg-info/requires.txt
+-rw-r--r--   0 justin    (1000) justin    (1000)       14 2020-05-12 20:40:09.000000 rest_uploader-1.9.0/rest_uploader.egg-info/top_level.txt
+-rwxrwxrwx   0 justin    (1000) justin    (1000)      396 2020-05-12 20:40:09.736682 rest_uploader-1.9.0/setup.cfg
+-rwxrwxrwx   0 justin    (1000) justin    (1000)     1676 2020-05-12 20:39:02.000000 rest_uploader-1.9.0/setup.py
+drwxr-xr-x   0 justin    (1000) justin    (1000)        0 2020-05-12 20:40:09.736682 rest_uploader-1.9.0/tests/
+-rwxrwxrwx   0 justin    (1000) justin    (1000)       68 2019-04-15 02:31:41.000000 rest_uploader-1.9.0/tests/__init__.py
+-rwxrwxrwx   0 justin    (1000) justin    (1000)      918 2019-06-26 15:30:30.000000 rest_uploader-1.9.0/tests/test_rest_uploader.py
```

### Comparing `rest_uploader-1.5.0/CONTRIBUTING.rst` & `rest_uploader-1.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rest_uploader-1.5.0/LICENSE` & `rest_uploader-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rest_uploader-1.5.0/PKG-INFO` & `rest_uploader-1.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: rest_uploader
-Version: 1.5.0
+Version: 1.9.0
 Summary: REST API Uploader
 Home-page: https://github.com/kellerjustin/rest-uploader
 Author: Justin Keller
 Author-email: kellerjustin@protonmail.com
 License: MIT license
 Description: =============
         rest_uploader
@@ -115,14 +115,35 @@
         
         
         1.5.0 (2020-02-19)
         ------------------
         
         * Embarrassingly dumb bug fix for autotag argument
         
+        
+        1.7.0 (2020-05-11)
+        ------------------
+        
+        * Added command line options for server, port, destination notebook
+        * Added some error handling to quit when Joplin is closed or there
+          is no valid notebook detected
+        * Removed the settings.py file - everything handled via command line
+          switches
+        * More verbose command line notifications
+        * Not leaving temp file location setting to user, handling this by 
+          detecting OS on startup
+        
+        
+        1.9.0 (2020-05-12)
+        ------------------
+        
+        * Immediately realized closing application if Joplin isn't running is
+          a bad idea in the case of startup scripts, etc - fixed logic to wait
+        * Made use of the tempfile library which made life easier
+        
 Keywords: rest_uploader,joplin,rest-uploader
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
```

### Comparing `rest_uploader-1.5.0/README.rst` & `rest_uploader-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `rest_uploader-1.5.0/docs/Makefile` & `rest_uploader-1.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rest_uploader-1.5.0/docs/conf.py` & `rest_uploader-1.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rest_uploader-1.5.0/docs/installation.rst` & `rest_uploader-1.9.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `rest_uploader-1.5.0/docs/make.bat` & `rest_uploader-1.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rest_uploader-1.5.0/rest_uploader/api_token.py` & `rest_uploader-1.9.0/rest_uploader/api_token.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import requests
 from os import path
-from .settings import SERVER
 
 
 def get_token():
     if path.exists(".api_token.txt"):
         with open(".api_token.txt", "r") as f:
             token = f.readline().rstrip()
     else:
@@ -14,22 +12,30 @@
     return token
 
 
 def get_token_suffix():
     return "?token=" + get_token()
 
 
-# Code from a non-Joplin API
+"""
+Code from a non-Joplin API
+Not currently used
+"""
+
+"""
+import requests
+
 def get_header():
     try:
         my_token = get_token()
         url = SERVER + "/ping"
-        head = {"Authorization": "Bearer {}".format(my_token)}
+        head = {"Authorization": f"Bearer {my_token}"}
         try:
             response = requests.get(url, headers=head)
             if response.status_code != 200:
                 print("Invalid token!")
         except ValueError:
             print("Token expired!")
     except FileNotFoundError:
         print("No Token!")
     return head
+"""
```

### Comparing `rest_uploader-1.5.0/rest_uploader/cli.py` & `rest_uploader-1.9.0/rest_uploader/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 # -*- coding: utf-8 -*-
 
 """Console script for rest_uploader."""
 import sys
 import click
-from .rest_uploader import watcher, set_autotag
-from .img_process import set_language
+from .rest_uploader import (
+    watcher,
+    set_autotag,
+    set_notebook_id,
+    set_working_directory,
+    set_endpoint,
+    set_token,
+)
+from .img_process import set_language, set_temp_path
 from . import __version__
 
 
-"""Helper function for wild arguments"""
 def parse_argument(arg):
+    """Helper function for wild arguments"""
     if arg in ["No", "N", "NO", "OFF", "off", "n", "no"]:
         arg = "no"
     else:
         arg = "yes"
     return arg
 
 
@@ -26,42 +33,88 @@
         dir_okay=True,
         writable=False,
         readable=True,
         resolve_path=True,
     ),
 )
 @click.option(
+    "-s",
+    "--server",
+    "server",
+    default="127.0.0.1",
+    help="""Specify the server to which the application"""
+    """ should connect. Default = "127.0.0.1" """,
+)
+@click.option(
+    "-p",
+    "--port",
+    "port",
+    default="41184",
+    help="""Specify the port to which the application should connect."""
+    """ Default = 41184 """,
+)
+@click.option(
     "-l",
     "--language",
     "language",
     default="eng",
-    help="""Specify OCR Language. 
-            Refer to Tesseract's documentation found here:
-            https://github.com/tesseract-ocr/tesseract/wiki""",
+    help="""Specify OCR Language. Refer to Tesseract's documentation found here: 
+    https://github.com/tesseract-ocr/tesseract/wiki""",
 )
 @click.option(
     "-t",
     "--autotag",
     "autotag",
     default="yes",
-    help="""Specify whether or not to automatically tag notes
-            based on OCR'd text. Default = 'yes', specify 'no' 
-            if this behavior is not desired""",
+    help="""Specify whether or not to automatically tag notes based on"""
+    """ OCR'd text. Default = 'yes', specify 'no' if this behavior is"""
+    """ not desired""",
+)
+@click.option(
+    "-d",
+    "--destination",
+    "destination",
+    default="inbox",
+    help="""Specify the notebook in which to place newly created notes."""
+    """ Specified notebook must exist or program will exit."""
+    """ Default = "inbox". """,
 )
 @click.version_option(version=__version__)
-def main(path=None, language="eng", autotag="yes"):
+def main(
+    path=None,
+    server="server",
+    port="port",
+    language="eng",
+    autotag="yes",
+    destination="inbox",
+):
     """ Console script for rest_uploader.
         Define file path to monitor, e.g.
         rest_uploader /home/user/Docouments/scans    
     """
     click.echo("Launching Application " "rest_uploader.cli.main")
+    set_working_directory()
+    set_endpoint(server, port)
+    set_token()
+    set_temp_path()
+    notebook_id = set_notebook_id(destination.strip())
+    if notebook_id == "err":
+        click.echo("Joplin may not be running, please ensure it is open.")
+        click.echo("     will check again when processing a file.")
+    elif notebook_id == "":
+        click.echo(f"Invalid Notebook, check to see if {destination.strip()} exists.")
+        click.echo(f"Please specify a valid notebook. Quitting application.")
+        return 0
+    else:
+        click.echo(f"Found Notebook ID: {notebook_id}")
     set_language(language)
     autotag = parse_argument(autotag)
     set_autotag(parse_argument(autotag))
     click.echo("Language: " + language)
     click.echo("Automatically Tag Notes? " + autotag)
+    click.echo("Desitnation Notebook: " + destination)
     watcher(path=path)
     return 0
 
 
 if __name__ == "__main__":
     sys.exit(main())  # pragma: no cover
```

### Comparing `rest_uploader-1.5.0/rest_uploader/img_process.py` & `rest_uploader-1.9.0/rest_uploader/img_process.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 import PyPDF2
 import os
+import tempfile
 from uuid import uuid4
 from PIL import Image
 from pdf2image import convert_from_path
 from pytesseract import image_to_string, TesseractError
-from .settings import TEMP_PATH
 
 
+TEMP_PATH = tempfile.gettempdir()
+
 def set_language(language):
     global LANGUAGE
     LANGUAGE = language
 
 
+def set_temp_path():
+    global TEMP_PATH
+    TEMP_PATH = tempfile.gettempdir()
+    print(f"Temp Path: {TEMP_PATH}")
+
+
 def open_pdf(filename):
     try:
         pdfFileObject = open(filename, "rb")
         pdf_reader = PyPDF2.PdfFileReader(pdfFileObject, strict=False)
         return pdf_reader
     except PyPDF2.utils.PdfReadError:
         print("PDF not fully written - no EOF Marker")
@@ -26,39 +34,41 @@
     if open_pdf(filename) is None:
         return False
     else:
         return True
 
 
 def pdf_page_to_image(filename, page_num=0):
+    global TEMP_PATH
     pages = convert_from_path(filename, 250)
     if page_num == 0:
-        tempfile = TEMP_PATH + "preview.png"
+        tempfile = f"{TEMP_PATH}/preview.png"
     else:
-        tempfile = TEMP_PATH + f"{uuid4()}.png"
+        tempfile = f"{TEMP_PATH}/{uuid4()}.png"
     pages[page_num].save(tempfile, "PNG")
     return tempfile
 
 
 def extract_text_from_pdf(filename):
+    global TEMP_PATH
     pdfReader = open_pdf(filename)
     count = pdfReader.numPages
     text = ""
     for i in range(count):
         text += f"\n\n***PAGE {i+1} of {count}*** \n\n"
         page = pdfReader.getPage(i)
         embedded_text = page.extractText()
         # if embedded PDF text is minimal or does not exist,
         # run OCR the images extracted from the PDF
         if len(embedded_text) >= 100:
             text += embedded_text
         else:
             extracted_image = pdf_page_to_image(filename, i)
             text += extract_text_from_image(extracted_image)
-            if extracted_image != TEMP_PATH + "preview.png":
+            if extracted_image != f"{TEMP_PATH}\preview.png":
                 os.remove(extracted_image)
     return text
 
 
 def extract_text_from_image(filename):
     try:
         text = image_to_string(Image.open(filename), lang=LANGUAGE)
```

### Comparing `rest_uploader-1.5.0/rest_uploader/rest_uploader.py` & `rest_uploader-1.9.0/rest_uploader/rest_uploader.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 from watchdog.observers import Observer
 from watchdog.events import FileSystemEventHandler
 from .img_process import (
     extract_text_from_image,
     extract_text_from_pdf,
     pdf_page_to_image,
     pdf_valid,
+    TEMP_PATH,
 )
-from .settings import SERVER, JOPLIN_NOTEBOOK, TEMP_PATH
 from .api_token import get_token_suffix
 from pathlib import Path
 
 
 """
 2018-09-24 JRK
 This program was created to upload files from a folder specified in the
@@ -88,154 +88,181 @@
 def set_autotag(autotag):
     global AUTOTAG
     AUTOTAG = True
     if autotag == "no":
         AUTOTAG = False
 
 
+def set_endpoint(server, port):
+    global ENDPOINT
+    ENDPOINT = f"http://{server}:{port}"
+    print(f"Endpoint: {ENDPOINT}")
+
+
+def initialize_notebook(notebook_name):
+    global NOTEBOOK_NAME
+    NOTEBOOK_NAME = notebook_name
+    global NOTEBOOK_ID
+    NOTEBOOK_ID = ""
+    return NOTEBOOK_NAME
+
+
+def set_notebook_id(notebook_name=None):
+    """ Find the ID of the destination folder 
+    adapted logic from jhf2442 on Joplin forum
+    https://discourse.joplin.cozic.net/t/import-txt-files/692
+    """
+    global NOTEBOOK_NAME
+    global NOTEBOOK_ID
+    if notebook_name is not None:
+        NOTEBOOK_NAME = initialize_notebook(notebook_name)
+    try:
+        res = requests.get(ENDPOINT + "/folders" + TOKEN)
+        folders = res.json()
+        for folder in folders:
+            if folder.get("title") == NOTEBOOK_NAME:
+                NOTEBOOK_ID = folder.get("id")
+        if NOTEBOOK_ID == "":
+            for folder in folders:
+                if "children" in folder:
+                    for child in folder.get("children"):
+                        if child.get("title") == NOTEBOOK_NAME:
+                            NOTEBOOK_ID = child.get("id")
+        return NOTEBOOK_ID
+    except requests.ConnectionError as e:
+        print("Connection Error - Is Joplin Running?")
+        return "err"
+
+
 def read_text_note(filename):
     with open(filename, "r") as myfile:
         text = myfile.read()
         print(text)
     return text
 
 
 def read_csv(filename):
     return csv.DictReader(open(filename))
 
 
-def get_notebook_id():
-    # Find the ID of the destination folder
-    # adapted logic from jhf2442 on Joplin forum
-    # https://discourse.joplin.cozic.net/t/import-txt-files/692
-    res = requests.get(SERVER + "/folders" + TOKEN)
-    folders = res.json()
-
-    notebook_id = 0
-    for folder in folders:
-        if folder.get("title") == JOPLIN_NOTEBOOK:
-            notebook_id = folder.get("id")
-    if notebook_id == 0:
-        for folder in folders:
-            if "children" in folder:
-                for child in folder.get("children"):
-                    if child.get("title") == JOPLIN_NOTEBOOK:
-                        notebook_id = child.get("id")
-    return notebook_id
-
-
 def apply_tags(text_to_match, note_id):
-    # Rudimentary Tag match using OCR'd text
-    res = requests.get(SERVER + "/tags" + TOKEN)
+    """ Rudimentary Tag match using OCR'd text """
+    res = requests.get(ENDPOINT + "/tags" + TOKEN)
     tags = res.json()
+    counter = 0
     for tag in tags:
         if tag.get("title").lower() in text_to_match.lower():
+            counter += 1
             tag_id = tag.get("id")
-            print(f"{tag_id} matches body for {note_id}")
-            response = requests.post(SERVER + f"/tags/{tag_id}/notes" + TOKEN, data=f'{{"id": "{note_id}"}}')
-    
+            response = requests.post(
+                ENDPOINT + f"/tags/{tag_id}/notes" + TOKEN,
+                data=f'{{"id": "{note_id}"}}',
+            )
+    print(f"Matched {counter} tag(s) for note {note_id}")
+    return counter
+
 
 def create_resource(filename):
+    if NOTEBOOK_ID == "":
+        set_notebook_id()
     basefile = os.path.basename(filename)
     title = os.path.splitext(basefile)[0]
     files = {
         "data": (json.dumps(filename), open(filename, "rb")),
-        "props": (None, '{{"title":"{}", "filename":"{}"}}'.format(title, basefile)),
+        "props": (None, f'{{"title":"{title}", "filename":"{basefile}"}}'),
     }
-    response = requests.post(SERVER + "/resources" + TOKEN, files=files)
+    response = requests.post(ENDPOINT + "/resources" + TOKEN, files=files)
     print(response.json())
     return response.json()
 
 
 def delete_resource(resource_id):
-    apitext = SERVER + "/resources/" + resource_id + TOKEN
+    apitext = ENDPOINT + "/resources/" + resource_id + TOKEN
     response = requests.delete(apitext)
     return response
 
 
 def get_resource(resource_id):
-    apitext = SERVER + "/resources/" + resource_id + TOKEN
+    apitext = ENDPOINT + "/resources/" + resource_id + TOKEN
     response = requests.get(apitext)
     return response
 
 
 def encode_image(filename, datatype):
     encoded = base64.b64encode(open(filename, "rb").read())
-    img = "data:{};base64,{}".format(datatype, encoded.decode())
+    img = f"data:{datatype};base64,{encoded.decode()}"
     return img
 
 
-def set_json_string(title, notebook_id, body, img=None):
+def set_json_string(title, NOTEBOOK_ID, body, img=None):
     if img is None:
         return '{{ "title": {}, "parent_id": "{}", "body": {} }}'.format(
-            json.dumps(title), notebook_id, json.dumps(body)
+            json.dumps(title), NOTEBOOK_ID, json.dumps(body)
         )
     else:
         return '{{ "title": "{}", "parent_id": "{}", "body": {}, "image_data_url": "{}" }}'.format(
-            title, notebook_id, json.dumps(body), img
+            title, NOTEBOOK_ID, json.dumps(body), img
         )
 
 
 def upload(filename):
     """ Get the default Notebook ID and process the passed in file"""
-    notebook_id = get_notebook_id()
     basefile = os.path.basename(filename)
     title, ext = os.path.splitext(basefile)
-    body = basefile + " uploaded from " + platform.node() + "\n"
+    body = f"{basefile} uploaded from {platform.node()}\n"
     datatype = mimetypes.guess_type(filename)[0]
     if datatype is None:
         # avoid subscript exception if datatype is None
         if ext in (".url", ".lnk"):
             datatype = "text/plain"
         else:
             datatype = ""
     if datatype == "text/plain":
         body += read_text_note(filename)
-        values = set_json_string(title, notebook_id, body)
+        values = set_json_string(title, NOTEBOOK_ID, body)
     if datatype == "text/csv":
         table = read_csv(filename)
         body += tabulate(table, headers="keys", numalign="right", tablefmt="pipe")
-        values = set_json_string(title, notebook_id, body)
+        values = set_json_string(title, NOTEBOOK_ID, body)
     elif datatype[:5] == "image":
         img = encode_image(filename, datatype)
         body += "\n<!---\n"
         body += extract_text_from_image(filename)
         body += "\n-->\n"
-        values = set_json_string(title, notebook_id, body, img)
+        values = set_json_string(title, NOTEBOOK_ID, body, img)
     else:
         response = create_resource(filename)
-        body += "[{}](:/{})".format(basefile, response["id"])
-        values = set_json_string(title, notebook_id, body)
+        body += f"[{basefile}](:/{response['id']})"
+        values = set_json_string(title, NOTEBOOK_ID, body)
         if response["file_extension"] == "pdf":
             # Special handling for PDFs
             body += "\n<!---\n"
             body += extract_text_from_pdf(filename)
             body += "\n-->\n"
-            previewfile = TEMP_PATH + "preview.png"
+            previewfile = f"{TEMP_PATH}\preview.png"
             if not os.path.exists(previewfile):
                 previewfile = pdf_page_to_image(filename)
             img = encode_image(previewfile, "image/png")
             os.remove(previewfile)
-            values = set_json_string(title, notebook_id, body, img)
+            values = set_json_string(title, NOTEBOOK_ID, body, img)
 
-    response = requests.post(SERVER + "/notes" + TOKEN, data=values)
-    print(response)
-    print(response.text)
+    response = requests.post(ENDPOINT + "/notes" + TOKEN, data=values)
+    # print(response)
+    # print(response.text)
     if AUTOTAG:
         apply_tags(body, response.json().get("id"))
+    print(f"Placed into note into notebook {NOTEBOOK_ID}: {NOTEBOOK_NAME}")
+    return 0
 
 
 def watcher(path=None):
-    set_working_directory()
-    set_token()
     if path is None:
         path = str(Path.home())
-
     event_handler = MyHandler()
-    print("Monitoring directory {} for files".format(path))
+    print(f"Monitoring directory {path} for files")
     observer = Observer()
     observer.schedule(event_handler, path=path, recursive=False)
     observer.start()
 
     try:
         while True:
             time.sleep(1)
```

### Comparing `rest_uploader-1.5.0/rest_uploader.egg-info/PKG-INFO` & `rest_uploader-1.9.0/rest_uploader.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: rest-uploader
-Version: 1.5.0
+Version: 1.9.0
 Summary: REST API Uploader
 Home-page: https://github.com/kellerjustin/rest-uploader
 Author: Justin Keller
 Author-email: kellerjustin@protonmail.com
 License: MIT license
 Description: =============
         rest_uploader
@@ -115,14 +115,35 @@
         
         
         1.5.0 (2020-02-19)
         ------------------
         
         * Embarrassingly dumb bug fix for autotag argument
         
+        
+        1.7.0 (2020-05-11)
+        ------------------
+        
+        * Added command line options for server, port, destination notebook
+        * Added some error handling to quit when Joplin is closed or there
+          is no valid notebook detected
+        * Removed the settings.py file - everything handled via command line
+          switches
+        * More verbose command line notifications
+        * Not leaving temp file location setting to user, handling this by 
+          detecting OS on startup
+        
+        
+        1.9.0 (2020-05-12)
+        ------------------
+        
+        * Immediately realized closing application if Joplin isn't running is
+          a bad idea in the case of startup scripts, etc - fixed logic to wait
+        * Made use of the tempfile library which made life easier
+        
 Keywords: rest_uploader,joplin,rest-uploader
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2
```

### Comparing `rest_uploader-1.5.0/rest_uploader.egg-info/SOURCES.txt` & `rest_uploader-1.9.0/rest_uploader.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 docs/_build/html/_static/minus.png
 docs/_build/html/_static/plus.png
 rest_uploader/__init__.py
 rest_uploader/api_token.py
 rest_uploader/cli.py
 rest_uploader/img_process.py
 rest_uploader/rest_uploader.py
-rest_uploader/settings.py
 rest_uploader.egg-info/PKG-INFO
 rest_uploader.egg-info/SOURCES.txt
 rest_uploader.egg-info/dependency_links.txt
 rest_uploader.egg-info/entry_points.txt
 rest_uploader.egg-info/not-zip-safe
 rest_uploader.egg-info/requires.txt
 rest_uploader.egg-info/top_level.txt
```

### Comparing `rest_uploader-1.5.0/setup.py` & `rest_uploader-1.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 requirements = [
     "Click>=6.0",
     "watchdog",
     "requests",
     "pytesseract",
     "pdf2image",
     "PyPDF2",
-    "tabulate"
+    "tabulate",
 ]
 
 setup_requirements = []
 
 test_requirements = []
 
 setup(
@@ -50,10 +50,10 @@
     keywords=["rest_uploader", "joplin", "rest-uploader"],
     name="rest_uploader",
     packages=find_packages(include=["rest_uploader"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/kellerjustin/rest-uploader",
-    version='1.5.0',
+    version="1.9.0",
     zip_safe=False,
 )
```

### Comparing `rest_uploader-1.5.0/tests/test_rest_uploader.py` & `rest_uploader-1.9.0/tests/test_rest_uploader.py`

 * *Files identical despite different names*

