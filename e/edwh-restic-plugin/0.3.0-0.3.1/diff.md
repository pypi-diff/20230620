# Comparing `tmp/edwh_restic_plugin-0.3.0.tar.gz` & `tmp/edwh_restic_plugin-0.3.1.tar.gz`

## Comparing `edwh_restic_plugin-0.3.0.tar` & `edwh_restic_plugin-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     5167 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/CHANGELOG.md
--rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/examples/captain-hooks/backup_files.sh
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/examples/captain-hooks/backup_minecraft.py
--rwxr-xr-x   0        0        0      593 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/examples/captain-hooks/backup_stream.sh
--rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/examples/captain-hooks/backup_stream_sql.sh
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/examples/captain-hooks/restore_files.sh
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/examples/captain-hooks/restore_stream.sh
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/src/edwh_restic_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/src/edwh_restic_plugin/__init__.py
--rw-r--r--   0        0        0    30353 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/src/edwh_restic_plugin/tasks.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/README.md
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     5418 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/CHANGELOG.md
+-rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/examples/captain-hooks/backup_files.sh
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/examples/captain-hooks/backup_minecraft.py
+-rwxr-xr-x   0        0        0      593 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/examples/captain-hooks/backup_stream.sh
+-rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/examples/captain-hooks/backup_stream_sql.sh
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/examples/captain-hooks/restore_files.sh
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/examples/captain-hooks/restore_stream.sh
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/src/edwh_restic_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/src/edwh_restic_plugin/__init__.py
+-rw-r--r--   0        0        0    30323 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/src/edwh_restic_plugin/tasks.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/README.md
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 edwh_restic_plugin-0.3.1/PKG-INFO
```

### Comparing `edwh_restic_plugin-0.3.0/CHANGELOG.md` & `edwh_restic_plugin-0.3.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.3.1 (2023-06-20)
+### Fix
+* Fixed color coding in restic plugin. now doesn't only print in white but in set color of the cmd ([`80ad277`](https://github.com/educationwarehouse/edwh-restic-plugin/commit/80ad27717a89c9843b62d002e214493ad428c39c))
+
 ## v0.3.0 (2023-06-09)
 ### Feature
 * Edwh-restic-plugin now exist with the highest status code one of the given shell scripts gave it ([`281f600`](https://github.com/educationwarehouse/edwh-restic-plugin/commit/281f600082cba3853b1bc35efda93ea50ea8f3b5))
 
 ## v0.2.7 (2023-06-09)
 ### Fix
 * Made it now so it gets the result is captured even when throwing exception ([`fad076a`](https://github.com/educationwarehouse/edwh-restic-plugin/commit/fad076aab666925c2bb795a2705500215f7500c5))
```

### Comparing `edwh_restic_plugin-0.3.0/examples/captain-hooks/backup_minecraft.py` & `edwh_restic_plugin-0.3.1/examples/captain-hooks/backup_minecraft.py`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.3.0/examples/captain-hooks/backup_stream.sh` & `edwh_restic_plugin-0.3.1/examples/captain-hooks/backup_stream.sh`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.3.0/src/edwh_restic_plugin/tasks.py` & `edwh_restic_plugin-0.3.1/src/edwh_restic_plugin/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,17 +206,17 @@
                 hide=True
             )
 
         print("\n\nfile status codes:")
 
         for idx in range(len(file_codes)):
             if file_codes[idx] == 0:
-                print(files[idx], tag="success", tag_color="green", color='white')
+                print(files[idx], tag="success", tag_color="green")
             else:
-                print("in", files[idx], tag="failure", tag_color="red", color='white')
+                print("in", files[idx], tag="failure", tag_color="red")
 
         if worst_status_code := max(file_codes) > 0:
             exit(worst_status_code)
 
     def backup(self, c, verbose: bool, target: str, message: str):
         """
         Backs up the specified target.
```

### Comparing `edwh_restic_plugin-0.3.0/LICENSE.txt` & `edwh_restic_plugin-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.3.0/README.md` & `edwh_restic_plugin-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.3.0/pyproject.toml` & `edwh_restic_plugin-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_restic_plugin-0.3.0/PKG-INFO` & `edwh_restic_plugin-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-restic-plugin
-Version: 0.3.0
+Version: 0.3.1
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-restic-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-restic-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-restic-plugin
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

