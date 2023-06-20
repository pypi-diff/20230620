# Comparing `tmp/vsiew-2.3.1.tar.gz` & `tmp/vsiew-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsiew-2.3.1.tar", last modified: Tue Jun 20 15:37:15 2023, max compression
+gzip compressed data, was "vsiew-2.3.2.tar", last modified: Tue Jun 20 15:43:30 2023, max compression
```

## Comparing `vsiew-2.3.1.tar` & `vsiew-2.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:37:15.152172 vsiew-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-20 15:36:48.000000 vsiew-2.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-20 15:37:15.148172 vsiew-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-20 15:36:48.000000 vsiew-2.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:37:15.152172 vsiew-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-20 15:36:48.000000 vsiew-2.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:37:15.148172 vsiew-2.3.1/vsiew/
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-20 15:36:48.000000 vsiew-2.3.1/vsiew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-20 15:36:48.000000 vsiew-2.3.1/vsiew/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-20 15:36:48.000000 vsiew-2.3.1/vsiew/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-06-20 15:36:48.000000 vsiew-2.3.1/vsiew/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:37:15.148172 vsiew-2.3.1/vsiew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-20 15:37:15.000000 vsiew-2.3.1/vsiew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-20 15:37:15.000000 vsiew-2.3.1/vsiew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:37:15.000000 vsiew-2.3.1/vsiew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 15:37:15.000000 vsiew-2.3.1/vsiew.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-20 15:37:15.000000 vsiew-2.3.1/vsiew.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 15:37:15.000000 vsiew-2.3.1/vsiew.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:43:30.843994 vsiew-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-20 15:43:08.000000 vsiew-2.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-20 15:43:30.843994 vsiew-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-20 15:43:08.000000 vsiew-2.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:43:30.843994 vsiew-2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-20 15:43:08.000000 vsiew-2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:43:30.839994 vsiew-2.3.2/vsiew/
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-20 15:43:08.000000 vsiew-2.3.2/vsiew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-20 15:43:08.000000 vsiew-2.3.2/vsiew/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-20 15:43:08.000000 vsiew-2.3.2/vsiew/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-20 15:43:08.000000 vsiew-2.3.2/vsiew/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:43:30.843994 vsiew-2.3.2/vsiew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-20 15:43:30.000000 vsiew-2.3.2/vsiew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-20 15:43:30.000000 vsiew-2.3.2/vsiew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:43:30.000000 vsiew-2.3.2/vsiew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 15:43:30.000000 vsiew-2.3.2/vsiew.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-20 15:43:30.000000 vsiew-2.3.2/vsiew.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 15:43:30.000000 vsiew-2.3.2/vsiew.egg-info/top_level.txt
```

### Comparing `vsiew-2.3.1/LICENSE` & `vsiew-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vsiew-2.3.1/PKG-INFO` & `vsiew-2.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsiew
-Version: 2.3.1
+Version: 2.3.2
 Summary: VapourSynth packages from Irrational Encoding Wizardry
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
```

### Comparing `vsiew-2.3.1/setup.py` & `vsiew-2.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `vsiew-2.3.1/vsiew/__init__.py` & `vsiew-2.3.2/vsiew/__init__.py`

 * *Files identical despite different names*

### Comparing `vsiew-2.3.1/vsiew/init.py` & `vsiew-2.3.2/vsiew/init.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,18 +70,21 @@
         message_succ: str = default_message, message_err: str = default_message
     ) -> None:
         nonlocal color, message, err
         color = 31 if err else 32
         message = (message_err if err else message_succ).format(err=err)
 
     if action == 'update':
-        err = _get_install_call('vs-iew', True)
+        packages = list(_get_iew_packages())
+        for name, _ in reversed(packages):
+            _get_uninstall_call(name)
 
-        if err:
-            err = _get_install_call('vsiew', False)
+        for _, repo_name in packages:
+            if _get_install_call(repo_name, False):
+                err += 1
 
         _set_message(
             'Successfully updated IEW packages!',
             'There was an error updating IEW packages!'
         )
     elif action == 'update-git':
         packages = list(_get_iew_packages())
```

### Comparing `vsiew-2.3.1/vsiew.egg-info/PKG-INFO` & `vsiew-2.3.2/vsiew.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsiew
-Version: 2.3.1
+Version: 2.3.2
 Summary: VapourSynth packages from Irrational Encoding Wizardry
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
```

