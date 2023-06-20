# Comparing `tmp/tcompress-0.0.3.tar.gz` & `tmp/tcompress-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcompress-0.0.3.tar", last modified: Tue Jun 20 06:45:17 2023, max compression
+gzip compressed data, was "tcompress-0.0.4.tar", last modified: Tue Jun 20 06:51:06 2023, max compression
```

## Comparing `tcompress-0.0.3.tar` & `tcompress-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:45:17.513166 tcompress-0.0.3/
--rw-r--r--   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:06:54.000000 tcompress-0.0.3/LICENSE
--rw-r--r--   0 talalzeini   (501) staff       (20)      499 2023-06-20 06:45:17.513250 tcompress-0.0.3/PKG-INFO
--rw-r--r--   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:08:04.000000 tcompress-0.0.3/README.md
--rw-r--r--   0 talalzeini   (501) staff       (20)      103 2023-06-20 06:09:35.000000 tcompress-0.0.3/pyproject.toml
--rw-r--r--   0 talalzeini   (501) staff       (20)      650 2023-06-20 06:45:17.513562 tcompress-0.0.3/setup.cfg
-drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:45:17.510266 tcompress-0.0.3/src/
-drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:45:17.511218 tcompress-0.0.3/src/tcompress/
--rw-r--r--   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:08:48.000000 tcompress-0.0.3/src/tcompress/__init__.py
-drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:45:17.513004 tcompress-0.0.3/src/tcompress/functions/
--rw-rw-r--   0 talalzeini   (501) staff       (20)     1924 2023-06-20 06:13:44.000000 tcompress-0.0.3/src/tcompress/functions/image.py
--rw-rw-r--   0 talalzeini   (501) staff       (20)      982 2023-06-20 06:13:44.000000 tcompress-0.0.3/src/tcompress/functions/main.py
--rw-rw-r--   0 talalzeini   (501) staff       (20)     1504 2023-06-20 06:13:44.000000 tcompress-0.0.3/src/tcompress/functions/manage.py
--rw-rw-r--   0 talalzeini   (501) staff       (20)      498 2023-06-20 06:13:44.000000 tcompress-0.0.3/src/tcompress/functions/random.py
--rw-rw-r--   0 talalzeini   (501) staff       (20)      447 2023-06-20 06:13:44.000000 tcompress-0.0.3/src/tcompress/functions/time.py
--rw-rw-r--   0 talalzeini   (501) staff       (20)      500 2023-06-20 06:13:44.000000 tcompress-0.0.3/src/tcompress/installer.py
-drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:45:17.511883 tcompress-0.0.3/src/tcompress.egg-info/
--rw-r--r--   0 talalzeini   (501) staff       (20)      499 2023-06-20 06:45:17.000000 tcompress-0.0.3/src/tcompress.egg-info/PKG-INFO
--rw-r--r--   0 talalzeini   (501) staff       (20)      408 2023-06-20 06:45:17.000000 tcompress-0.0.3/src/tcompress.egg-info/SOURCES.txt
--rw-r--r--   0 talalzeini   (501) staff       (20)        1 2023-06-20 06:45:17.000000 tcompress-0.0.3/src/tcompress.egg-info/dependency_links.txt
--rw-r--r--   0 talalzeini   (501) staff       (20)       10 2023-06-20 06:45:17.000000 tcompress-0.0.3/src/tcompress.egg-info/top_level.txt
+drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:51:06.497733 tcompress-0.0.4/
+-rw-r--r--   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:06:54.000000 tcompress-0.0.4/LICENSE
+-rw-r--r--   0 talalzeini   (501) staff       (20)      499 2023-06-20 06:51:06.497809 tcompress-0.0.4/PKG-INFO
+-rw-r--r--   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:08:04.000000 tcompress-0.0.4/README.md
+-rw-r--r--   0 talalzeini   (501) staff       (20)      103 2023-06-20 06:09:35.000000 tcompress-0.0.4/pyproject.toml
+-rw-r--r--   0 talalzeini   (501) staff       (20)      650 2023-06-20 06:51:06.498118 tcompress-0.0.4/setup.cfg
+drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:51:06.494175 tcompress-0.0.4/src/
+drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:51:06.495044 tcompress-0.0.4/src/tcompress/
+-rw-r--r--   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:08:48.000000 tcompress-0.0.4/src/tcompress/__init__.py
+drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:51:06.497535 tcompress-0.0.4/src/tcompress/functions/
+-rw-rw-r--   0 talalzeini   (501) staff       (20)     1924 2023-06-20 06:13:44.000000 tcompress-0.0.4/src/tcompress/functions/image.py
+-rw-rw-r--   0 talalzeini   (501) staff       (20)      982 2023-06-20 06:13:44.000000 tcompress-0.0.4/src/tcompress/functions/main.py
+-rw-rw-r--   0 talalzeini   (501) staff       (20)     1504 2023-06-20 06:13:44.000000 tcompress-0.0.4/src/tcompress/functions/manage.py
+-rw-rw-r--   0 talalzeini   (501) staff       (20)      498 2023-06-20 06:13:44.000000 tcompress-0.0.4/src/tcompress/functions/random.py
+-rw-rw-r--   0 talalzeini   (501) staff       (20)      447 2023-06-20 06:13:44.000000 tcompress-0.0.4/src/tcompress/functions/time.py
+-rw-rw-r--   0 talalzeini   (501) staff       (20)      500 2023-06-20 06:13:44.000000 tcompress-0.0.4/src/tcompress/installer.py
+drwxr-xr-x   0 talalzeini   (501) staff       (20)        0 2023-06-20 06:51:06.496261 tcompress-0.0.4/src/tcompress.egg-info/
+-rw-r--r--   0 talalzeini   (501) staff       (20)      499 2023-06-20 06:51:06.000000 tcompress-0.0.4/src/tcompress.egg-info/PKG-INFO
+-rw-r--r--   0 talalzeini   (501) staff       (20)      408 2023-06-20 06:51:06.000000 tcompress-0.0.4/src/tcompress.egg-info/SOURCES.txt
+-rw-r--r--   0 talalzeini   (501) staff       (20)        1 2023-06-20 06:51:06.000000 tcompress-0.0.4/src/tcompress.egg-info/dependency_links.txt
+-rw-r--r--   0 talalzeini   (501) staff       (20)       10 2023-06-20 06:51:06.000000 tcompress-0.0.4/src/tcompress.egg-info/top_level.txt
```

### Comparing `tcompress-0.0.3/setup.cfg` & `tcompress-0.0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tcompress
-version = 0.0.3
+version = 0.0.4
 author = Talal El Zeini
 author_email = talalelzeini@gmail.com
 description = A small example package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/talalzeini/compress
 project_urls =
```

### Comparing `tcompress-0.0.3/src/tcompress/functions/image.py` & `tcompress-0.0.4/src/tcompress/functions/image.py`

 * *Files identical despite different names*

### Comparing `tcompress-0.0.3/src/tcompress/functions/main.py` & `tcompress-0.0.4/src/tcompress/functions/main.py`

 * *Files identical despite different names*

### Comparing `tcompress-0.0.3/src/tcompress/functions/manage.py` & `tcompress-0.0.4/src/tcompress/functions/manage.py`

 * *Files identical despite different names*

