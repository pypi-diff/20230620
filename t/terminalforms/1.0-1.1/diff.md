# Comparing `tmp/terminalforms-1.0.tar.gz` & `tmp/terminalforms-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminalforms-1.0.tar", last modified: Tue Jun 20 20:18:18 2023, max compression
+gzip compressed data, was "terminalforms-1.1.tar", last modified: Tue Jun 20 20:22:05 2023, max compression
```

## Comparing `terminalforms-1.0.tar` & `terminalforms-1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 20:18:18.410320 terminalforms-1.0/
--rw-rw-rw-   0        0        0     1083 2023-06-19 23:44:07.000000 terminalforms-1.0/LICENSE
--rw-rw-rw-   0        0        0     3092 2023-06-20 20:18:18.412323 terminalforms-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2777 2023-06-20 20:14:17.000000 terminalforms-1.0/README.md
--rw-rw-rw-   0        0        0      133 2023-06-20 20:08:40.000000 terminalforms-1.0/pyproject.toml
--rw-rw-rw-   0        0        0      481 2023-06-20 20:18:18.430322 terminalforms-1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-20 20:18:18.295320 terminalforms-1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-20 20:18:18.337323 terminalforms-1.0/src/terminalforms/
--rw-rw-rw-   0        0        0        0 2023-06-19 23:42:06.000000 terminalforms-1.0/src/terminalforms/__init__.py
--rw-rw-rw-   0        0        0     3824 2023-06-20 20:13:30.000000 terminalforms-1.0/src/terminalforms/forms.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:18:18.407320 terminalforms-1.0/src/terminalforms.egg-info/
--rw-rw-rw-   0        0        0     3092 2023-06-20 20:18:18.000000 terminalforms-1.0/src/terminalforms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-06-20 20:18:18.000000 terminalforms-1.0/src/terminalforms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 20:18:18.000000 terminalforms-1.0/src/terminalforms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-20 20:18:18.000000 terminalforms-1.0/src/terminalforms.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-20 20:18:18.000000 terminalforms-1.0/src/terminalforms.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 20:22:05.415919 terminalforms-1.1/
+-rw-rw-rw-   0        0        0     1083 2023-06-19 23:44:07.000000 terminalforms-1.1/LICENSE
+-rw-rw-rw-   0        0        0     3092 2023-06-20 20:22:05.416917 terminalforms-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2777 2023-06-20 20:14:17.000000 terminalforms-1.1/README.md
+-rw-rw-rw-   0        0        0      133 2023-06-20 20:08:40.000000 terminalforms-1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      481 2023-06-20 20:22:05.422922 terminalforms-1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-20 20:22:05.314920 terminalforms-1.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-20 20:22:05.366924 terminalforms-1.1/src/terminalforms/
+-rw-rw-rw-   0        0        0       20 2023-06-20 20:21:12.000000 terminalforms-1.1/src/terminalforms/__init__.py
+-rw-rw-rw-   0        0        0     3824 2023-06-20 20:13:30.000000 terminalforms-1.1/src/terminalforms/forms.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:22:05.412915 terminalforms-1.1/src/terminalforms.egg-info/
+-rw-rw-rw-   0        0        0     3092 2023-06-20 20:22:05.000000 terminalforms-1.1/src/terminalforms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-06-20 20:22:05.000000 terminalforms-1.1/src/terminalforms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 20:22:05.000000 terminalforms-1.1/src/terminalforms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-20 20:22:05.000000 terminalforms-1.1/src/terminalforms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-20 20:22:05.000000 terminalforms-1.1/src/terminalforms.egg-info/top_level.txt
```

### Comparing `terminalforms-1.0/LICENSE` & `terminalforms-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `terminalforms-1.0/PKG-INFO` & `terminalforms-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminalforms
-Version: 1.0
+Version: 1.1
 Summary: Add forms to your terminal applications
 Home-page: https://github.com/W1L7dev/TerminalForms
 Author: W1L7dev
 Author-email: w1l7dev@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `terminalforms-1.0/README.md` & `terminalforms-1.1/README.md`

 * *Files identical despite different names*

### Comparing `terminalforms-1.0/src/terminalforms/forms.py` & `terminalforms-1.1/src/terminalforms/forms.py`

 * *Files identical despite different names*

### Comparing `terminalforms-1.0/src/terminalforms.egg-info/PKG-INFO` & `terminalforms-1.1/src/terminalforms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminalforms
-Version: 1.0
+Version: 1.1
 Summary: Add forms to your terminal applications
 Home-page: https://github.com/W1L7dev/TerminalForms
 Author: W1L7dev
 Author-email: w1l7dev@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

