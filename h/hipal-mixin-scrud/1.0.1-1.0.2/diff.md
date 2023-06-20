# Comparing `tmp/hipal_mixin_scrud-1.0.1.tar.gz` & `tmp/hipal_mixin_scrud-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hipal_mixin_scrud-1.0.1.tar", last modified: Tue Jun 20 21:29:35 2023, max compression
+gzip compressed data, was "dist\hipal_mixin_scrud-1.0.2.tar", last modified: Tue Jun 20 21:31:49 2023, max compression
```

## Comparing `hipal_mixin_scrud-1.0.1.tar` & `hipal_mixin_scrud-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 21:29:35.123133 hipal_mixin_scrud-1.0.1/
--rw-rw-rw-   0        0        0      316 2023-06-20 21:29:35.123133 hipal_mixin_scrud-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-20 21:29:35.083132 hipal_mixin_scrud-1.0.1/hipal_mixin_scrud/
--rw-rw-rw-   0        0        0        0 2023-06-20 21:27:42.000000 hipal_mixin_scrud-1.0.1/hipal_mixin_scrud/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 21:29:35.110131 hipal_mixin_scrud-1.0.1/hipal_mixin_scrud/crud/
--rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.1/hipal_mixin_scrud/crud/__init__.py
--rw-rw-rw-   0        0        0     5725 2023-06-20 21:25:12.000000 hipal_mixin_scrud-1.0.1/hipal_mixin_scrud/crud/generator.py
--rw-rw-rw-   0        0        0     3112 2023-06-20 21:25:07.000000 hipal_mixin_scrud-1.0.1/hipal_mixin_scrud/crud/mixin_list.py
-drwxrwxrwx   0        0        0        0 2023-06-20 21:29:35.115132 hipal_mixin_scrud-1.0.1/hipal_mixin_scrud/enums/
--rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.1/hipal_mixin_scrud/enums/__init__.py
--rw-rw-rw-   0        0        0      165 2023-06-20 18:14:02.000000 hipal_mixin_scrud-1.0.1/hipal_mixin_scrud/enums/operators.py
--rw-rw-rw-   0        0        0       82 2023-06-20 17:19:07.000000 hipal_mixin_scrud-1.0.1/hipal_mixin_scrud/enums/sorts.py
--rw-rw-rw-   0        0        0     3432 2023-06-20 21:25:59.000000 hipal_mixin_scrud-1.0.1/hipal_mixin_scrud/mixin.py
-drwxrwxrwx   0        0        0        0 2023-06-20 21:29:35.121133 hipal_mixin_scrud-1.0.1/hipal_mixin_scrud/schemas/
--rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.1/hipal_mixin_scrud/schemas/__init__.py
--rw-rw-rw-   0        0        0      396 2023-06-20 21:24:58.000000 hipal_mixin_scrud-1.0.1/hipal_mixin_scrud/schemas/paginate_params.py
--rw-rw-rw-   0        0        0      364 2023-06-15 00:38:39.000000 hipal_mixin_scrud-1.0.1/hipal_mixin_scrud/schemas/pagination_base.py
-drwxrwxrwx   0        0        0        0 2023-06-20 21:29:35.105133 hipal_mixin_scrud-1.0.1/hipal_mixin_scrud.egg-info/
--rw-rw-rw-   0        0        0      316 2023-06-20 21:29:34.000000 hipal_mixin_scrud-1.0.1/hipal_mixin_scrud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-06-20 21:29:35.000000 hipal_mixin_scrud-1.0.1/hipal_mixin_scrud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 21:29:34.000000 hipal_mixin_scrud-1.0.1/hipal_mixin_scrud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-20 21:29:34.000000 hipal_mixin_scrud-1.0.1/hipal_mixin_scrud.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-20 21:29:34.000000 hipal_mixin_scrud-1.0.1/hipal_mixin_scrud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 21:29:35.125132 hipal_mixin_scrud-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      483 2023-06-20 21:27:54.000000 hipal_mixin_scrud-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 21:31:49.935236 hipal_mixin_scrud-1.0.2/
+-rw-rw-rw-   0        0        0      316 2023-06-20 21:31:49.935236 hipal_mixin_scrud-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-20 21:31:49.903237 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/
+-rw-rw-rw-   0        0        0        0 2023-06-20 21:27:42.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 21:31:49.924238 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/crud/
+-rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/crud/__init__.py
+-rw-rw-rw-   0        0        0     5725 2023-06-20 21:25:12.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/crud/generator.py
+-rw-rw-rw-   0        0        0     3112 2023-06-20 21:25:07.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/crud/mixin_list.py
+drwxrwxrwx   0        0        0        0 2023-06-20 21:31:49.929238 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/enums/
+-rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/enums/__init__.py
+-rw-rw-rw-   0        0        0      165 2023-06-20 18:14:02.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/enums/operators.py
+-rw-rw-rw-   0        0        0       82 2023-06-20 17:19:07.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/enums/sorts.py
+-rw-rw-rw-   0        0        0     3432 2023-06-20 21:25:59.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/mixin.py
+drwxrwxrwx   0        0        0        0 2023-06-20 21:31:49.933237 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/schemas/
+-rw-rw-rw-   0        0        0        0 2023-06-20 21:28:13.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/schemas/__init__.py
+-rw-rw-rw-   0        0        0      396 2023-06-20 21:24:58.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/schemas/paginate_params.py
+-rw-rw-rw-   0        0        0      364 2023-06-15 00:38:39.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/schemas/pagination_base.py
+drwxrwxrwx   0        0        0        0 2023-06-20 21:31:49.919237 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud.egg-info/
+-rw-rw-rw-   0        0        0      316 2023-06-20 21:31:49.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2023-06-20 21:31:49.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 21:31:49.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-20 21:31:49.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-20 21:31:49.000000 hipal_mixin_scrud-1.0.2/hipal_mixin_scrud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 21:31:49.937237 hipal_mixin_scrud-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      483 2023-06-20 21:31:45.000000 hipal_mixin_scrud-1.0.2/setup.py
```

### Comparing `hipal_mixin_scrud-1.0.1/hipal_mixin_scrud/crud/generator.py` & `hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/crud/generator.py`

 * *Files identical despite different names*

### Comparing `hipal_mixin_scrud-1.0.1/hipal_mixin_scrud/crud/mixin_list.py` & `hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/crud/mixin_list.py`

 * *Files identical despite different names*

### Comparing `hipal_mixin_scrud-1.0.1/hipal_mixin_scrud/mixin.py` & `hipal_mixin_scrud-1.0.2/hipal_mixin_scrud/mixin.py`

 * *Files identical despite different names*

### Comparing `hipal_mixin_scrud-1.0.1/hipal_mixin_scrud.egg-info/SOURCES.txt` & `hipal_mixin_scrud-1.0.2/hipal_mixin_scrud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

