# Comparing `tmp/djangoldp_component-1.0.7.tar.gz` & `tmp/djangoldp_component-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_component-1.0.7.tar", last modified: Thu Jun  1 15:42:55 2023, max compression
+gzip compressed data, was "dist/djangoldp_component-1.0.8.tar", last modified: Tue Jun 20 15:54:07 2023, max compression
```

## Comparing `djangoldp_component-1.0.7.tar` & `djangoldp_component-1.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 15:42:55.000000 djangoldp_component-1.0.7/
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-06-01 15:42:38.000000 djangoldp_component-1.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 15:42:55.000000 djangoldp_component-1.0.7/djangoldp_component.egg-info/
--rw-r--r--   0 root         (0) root         (0)      294 2023-06-01 15:42:55.000000 djangoldp_component-1.0.7/djangoldp_component.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 15:42:55.000000 djangoldp_component-1.0.7/djangoldp_component.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      599 2023-06-01 15:42:55.000000 djangoldp_component-1.0.7/djangoldp_component.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-01 15:42:55.000000 djangoldp_component-1.0.7/djangoldp_component.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 15:42:55.000000 djangoldp_component-1.0.7/djangoldp_component.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-06-01 15:42:38.000000 djangoldp_component-1.0.7/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-06-01 15:42:55.000000 djangoldp_component-1.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      294 2023-06-01 15:42:55.000000 djangoldp_component-1.0.7/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 15:42:55.000000 djangoldp_component-1.0.7/djangoldp_component/
--rw-rw-rw-   0 root         (0) root         (0)     9713 2023-06-01 15:42:38.000000 djangoldp_component-1.0.7/djangoldp_component/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1630 2023-06-01 15:42:38.000000 djangoldp_component-1.0.7/djangoldp_component/admin.py
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-06-01 15:42:53.000000 djangoldp_component-1.0.7/djangoldp_component/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-01 15:42:38.000000 djangoldp_component-1.0.7/djangoldp_component/apps.py
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-01 15:42:38.000000 djangoldp_component-1.0.7/djangoldp_component/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 15:42:55.000000 djangoldp_component-1.0.7/djangoldp_component/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    12897 2023-06-01 15:42:38.000000 djangoldp_component-1.0.7/djangoldp_component/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      517 2023-06-01 15:42:38.000000 djangoldp_component-1.0.7/djangoldp_component/migrations/0003_component_auto_menu.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 15:42:38.000000 djangoldp_component-1.0.7/djangoldp_component/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-06-01 15:42:38.000000 djangoldp_component-1.0.7/djangoldp_component/migrations/0002_delete_dependency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 15:54:07.000000 djangoldp_component-1.0.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-06-20 15:53:48.000000 djangoldp_component-1.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 15:54:07.000000 djangoldp_component-1.0.8/djangoldp_component.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      294 2023-06-20 15:54:07.000000 djangoldp_component-1.0.8/djangoldp_component.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 15:54:07.000000 djangoldp_component-1.0.8/djangoldp_component.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      599 2023-06-20 15:54:07.000000 djangoldp_component-1.0.8/djangoldp_component.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-20 15:54:07.000000 djangoldp_component-1.0.8/djangoldp_component.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 15:54:07.000000 djangoldp_component-1.0.8/djangoldp_component.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-06-20 15:53:48.000000 djangoldp_component-1.0.8/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-06-20 15:54:07.000000 djangoldp_component-1.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      294 2023-06-20 15:54:07.000000 djangoldp_component-1.0.8/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 15:54:07.000000 djangoldp_component-1.0.8/djangoldp_component/
+-rw-rw-rw-   0 root         (0) root         (0)     9713 2023-06-20 15:53:48.000000 djangoldp_component-1.0.8/djangoldp_component/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1630 2023-06-20 15:53:48.000000 djangoldp_component-1.0.8/djangoldp_component/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-06-20 15:54:05.000000 djangoldp_component-1.0.8/djangoldp_component/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-20 15:53:48.000000 djangoldp_component-1.0.8/djangoldp_component/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-20 15:53:48.000000 djangoldp_component-1.0.8/djangoldp_component/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 15:54:07.000000 djangoldp_component-1.0.8/djangoldp_component/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    12897 2023-06-20 15:53:48.000000 djangoldp_component-1.0.8/djangoldp_component/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      517 2023-06-20 15:53:48.000000 djangoldp_component-1.0.8/djangoldp_component/migrations/0003_component_auto_menu.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 15:53:48.000000 djangoldp_component-1.0.8/djangoldp_component/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-06-20 15:53:48.000000 djangoldp_component-1.0.8/djangoldp_component/migrations/0002_delete_dependency.py
```

### Comparing `djangoldp_component-1.0.7/README.md` & `djangoldp_component-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_component-1.0.7/djangoldp_component.egg-info/SOURCES.txt` & `djangoldp_component-1.0.8/djangoldp_component.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_component-1.0.7/setup.cfg` & `djangoldp_component-1.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangoldp_component-1.0.7/djangoldp_component/models.py` & `djangoldp_component-1.0.8/djangoldp_component/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp_component-1.0.7/djangoldp_component/admin.py` & `djangoldp_component-1.0.8/djangoldp_component/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_component-1.0.7/djangoldp_component/migrations/0001_initial.py` & `djangoldp_component-1.0.8/djangoldp_component/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_component-1.0.7/djangoldp_component/migrations/0003_component_auto_menu.py` & `djangoldp_component-1.0.8/djangoldp_component/migrations/0003_component_auto_menu.py`

 * *Files identical despite different names*

