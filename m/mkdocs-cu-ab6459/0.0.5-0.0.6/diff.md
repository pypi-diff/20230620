# Comparing `tmp/mkdocs_cu_ab6459-0.0.5.tar.gz` & `tmp/mkdocs_cu_ab6459-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_cu_ab6459-0.0.5.tar", last modified: Tue Jun 20 09:51:48 2023, max compression
+gzip compressed data, was "mkdocs_cu_ab6459-0.0.6.tar", last modified: Tue Jun 20 09:54:33 2023, max compression
```

## Comparing `mkdocs_cu_ab6459-0.0.5.tar` & `mkdocs_cu_ab6459-0.0.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 09:51:48.661884 mkdocs_cu_ab6459-0.0.5/
--rw-rw-rw-   0        0        0      177 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      512 2023-06-20 09:51:48.661884 mkdocs_cu_ab6459-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       76 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 09:51:48.628129 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/
--rw-rw-rw-   0        0        0        0 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 09:51:48.643754 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/
--rw-rw-rw-   0        0        0    74437 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap-grid.css
--rw-rw-rw-   0        0        0    51824 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap-grid.min.css
--rw-rw-rw-   0        0        0    74510 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap-grid.rtl.css
--rw-rw-rw-   0        0        0    51899 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap-grid.rtl.min.css
--rw-rw-rw-   0        0        0    12525 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap-reboot.css
--rw-rw-rw-   0        0        0    10015 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap-reboot.min.css
--rw-rw-rw-   0        0        0    12515 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap-reboot.rtl.css
--rw-rw-rw-   0        0        0    10087 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap-reboot.rtl.min.css
--rw-rw-rw-   0        0        0   113076 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap-utilities.css
--rw-rw-rw-   0        0        0    85193 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap-utilities.min.css
--rw-rw-rw-   0        0        0   112935 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap-utilities.rtl.css
--rw-rw-rw-   0        0        0    85122 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap-utilities.rtl.min.css
--rw-rw-rw-   0        0        0   292882 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap.css
--rw-rw-rw-   0        0        0   232919 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap.min.css
--rw-rw-rw-   0        0        0   292425 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap.rtl.css
--rw-rw-rw-   0        0        0   233026 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap.rtl.min.css
--rw-rw-rw-   0        0        0     8148 2023-06-20 09:50:40.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/custom.css
--rw-rw-rw-   0        0        0     2170 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/diagram.css
--rw-rw-rw-   0        0        0    11870 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/prism.css
-drwxrwxrwx   0        0        0        0 2023-06-20 09:51:48.659379 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/images/
--rw-rw-rw-   0        0        0     7231 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/images/logo_dark.png
--rw-rw-rw-   0        0        0     7592 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/images/logo_light.png
-drwxrwxrwx   0        0        0        0 2023-06-20 09:51:48.661884 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/js/
--rw-rw-rw-   0        0        0   213731 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/js/bootstrap.bundle.js
--rw-rw-rw-   0        0        0    80427 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0   139896 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/js/bootstrap.esm.js
--rw-rw-rw-   0        0        0    73920 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/js/bootstrap.esm.min.js
--rw-rw-rw-   0        0        0   149493 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/js/bootstrap.js
--rw-rw-rw-   0        0        0    60354 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/js/bootstrap.min.js
--rw-rw-rw-   0        0        0     1197 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/js/darkmode.js
--rw-rw-rw-   0        0        0    42192 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/js/prism.js
--rw-rw-rw-   0        0        0    23168 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/js/simple-diagram.js
--rw-rw-rw-   0        0        0     6218 2023-06-20 09:45:37.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/main.html
--rw-rw-rw-   0        0        0       26 2023-06-20 09:45:32.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/mkdocs_theme.yml
-drwxrwxrwx   0        0        0        0 2023-06-20 09:51:48.643754 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459.egg-info/
--rw-rw-rw-   0        0        0      512 2023-06-20 09:51:48.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1617 2023-06-20 09:51:48.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 09:51:48.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-20 09:51:48.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-19 11:15:41.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-06-20 09:51:48.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-20 09:51:48.000000 mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 09:51:48.661884 mkdocs_cu_ab6459-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      884 2023-06-20 09:51:23.000000 mkdocs_cu_ab6459-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 09:54:33.925325 mkdocs_cu_ab6459-0.0.6/
+-rw-rw-rw-   0        0        0      177 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      512 2023-06-20 09:54:33.925325 mkdocs_cu_ab6459-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       76 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 09:54:33.893692 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/
+-rw-rw-rw-   0        0        0        0 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 09:54:33.919321 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/
+-rw-rw-rw-   0        0        0    74437 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap-grid.css
+-rw-rw-rw-   0        0        0    51824 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap-grid.min.css
+-rw-rw-rw-   0        0        0    74510 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap-grid.rtl.css
+-rw-rw-rw-   0        0        0    51899 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap-grid.rtl.min.css
+-rw-rw-rw-   0        0        0    12525 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap-reboot.css
+-rw-rw-rw-   0        0        0    10015 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap-reboot.min.css
+-rw-rw-rw-   0        0        0    12515 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap-reboot.rtl.css
+-rw-rw-rw-   0        0        0    10087 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap-reboot.rtl.min.css
+-rw-rw-rw-   0        0        0   113076 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap-utilities.css
+-rw-rw-rw-   0        0        0    85193 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap-utilities.min.css
+-rw-rw-rw-   0        0        0   112935 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap-utilities.rtl.css
+-rw-rw-rw-   0        0        0    85122 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap-utilities.rtl.min.css
+-rw-rw-rw-   0        0        0   292882 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap.css
+-rw-rw-rw-   0        0        0   232919 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap.min.css
+-rw-rw-rw-   0        0        0   292425 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap.rtl.css
+-rw-rw-rw-   0        0        0   233026 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap.rtl.min.css
+-rw-rw-rw-   0        0        0     8148 2023-06-20 09:50:40.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/custom.css
+-rw-rw-rw-   0        0        0     4013 2023-06-20 09:53:59.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/diagram.css
+-rw-rw-rw-   0        0        0    11870 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/prism.css
+drwxrwxrwx   0        0        0        0 2023-06-20 09:54:33.925325 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/images/
+-rw-rw-rw-   0        0        0     7231 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/images/logo_dark.png
+-rw-rw-rw-   0        0        0     7592 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/images/logo_light.png
+drwxrwxrwx   0        0        0        0 2023-06-20 09:54:33.925325 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/js/
+-rw-rw-rw-   0        0        0   213731 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/js/bootstrap.bundle.js
+-rw-rw-rw-   0        0        0    80427 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0   139896 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/js/bootstrap.esm.js
+-rw-rw-rw-   0        0        0    73920 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/js/bootstrap.esm.min.js
+-rw-rw-rw-   0        0        0   149493 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/js/bootstrap.js
+-rw-rw-rw-   0        0        0    60354 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0     1197 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/js/darkmode.js
+-rw-rw-rw-   0        0        0    42192 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/js/prism.js
+-rw-rw-rw-   0        0        0    23168 2023-06-19 11:13:25.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/js/simple-diagram.js
+-rw-rw-rw-   0        0        0     6218 2023-06-20 09:45:37.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/main.html
+-rw-rw-rw-   0        0        0       26 2023-06-20 09:45:32.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/mkdocs_theme.yml
+drwxrwxrwx   0        0        0        0 2023-06-20 09:54:33.909317 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459.egg-info/
+-rw-rw-rw-   0        0        0      512 2023-06-20 09:54:33.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1617 2023-06-20 09:54:33.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 09:54:33.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-20 09:54:33.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-19 11:15:41.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-06-20 09:54:33.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-20 09:54:33.000000 mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 09:54:33.925325 mkdocs_cu_ab6459-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      884 2023-06-20 09:54:17.000000 mkdocs_cu_ab6459-0.0.6/setup.py
```

### Comparing `mkdocs_cu_ab6459-0.0.5/PKG-INFO` & `mkdocs_cu_ab6459-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs_cu_ab6459
-Version: 0.0.5
+Version: 0.0.6
 Summary: Improved and extended version of the Windmill theme
 Home-page: https://github.coventry.ac.uk/ab6459/mkdocs_cu_ab6459
 Author: Ian Cornelius
 Author-email: ab6459@coventry.ac.uk
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Documentation
```

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap-grid.css` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap-grid.min.css` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap-grid.rtl.css` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap-grid.rtl.min.css` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap-reboot.css` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap-reboot.min.css` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap-reboot.rtl.css` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap-reboot.rtl.min.css` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap-utilities.css` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap-utilities.min.css` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap-utilities.rtl.css` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap-utilities.rtl.min.css` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap.css` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap.min.css` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap.rtl.css` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/bootstrap.rtl.min.css` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/custom.css` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/custom.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/css/prism.css` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/css/prism.css`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/images/logo_dark.png` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/images/logo_dark.png`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/images/logo_light.png` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/images/logo_light.png`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/js/bootstrap.bundle.js` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/js/bootstrap.bundle.min.js` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/js/bootstrap.esm.js` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/js/bootstrap.esm.min.js` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/js/bootstrap.js` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/js/bootstrap.min.js` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/js/darkmode.js` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/js/darkmode.js`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/js/prism.js` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/js/prism.js`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/js/simple-diagram.js` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/js/simple-diagram.js`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459/main.html` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459/main.html`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459.egg-info/PKG-INFO` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-cu-ab6459
-Version: 0.0.5
+Version: 0.0.6
 Summary: Improved and extended version of the Windmill theme
 Home-page: https://github.coventry.ac.uk/ab6459/mkdocs_cu_ab6459
 Author: Ian Cornelius
 Author-email: ab6459@coventry.ac.uk
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Documentation
```

### Comparing `mkdocs_cu_ab6459-0.0.5/mkdocs_cu_ab6459.egg-info/SOURCES.txt` & `mkdocs_cu_ab6459-0.0.6/mkdocs_cu_ab6459.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs_cu_ab6459-0.0.5/setup.py` & `mkdocs_cu_ab6459-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_desc = fh.read()
 
 setup(
     name="mkdocs_cu_ab6459",
-    version="0.0.5",
+    version="0.0.6",
     url='https://github.coventry.ac.uk/ab6459/mkdocs_cu_ab6459',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Topic :: Documentation',
         'Topic :: Text Processing',
     ],
     install_requires=[
```

